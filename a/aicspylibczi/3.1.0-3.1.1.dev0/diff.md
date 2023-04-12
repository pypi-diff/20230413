# Comparing `tmp/aicspylibczi-3.1.0.tar.gz` & `tmp/aicspylibczi-3.1.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicspylibczi-3.1.0.tar", last modified: Mon Feb 20 18:51:28 2023, max compression
+gzip compressed data, was "aicspylibczi-3.1.1.dev0.tar", last modified: Wed Apr 12 22:52:00 2023, max compression
```

## Comparing `aicspylibczi-3.1.0.tar` & `aicspylibczi-3.1.1.dev0.tar`

### file list

```diff
@@ -1,18 +1,655 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:51:28.894641 aicspylibczi-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-02-20 18:51:15.000000 aicspylibczi-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-02-20 18:51:28.894641 aicspylibczi-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-02-20 18:51:15.000000 aicspylibczi-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:51:28.894641 aicspylibczi-3.1.0/aicspylibczi/
--rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-02-20 18:51:15.000000 aicspylibczi-3.1.0/aicspylibczi/CziFile.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-20 18:51:15.000000 aicspylibczi-3.1.0/aicspylibczi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-20 18:51:15.000000 aicspylibczi-3.1.0/aicspylibczi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-02-20 18:51:16.000000 aicspylibczi-3.1.0/aicspylibczi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 18:51:28.894641 aicspylibczi-3.1.0/aicspylibczi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-02-20 18:51:28.000000 aicspylibczi-3.1.0/aicspylibczi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-20 18:51:28.000000 aicspylibczi-3.1.0/aicspylibczi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 18:51:28.000000 aicspylibczi-3.1.0/aicspylibczi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 18:51:28.000000 aicspylibczi-3.1.0/aicspylibczi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-20 18:51:28.000000 aicspylibczi-3.1.0/aicspylibczi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-20 18:51:28.000000 aicspylibczi-3.1.0/aicspylibczi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-20 18:51:28.894641 aicspylibczi-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-02-20 18:51:16.000000 aicspylibczi-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.643967 aicspylibczi-3.1.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-12 22:52:00.643967 aicspylibczi-3.1.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.563968 aicspylibczi-3.1.1.dev0/_aicspylibczi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/CSimpleStreamImplFromFd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/CSimpleStreamImplFromFd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/DimIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/DimIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/Image.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/Image.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/ImageFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/ImageFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/ImagesContainer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/IndexMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/IndexMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22052 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/Reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14433 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/Reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/SourceRange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/StreamImplLockingRead.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/StreamImplLockingRead.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/SubblockMetaVec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/SubblockSortable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/TargetRange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/Threadpool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/TypedImage.h
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/constants.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/helper_algorithms.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/inc_libCZI.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/pb_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/pb_caster_BytesIO.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/pb_caster_DimIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/pb_caster_ImagesContainer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/pb_caster_SubblockMetaVec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/pb_caster_libCZI_DimensionIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/pb_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/pb_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/pylibczi_ostream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/_aicspylibczi/pylibczi_ostream.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.563968 aicspylibczi-3.1.1.dev0/aicspylibczi/
+-rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/aicspylibczi/CziFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/aicspylibczi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/aicspylibczi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-12 22:51:47.000000 aicspylibczi-3.1.1.dev0/aicspylibczi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.563968 aicspylibczi-3.1.1.dev0/aicspylibczi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-04-12 22:52:00.000000 aicspylibczi-3.1.1.dev0/aicspylibczi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22028 2023-04-12 22:52:00.000000 aicspylibczi-3.1.1.dev0/aicspylibczi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 22:52:00.000000 aicspylibczi-3.1.1.dev0/aicspylibczi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 22:52:00.000000 aicspylibczi-3.1.1.dev0/aicspylibczi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-12 22:52:00.000000 aicspylibczi-3.1.1.dev0/aicspylibczi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 22:52:00.000000 aicspylibczi-3.1.1.dev0/aicspylibczi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.563968 aicspylibczi-3.1.1.dev0/libCZI/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 22:51:48.000000 aicspylibczi-3.1.1.dev0/libCZI/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.567968 aicspylibczi-3.1.1.dev0/libCZI/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.567968 aicspylibczi-3.1.1.dev0/libCZI/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/.github/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.567968 aicspylibczi-3.1.1.dev0/libCZI/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/.github/workflows/cla.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/.github/workflows/cmake.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/.github/workflows/mega-linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/.github/workflows/reuse.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/.mega-linter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.567968 aicspylibczi-3.1.1.dev0/libCZI/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/CPPLINT.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.567968 aicspylibczi-3.1.1.dev0/libCZI/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    42098 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/LICENSES/RSA-MD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.567968 aicspylibczi-3.1.1.dev0/libCZI/Src/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.571968 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/BitmapGen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   344178 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/BitmapGenFreeType.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/BitmapGenFreeType.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/BitmapGenGdiplus.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/BitmapGenGdiplus.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/BitmapGenNull.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/BitmapGenNull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/CZIcmd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/CZIcmd_Config.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/DisplaySettingsHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/IBitmapGen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/SaveBitmap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/SaveBitmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    70123 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/cmdlineoptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/cmdlineoptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/consoleio.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/consoleio.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41780 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/execute.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/execute.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/executeCreateCzi.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/executeCreateCzi.h
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/inc_CZIcmd_Config.h
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/inc_libCZI.h
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/inc_rapidjson.h
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/platform_defines.h
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/stdafx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/stdafx.h
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/targetver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/CZICmd/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)   124401 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.571968 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.579968 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/
+-rw-r--r--   0 runner    (1001) docker     (123)    31975 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRGlue.c
+-rw-r--r--   0 runner    (1001) docker     (123)    29672 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRGlue.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79862 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRGlueJxr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    69235 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRGluePFC.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRMeta.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRMeta.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRTest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRTest.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRTestBmp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRTestHdr.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRTestPnm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    27164 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRTestTif.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRTestWrapper.c
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRTestWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14928 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRTestYUV.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45760 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/JXRTranscode.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.579968 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/_x86/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/_x86/_x86.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12608 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/adapthuff.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/ansi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/decode.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/decode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/encode.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/encode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/image.c
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/jxr_defines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/perfTimer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/perfTimerANSI.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10268 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/postprocess.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/priv_guiddef.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42889 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/segdec.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43079 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/segenc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    37192 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/strFwdTransform.c
+-rw-r--r--   0 runner    (1001) docker     (123)    66836 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/strInvTransform.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/strPredQuant.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17865 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/strPredQuantDec.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/strPredQuantEnc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/strTransform.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/strTransform.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38332 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/strcodec.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22616 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/strcodec.h
+-rw-r--r--   0 runner    (1001) docker     (123)   147549 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/strdec.c
+-rw-r--r--   0 runner    (1001) docker     (123)    50202 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/strdec_x86.c
+-rw-r--r--   0 runner    (1001) docker     (123)    95696 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/strenc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/strenc_x86.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/windowsmediaphoto.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45103 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/wmsal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23104 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/wmspecstring.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/wmspecstrings_adt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56756 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/wmspecstrings_strict.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/Jxr/wmspecstrings_undef.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19611 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/JxrDecode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/JxrDecode.h
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/stdafx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/stdafx.h
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/JxrDecode/targetver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.591967 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/
+-rw-r--r--   0 runner    (1001) docker     (123)    15756 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/BitmapOperations.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/BitmapOperations.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/BitmapOperations.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CZIReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CZIReader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CreateBitmap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziAttachment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziAttachment.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziAttachmentsDirectory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziAttachmentsDirectory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziDimensionInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziDimensionInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14132 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziDisplaySettings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziDisplaySettings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziMetadata.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziMetadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36205 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziMetadataBuilder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziMetadataBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziMetadataDocumentInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziMetadataDocumentInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69987 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziMetadataDocumentInfo2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    40371 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziMetadataDocumentInfo2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziMetadataSegment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziMetadataSegment.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32099 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziParse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziParse.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36436 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziReaderWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziReaderWriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziStructs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziStructs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziSubBlock.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziSubBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziSubBlockDirectory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziSubBlockDirectory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziUtils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziUtils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    58313 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/CziWriter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/DimCoordinate.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.591967 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    24987 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/CZICmd_usage.markdown
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.595967 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/CZI_1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/CZI_2.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   629984 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/ScalingSingleChannelTileAccessor1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15606 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_2.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   508732 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_3.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   435548 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/SingleChannelTileAccessor_4.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    22752 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/Tinting-LUT.png
+-rw-r--r--   0 runner    (1001) docker     (123)    95014 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/VisualStudio_cmake1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   947057 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/ZEN_screenshot_1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   149904 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/ZEN_screenshot_2.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   242149 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/cmake_1_raspi.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    32954 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/cmake_1_raspi_help_freetype.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   270106 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/cmake_install_raspi1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    59883 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/cmake_raspi_unittests_1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/compositors_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/compositors_2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.595967 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/drawings/
+-rw-r--r--   0 runner    (1001) docker     (123)   100864 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/drawings/VS-project.pub
+-rw-r--r--   0 runner    (1001) docker     (123)   108032 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/drawings/VS-project_2.pub
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/gradationcurve_1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/gradationcurve_2.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/image_document_concept1.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    20658 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/image_document_concept2.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/image_document_concept3.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)    29100 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Images/image_document_concept4.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/Todos.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/accessors.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/building_libCZI.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)    92375 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/drawings.docx
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/image_document_concept.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/mainpage.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/multichannelcomposition.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/using_libCZI.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Doc/write_czi.markdown
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/FileHeaderSegmentData.h
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/ImportExport.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/IndexSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/IndexSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/MD5Sum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/MD5Sum.h
+-rw-r--r--   0 runner    (1001) docker     (123)    55139 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/MultiChannelCompositor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/MultiChannelCompositor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/SingleChannelAccessorBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/SingleChannelAccessorBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/SingleChannelPyramidLevelTileAccessor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/SingleChannelPyramidLevelTileAccessor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/SingleChannelScalingTileAccessor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/SingleChannelScalingTileAccessor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/SingleChannelTileAccessor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/SingleChannelTileAccessor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/SingleChannelTileCompositor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/SingleChannelTileCompositor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/Site.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19700 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/StreamImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/StreamImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10016 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/XmlNodeWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/bitmapData.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/decoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/decoder_wic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/decoder_wic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/decoder_zstd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/decoder_zstd.h
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/inc_libCZI_Config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34770 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29910 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_Compositor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_Config.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_DimCoordinate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_Helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_Lib.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    68869 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_Metadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)    62344 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_Metadata2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_Pixels.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_ReadWrite.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_Site.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_Site.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23328 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_Utilities.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_Utilities.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32167 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_Write.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40279 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_compress.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/libCZI_exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/priv_guiddef.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/pugiconfig.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   385316 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/pugixml.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    58161 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/pugixml.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/splines.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/splines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/stdAllocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/stdAllocator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/stdafx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/stdafx.h
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/targetver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/utilities.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/utilities.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/utilities_simd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI/zstdCompress.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.607967 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/CMakeLists.txt.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/MemInputOutputStream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/MemInputOutputStream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/MemOutputStream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/MemOutputStream.h
+-rw-r--r--   0 runner    (1001) docker     (123)   364946 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/MockMetadataSegment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/MockMetadataSegment.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/SegmentWalker.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/SegmentWalker.h
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/inc_libCZI.h
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/pch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/pch.h
+-rw-r--r--   0 runner    (1001) docker     (123)  8401252 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/testImage.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/testImage.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/testImage1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/testImageHiLo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_CziSubBlockDirectory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_DimCoordinate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_DisplaySettings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_IndexSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_JxrDecode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_LUT.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_StreamImplementations.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_Utilities.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_ZstdCompress.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_ZstdDecode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_bitmapOperations.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28041 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_metadatabuilder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25444 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_metadatareading.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_multichannelcomposite.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_reader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    44591 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_readerwriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_splines.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    79307 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/test_writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   728991 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/Src/libCZI_UnitTests/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/THIRD_PARTY_LICENSES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/cla_corporate.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/cla_individual.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.611967 aicspylibczi-3.1.1.dev0/libCZI/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/cmake/ExternalEIGEN3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/cmake/TestLargeFile.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/cmake/check_can_use_neon_intrinsics.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/cmake/check_unaligned_access.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 22:51:50.000000 aicspylibczi-3.1.1.dev0/libCZI/opencppcoverage.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.611967 aicspylibczi-3.1.1.dev0/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.clang-tidy
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.cmake-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.codespell-ignore-lines
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 22:51:49.000000 aicspylibczi-3.1.1.dev0/pybind11/.git
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.611967 aicspylibczi-3.1.1.dev0/pybind11/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.611967 aicspylibczi-3.1.1.dev0/pybind11/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/labeler_merged.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.611967 aicspylibczi-3.1.1.dev0/pybind11/.github/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/matchers/pylint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.611967 aicspylibczi-3.1.1.dev0/pybind11/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    31868 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.github/workflows/upstream.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.615967 aicspylibczi-3.1.1.dev0/pybind11/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.555968 aicspylibczi-3.1.1.dev0/pybind11/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.615967 aicspylibczi-3.1.1.dev0/pybind11/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.615967 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.619967 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/cast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26729 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.619967 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   114174 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/classes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.619967 aicspylibczi-3.1.1.dev0/pybind11/docs/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25777 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/compiling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    61034 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44653 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87708 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41121 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85853 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23489 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.555968 aicspylibczi-3.1.1.dev0/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.619967 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    65660 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.619967 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28251 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52929 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42613 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.623967 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)    31418 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79408 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   126420 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    94641 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.623967 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29747 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.623967 aicspylibczi-3.1.1.dev0/pybind11/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/pybind11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/pybind11/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/pybind11/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/pybind11/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/pybind11/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.639967 aicspylibczi-3.1.1.dev0/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.639967 aicspylibczi-3.1.1.dev0/pybind11/tests/extra_python_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.639967 aicspylibczi-3.1.1.dev0/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/local_bindings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/object.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_async.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_chrono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24874 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_class.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.639967 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.639967 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.639967 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.639967 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.639967 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.639967 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.639967 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_const_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19350 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_eigen_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_eigen_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_eigen_tensor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_eigen_tensor.inl
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_eigen_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.639967 aicspylibczi-3.1.1.dev0/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_iostream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21388 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30750 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_stl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_thread.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_union.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:52:00.643967 aicspylibczi-3.1.1.dev0/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-12 22:51:51.000000 aicspylibczi-3.1.1.dev0/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-12 22:52:00.643967 aicspylibczi-3.1.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-12 22:51:48.000000 aicspylibczi-3.1.1.dev0/setup.py
```

### Comparing `aicspylibczi-3.1.0/LICENSE` & `aicspylibczi-3.1.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.0/PKG-INFO` & `aicspylibczi-3.1.1.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicspylibczi
-Version: 3.1.0
+Version: 3.1.1.dev0
 Summary: A python module and a python extension for Zeiss (CZI/ZISRAW) microscopy files.
 Home-page: https://github.com/AllenCellModeling/aicspylibczi
 Author: Jamie Sherman, Paul Watkins
 Author-email: jamies@alleninstitute.org, pwatkins@gmail.com
 Keywords: aicspylibczi,allen cell,imaging,computational biology
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -12,15 +12,15 @@
 Provides-Extra: setup
 Provides-Extra: interactive
 Provides-Extra: all
 License-File: LICENSE
 
 # aicspylibczi
 
