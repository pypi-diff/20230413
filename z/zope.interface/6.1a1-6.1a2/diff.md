# Comparing `tmp/zope.interface-6.1a1.tar.gz` & `tmp/zope.interface-6.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.interface-6.1a1.tar", last modified: Thu Apr  6 05:52:36 2023, max compression
+gzip compressed data, was "zope.interface-6.1a2.tar", last modified: Thu Apr 13 06:24:13 2023, max compression
```

## Comparing `zope.interface-6.1a1.tar` & `zope.interface-6.1a2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-06 05:52:36.503778 zope.interface-6.1a1/
--rw-r--r--   0 mac        (513) staff       (20)      588 2023-04-06 05:52:35.000000 zope.interface-6.1a1/.coveragerc
--rwxr-xr-x   0 mac        (513) staff       (20)     2183 2023-04-06 05:52:35.000000 zope.interface-6.1a1/.manylinux-install.sh
--rwxr-xr-x   0 mac        (513) staff       (20)      509 2023-04-06 05:52:35.000000 zope.interface-6.1a1/.manylinux.sh
--rw-r--r--   0 mac        (513) staff       (20)    38556 2023-04-06 05:52:35.000000 zope.interface-6.1a1/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      799 2023-04-06 05:52:35.000000 zope.interface-6.1a1/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2023-04-06 05:52:35.000000 zope.interface-6.1a1/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2023-04-06 05:52:35.000000 zope.interface-6.1a1/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      564 2023-04-06 05:52:35.000000 zope.interface-6.1a1/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    41102 2023-04-06 05:52:36.503939 zope.interface-6.1a1/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1353 2023-04-06 05:52:35.000000 zope.interface-6.1a1/README.rst
--rw-r--r--   0 mac        (513) staff       (20)     1949 2023-04-06 05:52:35.000000 zope.interface-6.1a1/appveyor.yml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-06 05:52:36.474638 zope.interface-6.1a1/benchmarks/
--rw-r--r--   0 mac        (513) staff       (20)     8497 2023-04-06 05:52:35.000000 zope.interface-6.1a1/benchmarks/micro.py
--rw-r--r--   0 mac        (513) staff       (20)      838 2023-04-06 05:52:35.000000 zope.interface-6.1a1/build.cmd
--rw-r--r--   0 mac        (513) staff       (20)      215 2023-04-06 05:52:35.000000 zope.interface-6.1a1/buildout.cfg
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-06 05:52:36.480231 zope.interface-6.1a1/docs/
--rw-r--r--   0 mac        (513) staff       (20)     5592 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)    41051 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/README.rst
--rw-r--r--   0 mac        (513) staff       (20)    33998 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/README.ru.rst
--rw-r--r--   0 mac        (513) staff       (20)    18817 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/adapter.rst
--rw-r--r--   0 mac        (513) staff       (20)    21169 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/adapter.ru.rst
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-06 05:52:36.482420 zope.interface-6.1a1/docs/api/
--rw-r--r--   0 mac        (513) staff       (20)      691 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/api/adapters.rst
--rw-r--r--   0 mac        (513) staff       (20)     1283 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/api/common.rst
--rw-r--r--   0 mac        (513) staff       (20)     2465 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/api/components.rst
--rw-r--r--   0 mac        (513) staff       (20)    21746 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/api/declarations.rst
--rw-r--r--   0 mac        (513) staff       (20)      165 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/api/index.rst
--rw-r--r--   0 mac        (513) staff       (20)      687 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/api/ro.rst
--rw-r--r--   0 mac        (513) staff       (20)     9948 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/api/specifications.rst
--rw-r--r--   0 mac        (513) staff       (20)       28 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/changes.rst
--rw-r--r--   0 mac        (513) staff       (20)     9091 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)     1742 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/foodforthought.rst
--rw-r--r--   0 mac        (513) staff       (20)     9509 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/hacking.rst
--rw-r--r--   0 mac        (513) staff       (20)     6537 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/human.rst
--rw-r--r--   0 mac        (513) staff       (20)    10681 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/human.ru.rst
--rw-r--r--   0 mac        (513) staff       (20)      639 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)     5110 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/make.bat
--rw-r--r--   0 mac        (513) staff       (20)    10222 2023-04-06 05:52:35.000000 zope.interface-6.1a1/docs/verify.rst
--rw-r--r--   0 mac        (513) staff       (20)      286 2023-04-06 05:52:35.000000 zope.interface-6.1a1/rtd.txt
--rw-r--r--   0 mac        (513) staff       (20)      604 2023-04-06 05:52:36.504588 zope.interface-6.1a1/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     4885 2023-04-06 05:52:35.000000 zope.interface-6.1a1/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-06 05:52:36.467862 zope.interface-6.1a1/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-06 05:52:36.482761 zope.interface-6.1a1/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       56 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-06 05:52:36.490485 zope.interface-6.1a1/src/zope/interface/
--rw-r--r--   0 mac        (513) staff       (20)     3463 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     4369 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/_compat.py
--rw-r--r--   0 mac        (513) staff       (20)     1056 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/_flatten.py
--rw-r--r--   0 mac        (513) staff       (20)    57678 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/_zope_interface_coptimizations.c
--rw-r--r--   0 mac        (513) staff       (20)    36218 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/adapter.py
--rw-r--r--   0 mac        (513) staff       (20)     3890 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/advice.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-06 05:52:36.493476 zope.interface-6.1a1/src/zope/interface/common/
--rw-r--r--   0 mac        (513) staff       (20)    10461 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     3027 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/builtins.py
--rw-r--r--   0 mac        (513) staff       (20)     6792 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/collections.py
--rw-r--r--   0 mac        (513) staff       (20)    20858 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/idatetime.py
--rw-r--r--   0 mac        (513) staff       (20)     5367 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     1241 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/io.py
--rw-r--r--   0 mac        (513) staff       (20)     4677 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/mapping.py
--rw-r--r--   0 mac        (513) staff       (20)     1682 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/numbers.py
--rw-r--r--   0 mac        (513) staff       (20)     5525 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/sequence.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-06 05:52:36.496095 zope.interface-6.1a1/src/zope/interface/common/tests/
--rw-r--r--   0 mac        (513) staff       (20)     5310 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     3906 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/tests/basemapping.py
--rw-r--r--   0 mac        (513) staff       (20)     1345 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/tests/test_builtins.py
--rw-r--r--   0 mac        (513) staff       (20)     5724 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/tests/test_collections.py
--rw-r--r--   0 mac        (513) staff       (20)     1594 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/tests/test_idatetime.py
--rw-r--r--   0 mac        (513) staff       (20)      812 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/tests/test_import_interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     1597 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/tests/test_io.py
--rw-r--r--   0 mac        (513) staff       (20)     1394 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/common/tests/test_numbers.py
--rw-r--r--   0 mac        (513) staff       (20)    42843 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/declarations.py
--rw-r--r--   0 mac        (513) staff       (20)     4067 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/document.py
--rw-r--r--   0 mac        (513) staff       (20)     8635 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/exceptions.py
--rw-r--r--   0 mac        (513) staff       (20)    38825 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/interface.py
--rw-r--r--   0 mac        (513) staff       (20)    50125 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)    25828 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/registry.py
--rw-r--r--   0 mac        (513) staff       (20)    24155 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/ro.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-06 05:52:36.503452 zope.interface-6.1a1/src/zope/interface/tests/
--rw-r--r--   0 mac        (513) staff       (20)     3961 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      897 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/advisory_testing.py
--rw-r--r--   0 mac        (513) staff       (20)      911 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/dummy.py
--rw-r--r--   0 mac        (513) staff       (20)      889 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/idummy.py
--rw-r--r--   0 mac        (513) staff       (20)      812 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/m1.py
--rw-r--r--   0 mac        (513) staff       (20)     3015 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/odd.py
--rw-r--r--   0 mac        (513) staff       (20)    79548 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/test_adapter.py
--rw-r--r--   0 mac        (513) staff       (20)     5962 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/test_advice.py
--rw-r--r--   0 mac        (513) staff       (20)     1290 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/test_compile_flags.py
--rw-r--r--   0 mac        (513) staff       (20)    82128 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/test_declarations.py
--rw-r--r--   0 mac        (513) staff       (20)    16899 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/test_document.py
--rw-r--r--   0 mac        (513) staff       (20)     1118 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/test_element.py
--rw-r--r--   0 mac        (513) staff       (20)     6411 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/test_exceptions.py
--rw-r--r--   0 mac        (513) staff       (20)    91465 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/test_interface.py
--rw-r--r--   0 mac        (513) staff       (20)     4377 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/test_interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     7565 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/test_odd_declarations.py
--rw-r--r--   0 mac        (513) staff       (20)   112819 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/test_registry.py
--rw-r--r--   0 mac        (513) staff       (20)    14121 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/test_ro.py
--rw-r--r--   0 mac        (513) staff       (20)     1933 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/test_sorting.py
--rw-r--r--   0 mac        (513) staff       (20)    19190 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/tests/test_verify.py
--rw-r--r--   0 mac        (513) staff       (20)     7154 2023-04-06 05:52:35.000000 zope.interface-6.1a1/src/zope/interface/verify.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-06 05:52:36.485315 zope.interface-6.1a1/src/zope.interface.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    41102 2023-04-06 05:52:36.000000 zope.interface-6.1a1/src/zope.interface.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     2921 2023-04-06 05:52:36.000000 zope.interface-6.1a1/src/zope.interface.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-04-06 05:52:36.000000 zope.interface-6.1a1/src/zope.interface.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2023-04-06 05:52:36.000000 zope.interface-6.1a1/src/zope.interface.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-04-06 05:52:36.000000 zope.interface-6.1a1/src/zope.interface.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      153 2023-04-06 05:52:36.000000 zope.interface-6.1a1/src/zope.interface.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2023-04-06 05:52:36.000000 zope.interface-6.1a1/src/zope.interface.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1430 2023-04-06 05:52:35.000000 zope.interface-6.1a1/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.826079 zope.interface-6.1a2/
+-rw-r--r--   0 mac        (513) staff       (20)      588 2023-04-13 06:24:12.000000 zope.interface-6.1a2/.coveragerc
+-rwxr-xr-x   0 mac        (513) staff       (20)     2183 2023-04-13 06:24:12.000000 zope.interface-6.1a2/.manylinux-install.sh
+-rwxr-xr-x   0 mac        (513) staff       (20)      509 2023-04-13 06:24:12.000000 zope.interface-6.1a2/.manylinux.sh
+-rw-r--r--   0 mac        (513) staff       (20)    38648 2023-04-13 06:24:12.000000 zope.interface-6.1a2/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      799 2023-04-13 06:24:12.000000 zope.interface-6.1a2/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-04-13 06:24:12.000000 zope.interface-6.1a2/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-04-13 06:24:12.000000 zope.interface-6.1a2/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      564 2023-04-13 06:24:12.000000 zope.interface-6.1a2/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)    41194 2023-04-13 06:24:13.826254 zope.interface-6.1a2/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1353 2023-04-13 06:24:12.000000 zope.interface-6.1a2/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)     1949 2023-04-13 06:24:12.000000 zope.interface-6.1a2/appveyor.yml
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.794986 zope.interface-6.1a2/benchmarks/
+-rw-r--r--   0 mac        (513) staff       (20)     8497 2023-04-13 06:24:12.000000 zope.interface-6.1a2/benchmarks/micro.py
+-rw-r--r--   0 mac        (513) staff       (20)      838 2023-04-13 06:24:12.000000 zope.interface-6.1a2/build.cmd
+-rw-r--r--   0 mac        (513) staff       (20)      215 2023-04-13 06:24:12.000000 zope.interface-6.1a2/buildout.cfg
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.800061 zope.interface-6.1a2/docs/
+-rw-r--r--   0 mac        (513) staff       (20)     5592 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/Makefile
+-rw-r--r--   0 mac        (513) staff       (20)    41051 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)    33998 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/README.ru.rst
+-rw-r--r--   0 mac        (513) staff       (20)    18817 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/adapter.rst
+-rw-r--r--   0 mac        (513) staff       (20)    21169 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/adapter.ru.rst
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.803496 zope.interface-6.1a2/docs/api/
+-rw-r--r--   0 mac        (513) staff       (20)      691 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/api/adapters.rst
+-rw-r--r--   0 mac        (513) staff       (20)     1283 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/api/common.rst
+-rw-r--r--   0 mac        (513) staff       (20)     2465 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/api/components.rst
+-rw-r--r--   0 mac        (513) staff       (20)    21746 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/api/declarations.rst
+-rw-r--r--   0 mac        (513) staff       (20)      165 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/api/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)      687 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/api/ro.rst
+-rw-r--r--   0 mac        (513) staff       (20)     9948 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/api/specifications.rst
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/changes.rst
+-rw-r--r--   0 mac        (513) staff       (20)     9081 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/conf.py
+-rw-r--r--   0 mac        (513) staff       (20)     1742 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/foodforthought.rst
+-rw-r--r--   0 mac        (513) staff       (20)     9509 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/hacking.rst
+-rw-r--r--   0 mac        (513) staff       (20)     6537 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/human.rst
+-rw-r--r--   0 mac        (513) staff       (20)    10681 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/human.ru.rst
+-rw-r--r--   0 mac        (513) staff       (20)      639 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)     5110 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/make.bat
+-rw-r--r--   0 mac        (513) staff       (20)    10222 2023-04-13 06:24:12.000000 zope.interface-6.1a2/docs/verify.rst
+-rw-r--r--   0 mac        (513) staff       (20)      286 2023-04-13 06:24:12.000000 zope.interface-6.1a2/rtd.txt
+-rw-r--r--   0 mac        (513) staff       (20)      604 2023-04-13 06:24:13.826903 zope.interface-6.1a2/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     4885 2023-04-13 06:24:12.000000 zope.interface-6.1a2/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.788312 zope.interface-6.1a2/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.803831 zope.interface-6.1a2/src/zope/
+-rw-r--r--   0 mac        (513) staff       (20)       56 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.811390 zope.interface-6.1a2/src/zope/interface/
+-rw-r--r--   0 mac        (513) staff       (20)     3463 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     4369 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/_compat.py
+-rw-r--r--   0 mac        (513) staff       (20)     1056 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/_flatten.py
+-rw-r--r--   0 mac        (513) staff       (20)    57678 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/_zope_interface_coptimizations.c
+-rw-r--r--   0 mac        (513) staff       (20)    36218 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/adapter.py
+-rw-r--r--   0 mac        (513) staff       (20)     3890 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/advice.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.814552 zope.interface-6.1a2/src/zope/interface/common/
+-rw-r--r--   0 mac        (513) staff       (20)    10461 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     3027 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/builtins.py
+-rw-r--r--   0 mac        (513) staff       (20)     6792 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/collections.py
+-rw-r--r--   0 mac        (513) staff       (20)    20858 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/idatetime.py
+-rw-r--r--   0 mac        (513) staff       (20)     5367 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)     1241 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/io.py
+-rw-r--r--   0 mac        (513) staff       (20)     4677 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/mapping.py
+-rw-r--r--   0 mac        (513) staff       (20)     1682 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/numbers.py
+-rw-r--r--   0 mac        (513) staff       (20)     5525 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/sequence.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.817204 zope.interface-6.1a2/src/zope/interface/common/tests/
+-rw-r--r--   0 mac        (513) staff       (20)     5310 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     3906 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/basemapping.py
+-rw-r--r--   0 mac        (513) staff       (20)     1345 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/test_builtins.py
+-rw-r--r--   0 mac        (513) staff       (20)     5724 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/test_collections.py
+-rw-r--r--   0 mac        (513) staff       (20)     1594 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/test_idatetime.py
+-rw-r--r--   0 mac        (513) staff       (20)      812 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/test_import_interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)     1597 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/test_io.py
+-rw-r--r--   0 mac        (513) staff       (20)     1394 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/common/tests/test_numbers.py
+-rw-r--r--   0 mac        (513) staff       (20)    42843 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/declarations.py
+-rw-r--r--   0 mac        (513) staff       (20)     4067 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/document.py
+-rw-r--r--   0 mac        (513) staff       (20)     8635 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/exceptions.py
+-rw-r--r--   0 mac        (513) staff       (20)    38825 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/interface.py
+-rw-r--r--   0 mac        (513) staff       (20)    50125 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)    25828 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/registry.py
+-rw-r--r--   0 mac        (513) staff       (20)    24155 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/ro.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.825739 zope.interface-6.1a2/src/zope/interface/tests/
+-rw-r--r--   0 mac        (513) staff       (20)     3961 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      897 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/tests/advisory_testing.py
+-rw-r--r--   0 mac        (513) staff       (20)      911 2023-04-13 06:24:12.000000 zope.interface-6.1a2/src/zope/interface/tests/dummy.py
+-rw-r--r--   0 mac        (513) staff       (20)      889 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/idummy.py
+-rw-r--r--   0 mac        (513) staff       (20)      812 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/m1.py
+-rw-r--r--   0 mac        (513) staff       (20)     3015 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/odd.py
+-rw-r--r--   0 mac        (513) staff       (20)    79548 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_adapter.py
+-rw-r--r--   0 mac        (513) staff       (20)     5962 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_advice.py
+-rw-r--r--   0 mac        (513) staff       (20)     1290 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_compile_flags.py
+-rw-r--r--   0 mac        (513) staff       (20)    82128 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_declarations.py
+-rw-r--r--   0 mac        (513) staff       (20)    16899 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_document.py
+-rw-r--r--   0 mac        (513) staff       (20)     1118 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_element.py
+-rw-r--r--   0 mac        (513) staff       (20)     6411 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_exceptions.py
+-rw-r--r--   0 mac        (513) staff       (20)    91465 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_interface.py
+-rw-r--r--   0 mac        (513) staff       (20)     4377 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)     7565 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_odd_declarations.py
+-rw-r--r--   0 mac        (513) staff       (20)   112819 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_registry.py
+-rw-r--r--   0 mac        (513) staff       (20)    14121 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_ro.py
+-rw-r--r--   0 mac        (513) staff       (20)     1933 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_sorting.py
+-rw-r--r--   0 mac        (513) staff       (20)    19190 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/tests/test_verify.py
+-rw-r--r--   0 mac        (513) staff       (20)     7154 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope/interface/verify.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-04-13 06:24:13.806270 zope.interface-6.1a2/src/zope.interface.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)    41194 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope.interface.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     2921 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope.interface.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope.interface.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope.interface.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope.interface.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      153 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope.interface.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-04-13 06:24:13.000000 zope.interface-6.1a2/src/zope.interface.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1430 2023-04-13 06:24:13.000000 zope.interface-6.1a2/tox.ini
```

### Comparing `zope.interface-6.1a1/.coveragerc` & `zope.interface-6.1a2/.coveragerc`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/.manylinux-install.sh` & `zope.interface-6.1a2/.manylinux-install.sh`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/CHANGES.rst` & `zope.interface-6.1a2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
  Changes
 =========
 
