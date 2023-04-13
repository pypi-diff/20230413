# Comparing `tmp/sciqlopplots-0.2.2.tar.gz` & `tmp/sciqlopplots-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciqlopplots-0.2.2.tar", last modified: Mon Apr 10 17:05:07 2023, max compression
+gzip compressed data, was "sciqlopplots-0.2.4.tar", last modified: Thu Apr 13 11:33:35 2023, max compression
```

## Comparing `sciqlopplots-0.2.2.tar` & `sciqlopplots-0.2.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/.clang-format
--rw-r--r--   0        0        0     2077 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/.github/workflows/pythonpublish-linux.yml
--rw-r--r--   0        0        0     1779 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/.github/workflows/pythonpublish-osx.yml
--rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/.github/workflows/pythonpublish-win.yml
--rw-r--r--   0        0        0      207 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/.gitignore
--rw-r--r--   0        0        0     1552 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/COPYING
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/README.md
--rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/__init__.py
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/_QCustomPlot.hpp
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/bindings.h
--rw-r--r--   0        0        0    16781 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/bindings.xml
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/rpath-helper.py
--rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py
--rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py
--rwxr-xr-x   0        0        0     2052 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/src_list.py
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/bindings/snippets.cpp
--rw-r--r--   0        0        0     4717 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/SciQLopPlots/meson.build
--rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopColorMap.hpp
--rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopGraph.hpp
--rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopPlot.hpp
--rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopPlotItem.hpp
--rw-r--r--   0        0        0     8901 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopVerticalSpan.hpp
--rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/include/SciQLopPlots/constants.hpp
--rw-r--r--   0        0        0     5734 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/include/SciQLopPlots/numpy_wrappers.hpp
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/meson.build
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/meson_options.txt
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/pyproject.toml
--rwxr-xr-x   0        0        0    35147 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/qcustomplot-source/GPL.txt
--rwxr-xr-x   0        0        0    54691 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/qcustomplot-source/changelog.txt
--rw-r--r--   0        0        0  1307498 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/qcustomplot-source/qcustomplot.cpp
--rw-r--r--   0        0        0   310085 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/qcustomplot-source/qcustomplot.h
--rw-r--r--   0        0        0      296 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/setup.cfg
--rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/src/SciQLopColorMap.cpp
--rw-r--r--   0        0        0     5982 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/src/SciQLopGraph.cpp
--rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/src/SciQLopPlot.cpp
--rw-r--r--   0        0        0     1172 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/src/SciQLopPlotItem.cpp
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/src/SciQLopVerticalSpan.cpp
--rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/src/numpy_wrappers.cpp
--rw-r--r--   0        0        0       70 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/subprojects/cpp_utils.wrap
--rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/subprojects/hedley.wrap
--rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/tests/manual-tests/QCP_Examples/plots/main.py
--rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/tests/manual-tests/SciQLopColorMap/main.py
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/tests/manual-tests/SciQLopGraph/main.py
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/tests/manual-tests/SciQLopVerticalSpan/main.py
--rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/tests/manual-tests/StackedGraphs/main.py
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/tests/manual-tests/meson.build
--rw-r--r--   0        0        0       23 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/tests/meson.build
--rw-r--r--   0        0        0     3120 1970-01-01 00:00:00.000000 sciqlopplots-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/.clang-format
+-rw-r--r--   0        0        0     2077 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/.github/workflows/pythonpublish-linux.yml
+-rw-r--r--   0        0        0     1777 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/.github/workflows/pythonpublish-osx.yml
+-rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/.github/workflows/pythonpublish-win.yml
+-rw-r--r--   0        0        0      207 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1552 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/COPYING
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/README.md
+-rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/SciQLopPlots/__init__.py
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/SciQLopPlots/bindings/_QCustomPlot.hpp
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/SciQLopPlots/bindings/bindings.h
+-rw-r--r--   0        0        0    16781 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/SciQLopPlots/bindings/bindings.xml
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/SciQLopPlots/bindings/helper_scripts/rpath-helper.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py
+-rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py
+-rwxr-xr-x   0        0        0     2052 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/SciQLopPlots/bindings/helper_scripts/src_list.py
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/SciQLopPlots/bindings/snippets.cpp
+-rw-r--r--   0        0        0     4717 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/SciQLopPlots/meson.build
+-rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/include/SciQLopPlots/SciQLopColorMap.hpp
+-rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/include/SciQLopPlots/SciQLopGraph.hpp
+-rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/include/SciQLopPlots/SciQLopPlot.hpp
+-rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/include/SciQLopPlots/SciQLopPlotItem.hpp
+-rw-r--r--   0        0        0     8901 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/include/SciQLopPlots/SciQLopVerticalSpan.hpp
+-rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/include/SciQLopPlots/constants.hpp
+-rw-r--r--   0        0        0     5734 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/include/SciQLopPlots/numpy_wrappers.hpp
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/meson.build
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/meson_options.txt
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/pyproject.toml
+-rwxr-xr-x   0        0        0    35147 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/qcustomplot-source/GPL.txt
+-rwxr-xr-x   0        0        0    54691 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/qcustomplot-source/changelog.txt
+-rw-r--r--   0        0        0  1307498 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/qcustomplot-source/qcustomplot.cpp
+-rw-r--r--   0        0        0   310085 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/qcustomplot-source/qcustomplot.h
+-rw-r--r--   0        0        0      296 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/setup.cfg
+-rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/src/SciQLopColorMap.cpp
+-rw-r--r--   0        0        0     5982 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/src/SciQLopGraph.cpp
+-rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/src/SciQLopPlot.cpp
+-rw-r--r--   0        0        0     1172 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/src/SciQLopPlotItem.cpp
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/src/SciQLopVerticalSpan.cpp
+-rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/src/numpy_wrappers.cpp
+-rw-r--r--   0        0        0       70 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/subprojects/cpp_utils.wrap
+-rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/subprojects/hedley.wrap
+-rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/tests/manual-tests/QCP_Examples/plots/main.py
+-rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/tests/manual-tests/SciQLopColorMap/main.py
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/tests/manual-tests/SciQLopGraph/main.py
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/tests/manual-tests/SciQLopVerticalSpan/main.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/tests/manual-tests/StackedGraphs/main.py
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/tests/manual-tests/meson.build
+-rw-r--r--   0        0        0       23 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/tests/meson.build
+-rw-r--r--   0        0        0     3120 1970-01-01 00:00:00.000000 sciqlopplots-0.2.4/PKG-INFO
```

### Comparing `sciqlopplots-0.2.2/.clang-format` & `sciqlopplots-0.2.4/.clang-format`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/.github/workflows/pythonpublish-linux.yml` & `sciqlopplots-0.2.4/.github/workflows/pythonpublish-linux.yml`

 * *Files 6% similar despite different names*

