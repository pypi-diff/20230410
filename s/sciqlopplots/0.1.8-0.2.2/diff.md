# Comparing `tmp/sciqlopplots-0.1.8.tar.gz` & `tmp/sciqlopplots-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciqlopplots-0.1.8.tar", last modified: Thu Mar 23 12:17:03 2023, max compression
+gzip compressed data, was "sciqlopplots-0.2.2.tar", last modified: Mon Apr 10 17:05:07 2023, max compression
```

## Comparing `sciqlopplots-0.1.8.tar` & `sciqlopplots-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,49 @@
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/.clang-format
--rw-r--r--   0        0        0     2077 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/.github/workflows/pythonpublish-linux.yml
--rw-r--r--   0        0        0     1779 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/.github/workflows/pythonpublish-osx.yml
--rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/.github/workflows/pythonpublish-win.yml
--rw-r--r--   0        0        0      207 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/.gitignore
--rw-r--r--   0        0        0     1552 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/COPYING
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/README.md
--rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/SciQLopPlots/__init__.py
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build
--rw-r--r--   0        0        0     2115 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/SciQLopPlots/bindings/_QCustomPlot.hpp
--rw-r--r--   0        0        0      369 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/SciQLopPlots/bindings/bindings.h
--rw-r--r--   0        0        0    16181 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/SciQLopPlots/bindings/bindings.xml
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/SciQLopPlots/bindings/helper_scripts/rpath-helper.py
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py
--rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py
--rwxr-xr-x   0        0        0     2052 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/SciQLopPlots/bindings/helper_scripts/src_list.py
--rw-r--r--   0        0        0     1716 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/SciQLopPlots/bindings/snippets.cpp
--rw-r--r--   0        0        0     4236 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/SciQLopPlots/meson.build
--rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/include/SciQLopPlots/SciQLopColorMap.hpp
--rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/include/SciQLopPlots/SciQLopGraph.hpp
--rw-r--r--   0        0        0     5734 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/include/SciQLopPlots/numpy_wrappers.hpp
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/meson.build
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/meson_options.txt
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/pyproject.toml
--rwxr-xr-x   0        0        0    35147 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/qcustomplot-source/GPL.txt
--rwxr-xr-x   0        0        0    54691 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/qcustomplot-source/changelog.txt
--rw-r--r--   0        0        0  1307498 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/qcustomplot-source/qcustomplot.cpp
--rw-r--r--   0        0        0   310085 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/qcustomplot-source/qcustomplot.h
--rw-r--r--   0        0        0      296 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/setup.cfg
--rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/src/SciQLopColorMap.cpp
--rw-r--r--   0        0        0     5982 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/src/SciQLopGraph.cpp
--rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/src/numpy_wrappers.cpp
--rw-r--r--   0        0        0       70 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/subprojects/cpp_utils.wrap
--rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/subprojects/hedley.wrap
--rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/tests/manual-tests/QCP_Examples/plots/main.py
--rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/tests/manual-tests/SciQLopColorMap/main.py
--rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/tests/manual-tests/SciQLopGraph/main.py
--rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/tests/manual-tests/StackedGraphs/main.py
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/tests/manual-tests/meson.build
--rw-r--r--   0        0        0       23 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/tests/meson.build
--rw-r--r--   0        0        0     3120 1970-01-01 00:00:00.000000 sciqlopplots-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/.clang-format
+-rw-r--r--   0        0        0     2077 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/.github/workflows/pythonpublish-linux.yml
+-rw-r--r--   0        0        0     1779 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/.github/workflows/pythonpublish-osx.yml
+-rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/.github/workflows/pythonpublish-win.yml
+-rw-r--r--   0        0        0      207 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1552 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/COPYING
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/README.md
+-rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/__init__.py
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/_QCustomPlot.hpp
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/bindings.h
+-rw-r--r--   0        0        0    16781 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/bindings.xml
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/rpath-helper.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py
+-rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py
+-rwxr-xr-x   0        0        0     2052 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/src_list.py
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/snippets.cpp
+-rw-r--r--   0        0        0     4717 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/meson.build
+-rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopColorMap.hpp
+-rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopGraph.hpp
+-rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopPlot.hpp
+-rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopPlotItem.hpp
+-rw-r--r--   0        0        0     8901 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopVerticalSpan.hpp
+-rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/include/SciQLopPlots/constants.hpp
+-rw-r--r--   0        0        0     5734 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/include/SciQLopPlots/numpy_wrappers.hpp
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/meson.build
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/meson_options.txt
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/pyproject.toml
+-rwxr-xr-x   0        0        0    35147 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/qcustomplot-source/GPL.txt
+-rwxr-xr-x   0        0        0    54691 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/qcustomplot-source/changelog.txt
+-rw-r--r--   0        0        0  1307498 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/qcustomplot-source/qcustomplot.cpp
+-rw-r--r--   0        0        0   310085 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/qcustomplot-source/qcustomplot.h
+-rw-r--r--   0        0        0      296 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/setup.cfg
+-rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/src/SciQLopColorMap.cpp
+-rw-r--r--   0        0        0     5982 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/src/SciQLopGraph.cpp
+-rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/src/SciQLopPlot.cpp
+-rw-r--r--   0        0        0     1172 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/src/SciQLopPlotItem.cpp
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/src/SciQLopVerticalSpan.cpp
+-rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/src/numpy_wrappers.cpp
+-rw-r--r--   0        0        0       70 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/subprojects/cpp_utils.wrap
+-rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/subprojects/hedley.wrap
+-rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/tests/manual-tests/QCP_Examples/plots/main.py
+-rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/tests/manual-tests/SciQLopColorMap/main.py
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/tests/manual-tests/SciQLopGraph/main.py
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/tests/manual-tests/SciQLopVerticalSpan/main.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/tests/manual-tests/StackedGraphs/main.py
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/tests/manual-tests/meson.build
+-rw-r--r--   0        0        0       23 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/tests/meson.build
+-rw-r--r--   0        0        0     3120 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/PKG-INFO
```

### Comparing `sciqlopplots-0.1.8/.clang-format` & `sciqlopplots-0.2.2/.clang-format`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/.github/workflows/pythonpublish-linux.yml` & `sciqlopplots-0.2.2/.github/workflows/pythonpublish-linux.yml`

 * *Files 7% similar despite different names*

