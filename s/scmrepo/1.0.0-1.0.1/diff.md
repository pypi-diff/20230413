# Comparing `tmp/scmrepo-1.0.0.tar.gz` & `tmp/scmrepo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmrepo-1.0.0.tar", last modified: Mon Apr 10 08:50:52 2023, max compression
+gzip compressed data, was "scmrepo-1.0.1.tar", last modified: Thu Apr 13 07:13:27 2023, max compression
```

## Comparing `scmrepo-1.0.0.tar` & `scmrepo-1.0.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.317601 scmrepo-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-10 08:50:30.000000 scmrepo-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-10 08:50:30.000000 scmrepo-1.0.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-10 08:50:30.000000 scmrepo-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-10 08:50:30.000000 scmrepo-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-10 08:50:52.317601 scmrepo-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-10 08:50:30.000000 scmrepo-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-10 08:50:30.000000 scmrepo-1.0.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-10 08:50:30.000000 scmrepo-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-10 08:50:52.317601 scmrepo-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.309601 scmrepo-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/src/scmrepo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/asyn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/src/scmrepo/git/
--rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/src/scmrepo/git/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/src/scmrepo/git/backend/dulwich/
--rw-r--r--   0 runner    (1001) docker     (123)    29235 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/dulwich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/dulwich/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21888 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/gitpython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/src/scmrepo/git/backend/pygit2/
--rw-r--r--   0 runner    (1001) docker     (123)    27611 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/pygit2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/backend/pygit2/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    19779 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/git/stash.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/noscm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-10 08:50:30.000000 scmrepo-1.0.0/src/scmrepo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.313601 scmrepo-1.0.0/src/scmrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-10 08:50:52.000000 scmrepo-1.0.0/src/scmrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-10 08:50:52.000000 scmrepo-1.0.0/src/scmrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:50:52.000000 scmrepo-1.0.0/src/scmrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:50:52.000000 scmrepo-1.0.0/src/scmrepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-10 08:50:52.000000 scmrepo-1.0.0/src/scmrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 08:50:52.000000 scmrepo-1.0.0/src/scmrepo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.317601 scmrepo-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:50:52.317601 scmrepo-1.0.0/tests/git-init/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_dulwich.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34105 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_noscm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_pygit2.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_scmrepo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/test_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/user.key
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-10 08:50:30.000000 scmrepo-1.0.0/tests/user.key.pub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:27.804880 scmrepo-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 07:13:06.000000 scmrepo-1.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-13 07:13:06.000000 scmrepo-1.0.1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 07:13:06.000000 scmrepo-1.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:27.800881 scmrepo-1.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-13 07:13:06.000000 scmrepo-1.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:27.800881 scmrepo-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-13 07:13:06.000000 scmrepo-1.0.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-13 07:13:06.000000 scmrepo-1.0.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-13 07:13:06.000000 scmrepo-1.0.1/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-13 07:13:06.000000 scmrepo-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-13 07:13:06.000000 scmrepo-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-13 07:13:06.000000 scmrepo-1.0.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-13 07:13:06.000000 scmrepo-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-13 07:13:06.000000 scmrepo-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-13 07:13:27.804880 scmrepo-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-13 07:13:06.000000 scmrepo-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-13 07:13:06.000000 scmrepo-1.0.1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-13 07:13:06.000000 scmrepo-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-13 07:13:27.804880 scmrepo-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:27.796881 scmrepo-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:27.800881 scmrepo-1.0.1/src/scmrepo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:27.800881 scmrepo-1.0.1/src/scmrepo/git/
+-rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:27.804880 scmrepo-1.0.1/src/scmrepo/git/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/git/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/git/backend/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:27.804880 scmrepo-1.0.1/src/scmrepo/git/backend/dulwich/
+-rw-r--r--   0 runner    (1001) docker     (123)    29241 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/git/backend/dulwich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/git/backend/dulwich/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21888 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/git/backend/gitpython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:27.804880 scmrepo-1.0.1/src/scmrepo/git/backend/pygit2/
+-rw-r--r--   0 runner    (1001) docker     (123)    27611 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/git/backend/pygit2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/git/backend/pygit2/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20726 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/git/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/git/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/git/stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/noscm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-13 07:13:06.000000 scmrepo-1.0.1/src/scmrepo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:27.800881 scmrepo-1.0.1/src/scmrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-13 07:13:27.000000 scmrepo-1.0.1/src/scmrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-13 07:13:27.000000 scmrepo-1.0.1/src/scmrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:13:27.000000 scmrepo-1.0.1/src/scmrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 07:13:27.000000 scmrepo-1.0.1/src/scmrepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-13 07:13:27.000000 scmrepo-1.0.1/src/scmrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 07:13:27.000000 scmrepo-1.0.1/src/scmrepo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:27.804880 scmrepo-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:06.000000 scmrepo-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-13 07:13:06.000000 scmrepo-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-13 07:13:06.000000 scmrepo-1.0.1/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 07:13:27.804880 scmrepo-1.0.1/tests/git-init/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-13 07:13:06.000000 scmrepo-1.0.1/tests/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-13 07:13:06.000000 scmrepo-1.0.1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-13 07:13:06.000000 scmrepo-1.0.1/tests/test_dulwich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-13 07:13:06.000000 scmrepo-1.0.1/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34105 2023-04-13 07:13:06.000000 scmrepo-1.0.1/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-13 07:13:06.000000 scmrepo-1.0.1/tests/test_noscm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-13 07:13:06.000000 scmrepo-1.0.1/tests/test_pygit2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-13 07:13:06.000000 scmrepo-1.0.1/tests/test_scmrepo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-04-13 07:13:06.000000 scmrepo-1.0.1/tests/test_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-13 07:13:06.000000 scmrepo-1.0.1/tests/user.key
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-13 07:13:06.000000 scmrepo-1.0.1/tests/user.key.pub
```

### Comparing `scmrepo-1.0.0/.cruft.json` & `scmrepo-1.0.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/.github/dependabot.yml` & `scmrepo-1.0.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/.github/workflows/release.yaml` & `scmrepo-1.0.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/.github/workflows/tests.yaml` & `scmrepo-1.0.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/.gitignore` & `scmrepo-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/.pre-commit-config.yaml` & `scmrepo-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/CODE_OF_CONDUCT.rst` & `scmrepo-1.0.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/CONTRIBUTING.rst` & `scmrepo-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/LICENSE` & `scmrepo-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/PKG-INFO` & `scmrepo-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 1.0.0
+Version: 1.0.1
 Summary: SCM wrapper and fsspec filesystem for Git for use in DVC
 Home-page: https://github.com/iterative/scmrepo
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scmrepo-1.0.0/README.rst` & `scmrepo-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/noxfile.py` & `scmrepo-1.0.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/pyproject.toml` & `scmrepo-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/setup.cfg` & `scmrepo-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 	pytest-test-utils==0.0.8
 	pytest-asyncio==0.18.3
 	pytest-docker==0.12.0; python_version < '3.10' or sys_platform != 'win32'
 	mock==5.0.1
 	paramiko==3.1.0
 	types-certifi==2021.10.8.3
 	types-mock==5.0.0.6