```diff
@@ -14,30 +14,30 @@
       fail-fast: false
       matrix:
         python-version: ['cp38-cp38', 'cp39-cp39', 'cp310-cp310', 'cp311-cp311']
     steps:
       - name: add Python and qt dir to path
         run: |
             echo "/opt/python/${{ matrix.python-version }}/bin" >> $GITHUB_PATH
-            echo "/Qt/6.5.0/gcc_64/bin" >> $GITHUB_PATH
+            echo "/Qt/6.4.3/gcc_64/bin" >> $GITHUB_PATH
       - uses: actions/checkout@v3
         with:
           submodules: true
       - name: Build for Python ${{ matrix.python-version }}
         run: |
             dnf install -y /usr/lib64/libxkbcommon.so.0 /usr/lib64/libxslt.so.1 /usr/bin/llvm-config clang
             git config --global --add safe.directory '*'
             python -m pip install --upgrade "pip" "meson" "ninja" "numpy" "meson-python" "build" "wheel" "twine" "auditwheel" "aqtinstall"
-            python -m pip install "PySide6==6.5.0"
+            python -m pip install "PySide6==6.4.3"
             python -m pip install \
                 --index-url=http://download.qt.io/official_releases/QtForPython/ \
                 --trusted-host download.qt.io \
-                "shiboken6_generator==6.5.0"
-            aqt install-qt -O /Qt linux desktop 6.5.0
-            LD_LIBRARY_PATH=/Qt/6.5.0/gcc_64/lib python3 -m build --no-isolation  .
+                "shiboken6_generator==6.4.3"
+            aqt install-qt -O /Qt linux desktop 6.4.3
+            LD_LIBRARY_PATH=/Qt/6.4.3/gcc_64/lib python3 -m build --no-isolation  .
             rename 'linux_x86_64' 'manylinux_2_28_x86_64' dist/*.whl
       - name: Save packages as artifacts
         uses: actions/upload-artifact@v3
         with:
           name: sciqlopplots-linux-${{ matrix.python-version }}
           path: dist/*
       - name: Publish on PyPi
```