```diff
@@ -14,30 +14,30 @@
       fail-fast: false
       matrix:
         python-version: ['cp38-cp38', 'cp39-cp39', 'cp310-cp310', 'cp311-cp311']
     steps:
       - name: add Python and qt dir to path
         run: |
             echo "/opt/python/${{ matrix.python-version }}/bin" >> $GITHUB_PATH
-            echo "/Qt/6.4.2/gcc_64/bin" >> $GITHUB_PATH
+            echo "/Qt/6.5.0/gcc_64/bin" >> $GITHUB_PATH
       - uses: actions/checkout@v3
         with:
           submodules: true
       - name: Build for Python ${{ matrix.python-version }}
         run: |
             dnf install -y /usr/lib64/libxkbcommon.so.0 /usr/lib64/libxslt.so.1 /usr/bin/llvm-config clang
             git config --global --add safe.directory '*'
             python -m pip install --upgrade "pip" "meson" "ninja" "numpy" "meson-python" "build" "wheel" "twine" "auditwheel" "aqtinstall"
-            python -m pip install "PySide6==6.4.2"
+            python -m pip install "PySide6==6.5.0"
             python -m pip install \
                 --index-url=http://download.qt.io/official_releases/QtForPython/ \
                 --trusted-host download.qt.io \
-                "shiboken6_generator==6.4.2"
-            aqt install-qt -O /Qt linux desktop 6.4.2
-            LD_LIBRARY_PATH=/Qt/6.4.2/gcc_64/lib python3 -m build --no-isolation  .
+                "shiboken6_generator==6.5.0"
+            aqt install-qt -O /Qt linux desktop 6.5.0
+            LD_LIBRARY_PATH=/Qt/6.5.0/gcc_64/lib python3 -m build --no-isolation  .
             rename 'linux_x86_64' 'manylinux_2_28_x86_64' dist/*.whl
       - name: Save packages as artifacts
         uses: actions/upload-artifact@v3
         with:
           name: sciqlopplots-linux-${{ matrix.python-version }}
           path: dist/*
       - name: Publish on PyPi
```

### Comparing `sciqlopplots-0.1.8/.github/workflows/pythonpublish-osx.yml` & `sciqlopplots-0.2.2/.github/workflows/pythonpublish-osx.yml`

 * *Files 3% similar despite different names*