-	types-paramiko==3.0.0.6
+	types-paramiko==3.0.0.7
 dev = 
 	%(tests)s
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
```

### Comparing `scmrepo-1.0.0/src/scmrepo/asyn.py` & `scmrepo-1.0.1/src/scmrepo/asyn.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo/base.py` & `scmrepo-1.0.1/src/scmrepo/base.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo/exceptions.py` & `scmrepo-1.0.1/src/scmrepo/exceptions.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo/fs.py` & `scmrepo-1.0.1/src/scmrepo/fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo/git/__init__.py` & `scmrepo-1.0.1/src/scmrepo/git/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo/git/backend/base.py` & `scmrepo-1.0.1/src/scmrepo/git/backend/base.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo/git/backend/dulwich/__init__.py` & `scmrepo-1.0.1/src/scmrepo/git/backend/dulwich/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,15 +576,15 @@
 
             return new_refs
 
         try:
             result = client.send_pack(
                 path,
                 update_refs,
-                self.repo.object_store.generate_pack_data,
+                generate_pack_data=self.repo.generate_pack_data,
                 progress=(DulwichProgressReporter(progress) if progress else None),
             )
         except (NotGitRepository, SendPackError) as exc:
             src = [lh for (lh, _, _) in selected_refs]
             raise SCMError(f"Git failed to push '{src}' to '{url}'") from exc
         except HTTPUnauthorized as exc:
             raise AuthError(url) from exc