### Comparing `sciqlopplots-0.2.2/.github/workflows/pythonpublish-osx.yml` & `sciqlopplots-0.2.4/.github/workflows/pythonpublish-osx.yml`

 * *Files 10% similar despite different names*

```diff
@@ -3,40 +3,40 @@
 on:
   release:
     types: [published]
   push:
 
 jobs:
   build:
-    runs-on: macos-10.15
+    runs-on: macos-11
     strategy:
       max-parallel: 4
       matrix:
         python-version: ['3.8', '3.9', '3.10', '3.11']
     name: Python ${{ matrix.python-version }}
     steps:
       - uses: actions/checkout@v3
       - name: Build python wheel
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
       - name: add qt dir to path
         run: |
-            echo "$GITHUB_WORKSPACE/Qt/6.5.0/macos/bin" >> $GITHUB_PATH
+            echo "$GITHUB_WORKSPACE/Qt/6.4.3/macos/bin" >> $GITHUB_PATH
       - run: |
           brew install rename
           pip install --upgrade "meson" "ninja" "numpy" "meson-python" "build" "wheel" "twine" "aqtinstall"
-          pip install "PySide6==6.5.0"
+          pip install "PySide6==6.4.3"
           pip install \
               --index-url=http://download.qt.io/official_releases/QtForPython/ \
-              --trusted-host download.qt.io "shiboken6_generator==6.5.0"
-          aqt install-qt -O $GITHUB_WORKSPACE/Qt mac desktop 6.5.0
+              --trusted-host download.qt.io "shiboken6_generator==6.4.3"
+          aqt install-qt -O $GITHUB_WORKSPACE/Qt mac desktop 6.4.3
           python3 -m build --no-isolation .
-          rename 's/macosx_10_15_[0-9]_x86_64/macosx_10_15_x86_64/g' dist/*.whl
+          #rename 's/macosx_10_15_[0-9]_x86_64/macosx_10_15_x86_64/g' dist/*.whl
       - name: Save packages as artifacts
         uses: actions/upload-artifact@v3
         with:
           name: sciqlopplots-MacOs-${{ matrix.python-version }}
           path: dist/*
       - name: Publish on PyPi
         if: github.event.release
```

### Comparing `sciqlopplots-0.2.2/.github/workflows/pythonpublish-win.yml` & `sciqlopplots-0.2.4/.github/workflows/pythonpublish-win.yml`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,28 @@
       - name: Set up Clang
         uses: egor-tensin/setup-clang@v1
         with:
           version: latest
           platform: x64
       - name: add qt dir to path
         run: |