```diff
@@ -18,23 +18,23 @@
       - name: Build python wheel
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
       - name: add qt dir to path
         run: |
-            echo "$GITHUB_WORKSPACE/Qt/6.4.2/macos/bin" >> $GITHUB_PATH
+            echo "$GITHUB_WORKSPACE/Qt/6.5.0/macos/bin" >> $GITHUB_PATH
       - run: |
           brew install rename
           pip install --upgrade "meson" "ninja" "numpy" "meson-python" "build" "wheel" "twine" "aqtinstall"
-          pip install "PySide6==6.4.2"
+          pip install "PySide6==6.5.0"
           pip install \
               --index-url=http://download.qt.io/official_releases/QtForPython/ \
-              --trusted-host download.qt.io "shiboken6_generator==6.4.2"
-          aqt install-qt -O $GITHUB_WORKSPACE/Qt mac desktop 6.4.2
+              --trusted-host download.qt.io "shiboken6_generator==6.5.0"
+          aqt install-qt -O $GITHUB_WORKSPACE/Qt mac desktop 6.5.0
           python3 -m build --no-isolation .
           rename 's/macosx_10_15_[0-9]_x86_64/macosx_10_15_x86_64/g' dist/*.whl
       - name: Save packages as artifacts
         uses: actions/upload-artifact@v3
         with:
           name: sciqlopplots-MacOs-${{ matrix.python-version }}
           path: dist/*
```

### Comparing `sciqlopplots-0.1.8/.github/workflows/pythonpublish-win.yml` & `sciqlopplots-0.2.2/.github/workflows/pythonpublish-win.yml`

 * *Files 6% similar despite different names*

```diff
@@ -18,28 +18,28 @@
       - name: Set up Clang
         uses: egor-tensin/setup-clang@v1
         with:
           version: latest
           platform: x64
       - name: add qt dir to path
         run: |
-          echo "C:\Program Files\LLVM\bin;${{github.workspace}}\Qt\6.4.2\mingw_64\bin;C:\msys64\mingw64\bin" | Out-File -FilePath $env:GITHUB_PATH -Encoding utf8 -Append
+          echo "C:\Program Files\LLVM\bin;${{github.workspace}}\Qt\6.5.0\mingw_64\bin;C:\msys64\mingw64\bin" | Out-File -FilePath $env:GITHUB_PATH -Encoding utf8 -Append
       - name: Set python interpreter
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64 
       - name: Install deps and build package
         env:
           CLANG_INSTALL_DIR: C:\Program Files\LLVM\
         run: |
           pip install --upgrade "meson" "ninja" "numpy" "meson-python" "build" "wheel" "twine" "auditwheel" "aqtinstall"
-          pip install "PySide6==6.4.2"
-          pip install --index-url=http://download.qt.io/official_releases/QtForPython/ --trusted-host download.qt.io "shiboken6_generator==6.4.2"
-          aqt install-qt -O $env:GITHUB_WORKSPACE\Qt windows desktop 6.4.2 win64_mingw
+          pip install "PySide6==6.5.0"
+          pip install --index-url=http://download.qt.io/official_releases/QtForPython/ --trusted-host download.qt.io "shiboken6_generator==6.5.0"
+          aqt install-qt -O $env:GITHUB_WORKSPACE\Qt windows desktop 6.5.0 win64_mingw
           python3 -m build --no-isolation  .
 
       - name: Save packages as artifacts
         uses: actions/upload-artifact@v3
         with:
           name: sciqlopplots-windows-${{ matrix.python-version }}
           path: dist/*
```

### Comparing `sciqlopplots-0.1.8/COPYING` & `sciqlopplots-0.2.2/COPYING`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build` & `sciqlopplots-0.2.2/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/SciQLopPlots/bindings/_QCustomPlot.hpp` & `sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopPlot.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -16,25 +16,42 @@
 -- along with this program; if not, write to the Free Software
 -- Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 -------------------------------------------------------------------------------*/
 /*-- Author : Alexis Jeandet
 -- Mail : alexis.jeandet@member.fsf.org
 ----------------------------------------------------------------------------*/
 #pragma once
+#include <SciQLopPlots/SciQLopColorMap.hpp>
+
 
+#include "constants.hpp"
+#include <QPointF>
 #include <SciQLopPlots/SciQLopGraph.hpp>
