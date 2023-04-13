# Comparing `tmp/pikepdf-7.1.2.tar.gz` & `tmp/pikepdf-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikepdf-7.1.2.tar", last modified: Sat Mar 25 20:26:12 2023, max compression
+gzip compressed data, was "pikepdf-7.2.0.tar", last modified: Thu Apr 13 06:58:17 2023, max compression
```

## Comparing `pikepdf-7.1.2.tar` & `pikepdf-7.2.0.tar`

### file list

```diff
@@ -1,230 +1,231 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.489654 pikepdf-7.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-03-25 20:23:41.000000 pikepdf-7.1.2/.clang-format
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-03-25 20:23:41.000000 pikepdf-7.1.2/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-03-25 20:23:41.000000 pikepdf-7.1.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.461654 pikepdf-7.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-03-25 20:23:41.000000 pikepdf-7.1.2/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-03-25 20:23:41.000000 pikepdf-7.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.461654 pikepdf-7.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     8461 2023-03-25 20:23:41.000000 pikepdf-7.1.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-03-25 20:23:41.000000 pikepdf-7.1.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)      368 2023-03-25 20:23:41.000000 pikepdf-7.1.2/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-03-25 20:23:41.000000 pikepdf-7.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-03-25 20:23:41.000000 pikepdf-7.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-03-25 20:23:41.000000 pikepdf-7.1.2/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.461654 pikepdf-7.1.2/.reuse/
--rw-r--r--   0 runner    (1001) docker     (122)     4608 2023-03-25 20:23:41.000000 pikepdf-7.1.2/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (122)    16725 2023-03-25 20:23:41.000000 pikepdf-7.1.2/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.465654 pikepdf-7.1.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-03-25 20:23:41.000000 pikepdf-7.1.2/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    17023 2023-03-25 20:23:41.000000 pikepdf-7.1.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    12523 2023-03-25 20:23:41.000000 pikepdf-7.1.2/LICENSES/CC-BY-SA-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    14122 2023-03-25 20:23:41.000000 pikepdf-7.1.2/LICENSES/CC-BY-SA-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    14331 2023-03-25 20:23:41.000000 pikepdf-7.1.2/LICENSES/CC-BY-SA-2.5.txt
--rw-r--r--   0 runner    (1001) docker     (122)    21305 2023-03-25 20:23:41.000000 pikepdf-7.1.2/LICENSES/CC-BY-SA-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    18375 2023-03-25 20:23:41.000000 pikepdf-7.1.2/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7048 2023-03-25 20:23:41.000000 pikepdf-7.1.2/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    21097 2023-03-25 20:23:41.000000 pikepdf-7.1.2/LICENSES/CECILL-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    20272 2023-03-25 20:23:41.000000 pikepdf-7.1.2/LICENSES/GFDL-1.2-or-later.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-03-25 20:23:41.000000 pikepdf-7.1.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)    16727 2023-03-25 20:23:41.000000 pikepdf-7.1.2/LICENSES/MPL-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-03-25 20:23:41.000000 pikepdf-7.1.2/LICENSES/Zlib.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4662 2023-03-25 20:23:41.000000 pikepdf-7.1.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     7150 2023-03-25 20:26:12.485654 pikepdf-7.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6034 2023-03-25 20:23:41.000000 pikepdf-7.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.465654 pikepdf-7.1.2/build-scripts/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-03-25 20:23:41.000000 pikepdf-7.1.2/build-scripts/environ-from-pyproject.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      382 2023-03-25 20:23:41.000000 pikepdf-7.1.2/build-scripts/linux-build-sdist-deps.bash
--rwxr-xr-x   0 runner    (1001) docker     (122)      482 2023-03-25 20:23:41.000000 pikepdf-7.1.2/build-scripts/linux-build-wheel-deps.bash
--rwxr-xr-x   0 runner    (1001) docker     (122)      225 2023-03-25 20:23:41.000000 pikepdf-7.1.2/build-scripts/linux-download-qpdf.bash
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-03-25 20:23:41.000000 pikepdf-7.1.2/build-scripts/linux-install-libxmp.bash
--rw-r--r--   0 runner    (1001) docker     (122)      620 2023-03-25 20:23:41.000000 pikepdf-7.1.2/build-scripts/win-download-qpdf.ps1
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.465654 pikepdf-7.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7687 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.465654 pikepdf-7.1.2/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/_ext/fix_pybind11_autodoc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.465654 pikepdf-7.1.2/docs/_notebooks/
--rw-r--r--   0 runner    (1001) docker     (122)     6560 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/_notebooks/pages.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.465654 pikepdf-7.1.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/api/filters.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/api/main.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8520 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/api/models.rst
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/api/settings.rst
--rw-r--r--   0 runner    (1001) docker     (122)      528 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/binary-wheels.csv
--rw-r--r--   0 runner    (1001) docker     (122)    12111 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.469654 pikepdf-7.1.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (122)   543264 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/images/28fish.jpg
--rw-r--r--   0 runner    (1001) docker     (122)     8489 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/images/acrobat-attachments.png
--rw-r--r--   0 runner    (1001) docker     (122)    26172 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/images/congress_im0.jpg
--rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/images/pdfcoords.svg
--rw-r--r--   0 runner    (1001) docker     (122)   148388 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/images/pike-cartoon.png
--rw-r--r--   0 runner    (1001) docker     (122)    88609 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/images/pike-release.jpg
--rw-r--r--   0 runner    (1001) docker     (122)    32321 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/images/pike.png
--rw-r--r--   0 runner    (1001) docker     (122)    29276 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/images/pikemen.jpg
--rw-r--r--   0 runner    (1001) docker     (122)    65692 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/images/save-pike.jpg
--rw-r--r--   0 runner    (1001) docker     (122)   155993 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/images/sushi.jpg
--rw-r--r--   0 runner    (1001) docker     (122)     5602 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10090 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7265 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.469654 pikepdf-7.1.2/docs/references/
--rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/references/arch.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/references/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/references/debugging.rst
--rw-r--r--   0 runner    (1001) docker     (122)      788 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/references/resources.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.469654 pikepdf-7.1.2/docs/releasenotes/
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/releasenotes/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/releasenotes/version0.rst
--rw-r--r--   0 runner    (1001) docker     (122)    17003 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/releasenotes/version1.rst
--rw-r--r--   0 runner    (1001) docker     (122)    13480 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/releasenotes/version2.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3972 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/releasenotes/version3.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/releasenotes/version4.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4745 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/releasenotes/version5.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/releasenotes/version6.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/releasenotes/version7.rst
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.469654 pikepdf-7.1.2/docs/topics/
--rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/topics/attachments.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7605 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/topics/content_streams.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2730 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/topics/encoding.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6010 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/topics/images.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6187 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/topics/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/topics/nametrees.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5525 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/topics/objects.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/topics/outlines.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2661 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/topics/overlays.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1963 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/topics/page.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/topics/pagelayout.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8077 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/topics/pages.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/topics/security.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3409 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/topics/streams.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8468 2023-03-25 20:23:41.000000 pikepdf-7.1.2/docs/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.469654 pikepdf-7.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-03-25 20:23:41.000000 pikepdf-7.1.2/examples/find_links.py
--rw-r--r--   0 runner    (1001) docker     (122)    38728 2023-03-25 20:23:41.000000 pikepdf-7.1.2/licenses-for-wheels.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5912 2023-03-25 20:23:41.000000 pikepdf-7.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-25 20:26:12.489654 pikepdf-7.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3848 2023-03-25 20:23:41.000000 pikepdf-7.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.461654 pikepdf-7.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.473654 pikepdf-7.1.2/src/core/
--rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/annotation.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7216 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/embeddedfiles.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/gsl.h
--rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/jbig2-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)     5398 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/job.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/logger.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/mmap_inputsource-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/nametree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/numbertree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    42088 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/object.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/object_convert.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8731 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/object_repr.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    14258 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/page.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    11199 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/parsers.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/parsers.h
--rw-r--r--   0 runner    (1001) docker     (122)     8201 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/pikepdf.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/pikepdf.h
--rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/pipeline.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/pipeline.h
--rw-r--r--   0 runner    (1001) docker     (122)    38829 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/qpdf.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/qpdf_inputsource-inl.h
--rw-r--r--   0 runner    (1001) docker     (122)    13658 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/qpdf_pagelist.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/qpdf_pagelist.h
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/rectangle.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/tokenfilter.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/core/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.477654 pikepdf-7.1.2/src/pikepdf/
--rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6161 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/_augments.py
--rw-r--r--   0 runner    (1001) docker     (122)    25634 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/_core.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/_cpphelpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    54692 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/_qpdf.py
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      879 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/_xml.py
--rw-r--r--   0 runner    (1001) docker     (122)     5952 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/codec.py
--rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/jbig2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.477654 pikepdf-7.1.2/src/pikepdf/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/models/_content_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     8204 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/models/_transcoding.py
--rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/models/encryption.py
--rw-r--r--   0 runner    (1001) docker     (122)    36142 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/models/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     4484 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/models/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    31934 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    14786 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/models/outlines.py
--rw-r--r--   0 runner    (1001) docker     (122)    10415 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-03-25 20:23:41.000000 pikepdf-7.1.2/src/pikepdf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.477654 pikepdf-7.1.2/src/pikepdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7150 2023-03-25 20:26:12.000000 pikepdf-7.1.2/src/pikepdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-03-25 20:26:12.000000 pikepdf-7.1.2/src/pikepdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-25 20:26:12.000000 pikepdf-7.1.2/src/pikepdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-03-25 20:26:12.000000 pikepdf-7.1.2/src/pikepdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-03-25 20:26:12.000000 pikepdf-7.1.2/src/pikepdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.481654 pikepdf-7.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1731 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 20:26:12.485654 pikepdf-7.1.2/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (122)     5661 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/1biticc.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      420 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/Gray.icc
--rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/aquamarine-cie.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/aquamarine-cie.png
--rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/cmyk-jpeg.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    97969 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/congress-gray.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   193947 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/congress.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2889 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/content-stream-errors.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/form.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/formxobject.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/fourpages.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   296661 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/graph-encrypted.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   296322 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/graph.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/image-mono-inline.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/invalid_creationdate.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    20306 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/jbig2.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    60332 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/jbig2global.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/outlines.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      931 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/pal-1bit-rgb.pdf
--rw-r--r--   0 runner    (1001) docker     (122)      931 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/pal-1bit-trivial.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/pal.pdf
--rwxr-xr-x   0 runner    (1001) docker     (122)   533953 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/pdfx.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    18471 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/pike-flate-jp2.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    18152 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/pike-jp2.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/pink-palette-icc.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/pink-palette-icc.png
--rw-r--r--   0 runner    (1001) docker     (122)     5432 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/rle.pdf
--rw-r--r--   0 runner    (1001) docker     (122)   115546 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/sandwich.pdf
--rw-r--r--   0 runner    (1001) docker     (122)    10049 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_attachments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_augments.py
--rw-r--r--   0 runner    (1001) docker     (122)     4516 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_decimal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     3404 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_foreign.py
--rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_formxobject.py
--rw-r--r--   0 runner    (1001) docker     (122)    35498 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_image_access.py
--rw-r--r--   0 runner    (1001) docker     (122)     8880 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_ipython.py
--rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    25215 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_nametree.py
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_numbertree.py
--rw-r--r--   0 runner    (1001) docker     (122)    24622 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_object.py
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_objectlist.py
--rw-r--r--   0 runner    (1001) docker     (122)    17256 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_outlines.py
--rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (122)    15569 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_pages.py
--rw-r--r--   0 runner    (1001) docker     (122)     9522 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)    13688 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_pdfa.py
--rw-r--r--   0 runner    (1001) docker     (122)      754 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_private_pdfs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_refcount.py
--rw-r--r--   0 runner    (1001) docker     (122)     4682 2023-03-25 20:23:41.000000 pikepdf-7.1.2/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.790136 pikepdf-7.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.758135 pikepdf-7.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.762135 pikepdf-7.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     8461 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.762135 pikepdf-7.2.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (122)     4608 2023-04-13 06:55:41.000000 pikepdf-7.2.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (122)    16725 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.762135 pikepdf-7.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    17023 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    12523 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CC-BY-SA-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14122 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CC-BY-SA-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14331 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CC-BY-SA-2.5.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    21305 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CC-BY-SA-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    18375 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7048 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    21097 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/CECILL-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    20272 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/GFDL-1.2-or-later.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    16727 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-04-13 06:55:41.000000 pikepdf-7.2.0/LICENSES/Zlib.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4662 2023-04-13 06:55:41.000000 pikepdf-7.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     7150 2023-04-13 06:58:17.786136 pikepdf-7.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6034 2023-04-13 06:55:41.000000 pikepdf-7.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.762135 pikepdf-7.2.0/build-scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-13 06:55:41.000000 pikepdf-7.2.0/build-scripts/environ-from-pyproject.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      382 2023-04-13 06:55:41.000000 pikepdf-7.2.0/build-scripts/linux-build-sdist-deps.bash
+-rwxr-xr-x   0 runner    (1001) docker     (122)      482 2023-04-13 06:55:41.000000 pikepdf-7.2.0/build-scripts/linux-build-wheel-deps.bash
+-rwxr-xr-x   0 runner    (1001) docker     (122)      225 2023-04-13 06:55:41.000000 pikepdf-7.2.0/build-scripts/linux-download-qpdf.bash
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-13 06:55:41.000000 pikepdf-7.2.0/build-scripts/linux-install-libxmp.bash
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-04-13 06:55:41.000000 pikepdf-7.2.0/build-scripts/win-download-qpdf.ps1
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.762135 pikepdf-7.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7687 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.762135 pikepdf-7.2.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (122)     1477 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/_ext/fix_pybind11_autodoc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.762135 pikepdf-7.2.0/docs/_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (122)     6560 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/_notebooks/pages.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.766135 pikepdf-7.2.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/api/filters.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/api/main.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8520 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/api/models.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/api/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/binary-wheels.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    12349 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.766135 pikepdf-7.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (122)   543264 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/28fish.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)     8489 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/acrobat-attachments.png
+-rw-r--r--   0 runner    (1001) docker     (122)    26172 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/congress_im0.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)     2983 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/pdfcoords.svg
+-rw-r--r--   0 runner    (1001) docker     (122)   148388 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/pike-cartoon.png
+-rw-r--r--   0 runner    (1001) docker     (122)    88609 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/pike-release.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)    32321 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/pike.png
+-rw-r--r--   0 runner    (1001) docker     (122)    29276 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/pikemen.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)    65692 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/save-pike.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)   155993 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/images/sushi.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)     5602 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10090 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7265 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.766135 pikepdf-7.2.0/docs/references/
+-rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/references/arch.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/references/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4513 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/references/debugging.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/references/resources.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.770135 pikepdf-7.2.0/docs/releasenotes/
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    17003 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    13480 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3972 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version3.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version4.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4745 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version5.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version6.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3272 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/releasenotes/version7.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.770135 pikepdf-7.2.0/docs/topics/
+-rw-r--r--   0 runner    (1001) docker     (122)     3429 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/attachments.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7605 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/content_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2730 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/encoding.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6010 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/images.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6187 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/nametrees.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5525 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/objects.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/outlines.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2661 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/overlays.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1963 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/page.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1887 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/pagelayout.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8077 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/pages.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2689 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/security.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3409 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/topics/streams.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8468 2023-04-13 06:55:41.000000 pikepdf-7.2.0/docs/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.770135 pikepdf-7.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-04-13 06:55:41.000000 pikepdf-7.2.0/examples/find_links.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38728 2023-04-13 06:55:41.000000 pikepdf-7.2.0/licenses-for-wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5912 2023-04-13 06:55:41.000000 pikepdf-7.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 06:58:17.790136 pikepdf-7.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3848 2023-04-13 06:55:41.000000 pikepdf-7.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.758135 pikepdf-7.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.774135 pikepdf-7.2.0/src/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/annotation.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7216 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/embeddedfiles.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/gsl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/jbig2-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5398 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/job.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/logger.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/mmap_inputsource-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3621 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/nametree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3001 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/numbertree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    42088 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/object.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/object_convert.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10354 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/object_repr.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14258 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/page.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11199 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/parsers.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/parsers.h
+-rw-r--r--   0 runner    (1001) docker     (122)     8201 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/pikepdf.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/pikepdf.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1274 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/pipeline.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/pipeline.h
+-rw-r--r--   0 runner    (1001) docker     (122)    39387 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/qpdf.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/qpdf_inputsource-inl.h
+-rw-r--r--   0 runner    (1001) docker     (122)    15512 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/qpdf_pagelist.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/qpdf_pagelist.h
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/rectangle.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5455 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/tokenfilter.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/core/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.774135 pikepdf-7.2.0/src/pikepdf/
+-rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6161 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_augments.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25624 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_core.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_cpphelpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    54692 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_qpdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      879 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/_xml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5952 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/codec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3378 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/jbig2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.778135 pikepdf-7.2.0/src/pikepdf/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1139 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/_content_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8204 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/_transcoding.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36142 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5979 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31934 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14786 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/models/outlines.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10415 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-04-13 06:55:41.000000 pikepdf-7.2.0/src/pikepdf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.778135 pikepdf-7.2.0/src/pikepdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7150 2023-04-13 06:58:17.000000 pikepdf-7.2.0/src/pikepdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5304 2023-04-13 06:58:17.000000 pikepdf-7.2.0/src/pikepdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 06:58:17.000000 pikepdf-7.2.0/src/pikepdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-04-13 06:58:17.000000 pikepdf-7.2.0/src/pikepdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-13 06:58:17.000000 pikepdf-7.2.0/src/pikepdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.782136 pikepdf-7.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1731 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:58:17.786136 pikepdf-7.2.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)     5661 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/1biticc.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      420 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/Gray.icc
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/aquamarine-cie.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/aquamarine-cie.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1461 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/cmyk-jpeg.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    97969 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/congress-gray.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)   193947 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/congress.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2889 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/content-stream-errors.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    10876 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/form.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/formxobject.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/fourpages.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)   296661 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/graph-encrypted.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)   296322 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/graph.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/image-mono-inline.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/invalid_creationdate.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    20306 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/jbig2.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    60332 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/jbig2global.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     6994 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/outlines.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      931 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pal-1bit-rgb.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      931 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pal-1bit-trivial.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pal.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (122)   533953 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pdfx.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    18471 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pike-flate-jp2.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    18152 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pike-jp2.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2681 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pink-palette-icc.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/pink-palette-icc.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5432 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/rle.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)   115546 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/sandwich.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)    10049 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_augments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4516 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5610 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3404 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_foreign.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_formxobject.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35498 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_image_access.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8880 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_ipython.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25215 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_nametree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_numbertree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22294 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_objectlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17256 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_outlines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15569 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_pages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9522 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13688 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_pdfa.py
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_private_pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_refcount.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3642 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4682 2023-04-13 06:55:41.000000 pikepdf-7.2.0/tests/test_sanity.py
```

### Comparing `pikepdf-7.1.2/.clang-format` & `pikepdf-7.2.0/.clang-format`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/.github/FUNDING.yml` & `pikepdf-7.2.0/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/.github/workflows/build.yml` & `pikepdf-7.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/.github/workflows/codeql-analysis.yml` & `pikepdf-7.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/.pre-commit-config.yaml` & `pikepdf-7.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/.readthedocs.yaml` & `pikepdf-7.2.0/.readthedocs.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 
 # Optionally build your docs in additional formats such as PDF
 formats:
   - pdf
 
 # Optionally set the version of Python and requirements required to build your docs
 build:
-  os: ubuntu-20.04
+  os: ubuntu-22.04
   tools:
-    python: "3.9"
+    python: "3.11"
 
 python:
   install:
     - requirements: docs/requirements.txt
```