+6.1a2 (2023-04-13)
+==================
+
+- Fix building of the docs for non-final versions.
+
+
 6.1a1 (2023-04-06)
 ==================
 
 - Add support for building ppc64le wheels.
 
 
 6.0 (2023-03-17)
```

### Comparing `zope.interface-6.1a1/CONTRIBUTING.md` & `zope.interface-6.1a2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/LICENSE.txt` & `zope.interface-6.1a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/MANIFEST.in` & `zope.interface-6.1a2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/PKG-INFO` & `zope.interface-6.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.interface
-Version: 6.1a1
+Version: 6.1a2
 Summary: Interfaces for Python
 Home-page: https://github.com/zopefoundation/zope.interface
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: interface,components,plugins
 Classifier: Development Status :: 5 - Production/Stable
@@ -60,14 +60,20 @@
 
 For detailed documentation, please see https://zopeinterface.readthedocs.io/en/latest/
 
 =========
  Changes
 =========
 
+6.1a2 (2023-04-13)
+==================
+
+- Fix building of the docs for non-final versions.
+
+
 6.1a1 (2023-04-06)
 ==================
 
 - Add support for building ppc64le wheels.
 
 
 6.0 (2023-03-17)
```

### Comparing `zope.interface-6.1a1/README.rst` & `zope.interface-6.1a2/README.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/appveyor.yml` & `zope.interface-6.1a2/appveyor.yml`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/benchmarks/micro.py` & `zope.interface-6.1a2/benchmarks/micro.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/build.cmd` & `zope.interface-6.1a2/build.cmd`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/Makefile` & `zope.interface-6.1a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/README.rst` & `zope.interface-6.1a2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/README.ru.rst` & `zope.interface-6.1a2/docs/README.ru.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/adapter.rst` & `zope.interface-6.1a2/docs/adapter.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/adapter.ru.rst` & `zope.interface-6.1a2/docs/adapter.ru.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/api/adapters.rst` & `zope.interface-6.1a2/docs/api/adapters.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/api/common.rst` & `zope.interface-6.1a2/docs/api/common.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/api/components.rst` & `zope.interface-6.1a2/docs/api/components.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/api/declarations.rst` & `zope.interface-6.1a2/docs/api/declarations.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/api/ro.rst` & `zope.interface-6.1a2/docs/api/ro.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/api/specifications.rst` & `zope.interface-6.1a2/docs/api/specifications.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/conf.py` & `zope.interface-6.1a2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,22 +52,22 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'zope.interface'
-copyright = '2012-2017, Zope Foundation contributors'
+copyright = '2012-2023, Zope Foundation contributors'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '%s.%s' % tuple(map(int, rqmt.version.split('.')[:2]))
+version = '%s.%s' % tuple(rqmt.version.split('.')[:2])
 # The full version, including alpha/beta/rc tags.
 release = rqmt.version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