-#include <SciQLopPlots/SciQLopColorMap.hpp>
+#include <SciQLopPlots/SciQLopPlotItem.hpp>
+#include <optional>
 #include <qcustomplot.h>
 
-class _QCustomPlot : public QCustomPlot
+class SciQLopPlot : public QCustomPlot
 {
     Q_OBJECT
+
 public:
-    explicit _QCustomPlot(QWidget* parent = nullptr) : QCustomPlot { parent } {};
-    virtual ~_QCustomPlot() Q_DECL_OVERRIDE {};
+    explicit SciQLopPlot(QWidget* parent = nullptr) : QCustomPlot { parent }
+    {
+        using namespace Constants;
+        this->addLayer(
+            LayersNames::Spans, this->layer(LayersNames::Overlay), QCustomPlot::limAbove);
+        this->layer(LayersNames::Spans)->setMode(QCPLayer::lmBuffered);
+        this->layer(LayersNames::Spans)->setVisible(true);
+        this->addLayer(
+            LayersNames::SpansBorders, this->layer(LayersNames::Spans), QCustomPlot::limAbove);
+        this->layer(LayersNames::SpansBorders)->setMode(QCPLayer::lmBuffered);
+        this->layer(LayersNames::SpansBorders)->setVisible(true);
+    }
+    virtual ~SciQLopPlot() Q_DECL_OVERRIDE { }
     inline QCPColorMap* addColorMap(QCPAxis* x, QCPAxis* y)
     {
         auto cm = new QCPColorMap(x, y);
         return cm;
     }
 
     inline SciQLopGraph* addSciQLopGraph(QCPAxis* x, QCPAxis* y, QStringList labels,
@@ -45,8 +62,13 @@
     }
     inline SciQLopColorMap* addSciQLopColorMap(QCPAxis* x, QCPAxis* y, const QString& name,
         SciQLopColorMap::DataOrder dataOrder = SciQLopColorMap::DataOrder::xFirst)
     {
         auto sg = new SciQLopColorMap(this, x, y, name, dataOrder);
         return sg;
     }
+
+protected:
+    virtual void mousePressEvent(QMouseEvent* event) override;
+    virtual void mouseMoveEvent(QMouseEvent* event) override;
+    virtual void mouseReleaseEvent(QMouseEvent* event) override;
 };
```

### Comparing `sciqlopplots-0.1.8/SciQLopPlots/bindings/bindings.xml` & `sciqlopplots-0.2.2/SciQLopPlots/bindings/bindings.xml`

 * *Files 1% similar despite different names*

#### Comparing `sciqlopplots-0.1.8/SciQLopPlots/bindings/bindings.xml` & `sciqlopplots-0.2.2/SciQLopPlots/bindings/bindings.xml`

```diff
@@ -54,14 +54,24 @@
     <enum-type name="RefreshPriority"/>
     <modify-function signature="addColorMap(QCPAxis*, QCPAxis*)" return-type="QCPColorMap*" static="no">
       <modify-argument index="return">
         <define-ownership class="native" owner="c++"/>
         <define-ownership class="target" owner="c++"/>
       </modify-argument>
     </modify-function>
+  </object-type>
+  <object-type name="SciQLopPlot" parent-management="yes">
+    <enum-type name="LayerInsertMode"/>
+    <enum-type name="RefreshPriority"/>
+    <modify-function signature="addColorMap(QCPAxis*, QCPAxis*)" return-type="QCPColorMap*" static="no">
+      <modify-argument index="return">
+        <define-ownership class="native" owner="c++"/>
+        <define-ownership class="target" owner="c++"/>
+      </modify-argument>
+    </modify-function>
     <modify-function signature="addSciQLopGraph(QCPAxis*, QCPAxis*, QStringList, SciQLopGraph::DataOrder)">
       <modify-argument index="return">
         <define-ownership class="target" owner="target"/>
       </modify-argument>
     </modify-function>
     <modify-function signature="addSciQLopColorMap(QCPAxis*, QCPAxis*, const QString&amp;, SciQLopGraph::DataOrder)">
       <modify-argument index="return">
@@ -318,8 +328,9 @@
       <include file-name="SciQLopPlots/numpy_wrappers.hpp" location="global"/>
       <include file-name="utility" location="global"/>
     </extra-includes>
     <add-function signature="setData(PyObject *@x@, PyObject *@y@, PyObject *@z@)">
       <inject-code file="snippets.cpp" snippet="SciQLopColorMap-setData"/>
     </add-function>
   </object-type>