### Comparing `pikepdf-7.1.2/.reuse/dep5` & `pikepdf-7.2.0/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/LICENSE.txt` & `pikepdf-7.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/LICENSES/Apache-2.0.txt` & `pikepdf-7.2.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/LICENSES/CC-BY-4.0.txt` & `pikepdf-7.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/LICENSES/CC-BY-SA-1.0.txt` & `pikepdf-7.2.0/LICENSES/CC-BY-SA-1.0.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/LICENSES/CC-BY-SA-2.0.txt` & `pikepdf-7.2.0/LICENSES/CC-BY-SA-2.0.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/LICENSES/CC-BY-SA-2.5.txt` & `pikepdf-7.2.0/LICENSES/CC-BY-SA-2.5.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/LICENSES/CC-BY-SA-3.0.txt` & `pikepdf-7.2.0/LICENSES/CC-BY-SA-3.0.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/LICENSES/CC-BY-SA-4.0.txt` & `pikepdf-7.2.0/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/LICENSES/CC0-1.0.txt` & `pikepdf-7.2.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/LICENSES/CECILL-2.0.txt` & `pikepdf-7.2.0/LICENSES/CECILL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/LICENSES/GFDL-1.2-or-later.txt` & `pikepdf-7.2.0/LICENSES/GFDL-1.2-or-later.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/LICENSES/MIT.txt` & `pikepdf-7.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/LICENSES/MPL-2.0.txt` & `pikepdf-7.2.0/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/LICENSES/Zlib.txt` & `pikepdf-7.2.0/LICENSES/Zlib.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/Makefile` & `pikepdf-7.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/PKG-INFO` & `pikepdf-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikepdf
-Version: 7.1.2
+Version: 7.2.0
 Summary: Read and write PDFs with Python, powered by qpdf
 Author-email: "James R. Barlow" <james@purplerock.ca>
 License: MPL-2.0
 Project-URL: documentation, https://pikepdf.readthedocs.io/
 Project-URL: repository, https://github.com/pikepdf/pikepdf
 Project-URL: changelog, https://pikepdf.readthedocs.io/en/latest/releasenotes/index.html
 Keywords: PDF
