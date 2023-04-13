# Comparing `tmp/cmdlogtime-0.0.2.tar.gz` & `tmp/cmdlogtime-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdlogtime-0.0.2.tar", last modified: Mon Oct 24 18:41:39 2022, max compression
+gzip compressed data, was "cmdlogtime-0.0.3.tar", last modified: Thu Apr 13 18:28:08 2023, max compression
```

## Comparing `cmdlogtime-0.0.2.tar` & `cmdlogtime-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,636 @@
-drwxrwsr-x   0 jsteill  (73005484) regenerativebiology (694682113)        0 2022-10-24 18:41:39.006577 cmdlogtime-0.0.2/
--rw-rw-r--   0 jsteill  (73005484) regenerativebiology (694682113)     1068 2022-10-24 16:29:01.000000 cmdlogtime-0.0.2/LICENSE
--rw-rw-r--   0 jsteill  (73005484) regenerativebiology (694682113)       26 2022-10-24 14:54:40.000000 cmdlogtime-0.0.2/MANIFEST.in
--rwxrwxr-x   0 jsteill  (73005484) regenerativebiology (694682113)     3066 2022-10-24 18:41:39.005188 cmdlogtime-0.0.2/PKG-INFO
--rw-rw-r--   0 jsteill  (73005484) regenerativebiology (694682113)     2579 2022-10-24 16:28:56.000000 cmdlogtime-0.0.2/README.md
-drwxrwsr-x   0 jsteill  (73005484) regenerativebiology (694682113)        0 2022-10-24 18:41:38.966730 cmdlogtime-0.0.2/assets/
--rwxrwxr-x   0 jsteill  (73005484) regenerativebiology (694682113)     1170 2022-10-24 15:50:34.000000 cmdlogtime-0.0.2/assets/Readme.py
--rwxrwxr-x   0 jsteill  (73005484) regenerativebiology (694682113)     1118 2022-10-24 15:48:45.000000 cmdlogtime-0.0.2/assets/exampleCommandLine.txt
--rw-rw-r--   0 jsteill  (73005484) regenerativebiology (694682113)       96 2022-10-24 14:54:40.000000 cmdlogtime-0.0.2/pyproject.toml
--rwxrwxr-x   0 jsteill  (73005484) regenerativebiology (694682113)       38 2022-10-24 18:41:39.007724 cmdlogtime-0.0.2/setup.cfg
--rw-rw-r--   0 jsteill  (73005484) regenerativebiology (694682113)     1178 2022-10-24 18:41:11.000000 cmdlogtime-0.0.2/setup.py
-drwxrwsr-x   0 jsteill  (73005484) regenerativebiology (694682113)        0 2022-10-24 18:41:38.977641 cmdlogtime-0.0.2/src/
--rw-rw-r--   0 jsteill  (73005484) regenerativebiology (694682113)      199 2022-10-24 14:54:40.000000 cmdlogtime-0.0.2/src/__init__.py
-drwxrwsr-x   0 jsteill  (73005484) regenerativebiology (694682113)        0 2022-10-24 18:41:38.999344 cmdlogtime-0.0.2/src/cmdlogtime.egg-info/
--rwxrwxr-x   0 jsteill  (73005484) regenerativebiology (694682113)     3066 2022-10-24 18:41:38.000000 cmdlogtime-0.0.2/src/cmdlogtime.egg-info/PKG-INFO
--rwxrwxr-x   0 jsteill  (73005484) regenerativebiology (694682113)      286 2022-10-24 18:41:38.000000 cmdlogtime-0.0.2/src/cmdlogtime.egg-info/SOURCES.txt
--rwxrwxr-x   0 jsteill  (73005484) regenerativebiology (694682113)        1 2022-10-24 18:41:38.000000 cmdlogtime-0.0.2/src/cmdlogtime.egg-info/dependency_links.txt
--rwxrwxr-x   0 jsteill  (73005484) regenerativebiology (694682113)       11 2022-10-24 18:41:38.000000 cmdlogtime-0.0.2/src/cmdlogtime.egg-info/top_level.txt
--rwxrwxr-x   0 jsteill  (73005484) regenerativebiology (694682113)    12293 2022-10-24 18:36:49.000000 cmdlogtime-0.0.2/src/cmdlogtime.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.857075 cmdlogtime-0.0.3/
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.546733 cmdlogtime-0.0.3/.venv/
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.546892 cmdlogtime-0.0.3/.venv/lib/
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.547056 cmdlogtime-0.0.3/.venv/lib/python3.9/
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.562286 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.567736 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/_distutils_hack/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3686 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)       44 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/_distutils_hack/override.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.568566 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      368 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1198 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/__main__.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.574787 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      410 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     9643 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     9958 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/cache.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.583846 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/cli/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      132 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6350 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7741 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    28999 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      815 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2483 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2642 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    11097 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     8576 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    16884 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5347 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      116 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/cli/status_codes.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.596508 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3659 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7414 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1587 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2951 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     9206 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6806 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4993 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3431 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1713 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1149 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    27135 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    11331 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5598 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6866 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3216 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6233 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    13725 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/configuration.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.599597 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/distributions/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      864 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1245 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      667 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3900 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1205 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    13170 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/exceptions.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.602272 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/index/
+-rw-r--r--   0 johnsteill   (501) staff       (20)       30 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    18192 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    37294 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6557 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/index/sources.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.604642 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/locations/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4826 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5212 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5959 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1478 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      351 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/main.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.606644 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/metadata/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1471 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4750 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4248 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.616183 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/models/
+-rw-r--r--   0 johnsteill   (501) staff       (20)       63 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1001 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6555 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2629 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1092 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7472 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      770 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4613 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1947 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3962 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3614 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/models/wheel.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.621189 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/network/
+-rw-r--r--   0 johnsteill   (501) staff       (20)       50 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    11833 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2213 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6243 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7924 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    16247 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4072 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1703 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/network/xmlrpc.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.623766 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        0 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/__init__.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.627134 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/build/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        0 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1165 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1917 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1106 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3227 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5245 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     9999 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/freeze.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.629451 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/install/
+-rw-r--r--   0 johnsteill   (501) staff       (20)       51 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1396 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4177 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    29960 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    24850 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7061 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/pyproject.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.633993 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/req/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2983 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    16267 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    18000 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    32332 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7778 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4391 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/req/req_tracker.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    23468 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/req/req_uninstall.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.635131 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        0 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      563 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/base.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.636281 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/legacy/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        0 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    17934 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.640880 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        0 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5677 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    19976 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    24988 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5410 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7673 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2765 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6047 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    12085 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6484 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/self_outdated_check.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.658728 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        0 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1222 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1912 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5589 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      255 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3277 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3935 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1262 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1190 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1066 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6045 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      761 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3170 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5167 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      810 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    12133 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    23405 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1329 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2900 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3224 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/parallel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1106 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/pkg_resources.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5047 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    10036 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7950 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     9032 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1256 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3564 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6290 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/utils/wheel.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.663339 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/vcs/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      571 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2962 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    15431 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5043 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    11876 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    23086 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    11740 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_internal/wheel_builder.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.669594 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4760 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    25907 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/appdirs.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.675870 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      302 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1295 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4882 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      805 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.678562 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-r--r--   0 johnsteill   (501) staff       (20)       86 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4153 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      856 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      695 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    14149 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2533 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4070 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7091 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      690 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.680279 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/certifi/
+-rw-r--r--   0 johnsteill   (501) staff       (20)       62 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      255 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2840 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/certifi/core.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.702589 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3271 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    31254 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1757 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     9411 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3839 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5110 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.703401 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/cli/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        1 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2747 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3590 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1200 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1855 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1661 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3950 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    10510 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3749 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    13546 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1748 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    31621 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1747 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    20715 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1754 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    13838 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    25777 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    19643 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)   105697 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    99571 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    98776 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)   102498 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)   131180 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)   103312 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    95946 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5370 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3413 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2012 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    25481 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.704145 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/metadata/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        0 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    19474 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6136 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4309 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3774 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    12503 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2766 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      242 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/chardet/version.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.706853 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/colorama/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      239 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2522 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    10517 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1915 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5404 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6438 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/colorama/winterm.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.713349 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      581 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/__init__.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.715650 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/_backport/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      274 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/_backport/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      971 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/_backport/misc.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    25707 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/_backport/shutil.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    26854 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/_backport/sysconfig.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    92628 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/_backport/tarfile.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    41408 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    51059 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    21066 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    52100 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    14811 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4387 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    38962 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    10766 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    17180 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    59845 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    23391 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    41144 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    43628 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/distro.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.719710 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1160 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    16728 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/_ihatexml.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    32353 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/_inputstream.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    77040 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/_tokenizer.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.720949 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/_trie/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      109 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/_trie/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1013 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/_trie/_base.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1775 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/_trie/py.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4931 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/_utils.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    83464 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/constants.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.724377 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        0 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      919 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      286 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/base.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2945 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3643 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/lint.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    10588 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    26897 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1214 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/whitespace.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)   117186 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/html5parser.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    15759 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/serializer.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.725814 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treeadapters/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      679 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1715 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1776 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.728028 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treebuilders/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3592 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    14565 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treebuilders/base.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     8925 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    12836 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    14766 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.730525 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treewalkers/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5719 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7476 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treewalkers/base.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1413 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4551 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6357 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2309 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.734272 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/idna/
+-rw-r--r--   0 johnsteill   (501) staff       (20)       58 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3027 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      232 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    11849 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    42350 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1749 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)       21 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)   196224 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/idna/uts46data.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.736719 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/msgpack/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1118 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)       20 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/msgpack/_version.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1081 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6088 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    38026 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/msgpack/fallback.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.742138 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/packaging/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      726 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      562 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1128 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/packaging/_compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2022 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1824 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/packaging/_typing.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     9472 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5110 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    32208 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    29561 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4385 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    15974 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/packaging/version.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.746294 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pep517/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      130 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pep517/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3456 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pep517/build.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6082 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pep517/check.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4098 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pep517/colorlog.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      780 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pep517/compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1129 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pep517/dirtools.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6041 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pep517/envbuild.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.747146 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pep517/in_process/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      563 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pep517/in_process/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     8438 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pep517/in_process/_in_process.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2463 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pep517/meta.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    11044 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pep517/wrappers.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.748155 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pkg_resources/
+-rw-r--r--   0 johnsteill   (501) staff       (20)   108277 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      562 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pkg_resources/py31compat.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.750088 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/progress/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4857 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/progress/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2854 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/progress/bar.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1372 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/progress/counter.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1380 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/progress/spinner.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)   273394 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/pyparsing.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.757676 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4458 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      441 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1096 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    21548 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6496 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    10207 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      465 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2045 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    18430 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3173 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3578 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      757 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    34373 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      695 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    30137 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4188 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3005 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    30529 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/requests/utils.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.759831 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/resolvelib/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      537 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.760579 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/resolvelib/compat/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        0 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      156 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5638 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1364 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    17292 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4495 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    34159 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/six.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.765712 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/tenacity/
+-rw-r--r--   0 johnsteill   (501) staff       (20)    16528 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2833 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4555 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1307 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1154 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1784 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      739 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/tenacity/compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1280 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5463 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2435 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1729 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6017 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/tenacity/wait.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.767919 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/toml/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      747 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/toml/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    38954 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/toml/decoder.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     9964 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/toml/encoder.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      378 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/toml/ordered.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      701 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/toml/tz.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.772861 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2763 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    10811 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)       63 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    18748 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    37133 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.776103 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        0 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      957 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.777481 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        0 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    17649 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    13908 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    11034 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4160 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    16795 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    34303 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7097 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     8217 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     8579 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2440 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/filepost.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.778336 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      108 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.779187 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        0 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1417 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    32536 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/six.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.780093 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      757 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5679 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    19763 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5985 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    28203 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/response.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.785770 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/util/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1155 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4922 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1604 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      498 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4123 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3510 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    21396 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    16281 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6932 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    10003 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    13981 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5404 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      364 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/vendor.txt
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.787971 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/webencodings/
+-rw-r--r--   0 johnsteill   (501) staff       (20)    10579 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     8979 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1305 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6563 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4307 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.569808 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip-21.1.1.dist-info/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1090 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip-21.1.1.dist-info/LICENSE.txt
+-rw-r--r--   0 johnsteill   (501) staff       (20)      125 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip-21.1.1.dist-info/entry_points.txt
+-rw-r--r--   0 johnsteill   (501) staff       (20)        4 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pip-21.1.1.dist-info/top_level.txt
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.788390 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/
+-rw-r--r--   0 johnsteill   (501) staff       (20)   108202 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/__init__.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.789761 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        0 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    24701 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/appdirs.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.795385 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      736 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      562 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1128 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/_compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2022 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1812 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/_typing.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     9518 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4929 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    31944 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    24067 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1811 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    15470 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)   232055 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/_vendor/pyparsing.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.795814 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/extern/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2362 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/extern/__init__.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.561685 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/tests/
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.561842 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/tests/data/
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.796244 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/tests/data/my-test-package-source/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      104 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.807423 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7681 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      218 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_deprecation_warning.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.822555 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      250 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    20813 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     8572 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    14894 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    47437 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    18079 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/cmd.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.833143 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      799 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5562 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4913 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    35579 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/bdist_msi.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    21537 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    16030 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/bdist_wininst.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5767 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     8022 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    31685 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    17190 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     6232 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5637 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2776 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    13117 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    27482 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2822 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2603 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1298 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     8397 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2017 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      671 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    11712 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    19005 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7597 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4827 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     8876 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    16380 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      139 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3491 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7778 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    50421 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3577 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    10515 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    17784 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     8148 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    12832 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1969 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    30453 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    23540 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      455 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/py35compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      212 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4408 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    21349 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    12483 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    14696 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    20985 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    12514 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5133 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2388 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_imp.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.834319 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/
+-rw-r--r--   0 johnsteill   (501) staff       (20)        0 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    15130 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/ordered_set.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.839463 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/packaging/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      736 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      562 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1128 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/packaging/_compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2022 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1812 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/packaging/_typing.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     9509 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4917 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    31944 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    24067 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1811 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    15470 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)   232055 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/_vendor/pyparsing.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7077 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/archive_util.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    10280 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/build_meta.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.850325 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      551 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2381 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/alias.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    16604 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      900 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4415 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    13027 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     9473 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     8045 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/develop.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      960 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    85308 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    25079 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4705 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/install.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2203 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3875 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2593 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4946 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      468 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/register.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2128 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      658 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7818 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5051 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     9469 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/test.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      462 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/upload.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     7218 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    22020 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/config.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      949 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/dep_util.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5474 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/depends.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    40150 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/dist.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      524 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/errors.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1684 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/extension.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.850734 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/extern/
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2389 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     4873 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/glob.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3567 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/installer.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      812 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/launch.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2335 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/lib2to3_ex.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     5217 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/monkey.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    51126 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/msvc.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     3093 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/namespaces.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    40718 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/package_index.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      245 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/py34compat.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)    14151 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/sandbox.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     8565 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/ssl_support.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      941 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      144 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/version.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)     8288 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/wheel.py
+-rw-r--r--   0 johnsteill   (501) staff       (20)      714 2023-04-13 17:11:45.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools/windows_support.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.808683 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools-56.0.0.dist-info/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      239 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools-56.0.0.dist-info/dependency_links.txt
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2869 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools-56.0.0.dist-info/entry_points.txt
+-rw-r--r--   0 johnsteill   (501) staff       (20)       41 2023-04-13 17:11:46.000000 cmdlogtime-0.0.3/.venv/lib/python3.9/site-packages/setuptools-56.0.0.dist-info/top_level.txt
+-rw-r--r--   0 johnsteill   (501) staff       (20)     1068 2023-04-13 16:38:27.000000 cmdlogtime-0.0.3/LICENSE
+-rw-r--r--   0 johnsteill   (501) staff       (20)       26 2023-04-13 16:38:27.000000 cmdlogtime-0.0.3/MANIFEST.in
+-rw-r--r--   0 johnsteill   (501) staff       (20)      342 2023-04-13 18:28:08.857213 cmdlogtime-0.0.3/PKG-INFO
+-rw-r--r--   0 johnsteill   (501) staff       (20)     2579 2023-04-13 16:38:27.000000 cmdlogtime-0.0.3/README.md
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.851693 cmdlogtime-0.0.3/assets/
+-rwxr-xr-x   0 johnsteill   (501) staff       (20)     1170 2023-04-13 16:38:27.000000 cmdlogtime-0.0.3/assets/Readme.py
+-rwxr-xr-x   0 johnsteill   (501) staff       (20)     1118 2023-04-13 16:38:27.000000 cmdlogtime-0.0.3/assets/exampleCommandLine.txt
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.853372 cmdlogtime-0.0.3/cmdlogtime.egg-info/
+-rw-r--r--   0 johnsteill   (501) staff       (20)      342 2023-04-13 18:28:08.000000 cmdlogtime-0.0.3/cmdlogtime.egg-info/PKG-INFO
+-rw-r--r--   0 johnsteill   (501) staff       (20)    37457 2023-04-13 18:28:08.000000 cmdlogtime-0.0.3/cmdlogtime.egg-info/SOURCES.txt
+-rw-r--r--   0 johnsteill   (501) staff       (20)        1 2023-04-13 18:28:08.000000 cmdlogtime-0.0.3/cmdlogtime.egg-info/dependency_links.txt
+-rw-r--r--   0 johnsteill   (501) staff       (20)        4 2023-04-13 18:28:08.000000 cmdlogtime-0.0.3/cmdlogtime.egg-info/top_level.txt
+-rw-r--r--   0 johnsteill   (501) staff       (20)      438 2023-04-13 18:21:12.000000 cmdlogtime-0.0.3/pyproject.toml
+-rw-r--r--   0 johnsteill   (501) staff       (20)      380 2023-04-13 18:28:08.857909 cmdlogtime-0.0.3/setup.cfg
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.854190 cmdlogtime-0.0.3/src/
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.855502 cmdlogtime-0.0.3/src/UNKNOWN.egg-info/
+-rw-r--r--   0 johnsteill   (501) staff       (20)    37341 2023-04-13 18:19:57.000000 cmdlogtime-0.0.3/src/UNKNOWN.egg-info/SOURCES.txt
+-rw-r--r--   0 johnsteill   (501) staff       (20)        1 2023-04-13 18:19:56.000000 cmdlogtime-0.0.3/src/UNKNOWN.egg-info/dependency_links.txt
+-rw-r--r--   0 johnsteill   (501) staff       (20)       20 2023-04-13 18:19:56.000000 cmdlogtime-0.0.3/src/UNKNOWN.egg-info/top_level.txt
+-rw-r--r--   0 johnsteill   (501) staff       (20)      199 2023-04-13 16:38:27.000000 cmdlogtime-0.0.3/src/__init__.py
+drwxr-xr-x   0 johnsteill   (501) staff       (20)        0 2023-04-13 18:28:08.856745 cmdlogtime-0.0.3/src/cmdlogtime.egg-info/
+-rw-r--r--   0 johnsteill   (501) staff       (20)    37344 2023-04-13 18:21:23.000000 cmdlogtime-0.0.3/src/cmdlogtime.egg-info/SOURCES.txt
+-rw-r--r--   0 johnsteill   (501) staff       (20)        1 2023-04-13 18:21:23.000000 cmdlogtime-0.0.3/src/cmdlogtime.egg-info/dependency_links.txt
+-rw-r--r--   0 johnsteill   (501) staff       (20)       20 2023-04-13 18:21:23.000000 cmdlogtime-0.0.3/src/cmdlogtime.egg-info/top_level.txt
+-rwxr-xr-x   0 johnsteill   (501) staff       (20)    12394 2023-04-13 17:04:16.000000 cmdlogtime-0.0.3/src/cmdlogtime.py
```

### Comparing `cmdlogtime-0.0.2/LICENSE` & `cmdlogtime-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdlogtime-0.0.2/PKG-INFO` & `cmdlogtime-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: cmdlogtime
-Version: 0.0.2
-Summary: This package does command line processing, allows for logging, and keeps track of start, end, and elapsed time, along with a bunch of other stuff.
-Home-page: https://github.com/stewart-lab/cmdlogtime
-Author: Ron Stewart
-Author-email: rstewart@morgridge.org
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # How to use CMD Log time:
 
 ## Write a Command file that teaches cmdlogtime how to parse your input args:
 
 ```
 # first line is the description of what the program does.
 # subsequent lines list positional arguments (PA), then key-value (KV)arguments (KVA).
@@ -63,15 +53,7 @@
 if __name__ == "__main__":
     main()
 
 ```
 
 
 Reference Blog: https://towardsdatascience.com/an-end-to-end-guide-to-publish-your-python-package-bdb56639662c