```

### Comparing `scmrepo-1.0.0/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py` & `scmrepo-1.0.1/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo/git/backend/dulwich/client.py` & `scmrepo-1.0.1/src/scmrepo/git/backend/dulwich/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,12 +64,13 @@
             self._store_credentials.approve()
         return result
 
     def _get_auth(self) -> Dict[str, str]:
         from urllib3.util import make_headers
 
         try:
-            creds = Credential(username=self._username, url=self._base_url).fill()
+            base_url = self._base_url.rstrip("/")
+            creds = Credential(username=self._username, url=base_url).fill()
             self._store_credentials = creds
             return make_headers(basic_auth=f"{creds.username}:{creds.password}")
         except CredentialNotFoundError:
             return {}
```

### Comparing `scmrepo-1.0.0/src/scmrepo/git/backend/gitpython.py` & `scmrepo-1.0.1/src/scmrepo/git/backend/gitpython.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo/git/backend/pygit2/__init__.py` & `scmrepo-1.0.1/src/scmrepo/git/backend/pygit2/__init__.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo/git/backend/pygit2/callbacks.py` & `scmrepo-1.0.1/src/scmrepo/git/backend/pygit2/callbacks.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo/git/credentials.py` & `scmrepo-1.0.1/src/scmrepo/git/credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,22 +103,23 @@
     >>> helper = GitCredentialHelper("store") # Use `git credential-store`
     >>> generated = Credential(url="https://github.com/dtrifiro/aprivaterepo")
     >>> credentials = helper.get(generated)
     >>> username = credentials.username
     >>> password = credentials.password
     """
 
-    def __init__(self, command: str):
+    def __init__(self, command: str, use_http_path: bool = False):
         super().__init__()
         self._command = command
         self._run_kwargs: Dict[str, Any] = {}
         if self._command[0] == "!":
             # On Windows this will only work in git-bash and/or WSL2
             self._run_kwargs["shell"] = True
         self._encoding = locale.getpreferredencoding()
+        self.use_http_path = use_http_path
 
     def _prepare_command(self, action: Optional[str] = None) -> Union[str, List[str]]:
         if self._command[0] == "!":
             return self._command[1:] + (f" {action}" if action else "")
 
         if sys.platform != "win32":
             argv = shlex.split(self._command)
@@ -146,15 +147,20 @@
 
         return [executable, *argv[1:]]
 
     def get(self, credential: "Credential", **kwargs) -> "Credential":
         if not (credential.protocol or credential.host):
             raise ValueError("One of protocol, hostname must be provided")
         cmd = self._prepare_command("get")
-        helper_input = [f"{key}={value}" for key, value in credential.items()]
+        use_path = credential.protocol in ("http", "https") and self.use_http_path
+        helper_input = [
+            f"{key}={value}"
+            for key, value in credential.items()
+            if key != "path" or use_path
+        ]
         helper_input.append("")
 
         try:
             res = subprocess.run(  # type: ignore # nosec B603 # breaks on 3.6
                 cmd,
                 check=True,
                 capture_output=True,
@@ -166,31 +172,36 @@
             raise CredentialNotFoundError(exc.stderr) from exc
         except FileNotFoundError as exc:
             raise CredentialNotFoundError("Helper not found") from exc
         if res.stderr:
             logger.debug(res.stderr)
 
         credentials = {}
-        for line in res.stdout.strip().splitlines():
+        for line in res.stdout.splitlines():
             try:
-                key, value = line.split("=")
+                key, value = line.split("=", maxsplit=1)
                 credentials[key] = value
             except ValueError:
                 continue
         if not credentials:
             raise CredentialNotFoundError("No credentials found")
         quit_ = credentials.get("quit")
         if quit_ is not None and quit_.lower() in ("true", "1"):
             raise CredentialQuitError("Helper returned quit=1")
         return Credential(**credentials)
 
     def store(self, credential: "Credential", **kwargs):
         """Store the credential, if applicable to the helper"""
         cmd = self._prepare_command("store")
-        helper_input = [f"{key}={value}" for key, value in credential.items()]
+        use_path = credential.protocol in ("http", "https") and self.use_http_path
+        helper_input = [
+            f"{key}={value}"
+            for key, value in credential.items()
+            if key != "path" or use_path
+        ]
         helper_input.append("")
 
         try:
             res = subprocess.run(  # type: ignore # nosec B603 # pylint: disable=W1510
                 cmd,
                 capture_output=True,
                 input=os.linesep.join(helper_input),
@@ -201,15 +212,20 @@
                 logger.debug(res.stderr)
         except FileNotFoundError:
             logger.debug("Helper not found", exc_info=True)
 
     def erase(self, credential: "Credential", **kwargs):
         """Remove a matching credential, if any, from the helper’s storage"""
         cmd = self._prepare_command("erase")
-        helper_input = [f"{key}={value}" for key, value in credential.items()]
+        use_path = credential.protocol in ("http", "https") and self.use_http_path
+        helper_input = [
+            f"{key}={value}"
+            for key, value in credential.items()
+            if key != "path" or use_path
+        ]
         helper_input.append("")
 
         try:
             res = subprocess.run(  # type: ignore # nosec B603 # pylint: disable=W1510
                 cmd,
                 capture_output=True,
                 input=os.linesep.join(helper_input),
@@ -220,15 +236,15 @@
                 logger.debug(res.stderr)
         except FileNotFoundError:
             logger.debug("Helper not found", exc_info=True)
 
     @staticmethod
     def get_matching_commands(
         base_url: str, config: Optional[Union["ConfigDict", "StackedConfig"]] = None
-    ):
+    ) -> Iterator[Tuple[str, bool]]:
         config = config or StackedConfig.default()
         if isinstance(config, StackedConfig):
             backends: Iterable["ConfigDict"] = config.backends
         else:
             backends = [config]
 
         for conf in backends:
@@ -236,15 +252,19 @@
             # falling back to the generic section if there's no match
             for section in urlmatch_credential_sections(conf, base_url):
                 try:
                     command = conf.get(section, "helper")
                 except KeyError:
                     # no helper configured
                     continue
-                yield command.decode(conf.encoding or sys.getdefaultencoding())
+                use_http_path = conf.get_boolean(section, "usehttppath", False)
+                yield (
+                    command.decode(conf.encoding or sys.getdefaultencoding()),
+                    use_http_path,
+                )
 
 
 class _CredentialKey(NamedTuple):
     protocol: str
     host: Optional[str]
     path: Optional[str]
 
@@ -375,15 +395,16 @@
                 new.password = input_noecho(prompt)
         except KeyboardInterrupt:
             raise CredentialNotFoundError("User cancelled prompt")
         return new
 
     def store(self, credential: "Credential", **kwargs):
         """Store the credential, if applicable to the helper"""
-        self[credential] = credential
+        if credential.protocol or credential.host or credential.path:
+            self[credential] = credential
 
     def erase(self, credential: "Credential", **kwargs):
         """Remove a matching credential, if any, from the helper’s storage"""
         try:
             del self[credential]
         except KeyError:
             pass
@@ -489,14 +510,16 @@
             if not self.protocol:
                 raise ValueError("protocol must be specified when using URL")
             port = f":{parsed.port}" if parsed.port is not None else ""
             hostname = parsed.hostname or ""
             self.host = self.host or f"{hostname}{port}"
             self.username = self.username or parsed.username
             self.password = self.password or parsed.password
+            if parsed.path:
+                self.path = self.path or parsed.path.lstrip("/")
 
     def __getitem__(self, key: object) -> str:
         if isinstance(key, str):
             try:
                 return getattr(self, key)
             except AttributeError:
                 pass
@@ -536,16 +559,16 @@
             path = ""
         return urlunparse((self.protocol or "", netloc, path, "", "", ""))
 
     @cached_property
     def helpers(self) -> List["CredentialHelper"]:
         url = self.url
         return [
-            GitCredentialHelper(command)
-            for command in GitCredentialHelper.get_matching_commands(url)
+            GitCredentialHelper(command, use_http_path=use_http_path)
+            for command, use_http_path in GitCredentialHelper.get_matching_commands(url)
         ]
 
     def fill(self, interactive: bool = True) -> "Credential":
         """Return a new credential with filled username and password."""
         if self.username and self.password:
             return Credential(**self)
```

### Comparing `scmrepo-1.0.0/src/scmrepo/git/objects.py` & `scmrepo-1.0.1/src/scmrepo/git/objects.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo/git/stash.py` & `scmrepo-1.0.1/src/scmrepo/git/stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo/progress.py` & `scmrepo-1.0.1/src/scmrepo/progress.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo/utils.py` & `scmrepo-1.0.1/src/scmrepo/utils.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo.egg-info/PKG-INFO` & `scmrepo-1.0.1/src/scmrepo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 1.0.0
+Version: 1.0.1
 Summary: SCM wrapper and fsspec filesystem for Git for use in DVC
 Home-page: https://github.com/iterative/scmrepo
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scmrepo-1.0.0/src/scmrepo.egg-info/SOURCES.txt` & `scmrepo-1.0.1/src/scmrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/src/scmrepo.egg-info/requires.txt` & `scmrepo-1.0.1/src/scmrepo.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 mypy==0.971
 pytest-test-utils==0.0.8
 pytest-asyncio==0.18.3
 mock==5.0.1
 paramiko==3.1.0
 types-certifi==2021.10.8.3
 types-mock==5.0.0.6
-types-paramiko==3.0.0.6
+types-paramiko==3.0.0.7
 
 [dev:python_version < "3.10" or sys_platform != "win32"]
 pytest-docker==0.12.0
 
 [tests]
 pytest==7.2.0
 pytest-sugar==0.9.5
@@ -35,11 +35,11 @@
 mypy==0.971
 pytest-test-utils==0.0.8
 pytest-asyncio==0.18.3
 mock==5.0.1
 paramiko==3.1.0
 types-certifi==2021.10.8.3
 types-mock==5.0.0.6
-types-paramiko==3.0.0.6
+types-paramiko==3.0.0.7
 
 [tests:python_version < "3.10" or sys_platform != "win32"]
 pytest-docker==0.12.0
```

### Comparing `scmrepo-1.0.0/tests/conftest.py` & `scmrepo-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/tests/test_dulwich.py` & `scmrepo-1.0.1/tests/test_dulwich.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/tests/test_fs.py` & `scmrepo-1.0.1/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/tests/test_git.py` & `scmrepo-1.0.1/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/tests/test_noscm.py` & `scmrepo-1.0.1/tests/test_noscm.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/tests/test_pygit2.py` & `scmrepo-1.0.1/tests/test_pygit2.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/tests/test_scmrepo.py` & `scmrepo-1.0.1/tests/test_scmrepo.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/tests/test_stash.py` & `scmrepo-1.0.1/tests/test_stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.0/tests/user.key` & `scmrepo-1.0.1/tests/user.key`

 * *Files identical despite different names*