```

### Comparing `pikepdf-7.1.2/README.md` & `pikepdf-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/build-scripts/win-download-qpdf.ps1` & `pikepdf-7.2.0/build-scripts/win-download-qpdf.ps1`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/Makefile` & `pikepdf-7.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/_ext/fix_pybind11_autodoc.py` & `pikepdf-7.2.0/docs/_ext/fix_pybind11_autodoc.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/_notebooks/pages.ipynb` & `pikepdf-7.2.0/docs/_notebooks/pages.ipynb`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/api/exceptions.rst` & `pikepdf-7.2.0/docs/api/exceptions.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/api/filters.rst` & `pikepdf-7.2.0/docs/api/filters.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/api/main.rst` & `pikepdf-7.2.0/docs/api/main.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/api/models.rst` & `pikepdf-7.2.0/docs/api/models.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/binary-wheels.csv` & `pikepdf-7.2.0/docs/binary-wheels.csv`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/conf.py` & `pikepdf-7.2.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from __future__ import annotations
 
 import io
 import os
 import subprocess
 import sys
+import time
 from pathlib import Path
 
 try:
     import tomllib
 except ModuleNotFoundError:
     import tomli as tomllib  # type: ignore
 
@@ -56,19 +57,27 @@
     g = github.Github()
 
     runs = (
         g.get_repo('pikepdf/pikepdf').get_workflow('build.yml').get_runs(branch=branch)
     )
     artifacts_url = next(r for r in runs if r.head_sha == head_sha).artifacts_url
 
-    archive_download_url = next(
-        artifact
-        for artifact in requests.get(artifacts_url).json()['artifacts']
-        if artifact['name'] == 'rtd-wheel'
-    )['archive_download_url']
+    archive_download_url = ""
+    for i in range(5):
+        try:
+            archive_download_url = next(
+                artifact
+                for artifact in requests.get(artifacts_url).json()['artifacts']
+                if artifact['name'] == 'rtd-wheel'
+            )['archive_download_url']
+            break
+        except StopIteration:
+            if i == 4:
+                raise
+            time.sleep(15)
     artifact_bin = io.BytesIO(
         requests.get(
             archive_download_url,
             headers={'Authorization': f'token {github_token}'},
             stream=True,
         ).content
     )
```

