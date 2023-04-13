# Comparing `tmp/qulacs-0.5.6.tar.gz` & `tmp/qulacs-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qulacs-0.5.6.tar", last modified: Fri Feb 17 04:23:06 2023, max compression
+gzip compressed data, was "qulacs-0.6.0.tar", last modified: Thu Apr 13 06:42:32 2023, max compression
```

## Comparing `qulacs-0.5.6.tar` & `qulacs-0.6.0.tar`

### file list

```diff
@@ -1,395 +1,435 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.079955 qulacs-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-02-17 04:22:40.000000 qulacs-0.5.6/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.039956 qulacs-0.5.6/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-02-17 04:22:40.000000 qulacs-0.5.6/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     2346 2023-02-17 04:22:40.000000 qulacs-0.5.6/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.035956 qulacs-0.5.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.039956 qulacs-0.5.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-02-17 04:22:40.000000 qulacs-0.5.6/.github/workflows/build_devcontainer_image.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-02-17 04:22:40.000000 qulacs-0.5.6/.github/workflows/ci_macos.yml
--rw-r--r--   0 runner    (1001) docker     (122)     6901 2023-02-17 04:22:40.000000 qulacs-0.5.6/.github/workflows/ci_ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-02-17 04:22:40.000000 qulacs-0.5.6/.github/workflows/ci_windows.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-02-17 04:22:40.000000 qulacs-0.5.6/.github/workflows/wheel.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-02-17 04:22:40.000000 qulacs-0.5.6/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.039956 qulacs-0.5.6/.vscode/
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-02-17 04:22:40.000000 qulacs-0.5.6/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (122)    16209 2023-02-17 04:22:40.000000 qulacs-0.5.6/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-02-17 04:22:40.000000 qulacs-0.5.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-02-17 04:22:40.000000 qulacs-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    13053 2023-02-17 04:23:06.075955 qulacs-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11067 2023-02-17 04:22:40.000000 qulacs-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-17 04:22:40.000000 qulacs-0.5.6/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.039956 qulacs-0.5.6/benchmark/
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-02-17 04:22:40.000000 qulacs-0.5.6/benchmark/AdaptiveGate.py
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-02-17 04:22:40.000000 qulacs-0.5.6/benchmark/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-02-17 04:22:40.000000 qulacs-0.5.6/benchmark/benchmark2.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-02-17 04:22:40.000000 qulacs-0.5.6/benchmark/causalconetest.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-02-17 04:22:40.000000 qulacs-0.5.6/benchmark/libcppsim_benchmark.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    17638 2023-02-17 04:22:40.000000 qulacs-0.5.6/benchmark/libcsim_benchmark.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-02-17 04:22:40.000000 qulacs-0.5.6/benchmark/merge_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5914 2023-02-17 04:22:40.000000 qulacs-0.5.6/benchmark/test_qulacs_1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-02-17 04:22:40.000000 qulacs-0.5.6/benchmark/test_qulacs_2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.039956 qulacs-0.5.6/cmake_script/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.039956 qulacs-0.5.6/cmake_script/FetchContent/
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-02-17 04:22:40.000000 qulacs-0.5.6/cmake_script/FetchContent/CMakeLists.cmake.in
--rw-r--r--   0 runner    (1001) docker     (122)    38023 2023-02-17 04:22:40.000000 qulacs-0.5.6/cmake_script/FetchContent.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     1475 2023-02-17 04:22:40.000000 qulacs-0.5.6/cmake_script/FindAVX2.cmake
--rw-r--r--   0 runner    (1001) docker     (122)      951 2023-02-17 04:22:40.000000 qulacs-0.5.6/cmake_script/FindSVE.cmake
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.039956 qulacs-0.5.6/doc/
--rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.043956 qulacs-0.5.6/doc/en/
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.043956 qulacs-0.5.6/doc/en/source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.035956 qulacs-0.5.6/doc/en/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.043956 qulacs-0.5.6/doc/en/source/_static/images/
--rw-r--r--   0 runner    (1001) docker     (122)     7067 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/_static/images/dojo.png
--rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/_static/images/github.png
--rw-r--r--   0 runner    (1001) docker     (122)    54241 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/_static/images/logo-c-h.png
--rw-r--r--   0 runner    (1001) docker     (122)     2627 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/_static/images/slack.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.043956 qulacs-0.5.6/doc/en/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/_templates/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.043956 qulacs-0.5.6/doc/en/source/apply/
--rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/apply/0_overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)   162833 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/apply/5.2_qcl.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    30093 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/apply/6.2_vqe.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    55651 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/apply/6.3_ssvqe.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.043956 qulacs-0.5.6/doc/en/source/apply/img/
--rw-r--r--   0 runner    (1001) docker     (122)    59895 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/apply/img/QCL.png
--rw-r--r--   0 runner    (1001) docker     (122)     3200 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.043956 qulacs-0.5.6/doc/en/source/guide/
--rw-r--r--   0 runner    (1001) docker     (122)   140097 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/guide/2.0_python_advanced.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.043956 qulacs-0.5.6/doc/en/source/intro/
--rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/intro/0_about.md
--rw-r--r--   0 runner    (1001) docker     (122)     3799 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/intro/1_install.md
--rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/intro/2_faq.md
--rw-r--r--   0 runner    (1001) docker     (122)     2856 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/intro/3_usage.md
--rw-r--r--   0 runner    (1001) docker     (122)    24628 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/intro/4.1_python_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    25763 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/intro/4.2_cpp_tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.043956 qulacs-0.5.6/doc/en/source/pyRef/
--rw-r--r--   0 runner    (1001) docker     (122)      777 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/pyRef/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.043956 qulacs-0.5.6/doc/en/source/write/
--rw-r--r--   0 runner    (1001) docker     (122)     2574 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/en/source/write/0_readme.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.043956 qulacs-0.5.6/doc/ja/
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.043956 qulacs-0.5.6/doc/ja/source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.035956 qulacs-0.5.6/doc/ja/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.047956 qulacs-0.5.6/doc/ja/source/_static/images/
--rw-r--r--   0 runner    (1001) docker     (122)     7067 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/_static/images/dojo.png
--rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/_static/images/github.png
--rw-r--r--   0 runner    (1001) docker     (122)    54241 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/_static/images/logo-c-h.png
--rw-r--r--   0 runner    (1001) docker     (122)     2627 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/_static/images/slack.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.047956 qulacs-0.5.6/doc/ja/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (122)     3319 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.047956 qulacs-0.5.6/doc/ja/source/guide/
--rw-r--r--   0 runner    (1001) docker     (122)    68663 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/guide/2.0_python_advanced.md
--rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.047956 qulacs-0.5.6/doc/ja/source/intro/
--rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/intro/0_about.md
--rw-r--r--   0 runner    (1001) docker     (122)     3799 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/intro/1_install.md
--rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/intro/2_faq.md
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/intro/3_usage.md
--rw-r--r--   0 runner    (1001) docker     (122)    12988 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/intro/4.1_python_tutorial.md
--rw-r--r--   0 runner    (1001) docker     (122)    26305 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/intro/4.2_cpp_tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.047956 qulacs-0.5.6/doc/ja/source/pyRef/
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/ja/source/pyRef/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.047956 qulacs-0.5.6/doc/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)     5920 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/scripts/customdoxygen.css
--rw-r--r--   0 runner    (1001) docker     (122)    10217 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/scripts/doxy-boot.js
--rw-r--r--   0 runner    (1001) docker     (122)      710 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/scripts/footer.html
--rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/scripts/header.html
--rw-r--r--   0 runner    (1001) docker     (122)     7954 2023-02-17 04:22:40.000000 qulacs-0.5.6/doc/scripts/index.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.035956 qulacs-0.5.6/docker/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.047956 qulacs-0.5.6/docker/cpu/
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-02-17 04:22:40.000000 qulacs-0.5.6/docker/cpu/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.047956 qulacs-0.5.6/docker/gpu/
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-02-17 04:22:40.000000 qulacs-0.5.6/docker/gpu/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-02-17 04:22:40.000000 qulacs-0.5.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.035956 qulacs-0.5.6/pysrc/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.047956 qulacs-0.5.6/pysrc/qulacs/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32024 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-02-17 04:23:05.000000 qulacs-0.5.6/pysrc/qulacs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.047956 qulacs-0.5.6/pysrc/qulacs/circuit/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/circuit/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/circuit/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/circuit.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.051956 qulacs-0.5.6/pysrc/qulacs/converter/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13021 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/converter/qasm_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.051956 qulacs-0.5.6/pysrc/qulacs/gate/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/gate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10692 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/gate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/gate/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     6441 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/gate.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.051956 qulacs-0.5.6/pysrc/qulacs/observable/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/observable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/observable/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/observable/_get_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/observable/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/observable.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.051956 qulacs-0.5.6/pysrc/qulacs/quantum_operator/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/quantum_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/quantum_operator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/quantum_operator/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/quantum_operator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.051956 qulacs-0.5.6/pysrc/qulacs/state/
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2068 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/state/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/state/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1451 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/state.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.051956 qulacs-0.5.6/pysrc/qulacs/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/utils/conversions_openfermion.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.051956 qulacs-0.5.6/pysrc/qulacs/vistest/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/vistest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/vistest/test_vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.051956 qulacs-0.5.6/pysrc/qulacs/visualizer/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-02-17 04:22:40.000000 qulacs-0.5.6/pysrc/qulacs/visualizer/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.047956 qulacs-0.5.6/pysrc/qulacs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    13053 2023-02-17 04:23:05.000000 qulacs-0.5.6/pysrc/qulacs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10110 2023-02-17 04:23:06.000000 qulacs-0.5.6/pysrc/qulacs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-17 04:23:05.000000 qulacs-0.5.6/pysrc/qulacs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-17 04:23:05.000000 qulacs-0.5.6/pysrc/qulacs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-02-17 04:23:05.000000 qulacs-0.5.6/pysrc/qulacs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-02-17 04:23:05.000000 qulacs-0.5.6/pysrc/qulacs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.051956 qulacs-0.5.6/python/
--rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-02-17 04:22:40.000000 qulacs-0.5.6/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    70781 2023-02-17 04:22:40.000000 qulacs-0.5.6/python/cppsim_wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.051956 qulacs-0.5.6/python/stub-test/
--rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-02-17 04:22:40.000000 qulacs-0.5.6/python/stub-test/generate_mypy_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.051956 qulacs-0.5.6/python/test/
--rw-r--r--   0 runner    (1001) docker     (122)    52301 2023-02-17 04:22:40.000000 qulacs-0.5.6/python/test/test_qulacs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.055956 qulacs-0.5.6/script/
--rwxr-xr-x   0 runner    (1001) docker     (122)      303 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/build_clang.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      657 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/build_gcc.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      440 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/build_gcc_with_gpu.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      441 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/build_gcc_with_memory_sanitizer.sh
--rw-r--r--   0 runner    (1001) docker     (122)      300 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/build_msvc_2015.bat
--rw-r--r--   0 runner    (1001) docker     (122)      301 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/build_msvc_2015_with_gpu.bat
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/build_msvc_2017.bat
--rw-r--r--   0 runner    (1001) docker     (122)      301 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/build_msvc_2017_with_gpu.bat
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/build_msvc_2019.bat
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/build_msvc_2019_with_gpu.bat
--rwxr-xr-x   0 runner    (1001) docker     (122)      127 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/clean.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/download_wheel.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      318 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/fix_wheel_osx.sh
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/generate_msvc_project_2015.bat
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/generate_msvc_project_2015_with_gpu.bat
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/generate_msvc_project_2017.bat
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/generate_msvc_project_2017_with_gpu.bat
--rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/generate_msvc_project_2019.bat
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/generate_msvc_project_2019_with_gpu.bat
--rwxr-xr-x   0 runner    (1001) docker     (122)      436 2023-02-17 04:22:40.000000 qulacs-0.5.6/script/update_stubs.sh
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-17 04:23:06.079955 qulacs-0.5.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5049 2023-02-17 04:22:40.000000 qulacs-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.055956 qulacs-0.5.6/src/
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.059956 qulacs-0.5.6/src/cppsim/
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    20206 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    21953 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/circuit.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/circuit_builder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7895 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/circuit_optimizer.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/circuit_optimizer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8557 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/exception.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5100 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10490 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    31782 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    18683 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_factory.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    24644 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_general.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    12953 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6483 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_matrix_diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6184 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_matrix_diagonal.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5044 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_matrix_sparse.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5835 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_matrix_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    20532 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_merge.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6478 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_merge.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_named_one.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    14607 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_named_one.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7977 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_named_pauli.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8317 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_named_two.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    23274 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_noisy_evolution.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    12950 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_noisy_evolution.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_reflect.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_reversible.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2368 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/gate_to_gqo.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    34320 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/general_quantum_operator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    14623 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/general_quantum_operator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    14140 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/matrix_decomposition.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/noisesimulator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3925 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/noisesimulator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    13716 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/observable.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5966 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/observable.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    15000 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/pauli_operator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10673 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/pauli_operator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/qubit_info.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7181 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/qubit_info.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2374 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2795 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/simulator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2687 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/state.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    24409 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/state.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4610 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/state_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    16411 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/state_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/state_gpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    14607 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/state_gpu.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/type.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10550 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/utility.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8184 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/cppsim/utility.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.067956 qulacs-0.5.6/src/csim/
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/constant.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/constant.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/init_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      748 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/init_ops_fill.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4353 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/init_ops_random.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      661 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/memory_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/memory_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/memory_ops_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/memory_ops_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3410 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/stat_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2777 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/stat_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10432 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/stat_ops_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1639 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/stat_ops_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10821 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/stat_ops_expectation_value.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/stat_ops_probability.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4800 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/stat_ops_transition_amplitude.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/type.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    54340 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_control_multi_target_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    11713 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_control_multi_target_single.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_control_single_target_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10121 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_control_single_target_single.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    34691 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3689 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    45281 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_matrix_dense_double.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2387 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_matrix_dense_double_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_matrix_dense_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_matrix_dense_multi_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7745 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_matrix_dense_single.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3749 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_matrix_diagonal_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4173 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_matrix_diagonal_single.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3078 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_matrix_phase_single.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1542 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_named.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6056 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_named_CNOT.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4208 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_named_CZ.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_named_H.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5086 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_named_SWAP.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3255 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_named_X.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3742 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_named_Y.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_named_Z.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1865 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_named_projection.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_named_state.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    16633 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_pauli_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2359 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_pauli_single.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2922 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_qft.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      705 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_reflection.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/update_ops_reversible_boolean.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5153 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/utility.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5405 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/csim/utility.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.067956 qulacs-0.5.6/src/gpusim/
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6204 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/memory_ops.cu
--rw-r--r--   0 runner    (1001) docker     (122)      917 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/memory_ops.h
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/memory_ops_device_functions.h
--rw-r--r--   0 runner    (1001) docker     (122)    52450 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/stat_ops.cu
--rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/stat_ops.h
--rw-r--r--   0 runner    (1001) docker     (122)     2709 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/stat_ops_device_functions.h
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/test.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8162 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/update_ops_cuda.h
--rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/update_ops_cuda_device_functions.h
--rw-r--r--   0 runner    (1001) docker     (122)    69614 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/update_ops_multi.cu
--rw-r--r--   0 runner    (1001) docker     (122)    21139 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/update_ops_named.cu
--rw-r--r--   0 runner    (1001) docker     (122)    15186 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/update_ops_single.cu
--rw-r--r--   0 runner    (1001) docker     (122)    24389 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/util.cu
--rw-r--r--   0 runner    (1001) docker     (122)     2806 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/util.cuh
--rw-r--r--   0 runner    (1001) docker     (122)     2201 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/util.h
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/util_common.h
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/util_export.h
--rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/util_func.h
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/util_type.h
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/gpusim/util_type_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.071956 qulacs-0.5.6/src/vqcsim/
--rw-r--r--   0 runner    (1001) docker     (122)      372 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1910 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/GradCalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/GradCalculator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      730 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/boolean_formula.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8079 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/causalcone_simulator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/differential.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      788 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/differential.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/loss_function.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/loss_function.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3015 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/optimizer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    13788 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/parametric_circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3267 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/parametric_circuit.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/parametric_circuit_builder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10288 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/parametric_gate.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/parametric_gate_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      823 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/parametric_gate_factory.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/parametric_simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      603 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/parametric_simulator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/parser.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4262 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/problem.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5367 2023-02-17 04:22:40.000000 qulacs-0.5.6/src/vqcsim/solver.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.071956 qulacs-0.5.6/test/
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.075955 qulacs-0.5.6/test/cppsim/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      450 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/H2.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/test_KAK.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    30583 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/test_circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     9244 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/test_circuit_optimize_light.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    53940 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/test_gate.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    29782 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/test_gate_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    21214 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/test_hamiltonian.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5465 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/test_hamiltonian_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    12025 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/test_noise_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5334 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/test_noisesimulator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    20963 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/test_noisyevolution.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6242 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/test_pauli_operator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/test_simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    11552 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/test_state.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    11267 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/cppsim/test_state_dm.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.075955 qulacs-0.5.6/test/csim/
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/csim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1206 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/csim/test_memory.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/csim/test_omputil.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    26148 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/csim/test_stat.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10104 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/csim/test_update_control.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5690 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/csim/test_update_dense.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/csim/test_update_dense_double.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3340 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/csim/test_update_diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/csim/test_update_diagonal_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     9616 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/csim/test_update_named.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6955 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/csim/test_update_pauli.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.075955 qulacs-0.5.6/test/gpusim/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/gpusim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/gpusim/H2.txt
--rw-r--r--   0 runner    (1001) docker     (122)    33345 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/gpusim/test_circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     9054 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/gpusim/test_compat_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2249 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/gpusim/test_func_memory.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    46976 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/gpusim/test_gate.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     9409 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/gpusim/test_hamiltonian.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    43199 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/gpusim/test_state.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8477 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/gpusim/test_update_control.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    14992 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/gpusim/test_update_dense.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3689 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/gpusim/test_update_diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10223 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/gpusim/test_update_named.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8335 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/gpusim/test_update_pauli.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/gpusim/test_util.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.075955 qulacs-0.5.6/test/util/
--rw-r--r--   0 runner    (1001) docker     (122)    13090 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/util/util.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-17 04:23:06.075955 qulacs-0.5.6/test/vqcsim/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/vqcsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    15642 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/vqcsim/test.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4767 2023-02-17 04:22:40.000000 qulacs-0.5.6/test/vqcsim/test_backprop.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.288308 qulacs-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-13 06:41:58.000000 qulacs-0.6.0/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.208310 qulacs-0.6.0/.devcontainer/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.216309 qulacs-0.6.0/.devcontainer/cpu/
+-rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-04-13 06:41:58.000000 qulacs-0.6.0/.devcontainer/cpu/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-04-13 06:41:58.000000 qulacs-0.6.0/.devcontainer/cpu/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.216309 qulacs-0.6.0/.devcontainer/gpu/
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-13 06:41:58.000000 qulacs-0.6.0/.devcontainer/gpu/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     2766 2023-04-13 06:41:58.000000 qulacs-0.6.0/.devcontainer/gpu/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.208310 qulacs-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.216309 qulacs-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-04-13 06:41:58.000000 qulacs-0.6.0/.github/workflows/ci_macos.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     9050 2023-04-13 06:41:58.000000 qulacs-0.6.0/.github/workflows/ci_ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-04-13 06:41:58.000000 qulacs-0.6.0/.github/workflows/ci_windows.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-04-13 06:41:58.000000 qulacs-0.6.0/.github/workflows/wheel.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-04-13 06:41:58.000000 qulacs-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-04-13 06:41:58.000000 qulacs-0.6.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.216309 qulacs-0.6.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-04-13 06:41:58.000000 qulacs-0.6.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (122)    17144 2023-04-13 06:41:58.000000 qulacs-0.6.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-04-13 06:41:58.000000 qulacs-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-04-13 06:41:58.000000 qulacs-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    13054 2023-04-13 06:42:32.288308 qulacs-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11068 2023-04-13 06:41:58.000000 qulacs-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11431 2023-04-13 06:41:58.000000 qulacs-0.6.0/README_MPI.md
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-13 06:41:58.000000 qulacs-0.6.0/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.220309 qulacs-0.6.0/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/AdaptiveGate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4799 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/bench_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/benchmark2.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/causalconetest.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.220309 qulacs-0.6.0/benchmark/circuits/
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/circuits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/circuits/quantumvolume.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/circuits/qulacsbench.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/libcppsim_benchmark.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    17638 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/libcsim_benchmark.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/merge_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5914 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/test_qulacs_1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/test_qulacs_2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.220309 qulacs-0.6.0/cmake_script/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.220309 qulacs-0.6.0/cmake_script/FetchContent/
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-04-13 06:41:58.000000 qulacs-0.6.0/cmake_script/FetchContent/CMakeLists.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (122)    38023 2023-04-13 06:41:58.000000 qulacs-0.6.0/cmake_script/FetchContent.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     1475 2023-04-13 06:41:58.000000 qulacs-0.6.0/cmake_script/FindAVX2.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-04-13 06:41:58.000000 qulacs-0.6.0/cmake_script/FindSVE.cmake
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.220309 qulacs-0.6.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (122)     1935 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.220309 qulacs-0.6.0/doc/en/
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.224309 qulacs-0.6.0/doc/en/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.208310 qulacs-0.6.0/doc/en/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.224309 qulacs-0.6.0/doc/en/source/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (122)     7067 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_static/images/dojo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_static/images/github.png
+-rw-r--r--   0 runner    (1001) docker     (122)    54241 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_static/images/logo-c-h.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2627 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_static/images/slack.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.224309 qulacs-0.6.0/doc/en/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.224309 qulacs-0.6.0/doc/en/source/_templates/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/macros.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.224309 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/class.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/data.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/function.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/method.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/module.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/package.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/property.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/footer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.228309 qulacs-0.6.0/doc/en/source/apply/
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/apply/0_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)   162833 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/apply/5.2_qcl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    30093 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/apply/6.2_vqe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    55651 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/apply/6.3_ssvqe.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.228309 qulacs-0.6.0/doc/en/source/apply/img/
+-rw-r--r--   0 runner    (1001) docker     (122)    59895 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/apply/img/QCL.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.228309 qulacs-0.6.0/doc/en/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (122)   151517 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/guide/2.0_python_advanced.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.228309 qulacs-0.6.0/doc/en/source/intro/
+-rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/intro/0_about.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3799 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/intro/1_install.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/intro/2_faq.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2856 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/intro/3_usage.md
+-rw-r--r--   0 runner    (1001) docker     (122)    27329 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/intro/4.1_python_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    25763 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/intro/4.2_cpp_tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.228309 qulacs-0.6.0/doc/en/source/write/
+-rw-r--r--   0 runner    (1001) docker     (122)     2574 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/write/0_readme.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.228309 qulacs-0.6.0/doc/ja/
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.228309 qulacs-0.6.0/doc/ja/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.208310 qulacs-0.6.0/doc/ja/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.232309 qulacs-0.6.0/doc/ja/source/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (122)     7067 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_static/images/dojo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_static/images/github.png
+-rw-r--r--   0 runner    (1001) docker     (122)    54241 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_static/images/logo-c-h.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2627 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_static/images/slack.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.232309 qulacs-0.6.0/doc/ja/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.232309 qulacs-0.6.0/doc/ja/source/_templates/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/macros.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.232309 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/class.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/data.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/function.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/method.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/module.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/package.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/property.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4006 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.232309 qulacs-0.6.0/doc/ja/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (122)    75211 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/guide/2.0_python_advanced.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.232309 qulacs-0.6.0/doc/ja/source/intro/
+-rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/intro/0_about.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3799 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/intro/1_install.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/intro/2_faq.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/intro/3_usage.md
+-rw-r--r--   0 runner    (1001) docker     (122)    14702 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/intro/4.1_python_tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (122)    26305 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/intro/4.2_cpp_tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.236309 qulacs-0.6.0/doc/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     5920 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/scripts/customdoxygen.css
+-rw-r--r--   0 runner    (1001) docker     (122)    10217 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/scripts/doxy-boot.js
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/scripts/footer.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/scripts/header.html
+-rw-r--r--   0 runner    (1001) docker     (122)     7954 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/scripts/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2456 2023-04-13 06:41:58.000000 qulacs-0.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.212309 qulacs-0.6.0/pysrc/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.236309 qulacs-0.6.0/pysrc/qulacs/
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32351 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-13 06:42:32.000000 qulacs-0.6.0/pysrc/qulacs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/circuit/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/circuit/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/circuit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/circuit.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/converter/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13118 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/converter/qasm_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/gate/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/gate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10832 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/gate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/gate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     6526 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/gate.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/observable/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/observable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/observable/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/observable/_get_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/observable/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/observable.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/quantum_operator/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/quantum_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/quantum_operator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/quantum_operator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/quantum_operator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/state/
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2068 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/state/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/state/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1451 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/state.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/utils/conversions_openfermion.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/vistest/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/vistest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/vistest/test_vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.244309 qulacs-0.6.0/pysrc/qulacs/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/visualizer/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.236309 qulacs-0.6.0/pysrc/qulacs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    13054 2023-04-13 06:42:32.000000 qulacs-0.6.0/pysrc/qulacs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11697 2023-04-13 06:42:32.000000 qulacs-0.6.0/pysrc/qulacs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 06:42:32.000000 qulacs-0.6.0/pysrc/qulacs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 06:42:31.000000 qulacs-0.6.0/pysrc/qulacs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-13 06:42:32.000000 qulacs-0.6.0/pysrc/qulacs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-13 06:42:32.000000 qulacs-0.6.0/pysrc/qulacs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.244309 qulacs-0.6.0/python/
+-rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-04-13 06:41:58.000000 qulacs-0.6.0/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    71886 2023-04-13 06:41:58.000000 qulacs-0.6.0/python/cppsim_wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.244309 qulacs-0.6.0/python/stub-test/
+-rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-04-13 06:41:58.000000 qulacs-0.6.0/python/stub-test/generate_mypy_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.244309 qulacs-0.6.0/python/test/
+-rw-r--r--   0 runner    (1001) docker     (122)    52480 2023-04-13 06:41:58.000000 qulacs-0.6.0/python/test/test_qulacs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36446 2023-04-13 06:41:58.000000 qulacs-0.6.0/python/test/test_qulacs_multicpu.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.248309 qulacs-0.6.0/script/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      303 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_clang.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      691 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_gcc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      440 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_gcc_with_gpu.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      441 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_gcc_with_memory_sanitizer.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      122 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_mpicc.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_msvc_2015.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_msvc_2015_with_gpu.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_msvc_2017.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_msvc_2017_with_gpu.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_msvc_2019.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_msvc_2019_with_gpu.bat
+-rwxr-xr-x   0 runner    (1001) docker     (122)      127 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/clean.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/download_wheel.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      318 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/fix_wheel_osx.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/generate_msvc_project_2015.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/generate_msvc_project_2015_with_gpu.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/generate_msvc_project_2017.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/generate_msvc_project_2017_with_gpu.bat
+-rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/generate_msvc_project_2019.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/generate_msvc_project_2019_with_gpu.bat
+-rwxr-xr-x   0 runner    (1001) docker     (122)      436 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/update_stubs.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 06:42:32.288308 qulacs-0.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5235 2023-04-13 06:41:58.000000 qulacs-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.248309 qulacs-0.6.0/src/
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.256309 qulacs-0.6.0/src/cppsim/
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    20392 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    22387 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/circuit.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/circuit_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7895 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/circuit_optimizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/circuit_optimizer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9609 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5100 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10490 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    32399 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    19238 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_factory.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    24644 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_general.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13445 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6483 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_matrix_diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6184 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_matrix_diagonal.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5044 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_matrix_sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5835 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_matrix_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    20532 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_merge.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6478 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_merge.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5541 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_named_npair.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_named_one.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    16353 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_named_one.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7977 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_named_pauli.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8986 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_named_two.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    23274 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_noisy_evolution.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    12950 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_noisy_evolution.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_reflect.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_reversible.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2368 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_to_gqo.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    34378 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/general_quantum_operator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14623 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/general_quantum_operator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14140 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/matrix_decomposition.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/noisesimulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3925 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/noisesimulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13716 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/observable.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5966 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/observable.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14801 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/pauli_operator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10673 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/pauli_operator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/qubit_info.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7181 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/qubit_info.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2374 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/simulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2795 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/simulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/state.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    34493 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/state.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5116 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/state_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    16629 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/state_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/state_gpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15703 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/state_gpu.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/type.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10550 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/utility.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8184 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/utility.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.268308 qulacs-0.6.0/src/csim/
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7145 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/MPIutil.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2336 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/MPIutil.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/constant.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/constant.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/init_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/init_ops_fill.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/init_ops_random.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      661 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/memory_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/memory_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/memory_ops_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/memory_ops_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4584 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/stat_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/stat_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10432 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/stat_ops_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1639 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/stat_ops_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    30440 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/stat_ops_expectation_value.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/stat_ops_probability.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4800 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/stat_ops_transition_amplitude.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/type.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    60932 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7802 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_control_multi_target_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14209 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_control_multi_target_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5740 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_control_single_target_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    19452 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_control_single_target_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    34691 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3689 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    82604 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_dense_double.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2387 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_dense_double_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7071 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_dense_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_dense_multi_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    17967 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_dense_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3749 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_diagonal_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10516 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_diagonal_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_phase_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    12326 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_CNOT.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7080 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_CZ.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    12677 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_FusedSWAP.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9614 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_H.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11477 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_SWAP.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5205 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_X.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9384 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_Y.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_Z.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3194 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_projection.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    16633 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_pauli_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_pauli_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2922 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_qft.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      705 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_reflection.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_reversible_boolean.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5153 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/utility.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5405 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/utility.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.272308 qulacs-0.6.0/src/gpusim/
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6204 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/memory_ops.cu
+-rw-r--r--   0 runner    (1001) docker     (122)      917 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/memory_ops.h
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/memory_ops_device_functions.h
+-rw-r--r--   0 runner    (1001) docker     (122)    52450 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/stat_ops.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/stat_ops.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2709 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/stat_ops_device_functions.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8162 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/update_ops_cuda.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/update_ops_cuda_device_functions.h
+-rw-r--r--   0 runner    (1001) docker     (122)    69614 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/update_ops_multi.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    21139 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/update_ops_named.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    15186 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/update_ops_single.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    24389 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     2806 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util.cuh
+-rw-r--r--   0 runner    (1001) docker     (122)     2201 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util.h
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util_common.h
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util_export.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util_func.h
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util_type.h
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util_type_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.276308 qulacs-0.6.0/src/vqcsim/
+-rw-r--r--   0 runner    (1001) docker     (122)      372 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1910 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/GradCalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/GradCalculator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/boolean_formula.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8079 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/causalcone_simulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/differential.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/differential.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/loss_function.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/loss_function.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3015 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/optimizer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13788 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3267 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_circuit.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_circuit_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10288 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_gate.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_gate_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      823 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_gate_factory.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_simulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      603 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_simulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parser.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4262 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/problem.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5367 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/solver.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.276308 qulacs-0.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.280308 qulacs-0.6.0/test/cppsim/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/H2.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_KAK.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    30583 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    32800 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_circuit_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9942 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_circuit_optimize_light.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    55264 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_gate.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    29782 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_gate_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    57226 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_gate_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    21214 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_hamiltonian.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5465 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_hamiltonian_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15636 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_hamiltonian_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_mpiutil_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    12025 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_noise_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5334 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_noisesimulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    20963 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_noisyevolution.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6242 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_pauli_operator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_simulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11552 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11267 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_state_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5685 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_state_multicpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.284308 qulacs-0.6.0/test/csim/
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1206 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_memory.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_omputil.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    26768 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_stat.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10235 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_update_control.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5793 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_update_dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3594 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_update_dense_double.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3458 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_update_diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_update_diagonal_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13376 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_update_named.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6955 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_update_pauli.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.288308 qulacs-0.6.0/test/gpusim/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/H2.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    33345 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9054 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_compat_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2249 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_func_memory.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    47172 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_gate.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9409 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_hamiltonian.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    43543 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8633 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_update_control.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15382 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_update_dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3689 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_update_diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10371 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_update_named.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8491 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_update_pauli.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.288308 qulacs-0.6.0/test/util/
+-rw-r--r--   0 runner    (1001) docker     (122)    13090 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/util/util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.288308 qulacs-0.6.0/test/vqcsim/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/vqcsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/vqcsim/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15642 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/vqcsim/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4767 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/vqcsim/test_backprop.cpp
```

### Comparing `qulacs-0.5.6/.devcontainer/devcontainer.json` & `qulacs-0.6.0/.devcontainer/cpu/devcontainer.json`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 // For format details, see https://aka.ms/devcontainer.json. For config options, see the README at:
 // https://github.com/microsoft/vscode-dev-containers/tree/v0.209.6/containers/cpp
 {
-	"name": "C++",
+	"name": "CPU Environment",
 	"build": {
 		"dockerfile": "Dockerfile",
-		"cacheFrom": "ghcr.io/qulacs/qulacs-devcontainer:latest"
 	},
 	"runArgs": [
 		"--cap-add=SYS_PTRACE",
 		"--security-opt",
 		"seccomp=unconfined"
 	],
 	// Set *default* container specific settings.json values on container create.
-	"settings": {
-		"python.linting.enabled": true,
-		"python.linting.pylintEnabled": false,
-		"python.linting.flake8Enabled": true,
-		"python.formatting.provider": "black",
-		"editor.formatOnSave": true,
-		"editor.codeActionsOnSave": {
-			"source.organizeImports": true
-		},
-		"editor.defaultFormatter": "xaver.clang-format",
-		"python.linting.mypyEnabled": true,
-		"python.terminal.activateEnvironment": false,
-		// CAVEAT: you need to restart after building qulacs to take effect.
-		"C_Cpp.default.includePath": [
-			"include",
-			"/usr/local/include/python3.9"
-		]
+	"customizations": {
+		"vscode": {
+			"settings": {
+				"python.linting.enabled": true,
+				"python.linting.pylintEnabled": false,
+				"python.linting.flake8Enabled": true,
+				"python.formatting.provider": "black",
+				"editor.formatOnSave": true,
+				"editor.codeActionsOnSave": {
+					"source.organizeImports": true
+				},
+				"editor.defaultFormatter": "xaver.clang-format",
+				"python.linting.mypyEnabled": true,
+				"python.terminal.activateEnvironment": false,
+				// CAVEAT: you need to restart after building qulacs to take effect.
+				"C_Cpp.default.includePath": [
+					"include",
+					"/usr/local/include/python3.9"
+				]
+			},
+			// Add the IDs of extensions you want installed when the container is created.
+			"extensions": [
+				"ms-vscode.cpptools",
+				"ms-vscode.cmake-tools",
+				"ms-python.python",
+				"ms-python.vscode-pylance",
+				"xaver.clang-format"
+			]
+		}
 	},
-	// Add the IDs of extensions you want installed when the container is created.
-	"extensions": [
-		"ms-vscode.cpptools",
-		"ms-vscode.cmake-tools",
-		"ms-python.python",
-		"ms-python.vscode-pylance",
-		"xaver.clang-format"
-	],
+
 	// Required by `mounts`.
 	// c.f. https://code.visualstudio.com/remote/advancedcontainers/improve-performance#_use-a-targeted-named-volume
 	"workspaceMount": "source=${localWorkspaceFolder},target=/workspaces/qulacs,type=bind,consistency=cached",
 	"workspaceFolder": "/workspaces/qulacs",
 	"mounts": [
 		"source=${localWorkspaceFolderBasename}-build,target=${containerWorkspaceFolder}/build,type=volume"
 	],
```

### Comparing `qulacs-0.5.6/.github/workflows/ci_macos.yml` & `qulacs-0.6.0/.github/workflows/ci_macos.yml`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
       - name: Setup cmake
         uses: lukka/get-cmake@latest
 
       - name: Setup ccache
         uses: hendrikmuhs/ccache-action@v1.2
         with:
           # Include compiler to distinguish cache for each compiler.
-          key: ${{ github.job }}-${{ matrix.os }}-{{ matrix.compiler }}
+          key: ${{ github.job }}-macos-11-${{ matrix.compiler }}
           verbose: 2
 
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
```

### Comparing `qulacs-0.5.6/.github/workflows/ci_ubuntu.yml` & `qulacs-0.6.0/.github/workflows/ci_ubuntu.yml`

 * *Files 18% similar despite different names*

```diff
@@ -21,27 +21,26 @@
       matrix:
         python-version: ["3.10"]
     runs-on: "ubuntu-20.04"
     env:
       CXX_COMPILER: "/usr/lib/ccache/g++"
       C_COMPILER: "/usr/lib/ccache/gcc"
       QULACS_OPT_FLAGS: "-mtune=haswell -march=haswell -mfpmath=both"
-      PYTHON: ${{ matrix.python-version }}
       COVERAGE: "Yes"
-      CACHE_NAME: ccache-qulacs-build-v2
+      USE_TEST: "Yes"
     steps:
       - uses: actions/checkout@v3
 
       - name: Setup cmake
         uses: lukka/get-cmake@latest
 
       - name: Setup ccache
         uses: hendrikmuhs/ccache-action@v1.2
         with:
-          key: ${{ github.job }}-${{ matrix.os }}
+          key: "${{ github.job }}-ubuntu-20.04"
           verbose: 2
 
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           architecture: x64
@@ -52,15 +51,15 @@
       - name: Install LCOV
         run: |
           git clone -b v1.15 --depth 1 https://github.com/linux-test-project/lcov.git
           cd lcov
           sudo make install
 
       - name: Install qulacs for Ubuntu
-        run: USE_TEST=Yes ./script/build_gcc.sh
+        run: ./script/build_gcc.sh
 
       - name: Install qulacs Python module
         run: pip install .[ci]
       
       - name: Check stubs
         run: |
           ./script/update_stubs.sh
@@ -86,33 +85,32 @@
   gcc10-build-with-address-sanitizer:
     name: GCC10 build with -fsanitizer=address enabled
     runs-on: "ubuntu-20.04"
     env:
       CXX_COMPILER: "/usr/lib/ccache/g++"
       C_COMPILER: "/usr/lib/ccache/gcc"
       QULACS_OPT_FLAGS: "-mtune=haswell -march=haswell -mfpmath=both"
-      PYTHON: ${{ matrix.python-version }}
-      CACHE_NAME: ccache-qulacs-build-v2
+      USE_TEST: "Yes"
     steps:
       - uses: actions/checkout@v3
 
       - name: Setup cmake
         uses: lukka/get-cmake@latest
 
       - name: Setup ccache
         uses: hendrikmuhs/ccache-action@v1.2
         with:
-          key: ${{ github.job }}-${{ matrix.os }}
+          key: "${{ github.job }}-ubuntu-20.04"
           verbose: 2
 
       - name: Install boost
         run: sudo apt install libboost-dev
 
       - name: Install qulacs for Ubuntu
-        run: USE_TEST=Yes ./script/build_gcc_with_memory_sanitizer.sh
+        run: ./script/build_gcc_with_memory_sanitizer.sh
 
       - name: Test in Ubuntu
         # -j option is not appended because running this test in parallel is slower than sequential version.
         run: |
           cd ./build
           make test
 
@@ -121,25 +119,26 @@
     runs-on: "ubuntu-20.04"
     env:
       CXX_COMPILER: "/usr/lib/ccache/g++"
       C_COMPILER: "/usr/lib/ccache/gcc"
       QULACS_OPT_FLAGS: "-mtune=haswell -march=haswell -mfpmath=both"
       PYTHON: "3.7.5"
       COVERAGE: "ON"
-      CACHE_NAME: ccache-qulacs-gpu-build-v2
+      USE_TEST: "Yes"
+      USE_GPU: "Yes"
     steps:
       - uses: actions/checkout@v3
 
       - name: Setup cmake
         uses: lukka/get-cmake@latest
 
       - name: Setup ccache
         uses: hendrikmuhs/ccache-action@v1.2
         with:
-          key: ${{ github.job }}-${{ matrix.os }}
+          key: "${{ github.job }}-ubuntu-20.04"
           verbose: 2
 
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.7.5"
           architecture: x64
@@ -151,37 +150,39 @@
         uses: Jimver/cuda-toolkit@v0.2.5
         id: cuda-toolkit
 
       - name: Install qulacs for Ubuntu
         run: ./script/build_gcc_with_gpu.sh
 
       - name: Install qulacs Python module
-        run: USE_GPU=Yes pip install .[test]
+        run: pip install .[test]
+
+      - name: Build test
+        run: make -C build buildtest -j $(nproc)
 
       # Testing is removed because GPU is not available for GitHub-Hosted Runner.
 
   gcc11-sve-build:
     name: GCC11 + armv8.2-a+sve build
     runs-on: "ubuntu-22.04"
     env:
       C_COMPILER: "aarch64-linux-gnu-gcc-11"
       CXX_COMPILER: "aarch64-linux-gnu-g++-11"
       QULACS_OPT_FLAGS: "-march=armv8.2-a+sve"
       QEMU_LD_PREFIX: "/usr/aarch64-linux-gnu"
-      QEMU_CPU: "max,sve512=on"
     steps:
       - uses: actions/checkout@v3
 
       - name: Setup qemu
         run: |
           sudo apt-get update
           sudo apt-get install -y cmake ninja-build pkg-config libglib2.0-dev gcc-11-aarch64-linux-gnu g++-11-aarch64-linux-gnu
-          wget -q https://download.qemu.org/qemu-7.1.0.tar.xz
-          tar xJf qemu-7.1.0.tar.xz
-          pushd qemu-7.1.0
+          wget -q https://download.qemu.org/qemu-7.2.0.tar.xz
+          tar xJf qemu-7.2.0.tar.xz
+          pushd qemu-7.2.0
           mkdir build; cd build
           ../configure --target-list=aarch64-linux-user
           make -s -j $(nproc)
           sudo make install
 
       - name: Install boost
         run: sudo apt-get install libboost-dev
@@ -190,19 +191,22 @@
         run: USE_TEST=Yes ./script/build_gcc.sh
 
       - name: Test in Ubuntu
         run: |
           cd ./build
           make buildtest -j $(nproc)
           file ../bin/csim_test
-          qemu-aarch64 ../bin/csim_test
+          QEMU_CPU="max,sve512=on" qemu-aarch64 ../bin/csim_test
+          QEMU_CPU="max,sve256=on" qemu-aarch64 ../bin/csim_test
           file ../bin/cppsim_test
-          qemu-aarch64 ../bin/cppsim_test
+          QEMU_CPU="max,sve512=on" qemu-aarch64 ../bin/cppsim_test
+          QEMU_CPU="max,sve256=on" qemu-aarch64 ../bin/cppsim_test
           file ../bin/vqcsim_test
-          qemu-aarch64 ../bin/vqcsim_test
+          QEMU_CPU="max,sve512=on" qemu-aarch64 ../bin/vqcsim_test
+          QEMU_CPU="max,sve256=on" qemu-aarch64 ../bin/vqcsim_test
 
   format:
     name: Format with clang-format
     runs-on: "ubuntu-20.04"
     container:
       image: ghcr.io/qulacs-osaka/qulacs-ubuntu-clang-format:latest
     steps:
@@ -230,7 +234,80 @@
       - name: Compare diff
         run: |
           cd /qulacs
           diff=$(git diff)
           echo -n "$diff"
           # Without `-n`, `echo -n "$diff" | wc -l` is 1 even if `"$diff" is empty.`
           test $(echo -n "$diff" | wc -l) -eq 0
+
+  mpicc-build:
+    name: MPICC build
+    strategy:
+      matrix:
+        python-version: ["3.7.5"]
+    runs-on: "ubuntu-20.04"
+    env:
+      CXX_COMPILER: "mpic++"
+      C_COMPILER: "mpicc"
+      QULACS_OPT_FLAGS: "-mtune=haswell -march=haswell -mfpmath=both"
+      PYTHON: ${{ matrix.python-version }}
+      COVERAGE: "ON"
+    steps:
+      - uses: actions/checkout@v3
+
+      - name: Setup cmake
+        uses: lukka/get-cmake@latest
+
+      - name: Setup Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+          architecture: x64
+
+      - name: Install mpi-bin
+        run: sudo apt install openmpi-bin
+
+      - name: Install boost
+        run: sudo apt install libboost-dev
+
+      - name: Install LCOV
+        run: |
+          git clone -b v1.15 --depth 1 https://github.com/linux-test-project/lcov.git
+          cd lcov
+          sudo make install
+
+      - name: Install qulacs for Ubuntu
+        run: USE_TEST=Yes ./script/build_mpicc.sh
+
+      - name: Install qulacs Python module
+        run: USE_MPI=Yes pip install .[ci]
+
+      - name: Install MPI Python module
+        run: pip install mpi4py
+
+      - name: Check stubs
+        run: |
+          ./script/update_stubs.sh
+          diff=$(git diff)
+          echo -n "$diff"
+          # Without `-n`, `echo -n "$diff" | wc -l` is 1 even if `"$diff" is empty.`
+          test $(echo -n "$diff" | wc -l) -eq 0
+
+      - name: Test if stub is working
+        run: |
+          python python/stub-test/generate_mypy_tester.py qulacs
+          mypy python/stub-test/names_qulacs.py
+
+      - name: Test in Ubuntu
+        run: |
+          cd ./build
+          make coverage
+          make pythontest
+
+      - name: Test in Ubuntu
+        run: |
+          pip install pytest
+          mpirun -n 2 bin/cppsim_test --gtest_filter="*multicpu*"
+          mpirun -n 2 pytest python/test/test_qulacs_multicpu.py
+
+      - name: Upload coverage to codecov
+        uses: codecov/codecov-action@v3
```

### Comparing `qulacs-0.5.6/.github/workflows/ci_windows.yml` & `qulacs-0.6.0/.github/workflows/ci_windows.yml`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/.github/workflows/wheel.yml` & `qulacs-0.6.0/.github/workflows/wheel.yml`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/.gitignore` & `qulacs-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/.vscode/tasks.json` & `qulacs-0.6.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/CMakeLists.txt` & `qulacs-0.6.0/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 	cmake_policy(SET CMP0135 NEW)
 endif()
 
 project(qulacs)
 
 ##### Set default behavior #####
 set(DEFAULT_USE_OMP Yes)
+set(DEFAULT_USE_MPI No)
 set(DEFAULT_USE_GPU No)
 set(DEFAULT_USE_PYTHON Yes)
 set(DEFAULT_USE_TEST No)
 set(DEFAULT_COVERAGE No)
 if(("${CMAKE_HOST_SYSTEM_PROCESSOR}" STREQUAL "aarch64") OR
 		("${CMAKE_C_COMPILER}" MATCHES "/usr/bin/aarch64-linux-gnu-gcc*")) # for cross-compile
 	message(STATUS "SIMD SUPPORT: Yes")
@@ -67,14 +68,17 @@
 ##### Update with given flags #####
 if(NOT DEFINED USE_SIMD)
 	set(USE_SIMD ${DEFAULT_USE_SIMD})
 endif()
 if(NOT DEFINED USE_OMP)
 	set(USE_OMP ${DEFAULT_USE_OMP})
 endif()
+if(NOT DEFINED USE_MPI)
+	set(USE_MPI ${DEFAULT_USE_MPI})
+endif()
 if(NOT DEFINED USE_GPU)
 	set(USE_GPU ${DEFAULT_USE_GPU})
 endif()
 if(NOT DEFINED USE_PYTHON)
 	set(USE_PYTHON ${DEFAULT_USE_PYTHON})
 endif()
 if(NOT DEFINED USE_TEST)
@@ -86,14 +90,15 @@
 if(NOT DEFINED OPT_FLAGS)
 	set(OPT_FLAGS ${DEFAULT_OPT_FLAGS})
 endif()
 
 message(STATUS "CMAKE_HOST_SYSTEM_PROCESSOR = ${CMAKE_HOST_SYSTEM_PROCESSOR}")
 message(STATUS "USE_SIMD = ${USE_SIMD}")
 message(STATUS "USE_OMP = ${USE_OMP}")
+message(STATUS "USE_MPI = ${USE_MPI}")
 message(STATUS "USE_GPU = ${USE_GPU}")
 message(STATUS "USE_TEST = ${USE_TEST}")
 message(STATUS "COVERAGE = ${COVERAGE}")
 message(STATUS "USE_PYTHON = ${USE_PYTHON}")
 message(STATUS "OPT_FLAGS = ${OPT_FLAGS}")
 
 ##### configure include files #####
@@ -267,21 +272,35 @@
 	set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -pthread")
 	set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pthread")
 
 	# Enable imaginary literals for C++
 	if(NOT MINGW)
 		# set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fext-numeric-literals")
 	endif()
+	
+	# Disable assertion of Eigen
+	if(NOT USE_TEST)
+		add_compile_options("-D EIGEN_NO_DEBUG")
+	endif()
 
 	# Enable openmp
 	if(USE_OMP)
 		set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fopenmp")
 		set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fopenmp")
 	endif()
 
+	# Enable openmpi
+	if(USE_MPI)
+		if((NOT "${CMAKE_C_COMPILER}" MATCHES ".*mpicc") OR
+			(NOT "${CMAKE_CXX_COMPILER}" MATCHES ".*mpic\\+\\+"))
+			message(FATAL_ERROR, "USE_MPI must be used in mpicc/mpic++.")
+		endif()
+		add_compile_options("-D _USE_MPI -lmpi")
+	endif()
+
 	# Enable gpu
 	if(USE_GPU)
 		add_compile_options("-D _USE_GPU")
 		set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fPIC")
 		add_compile_options("-fPIC")
 	endif()
 
@@ -324,25 +343,35 @@
 		set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} --coverage")
 		set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} --coverage")
 	endif()
 
 elseif (${CMAKE_CXX_COMPILER_ID} STREQUAL "MSVC")
 	SET(CMAKE_C_COMPILER ${CMAKE_CXX_COMPILER})
 
+	# Disable assertion of Eigen
+	if(NOT USE_TEST)
+		add_compile_options("/D EIGEN_NO_DEBUG")
+	endif()
+
 elseif(MSVC)
 	# Compile csim with cpp compiler since VC does not completely support C99 complex values
 	# SET(CMAKE_C_COMPILER ${CMAKE_CXX_COMPILER})
 	# add_compile_options("/TP")
 
 	# Ignore warning
 	## ignore warning about template export
 	add_compile_options(/wd4251)
 	## ignore warning on non-Unicode files
 	add_compile_options(/wd4819)
 
+	# Disable assertion of Eigen
+	if(NOT USE_TEST)
+		add_compile_options("/D EIGEN_NO_DEBUG")
+	endif()
+
 	# Enable simd
 	## Check if AVX2 is supported
 	include(${CMAKE_SOURCE_DIR}/cmake_script/FindAVX2.cmake)
 	CHECK_AVX2_WINDOWS()
 	message(STATUS "AVX2_FOUND = ${AVX2_FOUND}")
 	if(USE_SIMD AND AVX2_FOUND)
 		message(STATUS "AVX2 Enabled")
@@ -352,14 +381,19 @@
 	endif()
 
 	# enable openmp
 	if(USE_OMP)
 		add_compile_options("/openmp")
 	endif()
 
+	# enable mpi
+	if(USE_MPI)
+		message(FATAL_ERROR, "USE_MPI is not supported in MSVC environment.")
+	endif()
+
 	# enable gpu
 	if(USE_GPU)
 		add_compile_options("/D_USE_GPU")
 	endif()
 
 	# Static link to multithread runtimes
 	set(variables
@@ -411,14 +445,20 @@
 			DEPENDS gpusim_test
 			DEPENDS vqcsim_test
 			COMMAND ${CMAKE_CURRENT_SOURCE_DIR}/bin/csim_test
 			COMMAND ${CMAKE_CURRENT_SOURCE_DIR}/bin/cppsim_test
 			COMMAND ${CMAKE_CURRENT_SOURCE_DIR}/bin/gpusim_test
 			COMMAND ${CMAKE_CURRENT_SOURCE_DIR}/bin/vqcsim_test
 		)
+		add_custom_target(buildtest
+			DEPENDS csim_test
+			DEPENDS cppsim_test
+			DEPENDS gpusim_test
+			DEPENDS vqcsim_test
+		)
 	else()
 		add_custom_target(test
 			DEPENDS csim_test
 			DEPENDS cppsim_test
 			DEPENDS vqcsim_test
 			COMMAND ${CMAKE_CURRENT_SOURCE_DIR}/bin/csim_test
 			COMMAND ${CMAKE_CURRENT_SOURCE_DIR}/bin/cppsim_test
```

### Comparing `qulacs-0.5.6/CONTRIBUTING.md` & `qulacs-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/LICENSE` & `qulacs-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/PKG-INFO` & `qulacs-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qulacs
-Version: 0.5.6
+Version: 0.6.0
 Summary: Quantum circuit simulator for research
 Author-email: QunaSys <qulacs@qunasys.com>
 License: MIT License
         
         Copyright (c) 2018 Qulacs Authors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,15 +48,15 @@
 [![macOS CI](https://github.com/qulacs/qulacs/actions/workflows/ci_macos.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/ci_macos.yml)
 [![Windows CI](https://github.com/qulacs/qulacs/actions/workflows/ci_windows.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/ci_windows.yml)
 [![Wheel build](https://github.com/qulacs/qulacs/actions/workflows/wheel.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/wheel.yml)
 [![Downloads](https://pepy.tech/badge/qulacs)](https://pepy.tech/project/qulacs)
 
 
 Qulacs is a Python/C++ library for fast simulation of large, noisy, or parametric quantum circuits.
-Qulacs is developed at QunaSys, Osaka University, NTT and Fujitsu.
+Qulacs is developed at QunaSys, Osaka University, NTT, and Fujitsu.
 
 Qulacs is licensed under the [MIT license](https://github.com/qulacs/qulacs/blob/master/LICENSE).
 
 ## Quick Install for Python
 
 ```
 pip install qulacs
```

### Comparing `qulacs-0.5.6/README.md` & `qulacs-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![macOS CI](https://github.com/qulacs/qulacs/actions/workflows/ci_macos.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/ci_macos.yml)
 [![Windows CI](https://github.com/qulacs/qulacs/actions/workflows/ci_windows.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/ci_windows.yml)
 [![Wheel build](https://github.com/qulacs/qulacs/actions/workflows/wheel.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/wheel.yml)
 [![Downloads](https://pepy.tech/badge/qulacs)](https://pepy.tech/project/qulacs)
 
 
 Qulacs is a Python/C++ library for fast simulation of large, noisy, or parametric quantum circuits.
-Qulacs is developed at QunaSys, Osaka University, NTT and Fujitsu.
+Qulacs is developed at QunaSys, Osaka University, NTT, and Fujitsu.
 
 Qulacs is licensed under the [MIT license](https://github.com/qulacs/qulacs/blob/master/LICENSE).
 
 ## Quick Install for Python
 
 ```
 pip install qulacs
```

### Comparing `qulacs-0.5.6/benchmark/AdaptiveGate.py` & `qulacs-0.6.0/benchmark/AdaptiveGate.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/benchmark/causalconetest.cpp` & `qulacs-0.6.0/benchmark/causalconetest.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/benchmark/libcppsim_benchmark.cpp` & `qulacs-0.6.0/benchmark/libcppsim_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/benchmark/libcsim_benchmark.cpp` & `qulacs-0.6.0/benchmark/libcsim_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/benchmark/test_qulacs_1.py` & `qulacs-0.6.0/benchmark/test_qulacs_1.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/benchmark/test_qulacs_2.py` & `qulacs-0.6.0/benchmark/test_qulacs_2.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/cmake_script/FetchContent/CMakeLists.cmake.in` & `qulacs-0.6.0/cmake_script/FetchContent/CMakeLists.cmake.in`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/cmake_script/FetchContent.cmake` & `qulacs-0.6.0/cmake_script/FetchContent.cmake`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/cmake_script/FindAVX2.cmake` & `qulacs-0.6.0/cmake_script/FindAVX2.cmake`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/cmake_script/FindSVE.cmake` & `qulacs-0.6.0/cmake_script/FindSVE.cmake`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# check for SVE instruction support
-# At current, only 512 bit vector length is supported.
+#check for SVE instruction support
+#At current, only 512 bit vector length is supported.
 
 INCLUDE(CheckCSourceRuns)
 INCLUDE(CheckCXXSourceRuns)
 
 SET(SVE_CODE "
-#include <assert.h>
 #include <arm_sve.h>
+#include <assert.h>
 int main() {
-  int n = 0;
-  n = svcntb() * 8;
-  if (n == 512) return 0;
-  else assert(0);
+    int n = 0;
+    n = svcntb() * 8;
+    if (!(n % 256))
+        return 0;
+    else
+        assert(0);
 }
 ")
 
 MACRO(CHECK_SVE_LINUX)
   SET(CMAKE_REQUIRED_FLAGS_SAVE ${CMAKE_REQUIRED_FLAGS})
 
   SET(CMAKE_REQUIRED_FLAGS "-march=armv8-a+sve")
```

### Comparing `qulacs-0.5.6/doc/.gitignore` & `qulacs-0.6.0/doc/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -133,12 +133,12 @@
 .DS_Store
 
 # build files
 
 **/_build/
 **/xml/
 */source/api
-
+*/source/pyRef
 
 **/.DS_Store
 .vscode/settings.json
-**/temp
+**/temp
```

### Comparing `qulacs-0.5.6/doc/en/Makefile` & `qulacs-0.6.0/doc/en/Makefile`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/make.bat` & `qulacs-0.6.0/doc/en/make.bat`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/source/_static/images/dojo.png` & `qulacs-0.6.0/doc/en/source/_static/images/dojo.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/source/_static/images/github.png` & `qulacs-0.6.0/doc/en/source/_static/images/github.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/source/_static/images/logo-c-h.png` & `qulacs-0.6.0/doc/en/source/_static/images/logo-c-h.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/source/_static/images/slack.png` & `qulacs-0.6.0/doc/en/source/_static/images/slack.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/source/apply/0_overview.ipynb` & `qulacs-0.6.0/doc/en/source/apply/0_overview.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/source/apply/5.2_qcl.ipynb` & `qulacs-0.6.0/doc/en/source/apply/5.2_qcl.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/source/apply/6.2_vqe.ipynb` & `qulacs-0.6.0/doc/en/source/apply/6.2_vqe.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/source/apply/6.3_ssvqe.ipynb` & `qulacs-0.6.0/doc/en/source/apply/6.3_ssvqe.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/source/apply/img/QCL.png` & `qulacs-0.6.0/doc/en/source/apply/img/QCL.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/source/conf.py` & `qulacs-0.6.0/doc/ja/source/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,137 @@
 import qulacs
 
 project = "Qulacs"
 
-language = "en"
-locale_dirs = ["locale/"]
+language = 'ja'
+locale_dirs = ['locale/']
 
 # The `extensions` list should already be in here from `sphinx-quickstart`
 extensions = [
     # there may be others here already, e.g. 'sphinx.ext.mathjax'
-    "breathe",
-    "exhale",
-    "myst_parser",
-    "nbsphinx",
-    "sphinx.ext.mathjax",
-    "sphinx_copybutton",
-    "sphinx.ext.napoleon",
-    "sphinx.ext.autodoc",
-    "sphinx.ext.graphviz",
-    "sphinx.ext.inheritance_diagram",
+    'breathe',
+    'exhale',
+    'myst_parser',
+    'nbsphinx',
+    'sphinx.ext.mathjax',
+    'sphinx_copybutton',
+    'sphinx.ext.napoleon',
+    'sphinx.ext.autodoc',
+    'sphinx.ext.graphviz',
+    'sphinx.ext.inheritance_diagram',
+    'autoapi.extension',
 ]
 
-exclude_patterns = ["_build", "**.ipynb_checkpoints"]
+exclude_patterns = ['_build', '**.ipynb_checkpoints']
 nbsphinx_allow_errors = True
 myst_enable_extensions = [
     "dollarmath",
 ]
 
+
 # source files for shpinx
 source_suffix = {
-    ".rst": "restructuredtext",
-    ".txt": "markdown",
-    ".md": "markdown",
+    '.rst': 'restructuredtext',
+    '.txt': 'markdown',
+    '.md': 'markdown',
 }
 
 # Setup the breathe extension
-breathe_projects = {"Docs": "./xml"}
+breathe_projects = {
+    "Docs": "./xml"
+}
 
 breathe_default_project = "Docs"
 
 # Setup the exhale extension
 exhale_args = {
     # These arguments are required
-    "containmentFolder": "./api",
-    "rootFileName": "cpp_library_root.rst",
-    "rootFileTitle": "C++ API Reference",
-    "doxygenStripFromPath": "..",
+    "containmentFolder":     "./api",
+    "rootFileName":          "cpp_library_root.rst",
+    "rootFileTitle":         "C++ APIリファレンス",
+    "doxygenStripFromPath":  "..",
     # Suggested optional arguments
-    "createTreeView": True,
+    "createTreeView":        True,
     # TIP: if using the sphinx-bootstrap-theme, you need
     # "treeViewIsBootstrap": True,
     "exhaleExecutesDoxygen": True,
-    "exhaleDoxygenStdin": "INPUT = ../../../src/cppsim ../../../src/vqcsim \n \
+    "exhaleDoxygenStdin": \
+        "INPUT = ../../../src/cppsim ../../../src/vqcsim \n \
+        OUTPUT_LANGUAGE = Japanese-en \n \
         FILE_PATTERNS          = *.hpp \n \
         WARN_IF_UNDOCUMENTED   = NO \n \
         ENABLE_PREPROCESSING   = YES \n \
         MACRO_EXPANSION        = YES \n \
         PREDEFINED             += __attribute__(x)= \n \
         PREDEFINED             += DllExport= \n \
-        OUTPUT_LANGUAGE = English \n \
         GENERATE_LEGEND        = YES \n \
         GRAPHICAL_HIERARCHY    = YES \n \
         CLASS_GRAPH            = YES \n \
         HIDE_UNDOC_RELATIONS   = YES\n \
-        CLASS_DIAGRAMS         = YES\n",
+        CLASS_DIAGRAMS         = YES\n"
 }
 
+autoapi_type = "python"
+autoapi_keep_files = True
+autoapi_root = "pyRef"
+# The order of `autoapi_file_patterns`` specifies the order of preference for reading files.
+# So, we give priority to `*.pyi`.
+# https://github.com/readthedocs/sphinx-autoapi/issues/243#issuecomment-684190179
+autoapi_file_patterns = ["*.pyi", "*.py"]
+autoapi_dirs = ["../../../pysrc/qulacs"]
+autoapi_add_toctree_entry = True
+autoapi_template_dir = "_templates/autoapi"
+# Avoid `maximum recursion depth exceeded while calling a Python object` error.
+autoapi_ignore = ["*/vistest/__init__.py", "*/visualizer/__init__.py"]
+autoapi_options = [
+    "members",
+    "undoc-members",
+    "show-inheritance",
+    "show-module-summary",
+    "imported-members",
+]
+
 # Tell sphinx what the primary language being documented is.
-# primary_domain = 'cpp'
+#primary_domain = 'cpp'
 
 # Tell sphinx what the pygments highlight language should be.
-# highlight_language = 'cpp'
+#highlight_language = 'cpp'
 
 #
 
 # on_rtd is whether we are on readthedocs.org, this line of code grabbed from docs.readthedocs.org
 import os
 
-on_rtd = os.environ.get("READTHEDOCS", None) == "True"
+on_rtd = os.environ.get('READTHEDOCS', None) == 'True'
 
 if not on_rtd:  # only import and set the theme if we're building docs locally
     import sphinx_rtd_theme
-
-    html_theme = "sphinx_rtd_theme"
+    html_theme = 'sphinx_rtd_theme'
     html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
 
 
 html_theme_options = {
     # 'canonical_url': '',
     # 'analytics_id': 'UA-XXXXXXX-1',  #  Provided by Google in your dashboard
-    "logo_only": False,
+    'logo_only': False,
     # 'display_version': True,
-    "prev_next_buttons_location": "bottom",
-    "style_external_links": False,
+    'prev_next_buttons_location': 'bottom',
+    'style_external_links': False,
     # 'vcs_pageview_mode': '',
-    "style_nav_header_background": "#004659",
+    'style_nav_header_background': '#004659',
     # Toc options
-    "collapse_navigation": True,
-    "sticky_navigation": True,
-    "navigation_depth": 2,
-    "includehidden": True,
-    "titles_only": False,
+    'collapse_navigation': True,
+    'sticky_navigation': True,
+    'navigation_depth': 2,
+    'includehidden': True,
+    'titles_only': False
 }
 
 templates_path = ["_templates"]
-html_static_path = ["_static"]
+html_static_path = ['_static']
 
-copyright = "2018 Qulacs Authors"
+copyright = '2018 Qulacs Authors'
 
 # `version` is only used for local build.
 # On Read the Docs, the latest version is `latest`` and the specific version
 # is the Git tag name.
 version = qulacs._version.__version__
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qulacs-0.5.6/doc/en/source/guide/2.0_python_advanced.ipynb` & `qulacs-0.6.0/doc/en/source/guide/2.0_python_advanced.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9759911644117925%*

 * *Differences: {"'cells'": "{3: {'execution_count': 2}, 5: {'execution_count': 3}, 7: {'execution_count': 4}, 13: "*

 * *            "{'execution_count': 7, 'outputs': {0: {'text': {insert: [(2, "*

 * *            "'[-0.08457288-0.14143014j -0.13386446+0.11328032j -0.22521966-0.16546737j\\n'), (3, ' "*

 * *            "-0.15105932+0.48125064j -0.45087363+0.17271267j -0.05855838+0.32498025j\\n'), (4, '  "*

 * *            "0.35972119+0.02643361j -0.10103482-0.35651694j]\\n')], delete: [4, 3, 2]}}}}, 15: "*

 * *            "{'execution_count': 8, ' […]*

```diff
@@ -24,15 +24,15 @@
             "source": [
                 "### Create and Destroy\n",
                 "Necessary memory is secured at the time of instance creation and released when the instance is destroyed, but you can explicitly destroy it to release the memory with `del`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** Quantum State ***\n",
@@ -62,15 +62,15 @@
                 "### Transform between quantum state and numpy array\n",
                 "Transformation between quantum state and numpy array can be realized by `get_vector` or `load` function. In principle, it is not checked whether the norm is saved.\n",
                 "While `get_vector` returns all the element as an array, `get_amplitude` can be used to quickly get a single element."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[1.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
@@ -96,49 +96,116 @@
             "source": [
                 "### Copy quantum states\n",
                 "Quantum states can generate new instances of the same state by `copy`. By giving a quantum state to the load function, it is possible to copy a quantum vector of another quantum state without allocating a new area in the existing quantum state. This allows you to reuse the already allocated space. You can use the `allocate_buffer` function if you want to allocate a state vector of the same size as the quantum state you already have and without copying the state."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from qulacs import QuantumState\n",
                 "\n",
                 "initial_state = QuantumState(3)\n",
                 "buffer = initial_state.allocate_buffer()\n",
                 "for ind in range(10):\n",
                 "    buffer.load(initial_state)\n",
                 "    # some computation and get results"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Store quantum state\n",
+                "Quantum states can be converted to JSON string.\n",
+                "You can restore a quantum state by loading JSON."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "original: [-0.53409555-0.11980945j  0.23272193+0.42256166j -0.65314356-0.07012461j\n",
+                        " -0.02987127+0.18778582j]\n",
+                        "restored: [-0.53409555-0.11980945j  0.23272193+0.42256166j -0.65314356-0.07012461j\n",
+                        " -0.02987127+0.18778582j]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from qulacs import QuantumState\n",
+                "from qulacs import state\n",
+                "\n",
+                "o_state = QuantumState(2)\n",
+                "o_state.set_Haar_random_state()\n",
+                "print(\"original:\", o_state.get_vector())\n",
+                "state_json = o_state.to_json()\n",
+                "\n",
+                "r_state = state.from_json(state_json)\n",
+                "print(\"restored:\", r_state.get_vector())"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Quantum states can also be saved to files in pickle format."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from qulacs import QuantumState\n",
+                "import pickle\n",
+                "\n",
+                "state = QuantumState(2)\n",
+                "\n",
+                "# store\n",
+                "with open('state.pickle', 'wb') as f:\n",
+                "    pickle.dump(state, f)\n",
+                "\n",
+                "# load\n",
+                "with open('state.pickle', 'rb') as f:\n",
+                "    state = pickle.load(f)"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Initialization of quantum state\n",
                 "The following is an function initializing a quantum state to a specific state."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[1.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
                         "[0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 1.+0.j 0.+0.j 0.+0.j]\n",
-                        "[ 0.17875932+0.12507972j  0.28161322-0.20162504j  0.21880416-0.04754893j\n",
-                        "  0.01570731+0.46979145j -0.0216192 +0.46023702j -0.20700612+0.09443371j\n",
-                        " -0.03203312+0.3305667j   0.43080876+0.03745933j]\n"
+                        "[-0.08457288-0.14143014j -0.13386446+0.11328032j -0.22521966-0.16546737j\n",
+                        " -0.15105932+0.48125064j -0.45087363+0.17271267j -0.05855838+0.32498025j\n",
+                        "  0.35972119+0.02643361j -0.10103482-0.35651694j]\n"
                     ]
                 }
             ],
             "source": [
                 "from qulacs import QuantumState\n",
                 "\n",
                 "n = 3\n",
@@ -163,27 +230,28 @@
             "source": [
                 "### Check quantum state\n",
                 "The following example is a list of functions to check quantum state information without changing the quantum state."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "qubit_count 5\n",
-                        "zero_prob_1 0.6177236324405834\n",
-                        "marginal_prob 0.3266606041128599\n",
-                        "entropy 3.1462789915919283\n",
-                        "sqaured_norm 0.9999999999999998\n",
-                        "sampling [10, 4, 4, 28, 21, 9, 22, 1, 21, 21]\n",
+                        "zero_prob_1 0.4601075596424598\n",
+                        "marginal_prob 0.20030608663813237\n",
+                        "entropy 3.1082736424124735\n",
+                        "sqaured_norm 0.9999999999999999\n",
+                        "sampling [11, 18, 12, 29, 21, 13, 28, 24, 10, 22]\n",
+                        "sampling (with seed) [23, 18, 28, 14, 17, 30, 9, 17, 16, 10]\n",
                         "device cpu\n"
                     ]
                 }
             ],
             "source": [
                 "from qulacs import QuantumState\n",
                 "\n",
@@ -237,28 +305,29 @@
             "source": [
                 "### Deformation of quantum state\n",
                 "The following functions modify a quantum state."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "state [1.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
                         "buffer [0.+0.j 0.+0.j 1.+0.j 0.+0.j]\n",
                         "added [1.+0.j 0.+0.j 1.+0.j 0.+0.j]\n",
                         "mul_coef [0.5+0.1j 0. +0.j  0.5+0.1j 0. +0.j ]\n",
+                        "mul_elementwise_func [ 0.5+0.1j  0. +0.j  -0.5-0.1j  0. -0.j ]\n",
                         "sq_norm 0.52\n",
-                        "normalized [0.69337525+0.13867505j 0.        +0.j         0.69337525+0.13867505j\n",
-                        " 0.        +0.j        ]\n",
+                        "normalized [ 0.69337525+0.13867505j  0.        +0.j         -0.69337525-0.13867505j\n",
+                        "  0.        -0.j        ]\n",
                         "sq_norm 0.9999999999999998\n"
                     ]
                 }
             ],
             "source": [
                 "from qulacs import QuantumState\n",
                 "state = QuantumState(2)\n",
@@ -305,15 +374,15 @@
             "source": [
                 "### Opetation on classic registers\n",
                 "Quantum states have classical registers as integer arrays with variable length. The classical register is used to write the result of the Instrument operation or to describe a gate that executes conditions as the result of the classical register. The value of a classic register that has not yet been written is 0. The classical register is copied at the same time when the quantum state is copied by the `copy` and `load` functions."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "20\n"
@@ -337,22 +406,22 @@
             "source": [
                 "### Calculation between quantum states\n",
                 "The inner product and tensor product between quantum states can be obtained by `inner_product` and `tensor_product` respectively."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "(0.0989867916539525+0.1746302369139219j)\n",
+                        "(-0.056292589186392766-0.06355316981838662j)\n",
                         "[0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 0.+0.j 1.+0.j 0.+0.j]\n"
                     ]
                 }
             ],
             "source": [
                 "from qulacs import QuantumState\n",
                 "from qulacs.state import inner_product, tensor_product\n",
@@ -386,35 +455,35 @@
                 "### Swap and delete qubits\n",
                 "You can swap indices of a qubit with `permutate_qubit()`.\n",
                 "You can get a projection onto a specified qubit with `drop_qubit()`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "original: [-0.25576074+0.00597572j -0.24574049-0.48099785j -0.13878694+0.39066629j\n",
-                        " -0.3435684 -0.36335378j  0.04902662+0.04174407j -0.15300638+0.2653734j\n",
-                        "  0.02229379-0.12168674j  0.24967543+0.21268185j]\n",
-                        "permutate: [-0.25576074+0.00597572j -0.13878694+0.39066629j  0.04902662+0.04174407j\n",
-                        "  0.02229379-0.12168674j -0.24574049-0.48099785j -0.3435684 -0.36335378j\n",
-                        " -0.15300638+0.2653734j   0.24967543+0.21268185j]\n",
-                        "\n",
-                        "original: [-0.11109937+0.50580828j  0.00858304-0.02332304j -0.03613546+0.40230458j\n",
-                        " -0.28334918+0.1866249j   0.30208259+0.11389186j  0.47513828+0.042232j\n",
-                        " -0.11088426-0.22169112j -0.22951727+0.08391248j]\n",
-                        "projection to 0: [-0.11109937+0.50580828j  0.00858304-0.02332304j  0.30208259+0.11389186j\n",
-                        "  0.47513828+0.042232j  ]\n",
-                        "projection to 1: [-0.03613546+0.40230458j -0.28334918+0.1866249j  -0.11088426-0.22169112j\n",
-                        " -0.22951727+0.08391248j]\n"
+                        "original: [ 0.04935285-0.33525621j -0.40848741-0.16861513j  0.0877062 +0.3016868j\n",
+                        "  0.43151866+0.12561444j  0.05137289-0.07313601j  0.10155306-0.05927549j\n",
+                        "  0.12474423-0.07303469j  0.23710293+0.53875064j]\n",
+                        "permutate: [ 0.04935285-0.33525621j  0.0877062 +0.3016868j   0.05137289-0.07313601j\n",
+                        "  0.12474423-0.07303469j -0.40848741-0.16861513j  0.43151866+0.12561444j\n",
+                        "  0.10155306-0.05927549j  0.23710293+0.53875064j]\n",
+                        "\n",
+                        "original: [-0.13129252+0.41425428j -0.06117213+0.11127952j -0.30889329-0.26279468j\n",
+                        " -0.14177694+0.05919262j  0.03556784-0.19266318j -0.24280479-0.45063361j\n",
+                        "  0.383783  -0.0233139j   0.34842192+0.19315843j]\n",
+                        "projection to 0: [-0.13129252+0.41425428j -0.06117213+0.11127952j  0.03556784-0.19266318j\n",
+                        " -0.24280479-0.45063361j]\n",
+                        "projection to 1: [-0.30889329-0.26279468j -0.14177694+0.05919262j  0.383783  -0.0233139j\n",
+                        "  0.34842192+0.19315843j]\n"
                     ]
                 }
             ],
             "source": [
                 "from qulacs import QuantumState\n",
                 "from qulacs.state import permutate_qubit, drop_qubit\n",
                 "\n",
@@ -446,15 +515,15 @@
                 "### Calculate partial trace\n",
                 "With `partial_trace()`, you can obtain a partial trace of a given qubit of a given quantum state as a density matrix.\n",
                 "The indices of the converted qubits are reassigned based on the order of the qubits before conversion."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[0.        +0.j 0.        +0.j 0.70710678+0.j 0.70710678+0.j\n",
@@ -546,15 +615,15 @@
                 "\n",
                 "### Generate and delete\n",
                 "The necessary memory is allocated when the instance is created. The memory is released when Python interpreter destroys the instance, but can be released with `del` if you want to explicitly destroy it to free memory."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** Density Matrix ***\n",
@@ -585,15 +654,15 @@
                 "You can convert quantum states and numpy array mutually with `get_matrix` and `load`.\n",
                 "If the array is 1-dimensional, it is converted from a state vector to a density matrix, and if it is 2-dimensional, it is read as a density matrix.\n",
                 "Basically, whether the norm is conserved or not is not checked."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[[1.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
@@ -631,61 +700,139 @@
                 "A quantum state can be instantiated by `copy` to create a new instance of itself.\n",
                 "Also, by giving a quantum state to the `load` function, you can copy the quantum vector or density matrix of another quantum state without allocating new space in the existing quantum state.\n",
                 "This allows you to reuse the space you have already allocated. If you want to allocate a density matrix of the same size as the quantum state you already have, but do not need to copy the state, you can use the `allocate_buffer` function."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from qulacs import QuantumState, DensityMatrix\n",
                 "\n",
                 "initial_state = DensityMatrix(3)\n",
                 "copied_state = initial_state.copy()\n",
                 "buffer = initial_state.allocate_buffer()\n",
                 "buffer.load(initial_state)\n",
                 "state_vector = QuantumState(3)\n",
                 "buffer.load(state_vector)"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Store quantum states\n",
+                "`DensityMatrix` can also be converted to/from JSON string"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 17,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "original: [[ 0.69553616+0.j         -0.30796432+0.24210111j -0.00753329-0.048494j\n",
+                        "  -0.16911174-0.16523753j]\n",
+                        " [-0.30796432-0.24210111j  0.22062831+0.j         -0.01354418+0.02409399j\n",
+                        "   0.01736242+0.13202679j]\n",
+                        " [-0.00753329+0.048494j   -0.01354418-0.02409399j  0.00346268+0.j\n",
+                        "   0.01335228-0.01000109j]\n",
+                        " [-0.16911174+0.16523753j  0.01736242-0.13202679j  0.01335228+0.01000109j\n",
+                        "   0.08037285+0.j        ]]\n",
+                        "restored: [[ 0.69553616+0.j         -0.30796432+0.24210111j -0.00753329-0.048494j\n",
+                        "  -0.16911174-0.16523753j]\n",
+                        " [-0.30796432-0.24210111j  0.22062831+0.j         -0.01354418+0.02409399j\n",
+                        "   0.01736242+0.13202679j]\n",
+                        " [-0.00753329+0.048494j   -0.01354418-0.02409399j  0.00346268+0.j\n",
+                        "   0.01335228-0.01000109j]\n",
+                        " [-0.16911174+0.16523753j  0.01736242-0.13202679j  0.01335228+0.01000109j\n",
+                        "   0.08037285+0.j        ]]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from qulacs import DensityMatrix\n",
+                "from qulacs import state\n",
+                "\n",
+                "o_state = DensityMatrix(2)\n",
+                "o_state.set_Haar_random_state()\n",
+                "print(\"original:\", o_state.get_matrix())\n",
+                "state_json = o_state.to_json()\n",
+                "\n",
+                "r_state = state.from_json(state_json)\n",
+                "print(\"restored:\", r_state.get_matrix())"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Density matrices can be stored to files in pickle format."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 18,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from qulacs import QuantumState\n",
+                "import pickle\n",
+                "\n",
+                "state = QuantumState(2)\n",
+                "\n",
+                "# store\n",
+                "with open('state.pickle', 'wb') as f:\n",
+                "    pickle.dump(state, f)\n",
+                "\n",
+                "# load\n",
+                "with open('state.pickle', 'rb') as f:\n",
+                "    state = pickle.load(f)"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Initialize quantum states\n",
                 "The following example shows functions to initialize a quantum state to a specific pure state."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[[1.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
                         " [0.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
                         " [0.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
                         " [0.+0.j 0.+0.j 0.+0.j 0.+0.j]]\n",
                         "[[0.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
                         " [0.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
                         " [0.+0.j 0.+0.j 1.+0.j 0.+0.j]\n",
                         " [0.+0.j 0.+0.j 0.+0.j 0.+0.j]]\n",
-                        "[[ 0.06955138-7.70125855e-20j -0.01203783+7.30292081e-02j\n",
-                        "   0.10872467+4.57411642e-02j -0.14160694+1.58965333e-01j]\n",
-                        " [-0.01203783-7.30292081e-02j  0.07876443-6.51380568e-19j\n",
-                        "   0.02921052-1.22078110e-01j  0.19142327+1.21174378e-01j]\n",
-                        " [ 0.10872467-4.57411642e-02j  0.02921052+1.22078110e-01j\n",
-                        "   0.20004359-5.57982323e-18j -0.11681879+3.41628304e-01j]\n",
-                        " [-0.14160694-1.58965333e-01j  0.19142327-1.21174378e-01j\n",
-                        "  -0.11681879-3.41628304e-01j  0.6516406 +8.34447617e-18j]]\n"
+                        "[[ 0.06955138+0.j         -0.01203783+0.07302921j  0.10872467+0.04574116j\n",
+                        "  -0.14160694+0.15896533j]\n",
+                        " [-0.01203783-0.07302921j  0.07876443+0.j          0.02921052-0.12207811j\n",
+                        "   0.19142327+0.12117438j]\n",
+                        " [ 0.10872467-0.04574116j  0.02921052+0.12207811j  0.20004359+0.j\n",
+                        "  -0.11681879+0.3416283j ]\n",
+                        " [-0.14160694-0.15896533j  0.19142327-0.12117438j -0.11681879-0.3416283j\n",
+                        "   0.6516406 +0.j        ]]\n"
                     ]
                 }
             ],
             "source": [
                 "from qulacs import DensityMatrix\n",
                 "\n",
                 "n = 2\n",
@@ -713,27 +860,27 @@
             "source": [
                 "### Check quantum states\n",
                 "The following example shows functions to check information of quantum states without changing the states."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "qubit_count 5\n",
-                        "zero_prob_1 0.46010755964245975\n",
-                        "marginal_prob 0.20030608663813235\n",
+                        "zero_prob_1 0.46010755964245986\n",
+                        "marginal_prob 0.20030608663813237\n",
                         "entropy 3.108273642412474\n",
-                        "sqaured_norm 0.9999999999999999\n",
-                        "sampling [18, 28, 22, 24, 21, 11, 29, 19, 30, 6]\n",
+                        "sqaured_norm 1.0000000000000002\n",
+                        "sampling [11, 30, 30, 30, 24, 6, 24, 3, 10, 29]\n",
                         "sampling (with seed) [23, 18, 28, 14, 17, 30, 9, 17, 16, 10]\n",
                         "device cpu\n"
                     ]
                 }
             ],
             "source": [
                 "from qulacs import DensityMatrix\n",
@@ -797,15 +944,15 @@
                 "- The operation corresponding to `multiply_coef(z)` of `QuantumState` is `multiply_coef(abs(z)**2)` for `DensityMatrix`\n",
                 "\n",
                 "Using `state.make_superposition()` `state.make_mixture()` is recommended since `add_state()` `multiply_coef()` make users confused with those generated by `QuantumState`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 21,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "state [[1.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
@@ -870,17 +1017,25 @@
             "source": [
                 "### Operation on classical registers\n",
                 "`DensityMatrix` also has classical registers as integer arrays with variable length."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 22,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "20\n"
+                    ]
+                }
+            ],
             "source": [
                 "from qulacs import DensityMatrix\n",
                 "state = DensityMatrix(3)\n",
                 "position = 0\n",
                 "# Set the value at `position`-th register.\n",
                 "state.set_classical_value(position, 20)\n",
                 "# Get the value at `position`-th register.\n",
@@ -897,17 +1052,29 @@
                 "\n",
                 "You can create superposition states and mixture states by using `make_superposition()` `make_mixture()` in `state` module.\n",
                 "These states can also be created by applying `add_state()` `multiply_coef()` to `QuantumState` `DensityMatrix`, but is deprecated due to low readability."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 23,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[0.5+0.j 0. +0.j 0. +0.j 0.5+0.j]\n",
+                        "[[0.5+0.j 0. +0.j 0. +0.j 0. +0.j]\n",
+                        " [0. +0.j 0. +0.j 0. +0.j 0. +0.j]\n",
+                        " [0. +0.j 0. +0.j 0. +0.j 0. +0.j]\n",
+                        " [0. +0.j 0. +0.j 0. +0.j 0.5+0.j]]\n"
+                    ]
+                }
+            ],
             "source": [
                 "from qulacs import QuantumState, DensityMatrix\n",
                 "from qulacs.state import make_superposition, make_mixture\n",
                 "# from QuantumState |a> and |b>, create a superposition state p|a> + q|b>\n",
                 "a = QuantumState(2)\n",
                 "a.set_computational_basis(0b00)\n",
                 "b = QuantumState(2)\n",
@@ -943,15 +1110,15 @@
                 "\n",
                 "### Common operations for quantum gates\n",
                 "The gate matrix of the generated quantum gate can be obtained with the `get_matrix` function. Control qubits are not included in the gate matrix. In particular, be careful when obtain gates that do not have a gate matrix (for example, $n$-qubit Pauli rotating gates), which require a very large amount of memory and time. `print` function displays the gate information."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 24,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[[0.+0.j 1.+0.j]\n",
@@ -976,27 +1143,82 @@
                 "gate = X(2)\n",
                 "mat = gate.get_matrix()\n",
                 "print(mat)\n",
                 "print(gate)"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Quantum gates can also be converted to/from JSON string.\n",
+                "Some types of gates are not supported."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 25,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        " *** gate info *** \n",
+                        " * gate name : X\n",
+                        " * target    : \n",
+                        " 2 : commute X     \n",
+                        " * control   : \n",
+                        " * Pauli     : yes\n",
+                        " * Clifford  : yes\n",
+                        " * Gaussian  : no\n",
+                        " * Parametric: no\n",
+                        " * Diagonal  : no\n",
+                        "\n",
+                        " *** gate info *** \n",
+                        " * gate name : X\n",
+                        " * target    : \n",
+                        " 2 : commute X     \n",
+                        " * control   : \n",
+                        " * Pauli     : yes\n",
+                        " * Clifford  : yes\n",
+                        " * Gaussian  : no\n",
+                        " * Parametric: no\n",
+                        " * Diagonal  : no\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from qulacs.gate import X\n",
+                "from qulacs import gate\n",
+                "\n",
+                "o_gate = X(2)\n",
+                "print(o_gate)\n",
+                "gate_json = o_gate.to_json()\n",
+                "\n",
+                "r_gate = gate.from_json(gate_json)\n",
+                "print(r_gate)"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Special gate\n",
                 "The special gates are listed below.\n",
                 "\n",
                 "#### 1 qubit gate\n",
                 "Takes the index of the target bit as the first argument."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** gate info *** \n",
@@ -1032,15 +1254,15 @@
                 "\n",
                 "#### 1 qubit rotating gate\n",
                 "Take the index of the target bit as the first argument and the rotation angle as the second argument."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** gate info *** \n",
@@ -1077,15 +1299,15 @@
                 "\n",
                 "#### IBMQ basis gate\n",
                 " IBMQ basis gate is a gate based on the virtual-Z decomposition defined by IBMQ's OpenQASM."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** gate info *** \n",
@@ -1124,15 +1346,15 @@
                 "\n",
                 "#### 2 qubit gate\n",
                 "Take the indexes of the target bit in the first and second arguments. The first argument of the CNOT gate is a control qubit. The remaining gates are symmetric operations."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** gate info *** \n",
@@ -1167,15 +1389,15 @@
             "source": [
                 "#### Multi-bit Pauli operation\n",
                 "Multi-bit Pauli operations define a gate with arguments as a list of target qubits and a list of Pauli operators. Since the update speed of an $n$-qubit Pauli operation has the same order as the update cost of a 1-qubit Pauli operation, Pauli's tensor product should be defined as the gate in this form. In the Pauli operator specification, 1, 2, and 3 correspond to X, Y, and Z, respectively."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** gate info *** \n",
@@ -1217,15 +1439,15 @@
             "source": [
                 "#### Multi-bit Pauli rotating operation\n",
                 "Multi-bit Pauli rotating operation rotates multi-bit Pauli operator. The multi-bit Pauli rotation becomes heavy calculation when the gate matrix is calculated greedily, but it can be updated efficiently if it is defined in this form."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** gate info *** \n",
@@ -1261,15 +1483,15 @@
             "source": [
                 "#### Reversible circuit\n",
                 "Reversible circuit performs permutation operation between basis by giving a bijective function to a total number of $2^n$ index. This is equivalent to the gate matrix being a permutation matrix. Please note that it will not work properly unless the given function is bijective."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** gate info *** \n",
@@ -1310,15 +1532,15 @@
                 "The above code moves the elements of the vector down one by one in the subspace of the qubit of interest (the bottom element moves to the top).\n",
                 "### State reflection\n",
                 "This gate is $(I-2\\ket{a}\\bra{a})$, which is defined with the quantum state $\\ket{a}$ as an argument. This corresponds to the operation of reflecting based on the quantum state $\\ket{a}$. This gate appears in Grover search. The number of qubits on which this gate operates must match the number of qubits in the quantum state given as an argument."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "axis [0.26990561+0.18885571j 0.42520294-0.30443016j 0.33036863-0.07179331j\n",
@@ -1353,15 +1575,15 @@
                 "\n",
                 "### Dense matrix gate\n",
                 "Gate defined based on a dense matrix."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** gate info *** \n",
@@ -1416,15 +1638,15 @@
             "source": [
                 "### Sparse matrix gate\n",
                 "A gate defined based on a sparse matrix. If the elements are sparse enough, they can be updated faster than a dense matrix. Define sparse matrices using scipy's `csc_matrix`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "sparse matrix   (1, 1)\t1.0\n",
@@ -1470,15 +1692,15 @@
             "source": [
                 "### Add control bit\n",
                 "General gates can add a control qubit using the `add_control_qubit` function. You can also specify whether the target qubit has an effect when control qubit is 0 or 1."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** gate info *** \n",
@@ -1531,15 +1753,15 @@
                 "## Operation to create a new gate from multiple gates\n",
                 "### Gate product\n",
                 "Combine successively the operating quantum gates to create a new single quantum gate. This reduces access to quantum states."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** gate info *** \n",
@@ -1585,15 +1807,15 @@
             "source": [
                 "### Gate sum\n",
                 "You can add multiple gates to create a new gate. This is useful for making the projection of the Pauli operator $P$ onto the +1 eigenvalue space such as $(I + P) / 2$."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** gate info *** \n",
@@ -1657,15 +1879,15 @@
             "source": [
                 "### Random unitary\n",
                 "Use the `RandomUnitary` function to sample a random unitary matrix with the Haar measure and generate a dense matrix gate."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** gate info *** \n",
@@ -1701,15 +1923,15 @@
             "source": [
                 "### Stochastic operation\n",
                 "Using the `Probabilistic` function, create the stochastic operation by giving multiple gate operations and probability distribution. If the sum of the given probability distributions is less than 1, `Identity` will operate with a probability less than 1."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** gate info *** \n",
@@ -1754,15 +1976,15 @@
             "metadata": {},
             "source": [
                 "`BitFlipNoise`, `DephasingNoise`, `IndependentXZNoise`, `DepolarizingNoise`, and `TwoQubitDepolarizingNoise` gates are defined as stochastic gates. `Probabilistic` instances are generated by entering the error probabilities."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[1.+0.j 0.+0.j 0.+0.j 0.+0.j]\n",
@@ -1811,15 +2033,15 @@
                 "    - `NoisyEvolution_fast` extracts a matrix and finds it by diagonalization.\n",
                 "\n",
                 "It is recommended to use `NoisyEvolution_fast` because `NoisyEvolution_fast` does not require specifying the time to make a small change and it is fast."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[0] exp: -0.0006155544536970823\n",
@@ -2877,15 +3099,15 @@
             "source": [
                 "### CPTP mapping\n",
                 "`CPTP` is created by giving a list of Claus operators that satisfy the completeness."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[0.+0.j 0.+0.j 1.+0.j 0.+0.j]\n",
@@ -2927,15 +3149,15 @@
             "metadata": {},
             "source": [
                 "The `AmplitudeDampingNoise` gate is defined as CPTP-map."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             " *** gate info *** \n",
                             " * gate name : Generic gate\n",
@@ -2967,15 +3189,15 @@
             "source": [
                 "### Instrument\n",
                 "Instrument is an operation to get the index of the Claus operator that acts randomly in addition to the general CPTP-map operation. For example, measurement on the Z basis is equivalent to applying a CPTP-map consisting of `P0` and `P1` and knowing which one has acted. In cppsim, this is achieved in the `Instrument` function, by specifying the information of the CPTP-map and the address of the classic register in which the index of the operated Claus operator is written."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "0 01 [0.+0.j 1.+0.j 0.+0.j 0.+0.j]\n",
@@ -3020,15 +3242,15 @@
             "metadata": {},
             "source": [
                 "Note that `Measurement` gate is defined as Instrument."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from qulacs.gate import Measurement\n",
                 "target = 0\n",
                 "classical_pos = 0\n",
                 "gate = Measurement(target, classical_pos)"
@@ -3040,15 +3262,15 @@
             "source": [
                 "### Adaptive operation\n",
                 "This is a gate that uses a function that returns a Boolean value with variable-length list of classical register values as an argument, and determines whether to perform an operation according to the conditions obtained from the classical register. Conditions can be written as python functions. A python function must be a function that takes a list of type `int` as an argument and returns a bool type value."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "func is called! content is  [0]\n",
@@ -3092,15 +3314,15 @@
                 "Observables are represented as linear combinations of Pauli operators with real coefficients. `PauliOperator` class is a class that expresses each term with the coefficient added to the $n$-qubit Pauli operator. Unlike gates, operator cannot update quantum states.\n",
                 "\n",
                 "#### Create Pauli operator and obtain state"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "(0.1+0j) X0 Y1 Z3 Y3\n"
@@ -3141,15 +3363,15 @@
             "source": [
                 "#### Expected value of Pauli operator\n",
                 "You can evaluate the expected value and transition moment of the Pauli operator for one state."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "expect (0.6132028798856664+0j)\n",
@@ -3185,15 +3407,15 @@
             "source": [
                 "### General linear operators\n",
                 "The linear operator `GeneralQuantumOperator` is represented by a linear combination of the Pauli operators with a complex coefficient. `PauliOperator` with coefficient can be added as a term with `add_operator`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "expect (-0.12123883067235244+0.004874745096201068j)\n",
@@ -3238,24 +3460,61 @@
                 "bra = QuantumState(n)\n",
                 "bra.set_Haar_random_state()\n",
                 "value = operator.get_transition_amplitude(bra, state)\n",
                 "print(\"transition\", value)"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Store linear operators\n",
+                "`GeneralQuantumOperator` can be converted to/from JSON string."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "original: (1,0) X 2 Y 0 + (0,0.5) Y 1 Z 0\n",
+                        "restored: (1,0) X 2 Y 0 + (0,0.5) Y 1 Z 0\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from qulacs import GeneralQuantumOperator\n",
+                "from qulacs import quantum_operator\n",
+                "\n",
+                "o_operator = GeneralQuantumOperator(3)\n",
+                "o_operator.add_operator(1.0, \"X 2 Y 0\")\n",
+                "o_operator.add_operator(0.5j, \"Y 1 Z 0\")\n",
+                "operator_json = o_operator.to_json()\n",
+                "print(\"original:\", o_operator)\n",
+                "\n",
+                "r_operator = quantum_operator.from_json(operator_json)\n",
+                "print(\"restored:\", r_operator)"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Generation of observables using OpenFermion\n",
                 "`OpenFermion` is a tool that gives Hamiltonian to be solved by chemical calculation in the form of Pauli operator. The output of this tool can be read in the form of a file or a string and can be used in the form of an operator."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "15\n",
@@ -3436,15 +3695,15 @@
                 "\n",
                 "### Structure of a quantum circuit\n",
                 "A quantum circuit is represented as a set of quantum gates. For example, a quantum circuit can be configured as follows."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 37,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[ 0.35355339+0.j -0.35355339-0.j -0.35355339-0.j  0.35355339+0.j\n",
@@ -3483,15 +3742,15 @@
                 "By combining quantum gates into a single quantum gate, the number of quantum gates and the time required for numerical calculations can be reduced. (Of course, if the number of target qubits increases, or if a quantum gate with a dedicated function is synthesized into a quantum gate without a dedicated function, the total calculation time may not decrease. It depends.)\n",
                 "\n",
                 "The code below uses the `optimize` function to repeat the greedy synthesis of the quantum gate of the quantum circuit until the target qubit becomes three."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 38,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "10\n",
@@ -3528,15 +3787,15 @@
             "source": [
                 "###  Debugging quantum circuits\n",
                 "When print a quantum circuit, statistical information about the gates included in the quantum circuit will be displayed."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 39,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "*** Quantum Circuit Info ***\n",
@@ -3561,27 +3820,115 @@
                 "    for i in range(n):\n",
                 "        circuit.add_H_gate(i)\n",
                 "\n",
                 "print(circuit)"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Store QuantumCircuit\n",
+                "`QuantumCircuit` can be converted to/from JSON string.\n",
+                "If it has unsupported gates, the conversion fails with an error."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "*** Quantum Circuit Info ***\n",
+                        "# of qubit: 3\n",
+                        "# of step : 2\n",
+                        "# of gate : 3\n",
+                        "# of 1 qubit gate: 2\n",
+                        "# of 2 qubit gate: 1\n",
+                        "Clifford  : no\n",
+                        "Gaussian  : no\n",
+                        "\n",
+                        "\n",
+                        "*** Quantum Circuit Info ***\n",
+                        "# of qubit: 3\n",
+                        "# of step : 2\n",
+                        "# of gate : 3\n",
+                        "# of 1 qubit gate: 2\n",
+                        "# of 2 qubit gate: 1\n",
+                        "Clifford  : no\n",
+                        "Gaussian  : no\n",
+                        "\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from qulacs import QuantumCircuit\n",
+                "from qulacs import circuit\n",
+                "\n",
+                "o_circuit = QuantumCircuit(3)\n",
+                "o_circuit.add_H_gate(0)\n",
+                "o_circuit.add_CNOT_gate(0, 1)\n",
+                "o_circuit.add_RZ_gate(2, 0.7)\n",
+                "circuit_json = o_circuit.to_json()\n",
+                "print(o_circuit)\n",
+                "\n",
+                "r_circuit = circuit.from_json(circuit_json)\n",
+                "print(r_circuit)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Quantum circuits can be stored to files in pickle format."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from qulacs import QuantumCircuit\n",
+                "import pickle\n",
+                "\n",
+                "circuit = QuantumCircuit(3)\n",
+                "circuit.add_H_gate(0)\n",
+                "circuit.add_CNOT_gate(0, 1)\n",
+                "circuit.add_RZ_gate(2, 0.7)\n",
+                "\n",
+                "# store\n",
+                "with open('circuit.pickle', 'wb') as f:\n",
+                "    pickle.dump(circuit, f)\n",
+                "\n",
+                "# load\n",
+                "with open('circuit.pickle', 'rb') as f:\n",
+                "    circuit = pickle.load(f)"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Parametric Quantum Circuits\n",
                 "Defining a quantum circuit as a `ParametricQuantumCircuit` class enables some functions that are useful for optimizing quantum circuits using variational methods, in addition to the usual functions of the `QuantumCircuit` class.\n",
                 "\n",
                 "### Application examples of parametric quantum circuits\n",
                 "Quantum gates with one rotation angle (`RX`, `RY`, `RZ`, `multi_qubit_pauli_rotation`) can be added to quantum circuits as parametric quantum gates. For a quantum gate added as a parametric gate, the number of parametric gates can be extracted after the quantum circuit is configured, and the rotation angle can be changed later."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 40,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** Quantum State ***\n",
@@ -3690,15 +4037,15 @@
                 "\n",
                 "- In `GradCalculator`, compute a gradient by calculating expected value with `CausalConeSimulator`.\n",
                 "- In `ParametricQuantumCircuit.backprop()`, compute a gradient by back propagation."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "[(0.1329240611221506+0j), (0.06968868323709176+0j), (0.14726262077628172+0j)]\n",
@@ -3726,25 +4073,120 @@
                 "# \u7b2c\u4e09\u5f15\u6570\u306b\u56de\u8ee2\u89d2\u3092\u6307\u5b9a\u3059\u308b\u3053\u3068\u3082\u53ef\u80fd\n",
                 "print(gcalc.calculate_grad(circuit, observable, theta))\n",
                 "# Backprop\u3092\u4f7f\u3063\u3066\u6c42\u3081\u305f\u5834\u5408\n",
                 "print(circuit.backprop(observable))"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Store parametric quantum circuits\n",
+                "\n",
+                "Parametric quantum circuits can be converted to/from JSON string.\n",
+                "If it has unsupported gates, the conversion fails with an error."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 3,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "*** Quantum Circuit Info ***\n",
+                        "# of qubit: 3\n",
+                        "# of step : 2\n",
+                        "# of gate : 3\n",
+                        "# of 1 qubit gate: 2\n",
+                        "# of 2 qubit gate: 0\n",
+                        "# of 3 qubit gate: 1\n",
+                        "Clifford  : no\n",
+                        "Gaussian  : no\n",
+                        "\n",
+                        "*** Parameter Info ***\n",
+                        "# of parameter: 1\n",
+                        "\n",
+                        "*** Quantum Circuit Info ***\n",
+                        "# of qubit: 3\n",
+                        "# of step : 2\n",
+                        "# of gate : 3\n",
+                        "# of 1 qubit gate: 2\n",
+                        "# of 2 qubit gate: 0\n",
+                        "# of 3 qubit gate: 1\n",
+                        "Clifford  : no\n",
+                        "Gaussian  : no\n",
+                        "\n",
+                        "*** Parameter Info ***\n",
+                        "# of parameter: 1\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from qulacs import ParametricQuantumCircuit\n",
+                "from qulacs import circuit\n",
+                "\n",
+                "o_circuit = ParametricQuantumCircuit(3)\n",
+                "o_circuit.add_H_gate(0)\n",
+                "o_circuit.add_parametric_RX_gate(1, 0.3)\n",
+                "o_circuit.add_multi_Pauli_rotation_gate([0, 1, 2], [1, 3, 2], 1.4)\n",
+                "circuit_json = o_circuit.to_json()\n",
+                "print(o_circuit)\n",
+                "\n",
+                "r_circuit = circuit.from_json(circuit_json)\n",
+                "print(r_circuit)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Parametric quantum circuits can be converted to files in pickle format."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from qulacs import ParametricQuantumCircuit\n",
+                "from qulacs import circuit\n",
+                "\n",
+                "circuit = ParametricQuantumCircuit(3)\n",
+                "circuit.add_H_gate(0)\n",
+                "circuit.add_parametric_RX_gate(1, 0.3)\n",
+                "circuit.add_multi_Pauli_rotation_gate([0, 1, 2], [1, 3, 2], 1.4)\n",
+                "\n",
+                "# store\n",
+                "with open('circuit.pickle', 'wb') as f:\n",
+                "    pickle.dump(circuit, f)\n",
+                "\n",
+                "# load\n",
+                "with open('circuit.pickle', 'rb') as f:\n",
+                "    circuit = pickle.load(f)"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Simulator\n",
                 "### `QuantumCircuitSimulator`\n",
                 "You can manage a circuit and quantum states together. It has a buffer for quantum state to swap the state to use."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "gate_count:  3\n",
@@ -3864,15 +4306,15 @@
                 "To set up noise, you should add a gate to the circuit using `add_noise_gate()`.\n",
                 "The first argument specifies the gate, the second the type of noise to add (`\"Depolarizing\"` / `\"BitFlip\"` / `\"Dephasing\"` / `\"IndependentXZ\"` / `\"AmplitudeDamping\"`), and the third the probability of noise generation.\n",
                 "In the case of a two-qubit gate, you can use `\"Depolarizing\"` only."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** Quantum State ***\n",
@@ -3934,15 +4376,15 @@
                 "Only the extracted gates can be applied to obtain the expected value of the physical quantity.\n",
                 "\n",
                 "This allows you to find the expected value of a circuit of large size qubits, since the shallower the depth of the circuit, the fewer the gates associated with it."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "(0.2919265817264289+0j)\n"
@@ -3976,15 +4418,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
                 "hash": "949777d72b0d2535278d3dc13498b2535136f6dfe0678499012e853ee9abcab1"
             }
         }
     },
```

### Comparing `qulacs-0.5.6/doc/en/source/index.md` & `qulacs-0.6.0/doc/en/source/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 ```
 
 ```{toctree}
 :maxdepth: 2
 :caption: API reference
 :hidden:
 
-pyRef/modules
+pyRef/index
 api/cpp_library_root
 ```
 
 ```{toctree}
 :maxdepth: 1
 :caption: Contributing
```

#### html2text {}

```diff
@@ -12,9 +12,9 @@
 {doc}`intro/2_faq`. For basic usage of Qulacs in Python and C++, see
 {doc}`intro/3_usage`. ```{toctree} :maxdepth: 1 :hidden: :caption: Get Started
 intro/0_about intro/1_install intro/2_faq intro/3_usage ``` ```{toctree} :
 maxdepth: 1 :caption: Tutorials intro/4.1_python_tutorial intro/
 4.2_cpp_tutorial ``` ```{toctree} :maxdepth: 2 :caption: User Manual guide/
 2.0_python_advanced ``` ```{toctree} :maxdepth: 2 :caption: Applications apply/
 0_overview ``` ```{toctree} :maxdepth: 2 :caption: API reference :hidden:
-pyRef/modules api/cpp_library_root ``` ```{toctree} :maxdepth: 1 :caption:
+pyRef/index api/cpp_library_root ``` ```{toctree} :maxdepth: 1 :caption:
 Contributing write/0_readme ```
```

### Comparing `qulacs-0.5.6/doc/en/source/intro/0_about.md` & `qulacs-0.6.0/doc/en/source/intro/0_about.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # About Qulacs
 
 Qulacs is a Python/C++ library for fast simulation of large, noisy, or parametric quantum circuits.
-Qulacs is developed at QunaSys, Osaka University, NTT and Fujitsu.
+Qulacs is developed at QunaSys, Osaka University, NTT, and Fujitsu.
 
 Qulacs is licensed under the [MIT license](https://github.com/qulacs/qulacs/blob/master/LICENSE).
 
 ## Features
 
 - Fast quantum circuit simulation with parallelized C/C++ backend
 - Noisy quantum gate for simulation of NISQ devices
```

### Comparing `qulacs-0.5.6/doc/en/source/intro/1_install.md` & `qulacs-0.6.0/doc/en/source/intro/1_install.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/source/intro/2_faq.md` & `qulacs-0.6.0/doc/en/source/intro/2_faq.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/source/intro/3_usage.md` & `qulacs-0.6.0/doc/en/source/intro/3_usage.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/source/intro/4.1_python_tutorial.ipynb` & `qulacs-0.6.0/doc/en/source/intro/4.1_python_tutorial.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9820188492063492%*

 * *Differences: {"'cells'": "{insert: [(52, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['### Obtain a inverse gate from a quantum gate\\n', '\\n', 'The hermitian "*

 * *            'conjugate `U†` of the generated quantum gate `U` can be obtained using a '*

 * *            '`get_inverse` function. The hermitian conjugate `U†` represents the inverse operation '*

 * *            'of the generated quantum gate `U`. If the hermitian conjugate function is not '*

 * *            "implemented, an e […]*

```diff
@@ -825,14 +825,58 @@
                 "print(matrix)\n",
                 "cnot_gate = CNOT(1,2)\n",
                 "matrix = cnot_gate.get_matrix()\n",
                 "print(matrix)"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Obtain a inverse gate from a quantum gate\n",
+                "\n",
+                "The hermitian conjugate `U\u2020` of the generated quantum gate `U` can be obtained using a `get_inverse` function. The hermitian conjugate `U\u2020` represents the inverse operation of the generated quantum gate `U`. If the hermitian conjugate function is not implemented, an exception is thrown."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "original:\n",
+                        " [[1.+0.j 0.+0.j]\n",
+                        " [0.+0.j 0.+1.j]]\n",
+                        "inversed:\n",
+                        " [[ 1.+0.j  0.+0.j]\n",
+                        " [ 0.+0.j -0.-1.j]]\n",
+                        "Exception occured as expected: this gate don't have get_inverse function\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from qulacs.gate import S, DepolarizingNoise\n",
+                "\n",
+                "s_gate = S(2)\n",
+                "s_dagger_gate = s_gate.get_inverse()\n",
+                "print(\"original:\\n\", s_gate.get_matrix())\n",
+                "print(\"inversed:\\n\", s_dagger_gate.get_matrix())\n",
+                "\n",
+                "noise_gate = DepolarizingNoise(0, 0.05)\n",
+                "try:\n",
+                "        noise_gate.get_inverse()\n",
+                "        assert 0, \"No exception occured. should not reach here.\"\n",
+                "except Exception as err:\n",
+                "        print(f\"Exception occured as expected: {err}\")"
+            ]
+        },
+        {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Quantum circuit"
             ]
         },
@@ -942,36 +986,88 @@
                 "circuit.add_RX_gate(2,0.1)\n",
                 "\n",
                 "from qulacs import QuantumState\n",
                 "state = QuantumState(n)\n",
                 "circuit.update_quantum_state(state)\n",
                 "print(state)"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Obtain a inverse circuit from a quantum circuit\n",
+                "\n",
+                "An inverse circuit of the quantum circuit can be obtained using a `get_inverse` function, as with the quantum gate.\n",
+                "If the quantum circuit contains quantum gates such that hermitian transpose is not implemented, an exception is thrown."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        " *** Quantum State ***\n",
+                        " * Qubit Count : 3\n",
+                        " * Dimension   : 8\n",
+                        " * State vector : \n",
+                        "(1,0)\n",
+                        "(0,0)\n",
+                        "(0,0)\n",
+                        "(0,0)\n",
+                        "(0,0)\n",
+                        "(0,0)\n",
+                        "(0,0)\n",
+                        "(0,0)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from qulacs import QuantumCircuit\n",
+                "\n",
+                "n=3\n",
+                "circuit = QuantumCircuit(n)\n",
+                "circuit.add_H_gate(1)\n",
+                "circuit.add_RX_gate(2,0.1)\n",
+                "\n",
+                "inverse_circuit = circuit.get_inverse()\n",
+                "\n",
+                "from qulacs import QuantumState\n",
+                "state = QuantumState(n)\n",
+                "circuit.update_quantum_state(state)\n",
+                "inverse_circuit.update_quantum_state(state)\n",
+                "print(state)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3.9.10 64-bit",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.4 (main, May  9 2022, 18:28:02) [GCC 9.4.0]"
+            "version": "3.9.10"
         },
         "vscode": {
             "interpreter": {
-                "hash": "84aa2c67dae1159a9469e7ac93262a46ff5158e6dcd4abab35ce17cbce36ce1e"
+                "hash": "949777d72b0d2535278d3dc13498b2535136f6dfe0678499012e853ee9abcab1"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `qulacs-0.5.6/doc/en/source/intro/4.2_cpp_tutorial.md` & `qulacs-0.6.0/doc/en/source/intro/4.2_cpp_tutorial.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/en/source/write/0_readme.md` & `qulacs-0.6.0/doc/en/source/write/0_readme.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/ja/Makefile` & `qulacs-0.6.0/doc/ja/Makefile`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/ja/make.bat` & `qulacs-0.6.0/doc/ja/make.bat`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/ja/source/_static/images/dojo.png` & `qulacs-0.6.0/doc/ja/source/_static/images/dojo.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/ja/source/_static/images/github.png` & `qulacs-0.6.0/doc/ja/source/_static/images/github.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/ja/source/_static/images/logo-c-h.png` & `qulacs-0.6.0/doc/ja/source/_static/images/logo-c-h.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/ja/source/_static/images/slack.png` & `qulacs-0.6.0/doc/ja/source/_static/images/slack.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/ja/source/conf.py` & `qulacs-0.6.0/doc/en/source/conf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,117 +1,134 @@
 import qulacs
 
 project = "Qulacs"
 
-language = 'ja'
-locale_dirs = ['locale/']
+language = "en"
+locale_dirs = ["locale/"]
 
 # The `extensions` list should already be in here from `sphinx-quickstart`
 extensions = [
     # there may be others here already, e.g. 'sphinx.ext.mathjax'
-    # there may be others here already, e.g. 'sphinx.ext.mathjax'
-    'breathe',
-    'exhale',
-    'myst_parser',
-    'nbsphinx',
-    'sphinx.ext.mathjax',
-    'sphinx_copybutton',
-    'sphinx.ext.napoleon',
-    'sphinx.ext.autodoc',
-    'sphinx.ext.graphviz',
-    'sphinx.ext.inheritance_diagram',
+    "breathe",
+    "exhale",
+    "myst_parser",
+    "nbsphinx",
+    "sphinx.ext.mathjax",
+    "sphinx_copybutton",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.graphviz",
+    "sphinx.ext.inheritance_diagram",
+    "autoapi.extension",
 ]
 
-exclude_patterns = ['_build', '**.ipynb_checkpoints']
+exclude_patterns = ["_build", "**.ipynb_checkpoints"]
 nbsphinx_allow_errors = True
 myst_enable_extensions = [
     "dollarmath",
 ]
 
-
 # source files for shpinx
 source_suffix = {
-    '.rst': 'restructuredtext',
-    '.txt': 'markdown',
-    '.md': 'markdown',
+    ".rst": "restructuredtext",
+    ".txt": "markdown",
+    ".md": "markdown",
 }
 
 # Setup the breathe extension
-breathe_projects = {
-    "Docs": "./xml"
-}
+breathe_projects = {"Docs": "./xml"}
 
 breathe_default_project = "Docs"
 
 # Setup the exhale extension
 exhale_args = {
     # These arguments are required
-    "containmentFolder":     "./api",
-    "rootFileName":          "cpp_library_root.rst",
-    "rootFileTitle":         "C++ APIリファレンス",
-    "doxygenStripFromPath":  "..",
+    "containmentFolder": "./api",
+    "rootFileName": "cpp_library_root.rst",
+    "rootFileTitle": "C++ API Reference",
+    "doxygenStripFromPath": "..",
     # Suggested optional arguments
-    "createTreeView":        True,
+    "createTreeView": True,
     # TIP: if using the sphinx-bootstrap-theme, you need
     # "treeViewIsBootstrap": True,
     "exhaleExecutesDoxygen": True,
-    "exhaleDoxygenStdin": \
-        "INPUT = ../../../src/cppsim ../../../src/vqcsim \n \
-        OUTPUT_LANGUAGE = Japanese-en \n \
+    "exhaleDoxygenStdin": "INPUT = ../../../src/cppsim ../../../src/vqcsim \n \
         FILE_PATTERNS          = *.hpp \n \
         WARN_IF_UNDOCUMENTED   = NO \n \
         ENABLE_PREPROCESSING   = YES \n \
         MACRO_EXPANSION        = YES \n \
         PREDEFINED             += __attribute__(x)= \n \
         PREDEFINED             += DllExport= \n \
+        OUTPUT_LANGUAGE = English \n \
         GENERATE_LEGEND        = YES \n \
         GRAPHICAL_HIERARCHY    = YES \n \
         CLASS_GRAPH            = YES \n \
         HIDE_UNDOC_RELATIONS   = YES\n \
-        CLASS_DIAGRAMS         = YES\n"
+        CLASS_DIAGRAMS         = YES\n",
 }
 
+autoapi_type = "python"
+autoapi_keep_files = True
+autoapi_root = "pyRef"
+# The order of `autoapi_file_patterns`` specifies the order of preference for reading files.
+# So, we give priority to `*.pyi`.
+# https://github.com/readthedocs/sphinx-autoapi/issues/243#issuecomment-684190179
+autoapi_file_patterns = ["*.pyi", "*.py"]
+autoapi_dirs = ["../../../pysrc/qulacs"]
+autoapi_add_toctree_entry = True
+autoapi_template_dir = "_templates/autoapi"
+# Avoid `maximum recursion depth exceeded while calling a Python object` error.
+autoapi_ignore = ["*/vistest/__init__.py", "*/visualizer/__init__.py"]
+autoapi_options = [
+    "members",
+    "undoc-members",
+    "show-inheritance",
+    "show-module-summary",
+    "imported-members",
+]
+
 # Tell sphinx what the primary language being documented is.
-#primary_domain = 'cpp'
+# primary_domain = 'cpp'
 
 # Tell sphinx what the pygments highlight language should be.
-#highlight_language = 'cpp'
+# highlight_language = 'cpp'
 
 #
 
 # on_rtd is whether we are on readthedocs.org, this line of code grabbed from docs.readthedocs.org
 import os
 
-on_rtd = os.environ.get('READTHEDOCS', None) == 'True'
+on_rtd = os.environ.get("READTHEDOCS", None) == "True"
 
 if not on_rtd:  # only import and set the theme if we're building docs locally
     import sphinx_rtd_theme
-    html_theme = 'sphinx_rtd_theme'
+
+    html_theme = "sphinx_rtd_theme"
     html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
 
 
 html_theme_options = {
     # 'canonical_url': '',
     # 'analytics_id': 'UA-XXXXXXX-1',  #  Provided by Google in your dashboard
-    'logo_only': False,
+    "logo_only": False,
     # 'display_version': True,
-    'prev_next_buttons_location': 'bottom',
-    'style_external_links': False,
+    "prev_next_buttons_location": "bottom",
+    "style_external_links": False,
     # 'vcs_pageview_mode': '',
-    'style_nav_header_background': '#004659',
+    "style_nav_header_background": "#004659",
     # Toc options
-    'collapse_navigation': True,
-    'sticky_navigation': True,
-    'navigation_depth': 2,
-    'includehidden': True,
-    'titles_only': False
+    "collapse_navigation": True,
+    "sticky_navigation": True,
+    "navigation_depth": 2,
+    "includehidden": True,
+    "titles_only": False,
 }
 
 templates_path = ["_templates"]
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
-copyright = '2018 Qulacs Authors'
+copyright = "2018 Qulacs Authors"
 
 # `version` is only used for local build.
 # On Read the Docs, the latest version is `latest`` and the specific version
 # is the Git tag name.
 version = qulacs._version.__version__
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qulacs-0.5.6/doc/ja/source/guide/2.0_python_advanced.md` & `qulacs-0.6.0/doc/ja/source/guide/2.0_python_advanced.md`

 * *Files 10% similar despite different names*

```diff
@@ -64,14 +64,56 @@
 initial_state = QuantumState(3)
 buffer = initial_state.allocate_buffer()
 for ind in range(10):
     buffer.load(initial_state)
     # some computation and get results
 ```
 
+### 量子状態の保存
+
+量子状態をJSON形式の文字列に変換して保存することができます。
+JSONをロードすれば量子状態を復元できます。
+
+```python
+from qulacs import QuantumState
+from qulacs import state
+
+o_state = QuantumState(2)
+o_state.set_Haar_random_state()
+print("original:", o_state.get_vector())
+state_json = o_state.to_json()
+
+r_state = state.from_json(state_json)
+print("restored:", r_state.get_vector())
+```
+
+```
+original: [ 0.28138293-0.06277525j  0.19610473-0.34365263j -0.418601  +0.64787757j
+  0.05418038-0.40301496j]
+restored: [ 0.28138293-0.06277525j  0.19610473-0.34365263j -0.418601  +0.64787757j
+  0.05418038-0.40301496j]
+```
+
+pickle形式でファイルに保存することもできます。
+
+```python
+from qulacs import QuantumState
+import pickle
+
+state = QuantumState(2)
+
+# store
+with open('state.pickle', 'wb') as f:
+    pickle.dump(state, f)
+
+# load
+with open('state.pickle', 'rb') as f:
+    state = pickle.load(f)
+```
+
 ### 量子状態の初期化
 
 下記は量子状態を特定の状態に初期化する関数です。
 
 ```python
 from qulacs import QuantumState
 
@@ -477,14 +519,67 @@
 copied_state = initial_state.copy()
 buffer = initial_state.allocate_buffer()
 buffer.load(initial_state)
 state_vector = QuantumState(3)
 buffer.load(state_vector)
 ```
 
+### 量子状態の保存
+
+`DensityMatrix` もJSON形式との変換が可能です。
+
+```python
+from qulacs import DensityMatrix
+from qulacs import state
+
+o_state = DensityMatrix(2)
+o_state.set_Haar_random_state()
+print("original:", o_state.get_matrix())
+state_json = o_state.to_json()
+
+r_state = state.from_json(state_json)
+print("restored:", r_state.get_matrix())
+```
+
+```
+original [[ 0.37583869+3.34698727e-18j -0.0327177 -4.68057147e-02j
+   0.2772076 +2.33005983e-01j -0.31619149-1.44861167e-02j]
+ [-0.0327177 +4.68057147e-02j  0.00867719+1.99864946e-19j
+  -0.05314941+1.42387692e-02j  0.02932931-3.81163955e-02j]
+ [ 0.2772076 -2.33005983e-01j -0.05314941-1.42387692e-02j
+   0.34891523+2.95031690e-19j -0.24219443+1.85342405e-01j]
+ [-0.31619149+1.44861167e-02j  0.02932931+3.81163955e-02j
+  -0.24219443-1.85342405e-01j  0.2665689 -6.89895889e-19j]]
+restored [[ 0.37583869+3.34698727e-18j -0.0327177 -4.68057147e-02j
+   0.2772076 +2.33005983e-01j -0.31619149-1.44861167e-02j]
+ [-0.0327177 +4.68057147e-02j  0.00867719+1.99864946e-19j
+  -0.05314941+1.42387692e-02j  0.02932931-3.81163955e-02j]
+ [ 0.2772076 -2.33005983e-01j -0.05314941-1.42387692e-02j
+   0.34891523+2.95031690e-19j -0.24219443+1.85342405e-01j]
+ [-0.31619149+1.44861167e-02j  0.02932931+3.81163955e-02j
+  -0.24219443-1.85342405e-01j  0.2665689 -6.89895889e-19j]]
+```
+
+pickle形式でファイルに保存することもできます。
+
+```python
+from qulacs import DensityMatrix
+import pickle
+
+state = DensityMatrix(2)
+
+# store
+with open('state.pickle', 'wb') as f:
+    pickle.dump(state, f)
+
+# load
+with open('state.pickle', 'rb') as f:
+    state = pickle.load(f)
+```
+
 ### 量子状態の初期化
 
 下記は量子状態を特定の純粋状態に初期化する関数です。
 
 ```python
 from qulacs import DensityMatrix
 
@@ -710,16 +805,14 @@
  [0. +0.j 0. +0.j 0. +0.j 0. +0.j]
  [0. +0.j 0. +0.j 0. +0.j 0. +0.j]
  [0. +0.j 0. +0.j 0. +0.j 0.5+0.j]]
 ```
 
 ## 量子ゲート
 
-### 量子ゲートに共通の操作
-
 ### 量子ゲートの種類
 
 量子ゲートは特殊ゲートと一般ゲートの二種類にわかれます。なお、Qulacsではユニタリ演算子に限らず、InstrumentやCPTP-mapをはじめとする任意の量子状態を更新する操作をゲートと呼びます。
 
 特殊ゲートは事前に指定されたゲート行列を持ち、量子ゲートに対し限定された変形しか行えないものを指します。例えば、パウリゲート、パウリでの回転ゲート、射影測定などが対応します。特殊ゲートの利点は、ゲートの特性が限定されているため量子状態の更新関数が一般ゲートに比べ効率的である点です。また、定義時に自身が各量子ビットで何らかのパウリの基底で対角化されるかの情報を保持しており、この情報は回路最適化の時に利用されます。特殊ゲートの欠点は上記の理由からゲートに対する可能な操作が限定されている点です。
 
 作用するゲート行列を露に持つゲートを一般ゲートと呼びます。一般ゲートの利点はゲート行列を好きに指定できるところですが、欠点は特殊ゲートに比べ更新が低速である点です。
@@ -751,14 +844,54 @@
  * Pauli     : yes
  * Clifford  : yes
  * Gaussian  : no
  * Parametric: no
  * Diagonal  : no
 ```
 
+量子ゲートもJSON形式との変換が可能です。
+一部、サポートされていないゲートがあります。
+サポートされていないゲートを変換しようとするとエラーが発生します。
+
+```python
+from qulacs.gate import X
+from qulacs import gate
+
+o_gate = X(2)
+print(o_gate)
+gate_json = o_gate.to_json()
+
+r_gate = gate.from_json(gate_json)
+print(r_gate)
+```
+
+```
+ *** gate info *** 
+ * gate name : X
+ * target    : 
+ 2 : commute X     
+ * control   : 
+ * Pauli     : yes
+ * Clifford  : yes
+ * Gaussian  : no
+ * Parametric: no
+ * Diagonal  : no
+
+ *** gate info *** 
+ * gate name : X
+ * target    : 
+ 2 : commute X     
+ * control   : 
+ * Pauli     : yes
+ * Clifford  : yes
+ * Gaussian  : no
+ * Parametric: no
+ * Diagonal  : no
+```
+
 ### 特殊ゲート
 
 下記に特殊ゲートを列挙します。
 
 #### 1量子ビットゲート
 
 第一引数に対象ビットの添え字を取ります。
@@ -1714,14 +1847,36 @@
 ```
 
 ```
 expect (0.01844802681960955+0.05946837146359432j)
 transition (-0.00359496979054156+0.0640782452494485j)
 ```
 
+#### 線形演算子の保存
+線形演算子もJSON形式との変換が可能です。
+
+```python
+from qulacs import GeneralQuantumOperator
+from qulacs import quantum_operator
+
+o_operator = GeneralQuantumOperator(3)
+o_operator.add_operator(1.0, "X 2 Y 0")
+o_operator.add_operator(0.5j, "Y 1 Z 0")
+operator_json = o_operator.to_json()
+print("original:", o_operator)
+
+r_operator = quantum_operator.from_json(operator_json)
+print("restored:", r_operator)
+```
+
+```
+original: (1,0) X 2 Y 0 + (0,0.5) Y 1 Z 0
+restored: (1,0) X 2 Y 0 + (0,0.5) Y 1 Z 0
+```
+
 #### OpenFermionを用いたオブザーバブルの生成
 
 OpenFermionは化学計算で解くべきハミルトニアンをパウリ演算子の表現で与えてくれるツールです。このツールの出力をファイルまたは文字列の形で読み取り、演算子の形で使用することが可能です。
 
 ``` python
 from qulacs.quantum_operator import create_quantum_operator_from_openfermion_file
 from qulacs.quantum_operator import create_quantum_operator_from_openfermion_text
@@ -1915,14 +2070,81 @@
 # of step : 10
 # of gate : 50
 # of 1 qubit gate: 50
 Clifford  : yes
 Gaussian  : no
 ```
 
+### 量子回路の保存
+量子回路もJSON形式との変換が可能です。
+サポートされていないゲートが含まれている場合エラーが発生します。
+
+```python
+from qulacs import QuantumCircuit
+from qulacs import circuit
+
+o_circuit = QuantumCircuit(3)
+o_circuit.add_H_gate(0)
+o_circuit.add_CNOT_gate(0, 1)
+o_circuit.add_RZ_gate(2, 0.7)
+circuit_json = o_circuit.to_json()
+print(o_circuit)
+
+r_circuit = circuit.from_json(circuit_json)
+print(r_circuit)
+```
+
+```
+*** Quantum Circuit Info ***
+# of qubit: 3
+# of step : 2
+# of gate : 3
+# of 1 qubit gate: 2
+# of 2 qubit gate: 0
+# of 3 qubit gate: 1
+Clifford  : no
+Gaussian  : no
+
+*** Parameter Info ***
+# of parameter: 1
+
+*** Quantum Circuit Info ***
+# of qubit: 3
+# of step : 2
+# of gate : 3
+# of 1 qubit gate: 2
+# of 2 qubit gate: 0
+# of 3 qubit gate: 1
+Clifford  : no
+Gaussian  : no
+
+*** Parameter Info ***
+# of parameter: 1
+```
+
+pickle形式でファイルに保存することもできます。
+
+```python
+from qulacs import QuantumCircuit
+import pickle
+
+circuit = QuantumCircuit(3)
+circuit.add_H_gate(0)
+circuit.add_CNOT_gate(0, 1)
+circuit.add_RZ_gate(2, 0.7)
+
+# store
+with open('circuit.pickle', 'wb') as f:
+    pickle.dump(circuit, f)
+
+# load
+with open('circuit.pickle', 'rb') as f:
+    circuit = pickle.load(f)
+```
+
 ## 変分量子回路
 
 量子回路を `ParametricQuantumCircuit` クラスとして定義すると、通常の `QuantumCircuit` クラスの関数に加え、変分法を用いて量子回路を最適化するのに便利ないくつかの関数を利用することができます。
 
 ### 変分量子回路の利用例
 
 一つの回転角を持つ量子ゲート(RX, RY, RZ, multi_qubit_pauli_rotation)はパラメトリックな量子ゲートとして量子回路に追加することができます。
@@ -2055,14 +2277,74 @@
 
 ```
 [(0.13292406112215058+0j), (0.06968868323709171+0j), (0.14726262077628174+0j)]
 [(0.13292406112215058+0j), (0.06968868323709171+0j), (0.14726262077628174+0j)]
 [0.1329240611221506, 0.06968868323709165, 0.14726262077628166]
 ```
 
+### 変分量子回路の保存
+
+変分量子回路もJSON形式との変換が可能です。
+サポートされていないゲートが含まれている場合エラーが発生します。
+
+```python
+from qulacs import ParametricQuantumCircuit
+from qulacs import circuit
+
+o_circuit = ParametricQuantumCircuit(3)
+o_circuit.add_H_gate(0)
+o_circuit.add_parametric_RX_gate(1, 0.3)
+o_circuit.add_multi_Pauli_rotation_gate([0, 1, 2], [1, 3, 2], 1.4)
+circuit_json = o_circuit.to_json()
+print(o_circuit)
+
+r_circuit = circuit.from_json(circuit_json)
+print(r_circuit)
+```
+
+```
+*** Quantum Circuit Info ***
+# of qubit: 3
+# of step : 2
+# of gate : 3
+# of 1 qubit gate: 2
+# of 2 qubit gate: 1
+Clifford  : no
+Gaussian  : no
+
+
+*** Quantum Circuit Info ***
+# of qubit: 3
+# of step : 2
+# of gate : 3
+# of 1 qubit gate: 2
+# of 2 qubit gate: 1
+Clifford  : no
+Gaussian  : no
+```
+
+pickle形式でファイルに保存することもできます。
+
+```python
+from qulacs import ParametricQuantumCircuit
+from qulacs import circuit
+
+circuit = ParametricQuantumCircuit(3)
+circuit.add_H_gate(0)
+circuit.add_parametric_RX_gate(1, 0.3)
+circuit.add_multi_Pauli_rotation_gate([0, 1, 2], [1, 3, 2], 1.4)
+
+# store
+with open('circuit.pickle', 'wb') as f:
+    pickle.dump(circuit, f)
+
+# load
+with open('circuit.pickle', 'rb') as f:
+    circuit = pickle.load(f)
+```
 ## シミュレータ
 
 ### QuantumCircuitSimulator
 
 `QuantumCircuitSimulator` を使用すると、回路と量子状態をあわせて管理することができます。
 量子状態のバッファを1つ持っており、切り替えて使用することができます。
```

### Comparing `qulacs-0.5.6/doc/ja/source/index.md` & `qulacs-0.6.0/doc/ja/source/index.md`

 * *Files 5% similar despite different names*

```diff
@@ -72,10 +72,10 @@
 ```
 
 ```{toctree}
 :maxdepth: 2
 :caption: API リファレンス
 :hidden:
 
-pyRef/modules
+pyRef/index
 api/cpp_library_root
 ```
```

#### html2text {}

```diff
@@ -9,9 +9,9 @@
 [_static/images/slack.png]_Slack_Community
 [_static/images/dojo.png]_Study_material_(Japanese)
 ## ã¤ã³ã¹ãã¼ã«æ¹æ³ ``` pip install qulacs ```
 ãã©ãã«ã·ã¥ã¼ãã£ã³ã°: {doc}`intro/2_faq`. ```{toctree} :maxdepth:
 1 :hidden: :caption: å¥é intro/0_about intro/1_install intro/2_faq intro/
 3_usage ``` ```{toctree} :maxdepth: 1 :caption: ãã¥ã¼ããªã¢ã« intro/
 4.1_python_tutorial guide/2.0_python_advanced intro/4.2_cpp_tutorial ``` ```
-{toctree} :maxdepth: 2 :caption: API ãªãã¡ã¬ã³ã¹ :hidden: pyRef/modules
+{toctree} :maxdepth: 2 :caption: API ãªãã¡ã¬ã³ã¹ :hidden: pyRef/index
 api/cpp_library_root ```
```

### Comparing `qulacs-0.5.6/doc/ja/source/intro/0_about.md` & `qulacs-0.6.0/doc/ja/source/intro/0_about.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # About Qulacs
 
 Qulacs is a Python/C++ library for fast simulation of large, noisy, or parametric quantum circuits.
-Qulacs is developed at QunaSys, Osaka University, NTT and Fujitsu.
+Qulacs is developed at QunaSys, Osaka University, NTT, and Fujitsu.
 
 Qulacs is licensed under the [MIT license](https://github.com/qulacs/qulacs/blob/master/LICENSE).
 
 ## Features
 
 - Fast quantum circuit simulation with parallelized C/C++ backend
 - Noisy quantum gate for simulation of NISQ devices
```

### Comparing `qulacs-0.5.6/doc/ja/source/intro/1_install.md` & `qulacs-0.6.0/doc/ja/source/intro/1_install.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/ja/source/intro/2_faq.md` & `qulacs-0.6.0/doc/ja/source/intro/2_faq.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/ja/source/intro/3_usage.md` & `qulacs-0.6.0/doc/ja/source/intro/3_usage.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Usage
 
 See the following documents for more detail.
 
 - {doc}`4.1_python_tutorial`
 - {doc}`4.2_cpp_tutorial`
 - {doc}`../guide/2.0_python_advanced`
-- {doc}`../pyRef/modules`
+- {doc}`../pyRef/index`
 - {doc}`../api/cpp_library_root`
 
 ## C++ Libraries
 
 Add `./<qulacs_path>/include/` to include path, and
 `./<qulacs_path>/lib/` to library path.
```

### Comparing `qulacs-0.5.6/doc/ja/source/intro/4.1_python_tutorial.md` & `qulacs-0.6.0/doc/ja/source/intro/4.1_python_tutorial.md`

 * *Files 19% similar despite different names*

```diff
@@ -440,14 +440,44 @@
 ```
 [[ 0.70710678+0.j  0.70710678+0.j]
  [ 0.70710678+0.j -0.70710678+0.j]]
 [[0.+0.j 1.+0.j]
  [1.+0.j 0.+0.j]]
 ```
 
+## 量子ゲートの逆操作の取得
+
+生成した量子ゲート `U` のエルミート共役 `U†` は `get_inverse` 関数で取得できます。エルミート共役 `U†` は量子ゲート `U` の逆操作を表現します。エルミート共役を取得する機能が実装されていない場合は例外が送出されます。
+
+```python
+from qulacs.gate import S, DepolarizingNoise
+
+s_gate = S(2)
+s_dagger_gate = s_gate.get_inverse()
+print("original:\n", s_gate.get_matrix())
+print("inversed:\n", s_dagger_gate.get_matrix())
+
+noise_gate = DepolarizingNoise(0, 0.05)
+try:
+        noise_gate.get_inverse()
+        assert 0, "No exception occured. should not reach here."
+except Exception as err:
+        print(f"Exception occured as expected: {err}")
+```
+
+```
+original:
+ [[1.+0.j 0.+0.j]
+ [0.+0.j 0.+1.j]]
+inversed:
+ [[ 1.+0.j  0.+0.j]
+ [ 0.+0.j -0.-1.j]]
+Exception occured as expected: this gate don't have get_inverse function
+```
+
 ## 量子回路
 
 ### 量子回路の生成と構成
 
 量子回路は `QuantumCircuit` クラスとして定義されています。`QuantumCircuit` クラスには `add_<gatename>_gate` としてゲートを追加するか、`add_gate` 関数を用いてゲートのインスタンスを追加できます。量子回路を `print` することで量子回路の情報が表示されます。
 
 ``` python
@@ -503,7 +533,44 @@
  (0.706223,0)
         (0,0)
 (0,0.0353406)
         (0,0)
 (0,0.0353406)
         (0,0)
 ```
+
+## 量子回路の逆操作の取得
+
+量子回路も量子ゲートと同様にして逆操作を取得することができます。
+量子回路の中にエルミート共役を取得する機能が実装されていない量子ゲートが含まれている場合は例外が送出されます。
+
+```python
+from qulacs import QuantumCircuit
+
+n=3
+circuit = QuantumCircuit(n)
+circuit.add_H_gate(1)
+circuit.add_RX_gate(2,0.1)
+
+inverse_circuit = circuit.get_inverse()
+
+from qulacs import QuantumState
+state = QuantumState(n)
+circuit.update_quantum_state(state)
+inverse_circuit.update_quantum_state(state)
+print(state)
+```
+
+```
+ *** Quantum State ***
+ * Qubit Count : 3
+ * Dimension   : 8
+ * State vector : 
+(1,0)
+(0,0)
+(0,0)
+(0,0)
+(0,0)
+(0,0)
+(0,0)
+(0,0)
+```
```

### Comparing `qulacs-0.5.6/doc/ja/source/intro/4.2_cpp_tutorial.md` & `qulacs-0.6.0/doc/ja/source/intro/4.2_cpp_tutorial.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/scripts/customdoxygen.css` & `qulacs-0.6.0/doc/scripts/customdoxygen.css`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/scripts/doxy-boot.js` & `qulacs-0.6.0/doc/scripts/doxy-boot.js`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/scripts/footer.html` & `qulacs-0.6.0/doc/scripts/footer.html`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/scripts/header.html` & `qulacs-0.6.0/doc/scripts/header.html`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/doc/scripts/index.html` & `qulacs-0.6.0/doc/scripts/index.html`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/pyproject.toml` & `qulacs-0.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -52,22 +52,23 @@
 ci = [
     "openfermion",
     "mypy",
     "pybind11-stubgen"
 ]
 
 doc = [
-    "sphinx",
-    "sphinx-rtd-theme",
-    "breathe",
-    "exhale",
-    "nbsphinx",
-    "myst-parser",
-    "sphinx-copybutton",
-    "ipykernel",
+    "sphinx == 4.5.0",
+    "sphinx-rtd-theme == 1.0.*",
+    "breathe == 4.33.*",
+    "exhale == 0.3.*",
+    "nbsphinx == 0.8.*",
+    "myst-parser == 0.18.*",
+    "sphinx-copybutton == 0.5.*",
+    "ipykernel == 6.17.*",
+    "sphinx-autoapi == 2.0.*"
 ]
 
 [tool.setuptools]
 include-package-data = true
 zip-safe = false
 
 [tool.cibuildwheel]
```

### Comparing `qulacs-0.5.6/pysrc/qulacs/__init__.pyi` & `qulacs-0.6.0/pysrc/qulacs/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     "QuantumGate_CPTP",
     "QuantumGate_Probabilistic",
     "QuantumGate_SingleParameter",
     "QuantumState",
     "QuantumStateBase",
     "SimulationResult",
     "StateVector",
+    "check_build_for_mpi",
     "circuit",
     "gate",
     "observable",
     "quantum_operator",
     "state",
     "to_general_quantum_operator"
 ]
@@ -375,14 +376,18 @@
         """
         Add CNOT gate
         """
     def add_CZ_gate(self, control: int, target: int) -> None: 
         """
         Add CNOT gate
         """
+    def add_FusedSWAP_gate(self, target1: int, target2: int, block_size: int) -> None: 
+        """
+        Add FusedSWAP gate
+        """
     def add_H_gate(self, index: int) -> None: 
         """
         Add Hadamard gate
         """
     def add_P0_gate(self, index: int) -> None: 
         """
         Add projection gate to |0> subspace
@@ -820,18 +825,21 @@
     def set_parameter_value(self, value: float) -> None: 
         """
         Set parameter value
         """
     pass
 class QuantumState(QuantumStateBase):
     def __getstate__(self) -> str: ...
+    @typing.overload
     def __init__(self, qubit_count: int) -> None: 
         """
         Constructor
         """
+    @typing.overload
+    def __init__(self, qubit_count: int, use_multi_cpu: bool) -> None: ...
     def __setstate__(self, arg0: str) -> None: ...
     def __str__(self) -> str: 
         """
         to string
         """
     def add_state(self, state: QuantumStateBase) -> None: 
         """
@@ -1056,9 +1064,11 @@
         get state
         """
     pass
 def StateVector(arg0: int) -> QuantumState:
     """
     StateVector
     """
+def check_build_for_mpi() -> bool:
+    pass
 def to_general_quantum_operator(gate: QuantumGateBase, qubits: int, tol: float) -> GeneralQuantumOperator:
     pass
```

### Comparing `qulacs-0.5.6/pysrc/qulacs/circuit/__init__.pyi` & `qulacs-0.6.0/pysrc/qulacs/circuit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/pysrc/qulacs/converter/qasm_converter.py` & `qulacs-0.6.0/pysrc/qulacs/converter/qasm_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
         if it.get_name() == "CNOT":
             out_strs.append(f"cx q[{clis[0]}],q[{tlis[0]}];")
         elif it.get_name() == "CZ":
             out_strs.append(f"cz q[{clis[0]}],q[{tlis[0]}];")
         elif it.get_name() == "SWAP":
             out_strs.append(f"swap q[{tlis[0]}],q[{tlis[1]}];")
+        elif it.get_name() == "FusedSWAP":
+            print("# FusedSWAP is not supported yet")
         elif it.get_name() == "Identity" or it.get_name() == "I":
             out_strs.append(f"id q[{tlis[0]}];")
         elif it.get_name() == "X":
             out_strs.append(f"x q[{tlis[0]}];")
         elif it.get_name() == "Y":
             out_strs.append(f"y q[{tlis[0]}];")
         elif it.get_name() == "Z":
```

### Comparing `qulacs-0.5.6/pysrc/qulacs/gate/__init__.pyi` & `qulacs-0.6.0/pysrc/qulacs/gate/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "CPTP",
     "CZ",
     "DenseMatrix",
     "DephasingNoise",
     "DepolarizingNoise",
     "DiagonalMatrix",
     "FREDKIN",
+    "FusedSWAP",
     "H",
     "Identity",
     "IndependentXZNoise",
     "Instrument",
     "Measurement",
     "NoisyEvolution",
     "NoisyEvolution_fast",
@@ -125,14 +126,18 @@
     """
     Create diagonal matrix gate
     """
 def FREDKIN(control: int, target1: int, target2: int) -> qulacs_core.QuantumGateMatrix:
     """
     Create FREDKIN gate
     """
+def FusedSWAP(target1: int, target2: int, block_size: int) -> ClsNpairQubitGate:
+    """
+    Create FusedSWAP gate
+    """
 def H(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create Hadamard gate
     """
 def Identity(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create identity gate
```

### Comparing `qulacs-0.5.6/pysrc/qulacs/gate.pyi` & `qulacs-0.6.0/pysrc/qulacs/gate.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 def DenseMatrix(index: int, matrix: numpy.ndarray[numpy.complex128[m,n]]) -> qulacs_core.QuantumGateMatrix: ...
 @overload
 def DenseMatrix(index_list: List[int], matrix: numpy.ndarray[numpy.complex128[m,n]]) -> qulacs_core.QuantumGateMatrix: ...
 def DephasingNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic: ...
 def DepolarizingNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic: ...
 def DiagonalMatrix(index_list: List[int], diagonal_element: numpy.ndarray[numpy.complex128[m,1]]) -> qulacs_core.QuantumGateDiagonalMatrix: ...
 def FREDKIN(control: int, target1: int, target2: int) -> qulacs_core.QuantumGateMatrix: ...
+def FusedSWAP(target1: int, target2: int, block_size: int) -> ClsNpairQubitGate: ...
 def H(index: int) -> qulacs_core.ClsOneQubitGate: ...
 def Identity(index: int) -> qulacs_core.ClsOneQubitGate: ...
 def IndependentXZNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic: ...
 def Instrument(kraus_list: List[qulacs_core.QuantumGateBase], register: int) -> qulacs_core.QuantumGateBase: ...
 def Measurement(index: int, register: int) -> qulacs_core.QuantumGate_CPTP: ...
 def NoisyEvolution(hamiltonian: qulacs_core.Observable, c_ops: List[qulacs_core.GeneralQuantumOperator], time: float, dt: float) -> qulacs_core.ClsNoisyEvolution: ...
 def NoisyEvolution_fast(hamiltonian: qulacs_core.Observable, c_ops: List[qulacs_core.GeneralQuantumOperator], time: float) -> qulacs_core.ClsNoisyEvolution_fast: ...
```

### Comparing `qulacs-0.5.6/pysrc/qulacs/observable/__init__.pyi` & `qulacs-0.6.0/pysrc/qulacs/observable/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/pysrc/qulacs/observable/_get_matrix.py` & `qulacs-0.6.0/pysrc/qulacs/observable/_get_matrix.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/pysrc/qulacs/quantum_operator/__init__.pyi` & `qulacs-0.6.0/pysrc/qulacs/quantum_operator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/pysrc/qulacs/state/__init__.pyi` & `qulacs-0.6.0/pysrc/qulacs/state/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/pysrc/qulacs/state.pyi` & `qulacs-0.6.0/pysrc/qulacs/state.pyi`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/pysrc/qulacs/utils/conversions_openfermion.py` & `qulacs-0.6.0/pysrc/qulacs/utils/conversions_openfermion.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/pysrc/qulacs/vistest/test_vis.py` & `qulacs-0.6.0/pysrc/qulacs/vistest/test_vis.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/pysrc/qulacs/visualizer/visualizer.py` & `qulacs-0.6.0/pysrc/qulacs/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/pysrc/qulacs.egg-info/PKG-INFO` & `qulacs-0.6.0/pysrc/qulacs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qulacs
-Version: 0.5.6
+Version: 0.6.0
 Summary: Quantum circuit simulator for research
 Author-email: QunaSys <qulacs@qunasys.com>
 License: MIT License
         
         Copyright (c) 2018 Qulacs Authors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,15 +48,15 @@
 [![macOS CI](https://github.com/qulacs/qulacs/actions/workflows/ci_macos.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/ci_macos.yml)
 [![Windows CI](https://github.com/qulacs/qulacs/actions/workflows/ci_windows.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/ci_windows.yml)
 [![Wheel build](https://github.com/qulacs/qulacs/actions/workflows/wheel.yml/badge.svg)](https://github.com/qulacs/qulacs/actions/workflows/wheel.yml)
 [![Downloads](https://pepy.tech/badge/qulacs)](https://pepy.tech/project/qulacs)
 
 
 Qulacs is a Python/C++ library for fast simulation of large, noisy, or parametric quantum circuits.
-Qulacs is developed at QunaSys, Osaka University, NTT and Fujitsu.
+Qulacs is developed at QunaSys, Osaka University, NTT, and Fujitsu.
 
 Qulacs is licensed under the [MIT license](https://github.com/qulacs/qulacs/blob/master/LICENSE).
 
 ## Quick Install for Python
 
 ```
 pip install qulacs
```

### Comparing `qulacs-0.5.6/pysrc/qulacs.egg-info/SOURCES.txt` & `qulacs-0.6.0/pysrc/qulacs.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,87 +1,111 @@
 .clang-format
 .gitignore
+.readthedocs.yaml
 CMakeLists.txt
 CONTRIBUTING.md
 LICENSE
 README.md
+README_MPI.md
 _config.yml
 pyproject.toml
 setup.py
-.devcontainer/Dockerfile
-.devcontainer/devcontainer.json
-.github/workflows/build_devcontainer_image.yml
+.devcontainer/cpu/Dockerfile
+.devcontainer/cpu/devcontainer.json
+.devcontainer/gpu/Dockerfile
+.devcontainer/gpu/devcontainer.json
 .github/workflows/ci_macos.yml
 .github/workflows/ci_ubuntu.yml
 .github/workflows/ci_windows.yml
 .github/workflows/wheel.yml
 .vscode/tasks.json
 benchmark/AdaptiveGate.py
 benchmark/CMakeLists.txt
+benchmark/bench_circuit.py
 benchmark/benchmark2.txt
 benchmark/causalconetest.cpp
 benchmark/libcppsim_benchmark.cpp
 benchmark/libcsim_benchmark.cpp
 benchmark/merge_circuit.py
 benchmark/test_qulacs_1.py
 benchmark/test_qulacs_2.py
+benchmark/circuits/__init__.py
+benchmark/circuits/quantumvolume.py
+benchmark/circuits/qulacsbench.py
 cmake_script/FetchContent.cmake
 cmake_script/FindAVX2.cmake
 cmake_script/FindSVE.cmake
 cmake_script/FetchContent/CMakeLists.cmake.in
 doc/.gitignore
 doc/README.md
-doc/requirements.txt
 doc/en/Makefile
 doc/en/make.bat
 doc/en/source/conf.py
 doc/en/source/index.md
 doc/en/source/_static/images/dojo.png
 doc/en/source/_static/images/github.png
 doc/en/source/_static/images/logo-c-h.png
 doc/en/source/_static/images/slack.png
 doc/en/source/_templates/footer.html
+doc/en/source/_templates/autoapi/index.rst
+doc/en/source/_templates/autoapi/macros.rst
+doc/en/source/_templates/autoapi/python/attribute.rst
+doc/en/source/_templates/autoapi/python/class.rst
+doc/en/source/_templates/autoapi/python/data.rst
+doc/en/source/_templates/autoapi/python/exception.rst
+doc/en/source/_templates/autoapi/python/function.rst
+doc/en/source/_templates/autoapi/python/method.rst
+doc/en/source/_templates/autoapi/python/module.rst
+doc/en/source/_templates/autoapi/python/package.rst
+doc/en/source/_templates/autoapi/python/property.rst
 doc/en/source/apply/0_overview.ipynb
 doc/en/source/apply/5.2_qcl.ipynb
 doc/en/source/apply/6.2_vqe.ipynb
 doc/en/source/apply/6.3_ssvqe.ipynb
 doc/en/source/apply/img/QCL.png
 doc/en/source/guide/2.0_python_advanced.ipynb
 doc/en/source/intro/0_about.md
 doc/en/source/intro/1_install.md
 doc/en/source/intro/2_faq.md
 doc/en/source/intro/3_usage.md
 doc/en/source/intro/4.1_python_tutorial.ipynb
 doc/en/source/intro/4.2_cpp_tutorial.md
-doc/en/source/pyRef/modules.rst
 doc/en/source/write/0_readme.md
 doc/ja/Makefile
 doc/ja/make.bat
 doc/ja/source/conf.py
 doc/ja/source/index.md
 doc/ja/source/_static/images/dojo.png
 doc/ja/source/_static/images/github.png
 doc/ja/source/_static/images/logo-c-h.png
 doc/ja/source/_static/images/slack.png
 doc/ja/source/_templates/footer.html
+doc/ja/source/_templates/autoapi/index.rst
+doc/ja/source/_templates/autoapi/macros.rst
+doc/ja/source/_templates/autoapi/python/attribute.rst
+doc/ja/source/_templates/autoapi/python/class.rst
+doc/ja/source/_templates/autoapi/python/data.rst
+doc/ja/source/_templates/autoapi/python/exception.rst
+doc/ja/source/_templates/autoapi/python/function.rst
+doc/ja/source/_templates/autoapi/python/method.rst
+doc/ja/source/_templates/autoapi/python/module.rst
+doc/ja/source/_templates/autoapi/python/package.rst
+doc/ja/source/_templates/autoapi/python/property.rst
 doc/ja/source/guide/2.0_python_advanced.md
 doc/ja/source/intro/0_about.md
 doc/ja/source/intro/1_install.md
 doc/ja/source/intro/2_faq.md
 doc/ja/source/intro/3_usage.md
 doc/ja/source/intro/4.1_python_tutorial.md
 doc/ja/source/intro/4.2_cpp_tutorial.md
-doc/ja/source/pyRef/modules.rst
 doc/scripts/customdoxygen.css
 doc/scripts/doxy-boot.js
 doc/scripts/footer.html
 doc/scripts/header.html
 doc/scripts/index.html
-docker/cpu/Dockerfile
-docker/gpu/Dockerfile
 pysrc/qulacs/__init__.py
 pysrc/qulacs/__init__.pyi
 pysrc/qulacs/_version.py
 pysrc/qulacs/circuit.pyi
 pysrc/qulacs/gate.pyi
 pysrc/qulacs/observable.pyi
 pysrc/qulacs/py.typed
@@ -117,18 +141,20 @@
 pysrc/qulacs/vistest/test_vis.py
 pysrc/qulacs/visualizer/__init__.py
 pysrc/qulacs/visualizer/visualizer.py
 python/CMakeLists.txt
 python/cppsim_wrapper.cpp
 python/stub-test/generate_mypy_tester.py
 python/test/test_qulacs.py
+python/test/test_qulacs_multicpu.py
 script/build_clang.sh
 script/build_gcc.sh
 script/build_gcc_with_gpu.sh
 script/build_gcc_with_memory_sanitizer.sh
+script/build_mpicc.sh
 script/build_msvc_2015.bat
 script/build_msvc_2015_with_gpu.bat
 script/build_msvc_2017.bat
 script/build_msvc_2017_with_gpu.bat
 script/build_msvc_2019.bat
 script/build_msvc_2019_with_gpu.bat
 script/clean.sh
@@ -158,14 +184,15 @@
 src/cppsim/gate_matrix.hpp
 src/cppsim/gate_matrix_diagonal.cpp
 src/cppsim/gate_matrix_diagonal.hpp
 src/cppsim/gate_matrix_sparse.cpp
 src/cppsim/gate_matrix_sparse.hpp
 src/cppsim/gate_merge.cpp
 src/cppsim/gate_merge.hpp
+src/cppsim/gate_named_npair.hpp
 src/cppsim/gate_named_one.cpp
 src/cppsim/gate_named_one.hpp
 src/cppsim/gate_named_pauli.hpp
 src/cppsim/gate_named_two.hpp
 src/cppsim/gate_noisy_evolution.cpp
 src/cppsim/gate_noisy_evolution.hpp
 src/cppsim/gate_reflect.hpp
@@ -190,14 +217,16 @@
 src/cppsim/state_dm.hpp
 src/cppsim/state_gpu.cpp
 src/cppsim/state_gpu.hpp
 src/cppsim/type.hpp
 src/cppsim/utility.cpp
 src/cppsim/utility.hpp
 src/csim/CMakeLists.txt
+src/csim/MPIutil.cpp
+src/csim/MPIutil.hpp
 src/csim/constant.cpp
 src/csim/constant.hpp
 src/csim/init_ops.hpp
 src/csim/init_ops_fill.cpp
 src/csim/init_ops_random.cpp
 src/csim/memory_ops.cpp
 src/csim/memory_ops.hpp
@@ -226,14 +255,15 @@
 src/csim/update_ops_matrix_dense_single.cpp
 src/csim/update_ops_matrix_diagonal_multi.cpp
 src/csim/update_ops_matrix_diagonal_single.cpp
 src/csim/update_ops_matrix_phase_single.cpp
 src/csim/update_ops_named.cpp
 src/csim/update_ops_named_CNOT.cpp
 src/csim/update_ops_named_CZ.cpp
+src/csim/update_ops_named_FusedSWAP.cpp
 src/csim/update_ops_named_H.cpp
 src/csim/update_ops_named_SWAP.cpp
 src/csim/update_ops_named_X.cpp
 src/csim/update_ops_named_Y.cpp
 src/csim/update_ops_named_Z.cpp
 src/csim/update_ops_named_projection.cpp
 src/csim/update_ops_named_state.cpp
@@ -285,29 +315,36 @@
 src/vqcsim/parametric_simulator.hpp
 src/vqcsim/parser.hpp
 src/vqcsim/problem.hpp
 src/vqcsim/solver.hpp
 test/CMakeLists.txt
 test/cppsim/CMakeLists.txt
 test/cppsim/H2.txt
+test/cppsim/main.cpp
 test/cppsim/test_KAK.cpp
 test/cppsim/test_circuit.cpp
+test/cppsim/test_circuit_multicpu.cpp
 test/cppsim/test_circuit_optimize_light.cpp
 test/cppsim/test_gate.cpp
 test/cppsim/test_gate_dm.cpp
+test/cppsim/test_gate_multicpu.cpp
 test/cppsim/test_hamiltonian.cpp
 test/cppsim/test_hamiltonian_dm.cpp
+test/cppsim/test_hamiltonian_multicpu.cpp
+test/cppsim/test_mpiutil_multicpu.cpp
 test/cppsim/test_noise_dm.cpp
 test/cppsim/test_noisesimulator.cpp
 test/cppsim/test_noisyevolution.cpp
 test/cppsim/test_pauli_operator.cpp
 test/cppsim/test_simulator.cpp
 test/cppsim/test_state.cpp
 test/cppsim/test_state_dm.cpp
+test/cppsim/test_state_multicpu.cpp
 test/csim/CMakeLists.txt
+test/csim/main.cpp
 test/csim/test_memory.cpp
 test/csim/test_omputil.cpp
 test/csim/test_stat.cpp
 test/csim/test_update_control.cpp
 test/csim/test_update_dense.cpp
 test/csim/test_update_dense_double.cpp
 test/csim/test_update_diagonal.cpp
@@ -326,9 +363,10 @@
 test/gpusim/test_update_dense.cpp
 test/gpusim/test_update_diagonal.cpp
 test/gpusim/test_update_named.cpp
 test/gpusim/test_update_pauli.cpp
 test/gpusim/test_util.hpp
 test/util/util.hpp
 test/vqcsim/CMakeLists.txt
+test/vqcsim/main.cpp
 test/vqcsim/test.cpp
 test/vqcsim/test_backprop.cpp
```

### Comparing `qulacs-0.5.6/python/CMakeLists.txt` & `qulacs-0.6.0/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/python/cppsim_wrapper.cpp` & `qulacs-0.6.0/python/cppsim_wrapper.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -330,14 +330,16 @@
         },
         py::return_value_policy::take_ownership, "from json string",
         py::arg("json"));
 
     py::class_<QuantumStateBase>(m, "QuantumStateBase");
     py::class_<QuantumState, QuantumStateBase>(m, "QuantumState")
         .def(py::init<UINT>(), "Constructor", py::arg("qubit_count"))
+        .def(py::init<UINT, bool>(), py::arg("qubit_count"),
+            py::arg("use_multi_cpu"))
         .def(
             "set_zero_state", &QuantumState::set_zero_state, "Set state to |0>")
         .def("set_computational_basis", &QuantumState::set_computational_basis,
             "Set state to computational basis", py::arg("comp_basis"))
         .def("set_Haar_random_state",
             py::overload_cast<>(&QuantumState::set_Haar_random_state),
             "Set Haar random state")
@@ -522,14 +524,20 @@
             },
             [](std::string json) -> DensityMatrix* {
                 return static_cast<DensityMatrix*>(
                     state::from_ptree(ptree::from_json(json)));
             }));
     ;
 
+#ifdef _USE_MPI
+    m.def("check_build_for_mpi", []() { return true; });
+#else
+    m.def("check_build_for_mpi", []() { return false; });
+#endif
+
 #ifdef _USE_GPU
     py::class_<QuantumStateGpu, QuantumStateBase>(m, "QuantumStateGpu")
         .def(py::init<UINT>(), "Constructor", py::arg("qubit_count"))
         .def(py::init<UINT, UINT>(), py::arg("qubit_count"),
             py::arg("device_number"))
         .def("set_zero_state", &QuantumStateGpu::set_zero_state,
             "Set state to |0>")
@@ -833,14 +841,17 @@
 
     mgate.def("CNOT", &gate::CNOT, py::return_value_policy::take_ownership,
         "Create CNOT gate", py::arg("control"), py::arg("target"));
     mgate.def("CZ", &gate::CZ, py::return_value_policy::take_ownership,
         "Create CZ gate", py::arg("control"), py::arg("target"));
     mgate.def("SWAP", &gate::SWAP, py::return_value_policy::take_ownership,
         "Create SWAP gate", py::arg("target1"), py::arg("target2"));
+    mgate.def("FusedSWAP", &gate::FusedSWAP,
+        py::return_value_policy::take_ownership, "Create FusedSWAP gate",
+        py::arg("target1"), py::arg("target2"), py::arg("block_size"));
 
     mgate.def(
         "TOFFOLI",
         [](UINT control_index1, UINT control_index2,
             UINT target_index) -> QuantumGateMatrix* {
             auto ptr = gate::X(target_index);
             auto toffoli = gate::to_matrix_gate(ptr);
@@ -1142,14 +1153,24 @@
             (void (QuantumCircuit::*)(QuantumStateBase*)) &
                 QuantumCircuit::update_quantum_state,
             "Update quantum state", py::arg("state"))
         .def("update_quantum_state",
             (void (QuantumCircuit::*)(QuantumStateBase*, UINT, UINT)) &
                 QuantumCircuit::update_quantum_state,
             py::arg("state"), py::arg("start"), py::arg("end"))
+#if 0  // not supported yet
+        .def("update_quantum_state",
+            (void (QuantumCircuit::*)(QuantumStateBase*, UINT)) &
+                QuantumCircuit::update_quantum_state,
+            py::arg("state"), py::arg("seed"))
+        .def("update_quantum_state",
+            (void (QuantumCircuit::*)(QuantumStateBase*, UINT, UINT, UINT)) &
+                QuantumCircuit::update_quantum_state,
+            py::arg("state"), py::arg("start"), py::arg("end"), py::arg("seed"))
+#endif
         .def("calculate_depth", &QuantumCircuit::calculate_depth,
             "Calculate depth of circuit")
         .def("to_string", &QuantumCircuit::to_string,
             "Get string representation")
 
         .def("add_X_gate", &QuantumCircuit::add_X_gate, "Add Pauli-X gate",
             py::arg("index"))
@@ -1182,14 +1203,17 @@
 
         .def("add_CNOT_gate", &QuantumCircuit::add_CNOT_gate, "Add CNOT gate",
             py::arg("control"), py::arg("target"))
         .def("add_CZ_gate", &QuantumCircuit::add_CZ_gate, "Add CNOT gate",
             py::arg("control"), py::arg("target"))
         .def("add_SWAP_gate", &QuantumCircuit::add_SWAP_gate, "Add SWAP gate",
             py::arg("target1"), py::arg("target2"))
+        .def("add_FusedSWAP_gate", &QuantumCircuit::add_FusedSWAP_gate,
+            "Add FusedSWAP gate", py::arg("target1"), py::arg("target2"),
+            py::arg("block_size"))
 
         .def("add_RX_gate", &QuantumCircuit::add_RX_gate,
             "Add Pauli-X rotation gate", py::arg("index"), py::arg("angle"))
         .def("add_RY_gate", &QuantumCircuit::add_RY_gate,
             "Add Pauli-Y rotation gate", py::arg("index"), py::arg("angle"))
         .def("add_RZ_gate", &QuantumCircuit::add_RZ_gate,
             "Add Pauli-Z rotation gate", py::arg("index"), py::arg("angle"))
```

### Comparing `qulacs-0.5.6/python/stub-test/generate_mypy_tester.py` & `qulacs-0.6.0/python/stub-test/generate_mypy_tester.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/python/test/test_qulacs.py` & `qulacs-0.6.0/python/test/test_qulacs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 import sys
 import unittest
 import warnings
 
 import numpy as np
 
 import qulacs
+if qulacs.check_build_for_mpi():
+    from mpi4py import MPI
+    mpicomm = MPI.COMM_WORLD
+    if mpicomm.Get_rank() == 0:
+        print("Test with MPI. size=", mpicomm.Get_size())
 
 for ind in range(1, len(sys.argv)):
     sys.path.append(sys.argv[ind])
 sys.argv = sys.argv[:1]
 
 
 class TestQuantumState(unittest.TestCase):
```

### Comparing `qulacs-0.5.6/script/build_gcc.sh` & `qulacs-0.6.0/script/build_gcc.sh`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 #!/bin/sh
 
 set -eux
 
 GCC_COMMAND=${C_COMPILER:-"gcc"}
 GXX_COMMAND=${CXX_COMPILER:-"g++"}
 
+USE_TEST=${USE_TEST:-"No"}
+USE_GPU=${USE_GPU:-"No"}
+USE_MPI=${USE_MPI:-"No"}
+COVERAGE=${COVERAGE:-"No"}
+
+CMAKE_OPS="-D CMAKE_C_COMPILER=$GCC_COMMAND -D CMAKE_CXX_COMPILER=$GXX_COMMAND -D CMAKE_BUILD_TYPE=Release"
+CMAKE_OPS="${CMAKE_OPS} -D USE_MPI=${USE_MPI} -D USE_GPU=${USE_GPU}"
+CMAKE_OPS="${CMAKE_OPS} -D USE_TEST=${USE_TEST} -D COVERAGE=${COVERAGE}"
+
 mkdir -p ./build
 cd ./build
 if [ "${QULACS_OPT_FLAGS:-"__UNSET__"}" = "__UNSET__" ]; then
-  cmake -G "Unix Makefiles" -D CMAKE_C_COMPILER=$GCC_COMMAND -D CMAKE_CXX_COMPILER=$GXX_COMMAND -D CMAKE_BUILD_TYPE=Release -D USE_GPU:STR=No -D USE_TEST="${USE_TEST:-No}" -D COVERAGE="${COVERAGE:-No}" ..
+  cmake -G "Unix Makefiles" ${CMAKE_OPS} ..
 else
-  cmake -G "Unix Makefiles" -D CMAKE_C_COMPILER=$GCC_COMMAND -D CMAKE_CXX_COMPILER=$GXX_COMMAND -D OPT_FLAGS="${QULACS_OPT_FLAGS}" -D CMAKE_BUILD_TYPE=Release -D USE_GPU:STR=No -D USE_TEST="${USE_TEST:-No}" -D COVERAGE="${COVERAGE:-No}" ..
+  cmake -G "Unix Makefiles" ${CMAKE_OPS} -D OPT_FLAGS="${QULACS_OPT_FLAGS}" ..
 fi
 make -j $(nproc)
 cd ../
```

### Comparing `qulacs-0.5.6/script/download_wheel.sh` & `qulacs-0.6.0/script/download_wheel.sh`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/setup.py` & `qulacs-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 
         if os.getenv("USE_GPU"):
             cmake_args += ["-DUSE_GPU:STR=" + os.getenv("USE_GPU")]
 
         if os.getenv("USE_OMP"):
             cmake_args += ["-DUSE_OMP:STR=" + os.getenv("USE_OMP")]
 
+        if os.getenv("USE_MPI"):
+            cmake_args += ["-DUSE_MPI:STR=" + os.getenv("USE_MPI")]
+
         env = os.environ.copy()
         env["CXXFLAGS"] = '{} -DVERSION_INFO=\\"{}\\"'.format(
             env.get("CXXFLAGS", ""), self.distribution.get_version()
         )
         if not os.path.exists(self.build_temp):
             os.makedirs(self.build_temp)
 
@@ -113,14 +116,17 @@
                     + ", ".join(e.name for e in self.extensions)
                 )
 
             cmake_args += ["-DCMAKE_C_COMPILER=" + gcc]
             cmake_args += ["-DCMAKE_CXX_COMPILER=" + gxx]
             cmake_args += ["-DCMAKE_BUILD_TYPE=" + cfg]
 
+            if gcc == "mpicc":
+                cmake_args += ["-DUSE_MPI:STR=Yes"]
+
             if platform.system() == "Darwin":
                 # This is for building Python package on GitHub Actions, whose architecture is x86_64.
                 # Without specifying the architecture explicitly, binaries for arm64 is built for x86_64 while cibuildwheel intends to build for arm64.
                 archs = re.findall(r"-arch (\S+)", os.environ.get("ARCHFLAGS", ""))
                 if len(archs) > 0:
                     cmake_args += ["-DCMAKE_OSX_ARCHITECTURES={}".format(";".join(archs))]
```

### Comparing `qulacs-0.5.6/src/cppsim/CMakeLists.txt` & `qulacs-0.6.0/src/cppsim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/circuit.cpp` & `qulacs-0.6.0/src/cppsim/circuit.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -350,14 +350,18 @@
 }
 void QuantumCircuit::add_CZ_gate(UINT control_index, UINT target_index) {
     this->add_gate(gate::CZ(control_index, target_index));
 }
 void QuantumCircuit::add_SWAP_gate(UINT target_index1, UINT target_index2) {
     this->add_gate(gate::SWAP(target_index1, target_index2));
 }
+void QuantumCircuit::add_FusedSWAP_gate(
+    UINT target_index1, UINT target_index2, UINT block_size) {
+    this->add_gate(gate::FusedSWAP(target_index1, target_index2, block_size));
+}
 void QuantumCircuit::add_RX_gate(UINT target_index, double angle) {
     this->add_gate(gate::RX(target_index, angle));
 }
 void QuantumCircuit::add_RY_gate(UINT target_index, double angle) {
     this->add_gate(gate::RY(target_index, angle));
 }
 void QuantumCircuit::add_RZ_gate(UINT target_index, double angle) {
@@ -527,8 +531,8 @@
     for (const boost::property_tree::ptree::value_type& gate_pair :
         pt.get_child("gate_list")) {
         QuantumGateBase* gate = gate::from_ptree(gate_pair.second);
         circuit->add_gate(gate);
     }
     return circuit;
 }
-}  // namespace circuit
+}  // namespace circuit
```

### Comparing `qulacs-0.5.6/src/cppsim/circuit.hpp` & `qulacs-0.6.0/src/cppsim/circuit.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -337,14 +337,24 @@
      *
      * @param[in] target_index1 作用するtarget qubitの添え字
      * @param[in] target_index2 作用するもう一方のtarget qubitの添え字
      */
     virtual void add_SWAP_gate(UINT target_index1, UINT target_index2);
 
     /**
+     * \~japanese-en FusedSWAP gateを追加する。
+     *
+     * @param[in] target_index1 作用するqubitブロックの先頭の添え字
+     * @param[in] target_index2 作用するもう一方のqubitブロックの先頭の添え字
+     * @param[in] block_size 作用するqubitブロックの大きさ
+     */
+    virtual void add_FusedSWAP_gate(
+        UINT target_index1, UINT target_index2, UINT block_size);
+
+    /**
      * \~japanese-en X-rotation gateを追加する。
      *
      * ゲートの表記は \f$ R_X(\theta) = \exp(i\theta X) \f$になっている。
      * @param[in] target_index 作用するtarget qubitの添え字
      * @param[in] angle 回転角\f$\theta\f$
      */
     virtual void add_RX_gate(UINT target_index, double angle);
@@ -570,8 +580,8 @@
 };
 
 namespace circuit {
 /**
  * \~japanese-en ptreeからQuantumCircuitを構築する
  */
 QuantumCircuit* from_ptree(const boost::property_tree::ptree& pt);
-}  // namespace circuit
+}  // namespace circuit
```

### Comparing `qulacs-0.5.6/src/cppsim/circuit_optimizer.cpp` & `qulacs-0.6.0/src/cppsim/circuit_optimizer.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/circuit_optimizer.hpp` & `qulacs-0.6.0/src/cppsim/circuit_optimizer.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/exception.hpp` & `qulacs-0.6.0/src/cppsim/exception.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,28 @@
      * @param message エラーメッセージ
      */
     NotImplementedException(const std::string& message)
         : std::logic_error(message) {}
 };
 
 /**
+ * \~japanese-en StateVectorとDensityMatrixが混ざっていて処理不能な例外
+ */
+class InoperatableQuantumStateTypeException : public std::logic_error {
+public:
+    /**
+     * \~japanese-en コンストラクタ
+     *
+     * @param message エラーメッセージ
+     */
+    InoperatableQuantumStateTypeException(const std::string& message)
+        : std::logic_error(message) {}
+};
+
+/**
  * \~japanese-en QuantumStateCpuとQuantumStateGpuを同じ演算中で用いている例外
  */
 class QuantumStateProcessorException : public std::logic_error {
 public:
     /**
      * \~japanese-en コンストラクタ
      *
@@ -312,7 +326,35 @@
     /**
      * \~japanese-en コンストラクタ
      *
      * @param message エラーメッセージ
      */
     IOException(const std::string& message) : std::runtime_error(message) {}
 };
+
+/**
+ * \~japanese-en MPIの実行時に失敗した例外
+ */
+class MPIRuntimeException : public std::runtime_error {
+public:
+    /**
+     * \~japanese-en コンストラクタ
+     *
+     * @param message エラーメッセージ
+     */
+    MPIRuntimeException(const std::string& message)
+        : std::runtime_error(message) {}
+};
+
+/**
+ * \~japanese-en mpi-size のエラー
+ */
+class MPISizeException : public std::runtime_error {
+public:
+    /**
+     * \~japanese-en コンストラクタ
+     *
+     * @param message エラーメッセージ
+     */
+    MPISizeException(const std::string& message)
+        : std::runtime_error(message) {}
+};
```

### Comparing `qulacs-0.5.6/src/cppsim/gate.cpp` & `qulacs-0.6.0/src/cppsim/gate.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate.hpp` & `qulacs-0.6.0/src/cppsim/gate.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_factory.cpp` & `qulacs-0.6.0/src/cppsim/gate_factory.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 #include "exception.hpp"
 #include "gate.hpp"
 #include "gate_matrix.hpp"
 #include "gate_matrix_diagonal.hpp"
 #include "gate_matrix_sparse.hpp"
 #include "gate_merge.hpp"
+#include "gate_named_npair.hpp"
 #include "gate_named_one.hpp"
 #include "gate_named_pauli.hpp"
 #include "gate_named_two.hpp"
 #include "gate_reflect.hpp"
 #include "gate_reversible.hpp"
 #include "state_dm.hpp"
 #include "type.hpp"
@@ -232,14 +233,28 @@
             "\nInfo: NULL used to be returned, "
             "but it changed to throw exception.");
     }
     auto ptr = new ClsTwoQubitGate();
     ptr->SWAPGateinit(qubit_index1, qubit_index2);
     return ptr;
 }
+ClsNpairQubitGate* FusedSWAP(
+    UINT qubit_index1, UINT qubit_index2, UINT block_size) {
+    if (std::min(qubit_index1, qubit_index2) + block_size >
+        std::max(qubit_index1, qubit_index2)) {
+        throw DuplicatedQubitIndexException(
+            "Error: gate::FusedSWAP(UINT, UINT, UINT): two specified blocks "
+            "are overlapping."
+            "\nInfo: NULL used to be returned, "
+            "but it changed to throw exception.");
+    }
+    auto ptr = new ClsNpairQubitGate();
+    ptr->FusedSWAPGateinit(qubit_index1, qubit_index2, block_size);
+    return ptr;
+}
 
 ClsPauliGate* Pauli(std::vector<UINT> target, std::vector<UINT> pauli_id) {
     if (!check_is_unique_index_list(target)) {
         throw DuplicatedQubitIndexException(
             "Error: gate::Pauli(std::vector<UINT> target, "
             "std::vector<UINT>pauli_id): target list contains "
             "duplicated values."
```

### Comparing `qulacs-0.5.6/src/cppsim/gate_factory.hpp` & `qulacs-0.6.0/src/cppsim/gate_factory.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #include <string>
 #include <vector>
 
 #include "gate.hpp"
 #include "gate_general.hpp"
 #include "gate_matrix_diagonal.hpp"
 #include "gate_matrix_sparse.hpp"
+#include "gate_named_npair.hpp"
 #include "gate_named_one.hpp"
 #include "gate_named_two.hpp"
 #include "gate_noisy_evolution.hpp"
 #include "gate_reflect.hpp"
 #include "gate_reversible.hpp"
 #include "observable.hpp"
 #include "type.hpp"
@@ -32,14 +33,15 @@
  * S            :   S \<index\>
  * Sdag         :   Sdag \<index\>
  * T            :   T \<index\>
  * Tdag         :   Tdag \<index\>
  * CNOT,CX      :   CNOT \<control\> \<target\>, or CX \<control\> \<target\>
  * CZ           :   CZ \<control\> \<target\>
  * SWAP         :   SWAP \<target1\> \<target2\>
+ * FusedSWAP    :   FusedSWAP \<target1\> \<target2\> \<blocksize\>
  * U1           :   U1 \<index\> \<angle1\>
  * U2           :   U2 \<index\> \<angle1\> \<angle2\>
  * U3           :   U3 \<index\> \<angle1\> \<angle2\> \<angle3\>
  * RX           :   RX \<index\> \<angle1\>
  * RY           :   RY \<index\> \<angle1\>
  * RZ           :   RZ \<index\> \<angle1\>
  * DifRot X     :   RDX \<index\>
@@ -271,14 +273,25 @@
  * @param[in] qubit_index1 ターゲットとなる量子ビットの添え字
  * @param[in] qubit_index2 ターゲットとなる量子ビットの添え字
  * @return 作成されたゲートのインスタンス
  */
 DllExport ClsTwoQubitGate* SWAP(UINT qubit_index1, UINT qubit_index2);
 
 /**
+ * \~japanese-en FusedSWAPゲートを作成する
+ *
+ * @param[in] qubit_index1 ターゲットとなる量子ビットの添え字
+ * @param[in] qubit_index2 ターゲットとなる量子ビットの添え字
+ * @param[in] block_size ターゲットとなる量子ブロックサイズ
+ * @return 作成されたゲートのインスタンス
+ */
+DllExport ClsNpairQubitGate* FusedSWAP(
+    UINT qubit_index1, UINT qubit_index2, UINT block_size);
+
+/**
  * \f$n\f$-qubit パウリ演算子のゲートを作成する
  *
  * 例えば\f$Y_1 X_3\f$であれば、<code>target_qubit_index_list = {1,3},
  * pauli_id_list = {2,1};</code>である。
  * @param[in] target_qubit_index_list ターゲットとなる量子ビットの添え字のリスト
  * @param[in] pauli_id_list
  * その量子ビットに作用するパウリ演算子。\f${I,X,Y,Z}\f$が\f${0,1,2,3}\f$に対応する。
```

### Comparing `qulacs-0.5.6/src/cppsim/gate_general.hpp` & `qulacs-0.6.0/src/cppsim/gate_general.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_matrix.cpp` & `qulacs-0.6.0/src/cppsim/gate_matrix.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -65,16 +65,14 @@
     this->_control_qubit_list =
         std::vector<ControlQubitInfo>(control_qubit_index_list_);
     this->_matrix_element.swap(*matrix_element);
     this->_name = "DenseMatrix";
 }
 
 void QuantumGateMatrix::update_quantum_state(QuantumStateBase* state) {
-    ITYPE dim = 1ULL << state->qubit_count;
-
     // Eigen::Matrix<std::complex<double>, Eigen::Dynamic, Eigen::Dynamic,
     // Eigen::RowMajor> row_matrix(this->_matrix_element); const CTYPE*
     // matrix_ptr = reinterpret_cast<const CTYPE*>(row_matrix.data()); const
     // CTYPE* matrix_ptr = reinterpret_cast<const
     // CTYPE*>(this->_matrix_element.data());
     /*
   #ifdef _USE_GPU
@@ -98,178 +96,202 @@
         this->_target_qubit_list.cend(), std::back_inserter(target_index),
         [](const TargetQubitInfo& value) { return value.index(); });
     for (auto val : this->_control_qubit_list) {
         control_index.push_back(val.index());
         control_value.push_back(val.control_value());
     }
 
-    if (state->is_state_vector()) {
-        // single qubit dense matrix gate
-        if (this->_target_qubit_list.size() == 1) {
-            // no control qubit
-            if (this->_control_qubit_list.size() == 0) {
-#ifdef _USE_GPU
-                if (state->get_device_name() == "gpu") {
-                    single_qubit_dense_matrix_gate_host(target_index[0],
-                        (const CPPCTYPE*)matrix_ptr, state->data(), dim,
-                        state->get_cuda_stream(), state->device_number);
-                } else {
-                    single_qubit_dense_matrix_gate(
-                        target_index[0], matrix_ptr, state->data_c(), dim);
-                }
-#else
-                single_qubit_dense_matrix_gate(
-                    target_index[0], matrix_ptr, state->data_c(), dim);
+    // dense matrix gate for Dense Matrix type simulation
+    if (!state->is_state_vector()) {
+        if (this->_control_qubit_list.size() == 0) {
+            if (this->_target_qubit_list.size() == 1) {
+                dm_single_qubit_dense_matrix_gate(
+                    target_index[0], matrix_ptr, state->data_c(), state->dim);
+            } else {
+                dm_multi_qubit_dense_matrix_gate(target_index.data(),
+                    (UINT)target_index.size(), matrix_ptr, state->data_c(),
+                    state->dim);
+            }
+        } else {
+            if (this->_target_qubit_list.size() == 1) {
+                dm_multi_qubit_control_single_qubit_dense_matrix_gate(
+                    control_index.data(), control_value.data(),
+                    (UINT)control_index.size(), target_index[0], matrix_ptr,
+                    state->data_c(), state->dim);
+            } else {
+                dm_multi_qubit_control_multi_qubit_dense_matrix_gate(
+                    control_index.data(), control_value.data(),
+                    (UINT)control_index.size(), target_index.data(),
+                    (UINT)target_index.size(), matrix_ptr, state->data_c(),
+                    state->dim);
+            }
+        }
+        return;
+    }
+
+    // dense matrix gate for State Vector type simulation
+    // single qubit dense matrix gate
+    if (this->_target_qubit_list.size() == 1) {
+        // no control qubit
+        if (this->_control_qubit_list.size() == 0) {
+#ifdef _USE_GPU
+            if (state->get_device_name() == "gpu") {
+                single_qubit_dense_matrix_gate_host(target_index[0],
+                    (const CPPCTYPE*)matrix_ptr, state->data(), state->dim,
+                    state->get_cuda_stream(), state->device_number);
+            } else
 #endif
+#ifdef _USE_MPI
+                if (state->outer_qc > 0) {
+                single_qubit_dense_matrix_gate_mpi(target_index[0], matrix_ptr,
+                    state->data_c(), state->dim, state->inner_qc);
+            } else
+#endif
+            {
+                single_qubit_dense_matrix_gate(
+                    target_index[0], matrix_ptr, state->data_c(), state->dim);
             }
-            // single control qubit
-            else if (this->_control_qubit_list.size() == 1) {
+        }
+        // single control qubit
+        else if (this->_control_qubit_list.size() == 1) {
 #ifdef _USE_GPU
-                if (state->get_device_name() == "gpu") {
-                    single_qubit_control_single_qubit_dense_matrix_gate_host(
-                        control_index[0], control_value[0], target_index[0],
-                        (const CPPCTYPE*)matrix_ptr, state->data(), dim,
-                        state->get_cuda_stream(), state->device_number);
-                } else {
-                    single_qubit_control_single_qubit_dense_matrix_gate(
-                        control_index[0], control_value[0], target_index[0],
-                        matrix_ptr, state->data_c(), dim);
-                }
-#else
-                single_qubit_control_single_qubit_dense_matrix_gate(
+            if (state->get_device_name() == "gpu") {
+                single_qubit_control_single_qubit_dense_matrix_gate_host(
+                    control_index[0], control_value[0], target_index[0],
+                    (const CPPCTYPE*)matrix_ptr, state->data(), state->dim,
+                    state->get_cuda_stream(), state->device_number);
+            } else
+#endif
+#ifdef _USE_MPI
+                if (state->outer_qc > 0) {
+                single_qubit_control_single_qubit_dense_matrix_gate_mpi(
                     control_index[0], control_value[0], target_index[0],
-                    matrix_ptr, state->data_c(), dim);
+                    matrix_ptr, state->data_c(), state->dim, state->inner_qc);
+            } else
 #endif
+            {
+                single_qubit_control_single_qubit_dense_matrix_gate(
+                    control_index[0], control_value[0], target_index[0],
+                    matrix_ptr, state->data_c(), state->dim);
             }
+        } else {
             // multiple control qubits
-            else {
 #ifdef _USE_GPU
-                if (state->get_device_name() == "gpu") {
-                    //
-                    // std::cerr << "Redirected to multi_control multi_target in
-                    // GPU" << std::endl;
-                    multi_qubit_control_multi_qubit_dense_matrix_gate_host(
+            if (state->get_device_name() == "gpu") {
+                //
+                // std::cerr << "Redirected to multi_control multi_target in
+                // GPU" << std::endl;
+                multi_qubit_control_multi_qubit_dense_matrix_gate_host(
+                    control_index.data(), control_value.data(),
+                    (UINT)(control_index.size()), target_index.data(),
+                    (UINT)(target_index.size()), (const CPPCTYPE*)matrix_ptr,
+                    state->data(), state->dim, state->get_cuda_stream(),
+                    state->device_number);
+                // exit(0);
+                /*
+                multi_qubit_control_single_qubit_dense_matrix_gate_host(
                         control_index.data(), control_value.data(),
-                        (UINT)(control_index.size()), target_index.data(),
-                        (UINT)(target_index.size()),
-                        (const CPPCTYPE*)matrix_ptr, state->data(), dim,
-                        state->get_cuda_stream(), state->device_number);
-                    // exit(0);
-                    /*
-                    multi_qubit_control_single_qubit_dense_matrix_gate_host(
-                            control_index.data(), control_value.data(),
+                (UINT)(control_index.size()), target_index[0], matrix_ptr,
+                state->data(), state->dim );
+                        */
+            } else
+#endif
+#ifdef _USE_MPI
+                if (state->outer_qc > 0) {
+                multi_qubit_control_single_qubit_dense_matrix_gate_mpi(
+                    control_index.data(), control_value.data(),
                     (UINT)(control_index.size()), target_index[0], matrix_ptr,
-                    state->data(), dim );
-                            */
-                } else {
-                    multi_qubit_control_single_qubit_dense_matrix_gate(
-                        control_index.data(), control_value.data(),
-                        (UINT)(control_index.size()), target_index[0],
-                        matrix_ptr, state->data_c(), dim);
-                }
-#else
+                    state->data_c(), state->dim, state->inner_qc);
+            } else
+#endif
+            {
                 multi_qubit_control_single_qubit_dense_matrix_gate(
                     control_index.data(), control_value.data(),
                     (UINT)(control_index.size()), target_index[0], matrix_ptr,
-                    state->data_c(), dim);
-#endif
+                    state->data_c(), state->dim);
             }
         }
-
+    } else {
         // multi qubit dense matrix gate
-        else {
-            // no control qubit
-            if (this->_control_qubit_list.size() == 0) {
+        // no control qubit
+        if (this->_control_qubit_list.size() == 0) {
 #ifdef _USE_GPU
-                if (state->get_device_name() == "gpu") {
-                    multi_qubit_dense_matrix_gate_host(target_index.data(),
-                        (UINT)(target_index.size()),
-                        (const CPPCTYPE*)matrix_ptr, state->data(), dim,
-                        state->get_cuda_stream(), state->device_number);
-                } else {
-                    multi_qubit_dense_matrix_gate(target_index.data(),
-                        (UINT)(target_index.size()), matrix_ptr,
-                        state->data_c(), dim);
-                }
-#else
-                multi_qubit_dense_matrix_gate(target_index.data(),
+            if (state->get_device_name() == "gpu") {
+                multi_qubit_dense_matrix_gate_host(target_index.data(),
+                    (UINT)(target_index.size()), (const CPPCTYPE*)matrix_ptr,
+                    state->data(), state->dim, state->get_cuda_stream(),
+                    state->device_number);
+            } else
+#endif
+#ifdef _USE_MPI
+                if (state->outer_qc > 0) {
+                multi_qubit_dense_matrix_gate_mpi(target_index.data(),
                     (UINT)(target_index.size()), matrix_ptr, state->data_c(),
-                    dim);
+                    state->dim, state->inner_qc);
+            } else
 #endif
+            {
+                multi_qubit_dense_matrix_gate(target_index.data(),
+                    (UINT)(target_index.size()), matrix_ptr, state->data_c(),
+                    state->dim);
             }
-            // single control qubit
-            else if (this->_control_qubit_list.size() == 1) {
+        }
+        // single control qubit
+        else if (this->_control_qubit_list.size() == 1) {
 #ifdef _USE_GPU
-                if (state->get_device_name() == "gpu") {
-                    single_qubit_control_multi_qubit_dense_matrix_gate_host(
-                        control_index[0], control_value[0], target_index.data(),
-                        (UINT)(target_index.size()),
-                        (const CPPCTYPE*)matrix_ptr, state->data(), dim,
-                        state->get_cuda_stream(), state->device_number);
-                } else {
-                    single_qubit_control_multi_qubit_dense_matrix_gate(
-                        control_index[0], control_value[0], target_index.data(),
-                        (UINT)(target_index.size()), matrix_ptr,
-                        state->data_c(), dim);
-                }
-#else
-                single_qubit_control_multi_qubit_dense_matrix_gate(
+            if (state->get_device_name() == "gpu") {
+                single_qubit_control_multi_qubit_dense_matrix_gate_host(
+                    control_index[0], control_value[0], target_index.data(),
+                    (UINT)(target_index.size()), (const CPPCTYPE*)matrix_ptr,
+                    state->data(), state->dim, state->get_cuda_stream(),
+                    state->device_number);
+            } else
+#endif
+#ifdef _USE_MPI
+                if (state->outer_qc > 0)
+                single_qubit_control_multi_qubit_dense_matrix_gate_mpi(
                     control_index[0], control_value[0], target_index.data(),
                     (UINT)(target_index.size()), matrix_ptr, state->data_c(),
-                    dim);
+                    state->dim, state->inner_qc);
+            else
 #endif
+            {
+                single_qubit_control_multi_qubit_dense_matrix_gate(
+                    control_index[0], control_value[0], target_index.data(),
+                    (UINT)(target_index.size()), matrix_ptr, state->data_c(),
+                    state->dim);
             }
-            // multiple control qubit
-            else {
+        }
+        // multiple control qubit
+        else {
 #ifdef _USE_GPU
-                if (state->get_device_name() == "gpu") {
-                    multi_qubit_control_multi_qubit_dense_matrix_gate_host(
-                        control_index.data(), control_value.data(),
-                        (UINT)(control_index.size()), target_index.data(),
-                        (UINT)(target_index.size()),
-                        (const CPPCTYPE*)matrix_ptr, state->data(), dim,
-                        state->get_cuda_stream(), state->device_number);
-                } else {
-                    multi_qubit_control_multi_qubit_dense_matrix_gate(
-                        control_index.data(), control_value.data(),
-                        (UINT)(control_index.size()), target_index.data(),
-                        (UINT)(target_index.size()), matrix_ptr,
-                        state->data_c(), dim);
-                }
-#else
-                multi_qubit_control_multi_qubit_dense_matrix_gate(
+            if (state->get_device_name() == "gpu") {
+                multi_qubit_control_multi_qubit_dense_matrix_gate_host(
                     control_index.data(), control_value.data(),
                     (UINT)(control_index.size()), target_index.data(),
-                    (UINT)(target_index.size()), matrix_ptr, state->data_c(),
-                    dim);
+                    (UINT)(target_index.size()), (const CPPCTYPE*)matrix_ptr,
+                    state->data(), state->dim, state->get_cuda_stream(),
+                    state->device_number);
+            } else
 #endif
-            }
-        }
-    } else {
-        if (this->_control_qubit_list.size() == 0) {
-            if (this->_target_qubit_list.size() == 1) {
-                dm_single_qubit_dense_matrix_gate(
-                    target_index[0], matrix_ptr, state->data_c(), dim);
-            } else {
-                dm_multi_qubit_dense_matrix_gate(target_index.data(),
-                    (UINT)target_index.size(), matrix_ptr, state->data_c(),
-                    dim);
-            }
-        } else {
-            if (this->_target_qubit_list.size() == 1) {
-                dm_multi_qubit_control_single_qubit_dense_matrix_gate(
+#ifdef _USE_MPI
+                if (state->outer_qc > 0)
+                multi_qubit_control_multi_qubit_dense_matrix_gate_mpi(
                     control_index.data(), control_value.data(),
-                    (UINT)control_index.size(), target_index[0], matrix_ptr,
-                    state->data_c(), dim);
-            } else {
-                dm_multi_qubit_control_multi_qubit_dense_matrix_gate(
+                    (UINT)(control_index.size()), target_index.data(),
+                    (UINT)(target_index.size()), matrix_ptr, state->data_c(),
+                    state->dim, state->inner_qc);
+            else
+#endif
+            {
+                multi_qubit_control_multi_qubit_dense_matrix_gate(
                     control_index.data(), control_value.data(),
-                    (UINT)control_index.size(), target_index.data(),
-                    (UINT)target_index.size(), matrix_ptr, state->data_c(),
-                    dim);
+                    (UINT)(control_index.size()), target_index.data(),
+                    (UINT)(target_index.size()), matrix_ptr, state->data_c(),
+                    state->dim);
             }
         }
     }
 }
 
 void QuantumGateMatrix::add_control_qubit(
     UINT qubit_index, UINT control_value) {
@@ -303,8 +325,8 @@
 std::ostream& operator<<(std::ostream& os, QuantumGateMatrix* gate) {
     os << *gate;
     return os;
 }
 
 QuantumGateMatrix* QuantumGateMatrix::get_inverse(void) const {
     return gate::get_adjoint_gate(this);
-}
+}
```

### Comparing `qulacs-0.5.6/src/cppsim/gate_matrix.hpp` & `qulacs-0.6.0/src/cppsim/gate_matrix.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_matrix_diagonal.cpp` & `qulacs-0.6.0/src/cppsim/gate_matrix_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_matrix_diagonal.hpp` & `qulacs-0.6.0/src/cppsim/gate_matrix_diagonal.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_matrix_sparse.cpp` & `qulacs-0.6.0/src/cppsim/gate_matrix_sparse.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_matrix_sparse.hpp` & `qulacs-0.6.0/src/cppsim/gate_matrix_sparse.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_merge.cpp` & `qulacs-0.6.0/src/cppsim/gate_merge.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_merge.hpp` & `qulacs-0.6.0/src/cppsim/gate_merge.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_named_one.cpp` & `qulacs-0.6.0/src/cppsim/gate_named_one.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_named_one.hpp` & `qulacs-0.6.0/src/cppsim/gate_named_one.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -14,22 +14,25 @@
 
 /**
  * \~japanese-en 1量子ビットを対象とする回転角固定のゲートのクラス
  */
 
 static void Igate_idling(UINT, CTYPE*, ITYPE){};
 static void Igate_idling_gpu(UINT, void*, ITYPE, void*, UINT){};
+static void Igate_idling_mpi(UINT, CTYPE*, ITYPE, UINT){};
 
 class ClsOneQubitGate : public QuantumGateBase {
 protected:
     using UpdateFunc = void (*)(UINT, CTYPE*, ITYPE);
     using UpdateFuncGpu = void (*)(UINT, void*, ITYPE, void*, UINT);
+    using UpdateFuncMpi = void (*)(UINT, CTYPE*, ITYPE, UINT);
     UpdateFunc _update_func;
     UpdateFunc _update_func_dm;
     UpdateFuncGpu _update_func_gpu;
+    UpdateFuncMpi _update_func_mpi;
     ComplexMatrix _matrix_element;
 
 public:
     explicit ClsOneQubitGate(){};
     /**
      * \~japanese-en 量子状態を更新する
      *
@@ -38,22 +41,26 @@
     virtual void update_quantum_state(QuantumStateBase* state) override {
         if (state->is_state_vector()) {
 #ifdef _USE_GPU
             if (state->get_device_name() == "gpu") {
                 _update_func_gpu(this->target_qubit_list[0].index(),
                     state->data(), state->dim, state->get_cuda_stream(),
                     state->device_number);
-            } else {
+            } else
+#endif
+#ifdef _USE_MPI
+                if (state->outer_qc > 0) {
+                _update_func_mpi(this->_target_qubit_list[0].index(),
+                    state->data_c(), state->dim, state->inner_qc);
+            } else
+#endif
+            {
                 _update_func(this->_target_qubit_list[0].index(),
                     state->data_c(), state->dim);
             }
-#else
-            _update_func(this->_target_qubit_list[0].index(), state->data_c(),
-                state->dim);
-#endif
         } else {
             _update_func_dm(this->_target_qubit_list[0].index(),
                 state->data_c(), state->dim);
         }
     };
     /**
      * \~japanese-en 自身のディープコピーを生成する
@@ -72,70 +79,83 @@
         matrix = this->_matrix_element;
     }
 
     void IGateinit(UINT target_qubit_index) {
         this->_update_func = Igate_idling;
         this->_update_func_dm = Igate_idling;
         this->_update_func_gpu = Igate_idling_gpu;
+        this->_update_func_mpi = Igate_idling_mpi;
         this->_name = "I";
         this->_target_qubit_list.push_back(TargetQubitInfo(target_qubit_index,
             FLAG_X_COMMUTE | FLAG_Y_COMMUTE | FLAG_Z_COMMUTE));
         this->_gate_property = FLAG_PAULI | FLAG_CLIFFORD | FLAG_GAUSSIAN;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 1, 0, 0, 1;
     }
 
     void XGateinit(UINT target_qubit_index) {
         this->_update_func = X_gate;
         this->_update_func_dm = dm_X_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = X_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = X_gate_mpi;
+#endif
         this->_name = "X";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_X_COMMUTE));
         this->_gate_property = FLAG_PAULI | FLAG_CLIFFORD;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 0, 1, 1, 0;
     }
 
     void YGateinit(UINT target_qubit_index) {
         this->_update_func = Y_gate;
         this->_update_func_dm = dm_Y_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = Y_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = Y_gate_mpi;
+#endif
         this->_name = "Y";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_Y_COMMUTE));
         this->_gate_property = FLAG_PAULI | FLAG_CLIFFORD;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 0, -1.i, 1.i, 0;
     }
 
     void ZGateinit(UINT target_qubit_index) {
         this->_update_func = Z_gate;
         this->_update_func_dm = dm_Z_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = Z_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = Z_gate_mpi;
+#endif
         this->_name = "Z";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_Z_COMMUTE));
         this->_gate_property = FLAG_PAULI | FLAG_CLIFFORD | FLAG_GAUSSIAN;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 1, 0, 0, -1;
     }
 
     void HGateinit(UINT target_qubit_index) {
         this->_update_func = H_gate;
         this->_update_func_dm = dm_H_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = H_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = H_gate_mpi;
+#endif
         this->_name = "H";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, 0));
         this->_gate_property = FLAG_CLIFFORD;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 1, 1, 1, -1;
         this->_matrix_element /= sqrt(2.);
@@ -143,137 +163,167 @@
 
     void SGateinit(UINT target_qubit_index) {
         this->_update_func = S_gate;
         this->_update_func_dm = dm_S_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = S_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = S_gate_mpi;
+#endif
         this->_name = "S";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_Z_COMMUTE));
         this->_gate_property = FLAG_CLIFFORD | FLAG_GAUSSIAN;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 1, 0, 0, 1.i;
     }
 
     void SdagGateinit(UINT target_qubit_index) {
         this->_update_func = Sdag_gate;
         this->_update_func_dm = dm_Sdag_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = Sdag_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = Sdag_gate_mpi;
+#endif
         this->_name = "Sdag";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_Z_COMMUTE));
         this->_gate_property = FLAG_CLIFFORD | FLAG_GAUSSIAN;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 1, 0, 0, -1.i;
     }
 
     void TGateinit(UINT target_qubit_index) {
         this->_update_func = T_gate;
         this->_update_func_dm = dm_T_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = T_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = T_gate_mpi;
+#endif
         this->_name = "T";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_Z_COMMUTE));
         this->_gate_property = FLAG_GAUSSIAN;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 1, 0, 0, (1. + 1.i) / sqrt(2.);
     }
 
     void TdagGateinit(UINT target_qubit_index) {
         this->_update_func = Tdag_gate;
         this->_update_func_dm = dm_Tdag_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = Tdag_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = Tdag_gate_mpi;
+#endif
         this->_name = "Tdag";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_Z_COMMUTE));
         this->_gate_property = FLAG_GAUSSIAN;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 1, 0, 0, (1. - 1.i) / sqrt(2.);
     }
 
     void sqrtXGateinit(UINT target_qubit_index) {
         this->_update_func = sqrtX_gate;
         this->_update_func_dm = dm_sqrtX_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = sqrtX_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = sqrtX_gate_mpi;
+#endif
         this->_name = "sqrtX";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_X_COMMUTE));
         this->_gate_property = FLAG_CLIFFORD;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 0.5 + 0.5i, 0.5 - 0.5i, 0.5 - 0.5i, 0.5 + 0.5i;
     }
     void sqrtXdagGateinit(UINT target_qubit_index) {
         this->_update_func = sqrtXdag_gate;
         this->_update_func_dm = dm_sqrtXdag_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = sqrtXdag_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = sqrtXdag_gate_mpi;
+#endif
         this->_name = "sqrtXdag";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_X_COMMUTE));
         this->_gate_property = FLAG_CLIFFORD;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 0.5 - 0.5i, 0.5 + 0.5i, 0.5 + 0.5i, 0.5 - 0.5i;
     }
     void sqrtYGateinit(UINT target_qubit_index) {
         this->_update_func = sqrtY_gate;
         this->_update_func_dm = dm_sqrtY_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = sqrtY_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = sqrtY_gate_mpi;
+#endif
         this->_name = "sqrtY";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_Y_COMMUTE));
         this->_gate_property = FLAG_CLIFFORD;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 0.5 + 0.5i, -0.5 - 0.5i, 0.5 + 0.5i,
             0.5 + 0.5i;
     }
     void sqrtYdagGateinit(UINT target_qubit_index) {
         this->_update_func = sqrtYdag_gate;
         this->_update_func_dm = dm_sqrtYdag_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = sqrtYdag_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = sqrtYdag_gate_mpi;
+#endif
         this->_name = "sqrtYdag";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_Y_COMMUTE));
         this->_gate_property = FLAG_CLIFFORD;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 0.5 - 0.5i, 0.5 - 0.5i, -0.5 + 0.5i,
             0.5 - 0.5i;
     }
     void P0Gateinit(UINT target_qubit_index) {
         this->_update_func = P0_gate;
         this->_update_func_dm = dm_P0_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = P0_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = P0_gate_mpi;
+#endif
         this->_name = "Projection-0";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, 0));
         this->_gate_property = FLAG_CLIFFORD | FLAG_GAUSSIAN;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 1, 0, 0, 0;
     }
     void P1Gateinit(UINT target_qubit_index) {
         this->_update_func = P1_gate;
         this->_update_func_dm = dm_P1_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = P1_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = P1_gate_mpi;
+#endif
         this->_name = "Projection-1";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, 0));
         this->_gate_property = FLAG_CLIFFORD | FLAG_GAUSSIAN;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << 0, 0, 0, 1;
     }
@@ -290,17 +340,19 @@
 /**
  * \~japanese-en 1量子ビットを対象とする回転ゲートのクラス
  */
 class ClsOneQubitRotationGate : public QuantumGateBase {
 protected:
     using UpdateFunc = void (*)(UINT, double, CTYPE*, ITYPE);
     using UpdateFuncGpu = void (*)(UINT, double, void*, ITYPE, void*, UINT);
+    using UpdateFuncMpi = void (*)(UINT, double, CTYPE*, ITYPE, UINT);
     UpdateFunc _update_func;
     UpdateFunc _update_func_dm;
     UpdateFuncGpu _update_func_gpu;
+    UpdateFuncMpi _update_func_mpi;
     ComplexMatrix _matrix_element;
     double _angle;
 
 public:
     explicit ClsOneQubitRotationGate(){};
     explicit ClsOneQubitRotationGate(double angle) : _angle(angle){};
     /**
@@ -311,22 +363,26 @@
     virtual void update_quantum_state(QuantumStateBase* state) override {
         if (state->is_state_vector()) {
 #ifdef _USE_GPU
             if (state->get_device_name() == "gpu") {
                 _update_func_gpu(this->_target_qubit_list[0].index(), _angle,
                     state->data(), state->dim, state->get_cuda_stream(),
                     state->device_number);
-            } else {
+            } else
+#endif
+#ifdef _USE_MPI
+                if (state->outer_qc > 0) {
+                _update_func_mpi(this->_target_qubit_list[0].index(), _angle,
+                    state->data_c(), state->dim, state->inner_qc);
+            } else
+#endif
+            {
                 _update_func(this->_target_qubit_list[0].index(), _angle,
                     state->data_c(), state->dim);
             }
-#else
-            _update_func(this->_target_qubit_list[0].index(), _angle,
-                state->data_c(), state->dim);
-#endif
         } else {
             _update_func_dm(this->_target_qubit_list[0].index(), _angle,
                 state->data_c(), state->dim);
         }
     };
     /**
      * \~japanese-en 自身のディープコピーを生成する
@@ -348,14 +404,17 @@
     void RXGateinit(UINT target_qubit_index, double angle) {
         this->_angle = angle;
         this->_update_func = RX_gate;
         this->_update_func_dm = dm_RX_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = RX_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = RX_gate_mpi;
+#endif
         this->_name = "X-rotation";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_X_COMMUTE));
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << cos(_angle / 2), sin(_angle / 2) * 1.i,
             sin(_angle / 2) * 1.i, cos(_angle / 2);
     }
@@ -363,14 +422,17 @@
     void RYGateinit(UINT target_qubit_index, double angle) {
         this->_angle = angle;
         this->_update_func = RY_gate;
         this->_update_func_dm = dm_RY_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = RY_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = RY_gate_mpi;
+#endif
         this->_name = "Y-rotation";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_Y_COMMUTE));
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << cos(_angle / 2), sin(_angle / 2),
             -sin(_angle / 2), cos(_angle / 2);
     }
@@ -378,14 +440,17 @@
     void RZGateinit(UINT target_qubit_index, double angle) {
         this->_angle = angle;
         this->_update_func = RZ_gate;
         this->_update_func_dm = dm_RZ_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = RZ_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = RZ_gate_mpi;
+#endif
         this->_name = "Z-rotation";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_Z_COMMUTE));
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
         this->_matrix_element << cos(_angle / 2) + 1.i * sin(_angle / 2), 0, 0,
             cos(_angle / 2) - 1.i * sin(_angle / 2);
     }
@@ -397,8 +462,8 @@
         pt.add("angle", _angle);
         return pt;
     }
     virtual ClsOneQubitRotationGate* get_inverse(void) const override;
 };
 
 using QuantumGate_OneQubit = ClsOneQubitGate;
-using QuantumGate_OneQubitRotation = ClsOneQubitRotationGate;
+using QuantumGate_OneQubitRotation = ClsOneQubitRotationGate;
```

### Comparing `qulacs-0.5.6/src/cppsim/gate_named_pauli.hpp` & `qulacs-0.6.0/src/cppsim/gate_named_pauli.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_named_two.hpp` & `qulacs-0.6.0/src/cppsim/gate_named_two.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 /**
  * \~japanese-en 2量子ビットを対象とする回転角固定のゲートのクラス
  */
 class ClsTwoQubitGate : public QuantumGateBase {
 protected:
     using UpdateFunc = void (*)(UINT, UINT, CTYPE*, ITYPE);
     using UpdateFuncGpu = void (*)(UINT, UINT, void*, ITYPE, void*, UINT);
+    using UpdateFuncMpi = void (*)(UINT, UINT, CTYPE*, ITYPE, UINT);
     UpdateFunc _update_func;
     UpdateFunc _update_func_dm;
     UpdateFuncGpu _update_func_gpu;
+    UpdateFuncMpi _update_func_mpi;
     ComplexMatrix _matrix_element;
 
 public:
     explicit ClsTwoQubitGate(){};
     /**
      * \~japanese-en 量子状態を更新する
      *
@@ -28,24 +30,28 @@
     virtual void update_quantum_state(QuantumStateBase* state) override {
         if (state->is_state_vector()) {
 #ifdef _USE_GPU
             if (state->get_device_name() == "gpu") {
                 _update_func_gpu(this->_target_qubit_list[0].index(),
                     this->_target_qubit_list[1].index(), state->data(),
                     state->dim, state->get_cuda_stream(), state->device_number);
-            } else {
+            } else
+#endif
+#ifdef _USE_MPI
+                if (state->outer_qc > 0) {
+                _update_func_mpi(this->_target_qubit_list[0].index(),
+                    this->_target_qubit_list[1].index(), state->data_c(),
+                    state->dim, state->inner_qc);
+            } else
+#endif
+            {
                 _update_func(this->_target_qubit_list[0].index(),
                     this->_target_qubit_list[1].index(), state->data_c(),
                     state->dim);
             }
-#else
-            _update_func(this->_target_qubit_list[0].index(),
-                this->_target_qubit_list[1].index(), state->data_c(),
-                state->dim);
-#endif
         } else {
             _update_func_dm(this->_target_qubit_list[0].index(),
                 this->_target_qubit_list[1].index(), state->data_c(),
                 state->dim);
         }
     };
     /**
@@ -67,14 +73,17 @@
 
     void SWAPGateinit(UINT target_qubit_index1, UINT target_qubit_index2) {
         this->_update_func = SWAP_gate;
         this->_update_func_dm = dm_SWAP_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = SWAP_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = SWAP_gate_mpi;
+#endif
         this->_name = "SWAP";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index1, 0));
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index2, 0));
         this->_gate_property = FLAG_CLIFFORD;
         this->_matrix_element = ComplexMatrix::Zero(4, 4);
@@ -114,17 +123,19 @@
  * \~japanese-en
  * 1量子ビットを対象とし1量子ビットにコントロールされる回転角固定のゲートのクラス
  */
 class ClsOneControlOneTargetGate : public QuantumGateBase {
 protected:
     using UpdateFunc = void (*)(UINT, UINT, CTYPE*, ITYPE);
     using UpdateFuncGpu = void (*)(UINT, UINT, void*, ITYPE, void*, UINT);
+    using UpdateFuncMpi = void (*)(UINT, UINT, CTYPE*, ITYPE, UINT);
     UpdateFunc _update_func;
     UpdateFunc _update_func_dm;
     UpdateFuncGpu _update_func_gpu;
+    UpdateFuncMpi _update_func_mpi;
     ComplexMatrix _matrix_element;
 
 public:
     explicit ClsOneControlOneTargetGate(){};
     /**
      * \~japanese-en 量子状態を更新する
      *
@@ -133,24 +144,28 @@
     virtual void update_quantum_state(QuantumStateBase* state) override {
         if (state->is_state_vector()) {
 #ifdef _USE_GPU
             if (state->get_device_name() == "gpu") {
                 _update_func_gpu(this->_control_qubit_list[0].index(),
                     this->_target_qubit_list[0].index(), state->data(),
                     state->dim, state->get_cuda_stream(), state->device_number);
-            } else {
+            } else
+#endif
+#ifdef _USE_MPI
+                if (state->outer_qc > 0) {
+                _update_func_mpi(this->_control_qubit_list[0].index(),
+                    this->_target_qubit_list[0].index(), state->data_c(),
+                    state->dim, state->inner_qc);
+            } else
+#endif
+            {
                 _update_func(this->_control_qubit_list[0].index(),
                     this->_target_qubit_list[0].index(), state->data_c(),
                     state->dim);
             }
-#else
-            _update_func(this->_control_qubit_list[0].index(),
-                this->_target_qubit_list[0].index(), state->data_c(),
-                state->dim);
-#endif
         } else {
             _update_func_dm(this->_control_qubit_list[0].index(),
                 this->_target_qubit_list[0].index(), state->data_c(),
                 state->dim);
         }
     };
     /**
@@ -172,14 +187,17 @@
 
     void CNOTGateinit(UINT control_qubit_index, UINT target_qubit_index) {
         this->_update_func = CNOT_gate;
         this->_update_func_dm = dm_CNOT_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = CNOT_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = CNOT_gate_mpi;
+#endif
         this->_name = "CNOT";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_X_COMMUTE));
         this->_control_qubit_list.push_back(
             ControlQubitInfo(control_qubit_index, 1));
         this->_gate_property = FLAG_CLIFFORD;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
@@ -188,14 +206,17 @@
 
     void CZGateinit(UINT control_qubit_index, UINT target_qubit_index) {
         this->_update_func = CZ_gate;
         this->_update_func_dm = dm_CZ_gate;
 #ifdef _USE_GPU
         this->_update_func_gpu = CZ_gate_host;
 #endif
+#ifdef _USE_MPI
+        this->_update_func_mpi = CZ_gate_mpi;
+#endif
         this->_name = "CZ";
         this->_target_qubit_list.push_back(
             TargetQubitInfo(target_qubit_index, FLAG_Z_COMMUTE));
         this->_control_qubit_list.push_back(
             ControlQubitInfo(control_qubit_index, 1));
         this->_gate_property = FLAG_CLIFFORD;
         this->_matrix_element = ComplexMatrix::Zero(2, 2);
```

### Comparing `qulacs-0.5.6/src/cppsim/gate_noisy_evolution.cpp` & `qulacs-0.6.0/src/cppsim/gate_noisy_evolution.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_noisy_evolution.hpp` & `qulacs-0.6.0/src/cppsim/gate_noisy_evolution.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_reflect.hpp` & `qulacs-0.6.0/src/cppsim/gate_reflect.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_reversible.hpp` & `qulacs-0.6.0/src/cppsim/gate_reversible.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/gate_to_gqo.hpp` & `qulacs-0.6.0/src/cppsim/gate_to_gqo.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/general_quantum_operator.cpp` & `qulacs-0.6.0/src/cppsim/general_quantum_operator.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,16 @@
     if (this->_qubit_count > state->qubit_count) {
         throw InvalidQubitCountException(
             "Error: GeneralQuantumOperator::get_expectation_value(const "
             "QuantumStateBase*): invalid qubit count");
     }
 
     const size_t n_terms = this->_operator_list.size();
-    if (state->get_device_name() == "gpu") {
+    std::string device = state->get_device_name();
+    if (device == "gpu" || device == "multi-cpu") {
         CPPCTYPE sum = 0;
         for (UINT i = 0; i < n_terms; ++i) {
             sum += _operator_list[i]->get_expectation_value(state);
         }
         return sum;
     }
```

### Comparing `qulacs-0.5.6/src/cppsim/general_quantum_operator.hpp` & `qulacs-0.6.0/src/cppsim/general_quantum_operator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/matrix_decomposition.hpp` & `qulacs-0.6.0/src/cppsim/matrix_decomposition.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/noisesimulator.cpp` & `qulacs-0.6.0/src/cppsim/noisesimulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/noisesimulator.hpp` & `qulacs-0.6.0/src/cppsim/noisesimulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/observable.cpp` & `qulacs-0.6.0/src/cppsim/observable.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/observable.hpp` & `qulacs-0.6.0/src/cppsim/observable.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/pauli_operator.cpp` & `qulacs-0.6.0/src/cppsim/pauli_operator.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,10 @@
-#include <stdarg.h>
-#include <stdio.h>
-#include <stdlib.h>
 
 #include <boost/dynamic_bitset.hpp>
-#include <cassert>
-#include <cstring>
-#include <fstream>
-#include <iostream>
-#include <string>
-#include <utility>
-#include <vector>
 
-#include "type.hpp"
 #include "utility.hpp"
 #ifdef _USE_GPU
 #include <gpusim/stat_ops.h>
 #endif
 
 #include <csim/stat_ops.hpp>
 #include <csim/stat_ops_dm.hpp>
@@ -157,30 +146,36 @@
             return _coef *
                    expectation_value_multi_qubit_Pauli_operator_partial_list_host(
                        this->get_index_list().data(),
                        this->get_pauli_id_list().data(),
                        (UINT)this->get_index_list().size(), state->data(),
                        state->dim, state->get_cuda_stream(),
                        state->device_number);
-        } else {
+        } else
+#endif
+#ifdef _USE_MPI
+            if (state->outer_qc > 0) {
+            CPPCTYPE result =
+                _coef *
+                expectation_value_multi_qubit_Pauli_operator_partial_list_mpi(
+                    this->get_index_list().data(),
+                    this->get_pauli_id_list().data(),
+                    (UINT)this->get_index_list().size(), state->data_c(),
+                    state->dim, state->outer_qc, state->inner_qc);
+            return result;
+        } else
+#endif
+        {
             return _coef *
                    expectation_value_multi_qubit_Pauli_operator_partial_list(
                        this->get_index_list().data(),
                        this->get_pauli_id_list().data(),
                        (UINT)this->get_index_list().size(), state->data_c(),
                        state->dim);
         }
-#else
-        return _coef *
-               expectation_value_multi_qubit_Pauli_operator_partial_list(
-                   this->get_index_list().data(),
-                   this->get_pauli_id_list().data(),
-                   (UINT)this->get_index_list().size(), state->data_c(),
-                   state->dim);
-#endif
     } else {
         return _coef *
                dm_expectation_value_multi_qubit_Pauli_operator_partial_list(
                    this->get_index_list().data(),
                    this->get_pauli_id_list().data(),
                    (UINT)this->get_index_list().size(), state->data_c(),
                    state->dim);
@@ -199,14 +194,20 @@
                        this->get_index_list().data(),
                        this->get_pauli_id_list().data(),
                        (UINT)this->get_index_list().size(), state->data(),
                        state->dim, state->get_cuda_stream(),
                        state->device_number);
         }
 #endif
+#ifdef _USE_MPI
+        if (state->outer_qc > 0)
+            std::cout
+                << "# Warning! This implementation with MPI is not thread-safe."
+                << std::endl;
+#endif
         return _coef *
                expectation_value_multi_qubit_Pauli_operator_partial_list_single_thread(
                    this->get_index_list().data(),
                    this->get_pauli_id_list().data(),
                    (UINT)this->get_index_list().size(), state->data_c(),
                    state->dim);
     } else {
@@ -235,32 +236,25 @@
                (CPPCTYPE)
                    transition_amplitude_multi_qubit_Pauli_operator_partial_list_host(
                        this->get_index_list().data(),
                        this->get_pauli_id_list().data(),
                        (UINT)this->get_index_list().size(), state_bra->data(),
                        state_ket->data(), state_bra->dim,
                        state_ket->get_cuda_stream(), state_ket->device_number);
-    } else {
+    } else
+#endif
+    {
         return _coef *
                (CPPCTYPE)
                    transition_amplitude_multi_qubit_Pauli_operator_partial_list(
                        this->get_index_list().data(),
                        this->get_pauli_id_list().data(),
                        (UINT)this->get_index_list().size(), state_bra->data_c(),
                        state_ket->data_c(), state_bra->dim);
     }
-#else
-    return _coef *
-           (CPPCTYPE)
-               transition_amplitude_multi_qubit_Pauli_operator_partial_list(
-                   this->get_index_list().data(),
-                   this->get_pauli_id_list().data(),
-                   (UINT)this->get_index_list().size(), state_bra->data_c(),
-                   state_ket->data_c(), state_bra->dim);
-#endif
 }
 
 PauliOperator* PauliOperator::copy() const {
     auto pauli = new PauliOperator(this->_coef);
     for (auto val : this->_pauli_list) {
         pauli->add_single_Pauli(val.index(), val.pauli_id());
     }
```

### Comparing `qulacs-0.5.6/src/cppsim/pauli_operator.hpp` & `qulacs-0.6.0/src/cppsim/pauli_operator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/qubit_info.cpp` & `qulacs-0.6.0/src/cppsim/qubit_info.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/qubit_info.hpp` & `qulacs-0.6.0/src/cppsim/qubit_info.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/simulator.cpp` & `qulacs-0.6.0/src/cppsim/simulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/simulator.hpp` & `qulacs-0.6.0/src/cppsim/simulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/state.hpp` & `qulacs-0.6.0/src/cppsim/state.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -3,58 +3,118 @@
 #include <csim/init_ops.hpp>
 #include <csim/memory_ops.hpp>
 #include <csim/stat_ops.hpp>
 #include <csim/update_ops.hpp>
 #include <iostream>
 #include <vector>
 
+#include "csim/MPIutil.hpp"
 #include "exception.hpp"
 #include "type.hpp"
 #include "utility.hpp"
 
 /**
  * \~japanese-en 量子状態の基底クラス
  */
 class QuantumStateBase {
 protected:
     ITYPE _dim;
     UINT _qubit_count;
+    UINT _inner_qc;
+    UINT _outer_qc;
     bool _is_state_vector;
     std::vector<UINT> _classical_register;
     UINT _device_number;
     void* _cuda_stream;
 
 public:
     const UINT& qubit_count; /**< \~japanese-en 量子ビット数 */
-    const ITYPE& dim;        /**< \~japanese-en 量子状態の次元 */
+    const UINT& inner_qc; /**< \~japanese-en ノード内量子ビット数 */
+    const UINT& outer_qc; /**< \~japanese-en ノード外量子ビット数 */
+    const ITYPE& dim;     /**< \~japanese-en 量子状態の次元 */
     const std::vector<UINT>&
         classical_register; /**< \~japanese-en 古典ビットのレジスタ */
     const UINT& device_number;
     /**
      * \~japanese-en コンストラクタ
      *
      * @param qubit_count_ 量子ビット数
      */
     QuantumStateBase(UINT qubit_count_, bool is_state_vector)
         : qubit_count(_qubit_count),
+          inner_qc(_inner_qc),
+          outer_qc(_outer_qc),
           dim(_dim),
           classical_register(_classical_register),
           device_number(_device_number) {
         this->_qubit_count = qubit_count_;
+        this->_inner_qc = qubit_count_;
+        this->_outer_qc = 0;
         this->_dim = 1ULL << qubit_count_;
         this->_is_state_vector = is_state_vector;
         this->_device_number = 0;
     }
+
+    // 本来、QuantumStateBase(UINT, bool, bool) とすべきだが、
+    // QuantumStateBase(UINT, bool, UINT) に対し ambiguous error が発生するため
+    // QuantumStateBase(UINT, bool, int) とした
+    QuantumStateBase(UINT qubit_count_, bool is_state_vector, int use_multi_cpu)
+        : qubit_count(_qubit_count),
+          inner_qc(_inner_qc),
+          outer_qc(_outer_qc),
+          dim(_dim),
+          classical_register(_classical_register),
+          device_number(_device_number) {
+        UINT mpirank;
+        UINT mpisize;
+        if (use_multi_cpu) {
+#ifdef _USE_MPI
+            MPIutil& mpiutil = MPIutil::get_inst();
+            mpirank = mpiutil.get_rank();
+            mpisize = mpiutil.get_size();
+#else
+            mpirank = 0;
+            mpisize = 1;
+#endif
+        } else {
+            mpirank = 0;
+            mpisize = 1;
+        }
+        if ((mpisize & (mpisize - 1))) {
+            throw MPISizeException(
+                "Error: QuantumStateBase::QuantumStateBase(UINT, bool, bool): "
+                "mpi-size must be power of 2");
+        }
+        UINT log_nodes = std::log2(mpisize);
+        if (use_multi_cpu &&
+            (qubit_count_ >= (log_nodes + 2))) {  // minimum inner_qc=2
+            this->_inner_qc = qubit_count_ - log_nodes;
+            this->_outer_qc = log_nodes;
+        } else {
+            this->_inner_qc = qubit_count_;
+            this->_outer_qc = 0;
+        }
+
+        this->_qubit_count = qubit_count_;
+        this->_dim = 1ULL << this->_inner_qc;
+        this->_is_state_vector = is_state_vector;
+        this->_device_number = mpirank;
+    }
+
     QuantumStateBase(
         UINT qubit_count_, bool is_state_vector, UINT device_number_)
         : qubit_count(_qubit_count),
+          inner_qc(_inner_qc),
+          outer_qc(_outer_qc),
           dim(_dim),
           classical_register(_classical_register),
           device_number(_device_number) {
         this->_qubit_count = qubit_count_;
+        this->_inner_qc = qubit_count_;
+        this->_outer_qc = 0;
         this->_dim = 1ULL << qubit_count_;
         this->_is_state_vector = is_state_vector;
         this->_device_number = device_number_;
     }
     /**
      * \~japanese-en デストラクタ
      */
@@ -303,17 +363,34 @@
      * @return 生成した文字列
      */
     virtual std::string to_string() const {
         std::stringstream os;
         ComplexVector eigen_state(this->dim);
         auto data = this->data_cpp();
         for (UINT i = 0; i < this->dim; ++i) eigen_state[i] = data[i];
+
         os << " *** Quantum State ***" << std::endl;
-        os << " * Qubit Count : " << this->qubit_count << std::endl;
-        os << " * Dimension   : " << this->dim << std::endl;
+        UINT myrank = 0;
+#ifdef _USE_MPI
+        if (this->outer_qc > 0) {
+            MPIutil& mpiutil = MPIutil::get_inst();
+            myrank = mpiutil.get_rank();
+        }
+#endif
+        if (myrank == 0) {
+            os << " * Qubit Count : " << this->qubit_count << std::endl;
+            os << " * Dimension   : " << this->dim << std::endl;
+#ifdef _USE_MPI
+            os << " * Local Qubit Count : " << this->inner_qc << std::endl;
+            os << " * Global Qubit Count : " << this->outer_qc << std::endl;
+#endif
+        }
+        if (this->outer_qc > 0) {
+            os << " * Rank : " << myrank << std::endl;
+        }
         os << " * State vector : \n" << eigen_state << std::endl;
         return os.str();
     }
 
     /**
      * \~japanese-en 量子状態のデバッグ情報を出力する。
      *
@@ -352,23 +429,57 @@
      */
     explicit QuantumStateCpu(UINT qubit_count_)
         : QuantumStateBase(qubit_count_, true) {
         this->_state_vector =
             reinterpret_cast<CPPCTYPE*>(allocate_quantum_state(this->_dim));
         initialize_quantum_state(this->data_c(), _dim);
     }
+
+    /**
+     * \~japanese-en コンストラクタ
+     *
+     * @param qubit_count_ 量子ビット数
+     * @param use_multi_cpu Flag to use multi CPUs
+     */
+    explicit QuantumStateCpu(UINT qubit_count_, bool use_multi_cpu)
+        : QuantumStateBase(qubit_count_, true, (int)use_multi_cpu) {
+        this->_state_vector =
+            reinterpret_cast<CPPCTYPE*>(allocate_quantum_state(this->_dim));
+#ifdef _USE_MPI
+        if (this->outer_qc > 0)
+            initialize_quantum_state_mpi(this->data_c(), _dim, this->outer_qc);
+        else
+#endif
+        {
+            initialize_quantum_state(this->data_c(), _dim);
+        }
+    }
+
     /**
      * \~japanese-en デストラクタ
      */
-    virtual ~QuantumStateCpu() { release_quantum_state(this->data_c()); }
+    virtual ~QuantumStateCpu() {
+#ifdef _USE_MPI
+        if (this->outer_qc > 0) {
+            MPIutil& mpiutil = MPIutil::get_inst();
+            mpiutil.release_workarea();
+        }
+#endif
+        release_quantum_state(this->data_c());
+    }
+
     /**
      * \~japanese-en 量子状態を計算基底の0状態に初期化する
      */
     virtual void set_zero_state() override {
+#ifdef _USE_MPI
+        initialize_quantum_state_mpi(this->data_c(), _dim, this->outer_qc);
+#else
         initialize_quantum_state(this->data_c(), _dim);
+#endif
     }
 
     /**
      * \~japanese-en 量子状態をノルム0の状態にする
      */
     virtual void set_zero_norm_state() override {
         set_zero_state();
@@ -385,41 +496,74 @@
             throw MatrixIndexOutOfRangeException(
                 "Error: QuantumStateCpu::set_computational_basis(ITYPE): "
                 "index of "
                 "computational basis must be smaller than 2^qubit_count");
         }
         set_zero_state();
         _state_vector[0] = 0.;
+#ifdef _USE_MPI
+        ITYPE myrank = 0;
+        if (this->outer_qc > 0) {
+            MPIutil& mpiutil = MPIutil::get_inst();
+            myrank = (ITYPE)mpiutil.get_rank();
+        }
+        if (this->outer_qc == 0 || (comp_basis >> this->inner_qc) == myrank) {
+            _state_vector[comp_basis & (this->_dim - 1)] = 1.;
+        }
+#else
         _state_vector[comp_basis] = 1.;
+#endif
     }
     /**
      * \~japanese-en 量子状態をHaar
      * randomにサンプリングされた量子状態に初期化する
      */
     virtual void set_Haar_random_state() override {
-        initialize_Haar_random_state_with_seed(
-            this->data_c(), _dim, random.int32());
+        UINT seed = random.int32();
+#ifdef _USE_MPI
+        if (this->outer_qc > 0) {
+            // すべてのrankで同一の結果を得るために、seedを共有する
+            MPIutil& mpiutil = MPIutil::get_inst();
+            if (mpiutil.get_size() > 1) mpiutil.s_u_bcast(&seed);
+        }
+#endif
+        set_Haar_random_state(seed);
     }
     /**
      * \~japanese-en 量子状態をシードを用いてHaar
      * randomにサンプリングされた量子状態に初期化する
      */
     virtual void set_Haar_random_state(UINT seed) override {
+#ifdef _USE_MPI
+        // 各rankで異なるseedを用いる必要がある
+        if (this->outer_qc > 0) {
+            MPIutil& mpiutil = MPIutil::get_inst();
+            seed += mpiutil.get_rank();
+        }
+        initialize_Haar_random_state_mpi_with_seed(
+            this->data_c(), _dim, this->outer_qc, seed);
+#else
         initialize_Haar_random_state_with_seed(this->data_c(), _dim, seed);
+#endif
     }
     /**
      * \~japanese-en
      * <code>target_qubit_index</code>の添え字の量子ビットを測定した時、0が観測される確率を計算する。
      *
      * 量子状態は変更しない。
      * @param target_qubit_index
      * @return double
      */
     virtual double get_zero_probability(
         UINT target_qubit_index) const override {
+#ifdef _USE_MPI
+        if (this->outer_qc > 0)
+            throw NotImplementedException(
+                "Error: get_zero_probability does not support multi-cpu");
+#endif
         if (target_qubit_index >= this->qubit_count) {
             throw QubitIndexOutOfRangeException(
                 "Error: QuantumStateCpu::get_zero_probability(UINT): index "
                 "of target qubit must be smaller than qubit_count");
         }
         return M0_prob(target_qubit_index, this->data_c(), _dim);
     }
@@ -428,14 +572,19 @@
      *
      * @param measured_values
      * 量子ビット数と同じ長さの0,1,2の配列。0,1はその値が観測され、2は測定をしないことを表す。
      * @return 計算された周辺確率
      */
     virtual double get_marginal_probability(
         std::vector<UINT> measured_values) const override {
+#ifdef _USE_MPI
+        if (this->outer_qc > 0)
+            throw NotImplementedException(
+                "Error: get_marginal_probability does not support multi-cpu");
+#endif
         if (measured_values.size() != this->qubit_count) {
             throw InvalidQubitCountException(
                 "Error: "
                 "QuantumStateCpu::get_marginal_probability(vector<UINT>): "
                 "the length of measured_values must be equal to qubit_count");
         }
 
@@ -454,25 +603,39 @@
     /**
      * \~japanese-en
      * 計算基底で測定した時得られる確率分布のエントロピーを計算する。
      *
      * @return エントロピー
      */
     virtual double get_entropy() const override {
-        return measurement_distribution_entropy(this->data_c(), _dim);
+        double entropy = measurement_distribution_entropy(this->data_c(), _dim);
+#ifdef _USE_MPI
+        MPIutil& mpiutil = MPIutil::get_inst();
+        if (this->outer_qc > 0) mpiutil.s_D_allreduce(&entropy);
+#endif
+        return entropy;
     }
 
     /**
      * \~japanese-en 量子状態のノルムを計算する
      *
      * 量子状態のノルムは非ユニタリなゲートを作用した時に小さくなる。
      * @return ノルム
      */
     virtual double get_squared_norm() const override {
-        return state_norm_squared(this->data_c(), _dim);
+        double norm;
+#ifdef _USE_MPI
+        if (this->outer_qc > 0) {
+            norm = state_norm_squared_mpi(this->data_c(), _dim);
+        } else
+#endif
+        {
+            norm = state_norm_squared(this->data_c(), _dim);
+        }
+        return norm;
     }
 
     /**
      * \~japanese-en 量子状態のノルムを計算する
      *
      * 量子状態のノルムは非ユニタリなゲートを作用した時に小さくなる。
      * @return ノルム
@@ -501,24 +664,33 @@
 
     /**
      * \~japanese-en バッファとして同じサイズの量子状態を作成する。
      *
      * @return 生成された量子状態
      */
     virtual QuantumStateCpu* allocate_buffer() const override {
-        QuantumStateCpu* new_state = new QuantumStateCpu(this->_qubit_count);
+        QuantumStateCpu* new_state;
+#ifdef _USE_MPI
+        if (this->outer_qc > 0)
+            new_state = new QuantumStateCpu(this->_qubit_count, true);
+        else
+            new_state = new QuantumStateCpu(this->_qubit_count, false);
+#else
+        new_state = new QuantumStateCpu(this->_qubit_count);
+#endif
         return new_state;
     }
     /**
      * \~japanese-en 自身の状態のディープコピーを生成する
      *
      * @return 自身のディープコピー
      */
     virtual QuantumStateCpu* copy() const override {
-        QuantumStateCpu* new_state = new QuantumStateCpu(this->_qubit_count);
+        QuantumStateCpu* new_state = this->allocate_buffer();
+
         memcpy(new_state->data_cpp(), _state_vector,
             (size_t)(sizeof(CPPCTYPE) * _dim));
         for (UINT i = 0; i < _classical_register.size(); ++i) {
             new_state->set_classical_value(i, _classical_register[i]);
         }
 
         return new_state;
@@ -528,23 +700,58 @@
      */
     virtual void load(const QuantumStateBase* _state) override {
         if (_state->qubit_count != this->qubit_count) {
             throw InvalidQubitCountException(
                 "Error: QuantumStateCpu::load(const QuantumStateBase*): "
                 "invalid qubit count");
         }
+        if (!_state->is_state_vector()) {
+            throw InoperatableQuantumStateTypeException(
+                "Error: QuantumStateCpu::load(const QuantumStateBase*): "
+                "cannot load DensityMatrix to StateVector");
+        }
 
         this->_classical_register = _state->classical_register;
         if (_state->get_device_name() == "gpu") {
             auto ptr = _state->duplicate_data_cpp();
             memcpy(this->data_cpp(), ptr, (size_t)(sizeof(CPPCTYPE) * _dim));
             free(ptr);
+#ifdef _USE_MPI
+        } else if (_state->outer_qc > 0) {
+            MPIutil& mpiutil = MPIutil::get_inst();
+            if (this->outer_qc > 0) {
+                if (_state->qubit_count != this->qubit_count) {
+                    throw InvalidQubitCountException(
+                        "Error: QuantumStateCpu::load(const QuantumStateBase*)"
+                        ": invalid global qubit count");
+                }
+                // load multicpu to multicpu
+                memcpy(this->data_cpp(), _state->data_cpp(),
+                    (size_t)(sizeof(CPPCTYPE) * _dim));
+            } else {
+                // load multicpu to cpu
+                mpiutil.m_DC_allgather(_state->data_cpp(), this->data_cpp(),
+                    _dim / mpiutil.get_size());
+            }
+#endif
         } else {
-            memcpy(this->data_cpp(), _state->data_cpp(),
-                (size_t)(sizeof(CPPCTYPE) * _dim));
+#ifdef _USE_MPI
+            if (this->outer_qc > 0) {
+                MPIutil& mpiutil = MPIutil::get_inst();
+                // load cpu to multicpu
+                ITYPE offs = _dim * mpiutil.get_rank();
+                memcpy(this->data_cpp(), _state->data_cpp() + offs,
+                    (size_t)(sizeof(CPPCTYPE) * _dim));
+            } else
+#endif
+            {
+                // load cpu to multicpu
+                memcpy(this->data_cpp(), _state->data_cpp(),
+                    (size_t)(sizeof(CPPCTYPE) * _dim));
+            }
         }
     }
     /**
      * \~japanese-en <code>state</code>の量子状態を自身へコピーする。
      */
     virtual void load(const std::vector<CPPCTYPE>& _state) override {
         if (_state.size() != _dim) {
@@ -563,15 +770,24 @@
         memcpy(this->data_cpp(), _state, (size_t)(sizeof(CPPCTYPE) * _dim));
     }
 
     /**
      * \~japanese-en
      * 量子状態が配置されているメモリを保持するデバイス名を取得する。
      */
-    virtual const std::string get_device_name() const override { return "cpu"; }
+    virtual const std::string get_device_name() const override {
+#ifdef _USE_MPI
+        if (this->outer_qc > 0) {
+            return "multi-cpu";
+        } else
+#endif
+        {
+            return "cpu";
+        }
+    }
 
     /**
      * \~japanese-en 量子状態のポインタをvoid*型として返す
      */
     virtual void* data() const override {
         return reinterpret_cast<void*>(this->_state_vector);
     }
@@ -603,39 +819,57 @@
         return new_data;
     }
 
     /**
      * \~japanese-en 量子状態を足しこむ
      */
     virtual void add_state(const QuantumStateBase* state) override {
+        if (!state->is_state_vector()) {
+            throw InoperatableQuantumStateTypeException(
+                "Error: QuantumStateCpu::add_state(const QuantumStateBase*): "
+                "cannot add DensityMatrix to StateVector");
+        }
         if (state->get_device_name() == "gpu") {
             throw QuantumStateProcessorException(
                 "State vector on GPU cannot be added to that on CPU");
         }
         state_add(state->data_c(), this->data_c(), this->dim);
     }
 
     /**
      * \~japanese-en 量子状態を足しこむ
      */
     virtual void add_state_with_coef(
         CPPCTYPE coef, const QuantumStateBase* state) override {
+        if (!state->is_state_vector()) {
+            throw InoperatableQuantumStateTypeException(
+                "Error: QuantumStateCpu::add_state_with_coef(CPPCTYPE, "
+                "const QuantumStateBase*): "
+                "cannot add DensityMatrix to StateVector");
+        }
         if (state->get_device_name() == "gpu") {
             std::cerr << "State vector on GPU cannot be added to that on CPU"
                       << std::endl;
             return;
         }
         state_add_with_coef(coef, state->data_c(), this->data_c(), this->dim);
     }
 
     /**
      * \~japanese-en 量子状態を足しこむ
      */
     virtual void add_state_with_coef_single_thread(
         CPPCTYPE coef, const QuantumStateBase* state) override {
+        if (!state->is_state_vector()) {
+            throw InoperatableQuantumStateTypeException(
+                "Error: "
+                "QuantumStateCpu::add_state_with_coef_single_thread(CPPCTYPE, "
+                "const QuantumStateBase*): "
+                "cannot add DensityMatrix to StateVector");
+        }
         if (state->get_device_name() == "gpu") {
             std::cerr << "State vector on GPU cannot be added to that on CPU"
                       << std::endl;
             return;
         }
         state_add_with_coef_single_thread(
             coef, state->data_c(), this->data_c(), this->dim);
@@ -659,14 +893,23 @@
     /**
      * \~japanese-en 量子状態を測定した際の計算基底のサンプリングを行う
      *
      * @param[in] sampling_count サンプリングを行う回数
      * @return サンプルされた値のリスト
      */
     virtual std::vector<ITYPE> sampling(UINT sampling_count) override {
+#ifdef _USE_MPI
+        if (this->outer_qc > 0) {
+            // すべてのrankで同一の結果を得るために、seedを共有する
+            UINT seed = random.int32();
+            MPIutil& mpiutil = MPIutil::get_inst();
+            if (mpiutil.get_size() > 1) mpiutil.s_u_bcast(&seed);
+            return this->sampling(sampling_count, seed);
+        }
+#endif
         std::vector<double> stacked_prob;
         std::vector<ITYPE> result;
         double sum = 0.;
         auto ptr = this->data_cpp();
         stacked_prob.push_back(0.);
         for (UINT i = 0; i < this->dim; ++i) {
             sum += norm(ptr[i]);
@@ -678,18 +921,75 @@
             auto ite =
                 std::lower_bound(stacked_prob.begin(), stacked_prob.end(), r);
             auto index = std::distance(stacked_prob.begin(), ite) - 1;
             result.push_back(index);
         }
         return result;
     }
+
     virtual std::vector<ITYPE> sampling(
         UINT sampling_count, UINT random_seed) override {
         random.set_seed(random_seed);
-        return this->sampling(sampling_count);
+        std::vector<ITYPE> result;
+
+#ifdef _USE_MPI
+        if (this->outer_qc > 0) {
+            std::vector<double> stacked_prob;
+            MPIutil& mpiutil = MPIutil::get_inst();
+            UINT mpirank = mpiutil.get_rank();
+            UINT mpisize = mpiutil.get_size();
+            double sum = 0.;
+            auto ptr = this->data_cpp();
+            // resize
+            stacked_prob.resize(this->dim + 1);
+            result.resize(sampling_count);
+
+            stacked_prob[0] = 0.;
+            for (UINT i = 0; i < this->dim; ++i) {
+                sum += norm(ptr[i]);
+                stacked_prob[i + 1] = sum;
+            }
+
+            double* sumrank_prob;
+            sumrank_prob = new double[mpisize];
+
+            mpiutil.s_D_allgather(sum, sumrank_prob);
+
+            double firstv = 0.;
+            for (UINT i = 0; i < mpirank; ++i) {
+                firstv += sumrank_prob[i];
+            }
+            for (ITYPE i = 0; i < this->dim + 1; ++i) {
+                stacked_prob[i] += firstv;
+            }
+            delete[] sumrank_prob;
+
+            for (UINT count = 0; count < sampling_count; ++count) {
+                double r = random.uniform();
+                auto ite = std::lower_bound(
+                    stacked_prob.begin(), stacked_prob.end(), r);
+                auto index = std::distance(stacked_prob.begin(), ite) - 1;
+                result[count] = index;
+            }
+
+            ITYPE geta = mpirank * this->dim;
+            for (UINT i = 0; i < sampling_count; ++i) {
+                if (result[i] == -1ULL or result[i] == this->dim)
+                    result[i] = 0ULL;
+                else
+                    result[i] += geta;
+            }
+            mpiutil.m_I_allreduce(result.data(), sampling_count);
+        } else
+#endif
+        {
+            result = this->sampling(sampling_count);
+        }
+
+        return result;
     }
     virtual boost::property_tree::ptree to_ptree() const override {
         boost::property_tree::ptree pt;
         pt.put("name", "QuantumState");
         pt.put("qubit_count", _qubit_count);
         pt.put_child(
             "classical_register", ptree::to_ptree(_classical_register));
```

### Comparing `qulacs-0.5.6/src/cppsim/state_dm.cpp` & `qulacs-0.6.0/src/cppsim/state_dm.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -27,29 +27,34 @@
         state->qubit_count, state->dim);
     return qs;
 }
 DensityMatrixCpu* partial_trace(
     const QuantumStateCpu* state, std::vector<UINT> target_traceout) {
     if (state->qubit_count <= target_traceout.size()) {
         throw InvalidQubitCountException(
-            "Error: drop_qubit(const QuantumState*, "
+            "Error: partial_trace(const QuantumState*, "
             "std::vector<UINT>): invalid qubit count");
     }
+    if (state->outer_qc > 0) {
+        throw NotImplementedException(
+            "Error: partial_trace(const QuantumState*, "
+            "std::vector<UINT>) using multi-cpu is not implemented");
+    }
     UINT qubit_count = state->qubit_count - (UINT)target_traceout.size();
     DensityMatrixCpu* qs = new DensityMatrixCpu(qubit_count);
     dm_state_partial_trace_from_state_vector(target_traceout.data(),
         (UINT)(target_traceout.size()), state->data_c(), qs->data_c(),
         state->dim);
     return qs;
 }
 DensityMatrixCpu* partial_trace(
     const DensityMatrixCpu* state, std::vector<UINT> target_traceout) {
     if (state->qubit_count <= target_traceout.size()) {
         throw InvalidQubitCountException(
-            "Error: drop_qubit(const QuantumState*, "
+            "Error: partial_trace(const QuantumState*, "
             "std::vector<UINT>): invalid qubit count");
     }
     UINT qubit_count = state->qubit_count - (UINT)target_traceout.size();
     DensityMatrixCpu* qs = new DensityMatrixCpu(qubit_count);
     dm_state_partial_trace_from_density_matrix(target_traceout.data(),
         (UINT)target_traceout.size(), state->data_c(), qs->data_c(),
         state->dim);
@@ -58,14 +63,20 @@
 DensityMatrixCpu* make_mixture(CPPCTYPE prob1, const QuantumStateBase* state1,
     CPPCTYPE prob2, const QuantumStateBase* state2) {
     if (state1->qubit_count != state2->qubit_count) {
         throw InvalidQubitCountException(
             "Error: make_mixture(CPPCTYPE, const QuantumStateBase*, "
             "CPPCTYPE, const QuantumStateBase*): invalid qubit count");
     }
+    if ((state1->outer_qc > 0) || (state2->outer_qc > 0)) {
+        throw NotImplementedException(
+            "Error: make_mixture(CPPCTYPE, const QuantumStateBase*, "
+            "CPPCTYPE, const QuantumStateBase*): invalid qubit count "
+            "using multi-cpu is not implemented");
+    }
     UINT qubit_count = state1->qubit_count;
     DensityMatrixCpu* dm1 = new DensityMatrixCpu(qubit_count);
     dm1->load(state1);
     DensityMatrixCpu* dm2 = new DensityMatrixCpu(qubit_count);
     dm2->load(state2);
     DensityMatrixCpu* mixture = new DensityMatrixCpu(qubit_count);
     mixture->set_zero_norm_state();
```

### Comparing `qulacs-0.5.6/src/cppsim/state_dm.hpp` & `qulacs-0.6.0/src/cppsim/state_dm.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,19 @@
      */
     virtual void load(const QuantumStateBase* _state) override {
         if (_state->qubit_count != this->qubit_count) {
             throw InvalidQubitCountException(
                 "Error: DensityMatrixCpu::load(const QuantumStateBase*): "
                 "invalid qubit count");
         }
+        if (_state->outer_qc > 0) {
+            throw NotImplementedException(
+                "Error: DensityMatrixCpu::load(const QuantumStateBase*) "
+                "using multi-cpu is not implemented");
+        }
         if (_state->is_state_vector()) {
             if (_state->get_device_name() == "gpu") {
                 auto ptr = _state->duplicate_data_c();
                 dm_initialize_with_pure_state(this->data_c(), ptr, dim);
                 free(ptr);
             } else {
                 dm_initialize_with_pure_state(
```

### Comparing `qulacs-0.5.6/src/cppsim/state_gpu.cpp` & `qulacs-0.6.0/src/cppsim/state_gpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/state_gpu.hpp` & `qulacs-0.6.0/src/cppsim/state_gpu.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,19 @@
             new_state->set_classical_value(i, _classical_register[i]);
         return new_state;
     }
     /**
      * \~japanese-en <code>state</code>の量子状態を自身へコピーする。
      */
     virtual void load(const QuantumStateBase* _state) override {
+        if (!_state->is_state_vector()) {
+            throw InoperatableQuantumStateTypeException(
+                "Error: QuantumStateGpu::load(const QuantumStateBase*): "
+                "cannot load DensityMatrix to StateVector");
+        }
         if (_state->get_device_name() == "gpu") {
             copy_quantum_state_from_device_to_device(
                 this->data(), _state->data(), dim, _cuda_stream, device_number);
         } else {
             this->load(_state->data_cpp());
         }
         this->_classical_register = _state->classical_register;
@@ -285,36 +290,54 @@
         return _copy_state;
     }
 
     /**
      * \~japanese-en 量子状態を足しこむ
      */
     virtual void add_state(const QuantumStateBase* state) override {
+        if (!state->is_state_vector()) {
+            throw InoperatableQuantumStateTypeException(
+                "Error: QuantumStateGpu::add_state(const QuantumStateBase*): "
+                "cannot add DensityMatrix to StateVector");
+        }
         state_add_host(state->data(), this->data(), this->dim, _cuda_stream,
             device_number);
     }
 
     /**
      * \~japanese-en 量子状態を足しこむ (とりあえずの実装なので遅い)
      */
     virtual void add_state_with_coef(
         CPPCTYPE coef, const QuantumStateBase* state) override {
+        if (!state->is_state_vector()) {
+            throw InoperatableQuantumStateTypeException(
+                "Error: QuantumStateGpu::add_state_with_coef(CPPCTYPE, "
+                "const QuantumStateBase*): "
+                "cannot add DensityMatrix to StateVector");
+        }
         state_multiply_host(
             coef, this->data(), this->dim, _cuda_stream, device_number);
         state_add_host(state->data(), this->data(), this->dim, _cuda_stream,
             device_number);
         state_multiply_host(CPPCTYPE(1) / coef, this->data(), this->dim,
             _cuda_stream, device_number);
     }
 
     /**
      * \~japanese-en 量子状態を足しこむ (とりあえずの実装なので遅い)
      */
     virtual void add_state_with_coef_single_thread(
         CPPCTYPE coef, const QuantumStateBase* state) override {
+        if (!state->is_state_vector()) {
+            throw InoperatableQuantumStateTypeException(
+                "Error: "
+                "QuantumStateGpu::add_state_with_coef_single_thread(CPPCTYPE, "
+                "const QuantumStateBase*): "
+                "cannot add DensityMatrix to StateVector");
+        }
         state_multiply_host(CPPCTYPE(1) / coef, this->data(), this->dim,
             _cuda_stream, device_number);
         state_add_host(state->data(), this->data(), this->dim, _cuda_stream,
             device_number);
         state_multiply_host(
             coef, this->data(), this->dim, _cuda_stream, device_number);
     }
```

### Comparing `qulacs-0.5.6/src/cppsim/type.hpp` & `qulacs-0.6.0/src/cppsim/type.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/utility.cpp` & `qulacs-0.6.0/src/cppsim/utility.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/cppsim/utility.hpp` & `qulacs-0.6.0/src/cppsim/utility.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/CMakeLists.txt` & `qulacs-0.6.0/src/csim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/constant.cpp` & `qulacs-0.6.0/src/csim/constant.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/constant.hpp` & `qulacs-0.6.0/src/csim/constant.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/init_ops.hpp` & `qulacs-0.6.0/src/csim/init_ops.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -17,7 +17,15 @@
  */
 DllExport void initialize_quantum_state(CTYPE* state, ITYPE dim);
 
 DllExport void initialize_Haar_random_state(CTYPE* state, ITYPE dim);
 
 DllExport void initialize_Haar_random_state_with_seed(
     CTYPE* state, ITYPE dim, UINT seed);
+
+#ifdef _USE_MPI
+DllExport void initialize_quantum_state_mpi(
+    CTYPE* state, ITYPE dim, UINT outer_qc);
+#endif
+
+DllExport void initialize_Haar_random_state_mpi_with_seed(
+    CTYPE* state, ITYPE dim, UINT outer_qc, UINT seed);
```

### Comparing `qulacs-0.5.6/src/csim/init_ops_fill.cpp` & `qulacs-0.6.0/src/csim/init_ops_fill.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 #include <limits.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <time.h>
 
+#include "MPIutil.hpp"
 #include "init_ops.hpp"
 #include "utility.hpp"
-#ifdef _OPENMP
-#include <omp.h>
-#endif
 
-// state initialization
-void initialize_quantum_state_parallel(CTYPE* state, ITYPE dim);
 void initialize_quantum_state(CTYPE* state, ITYPE dim) {
 #ifdef _OPENMP
     OMPutil::get_inst().set_qulacs_num_threads(dim, 15);
+#pragma omp parallel for
 #endif
-
-    initialize_quantum_state_parallel(state, dim);
-
+    for (ITYPE index = 0; index < dim; ++index) {
+        state[index] = 0;
+    }
 #ifdef _OPENMP
     OMPutil::get_inst().reset_qulacs_num_threads();
 #endif
+
+    state[0] = 1.0;
 }
 
-void initialize_quantum_state_parallel(CTYPE* state, ITYPE dim) {
-    ITYPE index;
+#ifdef _USE_MPI
+void initialize_quantum_state_mpi(CTYPE* state, ITYPE dim, UINT outer_qc) {
 #ifdef _OPENMP
+    OMPutil::get_inst().set_qulacs_num_threads(dim, 10);
 #pragma omp parallel for
 #endif
-    for (index = 0; index < dim; ++index) {
+    for (ITYPE index = 0; index < dim; ++index) {
         state[index] = 0;
     }
-    state[0] = 1.0;
+#ifdef _OPENMP
+    OMPutil::get_inst().reset_qulacs_num_threads();
+#endif
+
+    MPIutil& mpiutil = MPIutil::get_inst();
+    if (outer_qc == 0 || mpiutil.get_rank() == 0) state[0] = 1.0;
 }
+#endif
```

### Comparing `qulacs-0.5.6/src/csim/init_ops_random.cpp` & `qulacs-0.6.0/src/csim/init_ops_random.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,128 +1,123 @@
 #include <limits.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <time.h>
 
+#include "MPIutil.hpp"
+#include "csim/utility.hpp"
 #include "init_ops.hpp"
-#include "utility.hpp"
-#ifdef _OPENMP
-#include <omp.h>
-#endif
 
 // state randomization
 unsigned long xor_shift(unsigned long* state);
 double random_uniform(unsigned long* state);
 double random_normal(unsigned long* state);
-void initialize_Haar_random_state_with_seed_single(
-    CTYPE* state, ITYPE dim, UINT seed);
 void initialize_Haar_random_state_with_seed_parallel(
-    CTYPE* state, ITYPE dim, UINT seed);
+    CTYPE* state, ITYPE dim, UINT outer_qc, UINT seed);
 
 void initialize_Haar_random_state(CTYPE* state, ITYPE dim) {
     initialize_Haar_random_state_with_seed(state, dim, (unsigned)time(NULL));
 }
+
 void initialize_Haar_random_state_with_seed(
     CTYPE* state, ITYPE dim, UINT seed) {
+    initialize_Haar_random_state_mpi_with_seed(state, dim, 0, seed);
+}
+
+void initialize_Haar_random_state_mpi_with_seed(
+    CTYPE* state, ITYPE dim, UINT outer_qc, UINT seed) {
 #ifdef _OPENMP
-    UINT threshold = 8;
-    if (dim < (((ITYPE)1) << threshold)) {
-        initialize_Haar_random_state_with_seed_single(state, dim, seed);
-    } else {
-        initialize_Haar_random_state_with_seed_parallel(state, dim, seed);
-    }
-#else
-    initialize_Haar_random_state_with_seed_single(state, dim, seed);
+    OMPutil::get_inst().set_qulacs_num_threads(dim, 8);
+#endif
+    initialize_Haar_random_state_with_seed_parallel(state, dim, outer_qc, seed);
+#ifdef _OPENMP
+    OMPutil::get_inst().reset_qulacs_num_threads();
 #endif
 }
 
-// single thread
-void initialize_Haar_random_state_with_seed_single(
-    CTYPE* state, ITYPE dim, UINT seed) {
-    const int ignore_first = 40;
-    double norm = 0.;
-    unsigned long random_state[4];
-    srand(seed);
-    random_state[0] = rand();
-    random_state[1] = rand();
-    random_state[2] = rand();
-    random_state[3] = rand();
-    for (int i = 0; i < ignore_first; ++i) xor_shift(random_state);
-    for (ITYPE index = 0; index < dim; ++index) {
-        double r1, r2;
-        r1 = random_normal(random_state);
-        r2 = random_normal(random_state);
-        state[index] = r1 + 1.i * r2;
-        norm += r1 * r1 + r2 * r2;
-    }
-    norm = sqrt(norm);
-    for (ITYPE index = 0; index < dim; ++index) {
-        state[index] /= norm;
-    }
-}
-#ifdef _OPENMP
 void initialize_Haar_random_state_with_seed_parallel(
-    CTYPE* state, ITYPE dim, UINT seed) {
+    CTYPE* state, ITYPE dim, UINT outer_qc, UINT seed) {
+#ifndef _USE_MPI  // unused parameter if MPI is not used
+    (void)outer_qc;
+#endif
     // multi thread
+#ifdef _OPENMP
     OMPutil::get_inst().set_qulacs_num_threads(dim, 10);
-    const int ignore_first = 40;
     const UINT thread_count = omp_get_max_threads();
+#else
+    const UINT thread_count = 1;
+#endif
+    const int ignore_first = 40;
     const ITYPE block_size = dim / thread_count;
     const ITYPE residual = dim % thread_count;
 
     unsigned long* random_state_list =
         (unsigned long*)malloc(sizeof(unsigned long) * 4 * thread_count);
     srand(seed);
     for (UINT i = 0; i < 4 * thread_count; ++i) {
         random_state_list[i] = rand();
     }
 
     double* norm_list = (double*)malloc(sizeof(double) * thread_count);
     for (UINT i = 0; i < thread_count; ++i) {
         norm_list[i] = 0;
     }
+#ifdef _OPENMP
 #pragma omp parallel
+#endif
     {
+#ifdef _OPENMP
         UINT thread_id = omp_get_thread_num();
+#else
+        UINT thread_id = 0;
+#endif
         unsigned long* my_random_state = random_state_list + 4 * thread_id;
         ITYPE start_index = block_size * thread_id +
                             (residual > thread_id ? thread_id : residual);
         ITYPE end_index =
             block_size * (thread_id + 1) +
             (residual > (thread_id + 1) ? (thread_id + 1) : residual);
         ITYPE index;
 
         // ignore first randoms
         for (int i = 0; i < ignore_first; ++i) xor_shift(my_random_state);
 
         for (index = start_index; index < end_index; ++index) {
             double r1, r2;
-            r1 = r2 = 1;
             r1 = random_normal(my_random_state);
             r2 = random_normal(my_random_state);
             state[index] = r1 + 1.i * r2;
             norm_list[thread_id] += r1 * r1 + r2 * r2;
         }
     }
 
     double normalizer = 0.;
     for (UINT i = 0; i < thread_count; ++i) {
         normalizer += norm_list[i];
     }
+#ifdef _USE_MPI
+    if (outer_qc > 0) {
+        MPIutil& m = MPIutil::get_inst();
+        m.s_D_allreduce(&normalizer);
+    }
+#endif
     normalizer = 1. / sqrt(normalizer);
 
+#ifdef _OPENMP
 #pragma omp parallel for
+#endif
     for (ITYPE index = 0; index < dim; ++index) {
         state[index] *= normalizer;
     }
+#ifdef _OPENMP
     OMPutil::get_inst().reset_qulacs_num_threads();
+#endif
     free(random_state_list);
     free(norm_list);
 }
-#endif
 
 unsigned long xor_shift(unsigned long* state) {
     unsigned long t;
     t = (state[0] ^ (state[0] << 11));
     state[0] = state[1];
     state[1] = state[2];
     state[2] = state[3];
```

### Comparing `qulacs-0.5.6/src/csim/memory_ops.cpp` & `qulacs-0.6.0/src/csim/memory_ops.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/memory_ops_dm.cpp` & `qulacs-0.6.0/src/csim/memory_ops_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/memory_ops_dm.hpp` & `qulacs-0.6.0/src/csim/memory_ops_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/stat_ops.cpp` & `qulacs-0.6.0/src/csim/update_ops_matrix_phase_single.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,107 +1,118 @@
-#include "stat_ops.hpp"
 
-#include <math.h>
-#include <stdio.h>
-#include <stdlib.h>
-#include <string.h>
-
-#include "constant.hpp"
+#include "MPIutil.hpp"
+#include "update_ops.hpp"
 #include "utility.hpp"
 
-// calculate norm
-double state_norm_squared(const CTYPE* state, ITYPE dim) {
-    ITYPE index;
-    double norm = 0;
-#ifdef _OPENMP
-    OMPutil::get_inst().set_qulacs_num_threads(dim, 10);
-#pragma omp parallel for reduction(+ : norm)
+#ifdef _USE_SIMD
+#ifdef _MSC_VER
+#include <intrin.h>
+#else
+#include <x86intrin.h>
 #endif
-    for (index = 0; index < dim; ++index) {
-        norm += pow(_cabs(state[index]), 2);
-    }
+#endif
+
+void single_qubit_phase_gate(
+    UINT target_qubit_index, CTYPE phase, CTYPE* state, ITYPE dim) {
 #ifdef _OPENMP
-    OMPutil::get_inst().reset_qulacs_num_threads();
+    OMPutil::get_inst().set_qulacs_num_threads(dim, 12);
 #endif
-    return norm;
-}
 
-// calculate norm
-double state_norm_squared_single_thread(const CTYPE* state, ITYPE dim) {
-    ITYPE index;
-    double norm = 0;
-    for (index = 0; index < dim; ++index) {
-        norm += pow(_cabs(state[index]), 2);
-    }
-    return norm;
-}
+#ifdef _USE_SIMD
+    single_qubit_phase_gate_parallel_simd(
+        target_qubit_index, phase, state, dim);
+#else
+    single_qubit_phase_gate_parallel_unroll(
+        target_qubit_index, phase, state, dim);
+#endif
 
-// calculate inner product of two state vector
-CTYPE
-state_inner_product(const CTYPE* state_bra, const CTYPE* state_ket, ITYPE dim) {
-    double real_sum = 0.;
-    double imag_sum = 0.;
-    ITYPE index;
-#ifdef _OPENMP
-    OMPutil::get_inst().set_qulacs_num_threads(dim, 10);
-#pragma omp parallel for reduction(+ : real_sum, imag_sum)
-#endif
-    for (index = 0; index < dim; ++index) {
-        CTYPE value;
-        value += conj(state_bra[index]) * state_ket[index];
-        real_sum += _creal(value);
-        imag_sum += _cimag(value);
-    }
 #ifdef _OPENMP
     OMPutil::get_inst().reset_qulacs_num_threads();
 #endif
-    return real_sum + 1.i * imag_sum;
 }
 
-void state_tensor_product(const CTYPE* state_left, ITYPE dim_left,
-    const CTYPE* state_right, ITYPE dim_right, CTYPE* state_dst) {
-    ITYPE index_left, index_right;
-    for (index_left = 0; index_left < dim_left; ++index_left) {
-        CTYPE val_left = state_left[index_left];
-        for (index_right = 0; index_right < dim_right; ++index_right) {
-            state_dst[index_left * dim_right + index_right] =
-                val_left * state_right[index_right];
+void single_qubit_phase_gate_parallel_unroll(
+    UINT target_qubit_index, CTYPE phase, CTYPE* state, ITYPE dim) {
+    // target tmask
+    const ITYPE mask = 1ULL << target_qubit_index;
+    const ITYPE low_mask = mask - 1;
+    const ITYPE high_mask = ~low_mask;
+
+    // loop varaibles
+    const ITYPE loop_dim = dim / 2;
+    if (target_qubit_index == 0) {
+        ITYPE state_index;
+#ifdef _OPENMP
+#pragma omp parallel for
+#endif
+        for (state_index = 1; state_index < dim; state_index += 2) {
+            state[state_index] *= phase;
         }
-    }
-}
-void state_permutate_qubit(const UINT* qubit_order, const CTYPE* state_src,
-    CTYPE* state_dst, UINT qubit_count, ITYPE dim) {
-    ITYPE index;
-    for (index = 0; index < dim; ++index) {
-        ITYPE src_index = 0;
-        for (UINT qubit_index = 0; qubit_index < qubit_count; ++qubit_index) {
-            if ((index >> qubit_index) % 2) {
-                src_index += 1ULL << qubit_order[qubit_index];
-            }
+    } else {
+        ITYPE state_index;
+#ifdef _OPENMP
+#pragma omp parallel for
+#endif
+        for (state_index = 0; state_index < loop_dim; state_index += 2) {
+            ITYPE basis = (state_index & low_mask) +
+                          ((state_index & high_mask) << 1) + mask;
+            state[basis] *= phase;
+            state[basis + 1] *= phase;
         }
-        state_dst[index] = state_src[src_index];
     }
 }
 
-void state_drop_qubits(const UINT* target, const UINT* projection,
-    UINT target_count, const CTYPE* state_src, CTYPE* state_dst, ITYPE dim) {
-    ITYPE dst_dim = dim >> target_count;
-    UINT* sorted_target = create_sorted_ui_list(target, target_count);
-    ITYPE projection_mask = 0;
-    for (UINT target_index = 0; target_index < target_count; ++target_index) {
-        projection_mask ^= (projection[target_index] << target[target_index]);
+#ifdef _USE_SIMD
+void single_qubit_phase_gate_parallel_simd(
+    UINT target_qubit_index, CTYPE phase, CTYPE* state, ITYPE dim) {
+    // target tmask
+    const ITYPE mask = 1ULL << target_qubit_index;
+    const ITYPE low_mask = mask - 1;
+    const ITYPE high_mask = ~low_mask;
+
+    // loop varaibles
+    const ITYPE loop_dim = dim / 2;
+    if (target_qubit_index == 0) {
+        ITYPE state_index;
+#ifdef _OPENMP
+#pragma omp parallel for
+#endif
+        for (state_index = 1; state_index < dim; state_index += 2) {
+            state[state_index] *= phase;
+        }
+    } else {
+        ITYPE state_index;
+        __m256d mv0 = _mm256_set_pd(
+            -_cimag(phase), _creal(phase), -_cimag(phase), _creal(phase));
+        __m256d mv1 = _mm256_set_pd(
+            _creal(phase), _cimag(phase), _creal(phase), _cimag(phase));
+#ifdef _OPENMP
+#pragma omp parallel for
+#endif
+        for (state_index = 0; state_index < loop_dim; state_index += 2) {
+            ITYPE basis = (state_index & low_mask) +
+                          ((state_index & high_mask) << 1) + mask;
+            double* ptr = (double*)(state + basis);
+            __m256d data = _mm256_loadu_pd(ptr);
+            __m256d data0 = _mm256_mul_pd(data, mv0);
+            __m256d data1 = _mm256_mul_pd(data, mv1);
+            data = _mm256_hadd_pd(data0, data1);
+            _mm256_storeu_pd(ptr, data);
+        }
     }
+}
+#endif
 
-    ITYPE index;
-    for (index = 0; index < dst_dim; ++index) {
-        ITYPE src_index = index;
-        for (UINT target_index = 0; target_index < target_count;
-             ++target_index) {
-            UINT insert_index = sorted_target[target_index];
-            src_index = insert_zero_to_basis_index(
-                src_index, 1ULL << insert_index, insert_index);
-        }
-        src_index ^= projection_mask;
-        state_dst[index] = state_src[src_index];
+#ifdef _USE_MPI
+void single_qubit_phase_gate_mpi(UINT target_qubit_index, CTYPE phase,
+    CTYPE* state, ITYPE dim, UINT inner_qc) {
+    if (target_qubit_index < inner_qc) {
+        single_qubit_phase_gate(target_qubit_index, phase, state, dim);
+    } else {
+        int target_rank_bit = 1 << (target_qubit_index - inner_qc);
+        int rank = MPIutil::get_inst().get_rank();
+        if (rank & target_rank_bit) {
+            state_multiply(phase, state, dim);
+        }  // if else, nothing to do.
     }
-    free(sorted_target);
 }
+#endif
```

### Comparing `qulacs-0.5.6/src/csim/stat_ops.hpp` & `qulacs-0.6.0/src/csim/stat_ops.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 #pragma once
 
 #include "type.hpp"
 
 DllExport double state_norm_squared(const CTYPE* state, ITYPE dim);
 DllExport double state_norm_squared_single_thread(
     const CTYPE* state, ITYPE dim);
+DllExport double state_norm_squared_mpi(const CTYPE* state, ITYPE dim);
+
 DllExport double measurement_distribution_entropy(
     const CTYPE* state, ITYPE dim);
 DllExport CTYPE state_inner_product(
     const CTYPE* state_bra, const CTYPE* state_ket, ITYPE dim);
+DllExport CTYPE state_inner_product_mpi(const CTYPE* state_bra,
+    const CTYPE* state_ket, ITYPE dim_bra, ITYPE dim_ket);
 
 DllExport void state_tensor_product(const CTYPE* state_left, ITYPE dim_left,
     const CTYPE* state_right, ITYPE dim_right, CTYPE* state_dst);
 DllExport void state_permutate_qubit(const UINT* qubit_order,
     const CTYPE* state_src, CTYPE* state_dst, UINT qubit_count, ITYPE dim);
 DllExport void state_drop_qubits(const UINT* target, const UINT* projection,
     UINT target_count, const CTYPE* state_src, CTYPE* state_dst, ITYPE dim);
@@ -40,17 +44,14 @@
     const CTYPE* state_bra, const CTYPE* state_ket, ITYPE dim);
 DllExport CTYPE transition_amplitude_multi_qubit_Pauli_operator_partial_list(
     const UINT* target_qubit_index_list, const UINT* Pauli_operator_type_list,
     UINT target_qubit_index_count, const CTYPE* state_bra,
     const CTYPE* state_ket, ITYPE dim);
 
 DllExport double
-expectation_value_multi_qubit_Pauli_operator_XZ_mask_single_thread(
-    ITYPE bit_flip_mask, ITYPE phase_flip_mask, UINT global_phase_90rot_count,
-    UINT pivot_qubit_index, const CTYPE* state, ITYPE dim);
-DllExport double
-expectation_value_multi_qubit_Pauli_operator_Z_mask_single_thread(
-    ITYPE phase_flip_mask, const CTYPE* state, ITYPE dim);
-DllExport double
 expectation_value_multi_qubit_Pauli_operator_partial_list_single_thread(
     const UINT* target_qubit_index_list, const UINT* Pauli_operator_type_list,
     UINT target_qubit_index_count, const CTYPE* state, ITYPE dim);
+DllExport double expectation_value_multi_qubit_Pauli_operator_partial_list_mpi(
+    const UINT* target_qubit_index_list, const UINT* Pauli_operator_type_list,
+    UINT target_qubit_index_count, const CTYPE* state, ITYPE dim, UINT outer_qc,
+    UINT inner_qc);
```

### Comparing `qulacs-0.5.6/src/csim/stat_ops_dm.cpp` & `qulacs-0.6.0/src/csim/stat_ops_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/stat_ops_dm.hpp` & `qulacs-0.6.0/src/csim/stat_ops_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/stat_ops_expectation_value.cpp` & `qulacs-0.6.0/src/csim/update_ops_named_SWAP.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,274 +1,304 @@
-#include <math.h>
-#include <stdio.h>
-#include <stdlib.h>
-#include <string.h>
 
+#include <cstring>
+
+#include "MPIutil.hpp"
 #include "constant.hpp"
-#include "stat_ops.hpp"
+#include "update_ops.hpp"
 #include "utility.hpp"
-
-double expectation_value_X_Pauli_operator(
-    UINT target_qubit_index, const CTYPE* state, ITYPE dim);
-double expectation_value_Y_Pauli_operator(
-    UINT target_qubit_index, const CTYPE* state, ITYPE dim);
-double expectation_value_Z_Pauli_operator(
-    UINT target_qubit_index, const CTYPE* state, ITYPE dim);
-double expectation_value_multi_qubit_Pauli_operator_XZ_mask(ITYPE bit_flip_mask,
-    ITYPE phase_flip_mask, UINT global_phase_90rot_count,
-    UINT pivot_qubit_index, const CTYPE* state, ITYPE dim);
-double expectation_value_multi_qubit_Pauli_operator_Z_mask(
-    ITYPE phase_flip_mask, const CTYPE* state, ITYPE dim);
-
-// calculate expectation value of X on target qubit
-double expectation_value_X_Pauli_operator(
-    UINT target_qubit_index, const CTYPE* state, ITYPE dim) {
-    const ITYPE loop_dim = dim / 2;
-    const ITYPE mask = 1ULL << target_qubit_index;
-    ITYPE state_index;
-    double sum = 0.;
-#ifdef _OPENMP
-    OMPutil::get_inst().set_qulacs_num_threads(dim, 10);
-#pragma omp parallel for reduction(+ : sum)
-#endif
-    for (state_index = 0; state_index < loop_dim; ++state_index) {
-        ITYPE basis_0 =
-            insert_zero_to_basis_index(state_index, mask, target_qubit_index);
-        ITYPE basis_1 = basis_0 ^ mask;
-        sum += _creal(conj(state[basis_0]) * state[basis_1]) * 2;
-    }
 #ifdef _OPENMP
-    OMPutil::get_inst().reset_qulacs_num_threads();
+#include <omp.h>
 #endif
-    return sum;
-}
 
-// calculate expectation value of Y on target qubit
-double expectation_value_Y_Pauli_operator(
-    UINT target_qubit_index, const CTYPE* state, ITYPE dim) {
-    const ITYPE loop_dim = dim / 2;
-    const ITYPE mask = 1ULL << target_qubit_index;
-    ITYPE state_index;
-    double sum = 0.;
-#ifdef _OPENMP
-    OMPutil::get_inst().set_qulacs_num_threads(dim, 10);
-#pragma omp parallel for reduction(+ : sum)
+#ifdef _USE_SIMD
+#ifdef _MSC_VER
+#include <intrin.h>
+#else
+#include <x86intrin.h>
 #endif
-    for (state_index = 0; state_index < loop_dim; ++state_index) {
-        ITYPE basis_0 =
-            insert_zero_to_basis_index(state_index, mask, target_qubit_index);
-        ITYPE basis_1 = basis_0 ^ mask;
-        sum += _cimag(conj(state[basis_0]) * state[basis_1]) * 2;
-    }
-#ifdef _OPENMP
-    OMPutil::get_inst().reset_qulacs_num_threads();
 #endif
-    return sum;
-}
 
-// calculate expectation value of Z on target qubit
-double expectation_value_Z_Pauli_operator(
-    UINT target_qubit_index, const CTYPE* state, ITYPE dim) {
-    const ITYPE loop_dim = dim;
-    ITYPE state_index;
-    double sum = 0.;
+void SWAP_gate(UINT target_qubit_index_0, UINT target_qubit_index_1,
+    CTYPE* state, ITYPE dim) {
 #ifdef _OPENMP
-    OMPutil::get_inst().set_qulacs_num_threads(dim, 10);
-#pragma omp parallel for reduction(+ : sum)
+    OMPutil::get_inst().set_qulacs_num_threads(dim, 13);
 #endif
-    for (state_index = 0; state_index < loop_dim; ++state_index) {
-        int sign = 1 - 2 * ((state_index >> target_qubit_index) % 2);
-        sum += _creal(conj(state[state_index]) * state[state_index]) * sign;
-    }
+
+#ifdef _USE_SIMD
+    SWAP_gate_parallel_simd(
+        target_qubit_index_0, target_qubit_index_1, state, dim);
+#elif defined(_USE_SVE)
+    SWAP_gate_parallel_sve(
+        target_qubit_index_0, target_qubit_index_1, state, dim);
+#else
+    SWAP_gate_parallel_unroll(
+        target_qubit_index_0, target_qubit_index_1, state, dim);
+#endif
+
 #ifdef _OPENMP
     OMPutil::get_inst().reset_qulacs_num_threads();
 #endif
-    return sum;
 }
 
-// calculate expectation value for single-qubit pauli operator
-double expectation_value_single_qubit_Pauli_operator(UINT target_qubit_index,
-    UINT Pauli_operator_type, const CTYPE* state, ITYPE dim) {
-    if (Pauli_operator_type == 0) {
-        return state_norm_squared(state, dim);
-    } else if (Pauli_operator_type == 1) {
-        return expectation_value_X_Pauli_operator(
-            target_qubit_index, state, dim);
-    } else if (Pauli_operator_type == 2) {
-        return expectation_value_Y_Pauli_operator(
-            target_qubit_index, state, dim);
-    } else if (Pauli_operator_type == 3) {
-        return expectation_value_Z_Pauli_operator(
-            target_qubit_index, state, dim);
-    } else {
-        fprintf(
-            stderr, "invalid expectation value of pauli operator is called");
-        exit(1);
-    }
-}
+void SWAP_gate_parallel_unroll(UINT target_qubit_index_0,
+    UINT target_qubit_index_1, CTYPE* state, ITYPE dim) {
+    const ITYPE loop_dim = dim / 4;
+
+    const ITYPE mask_0 = 1ULL << target_qubit_index_0;
+    const ITYPE mask_1 = 1ULL << target_qubit_index_1;
+    const ITYPE mask = mask_0 + mask_1;
+
+    const UINT min_qubit_index =
+        get_min_ui(target_qubit_index_0, target_qubit_index_1);
+    const UINT max_qubit_index =
+        get_max_ui(target_qubit_index_0, target_qubit_index_1);
+    const ITYPE min_qubit_mask = 1ULL << min_qubit_index;
+    const ITYPE max_qubit_mask = 1ULL << (max_qubit_index - 1);
+    const ITYPE low_mask = min_qubit_mask - 1;
+    const ITYPE mid_mask = (max_qubit_mask - 1) ^ low_mask;
+    const ITYPE high_mask = ~(max_qubit_mask - 1);
 
-// calculate expectation value of multi-qubit Pauli operator on qubits.
-// bit-flip mask : the n-bit binary string of which the i-th element is 1 iff
-// the i-th pauli operator is X or Y phase-flip mask : the n-bit binary string
-// of which the i-th element is 1 iff the i-th pauli operator is Y or Z We
-// assume bit-flip mask is nonzero, namely, there is at least one X or Y
-// operator. the pivot qubit is any qubit index which has X or Y To generate
-// bit-flip mask and phase-flip mask, see get_masks_*_list at utility.h
-double expectation_value_multi_qubit_Pauli_operator_XZ_mask(ITYPE bit_flip_mask,
-    ITYPE phase_flip_mask, UINT global_phase_90rot_count,
-    UINT pivot_qubit_index, const CTYPE* state, ITYPE dim) {
-    const ITYPE loop_dim = dim / 2;
-    const ITYPE pivot_mask = 1ULL << pivot_qubit_index;
-    ITYPE state_index;
-    double sum = 0.;
+    ITYPE state_index = 0;
+    if (target_qubit_index_0 == 0 || target_qubit_index_1 == 0) {
 #ifdef _OPENMP
-    OMPutil::get_inst().set_qulacs_num_threads(dim, 10);
-#pragma omp parallel for reduction(+ : sum)
+#pragma omp parallel for
 #endif
-    for (state_index = 0; state_index < loop_dim; ++state_index) {
-        ITYPE basis_0 = insert_zero_to_basis_index(
-            state_index, pivot_mask, pivot_qubit_index);
-        ITYPE basis_1 = basis_0 ^ bit_flip_mask;
-        UINT sign_0 = count_population(basis_0 & phase_flip_mask) % 2;
-
-        sum += _creal(state[basis_0] * conj(state[basis_1]) *
-                      PHASE_90ROT[(global_phase_90rot_count + sign_0 * 2) % 4] *
-                      2.0);
-    }
+        for (state_index = 0; state_index < loop_dim; ++state_index) {
+            ITYPE basis_index_0 = (state_index & low_mask) +
+                                  ((state_index & mid_mask) << 1) +
+                                  ((state_index & high_mask) << 2) + mask_0;
+            ITYPE basis_index_1 = basis_index_0 ^ mask;
+            CTYPE temp = state[basis_index_0];
+            state[basis_index_0] = state[basis_index_1];
+            state[basis_index_1] = temp;
+        }
+    } else {
+        // a,a+1 is swapped to a^m, a^m+1, respectively
 #ifdef _OPENMP
-    OMPutil::get_inst().reset_qulacs_num_threads();
+#pragma omp parallel for
 #endif
-    return sum;
+        for (state_index = 0; state_index < loop_dim; state_index += 2) {
+            ITYPE basis_index_0 = (state_index & low_mask) +
+                                  ((state_index & mid_mask) << 1) +
+                                  ((state_index & high_mask) << 2) + mask_0;
+            ITYPE basis_index_1 = basis_index_0 ^ mask;
+            CTYPE temp0 = state[basis_index_0];
+            CTYPE temp1 = state[basis_index_0 + 1];
+            state[basis_index_0] = state[basis_index_1];
+            state[basis_index_0 + 1] = state[basis_index_1 + 1];
+            state[basis_index_1] = temp0;
+            state[basis_index_1 + 1] = temp1;
+        }
+    }
 }
 
-double expectation_value_multi_qubit_Pauli_operator_Z_mask(
-    ITYPE phase_flip_mask, const CTYPE* state, ITYPE dim) {
-    const ITYPE loop_dim = dim;
-    ITYPE state_index;
-    double sum = 0.;
+#ifdef _USE_SIMD
+void SWAP_gate_parallel_simd(UINT target_qubit_index_0,
+    UINT target_qubit_index_1, CTYPE* state, ITYPE dim) {
+    const ITYPE loop_dim = dim / 4;
+
+    const ITYPE mask_0 = 1ULL << target_qubit_index_0;
+    const ITYPE mask_1 = 1ULL << target_qubit_index_1;
+    const ITYPE mask = mask_0 + mask_1;
+
+    const UINT min_qubit_index =
+        get_min_ui(target_qubit_index_0, target_qubit_index_1);
+    const UINT max_qubit_index =
+        get_max_ui(target_qubit_index_0, target_qubit_index_1);
+    const ITYPE min_qubit_mask = 1ULL << min_qubit_index;
+    const ITYPE max_qubit_mask = 1ULL << (max_qubit_index - 1);
+    const ITYPE low_mask = min_qubit_mask - 1;
+    const ITYPE mid_mask = (max_qubit_mask - 1) ^ low_mask;
+    const ITYPE high_mask = ~(max_qubit_mask - 1);
+
+    ITYPE state_index = 0;
+    if (target_qubit_index_0 == 0 || target_qubit_index_1 == 0) {
 #ifdef _OPENMP
-    OMPutil::get_inst().set_qulacs_num_threads(dim, 10);
-#pragma omp parallel for reduction(+ : sum)
+#pragma omp parallel for
 #endif
-    for (state_index = 0; state_index < loop_dim; ++state_index) {
-        int bit_parity = count_population(state_index & phase_flip_mask) % 2;
-        int sign = 1 - 2 * bit_parity;
-        sum += pow(_cabs(state[state_index]), 2) * sign;
-    }
+        for (state_index = 0; state_index < loop_dim; ++state_index) {
+            ITYPE basis_index_0 = (state_index & low_mask) +
+                                  ((state_index & mid_mask) << 1) +
+                                  ((state_index & high_mask) << 2) + mask_0;
+            ITYPE basis_index_1 = basis_index_0 ^ mask;
+            CTYPE temp = state[basis_index_0];
+            state[basis_index_0] = state[basis_index_1];
+            state[basis_index_1] = temp;
+        }
+    } else {
+        // a,a+1 is swapped to a^m, a^m+1, respectively
 #ifdef _OPENMP
-    OMPutil::get_inst().reset_qulacs_num_threads();
+#pragma omp parallel for
 #endif
-    return sum;
-}
-
-double expectation_value_multi_qubit_Pauli_operator_partial_list(
-    const UINT* target_qubit_index_list, const UINT* Pauli_operator_type_list,
-    UINT target_qubit_index_count, const CTYPE* state, ITYPE dim) {
-    ITYPE bit_flip_mask = 0;
-    ITYPE phase_flip_mask = 0;
-    UINT global_phase_90rot_count = 0;
-    UINT pivot_qubit_index = 0;
-    get_Pauli_masks_partial_list(target_qubit_index_list,
-        Pauli_operator_type_list, target_qubit_index_count, &bit_flip_mask,
-        &phase_flip_mask, &global_phase_90rot_count, &pivot_qubit_index);
-    double result;
-    if (bit_flip_mask == 0) {
-        result = expectation_value_multi_qubit_Pauli_operator_Z_mask(
-            phase_flip_mask, state, dim);
-    } else {
-        result = expectation_value_multi_qubit_Pauli_operator_XZ_mask(
-            bit_flip_mask, phase_flip_mask, global_phase_90rot_count,
-            pivot_qubit_index, state, dim);
-    }
-    return result;
-}
-
-double expectation_value_multi_qubit_Pauli_operator_whole_list(
-    const UINT* Pauli_operator_type_list, UINT qubit_count, const CTYPE* state,
-    ITYPE dim) {
-    ITYPE bit_flip_mask = 0;
-    ITYPE phase_flip_mask = 0;
-    UINT global_phase_90rot_count = 0;
-    UINT pivot_qubit_index = 0;
-    get_Pauli_masks_whole_list(Pauli_operator_type_list, qubit_count,
-        &bit_flip_mask, &phase_flip_mask, &global_phase_90rot_count,
-        &pivot_qubit_index);
-    double result;
-    if (bit_flip_mask == 0) {
-        result = expectation_value_multi_qubit_Pauli_operator_Z_mask(
-            phase_flip_mask, state, dim);
-    } else {
-        result = expectation_value_multi_qubit_Pauli_operator_XZ_mask(
-            bit_flip_mask, phase_flip_mask, global_phase_90rot_count,
-            pivot_qubit_index, state, dim);
+        for (state_index = 0; state_index < loop_dim; state_index += 2) {
+            ITYPE basis_index_0 = (state_index & low_mask) +
+                                  ((state_index & mid_mask) << 1) +
+                                  ((state_index & high_mask) << 2) + mask_0;
+            ITYPE basis_index_1 = basis_index_0 ^ mask;
+            double* ptr0 = (double*)(state + basis_index_0);
+            double* ptr1 = (double*)(state + basis_index_1);
+            __m256d data0 = _mm256_loadu_pd(ptr0);
+            __m256d data1 = _mm256_loadu_pd(ptr1);
+            _mm256_storeu_pd(ptr1, data0);
+            _mm256_storeu_pd(ptr0, data1);
+        }
     }
-    return result;
 }
+#endif
 
-/****
- * Single thread version of expectation value
- **/
-// calculate expectation value of multi-qubit Pauli operator on qubits.
-// bit-flip mask : the n-bit binary string of which the i-th element is 1 iff
-// the i-th pauli operator is X or Y phase-flip mask : the n-bit binary string
-// of which the i-th element is 1 iff the i-th pauli operator is Y or Z We
-// assume bit-flip mask is nonzero, namely, there is at least one X or Y
-// operator. the pivot qubit is any qubit index which has X or Y To generate
-// bit-flip mask and phase-flip mask, see get_masks_*_list at utility.h
-double expectation_value_multi_qubit_Pauli_operator_XZ_mask_single_thread(
-    ITYPE bit_flip_mask, ITYPE phase_flip_mask, UINT global_phase_90rot_count,
-    UINT pivot_qubit_index, const CTYPE* state, ITYPE dim) {
-    const ITYPE loop_dim = dim / 2;
-    const ITYPE pivot_mask = 1ULL << pivot_qubit_index;
-    ITYPE state_index;
-    double sum = 0.;
-    UINT sign_0;
-    ITYPE basis_0, basis_1;
-    for (state_index = 0; state_index < loop_dim; ++state_index) {
-        basis_0 = insert_zero_to_basis_index(
-            state_index, pivot_mask, pivot_qubit_index);
-        basis_1 = basis_0 ^ bit_flip_mask;
-        sign_0 = count_population(basis_0 & phase_flip_mask) % 2;
-        sum += _creal(state[basis_0] * conj(state[basis_1]) *
-                      PHASE_90ROT[(global_phase_90rot_count + sign_0 * 2) % 4] *
-                      2.0);
-    }
-    return sum;
+#ifdef _USE_SVE
+void SWAP_gate_parallel_sve(UINT target_qubit_index_0,
+    UINT target_qubit_index_1, CTYPE* state, ITYPE dim) {
+    const ITYPE loop_dim = dim / 4;
+
+    const ITYPE mask_0 = 1ULL << target_qubit_index_0;
+    const ITYPE mask_1 = 1ULL << target_qubit_index_1;
+    const ITYPE mask = mask_0 + mask_1;
+
+    const UINT min_qubit_index =
+        get_min_ui(target_qubit_index_0, target_qubit_index_1);
+    const UINT max_qubit_index =
+        get_max_ui(target_qubit_index_0, target_qubit_index_1);
+    const ITYPE min_qubit_mask = 1ULL << min_qubit_index;
+    const ITYPE max_qubit_mask = 1ULL << (max_qubit_index - 1);
+    const ITYPE low_mask = min_qubit_mask - 1;
+    const ITYPE mid_mask = (max_qubit_mask - 1) ^ low_mask;
+    const ITYPE high_mask = ~(max_qubit_mask - 1);
+
+    ITYPE state_index = 0;
+
+    // # of complex128 numbers in an SVE register
+    ITYPE VL = svcntd() / 2;
+
+    if ((dim > VL) && (min_qubit_mask >= VL)) {
+#pragma omp parallel for
+        for (state_index = 0; state_index < loop_dim; state_index += VL) {
+            // Calculate indices
+            ITYPE basis_0 = (state_index & low_mask) +
+                            ((state_index & mid_mask) << 1) +
+                            ((state_index & high_mask) << 2) + mask_0;
+            ITYPE basis_1 = basis_0 ^ mask;
+
+            // Load values
+            svfloat64_t input0 = svld1(svptrue_b64(), (double*)&state[basis_0]);
+            svfloat64_t input1 = svld1(svptrue_b64(), (double*)&state[basis_1]);
+
+            // Store values
+            svst1(svptrue_b64(), (double*)&state[basis_0], input1);
+            svst1(svptrue_b64(), (double*)&state[basis_1], input0);
+        }
+    } else {  // if ((dim > VL) && (min_qubit_mask >= VL))
+#pragma omp parallel for
+        for (state_index = 0; state_index < loop_dim; ++state_index) {
+            ITYPE basis_index_0 = (state_index & low_mask) +
+                                  ((state_index & mid_mask) << 1) +
+                                  ((state_index & high_mask) << 2) + mask_0;
+            ITYPE basis_index_1 = basis_index_0 ^ mask;
+            CTYPE temp = state[basis_index_0];
+            state[basis_index_0] = state[basis_index_1];
+            state[basis_index_1] = temp;
+        }
+    }  // if ((dim > VL) && (min_qubit_mask >= VL))
 }
+#endif
 
-double expectation_value_multi_qubit_Pauli_operator_Z_mask_single_thread(
-    ITYPE phase_flip_mask, const CTYPE* state, ITYPE dim) {
-    const ITYPE loop_dim = dim;
-    ITYPE state_index;
-    double sum = 0.;
-    int bit_parity, sign;
-    for (state_index = 0; state_index < loop_dim; ++state_index) {
-        bit_parity = count_population(state_index & phase_flip_mask) % 2;
-        sign = 1 - 2 * bit_parity;
-        sum += pow(_cabs(state[state_index]), 2) * sign;
+#ifdef _USE_MPI
+void SWAP_gate_mpi(UINT target_qubit_index_0, UINT target_qubit_index_1,
+    CTYPE* state, ITYPE dim, UINT inner_qc) {
+    UINT left_qubit, right_qubit;
+    if (target_qubit_index_0 > target_qubit_index_1) {
+        left_qubit = target_qubit_index_0;
+        right_qubit = target_qubit_index_1;
+    } else {
+        left_qubit = target_qubit_index_1;
+        right_qubit = target_qubit_index_0;
     }
-    return sum;
-}
 
-double expectation_value_multi_qubit_Pauli_operator_partial_list_single_thread(
-    const UINT* target_qubit_index_list, const UINT* Pauli_operator_type_list,
-    UINT target_qubit_index_count, const CTYPE* state, ITYPE dim) {
-    ITYPE bit_flip_mask = 0;
-    ITYPE phase_flip_mask = 0;
-    UINT global_phase_90rot_count = 0;
-    UINT pivot_qubit_index = 0;
-    get_Pauli_masks_partial_list(target_qubit_index_list,
-        Pauli_operator_type_list, target_qubit_index_count, &bit_flip_mask,
-        &phase_flip_mask, &global_phase_90rot_count, &pivot_qubit_index);
-    double result;
-    if (bit_flip_mask == 0) {
-        result =
-            expectation_value_multi_qubit_Pauli_operator_Z_mask_single_thread(
-                phase_flip_mask, state, dim);
-    } else {
-        result =
-            expectation_value_multi_qubit_Pauli_operator_XZ_mask_single_thread(
-                bit_flip_mask, phase_flip_mask, global_phase_90rot_count,
-                pivot_qubit_index, state, dim);
+    if (left_qubit < inner_qc) {  // both qubits are inner
+        SWAP_gate(target_qubit_index_0, target_qubit_index_1, state, dim);
+    } else if (right_qubit < inner_qc) {  // one target is outer
+        MPIutil& m = MPIutil::get_inst();
+        const UINT rank = m.get_rank();
+        ITYPE dim_work = dim;
+        ITYPE num_work = 0;
+        CTYPE* t = m.get_workarea(&dim_work, &num_work);
+        const ITYPE tgt_rank_bit = 1 << (left_qubit - inner_qc);
+        const ITYPE rtgt_blk_dim = 1 << right_qubit;
+        const int pair_rank = rank ^ tgt_rank_bit;
+
+        ITYPE rtgt_offset = 0;
+        if ((rank & tgt_rank_bit) == 0) rtgt_offset = rtgt_blk_dim;
+
+        if (rtgt_blk_dim < dim_work) {
+            dim_work >>= 1;  // upper for send, lower for recv
+            CTYPE* t_send = t;
+            CTYPE* t_recv = t + dim_work;
+            const ITYPE num_rtgt_block = (dim / dim_work) >> 1;
+            const ITYPE num_elem_block = dim_work >> right_qubit;
+
+            CTYPE* si0 = state + rtgt_offset;
+            for (ITYPE i = 0; i < num_rtgt_block; ++i) {
+                // gather
+                CTYPE* si = si0;
+                CTYPE* ti = t_send;
+                for (ITYPE k = 0; k < num_elem_block; ++k) {
+                    memcpy(ti, si, rtgt_blk_dim * sizeof(CTYPE));
+                    si += (rtgt_blk_dim << 1);
+                    ti += rtgt_blk_dim;
+                }
+
+                // sendrecv
+                m.m_DC_sendrecv(t_send, t_recv, dim_work, pair_rank);
+
+                // scatter
+                si = t_recv;
+                ti = si0;
+                for (ITYPE k = 0; k < num_elem_block; ++k) {
+                    memcpy(ti, si, rtgt_blk_dim * sizeof(CTYPE));
+                    si += rtgt_blk_dim;
+                    ti += (rtgt_blk_dim << 1);
+                }
+                si0 += (dim_work << 1);
+            }
+
+        } else {  // rtgt_blk_dim >= dim_work
+            const ITYPE num_rtgt_block = dim >> (right_qubit + 1);
+            const ITYPE num_work_block = rtgt_blk_dim / dim_work;
+
+            CTYPE* si = state + rtgt_offset;
+            for (ITYPE i = 0; i < num_rtgt_block; ++i) {
+                for (ITYPE j = 0; j < num_work_block; ++j) {
+                    m.m_DC_sendrecv(si, t, dim_work, pair_rank);
+                    memcpy(si, t, dim_work * sizeof(CTYPE));
+                    si += dim_work;
+                }
+                si += rtgt_blk_dim;
+            }
+        }
+    } else {  // both targets are outer
+        MPIutil& m = MPIutil::get_inst();
+        const UINT rank = m.get_rank();
+        ITYPE dim_work = dim;
+        ITYPE num_work = 0;
+        CTYPE* t = m.get_workarea(&dim_work, &num_work);
+        const UINT tgt0_rank_bit = 1 << (left_qubit - inner_qc);
+        const UINT tgt1_rank_bit = 1 << (right_qubit - inner_qc);
+        const UINT tgt_rank_bit = tgt0_rank_bit + tgt1_rank_bit;
+
+        const int pair_rank = rank ^ tgt_rank_bit;
+        const int not_zerozero = ((rank & tgt_rank_bit) != 0);
+        const int with_zero =
+            (((rank & tgt0_rank_bit) * (rank & tgt1_rank_bit)) == 0);
+
+        CTYPE* si = state;
+        for (ITYPE i = 0; i < num_work; ++i) {
+            if (not_zerozero && with_zero) {  // 01 or 10
+                m.m_DC_sendrecv(si, t, dim_work, pair_rank);
+                memcpy(si, t, dim_work * sizeof(CTYPE));
+                si += dim_work;
+            } else {
+                m.get_tag();  // dummy to count up tag
+            }
+        }
     }
-    return result;
 }
+#endif
```

### Comparing `qulacs-0.5.6/src/csim/stat_ops_probability.cpp` & `qulacs-0.6.0/src/csim/stat_ops_probability.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/stat_ops_transition_amplitude.cpp` & `qulacs-0.6.0/src/csim/stat_ops_transition_amplitude.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/type.hpp` & `qulacs-0.6.0/src/csim/type.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -42,7 +42,13 @@
 
 //! define export command
 #if defined(__MINGW32__) || defined(_MSC_VER)
 #define DllExport __declspec(dllexport)
 #else
 #define DllExport __attribute__((visibility("default")))
 #endif
+
+//! ACLE
+#ifdef _USE_SVE
+#include "arm_acle.h"
+#include "arm_sve.h"
+#endif  // #ifdef _USE_SVE
```

### Comparing `qulacs-0.5.6/src/csim/update_ops.hpp` & `qulacs-0.6.0/src/csim/update_ops.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -38,14 +38,17 @@
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void X_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim);
 void X_gate_parallel_unroll(UINT target_qubit_index, CTYPE* state, ITYPE dim);
 void X_gate_parallel_simd(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+void X_gate_parallel_sve(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void X_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply the Pauli Y gate to the quantum state.
  *
  * Apply the Pauli Y gate to the quantum state.
  * @param[in] target_qubit_index index of the qubit
@@ -59,18 +62,19 @@
  * パウリY演算を作用させて状態を更新。
  * @param[in] target_qubit_index 作用する量子ビットのインデックス。
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void Y_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim);
-void Y_gate_single_unroll(UINT target_qubit_index, CTYPE* state, ITYPE dim);
-void Y_gate_single_simd(UINT target_qubit_index, CTYPE* state, ITYPE dim);
 void Y_gate_parallel_unroll(UINT target_qubit_index, CTYPE* state, ITYPE dim);
 void Y_gate_parallel_simd(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+void Y_gate_parallel_sve(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void Y_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply the Pauli Z gate to the quantum state.
  *
  * Apply the Pauli Z gate to the quantum state.
  * @param[in] target_qubit_index index of the qubit
@@ -84,18 +88,19 @@
  * パウリZ演算を作用させて状態を更新。
  * @param[in] target_qubit_index 作用する量子ビットのインデックス。
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void Z_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim);
-void Z_gate_single_unroll(UINT target_qubit_index, CTYPE* state, ITYPE dim);
-void Z_gate_single_simd(UINT target_qubit_index, CTYPE* state, ITYPE dim);
 void Z_gate_parallel_unroll(UINT target_qubit_index, CTYPE* state, ITYPE dim);
 void Z_gate_parallel_simd(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+void Z_gate_parallel_sve(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void Z_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply S gate to the quantum state.
  *
  * Apply S gate to the quantum state.
  * @param[in] target_qubit_index index of the qubit
@@ -109,14 +114,16 @@
  * 位相演算 S = diag(1,i) を作用させて状態を更新。
  * @param[in] target_qubit_index 作用する量子ビットのインデックス。
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void S_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void S_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT outer_qb);
 
 /**
  * \~english
  * Apply S gate to the quantum state.
  *
  * Apply S gate to the quantum state.
  * @param[in] target_qubit_index index of the qubit
@@ -130,14 +137,16 @@
  * 位相演算 S^dag = diag(1,-i) を作用させて状態を更新。
  * @param[in] target_qubit_index 作用する量子ビットのインデックス。
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void Sdag_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void Sdag_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT outer_qb);
 
 /**
  * \~english
  * Apply T gate to the quantum state.
  *
  * Apply T gate to the quantum state.
  * @param[in] target_qubit_index index of the qubit
@@ -152,14 +161,16 @@
  * を作用させて状態を更新。非クリフォード演算。
  * @param[in] target_qubit_index 作用する量子ビットのインデックス。
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void T_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void T_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT outer_qb);
 
 /**
  * \~english
  * Apply T^dag gate to the quantum state.
  *
  * Apply T^dag gate to the quantum state.
  * @param[in] target_qubit_index index of the qubit
@@ -174,14 +185,16 @@
  * を作用させて状態を更新。非クリフォード演算。
  * @param[in] target_qubit_index 作用する量子ビットのインデックス。
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void Tdag_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void Tdag_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT outer_qb);
 
 /**
  * \~english
  * Apply the square root of the X gate to the quantum state.
  *
  * Apply the square root of the X gate to the quantum state.
  * @param[in] target_qubit_index index of the qubit
@@ -195,14 +208,16 @@
  * パウリ X 演算子の平方根の演算子を作用させて状態を更新。非クリフォード演算。
  * @param[in] target_qubit_index 作用する量子ビットのインデックス。
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void sqrtX_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void sqrtX_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply hermitian conjugate of the square root of the X gate to the quantum
  * state.
  *
  * Apply hermitian conjugate of the square root of the X gate to the quantum
@@ -219,14 +234,16 @@
  * 演算子の平方根に対してエルミート共役な演算子を作用させて状態を更新。非クリフォード演算。
  * @param[in] target_qubit_index 作用する量子ビットのインデックス。
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void sqrtXdag_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void sqrtXdag_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply the square root of the Y gate to the quantum state.
  *
  * Apply the square root of the Y gate to the quantum state.
  * @param[in] target_qubit_index index of the qubit
@@ -240,14 +257,16 @@
  * パウリ Y 演算子の平方根の演算子を作用させて状態を更新。非クリフォード演算。
  * @param[in] target_qubit_index 作用する量子ビットのインデックス。
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void sqrtY_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void sqrtY_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply hermitian conjugate of the square root of the Y gate to the quantum
  * state.
  *
  * Apply hermitian conjugate of the square root of the Y gate to the quantum
@@ -264,14 +283,16 @@
  * 演算子の平方根に対してエルミート共役な演算子を作用させて状態を更新。非クリフォード演算。
  * @param[in] target_qubit_index 作用する量子ビットのインデックス。
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void sqrtYdag_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void sqrtYdag_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply the Hadamard gate to the quantum state.
  *
  * Apply the Hadamard gate to the quantum state.
  * @param[in] target_qubit_index index of the qubit
@@ -285,18 +306,20 @@
  * アダマール演算子を作用させて状態を更新。
  * @param[in] target_qubit_index 作用する量子ビットのインデックス。
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void H_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim);
-void H_gate_single_unroll(UINT target_qubit_index, CTYPE* state, ITYPE dim);
-void H_gate_single_simd(UINT target_qubit_index, CTYPE* state, ITYPE dim);
 void H_gate_parallel_unroll(UINT target_qubit_index, CTYPE* state, ITYPE dim);
 void H_gate_parallel_simd(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+void H_gate_parallel_sve(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void H_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc);
+void _H_gate_mpi(CTYPE* t, CTYPE* si, ITYPE dim, int flag);
 
 /** Hadamard gate multiplied sqrt(2) **/
 // DllExport void H_gate_unnormalized(UINT target_qubit_index, CTYPE *state,
 // ITYPE dim);
 
 /**
  * \~english
@@ -319,14 +342,18 @@
  */
 DllExport void CNOT_gate(
     UINT control_qubit_index, UINT target_qubit_index, CTYPE* state, ITYPE dim);
 void CNOT_gate_parallel_unroll(
     UINT control_qubit_index, UINT target_qubit_index, CTYPE* state, ITYPE dim);
 void CNOT_gate_parallel_simd(
     UINT control_qubit_index, UINT target_qubit_index, CTYPE* state, ITYPE dim);
+void CNOT_gate_parallel_sve(
+    UINT control_qubit_index, UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void CNOT_gate_mpi(UINT control_qubit_index, UINT target_qubit_index,
+    CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply the CZ gate to the quantum state.
  *
  * Apply the CZ gate to the quantum state.
  * @param[in] control_qubit_index index of control qubit
@@ -341,22 +368,22 @@
  * @param[in] control_qubit_index 制御量子ビットのインデックス
  * @param[in] target_qubit_index ターゲット量子ビットのインデックス
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  */
 DllExport void CZ_gate(
     UINT control_qubit_index, UINT target_qubit_index, CTYPE* state, ITYPE dim);
-void CZ_gate_single_unroll(
-    UINT control_qubit_index, UINT target_qubit_index, CTYPE* state, ITYPE dim);
 void CZ_gate_parallel_unroll(
     UINT control_qubit_index, UINT target_qubit_index, CTYPE* state, ITYPE dim);
-void CZ_gate_single_simd(
-    UINT control_qubit_index, UINT target_qubit_index, CTYPE* state, ITYPE dim);
 void CZ_gate_parallel_simd(
     UINT control_qubit_index, UINT target_qubit_index, CTYPE* state, ITYPE dim);
+void CZ_gate_parallel_sve(
+    UINT control_qubit_index, UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void CZ_gate_mpi(UINT control_qubit_index, UINT target_qubit_index,
+    CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply the SWAP to the quantum state.
  *
  * Apply the SWAP to the quantum state.
  * @param[in] control_qubit_index index of control qubit
@@ -371,22 +398,51 @@
  * @param[in] target_qubit_index_0 作用する量子ビットのインデックス
  * @param[in] target_qubit_index_1 作用する量子ビットのインデックス
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  */
 DllExport void SWAP_gate(UINT target_qubit_index_0, UINT target_qubit_index_1,
     CTYPE* state, ITYPE dim);
-void SWAP_gate_single_unroll(UINT target_qubit_index_0,
-    UINT target_qubit_index_1, CTYPE* state, ITYPE dim);
-void SWAP_gate_single_simd(UINT target_qubit_index_0, UINT target_qubit_index_1,
-    CTYPE* state, ITYPE dim);
 void SWAP_gate_parallel_unroll(UINT target_qubit_index_0,
     UINT target_qubit_index_1, CTYPE* state, ITYPE dim);
 void SWAP_gate_parallel_simd(UINT target_qubit_index_0,
     UINT target_qubit_index_1, CTYPE* state, ITYPE dim);
+void SWAP_gate_parallel_sve(UINT target_qubit_index_0,
+    UINT target_qubit_index_1, CTYPE* state, ITYPE dim);
+DllExport void SWAP_gate_mpi(UINT target_qubit_index_0,
+    UINT target_qubit_index_1, CTYPE* state, ITYPE dim, UINT inner_qc);
+
+/**
+ * \~english
+ * Apply the FusedSWAP to the quantum state.
+ *
+ * Apply the FusedSWAP to the quantum state.
+ * @param[in] control_qubit_index index of start target-0 qubit
+ * @param[in] target_qubit_index index of start target-1 qubit
+ * @param[in] number_qubits number of target qubits
+ * @param[in,out] state quantum state
+ * @param[in] dim dimension
+ *
+ * \~japanese-en
+ * FusedSWAP演算を作用させて状態を更新。
+ *
+ * (2n)量子ビット演算、FusedSWAP演算を作用させて状態を更新。block_size個の２つの量子ビットに対して対称に作用する（インデックスを入れ替えても同じ作用）。
+ * @param[in] target_qubit_index_0 作用する量子ビットの最初のインデックス
+ * @param[in] target_qubit_index_1 作用する量子ビットの最初のインデックス
+ * @param[in] block_size 作用する量子ビット数
+ * @param[in,out] state 量子状態
+ * @param[in] dim 次元
+ */
+DllExport void FusedSWAP_gate(UINT target_qubit_index_0,
+    UINT target_qubit_index_1, UINT block_size, CTYPE* state, ITYPE dim);
+void FusedSWAP_gate_global(UINT target_qubit_index_0, UINT target_qubit_index_1,
+    UINT block_size, CTYPE* state, ITYPE dim);
+DllExport void FusedSWAP_gate_mpi(UINT target_qubit_index_0,
+    UINT target_qubit_index_1, UINT block_size, CTYPE* state, ITYPE dim,
+    UINT inner_qc);
 
 /**
  * \~english
  * Project the quantum state to the 0 state.
  *
  * Project the quantum state to the 0 state. The output state is not normalized.
  * @param[in] target_qubit_index index of the qubit
@@ -400,16 +456,17 @@
  * を作用させて状態を更新する。ノルムは規格化されない。
  * @param[in] target_qubit_index 作用する量子ビットのインデックス
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void P0_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim);
-void P0_gate_single(UINT target_qubit_index, CTYPE* state, ITYPE dim);
 void P0_gate_parallel(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void P0_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Project the quantum state to the 1 state.
  *
  * Project the quantum state to the 1 state. The output state is not normalized.
  * @param[in] target_qubit_index index of the qubit
@@ -423,16 +480,17 @@
  * を作用させて状態を更新する。ノルムは規格化されない。
  * @param[in] target_qubit_index 作用する量子ビットのインデックス
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void P1_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim);
-void P1_gate_single(UINT target_qubit_index, CTYPE* state, ITYPE dim);
 void P1_gate_parallel(UINT target_qubit_index, CTYPE* state, ITYPE dim);
+DllExport void P1_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Normalize the quantum state.
  *
  * Normalize the quantum state by multiplying the normalization factor
  * 1/sqrt(norm).
@@ -496,14 +554,16 @@
  * @param[in] angle 回転角
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void RX_gate(
     UINT target_qubit_index, double angle, CTYPE* state, ITYPE dim);
+DllExport void RX_gate_mpi(UINT target_qubit_index, double angle, CTYPE* state,
+    ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply a Y rotation gate by angle to the quantum state.
  *
  * Apply a Y rotation gate by angle to the quantum state.
  * @param[in] target_qubit_index index of the qubit
@@ -524,14 +584,16 @@
  * @param[in] angle 回転角
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void RY_gate(
     UINT target_qubit_index, double angle, CTYPE* state, ITYPE dim);
+DllExport void RY_gate_mpi(UINT target_qubit_index, double angle, CTYPE* state,
+    ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply a Z rotation gate by angle to the quantum state.
  *
  * Apply a Z rotation gate by angle to the quantum state.
  * @param[in] target_qubit_index index of the qubit
@@ -552,14 +614,16 @@
  * @param[in] angle 回転角
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void RZ_gate(
     UINT target_qubit_index, double angle, CTYPE* state, ITYPE dim);
+DllExport void RZ_gate_mpi(UINT target_qubit_index, double angle, CTYPE* state,
+    ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply a single-qubit Pauli operator to the quantum state.
  *
  * Apply a single-qubit Pauli operator to the quantum state. Pauli_operator_type
  * must be 0,1,2,3 corresponding to the Pauli I, X, Y, Z operators respectively.
@@ -582,14 +646,15 @@
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  *
  */
 DllExport void single_qubit_Pauli_gate(
     UINT target_qubit_index, UINT Pauli_operator_type, CTYPE* state, ITYPE dim);
+// Not implemented for multi-cpu
 
 /**
  * \~english
  * Apply a single-qubit Pauli rotation operator to the quantum state.
  *
  * Apply a single-qubit Pauli rotation operator to the quantum state.
  * Pauli_operator_type must be 0,1,2,3 corresponding to the Pauli I, X, Y, Z
@@ -619,14 +684,15 @@
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  *
  */
 DllExport void single_qubit_Pauli_rotation_gate(UINT target_qubit_index,
     UINT Pauli_operator_index, double angle, CTYPE* state, ITYPE dim);
+// Not implemented for multi-cpu
 
 /**
  * \~english
  * Apply a single-qubit dense operator to the quantum state.
  *
  * Apply a single-qubit dense operator to the quantum state.
  *
@@ -655,14 +721,18 @@
     UINT target_qubit_index, const CTYPE matrix[4], CTYPE* state, ITYPE dim);
 void single_qubit_dense_matrix_gate_parallel_unroll(
     UINT target_qubit_index, const CTYPE matrix[4], CTYPE* state, ITYPE dim);
 void single_qubit_dense_matrix_gate_parallel(
     UINT target_qubit_index, const CTYPE matrix[4], CTYPE* state, ITYPE dim);
 void single_qubit_dense_matrix_gate_parallel_simd(
     UINT target_qubit_index, const CTYPE matrix[4], CTYPE* state, ITYPE dim);
+void single_qubit_dense_matrix_gate_parallel_sve(
+    UINT target_qubit_index, const CTYPE matrix[4], CTYPE* state, ITYPE dim);
+DllExport void single_qubit_dense_matrix_gate_mpi(UINT target_qubit_index,
+    const CTYPE matrix[4], CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply a single-qubit diagonal operator to the quantum state.
  *
  * Apply a single-qubit diagonal operator to the quantum state.
  *
@@ -687,14 +757,18 @@
  */
 DllExport void single_qubit_diagonal_matrix_gate(UINT target_qubit_index,
     const CTYPE diagonal_matrix[2], CTYPE* state, ITYPE dim);
 void single_qubit_diagonal_matrix_gate_parallel_unroll(UINT target_qubit_index,
     const CTYPE diagonal_matrix[2], CTYPE* state, ITYPE dim);
 void single_qubit_diagonal_matrix_gate_parallel_simd(UINT target_qubit_index,
     const CTYPE diagonal_matrix[2], CTYPE* state, ITYPE dim);
+void single_qubit_diagonal_matrix_gate_parallel_sve(UINT target_qubit_index,
+    const CTYPE diagonal_matrix[2], CTYPE* state, ITYPE dim);
+DllExport void single_qubit_diagonal_matrix_gate_mpi(UINT target_qubit_index,
+    const CTYPE diagonal_matrix[2], CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply a single-qubit phase operator to the quantum state.
  *
  * Apply a single-qubit phase operator, diag(1,phsae), to the quantum state.
  *
@@ -718,14 +792,16 @@
  */
 DllExport void single_qubit_phase_gate(
     UINT target_qubit_index, CTYPE phase, CTYPE* state, ITYPE dim);
 void single_qubit_phase_gate_parallel_unroll(
     UINT target_qubit_index, CTYPE phase, CTYPE* state, ITYPE dim);
 void single_qubit_phase_gate_parallel_simd(
     UINT target_qubit_index, CTYPE phase, CTYPE* state, ITYPE dim);
+DllExport void single_qubit_phase_gate_mpi(UINT target_qubit_index, CTYPE phase,
+    CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply a single-qubit controlled single-qubit gate.
  *
  * Apply a single-qubit controlled single-qubit gate.
  *
@@ -758,14 +834,20 @@
     const CTYPE matrix[4], CTYPE* state, ITYPE dim);
 void single_qubit_control_single_qubit_dense_matrix_gate_unroll(
     UINT control_qubit_index, UINT control_value, UINT target_qubit_index,
     const CTYPE matrix[4], CTYPE* state, ITYPE dim);
 void single_qubit_control_single_qubit_dense_matrix_gate_simd(
     UINT control_qubit_index, UINT control_value, UINT target_qubit_index,
     const CTYPE matrix[4], CTYPE* state, ITYPE dim);
+void single_qubit_control_single_qubit_dense_matrix_gate_sve512(
+    UINT control_qubit_index, UINT control_value, UINT target_qubit_index,
+    const CTYPE matrix[4], CTYPE* state, ITYPE dim);
+DllExport void single_qubit_control_single_qubit_dense_matrix_gate_mpi(
+    UINT control_qubit_index, UINT control_value, UINT target_qubit_index,
+    const CTYPE matrix[4], CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply a multi-qubit controlled single-qubit gate.
  *
  * Apply a multi-qubit controlled single-qubit gate.
  *
@@ -803,14 +885,18 @@
     const UINT* control_qubit_index_list, const UINT* control_value_list,
     UINT control_qubit_index_count, UINT target_qubit_index,
     const CTYPE matrix[4], CTYPE* state, ITYPE dim);
 void multi_qubit_control_single_qubit_dense_matrix_gate_simd(
     const UINT* control_qubit_index_list, const UINT* control_value_list,
     UINT control_qubit_index_count, UINT target_qubit_index,
     const CTYPE matrix[4], CTYPE* state, ITYPE dim);
+DllExport void multi_qubit_control_single_qubit_dense_matrix_gate_mpi(
+    const UINT* control_qubit_index_list, const UINT* control_value_list,
+    UINT control_qubit_index_count, UINT target_qubit_index,
+    const CTYPE matrix[4], CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply multi-qubit Pauli operator to the quantum state with a whole list.
  *
  * Apply multi-qubit Pauli operator to the quantum state with a whole list of
  * the Pauli operators. Pauli_operator_type_list must be a list of n single
@@ -837,14 +923,15 @@
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void multi_qubit_Pauli_gate_whole_list(
     const UINT* Pauli_operator_type_list, UINT qubit_count, CTYPE* state,
     ITYPE dim_);
+// Not implemented for multi-cpu
 
 /**
  * \~english
  * Apply multi-qubit Pauli operator to the quantum state with a whole list.
  *
  * Apply multi-qubit Pauli operator to the quantum state with a whole list of
  * the Pauli operators. Pauli_operator_type_list must be a list of n single
@@ -871,14 +958,15 @@
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void multi_qubit_Pauli_gate_whole_list_single_thread(
     const UINT* Pauli_operator_type_list, UINT qubit_count, CTYPE* state,
     ITYPE dim_);
+// Not implemented for multi-cpu
 
 /**
  * \~english
  * Apply multi-qubit Pauli operator to the quantum state with a partial list.
  *
  * Apply multi-qubit Pauli operator to the quantum state with a partial list of
  * the Pauli operators. Pauli_operator_type_list must be a list of n single
@@ -911,14 +999,17 @@
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void multi_qubit_Pauli_gate_partial_list(
     const UINT* target_qubit_index_list, const UINT* Pauli_operator_type_list,
     UINT target_qubit_index_count, CTYPE* state, ITYPE dim);
+// This function is used in apply_to_state and gate_noisy_evolution
+// TODO: multi_qubit_Pauli_gate_partial_list is not implemented for multi-cpu
+// yet
 
 /**
  * \~english
  * Apply multi-qubit Pauli operator to the quantum state with a partial list.
  *
  * Apply multi-qubit Pauli operator to the quantum state with a partial list of
  * the Pauli operators. Pauli_operator_type_list must be a list of n single
@@ -951,14 +1042,17 @@
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void multi_qubit_Pauli_gate_partial_list_single_thread(
     const UINT* target_qubit_index_list, const UINT* Pauli_operator_type_list,
     UINT target_qubit_index_count, CTYPE* state, ITYPE dim);
+// This function is used in gate_noisy_evolution
+// TODO: multi_qubit_Pauli_gate_partial_list_single_thread is not implemented
+// for multi-cpu yet
 
 /**
  * \~english
  * Apply multi-qubit Pauli rotation operator to the quantum state with a whole
  * list.
  *
  * Apply multi-qubit Pauli rotation operator to state with a whole list of the
@@ -996,14 +1090,15 @@
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void multi_qubit_Pauli_rotation_gate_whole_list(
     const UINT* Pauli_operator_type_list, UINT qubit_count, double angle,
     CTYPE* state, ITYPE dim_);
+// Not implemented for multi-cpu
 
 /**
  * \~english
  * Apply multi-qubit Pauli rotation operator to the quantum state with a whole
  * list.
  *
  * Apply multi-qubit Pauli rotation operator to state with a whole list of the
@@ -1041,14 +1136,15 @@
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void multi_qubit_Pauli_rotation_gate_whole_list_single_thread(
     const UINT* Pauli_operator_type_list, UINT qubit_count, double angle,
     CTYPE* state, ITYPE dim_);
+// Not implemented for multi-cpu
 
 /**
  * \~english
  * Apply multi-qubit Pauli rotation operator to the quantum state with a partial
  * list.
  *
  * Apply multi-qubit Pauli rotation operator to state with a partial list of the
@@ -1088,14 +1184,17 @@
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void multi_qubit_Pauli_rotation_gate_partial_list(
     const UINT* target_qubit_index_list, const UINT* Pauli_operator_type_list,
     UINT target_qubit_index_count, double angle, CTYPE* state, ITYPE dim);
+// This function is used in ClsPauliRotationGate
+// TODO: multi_qubit_Pauli_rotation_gate_partial_list is not implemented for
+// multi-cpu yet
 
 /**
  * \~english
  * Apply multi-qubit Pauli rotation operator to the quantum state with a partial
  * list.
  *
  * Apply multi-qubit Pauli rotation operator to state with a partial list of the
@@ -1135,14 +1234,15 @@
  * @param[in,out] state 量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void multi_qubit_Pauli_rotation_gate_partial_list_single_thread(
     const UINT* target_qubit_index_list, const UINT* Pauli_operator_type_list,
     UINT target_qubit_index_count, double angle, CTYPE* state, ITYPE dim);
+// Not implemented for multi-cpu
 
 /**
  * \~english
  * Apply a two-qubit arbitrary gate.
  *
  * Apply a two-qubit arbitrary gate defined by a dense matrix as a
  * one-dimentional array matrix[].
@@ -1169,14 +1269,19 @@
  */
 DllExport void double_qubit_dense_matrix_gate_c(UINT target_qubit_index1,
     UINT target_qubit_index2, const CTYPE matrix[16], CTYPE* state, ITYPE dim);
 void double_qubit_dense_matrix_gate_nosimd(UINT target_qubit_index1,
     UINT target_qubit_index2, const CTYPE matrix[16], CTYPE* state, ITYPE dim);
 void double_qubit_dense_matrix_gate_simd(UINT target_qubit_index1,
     UINT target_qubit_index2, const CTYPE matrix[16], CTYPE* state, ITYPE dim);
+void double_qubit_dense_matrix_gate_sve(UINT target_qubit_index1,
+    UINT target_qubit_index2, const CTYPE matrix[16], CTYPE* state, ITYPE dim);
+DllExport void double_qubit_dense_matrix_gate_mpi(UINT target_qubit_index1,
+    UINT target_qubit_index2, const CTYPE matrix[16], CTYPE* state, ITYPE dim,
+    UINT inner_qc);
 
 /**
  * \~english
  * Apply a multi-qubit arbitrary gate.
  *
  * Apply a multi-qubit arbitrary gate defined by a dense matrix as a
  * one-dimentional array matrix[].
@@ -1217,14 +1322,17 @@
  */
 DllExport void multi_qubit_dense_matrix_gate(
     const UINT* target_qubit_index_list, UINT target_qubit_index_count,
     const CTYPE* matrix, CTYPE* state, ITYPE dim);
 void multi_qubit_dense_matrix_gate_parallel(const UINT* target_qubit_index_list,
     UINT target_qubit_index_count, const CTYPE* matrix, CTYPE* state,
     ITYPE dim);
+DllExport void multi_qubit_dense_matrix_gate_mpi(
+    const UINT* target_qubit_index_list, UINT target_qubit_index_count,
+    const CTYPE* matrix, CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply a single-qubit controlled multi-qubit gate.
  *
  * Apply a single-qubit controlled multi-qubit gate. The multi-qubit gate is by
  * a dense matrix as a one-dimentional array matrix[].
@@ -1269,14 +1377,18 @@
  * @param[in] dim 次元
  *
  */
 DllExport void single_qubit_control_multi_qubit_dense_matrix_gate(
     UINT control_qubit_index, UINT control_value,
     const UINT* target_qubit_index_list, UINT target_qubit_index_count,
     const CTYPE* matrix, CTYPE* state, ITYPE dim);
+DllExport void single_qubit_control_multi_qubit_dense_matrix_gate_mpi(
+    UINT control_qubit_index, UINT control_value,
+    const UINT* target_qubit_index_list, UINT target_qubit_index_count,
+    const CTYPE* matrix, CTYPE* state, ITYPE dim, UINT inner_qc);
 
 /**
  * \~english
  * Apply a multi-qubit controlled multi-qubit gate.
  *
  * Apply a multi-qubit controlled multi-qubit gate. The multi-qubit gate is by a
  * dense matrix as a one-dimentional array matrix[].
@@ -1324,27 +1436,34 @@
  *
  */
 DllExport void multi_qubit_control_multi_qubit_dense_matrix_gate(
     const UINT* control_qubit_index_list, const UINT* control_value_list,
     UINT control_qubit_index_count, const UINT* target_qubit_index_list,
     UINT target_qubit_index_count, const CTYPE* matrix, CTYPE* state,
     ITYPE dim);
+void multi_qubit_control_multi_qubit_dense_matrix_gate_mpi(
+    const UINT* control_qubit_index_list, const UINT* control_value_list,
+    UINT control_qubit_index_count, const UINT* target_qubit_index_list,
+    UINT target_qubit_index_count, const CTYPE* matrix, CTYPE* state, ITYPE dim,
+    UINT inner_qc);
 
 /**
  * Diagonal gate
  **/
 DllExport void multi_qubit_diagonal_matrix_gate(
     const UINT* target_qubit_index_list, UINT target_qubit_index_count,
     const CTYPE* diagonal_element, CTYPE* state, ITYPE dim);
+// Not implemented for multi-cpu
 
 DllExport void multi_qubit_control_multi_qubit_diagonal_matrix_gate(
     const UINT* control_qubit_index_list, const UINT* control_value_list,
     UINT control_qubit_index_count, const UINT* target_qubit_index_list,
     UINT target_qubit_index_count, const CTYPE* diagonal_element, CTYPE* state,
     ITYPE dim);
+// Not implemented for multi-cpu
 
 /**
  * \~english
  * Reflect state according to another given state.
  *
  * Reflect state according to another given state. When reflect quantum state
  * |a> to state |s>, unitary operator give by 2|s><s|-I is applied to |a>.
@@ -1364,14 +1483,16 @@
  * @param[in] reflection_state reflection gateのユニタリを特徴づける量子状態
  * @param[in,out] state quantum 更新する量子状態
  * @param[in] dim 次元
  *
  */
 DllExport void reflection_gate(
     const CTYPE* reflection_state, CTYPE* state, ITYPE dim);
+// This function is used in ClsStateReflectionGate
+// TODO: reflection_gate is not implemented for multi-cpu yet
 
 DllExport void state_add(const CTYPE* state_added, CTYPE* state, ITYPE dim);
 DllExport void state_add_with_coef(
     CTYPE coef, const CTYPE* state_added, CTYPE* state, ITYPE dim);
 DllExport void state_add_with_coef_single_thread(
     CTYPE coef, const CTYPE* state_added, CTYPE* state, ITYPE dim);
 DllExport void state_multiply(CTYPE coef, CTYPE* state, ITYPE dim);
@@ -1387,30 +1508,35 @@
  * @param[in] c_bit index of control qubit
  * @param[in] t_bit index of target qubit
  * @param[in,out] state quantum state
  * @param[in] dim dimension
  */
 DllExport void CUz_gate(
     double angle, UINT c_bit, UINT t_bit, CTYPE* state, ITYPE dim);
+// TODO: CUz_gate is not implemented for multi-cpu yet
+
 /**
  * update quantum state with large dense matrix
  *
  * update quantum state with large dense matrix
  * @param[in] k ???
  * @param[in] Nbits the number of qubits
  * @param[in] doSWAP ???
  * @param[in,out] state quantum state
  * @param[in] dim dimension
  */
 DllExport void qft(UINT k, UINT Nbits, int doSWAP, CTYPE* state, ITYPE dim);
+// TODO: qft is not implemented for multi-cpu yet
+
 /**
  * update quantum state with large dense matrix
  *
  * update quantum state with large dense matrix
  * @param[in] k ???
  * @param[in] Nbits the number of qubits
  * @param[in] doSWAP ???
  * @param[in,out] state quantum state
  * @param[in] dim dimension
  */
 DllExport void inverse_qft(
     UINT k, UINT Nbits, int doSWAP, CTYPE* state, ITYPE dim);
+// TODO: inverse_qft is not implemented for multi-cpu yet
```

### Comparing `qulacs-0.5.6/src/csim/update_ops_control_multi_target_multi.cpp` & `qulacs-0.6.0/src/csim/update_ops_reversible_boolean.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,46 @@
 
-#include <stdio.h>
-#include <stdlib.h>
-#include <string.h>
-
-#include "constant.hpp"
-#include "update_ops.hpp"
+#include "update_ops_cpp.hpp"
 #include "utility.hpp"
-#ifdef _OPENMP
-#include <omp.h>
-#endif
-
-void multi_qubit_control_multi_qubit_dense_matrix_gate(
-    const UINT* control_qubit_index_list, const UINT* control_value_list,
-    UINT control_qubit_index_count, const UINT* target_qubit_index_list,
-    UINT target_qubit_index_count, const CTYPE* matrix, CTYPE* state,
-    ITYPE dim) {
+
+void reversible_boolean_gate(const UINT* target_qubit_index_list,
+    UINT target_qubit_index_count,
+    std::function<ITYPE(ITYPE, ITYPE)> function_ptr, CTYPE* state, ITYPE dim) {
     // matrix dim, mask, buffer
     const ITYPE matrix_dim = 1ULL << target_qubit_index_count;
-    ITYPE* matrix_mask_list = create_matrix_mask_list(
+    const ITYPE* matrix_mask_list = create_matrix_mask_list(
         target_qubit_index_list, target_qubit_index_count);
-    CTYPE* buffer = (CTYPE*)malloc((size_t)(sizeof(CTYPE) * matrix_dim));
 
     // insert index
-    const UINT insert_index_count =
-        target_qubit_index_count + control_qubit_index_count;
-    UINT* sorted_insert_index_list = create_sorted_ui_list_list(
-        target_qubit_index_list, target_qubit_index_count,
-        control_qubit_index_list, control_qubit_index_count);
-
-    // control mask
-    ITYPE control_mask = create_control_mask(control_qubit_index_list,
-        control_value_list, control_qubit_index_count);
-
-    // loop varaibles
-    const ITYPE loop_dim =
-        dim >> (target_qubit_index_count + control_qubit_index_count);
-    ITYPE state_index;
+    const UINT* sorted_insert_index_list = create_sorted_ui_list(
+        target_qubit_index_list, target_qubit_index_count);
 
+    // loop variables
+    const ITYPE loop_dim = dim >> target_qubit_index_count;
+
+    CTYPE* buffer = (CTYPE*)malloc((size_t)(sizeof(CTYPE) * matrix_dim));
+    ITYPE state_index;
     for (state_index = 0; state_index < loop_dim; ++state_index) {
         // create base index
         ITYPE basis_0 = state_index;
-        for (UINT cursor = 0; cursor < insert_index_count; cursor++) {
+        for (UINT cursor = 0; cursor < target_qubit_index_count; cursor++) {
             UINT insert_index = sorted_insert_index_list[cursor];
             basis_0 = insert_zero_to_basis_index(
                 basis_0, 1ULL << insert_index, insert_index);
         }
 
-        // flip control masks
-        basis_0 ^= control_mask;
+        // compute matrix-vector multiply
 
-        // compute matrix mul
-        for (ITYPE y = 0; y < matrix_dim; ++y) {
-            buffer[y] = 0;
-            for (ITYPE x = 0; x < matrix_dim; ++x) {
-                buffer[y] += matrix[y * matrix_dim + x] *
-                             state[basis_0 ^ matrix_mask_list[x]];
-            }
+        for (ITYPE x = 0; x < matrix_dim; ++x) {
+            ITYPE y = function_ptr(x, matrix_dim);
+            buffer[y] = state[basis_0 ^ matrix_mask_list[x]];
         }
 
         // set result
         for (ITYPE y = 0; y < matrix_dim; ++y) {
             state[basis_0 ^ matrix_mask_list[y]] = buffer[y];
         }
     }
-    free(sorted_insert_index_list);
     free(buffer);
-    free(matrix_mask_list);
+    free((UINT*)sorted_insert_index_list);
+    free((ITYPE*)matrix_mask_list);
 }
```

### Comparing `qulacs-0.5.6/src/csim/update_ops_control_multi_target_single.cpp` & `qulacs-0.6.0/src/csim/update_ops_control_multi_target_single.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 
+#include "MPIutil.hpp"
 #include "constant.hpp"
 #include "update_ops.hpp"
 #include "utility.hpp"
 #ifdef _OPENMP
 #include <omp.h>
 #endif
 
@@ -286,7 +287,65 @@
 
             _mm256_storeu_pd(ptr0, data_r0);
             _mm256_storeu_pd(ptr1, data_r1);
         }
     }
 }
 #endif
+
+#ifdef _USE_MPI
+void multi_qubit_control_single_qubit_dense_matrix_gate_mpi(
+    const UINT* control_index_list, const UINT* control_value_list,
+    UINT control_count, UINT target_index, const CTYPE matrix[4], CTYPE* state,
+    ITYPE dim, UINT inner_qc) {
+    const UINT rank = MPIutil::get_inst().get_rank();
+
+    UINT control_count_local = 0;
+    UINT mask_control_global_0 = 0;
+    UINT mask_control_global_1 = 0;
+    UINT* index_list_buf =
+        (UINT*)malloc((size_t)(sizeof(UINT) * control_count * 2));
+
+    if (target_index < inner_qc) {  // target qubit is local
+        UINT* new_control_index_list = index_list_buf;
+        UINT* new_control_value_list = index_list_buf + control_count;
+        for (UINT i = 0; i < control_count; ++i)
+            if (control_index_list[i] < inner_qc) {
+                new_control_index_list[control_count_local] =
+                    control_index_list[i];
+                new_control_value_list[control_count_local] =
+                    control_value_list[i];
+                control_count_local++;
+            } else {
+                if (control_value_list[i] == 0)
+                    mask_control_global_0 |=
+                        1 << (control_index_list[i] - inner_qc);
+                else
+                    mask_control_global_1 |=
+                        1 << (control_index_list[i] - inner_qc);
+            }
+
+        if ((rank & mask_control_global_0) |
+            ((~rank) & mask_control_global_1)) {  // do nothing
+        } else {
+            multi_qubit_control_single_qubit_dense_matrix_gate(
+                new_control_index_list, new_control_value_list,
+                control_count_local, target_index, matrix, state, dim);
+        }
+    } else {  // target is outer
+        UINT* control_index_list_swapped = index_list_buf;
+        for (UINT i = 0; i < control_count; ++i)
+            if (control_index_list[i] == inner_qc - 1) {
+                control_index_list_swapped[i] = target_index;
+            } else {
+                control_index_list_swapped[i] = control_index_list[i];
+            }
+        SWAP_gate_mpi(target_index, inner_qc - 1, state, dim, inner_qc);
+        multi_qubit_control_single_qubit_dense_matrix_gate_mpi(
+            control_index_list_swapped, control_value_list, control_count,
+            inner_qc - 1, matrix, state, dim, inner_qc);
+        SWAP_gate_mpi(inner_qc - 1, target_index, state, dim, inner_qc);
+    }
+    free(index_list_buf);
+    return;
+}
+#endif
```

### Comparing `qulacs-0.5.6/src/csim/update_ops_cpp.hpp` & `qulacs-0.6.0/src/csim/update_ops_cpp.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/update_ops_dm.cpp` & `qulacs-0.6.0/src/csim/update_ops_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/update_ops_dm.hpp` & `qulacs-0.6.0/src/csim/update_ops_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/update_ops_matrix_dense_double_eigen.cpp` & `qulacs-0.6.0/src/csim/update_ops_matrix_dense_double_eigen.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/update_ops_matrix_dense_multi.cpp` & `qulacs-0.6.0/src/csim/stat_ops.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,158 @@
+#include "stat_ops.hpp"
 
-#include <assert.h>
+#include <math.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 
+#include "MPIutil.hpp"
 #include "constant.hpp"
-#include "update_ops.hpp"
 #include "utility.hpp"
-#ifdef _OPENMP
-#include <omp.h>
-#endif
-#ifdef _USE_SIMD
-#ifdef _MSC_VER
-#include <intrin.h>
-#else
-#include <x86intrin.h>
-#endif
-#endif
 
-void create_shift_mask_list_from_list_buf(
-    const UINT* array, UINT count, UINT* dst_array, ITYPE* dst_mask);
+// calculate norm
+double state_norm_squared(const CTYPE* state, ITYPE dim) {
+    ITYPE index;
+    double norm = 0;
 
-void multi_qubit_dense_matrix_gate(const UINT* target_qubit_index_list,
-    UINT target_qubit_index_count, const CTYPE* matrix, CTYPE* state,
-    ITYPE dim) {
-    if (target_qubit_index_count == 1) {
-        single_qubit_dense_matrix_gate(
-            target_qubit_index_list[0], matrix, state, dim);
-    } else if (target_qubit_index_count == 2) {
-        double_qubit_dense_matrix_gate_c(target_qubit_index_list[0],
-            target_qubit_index_list[1], matrix, state, dim);
-    } else {
 #ifdef _OPENMP
-        OMPutil::get_inst().set_qulacs_num_threads(dim, 10);
+    OMPutil::get_inst().set_qulacs_num_threads(dim, 10);
+#pragma omp parallel for reduction(+ : norm)
 #endif
-        multi_qubit_dense_matrix_gate_parallel(target_qubit_index_list,
-            target_qubit_index_count, matrix, state, dim);
+    for (index = 0; index < dim; ++index) {
+        norm += pow(_cabs(state[index]), 2);
+    }
 #ifdef _OPENMP
-        OMPutil::get_inst().reset_qulacs_num_threads();
+    OMPutil::get_inst().reset_qulacs_num_threads();
 #endif
-    }
+
+    return norm;
 }
 
-void create_shift_mask_list_from_list_buf(
-    const UINT* array, UINT count, UINT* dst_array, ITYPE* dst_mask) {
-    memcpy(dst_array, array, sizeof(UINT) * count);
-    sort_ui(dst_array, count);
-    for (UINT i = 0; i < count; ++i) {
-        dst_mask[i] = (1UL << dst_array[i]) - 1;
+// calculate norm
+double state_norm_squared_single_thread(const CTYPE* state, ITYPE dim) {
+    ITYPE index;
+    double norm = 0;
+    for (index = 0; index < dim; ++index) {
+        norm += pow(_cabs(state[index]), 2);
     }
+    return norm;
 }
 
-void multi_qubit_dense_matrix_gate_parallel(const UINT* target_qubit_index_list,
-    UINT target_qubit_index_count, const CTYPE* matrix, CTYPE* state,
-    ITYPE dim) {
-    UINT sort_array[64];
-    ITYPE mask_array[64];
-    create_shift_mask_list_from_list_buf(target_qubit_index_list,
-        target_qubit_index_count, sort_array, mask_array);
-
-    // matrix dim, mask, buffer
-    const ITYPE matrix_dim = 1ULL << target_qubit_index_count;
-    const ITYPE* matrix_mask_list = create_matrix_mask_list(
-        target_qubit_index_list, target_qubit_index_count);
-    // loop variables
-    const ITYPE loop_dim = dim >> target_qubit_index_count;
+// calculate norm for mpi
+#ifdef _USE_MPI
+double state_norm_squared_mpi(const CTYPE* state, ITYPE dim) {
+    ITYPE index;
+    double norm = 0;
 
 #ifdef _OPENMP
-    const UINT thread_count = omp_get_max_threads();
-#else
-    const UINT thread_count = 1;
+    OMPutil::get_inst().set_qulacs_num_threads(dim, 15);
+#pragma omp parallel for reduction(+ : norm)
+#endif
+    for (index = 0; index < dim; ++index) {
+        norm += pow(_cabs(state[index]), 2);
+    }
+#ifdef _OPENMP
+    OMPutil::get_inst().reset_qulacs_num_threads();
 #endif
-    CTYPE* buffer_list =
-        (CTYPE*)malloc((size_t)(sizeof(CTYPE) * matrix_dim * thread_count));
 
-    const ITYPE block_size = loop_dim / thread_count;
-    const ITYPE residual = loop_dim % thread_count;
+    MPIutil::get_inst().s_D_allreduce(&norm);
 
-#ifdef _OPENMP
-#pragma omp parallel
+    return norm;
+}
 #endif
-    {
+
+// calculate inner product of two state vector
+CTYPE
+state_inner_product(const CTYPE* state_bra, const CTYPE* state_ket, ITYPE dim) {
+    double real_sum = 0.;
+    double imag_sum = 0.;
+    ITYPE index;
+
+#ifdef _OPENMP
+    OMPutil::get_inst().set_qulacs_num_threads(dim, 15);
+#pragma omp parallel for reduction(+ : real_sum, imag_sum)
+#endif
+    for (index = 0; index < dim; ++index) {
+        CTYPE value;
+        value += conj(state_bra[index]) * state_ket[index];
+        real_sum += _creal(value);
+        imag_sum += _cimag(value);
+    }
 #ifdef _OPENMP
-        UINT thread_id = omp_get_thread_num();
-#else
-        UINT thread_id = 0;
+    OMPutil::get_inst().reset_qulacs_num_threads();
 #endif
-        ITYPE start_index = block_size * thread_id +
-                            (residual > thread_id ? thread_id : residual);
-        ITYPE end_index =
-            block_size * (thread_id + 1) +
-            (residual > (thread_id + 1) ? (thread_id + 1) : residual);
-        CTYPE* buffer = buffer_list + thread_id * matrix_dim;
 
-        ITYPE state_index;
-        for (state_index = start_index; state_index < end_index;
-             ++state_index) {
-            // create base index
-            ITYPE basis_0 = state_index;
-            for (UINT cursor = 0; cursor < target_qubit_index_count; ++cursor) {
-                basis_0 = (basis_0 & mask_array[cursor]) +
-                          ((basis_0 & (~mask_array[cursor])) << 1);
-            }
+    return real_sum + 1.i * imag_sum;
+}
 
-            // compute matrix-vector multiply
-            for (ITYPE y = 0; y < matrix_dim; ++y) {
-                buffer[y] = 0;
-                for (ITYPE x = 0; x < matrix_dim; ++x) {
-                    buffer[y] += matrix[y * matrix_dim + x] *
-                                 state[basis_0 ^ matrix_mask_list[x]];
-                }
-            }
+#ifdef _USE_MPI
+// calculate inner product of two state vector for mpi
+CTYPE
+state_inner_product_mpi(const CTYPE* state_bra, const CTYPE* state_ket,
+    ITYPE dim_bra, ITYPE dim_ket) {
+    CTYPE sum = 0.;
+    ITYPE index;
+    ITYPE dim = std::min(dim_bra, dim_ket);
+    MPIutil& m = MPIutil::get_inst();
+    const CTYPE* new_bra = state_bra;
+    const CTYPE* new_ket = state_ket;
+    ITYPE offs = m.get_rank() * dim;
+    if (dim_bra < dim_ket)
+        new_ket += offs;
+    else if (dim_bra > dim_ket)
+        new_bra += offs;
+
+    sum = state_inner_product(new_bra, new_ket, dim);
+    m.s_DC_allreduce(&sum);
+    return sum;
+}
+#endif
 
-            // set result
-            for (ITYPE y = 0; y < matrix_dim; ++y) {
-                state[basis_0 ^ matrix_mask_list[y]] = buffer[y];
+void state_tensor_product(const CTYPE* state_left, ITYPE dim_left,
+    const CTYPE* state_right, ITYPE dim_right, CTYPE* state_dst) {
+    ITYPE index_left, index_right;
+    for (index_left = 0; index_left < dim_left; ++index_left) {
+        CTYPE val_left = state_left[index_left];
+        for (index_right = 0; index_right < dim_right; ++index_right) {
+            state_dst[index_left * dim_right + index_right] =
+                val_left * state_right[index_right];
+        }
+    }
+}
+void state_permutate_qubit(const UINT* qubit_order, const CTYPE* state_src,
+    CTYPE* state_dst, UINT qubit_count, ITYPE dim) {
+    ITYPE index;
+    for (index = 0; index < dim; ++index) {
+        ITYPE src_index = 0;
+        for (UINT qubit_index = 0; qubit_index < qubit_count; ++qubit_index) {
+            if ((index >> qubit_index) % 2) {
+                src_index += 1ULL << qubit_order[qubit_index];
             }
         }
+        state_dst[index] = state_src[src_index];
+    }
+}
+
+void state_drop_qubits(const UINT* target, const UINT* projection,
+    UINT target_count, const CTYPE* state_src, CTYPE* state_dst, ITYPE dim) {
+    ITYPE dst_dim = dim >> target_count;
+    UINT* sorted_target = create_sorted_ui_list(target, target_count);
+    ITYPE projection_mask = 0;
+    for (UINT target_index = 0; target_index < target_count; ++target_index) {
+        projection_mask ^= (projection[target_index] << target[target_index]);
+    }
+
+    ITYPE index;
+    for (index = 0; index < dst_dim; ++index) {
+        ITYPE src_index = index;
+        for (UINT target_index = 0; target_index < target_count;
+             ++target_index) {
+            UINT insert_index = sorted_target[target_index];
+            src_index = insert_zero_to_basis_index(
+                src_index, 1ULL << insert_index, insert_index);
+        }
+        src_index ^= projection_mask;
+        state_dst[index] = state_src[src_index];
     }
-    free(buffer_list);
-    free((ITYPE*)matrix_mask_list);
+    free(sorted_target);
 }
```

### Comparing `qulacs-0.5.6/src/csim/update_ops_matrix_dense_multi_eigen.cpp` & `qulacs-0.6.0/src/csim/update_ops_matrix_dense_multi_eigen.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/update_ops_matrix_diagonal_multi.cpp` & `qulacs-0.6.0/src/csim/update_ops_matrix_diagonal_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/update_ops_matrix_phase_single.cpp` & `qulacs-0.6.0/src/csim/update_ops_named_projection.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,111 +1,116 @@
 
-#include <assert.h>
-#include <stdio.h>
-#include <stdlib.h>
-#include <string.h>
-
-#include "constant.hpp"
+#include "MPIutil.hpp"
 #include "update_ops.hpp"
 #include "utility.hpp"
-#ifdef _OPENMP
-#include <omp.h>
-#endif
 
 #ifdef _USE_SIMD
 #ifdef _MSC_VER
 #include <intrin.h>
 #else
 #include <x86intrin.h>
 #endif
 #endif
 
-void single_qubit_phase_gate(
-    UINT target_qubit_index, CTYPE phase, CTYPE* state, ITYPE dim) {
+void P0_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim) {
 #ifdef _OPENMP
-    OMPutil::get_inst().set_qulacs_num_threads(dim, 12);
+    OMPutil::get_inst().set_qulacs_num_threads(dim, 13);
 #endif
 
-#ifdef _USE_SIMD
-    single_qubit_phase_gate_parallel_simd(
-        target_qubit_index, phase, state, dim);
-#else
-    single_qubit_phase_gate_parallel_unroll(
-        target_qubit_index, phase, state, dim);
+    P0_gate_parallel(target_qubit_index, state, dim);
+
+#ifdef _OPENMP
+    OMPutil::get_inst().reset_qulacs_num_threads();
+#endif
+}
+
+void P1_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim) {
+#ifdef _OPENMP
+    OMPutil::get_inst().set_qulacs_num_threads(dim, 13);
 #endif
 
+    P1_gate_parallel(target_qubit_index, state, dim);
+
 #ifdef _OPENMP
     OMPutil::get_inst().reset_qulacs_num_threads();
 #endif
 }
 
-void single_qubit_phase_gate_parallel_unroll(
-    UINT target_qubit_index, CTYPE phase, CTYPE* state, ITYPE dim) {
-    // target tmask
-    const ITYPE mask = 1ULL << target_qubit_index;
+void P0_gate_parallel(UINT target_qubit_index, CTYPE* state, ITYPE dim) {
+    const ITYPE loop_dim = dim / 2;
+    const ITYPE mask = (1ULL << target_qubit_index);
     const ITYPE low_mask = mask - 1;
     const ITYPE high_mask = ~low_mask;
 
-    // loop varaibles
-    const ITYPE loop_dim = dim / 2;
-    if (target_qubit_index == 0) {
-        ITYPE state_index;
-#ifdef _OPENMP
-#pragma omp parallel for
-#endif
-        for (state_index = 1; state_index < dim; state_index += 2) {
-            state[state_index] *= phase;
-        }
-    } else {
-        ITYPE state_index;
+    ITYPE state_index;
 #ifdef _OPENMP
 #pragma omp parallel for
 #endif
-        for (state_index = 0; state_index < loop_dim; state_index += 2) {
-            ITYPE basis = (state_index & low_mask) +
-                          ((state_index & high_mask) << 1) + mask;
-            state[basis] *= phase;
-            state[basis + 1] *= phase;
-        }
+    for (state_index = 0; state_index < loop_dim; ++state_index) {
+        ITYPE temp_index =
+            (state_index & low_mask) + ((state_index & high_mask) << 1) + mask;
+        state[temp_index] = 0;
     }
 }
 
-#ifdef _USE_SIMD
-void single_qubit_phase_gate_parallel_simd(
-    UINT target_qubit_index, CTYPE phase, CTYPE* state, ITYPE dim) {
-    // target tmask
-    const ITYPE mask = 1ULL << target_qubit_index;
+void P1_gate_parallel(UINT target_qubit_index, CTYPE* state, ITYPE dim) {
+    const ITYPE loop_dim = dim / 2;
+    const ITYPE mask = (1ULL << target_qubit_index);
     const ITYPE low_mask = mask - 1;
     const ITYPE high_mask = ~low_mask;
 
-    // loop varaibles
-    const ITYPE loop_dim = dim / 2;
-    if (target_qubit_index == 0) {
-        ITYPE state_index;
+    ITYPE state_index;
+#ifdef _OPENMP
+#pragma omp parallel for
+#endif
+    for (state_index = 0; state_index < loop_dim; ++state_index) {
+        ITYPE temp_index =
+            (state_index & low_mask) + ((state_index & high_mask) << 1);
+        state[temp_index] = 0;
+    }
+}
+
+#ifdef _USE_MPI
+void P0_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc) {
+    if (target_qubit_index < inner_qc) {
+        P0_gate(target_qubit_index, state, dim);
+    } else {
+        const int rank = MPIutil::get_inst().get_rank();
+        const int pair_rank_bit = 1 << (target_qubit_index - inner_qc);
+        if ((rank & pair_rank_bit) != 0) {
 #ifdef _OPENMP
+            OMPutil::get_inst().set_qulacs_num_threads(dim, 13);
 #pragma omp parallel for
 #endif
-        for (state_index = 1; state_index < dim; state_index += 2) {
-            state[state_index] *= phase;
-        }
+            for (ITYPE iter = 0; iter < dim; ++iter) {
+                state[iter] = 0;
+            }
+#ifdef _OPENMP
+            OMPutil::get_inst().reset_qulacs_num_threads();
+#endif
+        }  // else nothing to do.
+    }
+}
+
+void P1_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc) {
+    if (target_qubit_index < inner_qc) {
+        P1_gate(target_qubit_index, state, dim);
     } else {
-        ITYPE state_index;
-        __m256d mv0 = _mm256_set_pd(
-            -_cimag(phase), _creal(phase), -_cimag(phase), _creal(phase));
-        __m256d mv1 = _mm256_set_pd(
-            _creal(phase), _cimag(phase), _creal(phase), _cimag(phase));
+        const int rank = MPIutil::get_inst().get_rank();
+        const int pair_rank_bit = 1 << (target_qubit_index - inner_qc);
+        if ((rank & pair_rank_bit) == 0) {
 #ifdef _OPENMP
+            OMPutil::get_inst().set_qulacs_num_threads(dim, 13);
 #pragma omp parallel for
 #endif
-        for (state_index = 0; state_index < loop_dim; state_index += 2) {
-            ITYPE basis = (state_index & low_mask) +
-                          ((state_index & high_mask) << 1) + mask;
-            double* ptr = (double*)(state + basis);
-            __m256d data = _mm256_loadu_pd(ptr);
-            __m256d data0 = _mm256_mul_pd(data, mv0);
-            __m256d data1 = _mm256_mul_pd(data, mv1);
-            data = _mm256_hadd_pd(data0, data1);
-            _mm256_storeu_pd(ptr, data);
-        }
+            for (ITYPE iter = 0; iter < dim; ++iter) {
+                state[iter] = 0;
+            }
+#ifdef _OPENMP
+            OMPutil::get_inst().reset_qulacs_num_threads();
+#endif
+        }  // else nothing to do.
     }
 }
 #endif
```

### Comparing `qulacs-0.5.6/src/csim/update_ops_named.cpp` & `qulacs-0.6.0/src/csim/update_ops_named.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,10 @@
 
-#include <stdio.h>
-#include <stdlib.h>
-#include <string.h>
-
-#include "constant.hpp"
 #include "update_ops.hpp"
 #include "utility.hpp"
-#ifdef _OPENMP
-#include <omp.h>
-#endif
 
 #ifdef _USE_SIMD
 #ifdef _MSC_VER
 #include <intrin.h>
 #else
 #include <x86intrin.h>
 #endif
@@ -44,7 +36,47 @@
     single_qubit_dense_matrix_gate(
         target_qubit_index, SQRT_Y_GATE_MATRIX, state, dim);
 }
 void sqrtYdag_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim) {
     single_qubit_dense_matrix_gate(
         target_qubit_index, SQRT_Y_DAG_GATE_MATRIX, state, dim);
 }
+#ifdef _USE_MPI
+void S_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc) {
+    single_qubit_phase_gate_mpi(target_qubit_index, 1.i, state, dim, inner_qc);
+}
+void Sdag_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc) {
+    single_qubit_phase_gate_mpi(target_qubit_index, -1.i, state, dim, inner_qc);
+}
+void T_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc) {
+    single_qubit_phase_gate_mpi(
+        target_qubit_index, (1. + 1.i) / sqrt(2.), state, dim, inner_qc);
+}
+void Tdag_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc) {
+    single_qubit_phase_gate_mpi(
+        target_qubit_index, (1. - 1.i) / sqrt(2.), state, dim, inner_qc);
+}
+void sqrtX_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc) {
+    single_qubit_dense_matrix_gate_mpi(
+        target_qubit_index, SQRT_X_GATE_MATRIX, state, dim, inner_qc);
+}
+void sqrtXdag_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc) {
+    single_qubit_dense_matrix_gate_mpi(
+        target_qubit_index, SQRT_X_DAG_GATE_MATRIX, state, dim, inner_qc);
+}
+void sqrtY_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc) {
+    single_qubit_dense_matrix_gate_mpi(
+        target_qubit_index, SQRT_Y_GATE_MATRIX, state, dim, inner_qc);
+}
+void sqrtYdag_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc) {
+    single_qubit_dense_matrix_gate_mpi(
+        target_qubit_index, SQRT_Y_DAG_GATE_MATRIX, state, dim, inner_qc);
+}
+#endif
```

### Comparing `qulacs-0.5.6/src/csim/update_ops_named_CNOT.cpp` & `qulacs-0.6.0/src/csim/update_ops_named_X.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-#include <stddef.h>
 
+#include <cstring>
+
+#include "MPIutil.hpp"
 #include "constant.hpp"
 #include "update_ops.hpp"
 #include "utility.hpp"
 #ifdef _OPENMP
 #include <omp.h>
 #endif
 
@@ -11,157 +13,144 @@
 #ifdef _MSC_VER
 #include <intrin.h>
 #else
 #include <x86intrin.h>
 #endif
 #endif
 
-void CNOT_gate(UINT control_qubit_index, UINT target_qubit_index, CTYPE* state,
-    ITYPE dim) {
+void X_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim) {
 #ifdef _OPENMP
     OMPutil::get_inst().set_qulacs_num_threads(dim, 13);
 #endif
 
 #ifdef _USE_SIMD
-    CNOT_gate_parallel_simd(
-        control_qubit_index, target_qubit_index, state, dim);
+    X_gate_parallel_simd(target_qubit_index, state, dim);
+#elif defined(_USE_SVE)
+    X_gate_parallel_sve(target_qubit_index, state, dim);
 #else
-    CNOT_gate_parallel_unroll(
-        control_qubit_index, target_qubit_index, state, dim);
+    X_gate_parallel_unroll(target_qubit_index, state, dim);
 #endif
 
 #ifdef _OPENMP
     OMPutil::get_inst().reset_qulacs_num_threads();
 #endif
 }
 
-void CNOT_gate_parallel_unroll(UINT control_qubit_index,
-    UINT target_qubit_index, CTYPE* state, ITYPE dim) {
-    const ITYPE loop_dim = dim / 4;
-
-    const ITYPE target_mask = 1ULL << target_qubit_index;
-    const ITYPE control_mask = 1ULL << control_qubit_index;
-
-    const UINT min_qubit_index =
-        get_min_ui(control_qubit_index, target_qubit_index);
-    const UINT max_qubit_index =
-        get_max_ui(control_qubit_index, target_qubit_index);
-    const ITYPE min_qubit_mask = 1ULL << min_qubit_index;
-    const ITYPE max_qubit_mask = 1ULL << (max_qubit_index - 1);
-    const ITYPE low_mask = min_qubit_mask - 1;
-    const ITYPE mid_mask = (max_qubit_mask - 1) ^ low_mask;
-    const ITYPE high_mask = ~(max_qubit_mask - 1);
-
+void X_gate_parallel_unroll(UINT target_qubit_index, CTYPE* state, ITYPE dim) {
+    const ITYPE loop_dim = dim / 2;
+    const ITYPE mask = (1ULL << target_qubit_index);
+    const ITYPE mask_low = mask - 1;
+    const ITYPE mask_high = ~mask_low;
     ITYPE state_index = 0;
     if (target_qubit_index == 0) {
-        // swap neighboring two basis
-#ifdef _OPENMP
+        ITYPE basis_index = 0;
 #pragma omp parallel for
-#endif
-        for (state_index = 0; state_index < loop_dim; ++state_index) {
-            ITYPE basis_index = ((state_index & mid_mask) << 1) +
-                                ((state_index & high_mask) << 2) + control_mask;
+        for (basis_index = 0; basis_index < dim; basis_index += 2) {
             CTYPE temp = state[basis_index];
             state[basis_index] = state[basis_index + 1];
             state[basis_index + 1] = temp;
         }
-    } else if (control_qubit_index == 0) {
-        // no neighboring swap
-#ifdef _OPENMP
-#pragma omp parallel for
-#endif
-        for (state_index = 0; state_index < loop_dim; ++state_index) {
-            ITYPE basis_index_0 =
-                (state_index & low_mask) + ((state_index & mid_mask) << 1) +
-                ((state_index & high_mask) << 2) + control_mask;
-            ITYPE basis_index_1 = basis_index_0 + target_mask;
-            CTYPE temp = state[basis_index_0];
-            state[basis_index_0] = state[basis_index_1];
-            state[basis_index_1] = temp;
-        }
     } else {
-        // a,a+1 is swapped to a^m, a^m+1, respectively
-#ifdef _OPENMP
 #pragma omp parallel for
-#endif
         for (state_index = 0; state_index < loop_dim; state_index += 2) {
             ITYPE basis_index_0 =
-                (state_index & low_mask) + ((state_index & mid_mask) << 1) +
-                ((state_index & high_mask) << 2) + control_mask;
-            ITYPE basis_index_1 = basis_index_0 + target_mask;
+                (state_index & mask_low) + ((state_index & mask_high) << 1);
+            ITYPE basis_index_1 = basis_index_0 + mask;
             CTYPE temp0 = state[basis_index_0];
             CTYPE temp1 = state[basis_index_0 + 1];
             state[basis_index_0] = state[basis_index_1];
             state[basis_index_0 + 1] = state[basis_index_1 + 1];
             state[basis_index_1] = temp0;
             state[basis_index_1 + 1] = temp1;
         }
     }
 }
 
 #ifdef _USE_SIMD
-void CNOT_gate_parallel_simd(UINT control_qubit_index, UINT target_qubit_index,
-    CTYPE* state, ITYPE dim) {
-    const ITYPE loop_dim = dim / 4;
-
-    const ITYPE target_mask = 1ULL << target_qubit_index;
-    const ITYPE control_mask = 1ULL << control_qubit_index;
-
-    const UINT min_qubit_index =
-        get_min_ui(control_qubit_index, target_qubit_index);
-    const UINT max_qubit_index =
-        get_max_ui(control_qubit_index, target_qubit_index);
-    const ITYPE min_qubit_mask = 1ULL << min_qubit_index;
-    const ITYPE max_qubit_mask = 1ULL << (max_qubit_index - 1);
-    const ITYPE low_mask = min_qubit_mask - 1;
-    const ITYPE mid_mask = (max_qubit_mask - 1) ^ low_mask;
-    const ITYPE high_mask = ~(max_qubit_mask - 1);
-
+void X_gate_parallel_simd(UINT target_qubit_index, CTYPE* state, ITYPE dim) {
+    const ITYPE loop_dim = dim / 2;
+    const ITYPE mask = (1ULL << target_qubit_index);
+    const ITYPE mask_low = mask - 1;
+    const ITYPE mask_high = ~mask_low;
     ITYPE state_index = 0;
+    // double* cast_state = (double*)state;
     if (target_qubit_index == 0) {
-        // swap neighboring two basis
-#ifdef _OPENMP
+        ITYPE basis_index = 0;
 #pragma omp parallel for
-#endif
-        for (state_index = 0; state_index < loop_dim; ++state_index) {
-            ITYPE basis_index = ((state_index & mid_mask) << 1) +
-                                ((state_index & high_mask) << 2) + control_mask;
+        for (basis_index = 0; basis_index < dim; basis_index += 2) {
             double* ptr = (double*)(state + basis_index);
             __m256d data = _mm256_loadu_pd(ptr);
             data = _mm256_permute4x64_pd(data,
                 78);  // (3210) -> (1032) : 1*2 + 4*3 + 16*0 + 64*1 = 2+12+64=78
             _mm256_storeu_pd(ptr, data);
         }
-    } else if (control_qubit_index == 0) {
-        // no neighboring swap
-#ifdef _OPENMP
-#pragma omp parallel for
-#endif
-        for (state_index = 0; state_index < loop_dim; ++state_index) {
-            ITYPE basis_index_0 =
-                (state_index & low_mask) + ((state_index & mid_mask) << 1) +
-                ((state_index & high_mask) << 2) + control_mask;
-            ITYPE basis_index_1 = basis_index_0 + target_mask;
-            CTYPE temp = state[basis_index_0];
-            state[basis_index_0] = state[basis_index_1];
-            state[basis_index_1] = temp;
-        }
     } else {
-        // a,a+1 is swapped to a^m, a^m+1, respectively
-#ifdef _OPENMP
 #pragma omp parallel for
-#endif
         for (state_index = 0; state_index < loop_dim; state_index += 2) {
             ITYPE basis_index_0 =
-                (state_index & low_mask) + ((state_index & mid_mask) << 1) +
-                ((state_index & high_mask) << 2) + control_mask;
-            ITYPE basis_index_1 = basis_index_0 + target_mask;
+                (state_index & mask_low) + ((state_index & mask_high) << 1);
+            ITYPE basis_index_1 = basis_index_0 + mask;
             double* ptr0 = (double*)(state + basis_index_0);
             double* ptr1 = (double*)(state + basis_index_1);
             __m256d data0 = _mm256_loadu_pd(ptr0);
             __m256d data1 = _mm256_loadu_pd(ptr1);
             _mm256_storeu_pd(ptr1, data0);
             _mm256_storeu_pd(ptr0, data1);
         }
     }
 }
 #endif
+
+#ifdef _USE_SVE
+void X_gate_parallel_sve(UINT target_qubit_index, CTYPE* state, ITYPE dim) {
+    const ITYPE loop_dim = dim / 2;
+    const ITYPE mask = (1ULL << target_qubit_index);
+    const ITYPE mask_low = mask - 1;
+    const ITYPE mask_high = ~mask_low;
+    ITYPE state_index = 0;
+
+    // # of complex128 numbers in an SVE register
+    ITYPE VL = svcntd() / 2;
+
+    if (mask < VL) {
+        X_gate_parallel_unroll(target_qubit_index, state, dim);
+    } else {
+#pragma omp parallel for
+        for (state_index = 0; state_index < loop_dim; state_index += VL) {
+            ITYPE basis_index_0 =
+                (state_index & mask_low) + ((state_index & mask_high) << 1);
+            ITYPE basis_index_1 = basis_index_0 + mask;
+
+            svfloat64_t sv_data0 =
+                svld1(svptrue_b64(), (double*)&state[basis_index_0]);
+            svfloat64_t sv_data1 =
+                svld1(svptrue_b64(), (double*)&state[basis_index_1]);
+            svst1(svptrue_b64(), (double*)&state[basis_index_0], sv_data1);
+            svst1(svptrue_b64(), (double*)&state[basis_index_1], sv_data0);
+        }
+    }
+}
+#endif
+
+#ifdef _USE_MPI
+void X_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc) {
+    if (target_qubit_index < inner_qc) {
+        X_gate(target_qubit_index, state, dim);
+    } else {
+        MPIutil& m = MPIutil::get_inst();
+        const int rank = m.get_rank();
+        ITYPE dim_work = dim;
+        ITYPE num_work = 0;
+        CTYPE* t = m.get_workarea(&dim_work, &num_work);
+        assert(num_work > 0);
+        const int pair_rank_bit = 1 << (target_qubit_index - inner_qc);
+        const int pair_rank = rank ^ pair_rank_bit;
+        CTYPE* si = state;
+        for (ITYPE i = 0; i < num_work; ++i) {
+            m.m_DC_sendrecv(si, t, dim_work, pair_rank);
+            memcpy(si, t, dim_work * sizeof(CTYPE));
+            si += dim_work;
+        }
+    }
+}
+#endif
```

### Comparing `qulacs-0.5.6/src/csim/update_ops_named_Z.cpp` & `qulacs-0.6.0/src/csim/update_ops_named_Z.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+#include "MPIutil.hpp"
 #include "constant.hpp"
 #include "update_ops.hpp"
 #include "utility.hpp"
 #ifdef _OPENMP
 #include <omp.h>
 #endif
 
@@ -17,14 +18,16 @@
 void Z_gate(UINT target_qubit_index, CTYPE* state, ITYPE dim) {
 #ifdef _OPENMP
     OMPutil::get_inst().set_qulacs_num_threads(dim, 13);
 #endif
 
 #ifdef _USE_SIMD
     Z_gate_parallel_simd(target_qubit_index, state, dim);
+#elif defined(_USE_SVE)
+    Z_gate_parallel_sve(target_qubit_index, state, dim);
 #else
     Z_gate_parallel_unroll(target_qubit_index, state, dim);
 #endif
 
 #ifdef _OPENMP
     OMPutil::get_inst().reset_qulacs_num_threads();
 #endif
@@ -82,7 +85,49 @@
             __m256d data0 = _mm256_loadu_pd(ptr0);
             data0 = _mm256_mul_pd(data0, minus_one);
             _mm256_storeu_pd(ptr0, data0);
         }
     }
 }
 #endif
+
+#ifdef _USE_SVE
+void Z_gate_parallel_sve(UINT target_qubit_index, CTYPE* state, ITYPE dim) {
+    const ITYPE loop_dim = dim / 2;
+    const ITYPE mask = (1ULL << target_qubit_index);
+    const ITYPE mask_low = mask - 1;
+    const ITYPE mask_high = ~mask_low;
+    ITYPE state_index = 0;
+
+    // # of complex128 numbers in an SVE register
+    ITYPE VL = svcntd() / 2;
+
+    if (mask < VL) {
+        Z_gate_parallel_unroll(target_qubit_index, state, dim);
+    } else {
+#pragma omp parallel for
+        for (state_index = 0; state_index < loop_dim; state_index += VL) {
+            ITYPE basis_index = (state_index & mask_low) +
+                                ((state_index & mask_high) << 1) + mask;
+            svfloat64_t sv_data =
+                svld1(svptrue_b64(), (double*)&state[basis_index]);
+            sv_data = svneg_z(svptrue_b64(), sv_data);
+            svst1(svptrue_b64(), (double*)&state[basis_index], sv_data);
+        }
+    }
+}
+#endif
+
+#ifdef _USE_MPI
+void Z_gate_mpi(
+    UINT target_qubit_index, CTYPE* state, ITYPE dim, UINT inner_qc) {
+    if (target_qubit_index < inner_qc) {
+        Z_gate(target_qubit_index, state, dim);
+    } else {
+        const int rank = MPIutil::get_inst().get_rank();
+        const int pair_rank_bit = 1 << (target_qubit_index - inner_qc);
+        if (rank & pair_rank_bit) {
+            state_multiply(-1., state, dim);
+        }
+    }
+}
+#endif
```

### Comparing `qulacs-0.5.6/src/csim/update_ops_named_state.cpp` & `qulacs-0.6.0/src/csim/update_ops_named_state.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -39,28 +39,30 @@
     const double normalize_factor = sqrt(1. / squared_norm);
     ITYPE state_index;
     for (state_index = 0; state_index < loop_dim; ++state_index) {
         state[state_index] *= normalize_factor;
     }
 }
 
+// TODO: support when one of the states is multi-cpu
 void state_add(const CTYPE* state_added, CTYPE* state, ITYPE dim) {
     ITYPE index;
 #ifdef _OPENMP
     OMPutil::get_inst().set_qulacs_num_threads(dim, 13);
 #pragma omp parallel for
 #endif
     for (index = 0; index < dim; ++index) {
         state[index] += state_added[index];
     }
 #ifdef _OPENMP
     OMPutil::get_inst().reset_qulacs_num_threads();
 #endif
 }
 
+// TODO: support when one of the states is multi-cpu
 void state_add_with_coef(
     CTYPE coef, const CTYPE* state_added, CTYPE* state, ITYPE dim) {
     ITYPE index;
 #ifdef _OPENMP
     OMPutil::get_inst().set_qulacs_num_threads(dim, 13);
 #pragma omp parallel for
 #endif
@@ -68,14 +70,15 @@
         state[index] += coef * state_added[index];
     }
 #ifdef _OPENMP
     OMPutil::get_inst().reset_qulacs_num_threads();
 #endif
 }
 
+// TODO: support when one of the states is multi-cpu
 void state_add_with_coef_single_thread(
     CTYPE coef, const CTYPE* state_added, CTYPE* state, ITYPE dim) {
     ITYPE index;
     for (index = 0; index < dim; ++index) {
         state[index] += coef * state_added[index];
     }
 }
```

### Comparing `qulacs-0.5.6/src/csim/update_ops_pauli_multi.cpp` & `qulacs-0.6.0/src/csim/update_ops_pauli_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/update_ops_qft.cpp` & `qulacs-0.6.0/src/csim/update_ops_qft.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/update_ops_reflection.cpp` & `qulacs-0.6.0/src/csim/update_ops_reflection.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/utility.cpp` & `qulacs-0.6.0/src/csim/utility.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/csim/utility.hpp` & `qulacs-0.6.0/src/csim/utility.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/CMakeLists.txt` & `qulacs-0.6.0/src/gpusim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/memory_ops.cu` & `qulacs-0.6.0/src/gpusim/memory_ops.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/memory_ops.h` & `qulacs-0.6.0/src/gpusim/memory_ops.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/memory_ops_device_functions.h` & `qulacs-0.6.0/src/gpusim/memory_ops_device_functions.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/stat_ops.cu` & `qulacs-0.6.0/src/gpusim/stat_ops.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/stat_ops.h` & `qulacs-0.6.0/src/gpusim/stat_ops.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/stat_ops_device_functions.h` & `qulacs-0.6.0/src/gpusim/stat_ops_device_functions.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/test.cpp` & `qulacs-0.6.0/src/gpusim/test.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/update_ops_cuda.h` & `qulacs-0.6.0/src/gpusim/update_ops_cuda.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/update_ops_cuda_device_functions.h` & `qulacs-0.6.0/src/gpusim/update_ops_cuda_device_functions.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/update_ops_multi.cu` & `qulacs-0.6.0/src/gpusim/update_ops_multi.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/update_ops_named.cu` & `qulacs-0.6.0/src/gpusim/update_ops_named.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/update_ops_single.cu` & `qulacs-0.6.0/src/gpusim/update_ops_single.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/util.cu` & `qulacs-0.6.0/src/gpusim/util.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/util.cuh` & `qulacs-0.6.0/src/gpusim/util.cuh`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/util.h` & `qulacs-0.6.0/src/gpusim/util.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/util_common.h` & `qulacs-0.6.0/src/gpusim/util_common.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/gpusim/util_func.h` & `qulacs-0.6.0/src/gpusim/util_func.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/GradCalculator.cpp` & `qulacs-0.6.0/src/vqcsim/GradCalculator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/boolean_formula.hpp` & `qulacs-0.6.0/src/vqcsim/boolean_formula.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/causalcone_simulator.hpp` & `qulacs-0.6.0/src/vqcsim/causalcone_simulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/differential.cpp` & `qulacs-0.6.0/src/vqcsim/differential.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/differential.hpp` & `qulacs-0.6.0/src/vqcsim/differential.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/loss_function.cpp` & `qulacs-0.6.0/src/vqcsim/loss_function.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/loss_function.hpp` & `qulacs-0.6.0/src/vqcsim/loss_function.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/optimizer.hpp` & `qulacs-0.6.0/src/vqcsim/optimizer.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/parametric_circuit.cpp` & `qulacs-0.6.0/src/vqcsim/parametric_circuit.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/parametric_circuit.hpp` & `qulacs-0.6.0/src/vqcsim/parametric_circuit.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/parametric_gate.hpp` & `qulacs-0.6.0/src/vqcsim/parametric_gate.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/parametric_gate_factory.cpp` & `qulacs-0.6.0/src/vqcsim/parametric_gate_factory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/parametric_gate_factory.hpp` & `qulacs-0.6.0/src/vqcsim/parametric_gate_factory.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/parametric_simulator.cpp` & `qulacs-0.6.0/src/vqcsim/parametric_simulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/parametric_simulator.hpp` & `qulacs-0.6.0/src/vqcsim/parametric_simulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/problem.hpp` & `qulacs-0.6.0/src/vqcsim/problem.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/src/vqcsim/solver.hpp` & `qulacs-0.6.0/src/vqcsim/solver.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/cppsim/test_KAK.cpp` & `qulacs-0.6.0/test/cppsim/test_KAK.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/cppsim/test_circuit.cpp` & `qulacs-0.6.0/test/cppsim/test_circuit.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/cppsim/test_circuit_optimize_light.cpp` & `qulacs-0.6.0/test/cppsim/test_circuit_optimize_light.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -277,7 +277,31 @@
         state.load(&org_state);
         copy_circuit->update_quantum_state(&state);
 
         ASSERT_STATE_NEAR(state, test_state, eps);
         delete copy_circuit;
     }
 }
+
+// see https://github.com/qulacs/qulacs/pull/514 for details.
+TEST(CircuitTest, FusedSWAPregression1) {
+    const UINT n = 4;
+    const UINT dim = 1ULL << n;
+
+    QuantumState opt_state(n), ref_state(n);
+    opt_state.set_Haar_random_state();
+    ref_state.load(&opt_state);
+    QuantumCircuit circuit(n);
+
+    circuit.add_H_gate(1);
+    circuit.add_FusedSWAP_gate(0, 2, 2);
+    circuit.add_H_gate(1);
+
+    QuantumCircuit* opt_circuit = circuit.copy();
+    QuantumCircuitOptimizer qco;
+    qco.optimize_light(opt_circuit);
+    circuit.update_quantum_state(&ref_state);
+    opt_circuit->update_quantum_state(&opt_state);
+
+    ASSERT_STATE_NEAR(ref_state, opt_state, eps);
+    delete opt_circuit;
+}
```

### Comparing `qulacs-0.5.6/test/cppsim/test_gate.cpp` & `qulacs-0.6.0/test/cppsim/test_gate.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -369,14 +369,57 @@
         gate->update_quantum_state(&state);
         delete gate;
         for (ITYPE i = 0; i < dim; ++i)
             ASSERT_NEAR(abs(state.data_cpp()[i] - test_state1[i]), 0, eps);
     }
 }
 
+void _ApplyFusedSWAPGate(UINT n, UINT target0, UINT target1, UINT block_size) {
+    const ITYPE dim = 1ULL << n;
+
+    QuantumState state_ref(n);
+    QuantumState state(n);
+
+    {
+        state_ref.set_Haar_random_state(2022);
+        state.load(&state_ref);
+
+        // update "state_ref" using SWAP gate
+        for (UINT i = 0; i < block_size; ++i) {
+            auto swap_gate = gate::SWAP(target0 + i, target1 + i);
+            swap_gate->update_quantum_state(&state_ref);
+            delete swap_gate;
+        }
+
+        // update "state" using FusedSWAP gate
+        auto bswap_gate = gate::FusedSWAP(target0, target1, block_size);
+        bswap_gate->update_quantum_state(&state);
+        delete bswap_gate;
+
+        for (ITYPE i = 0; i < dim; ++i)
+            ASSERT_NEAR(
+                abs(state.data_cpp()[i] - state_ref.data_cpp()[(i) % dim]), 0,
+                eps);
+    }
+}
+
+TEST(GateTest, ApplyFusedSWAPGate_10qubit_all) {
+    UINT n = 10;
+    for (UINT t0 = 0; t0 < n; ++t0) {
+        for (UINT t1 = 0; t1 < n; ++t1) {
+            if (t0 == t1) continue;
+            UINT max_bs = std::min(
+                (t0 < t1) ? (t1 - t0) : (t0 - t1), std::min(n - t0, n - t1));
+            for (UINT bs = 1; bs <= max_bs; ++bs) {
+                _ApplyFusedSWAPGate(n, t0, t1, bs);
+            }
+        }
+    }
+}
+
 TEST(GateTest, MergeTensorProduct) {
     UINT n = 2;
     ITYPE dim = 1ULL << n;
 
     auto x0 = gate::X(0);
     auto y1 = gate::Y(1);
     auto xy01 = gate::merge(x0, y1);
```

### Comparing `qulacs-0.5.6/test/cppsim/test_gate_dm.cpp` & `qulacs-0.6.0/test/cppsim/test_gate_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/cppsim/test_hamiltonian.cpp` & `qulacs-0.6.0/test/cppsim/test_hamiltonian.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/cppsim/test_hamiltonian_dm.cpp` & `qulacs-0.6.0/test/cppsim/test_hamiltonian_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/cppsim/test_noise_dm.cpp` & `qulacs-0.6.0/test/cppsim/test_noise_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/cppsim/test_noisesimulator.cpp` & `qulacs-0.6.0/test/cppsim/test_noisesimulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/cppsim/test_noisyevolution.cpp` & `qulacs-0.6.0/test/cppsim/test_noisyevolution.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/cppsim/test_pauli_operator.cpp` & `qulacs-0.6.0/test/cppsim/test_pauli_operator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/cppsim/test_simulator.cpp` & `qulacs-0.6.0/test/cppsim/test_simulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/cppsim/test_state.cpp` & `qulacs-0.6.0/test/cppsim/test_state.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/cppsim/test_state_dm.cpp` & `qulacs-0.6.0/test/cppsim/test_state_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/csim/test_memory.cpp` & `qulacs-0.6.0/test/csim/test_memory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/csim/test_omputil.cpp` & `qulacs-0.6.0/test/csim/test_omputil.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/csim/test_stat.cpp` & `qulacs-0.6.0/test/csim/test_stat.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -347,14 +347,19 @@
             ASSERT_NEAR(value.imag(), 0, eps);
             double test_expectation = value.real();
             double expectation =
                 expectation_value_multi_qubit_Pauli_operator_partial_list(
                     pauli_index.data(), pauli_partial.data(),
                     (UINT)pauli_index.size(), state, dim);
             ASSERT_NEAR(expectation, test_expectation, eps);
+            double expectation_st =
+                expectation_value_multi_qubit_Pauli_operator_partial_list_single_thread(
+                    pauli_index.data(), pauli_partial.data(),
+                    (UINT)pauli_index.size(), state, dim);
+            ASSERT_NEAR(expectation_st, test_expectation, eps);
         }
     }
     release_quantum_state(state);
 }
 
 // multi qubit expectation value whole
 TEST(StatOperationTest, MultiQubitExpectationValueZopPartialTest) {
@@ -408,14 +413,19 @@
             ASSERT_NEAR(value.imag(), 0, eps);
             double test_expectation = value.real();
             double expectation =
                 expectation_value_multi_qubit_Pauli_operator_partial_list(
                     pauli_index.data(), pauli_partial.data(),
                     (UINT)pauli_index.size(), state, dim);
             ASSERT_NEAR(expectation, test_expectation, eps);
+            double expectation_st =
+                expectation_value_multi_qubit_Pauli_operator_partial_list_single_thread(
+                    pauli_index.data(), pauli_partial.data(),
+                    (UINT)pauli_index.size(), state, dim);
+            ASSERT_NEAR(expectation_st, test_expectation, eps);
         }
     }
     release_quantum_state(state);
 }
 
 // multi qubit expectation value whole
 TEST(StatOperationTest, MultiQubitTransitionAmplitudeWholeTest) {
```

### Comparing `qulacs-0.5.6/test/csim/test_update_control.cpp` & `qulacs-0.6.0/test/csim/test_update_control.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,18 @@
         single_qubit_control_single_qubit_dense_matrix_gate);
     test_single_control_single_target(
         single_qubit_control_single_qubit_dense_matrix_gate_unroll);
 #ifdef _USE_SIMD
     test_single_control_single_target(
         single_qubit_control_single_qubit_dense_matrix_gate_simd);
 #endif
+#ifdef _USE_SVE
+    test_single_control_single_target(
+        single_qubit_control_single_qubit_dense_matrix_gate_sve512);
+#endif
 }
 
 void test_two_control_single_target(std::function<void(
         const UINT*, const UINT*, UINT, UINT, const CTYPE*, CTYPE*, ITYPE)>
         func) {
     const UINT n = 6;
     const ITYPE dim = 1ULL << n;
```

### Comparing `qulacs-0.5.6/test/csim/test_update_dense.cpp` & `qulacs-0.6.0/test/csim/test_update_dense.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
     test_single_dense_matrix_gate(single_qubit_dense_matrix_gate);
     test_single_dense_matrix_gate(single_qubit_dense_matrix_gate_parallel);
     test_single_dense_matrix_gate(
         single_qubit_dense_matrix_gate_parallel_unroll);
 #ifdef _USE_SIMD
     test_single_dense_matrix_gate(single_qubit_dense_matrix_gate_parallel_simd);
 #endif
+#ifdef _USE_SVE
+    test_single_dense_matrix_gate(single_qubit_dense_matrix_gate_parallel_sve);
+#endif
 }
 
 void test_general_dense_matrix_gate(
     std::function<void(const UINT*, UINT, const CTYPE*, CTYPE*, ITYPE)> func) {
     const UINT n = 6;
     const ITYPE dim = 1ULL << n;
     const UINT max_repeat = 10;
```

### Comparing `qulacs-0.5.6/test/csim/test_update_dense_double.cpp` & `qulacs-0.6.0/test/csim/test_update_dense_double.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -91,8 +91,11 @@
 
 TEST(UpdateTest, TwoQubitDenseMatrixTest) {
     test_double_dense_matrix_gate(double_qubit_dense_matrix_gate_c);
     test_double_dense_matrix_gate(double_qubit_dense_matrix_gate_nosimd);
 #ifdef _USE_SIMD
     test_double_dense_matrix_gate(double_qubit_dense_matrix_gate_simd);
 #endif
+#ifdef _USE_SVE
+    test_double_dense_matrix_gate(double_qubit_dense_matrix_gate_sve);
+#endif
 }
```

### Comparing `qulacs-0.5.6/test/csim/test_update_diagonal.cpp` & `qulacs-0.6.0/test/csim/test_update_diagonal.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,18 @@
     test_single_diagonal_matrix_gate(single_qubit_diagonal_matrix_gate);
     test_single_diagonal_matrix_gate(
         single_qubit_diagonal_matrix_gate_parallel_unroll);
 #ifdef _USE_SIMD
     test_single_diagonal_matrix_gate(
         single_qubit_diagonal_matrix_gate_parallel_simd);
 #endif
+#ifdef _USE_SVE
+    test_single_diagonal_matrix_gate(
+        single_qubit_diagonal_matrix_gate_parallel_sve);
+#endif
 }
 
 void test_single_phase_gate(
     std::function<void(UINT, CTYPE, CTYPE*, ITYPE)> func) {
     const UINT n = 6;
     const ITYPE dim = 1ULL << n;
     const UINT max_repeat = 10;
```

### Comparing `qulacs-0.5.6/test/csim/test_update_diagonal_multi.cpp` & `qulacs-0.6.0/test/csim/test_update_diagonal_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/csim/test_update_named.cpp` & `qulacs-0.6.0/test/csim/test_update_named.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -46,44 +46,88 @@
     Eigen::MatrixXcd mat(2, 2);
     mat << 0, 1, 1, 0;
     test_single_qubit_named_gate(6, "XGate", X_gate, mat);
     test_single_qubit_named_gate(6, "XGate", X_gate_parallel_unroll, mat);
 #ifdef _USE_SIMD
     test_single_qubit_named_gate(6, "XGate", X_gate_parallel_simd, mat);
 #endif
+#ifdef _USE_SVE
+    test_single_qubit_named_gate(
+        1, "XGate", X_gate_parallel_sve, mat);  //  256-bit
+    test_single_qubit_named_gate(
+        2, "XGate", X_gate_parallel_sve, mat);  //  512-bit
+    test_single_qubit_named_gate(
+        3, "XGate", X_gate_parallel_sve, mat);  // 1024-bit
+    test_single_qubit_named_gate(
+        4, "XGate", X_gate_parallel_sve, mat);  // 2048-bit
+    test_single_qubit_named_gate(6, "XGate", X_gate_parallel_sve, mat);
+#endif
 }
 TEST(UpdateTest, YGate) {
     Eigen::MatrixXcd mat(2, 2);
     mat << 0, -1.i, 1.i, 0;
     test_single_qubit_named_gate(6, "YGate", Y_gate, mat);
     test_single_qubit_named_gate(6, "YGate", Y_gate_parallel_unroll, mat);
 #ifdef _USE_SIMD
     test_single_qubit_named_gate(6, "YGate", Y_gate_parallel_simd, mat);
 #endif
+#ifdef _USE_SVE
+    test_single_qubit_named_gate(
+        1, "YGate", Y_gate_parallel_sve, mat);  //  256-bit
+    test_single_qubit_named_gate(
+        2, "YGate", Y_gate_parallel_sve, mat);  //  512-bit
+    test_single_qubit_named_gate(
+        3, "YGate", Y_gate_parallel_sve, mat);  // 1024-bit
+    test_single_qubit_named_gate(
+        4, "YGate", Y_gate_parallel_sve, mat);  // 2048-bit
+    test_single_qubit_named_gate(6, "YGate", Y_gate_parallel_sve, mat);
+#endif
 }
 TEST(UpdateTest, ZGate) {
     const UINT n = 3;
     Eigen::MatrixXcd mat(2, 2);
     mat << 1, 0, 0, -1;
     test_single_qubit_named_gate(6, "ZGate", Z_gate, mat);
     test_single_qubit_named_gate(6, "ZGate", Z_gate_parallel_unroll, mat);
 #ifdef _USE_SIMD
     test_single_qubit_named_gate(6, "ZGate", Z_gate_parallel_simd, mat);
 #endif
+#ifdef _USE_SVE
+    test_single_qubit_named_gate(
+        1, "ZGate", Z_gate_parallel_sve, mat);  //  256-bit
+    test_single_qubit_named_gate(
+        2, "ZGate", Z_gate_parallel_sve, mat);  //  512-bit
+    test_single_qubit_named_gate(
+        3, "ZGate", Z_gate_parallel_sve, mat);  // 1024-bit
+    test_single_qubit_named_gate(
+        4, "ZGate", Z_gate_parallel_sve, mat);  // 2048-bit
+    test_single_qubit_named_gate(6, "ZGate", Z_gate_parallel_sve, mat);
+#endif
 }
 TEST(UpdateTest, HGate) {
     const UINT n = 3;
     Eigen::MatrixXcd mat(2, 2);
     mat << 1, 1, 1, -1;
     mat /= sqrt(2.);
     test_single_qubit_named_gate(n, "HGate", H_gate, mat);
     test_single_qubit_named_gate(6, "HGate", H_gate_parallel_unroll, mat);
 #ifdef _USE_SIMD
     test_single_qubit_named_gate(6, "HGate", H_gate_parallel_simd, mat);
 #endif
+#ifdef _USE_SVE
+    test_single_qubit_named_gate(
+        1, "HGate", H_gate_parallel_sve, mat);  //  256-bit
+    test_single_qubit_named_gate(
+        2, "HGate", H_gate_parallel_sve, mat);  //  512-bit
+    test_single_qubit_named_gate(
+        3, "HGate", H_gate_parallel_sve, mat);  // 1024-bit
+    test_single_qubit_named_gate(
+        4, "HGate", H_gate_parallel_sve, mat);  // 2048-bit
+    test_single_qubit_named_gate(6, "HGate", H_gate_parallel_sve, mat);
+#endif
 }
 
 TEST(UpdateTest, SGate) {
     const UINT n = 3;
     Eigen::MatrixXcd mat(2, 2);
     mat << 1, 0, 0, 1.i;
     test_single_qubit_named_gate(n, "SGate", S_gate, mat);
@@ -251,31 +295,67 @@
         n, "CNOT", CNOT_gate, get_eigen_matrix_full_qubit_CNOT);
     test_two_qubit_named_gate(6, "CNOTGate", CNOT_gate_parallel_unroll,
         get_eigen_matrix_full_qubit_CNOT);
 #ifdef _USE_SIMD
     test_two_qubit_named_gate(6, "CNOTGate", CNOT_gate_parallel_simd,
         get_eigen_matrix_full_qubit_CNOT);
 #endif
+#ifdef _USE_SVE
+    test_two_qubit_named_gate(1, "CNOTGate", CNOT_gate_parallel_sve,
+        get_eigen_matrix_full_qubit_CNOT);  //  256-bit
+    test_two_qubit_named_gate(2, "CNOTGate", CNOT_gate_parallel_sve,
+        get_eigen_matrix_full_qubit_CNOT);  //  512-bit
+    test_two_qubit_named_gate(3, "CNOTGate", CNOT_gate_parallel_sve,
+        get_eigen_matrix_full_qubit_CNOT);  // 1024-bit
+    test_two_qubit_named_gate(4, "CNOTGate", CNOT_gate_parallel_sve,
+        get_eigen_matrix_full_qubit_CNOT);  // 2048-bit
+    test_two_qubit_named_gate(6, "CNOTGate", CNOT_gate_parallel_sve,
+        get_eigen_matrix_full_qubit_CNOT);
+#endif
 }
 
 TEST(UpdateTest, CZGate) {
     const UINT n = 4;
     test_two_qubit_named_gate(n, "CZ", CZ_gate, get_eigen_matrix_full_qubit_CZ);
     test_two_qubit_named_gate(
         6, "CZGate", CZ_gate_parallel_unroll, get_eigen_matrix_full_qubit_CZ);
 #ifdef _USE_SIMD
     test_two_qubit_named_gate(
         6, "CZGate", CZ_gate_parallel_simd, get_eigen_matrix_full_qubit_CZ);
 #endif
+#ifdef _USE_SVE
+    test_two_qubit_named_gate(1, "CZGate", CZ_gate_parallel_sve,
+        get_eigen_matrix_full_qubit_CZ);  //  256-bit
+    test_two_qubit_named_gate(2, "CZGate", CZ_gate_parallel_sve,
+        get_eigen_matrix_full_qubit_CZ);  //  512-bit
+    test_two_qubit_named_gate(3, "CZGate", CZ_gate_parallel_sve,
+        get_eigen_matrix_full_qubit_CZ);  // 1024-bit
+    test_two_qubit_named_gate(4, "CZGate", CZ_gate_parallel_sve,
+        get_eigen_matrix_full_qubit_CZ);  // 2048-bit
+    test_two_qubit_named_gate(
+        6, "CZGate", CZ_gate_parallel_sve, get_eigen_matrix_full_qubit_CZ);
+#endif
 }
 
 TEST(UpdateTest, SWAPGate) {
     const UINT n = 4;
     test_two_qubit_named_gate(
         n, "SWAP", SWAP_gate, get_eigen_matrix_full_qubit_SWAP);
     test_two_qubit_named_gate(6, "SWAPGate", SWAP_gate_parallel_unroll,
         get_eigen_matrix_full_qubit_SWAP);
 #ifdef _USE_SIMD
     test_two_qubit_named_gate(6, "SWAPGate", SWAP_gate_parallel_simd,
         get_eigen_matrix_full_qubit_SWAP);
 #endif
+#ifdef _USE_SVE
+    test_two_qubit_named_gate(1, "SWAPGate", SWAP_gate_parallel_sve,
+        get_eigen_matrix_full_qubit_SWAP);  //  256-bit
+    test_two_qubit_named_gate(2, "SWAPGate", SWAP_gate_parallel_sve,
+        get_eigen_matrix_full_qubit_SWAP);  //  512-bit
+    test_two_qubit_named_gate(3, "SWAPGate", SWAP_gate_parallel_sve,
+        get_eigen_matrix_full_qubit_SWAP);  // 1024-bit
+    test_two_qubit_named_gate(4, "SWAPGate", SWAP_gate_parallel_sve,
+        get_eigen_matrix_full_qubit_SWAP);  // 2048-bit
+    test_two_qubit_named_gate(6, "SWAPGate", SWAP_gate_parallel_sve,
+        get_eigen_matrix_full_qubit_SWAP);
+#endif
 }
```

### Comparing `qulacs-0.5.6/test/csim/test_update_pauli.cpp` & `qulacs-0.6.0/test/csim/test_update_pauli.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/gpusim/test_circuit.cpp` & `qulacs-0.6.0/test/gpusim/test_circuit.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/gpusim/test_compat_cpu.cpp` & `qulacs-0.6.0/test/gpusim/test_compat_cpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/gpusim/test_func_memory.cpp` & `qulacs-0.6.0/test/gpusim/test_func_memory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/gpusim/test_gate.cpp` & `qulacs-0.6.0/test/gpusim/test_gate.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -805,16 +805,16 @@
             test_state.load(&state);
             set_eigen_from_gpu(test_state_eigen, state, dim);
 
             // check equivalence
             assert_eigen_eq_gpu(test_state_eigen, state, dim, eps);
             assert_gpu_eq_gpu(test_state, state, dim, eps);
 
-            auto merged_gate1 = gate::Identity(0);
-            auto merged_gate2 = gate::Identity(0);
+            QuantumGateBase* merged_gate1 = gate::Identity(0);
+            QuantumGateBase* merged_gate2 = gate::Identity(0);
             QuantumGateMatrix* next_merged_gate = NULL;
             QuantumGateBase* new_gate = NULL;
             for (UINT gate_index = 0; gate_index < gate_count; ++gate_index) {
                 // pick random pauli
                 UINT new_pauli_id = (random.int32() % 3) + 1;
                 UINT target = random.int32() % n;
                 double di = random.uniform();
@@ -1084,14 +1084,16 @@
             ComplexVector test_state_eigen(dim);
             state.set_Haar_random_state();
             test_state.load(&state);
             set_eigen_from_gpu(test_state_eigen, state, dim);
             QuantumGateBase* merge_gate1 = gate::Identity(0);
             QuantumGateBase* merge_gate2 = gate::Identity(0);
 
+            std::random_device seed_gen;
+            std::mt19937 engine(seed_gen());
             for (UINT gate_index = 0; gate_index < gate_count; ++gate_index) {
                 std::shuffle(arr.begin(), arr.end(), engine);
                 UINT target = arr[0];
                 UINT control = arr[1];
                 auto new_gate = gate::CNOT(control, target);
                 merge_gate1 = gate::merge(merge_gate1, new_gate);
 
@@ -1128,14 +1130,16 @@
             ComplexVector test_state_eigen(dim);
             state.set_Haar_random_state();
             test_state.load(&state);
             set_eigen_from_gpu(test_state_eigen, state, dim);
             QuantumGateBase* merge_gate1 = gate::Identity(0);
             QuantumGateBase* merge_gate2 = gate::Identity(0);
 
+            std::random_device seed_gen;
+            std::mt19937 engine(seed_gen());
             for (UINT gate_index = 0; gate_index < gate_count; ++gate_index) {
                 std::shuffle(arr.begin(), arr.end(), engine);
                 UINT target = arr[0];
                 UINT control = arr[1];
                 auto new_gate = gate::CNOT(control, target);
                 merge_gate1 = gate::merge(merge_gate1, new_gate);
```

### Comparing `qulacs-0.5.6/test/gpusim/test_hamiltonian.cpp` & `qulacs-0.6.0/test/gpusim/test_hamiltonian.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/gpusim/test_state.cpp` & `qulacs-0.6.0/test/gpusim/test_state.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -427,14 +427,16 @@
 
             Eigen::MatrixXcd Identity(2, 2), X(2, 2), Y(2, 2), Z(2, 2);
             Identity << 1, 0, 0, 1;
             X << 0, 1, 1, 0;
             Z << 1, 0, 0, -1;
             Y << 0, -1.i, 1.i, 0;
 
+            std::random_device seed_gen;
+            std::mt19937 engine(seed_gen());
             for (UINT target = 0; target < n; ++target) {
                 // multi qubit expectation partial list value check
                 Eigen::MatrixXcd mat = Eigen::MatrixXcd::Identity(1, 1);
                 Eigen::MatrixXcd pauli_op;
 
                 std::vector<UINT> pauli_partial, pauli_index;
                 std::vector<std::pair<UINT, UINT>> pauli_partial_pair;
@@ -500,14 +502,16 @@
 
             Eigen::MatrixXcd Identity(2, 2), X(2, 2), Y(2, 2), Z(2, 2);
             Identity << 1, 0, 0, 1;
             X << 0, 1, 1, 0;
             Z << 1, 0, 0, -1;
             Y << 0, -1.i, 1.i, 0;
 
+            std::random_device seed_gen;
+            std::mt19937 engine(seed_gen());
             for (UINT target = 0; target < n; ++target) {
                 // multi qubit expectation partial list value check
                 Eigen::MatrixXcd mat = Eigen::MatrixXcd::Identity(1, 1);
                 Eigen::MatrixXcd pauli_op;
 
                 std::vector<UINT> pauli_partial, pauli_index;
                 std::vector<std::pair<UINT, UINT>> pauli_partial_pair;
@@ -745,14 +749,16 @@
                 state_ket_gpu, state_ket, dim, stream_ptr, idx);
             get_quantum_state_host(
                 state_bra_gpu, state_bra, dim, stream_ptr, idx);
 
             for (ITYPE i = 0; i < dim; ++i) test_state_ket[i] = state_ket[i];
             for (ITYPE i = 0; i < dim; ++i) test_state_bra[i] = state_bra[i];
 
+            std::random_device seed_gen;
+            std::mt19937 engine(seed_gen());
             for (UINT target = 0; target < n; ++target) {
                 // multi qubit expectation partial list value check
                 Eigen::MatrixXcd mat = Eigen::MatrixXcd::Identity(1, 1);
                 Eigen::MatrixXcd pauli_op;
 
                 std::vector<UINT> pauli_partial, pauli_index;
                 std::vector<std::pair<UINT, UINT>> pauli_partial_pair;
@@ -838,14 +844,16 @@
                 state_ket_gpu, state_ket, dim, stream_ptr, idx);
             get_quantum_state_host(
                 state_bra_gpu, state_bra, dim, stream_ptr, idx);
 
             for (ITYPE i = 0; i < dim; ++i) test_state_ket[i] = state_ket[i];
             for (ITYPE i = 0; i < dim; ++i) test_state_bra[i] = state_bra[i];
 
+            std::random_device seed_gen;
+            std::mt19937 engine(seed_gen());
             for (UINT target = 0; target < n; ++target) {
                 // multi qubit expectation partial list value check
                 Eigen::MatrixXcd mat = Eigen::MatrixXcd::Identity(1, 1);
                 Eigen::MatrixXcd pauli_op;
 
                 std::vector<UINT> pauli_partial, pauli_index;
                 std::vector<std::pair<UINT, UINT>> pauli_partial_pair;
```

### Comparing `qulacs-0.5.6/test/gpusim/test_update_control.cpp` & `qulacs-0.6.0/test/gpusim/test_update_control.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,16 @@
         auto state = allocate_quantum_state_host(dim, idx);
         initialize_Haar_random_state_host(state, dim, stream_ptr, idx);
         Eigen::VectorXcd test_state =
             copy_cpu_from_gpu(state, dim, stream_ptr, idx);
 
         Eigen::MatrixXcd whole_I = Eigen::MatrixXcd::Identity(dim, dim);
 
+        std::random_device seed_gen;
+        std::mt19937 engine(seed_gen());
         for (UINT rep = 0; rep < max_repeat; ++rep) {
             // single qubit 1-controlled qubit dense matrix gate
             U = get_eigen_matrix_random_single_qubit_unitary();
             U2 = get_eigen_matrix_random_single_qubit_unitary();
             std::shuffle(index_list.begin(), index_list.end(), engine);
             targets[0] = index_list[0];
             targets[1] = index_list[1];
@@ -153,14 +155,16 @@
         auto state = allocate_quantum_state_host(dim, idx);
         initialize_Haar_random_state_host(state, dim, stream_ptr, idx);
         Eigen::VectorXcd test_state =
             copy_cpu_from_gpu(state, dim, stream_ptr, idx);
 
         Eigen::MatrixXcd whole_I = Eigen::MatrixXcd::Identity(dim, dim);
 
+        std::random_device seed_gen;
+        std::mt19937 engine(seed_gen());
         for (UINT rep = 0; rep < max_repeat; ++rep) {
             // two qubit control-11 two qubit gate
             U = get_eigen_matrix_random_single_qubit_unitary();
             U2 = get_eigen_matrix_random_single_qubit_unitary();
             std::shuffle(index_list.begin(), index_list.end(), engine);
             targets[0] = index_list[0];
             targets[1] = index_list[1];
```

### Comparing `qulacs-0.5.6/test/gpusim/test_update_dense.cpp` & `qulacs-0.6.0/test/gpusim/test_update_dense.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -69,14 +69,16 @@
         auto state = allocate_quantum_state_host(dim, idx);
         initialize_Haar_random_state_host(state, dim, stream_ptr, idx);
         Eigen::VectorXcd test_state =
             copy_cpu_from_gpu(state, dim, stream_ptr, idx);
 
         Eigen::MatrixXcd whole_I = Eigen::MatrixXcd::Identity(dim, dim);
 
+        std::random_device seed_gen;
+        std::mt19937 engine(seed_gen());
         for (UINT rep = 0; rep < max_repeat; ++rep) {
             // two qubit dense matrix gate
             U = get_eigen_matrix_random_single_qubit_unitary();
             U2 = get_eigen_matrix_random_single_qubit_unitary();
 
             std::shuffle(index_list.begin(), index_list.end(), engine);
 
@@ -128,14 +130,16 @@
         Eigen::VectorXcd test_state =
             copy_cpu_from_gpu(state, dim, stream_ptr, idx);
 
         Eigen::MatrixXcd whole_I = Eigen::MatrixXcd::Identity(dim, dim);
 
         Eigen::Matrix<std::complex<double>, 8, 8, Eigen::RowMajor> Umerge;
 
+        std::random_device seed_gen;
+        std::mt19937 engine(seed_gen());
         for (UINT rep = 0; rep < max_repeat; ++rep) {
             // two qubit dense matrix gate
             U1 = get_eigen_matrix_random_single_qubit_unitary();
             U2 = get_eigen_matrix_random_single_qubit_unitary();
             U3 = get_eigen_matrix_random_single_qubit_unitary();
 
             std::shuffle(index_list.begin(), index_list.end(), engine);
@@ -187,14 +191,16 @@
         Eigen::VectorXcd test_state =
             copy_cpu_from_gpu(state, dim, stream_ptr, idx);
 
         Eigen::MatrixXcd whole_I = Eigen::MatrixXcd::Identity(dim, dim);
 
         Eigen::Matrix<std::complex<double>, 16, 16, Eigen::RowMajor> Umerge;
 
+        std::random_device seed_gen;
+        std::mt19937 engine(seed_gen());
         for (UINT rep = 0; rep < max_repeat; ++rep) {
             // two qubit dense matrix gate
             U1 = get_eigen_matrix_random_single_qubit_unitary();
             U2 = get_eigen_matrix_random_single_qubit_unitary();
             U3 = get_eigen_matrix_random_single_qubit_unitary();
             U4 = get_eigen_matrix_random_single_qubit_unitary();
 
@@ -250,14 +256,16 @@
         Eigen::VectorXcd test_state =
             copy_cpu_from_gpu(state, dim, stream_ptr, idx);
 
         Eigen::MatrixXcd whole_I = Eigen::MatrixXcd::Identity(dim, dim);
 
         Eigen::Matrix<std::complex<double>, 32, 32, Eigen::RowMajor> Umerge;
 
+        std::random_device seed_gen;
+        std::mt19937 engine(seed_gen());
         for (UINT rep = 0; rep < max_repeat; ++rep) {
             // two qubit dense matrix gate
             U1 = get_eigen_matrix_random_single_qubit_unitary();
             U2 = get_eigen_matrix_random_single_qubit_unitary();
             U3 = get_eigen_matrix_random_single_qubit_unitary();
             U4 = get_eigen_matrix_random_single_qubit_unitary();
             U5 = get_eigen_matrix_random_single_qubit_unitary();
@@ -318,14 +326,16 @@
         Eigen::VectorXcd test_state =
             copy_cpu_from_gpu(state, dim, stream_ptr, idx);
 
         Eigen::MatrixXcd whole_I = Eigen::MatrixXcd::Identity(dim, dim);
 
         Eigen::Matrix<std::complex<double>, 64, 64, Eigen::RowMajor> Umerge;
 
+        std::random_device seed_gen;
+        std::mt19937 engine(seed_gen());
         for (UINT rep = 0; rep < max_repeat; ++rep) {
             // two qubit dense matrix gate
             U1 = get_eigen_matrix_random_single_qubit_unitary();
             U2 = get_eigen_matrix_random_single_qubit_unitary();
             U3 = get_eigen_matrix_random_single_qubit_unitary();
             U4 = get_eigen_matrix_random_single_qubit_unitary();
             U5 = get_eigen_matrix_random_single_qubit_unitary();
```

### Comparing `qulacs-0.5.6/test/gpusim/test_update_diagonal.cpp` & `qulacs-0.6.0/test/gpusim/test_update_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/gpusim/test_update_named.cpp` & `qulacs-0.6.0/test/gpusim/test_update_named.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
             state, dim, 0, stream_ptr, idx);
 
         Eigen::VectorXcd test_state =
             copy_cpu_from_gpu(state, dim, stream_ptr, idx);
         std::vector<UINT> indices;
         for (UINT i = 0; i < n; ++i) indices.push_back(i);
 
+        std::random_device seed_gen;
+        std::mt19937 engine(seed_gen());
         for (UINT rep = 0; rep < max_repeat; ++rep) {
             for (UINT i = 0; i < n; ++i) {
                 UINT target = indices[i];
                 func(target, state, dim, stream_ptr, idx);
                 test_state =
                     get_expanded_eigen_matrix_with_identity(target, mat, n) *
                     test_state;
@@ -219,14 +221,16 @@
 void test_two_qubit_named_gate(UINT n, std::string name,
     std::function<void(UINT, UINT, void*, ITYPE, void*, UINT)> func,
     std::function<Eigen::MatrixXcd(UINT, UINT, UINT)> matfunc) {
     const ITYPE dim = 1ULL << n;
     const UINT max_repeat = 2;
 
     int ngpus = get_num_device();
+    std::random_device seed_gen;
+    std::mt19937 engine(seed_gen());
     for (int idx = 0; idx < ngpus; ++idx) {
         set_device(idx);
         auto stream_ptr = allocate_cuda_stream_host(1, idx);
         auto state = allocate_quantum_state_host(dim, idx);
         initialize_Haar_random_state_with_seed_host(
             state, dim, 0, stream_ptr, idx);
```

### Comparing `qulacs-0.5.6/test/gpusim/test_update_pauli.cpp` & `qulacs-0.6.0/test/gpusim/test_update_pauli.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,16 @@
         set_device(idx);
         auto stream_ptr = allocate_cuda_stream_host(1, idx);
         auto state = allocate_quantum_state_host(dim, idx);
         initialize_Haar_random_state_host(state, dim, stream_ptr, idx);
         Eigen::VectorXcd test_state =
             copy_cpu_from_gpu(state, dim, stream_ptr, idx);
 
+        std::random_device seed_gen;
+        std::mt19937 engine(seed_gen());
         for (UINT rep = 0; rep < max_repeat; ++rep) {
             // multi pauli whole
             std::vector<UINT> pauli_whole, pauli_partial, pauli_partial_index;
             std::vector<std::pair<UINT, UINT>> pauli_partial_pair;
 
             pauli_whole.resize(n);
             for (UINT i = 0; i < n; ++i) {
@@ -158,14 +160,16 @@
         auto state = allocate_quantum_state_host(dim, idx);
         initialize_Haar_random_state_host(state, dim, stream_ptr, idx);
         Eigen::VectorXcd test_state =
             copy_cpu_from_gpu(state, dim, stream_ptr, idx);
 
         Eigen::MatrixXcd whole_I = Eigen::MatrixXcd::Identity(dim, dim);
 
+        std::random_device seed_gen;
+        std::mt19937 engine(seed_gen());
         for (UINT rep = 0; rep < max_repeat; ++rep) {
             std::vector<UINT> pauli_whole, pauli_partial, pauli_partial_index;
             std::vector<std::pair<UINT, UINT>> pauli_partial_pair;
 
             // multi pauli rotation whole
             pauli_whole.resize(n);
             for (UINT i = 0; i < n; ++i) {
```

### Comparing `qulacs-0.5.6/test/gpusim/test_util.hpp` & `qulacs-0.6.0/test/gpusim/test_util.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/util/util.hpp` & `qulacs-0.6.0/test/util/util.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/vqcsim/test.cpp` & `qulacs-0.6.0/test/vqcsim/test.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.5.6/test/vqcsim/test_backprop.cpp` & `qulacs-0.6.0/test/vqcsim/test_backprop.cpp`

 * *Files identical despite different names*