-          echo "C:\Program Files\LLVM\bin;${{github.workspace}}\Qt\6.5.0\mingw_64\bin;C:\msys64\mingw64\bin" | Out-File -FilePath $env:GITHUB_PATH -Encoding utf8 -Append
+          echo "C:\Program Files\LLVM\bin;${{github.workspace}}\Qt\6.4.3\mingw_64\bin;C:\msys64\mingw64\bin" | Out-File -FilePath $env:GITHUB_PATH -Encoding utf8 -Append
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
-          pip install "PySide6==6.5.0"
-          pip install --index-url=http://download.qt.io/official_releases/QtForPython/ --trusted-host download.qt.io "shiboken6_generator==6.5.0"
-          aqt install-qt -O $env:GITHUB_WORKSPACE\Qt windows desktop 6.5.0 win64_mingw
+          pip install "PySide6==6.4.3"
+          pip install --index-url=http://download.qt.io/official_releases/QtForPython/ --trusted-host download.qt.io "shiboken6_generator==6.4.3"
+          aqt install-qt -O $env:GITHUB_WORKSPACE\Qt windows desktop 6.4.3 win64_mingw
           python3 -m build --no-isolation  .
 
       - name: Save packages as artifacts
         uses: actions/upload-artifact@v3
         with:
           name: sciqlopplots-windows-${{ matrix.python-version }}
           path: dist/*
```

### Comparing `sciqlopplots-0.2.2/COPYING` & `sciqlopplots-0.2.4/COPYING`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build` & `sciqlopplots-0.2.4/SciQLopPlots/bindings/SciQLopPlotsBindings/meson.build`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/SciQLopPlots/bindings/_QCustomPlot.hpp` & `sciqlopplots-0.2.4/SciQLopPlots/bindings/_QCustomPlot.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/SciQLopPlots/bindings/bindings.xml` & `sciqlopplots-0.2.4/SciQLopPlots/bindings/bindings.xml`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/rpath-helper.py` & `sciqlopplots-0.2.4/SciQLopPlots/bindings/helper_scripts/rpath-helper.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py` & `sciqlopplots-0.2.4/SciQLopPlots/bindings/helper_scripts/shiboken-gen.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py` & `sciqlopplots-0.2.4/SciQLopPlots/bindings/helper_scripts/shiboken-helper.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/SciQLopPlots/bindings/helper_scripts/src_list.py` & `sciqlopplots-0.2.4/SciQLopPlots/bindings/helper_scripts/src_list.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/SciQLopPlots/bindings/snippets.cpp` & `sciqlopplots-0.2.4/SciQLopPlots/bindings/snippets.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/SciQLopPlots/meson.build` & `sciqlopplots-0.2.4/SciQLopPlots/meson.build`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopColorMap.hpp` & `sciqlopplots-0.2.4/include/SciQLopPlots/SciQLopColorMap.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopGraph.hpp` & `sciqlopplots-0.2.4/include/SciQLopPlots/SciQLopGraph.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopPlot.hpp` & `sciqlopplots-0.2.4/include/SciQLopPlots/SciQLopPlot.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopPlotItem.hpp` & `sciqlopplots-0.2.4/include/SciQLopPlots/SciQLopPlotItem.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/include/SciQLopPlots/SciQLopVerticalSpan.hpp` & `sciqlopplots-0.2.4/include/SciQLopPlots/SciQLopVerticalSpan.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/include/SciQLopPlots/constants.hpp` & `sciqlopplots-0.2.4/include/SciQLopPlots/constants.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/include/SciQLopPlots/numpy_wrappers.hpp` & `sciqlopplots-0.2.4/include/SciQLopPlots/numpy_wrappers.hpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/meson.build` & `sciqlopplots-0.2.4/meson.build`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-project('SciQLopPlots', 'cpp',default_options : ['cpp_std=c++17', 'buildtype=release'], license: 'GPL3', version: '0.2.2')
+project('SciQLopPlots', 'cpp',default_options : ['cpp_std=c++17', 'buildtype=release'], license: 'GPL3', version: '0.2.4')
 add_project_arguments(
             '-DCATCH_CONFIG_NO_POSIX_SIGNALS', # workaround for this https://github.com/catchorg/Catch2/issues/2192
             language: 'cpp',
             native: true
 )
 qt_sdk='qt6'
```

### Comparing `sciqlopplots-0.2.2/pyproject.toml` & `sciqlopplots-0.2.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = [
     "wheel",
     "ninja",
     "numpy",
     "meson-python",
     "meson>=0.63",
-    "shiboken6==6.5.0",
-    "pyside6==6.5.0",
-    "shiboken6_generator==6.5.0"
+    "shiboken6==6.4.3",
+    "pyside6==6.4.3",
+    "shiboken6_generator==6.4.3"
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
-dependencies = ['numpy', 'pyside6==6.5.0', 'shiboken6==6.5.0']
+dependencies = ['numpy', 'pyside6==6.4.3', 'shiboken6==6.4.3']
 dynamic = [
   'version',
 ]
 [project.urls]
 homepage = "https://github.com/SciQLop/SciQLopPlots"
```

### Comparing `sciqlopplots-0.2.2/qcustomplot-source/GPL.txt` & `sciqlopplots-0.2.4/qcustomplot-source/GPL.txt`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/qcustomplot-source/changelog.txt` & `sciqlopplots-0.2.4/qcustomplot-source/changelog.txt`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/qcustomplot-source/qcustomplot.cpp` & `sciqlopplots-0.2.4/qcustomplot-source/qcustomplot.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/qcustomplot-source/qcustomplot.h` & `sciqlopplots-0.2.4/qcustomplot-source/qcustomplot.h`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/src/SciQLopColorMap.cpp` & `sciqlopplots-0.2.4/src/SciQLopColorMap.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/src/SciQLopGraph.cpp` & `sciqlopplots-0.2.4/src/SciQLopGraph.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/src/SciQLopPlot.cpp` & `sciqlopplots-0.2.4/src/SciQLopPlot.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/src/SciQLopPlotItem.cpp` & `sciqlopplots-0.2.4/src/SciQLopPlotItem.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/src/SciQLopVerticalSpan.cpp` & `sciqlopplots-0.2.4/src/SciQLopVerticalSpan.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/src/numpy_wrappers.cpp` & `sciqlopplots-0.2.4/src/numpy_wrappers.cpp`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/tests/manual-tests/QCP_Examples/plots/main.py` & `sciqlopplots-0.2.4/tests/manual-tests/QCP_Examples/plots/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/tests/manual-tests/SciQLopColorMap/main.py` & `sciqlopplots-0.2.4/tests/manual-tests/SciQLopColorMap/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/tests/manual-tests/SciQLopGraph/main.py` & `sciqlopplots-0.2.4/tests/manual-tests/SciQLopGraph/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/tests/manual-tests/SciQLopVerticalSpan/main.py` & `sciqlopplots-0.2.4/tests/manual-tests/SciQLopVerticalSpan/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/tests/manual-tests/StackedGraphs/main.py` & `sciqlopplots-0.2.4/tests/manual-tests/StackedGraphs/main.py`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/tests/manual-tests/meson.build` & `sciqlopplots-0.2.4/tests/manual-tests/meson.build`

 * *Files identical despite different names*

### Comparing `sciqlopplots-0.2.2/PKG-INFO` & `sciqlopplots-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciqlopplots
-Version: 0.2.2
+Version: 0.2.4
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
-Requires-Dist: pyside6==6.5.0
-Requires-Dist: shiboken6==6.5.0
+Requires-Dist: pyside6==6.4.3
+Requires-Dist: shiboken6==6.4.3
 Description-Content-Type: text/markdown
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![CPP17](https://img.shields.io/badge/Language-C++17-blue.svg)]()
 [![PyPi](https://img.shields.io/pypi/v/sciqlopplots.svg)](https://pypi.python.org/pypi/sciqlopplots)
 [![Coverage](https://codecov.io/gh/SciQLop/CDFpp/coverage.svg?branch=main)](https://codecov.io/gh/SciQLop/SciQLopPlots/branch/main)
```