### Comparing `pikepdf-7.1.2/docs/images/28fish.jpg` & `pikepdf-7.2.0/docs/images/28fish.jpg`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/images/acrobat-attachments.png` & `pikepdf-7.2.0/docs/images/acrobat-attachments.png`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/images/congress_im0.jpg` & `pikepdf-7.2.0/docs/images/congress_im0.jpg`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/images/pdfcoords.svg` & `pikepdf-7.2.0/docs/images/pdfcoords.svg`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/images/pike-cartoon.png` & `pikepdf-7.2.0/docs/images/pike-cartoon.png`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/images/pike-release.jpg` & `pikepdf-7.2.0/docs/images/pike-release.jpg`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/images/pike.png` & `pikepdf-7.2.0/docs/images/pike.png`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/images/pikemen.jpg` & `pikepdf-7.2.0/docs/images/pikemen.jpg`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/images/save-pike.jpg` & `pikepdf-7.2.0/docs/images/save-pike.jpg`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/images/sushi.jpg` & `pikepdf-7.2.0/docs/images/sushi.jpg`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/index.rst` & `pikepdf-7.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/installation.rst` & `pikepdf-7.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/make.bat` & `pikepdf-7.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/references/arch.rst` & `pikepdf-7.2.0/docs/references/arch.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/references/contributing.rst` & `pikepdf-7.2.0/docs/references/contributing.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/references/debugging.rst` & `pikepdf-7.2.0/docs/references/debugging.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/references/resources.rst` & `pikepdf-7.2.0/docs/references/resources.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/releasenotes/index.rst` & `pikepdf-7.2.0/docs/releasenotes/index.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/releasenotes/version0.rst` & `pikepdf-7.2.0/docs/releasenotes/version0.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/releasenotes/version1.rst` & `pikepdf-7.2.0/docs/releasenotes/version1.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/releasenotes/version2.rst` & `pikepdf-7.2.0/docs/releasenotes/version2.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/releasenotes/version3.rst` & `pikepdf-7.2.0/docs/releasenotes/version3.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/releasenotes/version4.rst` & `pikepdf-7.2.0/docs/releasenotes/version4.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/releasenotes/version5.rst` & `pikepdf-7.2.0/docs/releasenotes/version5.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/releasenotes/version6.rst` & `pikepdf-7.2.0/docs/releasenotes/version6.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/releasenotes/version7.rst` & `pikepdf-7.2.0/docs/releasenotes/version7.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v7.2.0
+======
+
+- Improved Object.repr() to avoid printing the entire contents of large object trees
+  such as those in PDFs with structural element trees.
+- Fixed typing of NumberTree.
+- Improved matrix documentation, interoperability with numpy, and added matrix inverse.
+- Documentation improvements.
+
 v7.1.2
 ======
 
 - Fixed possible segfault if a PDF is opened and accessed without being assigned to a
   variable. :issue:`465`
 
 v7.1.1
```

### Comparing `pikepdf-7.1.2/docs/topics/attachments.rst` & `pikepdf-7.2.0/docs/topics/attachments.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/topics/content_streams.rst` & `pikepdf-7.2.0/docs/topics/content_streams.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/topics/encoding.rst` & `pikepdf-7.2.0/docs/topics/encoding.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/topics/images.rst` & `pikepdf-7.2.0/docs/topics/images.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/topics/metadata.rst` & `pikepdf-7.2.0/docs/topics/metadata.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/topics/nametrees.rst` & `pikepdf-7.2.0/docs/topics/nametrees.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/topics/objects.rst` & `pikepdf-7.2.0/docs/topics/objects.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/topics/outlines.rst` & `pikepdf-7.2.0/docs/topics/outlines.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/topics/overlays.rst` & `pikepdf-7.2.0/docs/topics/overlays.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/topics/page.rst` & `pikepdf-7.2.0/docs/topics/page.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/topics/pagelayout.rst` & `pikepdf-7.2.0/docs/topics/pagelayout.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/topics/pages.rst` & `pikepdf-7.2.0/docs/topics/pages.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/topics/security.rst` & `pikepdf-7.2.0/docs/topics/security.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/topics/streams.rst` & `pikepdf-7.2.0/docs/topics/streams.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/docs/tutorial.rst` & `pikepdf-7.2.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/examples/find_links.py` & `pikepdf-7.2.0/examples/find_links.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/licenses-for-wheels.txt` & `pikepdf-7.2.0/licenses-for-wheels.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/pyproject.toml` & `pikepdf-7.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/setup.py` & `pikepdf-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/annotation.cpp` & `pikepdf-7.2.0/src/core/annotation.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/embeddedfiles.cpp` & `pikepdf-7.2.0/src/core/embeddedfiles.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/gsl.h` & `pikepdf-7.2.0/src/core/gsl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/jbig2-inl.h` & `pikepdf-7.2.0/src/core/jbig2-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/job.cpp` & `pikepdf-7.2.0/src/core/job.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/logger.cpp` & `pikepdf-7.2.0/src/core/logger.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/mmap_inputsource-inl.h` & `pikepdf-7.2.0/src/core/mmap_inputsource-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/nametree.cpp` & `pikepdf-7.2.0/src/core/nametree.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/numbertree.cpp` & `pikepdf-7.2.0/src/core/numbertree.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/object.cpp` & `pikepdf-7.2.0/src/core/object.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/object_convert.cpp` & `pikepdf-7.2.0/src/core/object_convert.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/object_repr.cpp` & `pikepdf-7.2.0/src/core/object_repr.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 #include <qpdf/Types.h>
 #include <qpdf/DLL.h>
 #include <qpdf/QPDFExc.hh>
 #include <qpdf/QPDFObjGen.hh>
 #include <qpdf/QPDFObjectHandle.hh>
 #include <qpdf/QPDF.hh>
 #include <qpdf/QPDFWriter.hh>
+#include <qpdf/QUtil.hh>
 
 #include "pikepdf.h"
 
 std::string objecthandle_scalar_value(QPDFObjectHandle h)
 {
     std::ostringstream ss;
     ss.imbue(std::locale::classic());
@@ -117,40 +118,78 @@
     auto pythonic_typename = objecthandle_pythonic_typename(h);
     if (pythonic_typename.empty()) {
         return objecthandle_scalar_value(h);
     }
     return objecthandle_pythonic_typename(h) + "(" + objecthandle_scalar_value(h) + ")";
 }
 
