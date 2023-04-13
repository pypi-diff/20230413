# Comparing `tmp/ape-solidity-0.6.2.tar.gz` & `tmp/ape-solidity-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-solidity-0.6.2.tar", last modified: Tue Mar 21 23:02:07 2023, max compression
+gzip compressed data, was "ape-solidity-0.6.3.tar", last modified: Thu Apr 13 22:00:18 2023, max compression
```

## Comparing `ape-solidity-0.6.2.tar` & `ape-solidity-0.6.3.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.742077 ape-solidity-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.734077 ape-solidity-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.734077 ape-solidity-0.6.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.734077 ape-solidity-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-03-21 23:02:07.742077 ape-solidity-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.734077 ape-solidity-0.6.2/ape_solidity/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/ape_solidity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/ape_solidity/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27577 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/ape_solidity/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/ape_solidity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/ape_solidity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-21 23:02:07.000000 ape-solidity-0.6.2/ape_solidity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.734077 ape-solidity-0.6.2/ape_solidity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-03-21 23:02:07.000000 ape-solidity-0.6.2/ape_solidity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-03-21 23:02:07.000000 ape-solidity-0.6.2/ape_solidity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 23:02:07.000000 ape-solidity-0.6.2/ape_solidity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 23:02:07.000000 ape-solidity-0.6.2/ape_solidity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-21 23:02:07.000000 ape-solidity-0.6.2/ape_solidity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-21 23:02:07.000000 ape-solidity-0.6.2/ape_solidity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-21 23:02:07.742077 ape-solidity-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.734077 ape-solidity-0.6.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.738077 ape-solidity-0.6.2/tests/BrownieProject/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/BrownieProject/brownie-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.738077 ape-solidity-0.6.2/tests/BrownieProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/BrownieProject/contracts/BrownieContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.738077 ape-solidity-0.6.2/tests/BrownieStyleDependency/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/BrownieStyleDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.738077 ape-solidity-0.6.2/tests/BrownieStyleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/BrownieStyleDependency/contracts/FailingContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.738077 ape-solidity-0.6.2/tests/Dependency/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/Dependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.738077 ape-solidity-0.6.2/tests/Dependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/Dependency/contracts/Dependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/Dependency/contracts/OlderDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.738077 ape-solidity-0.6.2/tests/Dependency/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.738077 ape-solidity-0.6.2/tests/Dependency/contracts/subfolder_with_imports/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.738077 ape-solidity-0.6.2/tests/DependencyOfDependency/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/DependencyOfDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.738077 ape-solidity-0.6.2/tests/DependencyOfDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.738077 ape-solidity-0.6.2/tests/ProjectWithinProject/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/ProjectWithinProject/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.738077 ape-solidity-0.6.2/tests/ProjectWithinProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/ProjectWithinProject/contracts/Contract.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.738077 ape-solidity-0.6.2/tests/VersionSpecifiedInConfig/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/VersionSpecifiedInConfig/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.738077 ape-solidity-0.6.2/tests/VersionSpecifiedInConfig/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.742077 ape-solidity-0.6.2/tests/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/CircularImport1.sol
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/CircularImport2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/CompilesOnce.sol
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/DifferentNameThanFile.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.742077 ape-solidity-0.6.2/tests/contracts/DirectoryWithExtension.sol/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/DirectoryWithExtension.sol/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/ExperimentalABIEncoderV2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/ImportOlderDependency.sol
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/ImportSourceWithEqualSignVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/ImportSourceWithNoPrefixVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/ImportingLessConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/Imports.sol
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/LibraryFun.sol
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/MissingPragma.sol
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/MultipleDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/NumerousDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/OlderVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/RandomVyperFile.vy
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/RangedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/SpacesInPragma.sol
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/SpecificVersionNoPrefix.sol
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/SpecificVersionNoPrefix2.sol
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/SpecificVersionRange.sol
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/SpecificVersionWithEqualSign.sol
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/UseYearn.sol
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/VagueVersion.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.742077 ape-solidity-0.6.2/tests/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/subfolder/Relativecontract.sol
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:02:07.742077 ape-solidity-0.6.2/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/scripts/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    15704 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-03-21 23:01:17.000000 ape-solidity-0.6.2/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.297256 ape-solidity-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.289256 ape-solidity-0.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.289256 ape-solidity-0.6.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.289256 ape-solidity-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-13 22:00:18.297256 ape-solidity-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.289256 ape-solidity-0.6.3/ape_solidity/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/ape_solidity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/ape_solidity/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28796 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/ape_solidity/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/ape_solidity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/ape_solidity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 22:00:18.000000 ape-solidity-0.6.3/ape_solidity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/ape_solidity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-13 22:00:18.000000 ape-solidity-0.6.3/ape_solidity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-13 22:00:18.000000 ape-solidity-0.6.3/ape_solidity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:00:18.000000 ape-solidity-0.6.3/ape_solidity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:00:18.000000 ape-solidity-0.6.3/ape_solidity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-13 22:00:18.000000 ape-solidity-0.6.3/ape_solidity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 22:00:18.000000 ape-solidity-0.6.3/ape_solidity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 22:00:18.297256 ape-solidity-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/BrownieProject/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/BrownieProject/brownie-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/BrownieProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/BrownieProject/contracts/BrownieContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/BrownieStyleDependency/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/BrownieStyleDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/BrownieStyleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/BrownieStyleDependency/contracts/FailingContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/Dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/Dependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/Dependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/Dependency/contracts/Dependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/Dependency/contracts/OlderDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/Dependency/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/Dependency/contracts/subfolder_with_imports/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/DependencyOfDependency/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/DependencyOfDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/DependencyOfDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/ProjectWithinProject/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/ProjectWithinProject/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/ProjectWithinProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/ProjectWithinProject/contracts/Contract.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/VersionSpecifiedInConfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/VersionSpecifiedInConfig/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.293256 ape-solidity-0.6.3/tests/VersionSpecifiedInConfig/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.297256 ape-solidity-0.6.3/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/CircularImport1.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/CircularImport2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/CompilesOnce.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/DifferentNameThanFile.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.297256 ape-solidity-0.6.3/tests/contracts/DirectoryWithExtension.sol/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/DirectoryWithExtension.sol/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/ExperimentalABIEncoderV2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/ImportOlderDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/ImportSourceWithEqualSignVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/ImportSourceWithNoPrefixVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/ImportingLessConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/Imports.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/LibraryFun.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/MissingPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/MultipleDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/NumerousDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/OlderVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/RandomVyperFile.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/RangedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/SpacesInPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/SpecificVersionNoPrefix.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/SpecificVersionNoPrefix2.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/SpecificVersionRange.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/SpecificVersionWithEqualSign.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/UseYearn.sol
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/VagueVersion.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.297256 ape-solidity-0.6.3/tests/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/subfolder/Relativecontract.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:00:18.297256 ape-solidity-0.6.3/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/scripts/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16112 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-13 21:59:31.000000 ape-solidity-0.6.3/tests/test_integration.py
```

### Comparing `ape-solidity-0.6.2/.github/ISSUE_TEMPLATE/bug.md` & `ape-solidity-0.6.3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/.github/ISSUE_TEMPLATE/feature.md` & `ape-solidity-0.6.3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/.github/ISSUE_TEMPLATE/work-item.md` & `ape-solidity-0.6.3/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/.github/release-drafter.yml` & `ape-solidity-0.6.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/.github/workflows/codeql.yml` & `ape-solidity-0.6.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/.github/workflows/prtitle.yaml` & `ape-solidity-0.6.3/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/.github/workflows/publish.yaml` & `ape-solidity-0.6.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/.github/workflows/stale-prs.yml` & `ape-solidity-0.6.3/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/.github/workflows/test.yaml` & `ape-solidity-0.6.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/.gitignore` & `ape-solidity-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/.pre-commit-config.yaml` & `ape-solidity-0.6.3/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 -   repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
     -   id: mypy