-
-
-# CHANGELOG
-
-## Version 0.0.1 10/24/2022
-## Version 0.0.2 10/24/2022
-- Whitespace Errors & Docstring
-
```

### Comparing `cmdlogtime-0.0.2/assets/Readme.py` & `cmdlogtime-0.0.3/assets/Readme.py`

 * *Files identical despite different names*

### Comparing `cmdlogtime-0.0.2/assets/exampleCommandLine.txt` & `cmdlogtime-0.0.3/assets/exampleCommandLine.txt`

 * *Files identical despite different names*

### Comparing `cmdlogtime-0.0.2/src/cmdlogtime.py` & `cmdlogtime-0.0.3/src/cmdlogtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 #!/usr/bin/env python
-'''
-Help: see https://github.com/stewart-lab/cmdlogtime
-'''
-__author__='Ron Stewart'
-__author_email__='rstewart@morgridge.org'
 import argparse
 import os.path
 from pathlib import Path as ph
 import time
 import sys
 import pkg_resources
 
 # ---------------  FUNCTIONS -------------------
 def begin(command_line_def_file, write_msgs_to_stdout = 1):
+    print ("IN LOCAL")
     (start_time_secs, pretty_start_time) = get_time_and_pretty_time() 
     my_args = get_args(start_time_secs, pretty_start_time, command_line_def_file)
     addl_logfile = open_log_file(my_args["addl_logfile"])
     addl_logfile.write("Start: " + pretty_start_time +"\n")
     parms_logfile = open_log_file(my_args["parms_logfile"])
     script_logfile = open_log_file(my_args["script_logfile"])
     pkgs_logfile = open_log_file(my_args["pkgs_logfile"])