+std::string peek_stream_data(QPDFObjectHandle h, uint recursion_depth)
+{
+    const uint MAX_PEEK_RECURSION_DEPTH = 1;
+    const size_t MAX_PEEK_BYTES         = 20;
+
+    std::ostringstream ss;
+    ss.imbue(std::locale::classic());
+
+    if (recursion_depth > MAX_PEEK_RECURSION_DEPTH) {
+        ss << "<...>";
+        return ss.str();
+    }
+
+    auto buffer = h.getStreamData();
+    auto data   = buffer->getBuffer();
+    std::string data_str(reinterpret_cast<const char *>(data),
+        std::min(MAX_PEEK_BYTES, buffer->getSize()));
+
+    py::bytes pydata(data_str); // Use py::bytes to format output like Python does
+    if (buffer->getSize() > MAX_PEEK_BYTES) {
+        ss << py::repr(pydata) << "...";
+    } else {
+        ss << py::repr(pydata);
+    }
+    return ss.str();
+}
+
 static std::string objecthandle_repr_inner(QPDFObjectHandle h,
     uint recursion_depth,
     uint indent_depth,
-    std::set<QPDFObjGen> *visited,
-    bool *pure_expr)
+    uint &object_count,            // shared between recursive calls
+    std::set<QPDFObjGen> &visited, // shared between recursive calls
+    bool &pure_expr)               // shared between recursive calls
 {
+    const uint MAX_OBJECT_COUNT = 40;
+
     StackGuard sg(" objecthandle_repr_inner");
     std::ostringstream ss;
     ss.imbue(std::locale::classic());
 
     if (!h.isScalar()) {
-        if (visited->count(h.getObjGen()) > 0) {
-            *pure_expr = false;
+        if (visited.count(h.getObjGen()) > 0) {
+            pure_expr = false;
             ss << "<.get_object(" << h.getObjGen() << ")>";
             return ss.str();
         }
 
         if (!(h.getObjGen() == QPDFObjGen(0, 0)))
-            visited->insert(h.getObjGen());
+            visited.insert(h.getObjGen());
     }
     if (h.isPageObject() && recursion_depth >= 1 && h.isIndirect()) {
         ss << "<Pdf.pages.from_objgen"
            << "(" << h.getObjGen() << ")"
            << ">";
         return ss.str();
     }
+    object_count++;
+    if (object_count > MAX_OBJECT_COUNT && recursion_depth > 1) {
+        // If we've printed too many objects, start printing <...> instead
+        // for objects that aren't the top level object.
+        pure_expr = false;
+        ss << "<...>";
+        return ss.str();
+    }
 
     switch (h.getTypeCode()) {
     case qpdf_object_type_e::ot_null:
     case qpdf_object_type_e::ot_boolean:
     case qpdf_object_type_e::ot_integer:
     case qpdf_object_type_e::ot_real:
     case qpdf_object_type_e::ot_name:
@@ -177,16 +216,20 @@
             ss << " ";
             for (auto item : h.getArrayAsVector()) {
                 if (!first_item)
                     ss << ", ";
                 first_item = false;
                 // We don't increase indent_depth when recursing into arrays,
                 // because it doesn't look right. Always increase recursion_depth.
-                ss << objecthandle_repr_inner(
-                    item, recursion_depth + 1, indent_depth, visited, pure_expr);
+                ss << objecthandle_repr_inner(item,
+                    recursion_depth + 1,
+                    indent_depth,
+                    object_count,
+                    visited,
+                    pure_expr);
             }
             ss << " ";
         }
         ss << "]";
         break;
     case qpdf_object_type_e::ot_dictionary:
         ss << "{"; // This will end the line
@@ -205,29 +248,33 @@
                     // repr() of a single page
                     ss << std::quoted(key) << ": <reference to /Pages>";
                 } else {
                     ss << std::quoted(key) << ": "
                        << objecthandle_repr_inner(obj,
                               recursion_depth + 1,
                               indent_depth + 1,
+                              object_count,
                               visited,
                               pure_expr);
                 }
             }
             ss << "\n";
         }
         ss << std::string(indent_depth * 2, ' ') // Restore previous indent level
            << "}";
         break;
     case qpdf_object_type_e::ot_stream:
-        *pure_expr = false;
-        ss << objecthandle_pythonic_typename(h) << "(owner=<...>, data=<...>, "
+        pure_expr = false;
+        ss << objecthandle_pythonic_typename(h) << "("
+           << "owner=<...>, "
+           << "data=" << peek_stream_data(h, recursion_depth) << ", "
            << objecthandle_repr_inner(h.getDict(),
                   recursion_depth + 1,
-                  indent_depth + 1,
+                  indent_depth, // Don't indent here to align dict with stream
+                  object_count,
                   visited,
                   pure_expr)
            << ")";
         break;
     // LCOV_EXCL_START
     default:
         ss << "Unexpected QPDF object type value: " << h.getTypeCode();
@@ -247,15 +294,17 @@
         // qpdf does not consider Operator a scalar but it is as far we
         // are concerned here
         return objecthandle_repr_typename_and_value(h);
     }
 
     std::set<QPDFObjGen> visited;
     bool pure_expr    = true;