+  <object-type name="SciQLopVerticalSpan" parent-management="yes"/>
 </typesystem>
```

### Comparing `sciqlopplots-0.1.8/SciQLopPlots/bindings/helper_scripts/rpath-helper.py` & `sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/rpath-helper.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py` & `sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py` & `sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/SciQLopPlots/bindings/helper_scripts/src_list.py` & `sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/src_list.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/SciQLopPlots/bindings/snippets.cpp` & `sciqlopplots-0.2.2/SciQLopPlots/bindings/snippets.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 // @snippet QCPGraph-setData
 NpArray_view x{pyArgs[0]};
 NpArray_view y{pyArgs[1]};
+Py_BEGIN_ALLOW_THREADS
 QVector<QCPGraphData> data(x.flat_size());
 const auto x_data = x.data();
 const auto y_data = y.data();
 for(auto i=0UL;i<x.flat_size();i++)
 {
     data[i]={x_data[i],y_data[i]};
 }
 %CPPSELF.data()->set(std::move(data),true);
+Py_END_ALLOW_THREADS
 // @snippet QCPGraph-setData
 
 // @snippet QCPGraph-setSelected
 if(%1)
 {
     %CPPSELF->setSelection(QCPDataSelection(%CPPSELF->data()->dataRange()));
 }
```

### Comparing `sciqlopplots-0.1.8/SciQLopPlots/meson.build` & `sciqlopplots-0.2.2/SciQLopPlots/meson.build`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 qtmod = import(qt_sdk)
-qtdeps = dependency(qt_sdk, modules : ['Core','Widgets','Gui','Svg','PrintSupport', 'OpenGL'])
+qtdeps = dependency(qt_sdk, modules : ['Core','Widgets','Gui','Svg','PrintSupport', 'OpenGL'], method:'qmake')
 
 cpp_utils_dep = dependency('cpp_utils', fallback : ['cpp_utils', 'cpp_utils_dep'], default_options: [f'with_tests=false'])
 hedley_dep = dependency('hedley', main : true, fallback : ['hedley', 'hedley_dep'])
 
 
-qmake_possible_names = ['qmake','qmake6']
+qmake_possible_names = ['qmake-qt6','qmake6','qmake']
 pyside_version = '6'
 
 
 project_source_root = meson.project_source_root()
 current_source_dir = meson.current_source_dir()
 
 src_list = find_program('bindings/helper_scripts/src_list.py')
@@ -49,29 +49,41 @@
 
 shiboken_dep = declare_dependency(compile_args: shiboken_build_flags, link_args: shiboken_link_flags)
 
 moc_headers = [
     'bindings/_QCustomPlot.hpp',
     project_source_root+'/include/SciQLopPlots/SciQLopGraph.hpp',
     project_source_root+'/include/SciQLopPlots/SciQLopColorMap.hpp',
+    project_source_root+'/include/SciQLopPlots/SciQLopVerticalSpan.hpp',
+    project_source_root+'/include/SciQLopPlots/SciQLopPlotItem.hpp',
+    project_source_root+'/include/SciQLopPlots/SciQLopPlot.hpp',
     project_source_root+'/qcustomplot-source/qcustomplot.h'
 ]
 
 moc_sources = []
-headers = moc_headers + [project_source_root+'/include/SciQLopPlots/numpy_wrappers.hpp']
+headers = moc_headers + \
+         [project_source_root+'/include/SciQLopPlots/numpy_wrappers.hpp',
+         project_source_root+'/include/SciQLopPlots/constants.hpp']
 
 includes = include_directories(['../include', '../qcustomplot-source', numpy_inc])
 
 moc_files = qtmod.preprocess(
                             moc_headers : moc_headers,
                             moc_sources : moc_sources,
                             include_directories : includes)
 
 
-sources = moc_files + sciqlopplots_bindings_src + shiboken_generator_out +['../src/SciQLopGraph.cpp', '../src/SciQLopColorMap.cpp', '../src/numpy_wrappers.cpp' , '../qcustomplot-source/qcustomplot.cpp']
+sources = moc_files \
+        + sciqlopplots_bindings_src \
+        + shiboken_generator_out \
+        + [ '../src/SciQLopPlot.cpp', '../src/SciQLopPlotItem.cpp',
+            '../src/SciQLopVerticalSpan.cpp', '../src/SciQLopGraph.cpp',
+            '../src/SciQLopColorMap.cpp', '../src/numpy_wrappers.cpp' ,
+            '../qcustomplot-source/qcustomplot.cpp'
+        ]
 
 sciqlopplots_bindings = python3.extension_module('SciQLopPlotsBindings',
         sources,
         dependencies : [ python3_dep, shiboken_dep, qtdeps, cpp_utils_dep],
         cpp_args:['-DQCUSTOMPLOT_USE_OPENGL'],
         subdir : 'SciQLopPlots',
         install: true,
```