```

### Comparing `zope.interface-6.1a1/docs/foodforthought.rst` & `zope.interface-6.1a2/docs/foodforthought.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/hacking.rst` & `zope.interface-6.1a2/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/human.rst` & `zope.interface-6.1a2/docs/human.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/human.ru.rst` & `zope.interface-6.1a2/docs/human.ru.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/index.rst` & `zope.interface-6.1a2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/make.bat` & `zope.interface-6.1a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/docs/verify.rst` & `zope.interface-6.1a2/docs/verify.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/setup.cfg` & `zope.interface-6.1a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/setup.py` & `zope.interface-6.1a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 long_description = (
         read('README.rst')
         + '\n' +
         read('CHANGES.rst')
         )
 
 setup(name='zope.interface',
-      version='6.1a1',
+      version='6.1a2',
       url='https://github.com/zopefoundation/zope.interface',
       license='ZPL 2.1',
       description='Interfaces for Python',
       author='Zope Foundation and Contributors',
       author_email='zope-dev@zope.org',
       long_description=long_description,
       classifiers=[
```

### Comparing `zope.interface-6.1a1/src/zope/interface/__init__.py` & `zope.interface-6.1a2/src/zope/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/_compat.py` & `zope.interface-6.1a2/src/zope/interface/_compat.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/_flatten.py` & `zope.interface-6.1a2/src/zope/interface/_flatten.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/_zope_interface_coptimizations.c` & `zope.interface-6.1a2/src/zope/interface/_zope_interface_coptimizations.c`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/adapter.py` & `zope.interface-6.1a2/src/zope/interface/adapter.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/advice.py` & `zope.interface-6.1a2/src/zope/interface/advice.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/__init__.py` & `zope.interface-6.1a2/src/zope/interface/common/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/builtins.py` & `zope.interface-6.1a2/src/zope/interface/common/builtins.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/collections.py` & `zope.interface-6.1a2/src/zope/interface/common/collections.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/idatetime.py` & `zope.interface-6.1a2/src/zope/interface/common/idatetime.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/interfaces.py` & `zope.interface-6.1a2/src/zope/interface/common/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/io.py` & `zope.interface-6.1a2/src/zope/interface/common/io.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/mapping.py` & `zope.interface-6.1a2/src/zope/interface/common/mapping.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/numbers.py` & `zope.interface-6.1a2/src/zope/interface/common/numbers.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/sequence.py` & `zope.interface-6.1a2/src/zope/interface/common/sequence.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/tests/__init__.py` & `zope.interface-6.1a2/src/zope/interface/common/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/tests/basemapping.py` & `zope.interface-6.1a2/src/zope/interface/common/tests/basemapping.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/tests/test_builtins.py` & `zope.interface-6.1a2/src/zope/interface/common/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/tests/test_collections.py` & `zope.interface-6.1a2/src/zope/interface/common/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/tests/test_idatetime.py` & `zope.interface-6.1a2/src/zope/interface/common/tests/test_idatetime.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/tests/test_import_interfaces.py` & `zope.interface-6.1a2/src/zope/interface/common/tests/test_import_interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/tests/test_io.py` & `zope.interface-6.1a2/src/zope/interface/common/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/common/tests/test_numbers.py` & `zope.interface-6.1a2/src/zope/interface/common/tests/test_numbers.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/declarations.py` & `zope.interface-6.1a2/src/zope/interface/declarations.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/document.py` & `zope.interface-6.1a2/src/zope/interface/document.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/exceptions.py` & `zope.interface-6.1a2/src/zope/interface/exceptions.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/interface.py` & `zope.interface-6.1a2/src/zope/interface/interface.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/interfaces.py` & `zope.interface-6.1a2/src/zope/interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/registry.py` & `zope.interface-6.1a2/src/zope/interface/registry.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/ro.py` & `zope.interface-6.1a2/src/zope/interface/ro.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/__init__.py` & `zope.interface-6.1a2/src/zope/interface/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/advisory_testing.py` & `zope.interface-6.1a2/src/zope/interface/tests/advisory_testing.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/dummy.py` & `zope.interface-6.1a2/src/zope/interface/tests/dummy.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/idummy.py` & `zope.interface-6.1a2/src/zope/interface/tests/idummy.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/m1.py` & `zope.interface-6.1a2/src/zope/interface/tests/m1.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/odd.py` & `zope.interface-6.1a2/src/zope/interface/tests/odd.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/test_adapter.py` & `zope.interface-6.1a2/src/zope/interface/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/test_advice.py` & `zope.interface-6.1a2/src/zope/interface/tests/test_advice.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/test_compile_flags.py` & `zope.interface-6.1a2/src/zope/interface/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/test_declarations.py` & `zope.interface-6.1a2/src/zope/interface/tests/test_declarations.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/test_document.py` & `zope.interface-6.1a2/src/zope/interface/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/test_element.py` & `zope.interface-6.1a2/src/zope/interface/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/test_exceptions.py` & `zope.interface-6.1a2/src/zope/interface/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/test_interface.py` & `zope.interface-6.1a2/src/zope/interface/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/test_interfaces.py` & `zope.interface-6.1a2/src/zope/interface/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/test_odd_declarations.py` & `zope.interface-6.1a2/src/zope/interface/tests/test_odd_declarations.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/test_registry.py` & `zope.interface-6.1a2/src/zope/interface/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/test_ro.py` & `zope.interface-6.1a2/src/zope/interface/tests/test_ro.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/test_sorting.py` & `zope.interface-6.1a2/src/zope/interface/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/tests/test_verify.py` & `zope.interface-6.1a2/src/zope/interface/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope/interface/verify.py` & `zope.interface-6.1a2/src/zope/interface/verify.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/src/zope.interface.egg-info/PKG-INFO` & `zope.interface-6.1a2/src/zope.interface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.interface
-Version: 6.1a1
+Version: 6.1a2
 Summary: Interfaces for Python
 Home-page: https://github.com/zopefoundation/zope.interface
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: interface,components,plugins
 Classifier: Development Status :: 5 - Production/Stable
@@ -60,14 +60,20 @@
 
 For detailed documentation, please see https://zopeinterface.readthedocs.io/en/latest/
 
 =========
  Changes
 =========
 
+6.1a2 (2023-04-13)
+==================
+
+- Fix building of the docs for non-final versions.
+
+
 6.1a1 (2023-04-06)
 ==================
 
 - Add support for building ppc64le wheels.
 
 
 6.0 (2023-03-17)
```

### Comparing `zope.interface-6.1a1/src/zope.interface.egg-info/SOURCES.txt` & `zope.interface-6.1a2/src/zope.interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.1a1/tox.ini` & `zope.interface-6.1a2/tox.ini`

 * *Files identical despite different names*