-    std::string inner = objecthandle_repr_inner(h, 0, 0, &visited, &pure_expr);
+    uint object_count = 0;
+    std::string inner =
+        objecthandle_repr_inner(h, 0, 0, object_count, visited, pure_expr);
     std::string output;
 
     if (h.isScalar() || h.isDictionary() || h.isArray()) {
         output = objecthandle_pythonic_typename(h) + "(" + inner + ")";
     } else {
         output    = inner;
         pure_expr = false;
```

### Comparing `pikepdf-7.1.2/src/core/page.cpp` & `pikepdf-7.2.0/src/core/page.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/parsers.cpp` & `pikepdf-7.2.0/src/core/parsers.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/parsers.h` & `pikepdf-7.2.0/src/core/parsers.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/pikepdf.cpp` & `pikepdf-7.2.0/src/core/pikepdf.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/pikepdf.h` & `pikepdf-7.2.0/src/core/pikepdf.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/pipeline.cpp` & `pikepdf-7.2.0/src/core/pipeline.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/pipeline.h` & `pikepdf-7.2.0/src/core/pipeline.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/qpdf.cpp` & `pikepdf-7.2.0/src/core/qpdf.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -525,15 +525,26 @@
             "new",
             []() {
                 auto q = std::make_shared<QPDF>();
                 q->emptyPDF();
                 qpdf_basic_settings(*q);
                 return q;
             },
-            "Create a new empty PDF from scratch.")
+            R"~~~(
+            Create a new, empty PDF.
+
+            This is best when you are constructing a PDF from scratch.
+
+            In most cases, if you are working from an existing PDF, you should open the
+            PDF using :meth:`pikepdf.Pdf.open` and transform it, instead of a creating
+            a new one, to preserve metadata and structural information. For example,
+            if you want to split a PDF into two parts, you should open the PDF and
+            transform it into the desired parts, rather than creating a new PDF and
+            copying pages into it.
+            )~~~")
         .def_static("_open",
             open_pdf,
             py::arg("filename_or_stream"),
             py::kw_only(),
             py::arg("password")                = "",
             py::arg("hex_password")            = false,
             py::arg("ignore_xref_streams")     = false,
```

### Comparing `pikepdf-7.1.2/src/core/qpdf_inputsource-inl.h` & `pikepdf-7.2.0/src/core/qpdf_inputsource-inl.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/qpdf_pagelist.cpp` & `pikepdf-7.2.0/src/core/qpdf_pagelist.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -234,16 +234,26 @@
             "p",
             [](PageList &pl, py::ssize_t pnum) {
                 if (pnum <= 0) // Indexing past end is checked in .get_page
                     throw py::index_error(
                         "page access out of range in 1-based indexing");
                 return pl.get_page(pnum - 1);
             },
-            "Convenience - look up page number in ordinal numbering, ``.p(1)`` is "
-            "first page",
+            R"~~~(
+            Look up page number in ordinal numbering, ``.p(1)`` is the first page.
+
+            This is provided for convenience in situations where ordinal numbering
+            is more natural. It is equivalent to ``.pages[pnum - 1]``. ``.p(0)``
+            is an error and negative indexing is not supported.
+
+            If the PDF defines custom page labels (such as labeling front matter
+            with Roman numerals and the main body with Arabic numerals), this
+            function does not account for that. Use :attr:`pikepdf.Page.label`
+            to get the page label for a page.
+            )~~~",
             py::arg("pnum"))
         .def("__iter__", [](PageList &pl) { return PageList(pl.qpdf, 0); })
         .def("__next__",
             [](PageList &pl) {
                 if (pl.iterpos < pl.count())
                     return pl.get_page(pl.iterpos++);
                 throw py::stop_iteration();
@@ -275,46 +285,74 @@
             },
             "Reverse the order of pages.")
         .def(
             "append",
             [](PageList &pl, QPDFPageObjectHelper &page) {
                 pl.insert_page(pl.count(), page);
             },
-            "Add another page to the end.",
+            R"~~~(
+            Add another page to the end.
+
+            While this method copies pages from one document to another, it does not
+            copy certain metadata such as annotations, form fields, bookmarks or
+            structural tree elements. Copying these is a more complex, application
+            specific operation.
+            )~~~",
             py::arg("page"))
         .def(
             "append",
             [](PageList &pl, py::handle page) { pl.insert_page(pl.count(), page); },
-            "Add another page to the end.",
+            R"~~~(
+            Add another page to the end.
+
+            While this method copies pages from one document to another, it does not
+            copy certain metadata such as annotations, form fields, bookmarks or
+            structural tree elements. Copying these is a more complex, application
+            specific operation.
+            )~~~",
             py::arg("page"))
         .def(
             "extend",
             [](PageList &pl, PageList &other) {
                 auto other_count = other.count();
                 for (decltype(other_count) i = 0; i < other_count; i++) {
                     if (other_count != other.count())
                         throw py::value_error(
                             "source page list modified during iteration");
                     pl.insert_page(pl.count(), other.get_page(i));
                 }
             },
-            "Extend the ``Pdf`` by adding pages from another ``Pdf.pages``.",
+            R"~~~(
+            Extend the ``Pdf`` by adding pages from another ``Pdf.pages``.
+
+            While this method copies pages from one document to another, it does not
+            copy certain metadata such as annotations, form fields, bookmarks or
+            structural tree elements. Copying these is a more complex, application
+            specific operation.
+            )~~~",
             py::arg("other"))
         .def(
             "extend",
             [](PageList &pl, py::iterable iterable) {
                 py::iterator it = iterable.attr("__iter__")();
                 while (it != py::iterator::sentinel()) {
                     // assert_pyobject_is_page_obj(*it);
                     assert_pyobject_is_page_helper(*it);
                     pl.insert_page(pl.count(), *it);
                     ++it;
                 }
             },
-            "Extend the ``Pdf`` by adding pages from an iterable of pages.",
+            R"~~~(
+            Extend the ``Pdf`` by adding pages from an iterable of pages.
+
+            While this method copies pages from one document to another, it does not
+            copy certain metadata such as annotations, form fields, bookmarks or
+            structural tree elements. Copying these is a more complex, application
+            specific operation.
+            )~~~",
             py::arg("iterable"))
         .def(
             "remove",
             [](PageList &pl, py::kwargs kwargs) {
                 auto pnum = kwargs["p"].cast<py::ssize_t>();
                 if (pnum <= 0) // Indexing past end is checked in .get_page
                     throw py::index_error(
@@ -329,51 +367,51 @@
             )~~~")
         .def(
             "index",
             [](PageList &pl, const QPDFObjectHandle &h) {
                 return page_index(*pl.qpdf, h);
             },
             R"~~~(
-            Given a pikepdf.Object that is a page, find the index.
+            Given a pikepdf.Object that is a page, find the index number.
 
             That is, returns ``n`` such that ``pdf.pages[n] == this_page``.
             A ``ValueError`` exception is thrown if the page does not belong to
-            to this ``Pdf``.
+            to this ``Pdf``. The first page has index 0.
             )~~~")
         .def(
             "index",
             [](PageList &pl, const QPDFPageObjectHelper &poh) {
                 return page_index(*pl.qpdf, poh.getObjectHandle());
             },
             R"~~~(
             Given a pikepdf.Page (page helper), find the index.
 
             That is, returns ``n`` such that ``pdf.pages[n] == this_page``.
             A ``ValueError`` exception is thrown if the page does not belong to
-            to this ``Pdf``.
+            to this ``Pdf``. The first page has index 0.
             )~~~")
         .def("__repr__",
             [](PageList &pl) {
                 return std::string("<pikepdf._core.PageList len=") +
                        std::to_string(pl.count()) + std::string(">");
             })
         .def(
             "from_objgen",
             [](PageList &pl, int obj, int gen) {
                 return from_objgen(*pl.qpdf, QPDFObjGen(obj, gen));
             },
             R"~~~(
             Given an "objgen" (object ID, generation), return the page.
 
-            Raises an exception if no page matches .
+            Raises an exception if no page matches.
             )~~~")
         .def(
             "from_objgen",
             [](PageList &pl, std::pair<int, int> objgen) {
                 return from_objgen(*pl.qpdf, QPDFObjGen(objgen.first, objgen.second));
             },
             R"~~~(
             Given an "objgen" (object ID, generation), return the page.
 
-            Raises an exception if no page matches .
+            Raises an exception if no page matches.
             )~~~");
 }
```

### Comparing `pikepdf-7.1.2/src/core/qpdf_pagelist.h` & `pikepdf-7.2.0/src/core/qpdf_pagelist.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/rectangle.cpp` & `pikepdf-7.2.0/src/core/rectangle.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/tokenfilter.cpp` & `pikepdf-7.2.0/src/core/tokenfilter.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/utils.cpp` & `pikepdf-7.2.0/src/core/utils.cpp`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/core/utils.h` & `pikepdf-7.2.0/src/core/utils.h`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/__init__.py` & `pikepdf-7.2.0/src/pikepdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/_augments.py` & `pikepdf-7.2.0/src/pikepdf/_augments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/_core.pyi` & `pikepdf-7.2.0/src/pikepdf/_core.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -670,15 +670,15 @@
     def __contains__(self, key: object) -> bool: ...
     def __delitem__(self, key: int) -> None: ...
     def __eq__(self, other: Any) -> bool: ...
     def __getitem__(self, key: int) -> Object: ...
     def __iter__(self) -> Iterator[int]: ...
     def __len__(self) -> int: ...
     def __setitem__(self, key: int, o: Object) -> None: ...
-    def __init__(self, obj: Object, pdf: Pdf, *, auto_repair: bool = ...) -> None: ...
+    def __init__(self, obj: Object, *, auto_repair: bool = ...) -> None: ...
     def _as_map(self) -> _ObjectMapping: ...
     @property
     def obj(self) -> Object: ...
 
 class ContentStreamInstruction:
     @property
     def operands(self) -> _ObjectList: ...
```

### Comparing `pikepdf-7.1.2/src/pikepdf/_cpphelpers.py` & `pikepdf-7.2.0/src/pikepdf/_cpphelpers.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/_methods.py` & `pikepdf-7.2.0/src/pikepdf/_methods.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/_qpdf.py` & `pikepdf-7.2.0/src/pikepdf/_qpdf.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/_xml.py` & `pikepdf-7.2.0/src/pikepdf/_xml.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/codec.py` & `pikepdf-7.2.0/src/pikepdf/codec.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/jbig2.py` & `pikepdf-7.2.0/src/pikepdf/jbig2.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/models/__init__.py` & `pikepdf-7.2.0/src/pikepdf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/models/_content_stream.py` & `pikepdf-7.2.0/src/pikepdf/models/_content_stream.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/models/_transcoding.py` & `pikepdf-7.2.0/src/pikepdf/models/_transcoding.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/models/encryption.py` & `pikepdf-7.2.0/src/pikepdf/models/encryption.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/models/image.py` & `pikepdf-7.2.0/src/pikepdf/models/image.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/models/matrix.py` & `pikepdf-7.2.0/src/pikepdf/models/matrix.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,22 +8,36 @@
 from math import cos, pi, sin
 
 
 class PdfMatrix:
     """Support class for PDF content stream matrices.
 
     PDF content stream matrices are 3x3 matrices summarized by a shorthand
-    ``(a, b, c, d, e, f)`` which correspond to the first two column vectors.
-    The final column vector is always ``(0, 0, 1)`` since this is using
+    ``(a, b, c, d, e, f)``, where the first column vector is ``(a, c, e)``
+    and the second column vector is ``(b, d, f)``. The final column vector
+    is always ``(0, 0, 1)`` since PDF uses
     `homogenous coordinates <https://en.wikipedia.org/wiki/Homogeneous_coordinates>`_.
 
+    ``a`` is the horizontal scaling factor.
+    ``b`` is horizontal skewing.
+    ``c`` is vertical skewing.
+    ``d`` is the vertical scaling factor.
+    ``e`` is the horizontal translation.
+    ``f`` is the vertical translation.
+
+    For scaling, ``a`` and ``d`` are the scaling factors in the horizontal and vertical
+    directions, respectively; for pure scaling, ``b`` and ``c`` are zero.
+
     PDF uses row vectors.  That is, ``vr @ A'`` gives the effect of transforming
     a row vector ``vr=(x, y, 1)`` by the matrix ``A'``.  Most textbook
     treatments use ``A @ vc`` where the column vector ``vc=(x, y, 1)'``.
 
+    Matrices should be **premultipled** with other matrices to concatenate
+    transformations.
+
     (``@`` is the Python matrix multiplication operator.)
 
     Addition and other operations are not implemented because they're not that
     meaningful in a PDF context (they can be defined and are mathematically
     meaningful in general).
 
     PdfMatrix objects are immutable. All transformations on them produce a new
@@ -48,14 +62,20 @@
                            (c, d, 0),
                            (e, f, 1))
         elif len(args[0]) == 3 and len(args[0][0]) == 3:
             self.values = (tuple(args[0][0]),
                            tuple(args[0][1]),
                            tuple(args[0][2]))
         else:
+            try:
+                import numpy as np
+                if isinstance(args[0], (np.ndarray, np.generic)):
+                    self.values = tuple(map(tuple, args[0]))
+            except ImportError:
+                pass
             raise ValueError('invalid arguments: ' + repr(args))
         # fmt: on
 
     @staticmethod
     def identity():
         """Return an identity matrix."""
         return PdfMatrix()
@@ -70,14 +90,36 @@
         return PdfMatrix(
             [
                 [sum(float(i) * float(j) for i, j in zip(row, col)) for col in zip(*b)]
                 for row in a
             ]
         )
 
+    def __array__(self):
+        """Return a numpy array of the matrix.
+
+        This function requires numpy, which is an optional dependency of pikepdf.
+        If numpy is not installed, an ImportError will be raised.
+        """
+        import numpy as np
+
+        return np.array(self.values)
+
+    def inverse(self):
+        """Return the inverse of this matrix.
+
+        The inverse matrix reverses the transformation of the original matrix.
+
+        This function requires numpy, which is an optional dependency of pikepdf.
+        If numpy is not installed, an ImportError will be raised.
+        """
+        import numpy as np
+
+        return PdfMatrix(np.linalg.inv(self.__array__()))
+
     def scaled(self, x, y):
         """Concatenate a scaling matrix to this matrix."""
         return self @ PdfMatrix((x, 0, 0, y, 0, 0))
 
     def rotated(self, angle_degrees_ccw):
         """Concatenate a rotation matrix to this matrix."""
         angle = angle_degrees_ccw / 180.0 * pi
@@ -91,43 +133,43 @@
     @property
     def shorthand(self):
         """Return the 6-tuple (a,b,c,d,e,f) that describes this matrix."""
         return (self.a, self.b, self.c, self.d, self.e, self.f)
 
     @property
     def a(self):
-        """Return matrix this value."""
+        """Return the horizontal scaling factor."""
         return self.values[0][0]
 
     @property
     def b(self):
-        """Return matrix this value."""
+        """Return horizontal skew."""
         return self.values[0][1]
 
     @property
     def c(self):
-        """Return matrix this value."""
+        """Return vertical skew."""
         return self.values[1][0]
 
     @property
     def d(self):
-        """Return matrix this value."""
+        """Return the vertical scaling factor."""
         return self.values[1][1]
 
     @property
     def e(self):
-        """Return matrix this value.
+        """Return the horizontal translation.
 
         Typically corresponds to translation on the x-axis.
         """
         return self.values[2][0]
 
     @property
     def f(self):
-        """Return matrix this value.
+        """Return the vertical translation.
 
         Typically corresponds to translation on the y-axis.
         """
         return self.values[2][1]
 
     def __eq__(self, other):
         if isinstance(other, PdfMatrix):
```

### Comparing `pikepdf-7.1.2/src/pikepdf/models/metadata.py` & `pikepdf-7.2.0/src/pikepdf/models/metadata.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/models/outlines.py` & `pikepdf-7.2.0/src/pikepdf/models/outlines.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf/objects.py` & `pikepdf-7.2.0/src/pikepdf/objects.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/src/pikepdf.egg-info/PKG-INFO` & `pikepdf-7.2.0/src/pikepdf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikepdf
-Version: 7.1.2
+Version: 7.2.0
 Summary: Read and write PDFs with Python, powered by qpdf
 Author-email: "James R. Barlow" <james@purplerock.ca>
 License: MPL-2.0
 Project-URL: documentation, https://pikepdf.readthedocs.io/
 Project-URL: repository, https://github.com/pikepdf/pikepdf
 Project-URL: changelog, https://pikepdf.readthedocs.io/en/latest/releasenotes/index.html
 Keywords: PDF
```

### Comparing `pikepdf-7.1.2/src/pikepdf.egg-info/SOURCES.txt` & `pikepdf-7.2.0/src/pikepdf.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -169,14 +169,15 @@
 tests/test_pages.py
 tests/test_parsers.py
 tests/test_pdf.py
 tests/test_pdfa.py
 tests/test_private_pdfs.py
 tests/test_rectangle.py
 tests/test_refcount.py
+tests/test_repr.py
 tests/test_sanity.py
 tests/resources/1biticc.pdf
 tests/resources/Gray.icc
 tests/resources/aquamarine-cie.pdf
 tests/resources/aquamarine-cie.png
 tests/resources/cmyk-jpeg.pdf
 tests/resources/congress-gray.pdf
```

### Comparing `pikepdf-7.1.2/src/pikepdf.egg-info/requires.txt` & `pikepdf-7.2.0/src/pikepdf.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/conftest.py` & `pikepdf-7.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/1biticc.pdf` & `pikepdf-7.2.0/tests/resources/1biticc.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/aquamarine-cie.pdf` & `pikepdf-7.2.0/tests/resources/aquamarine-cie.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/aquamarine-cie.png` & `pikepdf-7.2.0/tests/resources/aquamarine-cie.png`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/cmyk-jpeg.pdf` & `pikepdf-7.2.0/tests/resources/cmyk-jpeg.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/congress-gray.pdf` & `pikepdf-7.2.0/tests/resources/congress-gray.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/congress.pdf` & `pikepdf-7.2.0/tests/resources/congress.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/content-stream-errors.pdf` & `pikepdf-7.2.0/tests/resources/content-stream-errors.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/form.pdf` & `pikepdf-7.2.0/tests/resources/form.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/formxobject.pdf` & `pikepdf-7.2.0/tests/resources/formxobject.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/fourpages.pdf` & `pikepdf-7.2.0/tests/resources/fourpages.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/graph-encrypted.pdf` & `pikepdf-7.2.0/tests/resources/graph-encrypted.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/graph.pdf` & `pikepdf-7.2.0/tests/resources/graph.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/image-mono-inline.pdf` & `pikepdf-7.2.0/tests/resources/image-mono-inline.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/invalid_creationdate.pdf` & `pikepdf-7.2.0/tests/resources/invalid_creationdate.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/jbig2.pdf` & `pikepdf-7.2.0/tests/resources/jbig2.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/jbig2global.pdf` & `pikepdf-7.2.0/tests/resources/jbig2global.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/outlines.pdf` & `pikepdf-7.2.0/tests/resources/outlines.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/pal-1bit-rgb.pdf` & `pikepdf-7.2.0/tests/resources/pal-1bit-rgb.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/pal-1bit-trivial.pdf` & `pikepdf-7.2.0/tests/resources/pal-1bit-trivial.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/pal.pdf` & `pikepdf-7.2.0/tests/resources/pal.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/pdfx.pdf` & `pikepdf-7.2.0/tests/resources/pdfx.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/pike-flate-jp2.pdf` & `pikepdf-7.2.0/tests/resources/pike-flate-jp2.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/pike-jp2.pdf` & `pikepdf-7.2.0/tests/resources/pike-jp2.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/pink-palette-icc.pdf` & `pikepdf-7.2.0/tests/resources/pink-palette-icc.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/pink-palette-icc.png` & `pikepdf-7.2.0/tests/resources/pink-palette-icc.png`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/rle.pdf` & `pikepdf-7.2.0/tests/resources/rle.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/sandwich.pdf` & `pikepdf-7.2.0/tests/resources/sandwich.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf` & `pikepdf-7.2.0/tests/resources/veraPDF test suite 6-2-10-t02-pass-a.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf` & `pikepdf-7.2.0/tests/resources/veraPDF test suite 6-2-3-3-t01-fail-c.pdf`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_annotation.py` & `pikepdf-7.2.0/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_attachments.py` & `pikepdf-7.2.0/tests/test_attachments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_augments.py` & `pikepdf-7.2.0/tests/test_augments.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_codec.py` & `pikepdf-7.2.0/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_decimal.py` & `pikepdf-7.2.0/tests/test_decimal.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_dictionary.py` & `pikepdf-7.2.0/tests/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_encrypt.py` & `pikepdf-7.2.0/tests/test_encrypt.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_errors.py` & `pikepdf-7.2.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_filters.py` & `pikepdf-7.2.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_foreign.py` & `pikepdf-7.2.0/tests/test_foreign.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_formxobject.py` & `pikepdf-7.2.0/tests/test_formxobject.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_image_access.py` & `pikepdf-7.2.0/tests/test_image_access.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_io.py` & `pikepdf-7.2.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_ipython.py` & `pikepdf-7.2.0/tests/test_ipython.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_job.py` & `pikepdf-7.2.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_matrix.py` & `pikepdf-7.2.0/tests/test_matrix.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,29 +6,31 @@
 from math import isclose
 
 import pytest
 
 from pikepdf.models import PdfMatrix
 
 
+def allclose(m1, m2, abs_tol=1e-6):
+    return all(
+        isclose(x, y, abs_tol=abs_tol) for x, y in zip(m1.shorthand, m2.shorthand)
+    )
+
+
 def test_init_6():
     m = PdfMatrix(1, 0, 0, 1, 0, 0)
     m2 = m.scaled(2, 2)
     m2t = m2.translated(2, 3)
     assert (
         repr(m2t)
         == 'pikepdf.PdfMatrix(((2.0, 0.0, 0.0), (0.0, 2.0, 0.0), (2.0, 3.0, 1.0)))'
     )
     m2tr = m2t.rotated(90)
-    assert isclose(m2tr.a, 0, abs_tol=1e-6)
-    assert isclose(m2tr.b, 2, abs_tol=1e-6)
-    assert isclose(m2tr.c, -2, abs_tol=1e-6)
-    assert isclose(m2tr.d, 0, abs_tol=1e-6)
-    assert isclose(m2tr.e, -3, abs_tol=1e-6)
-    assert isclose(m2tr.f, 2, abs_tol=1e-6)
+    expected = PdfMatrix(0, 2, -2, 0, -3, 2)
+    assert allclose(m2tr, expected)
 
 
 def test_invalid_init():
     with pytest.raises(ValueError, match='arguments'):
         PdfMatrix('strings')
 
 
@@ -38,7 +40,26 @@
     assert m == m_copy
     assert m != 'not matrix'
 
 
 def test_matrix_encode():
     m = PdfMatrix(1, 0, 0, 1, 0, 0)
     assert m.encode() == b'1.000000 0.000000 0.000000 1.000000 0.000000 0.000000'
+
+
+def test_matrix_inverse():
+    pytest.importorskip('numpy')
+
+    m = PdfMatrix(2, 0, 0, 1, 0, 3)
+    minv_m = m.inverse() @ m
+    assert allclose(minv_m, PdfMatrix.identity())
+
+
+def test_numpy():
+    np = pytest.importorskip('numpy')
+
+    m = PdfMatrix(1, 0, 0, 2, 7, 0)
+    m2 = PdfMatrix(np.array([[1, 0, 0], [0, 2, 0], [7, 0, 1]]))
+    assert m == m2
+    arr = np.array(m)
+    arr2 = np.array(m2)
+    assert np.array_equal(arr, arr2)
```

### Comparing `pikepdf-7.1.2/tests/test_metadata.py` & `pikepdf-7.2.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_nametree.py` & `pikepdf-7.2.0/tests/test_nametree.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_numbertree.py` & `pikepdf-7.2.0/tests/test_numbertree.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_object.py` & `pikepdf-7.2.0/tests/test_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -332,84 +332,14 @@
 
 
 def test_not_constructible():
     with pytest.raises(TypeError, match="constructor"):
         Object()
 
 
-class TestRepr:
-    def test_repr_dict(self):
-        d = Dictionary(
-            {
-                '/Boolean': True,
-                '/Integer': 42,
-                '/Real': Decimal('42.42'),
-                '/String': String('hi'),
-                '/Array': Array([1, 2, 3.14]),
-                '/Operator': Operator('q'),
-                '/Dictionary': Dictionary({'/Color': 'Red'}),
-                '/None': None,
-            }
-        )
-        short_pi = '3.14'
-        expected = (
-            """\
-            pikepdf.Dictionary({
-                "/Array": [ 1, 2, Decimal('%s') ],
-                "/Boolean": True,
-                "/Dictionary": {
-                    "/Color": "Red"
-                },
-                "/Integer": 42,
-                "/None": None,
-                "/Operator": pikepdf.Operator("q"),
-                "/Real": Decimal('42.42'),
-                "/String": "hi"
-            })
-        """
-            % short_pi
-        )
-
-        def strip_all_whitespace(s):
-            return ''.join(s.split())
-
-        assert strip_all_whitespace(repr(d)) == strip_all_whitespace(expected)
-        assert eval(repr(d)) == d
-
-    def test_repr_scalar(self):
-        scalars = [
-            False,
-            666,
-            Decimal('3.14'),
-            String('scalar'),
-            Name('/Bob'),
-            Operator('Q'),
-        ]
-        for s in scalars:
-            assert eval(repr(s)) == s
-
-    def test_repr_indirect(self, resources):
-        with pikepdf.open(resources / 'graph.pdf') as graph:
-            repr_page0 = repr(graph.pages[0])
-            assert repr_page0[0] == '<', 'should not be constructible'
-
-    def test_repr_circular(self):
-        with pikepdf.new() as pdf:
-            pdf.Root.Circular = pdf.make_indirect(Dictionary())
-            pdf.Root.Circular.Parent = pdf.make_indirect(Dictionary())
-            pdf.Root.Circular.Parent = pdf.make_indirect(pdf.Root.Circular)
-            assert '.get_object' in repr(pdf.Root.Circular)
-
-    def test_repr_indirect_page(self, resources):
-        with pikepdf.open(resources / 'outlines.pdf') as outlines:
-            assert 'from_objgen' in repr(outlines.Root.Pages.Kids)
-            # An indirect page reference in the Dests name tree
-            assert 'from_objgen' in repr(outlines.Root.Names.Dests.Kids[0].Names[1])
-
-
 def test_operator_inline(resources):
     with pikepdf.open(resources / 'image-mono-inline.pdf') as pdf:
         instructions = parse_content_stream(pdf.pages[0], operators='BI ID EI')
         assert len(instructions) == 1
         _operands, operator = instructions[0]
         assert operator == pikepdf.Operator("INLINE IMAGE")
```

### Comparing `pikepdf-7.1.2/tests/test_outlines.py` & `pikepdf-7.2.0/tests/test_outlines.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_page.py` & `pikepdf-7.2.0/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_pages.py` & `pikepdf-7.2.0/tests/test_pages.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_parsers.py` & `pikepdf-7.2.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_pdf.py` & `pikepdf-7.2.0/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_pdfa.py` & `pikepdf-7.2.0/tests/test_pdfa.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_private_pdfs.py` & `pikepdf-7.2.0/tests/test_private_pdfs.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_rectangle.py` & `pikepdf-7.2.0/tests/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_refcount.py` & `pikepdf-7.2.0/tests/test_refcount.py`

 * *Files identical despite different names*

### Comparing `pikepdf-7.1.2/tests/test_sanity.py` & `pikepdf-7.2.0/tests/test_sanity.py`

 * *Files identical despite different names*