@@ -161,35 +157,37 @@
                 arg_defs = get_args_from_line(line)
                 tmp_name = arg_defs["name"]
                 if (arg_defs["name"].startswith("-")):
                     tmp_name = arg_defs["alt_name"].lstrip("-")
                 new_args[tmp_name] = args.__dict__[tmp_name]  # if it is a directory or file,  new_args[tmp_name] will be overlain below
                 if (arg_defs["is_dir"] == "1" or arg_defs["is_file"] == "1"):
                     if (args.__dict__[tmp_name]): #rms. I don't like this.  I think I need a different way to check that the flagged arg is NOT filled in, versus filled in incorrectly
-                        new_args[tmp_name] = os.path.abspath(args.__dict__[tmp_name])
+                	    new_args[tmp_name] = os.path.abspath(args.__dict__[tmp_name]) 	   
                 if (arg_defs["is_out_dir"]  == "1"):
-                    the_out_dir = new_args[tmp_name]
+                	the_out_dir = new_args[tmp_name]
                 if (arg_defs["check_dir"] == "1"):
-                    if (args.__dict__[tmp_name]):  
-                        #rms. I don't like this.  I think I need a different way to check that the flagged arg is NOT filled in, versus filled in incorrectly
-                        dirs_to_check.append(new_args[tmp_name])
+                    if (args.__dict__[tmp_name]):  #rms. I don't like this.  I think I need a different way to check that the flagged arg is NOT filled in, versus filled in incorrectly
+                	    dirs_to_check.append(new_args[tmp_name])
                 if (arg_defs["check_file"] == "1"):  # same goes for files, see rms comment 2 lines above.