### Comparing `sciqlopplots-0.1.8/include/SciQLopPlots/SciQLopColorMap.hpp` & `sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopColorMap.hpp`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 -- along with this program; if not, write to the Free Software
 -- Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 -------------------------------------------------------------------------------*/
 /*-- Author : Alexis Jeandet
 -- Mail : alexis.jeandet@member.fsf.org
 ----------------------------------------------------------------------------*/
 #pragma once
-
 #include "numpy_wrappers.hpp"
+
 #include <QMutex>
 #include <qcustomplot.h>
 
 class SciQLopColorMap : public QObject
 {
     NpArray_view _x;
     NpArray_view _y;
```

### Comparing `sciqlopplots-0.1.8/include/SciQLopPlots/SciQLopGraph.hpp` & `sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopGraph.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/include/SciQLopPlots/numpy_wrappers.hpp` & `sciqlopplots-0.2.2/include/SciQLopPlots/numpy_wrappers.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/meson.build` & `sciqlopplots-0.2.2/meson.build`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-project('SciQLopPlots', 'cpp',default_options : ['cpp_std=c++17', 'buildtype=release'], license: 'GPL3', version: '0.1.8')
+project('SciQLopPlots', 'cpp',default_options : ['cpp_std=c++17', 'buildtype=release'], license: 'GPL3', version: '0.2.2')
 add_project_arguments(
             '-DCATCH_CONFIG_NO_POSIX_SIGNALS', # workaround for this https://github.com/catchorg/Catch2/issues/2192
             language: 'cpp',
             native: true
 )
 qt_sdk='qt6'
```

### Comparing `sciqlopplots-0.1.8/pyproject.toml` & `sciqlopplots-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = [
     "wheel",
     "ninja",
     "numpy",
     "meson-python",
     "meson>=0.63",
-    "shiboken6==6.4.2",
-    "pyside6==6.4.2",
-    "shiboken6_generator==6.4.2"
+    "shiboken6==6.5.0",
+    "pyside6==6.5.0",
+    "shiboken6_generator==6.5.0"
 ]
 build-backend = 'mesonpy'
 
 [project]
 name = "SciQLopPlots"
 description="SciQLop plot API based on QCustomPlot"
 authors = [{name="Alexis Jeandet", email="alexis.jeandet@member.fsf.org"}]
@@ -26,13 +26,13 @@
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-dependencies = ['numpy', 'pyside6==6.4.2', 'shiboken6==6.4.2']
+dependencies = ['numpy', 'pyside6==6.5.0', 'shiboken6==6.5.0']
 dynamic = [
   'version',
 ]
 [project.urls]
 homepage = "https://github.com/SciQLop/SciQLopPlots"