-[![C++ Build & Test](https://github.com/AllenCellModeling/aicspylibczi/workflows/C%2B%2B%20Build%20Main/badge.svg)](https://github.com/AllenCellModeling/aicspylibczi/actions)
+[![C++ Build & Test](https://github.com/AllenCellModeling/aicspylibczi/workflows/C%2B%2B%20Main%20Build/badge.svg)](https://github.com/AllenCellModeling/aicspylibczi/actions)
 [![Python Build & Test](https://github.com/AllenCellModeling/aicspylibczi/workflows/Python%20Build%20Main/badge.svg)](https://github.com/AllenCellModeling/aicspylibczi/actions)
 [![codecov](https://codecov.io/gh/AllenCellModeling/aicspylibczi/branch/master/graph/badge.svg)](https://codecov.io/gh/AllenCellModeling/aicspylibczi)
 [![License: GPLv3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/AllenCellModeling/aicspylibczi/blob/master/LICENSE)
 
 Python module to expose [libCZI](https://github.com/zeiss-microscopy/libCZI) functionality for reading (subset of) Zeiss
 CZI files and meta-data. We only support 64bit architectures currently if you desperately need 32 bit support please make an issue or modify the source and build it for your use case.
```

### Comparing `aicspylibczi-3.1.0/README.md` & `aicspylibczi-3.1.1.dev0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # aicspylibczi
 
-[![C++ Build & Test](https://github.com/AllenCellModeling/aicspylibczi/workflows/C%2B%2B%20Build%20Main/badge.svg)](https://github.com/AllenCellModeling/aicspylibczi/actions)
+[![C++ Build & Test](https://github.com/AllenCellModeling/aicspylibczi/workflows/C%2B%2B%20Main%20Build/badge.svg)](https://github.com/AllenCellModeling/aicspylibczi/actions)
 [![Python Build & Test](https://github.com/AllenCellModeling/aicspylibczi/workflows/Python%20Build%20Main/badge.svg)](https://github.com/AllenCellModeling/aicspylibczi/actions)
 [![codecov](https://codecov.io/gh/AllenCellModeling/aicspylibczi/branch/master/graph/badge.svg)](https://codecov.io/gh/AllenCellModeling/aicspylibczi)
 [![License: GPLv3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/AllenCellModeling/aicspylibczi/blob/master/LICENSE)
 
 Python module to expose [libCZI](https://github.com/zeiss-microscopy/libCZI) functionality for reading (subset of) Zeiss
 CZI files and meta-data. We only support 64bit architectures currently if you desperately need 32 bit support please make an issue or modify the source and build it for your use case.
```

### Comparing `aicspylibczi-3.1.0/aicspylibczi/CziFile.py` & `aicspylibczi-3.1.1.dev0/aicspylibczi/CziFile.py`

 * *Files identical despite different names*

### Comparing `aicspylibczi-3.1.0/aicspylibczi.egg-info/PKG-INFO` & `aicspylibczi-3.1.1.dev0/aicspylibczi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicspylibczi
-Version: 3.1.0
+Version: 3.1.1.dev0
 Summary: A python module and a python extension for Zeiss (CZI/ZISRAW) microscopy files.
 Home-page: https://github.com/AllenCellModeling/aicspylibczi
 Author: Jamie Sherman, Paul Watkins
 Author-email: jamies@alleninstitute.org, pwatkins@gmail.com
 Keywords: aicspylibczi,allen cell,imaging,computational biology
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -12,15 +12,15 @@
 Provides-Extra: setup
 Provides-Extra: interactive
 Provides-Extra: all
 License-File: LICENSE
 
 # aicspylibczi
 
-[![C++ Build & Test](https://github.com/AllenCellModeling/aicspylibczi/workflows/C%2B%2B%20Build%20Main/badge.svg)](https://github.com/AllenCellModeling/aicspylibczi/actions)
+[![C++ Build & Test](https://github.com/AllenCellModeling/aicspylibczi/workflows/C%2B%2B%20Main%20Build/badge.svg)](https://github.com/AllenCellModeling/aicspylibczi/actions)
 [![Python Build & Test](https://github.com/AllenCellModeling/aicspylibczi/workflows/Python%20Build%20Main/badge.svg)](https://github.com/AllenCellModeling/aicspylibczi/actions)
 [![codecov](https://codecov.io/gh/AllenCellModeling/aicspylibczi/branch/master/graph/badge.svg)](https://codecov.io/gh/AllenCellModeling/aicspylibczi)
 [![License: GPLv3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/AllenCellModeling/aicspylibczi/blob/master/LICENSE)
 
 Python module to expose [libCZI](https://github.com/zeiss-microscopy/libCZI) functionality for reading (subset of) Zeiss
 CZI files and meta-data. We only support 64bit architectures currently if you desperately need 32 bit support please make an issue or modify the source and build it for your use case.
```

### Comparing `aicspylibczi-3.1.0/aicspylibczi.egg-info/requires.txt` & `aicspylibczi-3.1.1.dev0/aicspylibczi.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 numpy>=1.14.1
 
 [all]
 numpy>=1.14.1
-codecov
 flake8
 pytest
 pytest-cov
 pytest-raises
 pytest-xdist
 pytest-runner
 bump2version>=1.0.1
@@ -54,13 +53,12 @@
 matplotlib
 pillow
 
 [setup]
 pytest-runner
 
 [test]
-codecov
 flake8
 pytest
 pytest-cov
 pytest-raises
 pytest-xdist
```

### Comparing `aicspylibczi-3.1.0/setup.cfg` & `aicspylibczi-3.1.1.dev0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 3.1.0
+current_version = 3.1.1.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `aicspylibczi-3.1.0/setup.py` & `aicspylibczi-3.1.1.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     readme = readme_file.read()
 
 requirements = [
     "numpy>=1.14.1",
 ]
 
 test_requirements = [
-    "codecov",
     "flake8",
     "pytest",
     "pytest-cov",
     "pytest-raises",
     "pytest-xdist",
 ]
 
@@ -104,15 +103,15 @@
         subprocess.check_call(['cmake', ext.sourcedir] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call(['cmake', '--build', '.', '--target', '_aicspylibczi'] + build_args, cwd=self.build_temp, env=env)
 
 setup(
     name='aicspylibczi',
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.md
-    version='3.1.0',
+    version='3.1.1.dev0',
     author='Jamie Sherman, Paul Watkins',
     author_email='jamies@alleninstitute.org, pwatkins@gmail.com',
     description='A python module and a python extension for Zeiss (CZI/ZISRAW) microscopy files.',
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="aicspylibczi, allen cell, imaging, computational biology",
```