-                    if (not args.__dict__[tmp_name].endswith("ZZZ")): #I think this is the correct logic... RMS.  magic number. Ugh.
-                        file_paths_to_check.append(new_args[tmp_name])
+                	if (not args.__dict__[tmp_name].endswith("ZZZ")): #I think this is the correct logic... RMS.  magic number. Ugh.
+                		file_paths_to_check.append(new_args[tmp_name])  
     for fpath in file_paths_to_check:
         assert os.path.isfile(fpath), fpath + " file does NOT exist!"
     new_args["start_time_secs"] = start_time_secs
     new_args["pretty_start_time"] = pretty_start_time
     assert(the_out_dir != "")
     if ("rerun_out_directory" in new_args and new_args["rerun_out_directory"] != None):
         the_out_dir = new_args["rerun_out_directory"]
         print("rerundir in cmdlogtime:", new_args["rerun_out_directory"])
     else:
         make_dir(the_out_dir)
-        the_out_dir = os.path.join(the_out_dir, pretty_start_time)
+        pretty_start_time_mod = pretty_start_time
+        if ("out_dir_suffix" in new_args and new_args["out_dir_suffix"] != "AAAAZZZZ"):
+            pretty_start_time_mod = pretty_start_time_mod + "_" + str(new_args["out_dir_suffix"])
+        the_out_dir = os.path.join(the_out_dir, pretty_start_time_mod)
     make_dir(the_out_dir)
     
     for dir in dirs_to_check:
         assert os.path.isdir(dir), dir + " directory does NOT exist!"
     
     new_args["out_dir"] = the_out_dir
     addl_logfile, parms_logfile, script_logfile, pkgs_logfile = build_log_files(the_out_dir, pretty_start_time)  #requires an out_dir RMS!!!
@@ -250,8 +248,8 @@
 
 # ----------------------------------   END LOGGING FUNCTIONS ----------------------
 def get_time_and_pretty_time():
     time_struct = time.localtime()
     time_secs = time.mktime(time_struct)  #need to use something besides time.mktime if want fractions of sec.
     #pretty_time = time.strftime("%d_%b_%Y_%H_%M_%S", time_struct)  #old format
     pretty_time = time.strftime("%Y_%m_%d_%H_%M_%S", time_struct)  #New format that will sort better
-    return(time_secs, pretty_time)         
+    return(time_secs, pretty_time)
```