```

### Comparing `sciqlopplots-0.1.8/qcustomplot-source/GPL.txt` & `sciqlopplots-0.2.2/qcustomplot-source/GPL.txt`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/qcustomplot-source/changelog.txt` & `sciqlopplots-0.2.2/qcustomplot-source/changelog.txt`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/qcustomplot-source/qcustomplot.cpp` & `sciqlopplots-0.2.2/qcustomplot-source/qcustomplot.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/qcustomplot-source/qcustomplot.h` & `sciqlopplots-0.2.2/qcustomplot-source/qcustomplot.h`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/src/SciQLopColorMap.cpp` & `sciqlopplots-0.2.2/src/SciQLopColorMap.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/src/SciQLopGraph.cpp` & `sciqlopplots-0.2.2/src/SciQLopGraph.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/src/numpy_wrappers.cpp` & `sciqlopplots-0.2.2/src/numpy_wrappers.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/tests/manual-tests/QCP_Examples/plots/main.py` & `sciqlopplots-0.2.2/tests/manual-tests/QCP_Examples/plots/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/tests/manual-tests/SciQLopColorMap/main.py` & `sciqlopplots-0.2.2/tests/manual-tests/SciQLopColorMap/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/tests/manual-tests/SciQLopGraph/main.py` & `sciqlopplots-0.2.2/tests/manual-tests/SciQLopGraph/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from SciQLopPlots import QCustomPlot, QCP, QCPColorMap, QCPRange, QCPColorScale, QCPAxis, QCPColorGradient, QCPMarginGroup
+from SciQLopPlots import SciQLopPlot,QCustomPlot, QCP, QCPColorMap, QCPRange, QCPColorScale, QCPAxis, QCPColorGradient, QCPMarginGroup
 from PySide6.QtWidgets import QMainWindow, QApplication
 from PySide6.QtGui import QPen, QColorConstants, QColor, QBrush
 import sys
 import math
 import numpy as np
 from types import SimpleNamespace
 
@@ -10,15 +10,15 @@
 class MainWindow(QMainWindow):
     def __init__(self):
         QMainWindow.__init__(self)
         self._setup_ui()
         self.setGeometry(400, 250, 542, 390);
 
     def _setup_ui(self):
-        plot: QCustomPlot = QCustomPlot(self)
+        plot: SciQLopPlot = SciQLopPlot(self)
         plot.setInteractions(QCP.iRangeDrag|QCP.iRangeZoom|QCP.iSelectPlottables)
         self.setCentralWidget(plot)
         self.graph = plot.addSciQLopGraph(plot.xAxis, plot.yAxis, ["X","Y","Z"])
         x=np.arange(3e7)*1.
         y=np.ones((3,len(x)))
         y[0]=np.cos(x/60)
         y[1]=np.cos(x/600)*1.3
```

### Comparing `sciqlopplots-0.1.8/tests/manual-tests/StackedGraphs/main.py` & `sciqlopplots-0.2.2/tests/manual-tests/StackedGraphs/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.1.8/tests/manual-tests/meson.build` & `sciqlopplots-0.2.2/tests/manual-tests/meson.build`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 examples = [
     {'name':'plots', 'source': meson.current_source_dir()+'/QCP_Examples/plots/main.py'},
     {'name':'SciQLopGraph', 'source': meson.current_source_dir()+'/SciQLopGraph/main.py'},
     {'name':'SciQLopColorMap', 'source': meson.current_source_dir()+'/SciQLopColorMap/main.py'},
     {'name':'StackedGraphs', 'source': meson.current_source_dir()+'/StackedGraphs/main.py'},
+    {'name':'SciQLopVerticalSpan', 'source': meson.current_source_dir()+'/SciQLopVerticalSpan/main.py'},
 ]
 
 foreach example:examples
     run_target('examples_'+example['name'],
         command:[python3, example['source']],
         env: ['PYTHONPATH='+meson.project_build_root()]
     )
```

### Comparing `sciqlopplots-0.1.8/PKG-INFO` & `sciqlopplots-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciqlopplots
-Version: 0.1.8
+Version: 0.2.2
 Summary: SciQLop plot API based on QCustomPlot
 Home-page: https://github.com/SciQLop/SciQLopPlots
 Author-Email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 License: GNU GENERAL PUBLIC LICENSE
                               Version 3, 29 June 2007
         
             An easy to use ISTP loader package.
@@ -44,16 +44,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Homepage, https://github.com/SciQLop/SciQLopPlots
 Requires-Python: >=3.7
 Requires-Dist: numpy
-Requires-Dist: pyside6==6.4.2
-Requires-Dist: shiboken6==6.4.2
+Requires-Dist: pyside6==6.5.0
+Requires-Dist: shiboken6==6.5.0
 Description-Content-Type: text/markdown
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![CPP17](https://img.shields.io/badge/Language-C++17-blue.svg)]()
 [![PyPi](https://img.shields.io/pypi/v/sciqlopplots.svg)](https://pypi.python.org/pypi/sciqlopplots)
 [![Coverage](https://codecov.io/gh/SciQLop/CDFpp/coverage.svg?branch=main)](https://codecov.io/gh/SciQLop/SciQLopPlots/branch/main)
```