```

### Comparing `ape-solidity-0.6.2/CONTRIBUTING.md` & `ape-solidity-0.6.3/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 It's a good idea to make pull requests early on.
 A pull request represents the start of a discussion, and doesn't necessarily need to be the final, finished submission.
 
 If you are opening a work-in-progress pull request to verify that it passes CI tests, please consider
 [marking it as a draft](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests#draft-pull-requests).
 
-Join the Ethereum Python [Discord](https://discord.gg/PcEJ54yX) if you have any questions.
+Join the ApeWorX [Discord](https://discord.gg/apeworx) if you have any questions.
 
 ## Testing
 
 By default, the test suite will use a new, temporary path for the Solidity compiler installations.
 This ensures that the tests always run from a clean slate without any relying on existing installations.
 
 If you wish to use your existing `~/.solcx` installations instead, you must set the environment variable `APE_SOLIDITY_USE_SYSTEM_SOLC=1`.
```

### Comparing `ape-solidity-0.6.2/LICENSE` & `ape-solidity-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/PKG-INFO` & `ape-solidity-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.6.2
+Version: 0.6.3
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-solidity-0.6.2/README.md` & `ape-solidity-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/ape_solidity/_utils.py` & `ape-solidity-0.6.3/ape_solidity/_utils.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/ape_solidity/compiler.py` & `ape-solidity-0.6.3/ape_solidity/compiler.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from copy import copy
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Set, Tuple, Union, cast
 
 import solcx  # type: ignore
 from ape.api import CompilerAPI, PluginConfig
 from ape.contracts import ContractInstance
-from ape.exceptions import CompilerError
+from ape.exceptions import CompilerError, ContractLogicError
 from ape.logging import logger
 from ape.types import AddressType, ContractType
 from ape.utils import cached_property, get_relative_path
-from ethpm_types import PackageManifest
+from eth_utils import is_0x_prefixed
+from ethpm_types import HexBytes, PackageManifest
 from requests.exceptions import ConnectionError
 from semantic_version import NpmSpec, Version  # type: ignore
 from solcx.exceptions import SolcError  # type: ignore
 from solcx.install import get_executable  # type: ignore
 from solcx.main import _compile_combined_json  # type: ignore
 
 from ape_solidity._utils import (
@@ -255,15 +256,14 @@
                         builder.contracts_cache / dep_id,
                         builder,
                     )
 
     def get_compiler_settings(
         self, contract_filepaths: List[Path], base_path: Optional[Path] = None
     ) -> Dict[Version, Dict]:
-
         # Currently needed because of a bug in Ape core 0.5.5.
         only_files = []
         for path in contract_filepaths:
             if path.is_dir():
                 logger.error(
                     f"Unable to get compiler settings for directory '{path.name}'. Skipping."
                 )
@@ -655,7 +655,39 @@
     def _get_best_version(self, path: Path, source_by_pragma_spec: Dict) -> Version:
         pragma_spec = source_by_pragma_spec[path]
         return (
             pragma_spec.select(self.installed_versions)
             if pragma_spec
             else max(self.installed_versions)
         )
+
+    def enrich_error(self, err: ContractLogicError) -> ContractLogicError:
+        if not is_0x_prefixed(err.revert_message):
+            return err
+
+        # Check for ErrorABI.
+        bytes_message = HexBytes(err.revert_message)
+        selector = bytes_message[:4]
+        input_data = bytes_message[4:]
+        address = err.contract_address or getattr(err.txn, "receiver", None)
+        if not address:
+            return err
+
+        if not self.network_manager.active_provider:
+            # Connection required.
+            return err
+
+        contract = self.chain_manager.contracts.instance_at(address)
+        if not contract:
+            return err
+
+        if selector not in contract.contract_type.errors:
+            # Not an ErrorABI selector.
+            return err
+
+        ecosystem = self.provider.network.ecosystem
+        abi = contract.contract_type.errors[selector]
+        inputs = ecosystem.decode_calldata(abi, input_data)
+        error_class = contract.get_error_by_signature(abi.signature)
+        return error_class(
+            abi, inputs, txn=err.txn, trace=err.trace, contract_address=err.contract_address
+        )
```

### Comparing `ape-solidity-0.6.2/ape_solidity.egg-info/PKG-INFO` & `ape-solidity-0.6.3/ape_solidity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.6.2
+Version: 0.6.3
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-solidity-0.6.2/ape_solidity.egg-info/SOURCES.txt` & `ape-solidity-0.6.3/ape_solidity.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 tests/VersionSpecifiedInConfig/ape-config.yaml
 tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
 tests/contracts/CircularImport1.sol
 tests/contracts/CircularImport2.sol
 tests/contracts/CompilesOnce.sol
 tests/contracts/DifferentNameThanFile.sol
 tests/contracts/ExperimentalABIEncoderV2.sol
+tests/contracts/HasError.sol
 tests/contracts/ImportOlderDependency.sol
 tests/contracts/ImportSourceWithEqualSignVersion.sol
 tests/contracts/ImportSourceWithNoPrefixVersion.sol
 tests/contracts/ImportingLessConstrainedVersion.sol
 tests/contracts/Imports.sol
 tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
 tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
```

### Comparing `ape-solidity-0.6.2/ape_solidity.egg-info/requires.txt` & `ape-solidity-0.6.3/ape_solidity.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 py-solc-x<2,>=1.1.0
-eth-ape<0.7,>=0.6.4
+eth-ape<0.7,>=0.6.8
 ethpm-types
 packaging
 requests
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
-black>=22.12.0
-mypy>=0.991
+black<24,>=23.3.0
+mypy<1,>=0.991
 types-requests
 types-setuptools
-flake8>=5.0.4
-isort>=5.10.1
+flake8<7,>=6.0.0
+isort<6,>=5.10.1
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
 setuptools
@@ -32,20 +32,20 @@
 
 [doc]
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
 
 [lint]
-black>=22.12.0
-mypy>=0.991
+black<24,>=23.3.0
+mypy<1,>=0.991
 types-requests
 types-setuptools
-flake8>=5.0.4
-isort>=5.10.1
+flake8<7,>=6.0.0
+isort<6,>=5.10.1
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 
 [release]
 setuptools
 setuptools-scm
```

### Comparing `ape-solidity-0.6.2/pyproject.toml` & `ape-solidity-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/setup.py` & `ape-solidity-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=22.12.0",  # auto-formatter and linter
-        "mypy>=0.991",  # Static type analyzer
+        "black>=23.3.0,<24",  # Auto-formatter and linter
+        "mypy>=0.991,<1",  # Static type analyzer
         "types-requests",  # Needed due to mypy typeshed
         "types-setuptools",  # Needed due to mypy typeshed
-        "flake8>=5.0.4",  # Style linter
-        "isort>=5.10.1",  # Import sorting linter
+        "flake8>=6.0.0,<7",  # Style linter
+        "isort>=5.10.1,<6",  # Import sorting linter
         "mdformat>=0.7.16",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
     ],
     "doc": [
         "Sphinx>=3.4.3,<4",  # Documentation generator
         "sphinx_rtd_theme>=0.1.9,<1",  # Readthedocs.org theme
@@ -61,15 +61,15 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-solidity",
     include_package_data=True,
     install_requires=[
         "py-solc-x>=1.1.0,<2",
-        "eth-ape>=0.6.4,<0.7",
+        "eth-ape>=0.6.8,<0.7",
         "ethpm-types",  # Use the version ape requires
         "packaging",  # Use the version ape requires
         "requests",
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_solidity"],
```

### Comparing `ape-solidity-0.6.2/tests/ape-config.yaml` & `ape-solidity-0.6.3/tests/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/tests/conftest.py` & `ape-solidity-0.6.3/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,10 +106,20 @@
 
 @pytest.fixture
 def account():
     return ape.accounts.test_accounts[0]
 
 
 @pytest.fixture
+def owner():
+    return ape.accounts.test_accounts[1]
+
+
+@pytest.fixture
+def not_owner():
+    return ape.accounts.test_accounts[2]
+
+
+@pytest.fixture
 def connection():
     with ape.networks.ethereum.local.use_provider("test"):
         yield
```

### Comparing `ape-solidity-0.6.2/tests/contracts/Imports.sol` & `ape-solidity-0.6.3/tests/contracts/Imports.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/tests/contracts/LibraryFun.sol` & `ape-solidity-0.6.3/tests/contracts/LibraryFun.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/tests/scripts/clean.py` & `ape-solidity-0.6.3/tests/scripts/clean.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.6.2/tests/test_compiler.py` & `ape-solidity-0.6.3/tests/test_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,7 +380,18 @@
         _ = project.C
 
     library = project.Set.deploy(sender=account)
     compiler.add_library(library)
 
     # After deploying and adding the library, we can use contracts that need it.
     assert project.C
+
+
+def test_enrich_error(compiler, project, owner, not_owner, connection):
+    compiler.compile((project.contracts_folder / "HasError.sol",))
+
+    # Deploy so Ape know about contract type.
+    contract = owner.deploy(project.HasError)
+    with pytest.raises(contract.Unauthorized) as err:
+        contract.withdraw(sender=not_owner)
+
+    assert err.value.inputs == {"addr": not_owner.address, "counter": 123}
```

### Comparing `ape-solidity-0.6.2/tests/test_integration.py` & `ape-solidity-0.6.3/tests/test_integration.py`

 * *Files identical despite different names*

