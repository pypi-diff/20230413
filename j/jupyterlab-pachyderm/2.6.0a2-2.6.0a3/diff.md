# Comparing `tmp/jupyterlab_pachyderm-2.6.0a2.tar.gz` & `tmp/jupyterlab_pachyderm-2.6.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_pachyderm-2.6.0a2.tar", last modified: Thu Mar 16 17:16:32 2023, max compression
+gzip compressed data, was "jupyterlab_pachyderm-2.6.0a3.tar", last modified: Thu Mar 30 20:29:36 2023, max compression
```

## Comparing `jupyterlab_pachyderm-2.6.0a2.tar` & `jupyterlab_pachyderm-2.6.0a3.tar`

### file list

```diff
@@ -1,159 +1,162 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.852850 jupyterlab_pachyderm-2.6.0a2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      702 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10706 2023-03-16 17:16:32.852850 jupyterlab_pachyderm-2.6.0a2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9679 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/babel.config.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/install.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jest.config.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.836850 jupyterlab_pachyderm-2.6.0a2/jupyter-config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.840850 jupyterlab_pachyderm-2.6.0a2/jupyter-config/nb-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jupyter-config/nb-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.840850 jupyterlab_pachyderm-2.6.0a2/jupyter-config/server-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jupyter-config/server-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.840850 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/dev_server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/env.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/filemanager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10822 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/handlers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.840850 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4388 2023-03-16 17:16:30.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.836850 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/schemas/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.844850 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-03-16 17:16:21.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-03-16 17:16:21.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-03-16 17:16:21.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4246 2023-03-16 17:16:21.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-03-16 17:16:21.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.844850 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-03-16 17:16:30.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-03-16 17:16:30.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-03-16 17:16:30.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-03-16 17:16:30.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-03-16 17:16:30.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-03-16 17:16:30.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15787 2023-03-16 17:16:30.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/747.4bacb4613a4fbdd0e8a7.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   154745 2023-03-16 17:16:30.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/869.6da4802142bf08400b17.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8177 2023-03-16 17:16:30.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/remoteEntry.052fe0d2650242075a28.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-03-16 17:16:21.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/style.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-03-16 17:16:30.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/log.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6004 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/mount_server_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/pachyderm.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.844850 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15825 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/tests/test_handlers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11081 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/tests/test_integrations.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.840850 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10706 2023-03-16 17:16:32.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4506 2023-03-16 17:16:32.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-16 17:16:32.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-16 17:16:06.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2023-03-16 17:16:32.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-03-16 17:16:32.000000 jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4246 2023-03-16 17:14:39.000000 jupyterlab_pachyderm-2.6.0a2/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.844850 jupyterlab_pachyderm-2.6.0a2/schema/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/schema/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/schema/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/schema/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/schema/telemetry.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      977 2023-03-16 17:16:32.856850 jupyterlab_pachyderm-2.6.0a2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.844850 jupyterlab_pachyderm-2.6.0a2/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/global.d.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/handler.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.836850 jupyterlab_pachyderm-2.6.0a2/src/plugins/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/examples/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/examples/__test__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/examples/__test__/examples.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/examples/examples.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/examples/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/help/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/help/__tests__/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/help/__tests__/__snapshots__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/help/__tests__/help.test.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/help/help.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/help/help.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/help/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4507 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/__tests__/mount.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.836850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Config/Config.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Config/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Config/__tests__/Config.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Config/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Config/hooks/useConfig.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Datum/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Datum/Datum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Datum/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Datum/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Datum/hooks/useDatum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/FullPageError/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/FullPageError/FullPageError.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/FullPageError/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4737 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Pipeline/Pipeline.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Pipeline/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1754 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.848850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Pipeline/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1658 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.852850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/SortableList/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/SortableList/ListMount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/SortableList/ListUnmount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3415 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/SortableList/SortableList.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.852850 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/SortableList/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14680 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/customFileBrowser.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      730 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7755 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/mount.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16886 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/mount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/mountDrive.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3658 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/pollMounts.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1648 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/types.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.852850 jupyterlab_pachyderm-2.6.0a2/src/plugins/telemetry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.852850 jupyterlab_pachyderm-2.6.0a2/src/plugins/telemetry/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/telemetry/__tests__/telemetry.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/telemetry/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/plugins/telemetry/telemetry.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/setupTests.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.852850 jupyterlab_pachyderm-2.6.0a2/src/utils/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.836850 jupyterlab_pachyderm-2.6.0a2/src/utils/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.852850 jupyterlab_pachyderm-2.6.0a2/src/utils/components/Circle/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/utils/components/Circle/Circle.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/utils/components/Circle/circle.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.852850 jupyterlab_pachyderm-2.6.0a2/src/utils/components/LoadingDots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/utils/components/LoadingDots/LoadingDots.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/utils/components/LoadingDots/loadingDots.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.852850 jupyterlab_pachyderm-2.6.0a2/src/utils/components/Svgs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/utils/components/Svgs/GenericError.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/utils/components/Svgs/KubernetesElephant.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/utils/components/Svgs/PachydermLogo.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/utils/components/Svgs/StatusWarning.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/utils/components/Svgs/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.852850 jupyterlab_pachyderm-2.6.0a2/src/utils/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/utils/hooks/usePreviousValue.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/utils/hooks/useSort.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/utils/icons.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/src/utils/testUtils.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.852850 jupyterlab_pachyderm-2.6.0a2/style/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/style/base.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.852850 jupyterlab_pachyderm-2.6.0a2/style/components/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1415 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/style/components/button.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/style/components/input.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-16 17:16:32.852850 jupyterlab_pachyderm-2.6.0a2/style/icons/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/style/icons/file.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/style/icons/info.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/style/icons/mount-logo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/style/icons/repo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/style/index.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/style/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-03-16 17:14:38.000000 jupyterlab_pachyderm-2.6.0a2/tsconfig.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      749 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10656 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9679 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/babel.config.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/install.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jest.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.934847 jupyterlab_pachyderm-2.6.0a3/jupyter-config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.942847 jupyterlab_pachyderm-2.6.0a3/jupyter-config/nb-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyter-config/nb-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.942847 jupyterlab_pachyderm-2.6.0a3/jupyter-config/server-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyter-config/server-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.942847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/dev_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/env.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/filemanager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11627 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/handlers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.942847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4388 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.934847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.946847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-03-30 20:29:24.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-03-30 20:29:24.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-03-30 20:29:24.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4246 2023-03-30 20:29:24.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-03-30 20:29:24.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.946847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15787 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/747.4bacb4613a4fbdd0e8a7.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   156706 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/869.aa9313c5e001be51e97f.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8237 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/remoteEntry.8cf7225b6da9d05077a7.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-03-30 20:29:24.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/style.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-03-30 20:29:34.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/log.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6171 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/mount_server_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/pachyderm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4355 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/pps_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.946847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.946847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16212 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/test_handlers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12887 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/test_integrations.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.942847 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10656 2023-03-30 20:29:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4592 2023-03-30 20:29:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-30 20:29:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-30 20:29:09.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-03-30 20:29:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-03-30 20:29:36.000000 jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4246 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/schema/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/schema/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/schema/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/schema/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/schema/telemetry.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      958 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/global.d.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/handler.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.938847 jupyterlab_pachyderm-2.6.0a3/src/plugins/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/examples/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/examples/__test__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/examples/__test__/examples.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/examples/examples.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/examples/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/__tests__/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/__tests__/__snapshots__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/__tests__/help.test.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/help.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/help.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/help/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4685 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/__tests__/mount.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.938847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/Config.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/__tests__/Config.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.950847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/hooks/useConfig.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/Datum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/hooks/useDatum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/FullPageError/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/FullPageError/FullPageError.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/FullPageError/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4996 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/Pipeline.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2234 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3255 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/ListMount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/ListUnmount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3415 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/SortableList.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14680 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/customFileBrowser.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      864 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7755 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/mount.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18827 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/mount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/mountDrive.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3658 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/pollMounts.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2430 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/types.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/telemetry/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/plugins/telemetry/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/telemetry/__tests__/telemetry.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/telemetry/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/plugins/telemetry/telemetry.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/setupTests.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/utils/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.938847 jupyterlab_pachyderm-2.6.0a3/src/utils/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Circle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Circle/Circle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Circle/circle.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.954847 jupyterlab_pachyderm-2.6.0a3/src/utils/components/LoadingDots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/LoadingDots/LoadingDots.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/LoadingDots/loadingDots.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/GenericError.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/KubernetesElephant.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/PachydermLogo.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/StatusWarning.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/src/utils/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/hooks/usePreviousValue.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/hooks/useSort.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/icons.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/src/utils/testUtils.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/style/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/base.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/style/components/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1415 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/components/button.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/components/input.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-30 20:29:36.958847 jupyterlab_pachyderm-2.6.0a3/style/icons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/icons/file.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/icons/info.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/icons/mount-logo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/icons/repo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/index.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/style/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-03-30 20:27:36.000000 jupyterlab_pachyderm-2.6.0a3/tsconfig.json
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/LICENSE` & `jupyterlab_pachyderm-2.6.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/MANIFEST.in` & `jupyterlab_pachyderm-2.6.0a3/MANIFEST.in`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 include LICENSE
 include *.md
 include pyproject.toml
 recursive-include jupyter-config *.json
+recursive-include jupyterlab_pachyderm *.ipynb
 
 exclude ci-requirements.txt
 exclude .circleci/*
 exclude cypress/*
 exclude cypress.json
 exclude Dockerfile
 exclude scripts/*
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/PKG-INFO` & `jupyterlab_pachyderm-2.6.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: jupyterlab_pachyderm
-Version: 2.6.0a2
+Version: 2.6.0a3
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: <4,>=3.7
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # jupyterlab-pachyderm
 
 [![CircleCI](https://circleci.com/gh/pachyderm/jupyterlab-pachyderm/tree/main.svg?style=shield&circle-token=23e1645bde6312d903e50be2dec7073bf0bcfbd0)](https://circleci.com/gh/pachyderm/jupyterlab-pachyderm/tree/main)
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/README.md` & `jupyterlab_pachyderm-2.6.0a3/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/__init__.py` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/_version.py` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/handlers.py` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/handlers.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,26 +4,31 @@
 import tornado
 
 from .env import PFS_MOUNT_DIR
 from .filemanager import PFSContentsManager
 from .log import get_logger
 from .pachyderm import MountInterface
 from .mount_server_client import MountServerClient
+from .pps_client import PPSClient
 
 
 # Frontend hard codes this in src/handler.ts
 NAMESPACE = "pachyderm"
 VERSION = "v2"
 
 
 class BaseHandler(APIHandler):
     @property
     def mount_client(self) -> MountInterface:
         return self.settings["pachyderm_mount_client"]
 
+    @property
+    def pps_client(self) -> PPSClient:
+        return self.settings["pachyderm_pps_client"]
+
 
 class ReposHandler(BaseHandler):
     # The following decorator should be present on all verb methods (head, get, post,
     # patch, put, delete, options) to ensure only authorized user can request the
     # Jupyter server
     @tornado.web.authenticated
     async def get(self):
@@ -261,18 +266,36 @@
         except Exception:
             get_logger().error("Mount server not running.")
             raise tornado.web.HTTPError(
                 status_code=500, reason=f"Mount server not running."
             )
 
 
+class PPSCreateHandler(BaseHandler):
+
+    @tornado.web.authenticated
+    async def get(self, path):
+        """Get the pipeline spec for the specified notebook."""
+        body = self.get_json_body()
+        response = await self.pps_client.generate(path, body)
+        self.finish(response)
+
+    @tornado.web.authenticated
+    async def put(self, path):
+        """Create the pipeline for the specified notebook."""
+        body = self.get_json_body()
+        response = await self.pps_client.create(path, body)
+        self.finish(response)
+
+
 def setup_handlers(web_app):
     get_logger().info(f"Using PFS_MOUNT_DIR={PFS_MOUNT_DIR}")
     web_app.settings["pfs_contents_manager"] = PFSContentsManager(PFS_MOUNT_DIR)
     web_app.settings["pachyderm_mount_client"] = MountServerClient(PFS_MOUNT_DIR)
+    web_app.settings["pachyderm_pps_client"] = PPSClient()
 
     _handlers = [
         ("/repos", ReposHandler),
         ("/mounts", MountsHandler),
         ("/_mount", MountHandler),
         ("/_unmount", UnmountHandler),
         ("/_commit", CommitHandler),
@@ -281,14 +304,15 @@
         (r"/_show_datum", ShowDatumHandler),
         (r"/pfs%s" % path_regex, PFSHandler),
         ("/datums", DatumsHandler),
         ("/config", ConfigHandler),
         ("/auth/_login", AuthLoginHandler),
         ("/auth/_logout", AuthLogoutHandler),
         ("/health", HealthHandler),
+        (r"/pps/_create%s" % path_regex, PPSCreateHandler),
     ]
 
     base_url = web_app.settings["base_url"]
     handlers = [
         (url_path_join(base_url, NAMESPACE, VERSION, endpoint), handler)
         for endpoint, handler in _handlers
     ]
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/package.json` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'2.6.0-alpha.3'"}*

```diff
@@ -65,19 +65,14 @@
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "npm"
             ]
         }
     },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.052fe0d2650242075a28.js",
-            "style": "./style"
-        },
         "disabledExtensions": [
             "jupyterlab-pachyderm:examples"
         ],
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_pachyderm"
@@ -132,9 +127,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.0-alpha.2"
+    "version": "2.6.0-alpha.3"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig` & `jupyterlab_pachyderm-2.6.0a3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.6.0-alpha.3'"}*

```diff
@@ -127,9 +127,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.0-alpha.2"
+    "version": "2.6.0-alpha.3"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/747.4bacb4613a4fbdd0e8a7.js` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/747.4bacb4613a4fbdd0e8a7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/869.6da4802142bf08400b17.js` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/869.aa9313c5e001be51e97f.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (self.webpackChunkjupyterlab_pachyderm = self.webpackChunkjupyterlab_pachyderm || []).push([
     [869], {
         1979: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => me
+                default: () => ue
             });
             var r = a(3279),
                 n = a.n(r),
                 l = a(4234);
             const s = n()((e => {
                     const t = e.target.getAttribute("data-testid");
                     t && (0, l.track)("notebook:click", {
@@ -20,18 +20,18 @@
                 i = {
                     id: "jupyterlab-pachyderm:telemetry",
                     autoStart: !0,
                     activate: e => {
                         (0, l.load)("20C6D2xFLRmyFTqtvYDEgNfwcRG", "https://pachyderm-dataplane.rudderstack.com"), window.document.onclick !== s && window.document.addEventListener("click", s)
                     }
                 };
-            var c = a(5705),
+            var c = a(9448),
                 o = a(6271),
                 m = a.n(o),
-                d = a(5510);
+                d = a(2884);
             const u = e => o.createElement("svg", Object.assign({
                 xmlns: "http://www.w3.org/2000/svg",
                 xmlnsXlink: "http://www.w3.org/1999/xlink",
                 viewBox: "0 0 100 170"
             }, e), o.createElement("defs", null, o.createElement("linearGradient", {
                 id: "pachydermLogo_svg__b",
                 x1: "90.51%",
@@ -301,18 +301,18 @@
                             command: h.openDocs
                         }, {
                             command: h.contactSupport
                         }], 20))
                     })(e, t)
                 }
             };
-            var f = a(1279),
-                E = a(4886),
-                _ = a(1258),
-                g = a(6591);
+            var f = a(8529),
+                E = a(6848),
+                _ = a(5613),
+                g = a(3215);
             const v = new g.LabIcon({
                     name: "jupyterlab-pachyderm:file",
                     svgstr: '<svg  viewBox="0 0 21 31" width="21px" height="31px" xmlns="http://www.w3.org/2000/svg">\n  <path d="M.85.001C.365.055-.003.491 0 1.008v28.19c0 .556.425 1.007.95 1.007h18.98c.524 0 .949-.45.949-1.007V6.608a1.04 1.04 0 00-.277-.713l-5.299-5.6a.923.923 0 00-.662-.294H.949a.895.895 0 00-.099 0zm1.048 2.014h11.705v4.698c0 .556.425 1.007.949 1.007h4.429v20.472H1.898V2.015zm13.603 1.332l2.234 2.36h-2.234v-2.36zM4.646 12.083a.949.949 0 00-.797.549c-.154.32-.135.704.05 1.007a.935.935 0 00.846.457h6.327a.94.94 0 00.833-.499 1.06 1.06 0 000-1.015.94.94 0 00-.833-.5H4.745a.895.895 0 00-.099 0zm0 4.698a.949.949 0 00-.797.549c-.154.32-.135.705.05 1.007a.935.935 0 00.846.458h11.389a.94.94 0 00.833-.5 1.06 1.06 0 000-1.015.94.94 0 00-.833-.499H4.745a.895.895 0 00-.099 0zm0 4.699a.949.949 0 00-.797.548c-.154.321-.135.705.05 1.007a.935.935 0 00.846.458h11.389a.94.94 0 00.833-.5 1.06 1.06 0 000-1.014.94.94 0 00-.833-.5H4.745a.895.895 0 00-.099 0z" fill="#582F6B" fill-rule="nonzero"/>\n</svg>\n'
                 }),
                 k = new g.LabIcon({
                     name: "jupyterlab-pachyderm:mount-logo",
                     svgstr: '<?xml version="1.0" encoding="UTF-8"?>\n<svg width="20px" height="20px" viewBox="0 0 20 20" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">\n    <defs>\n        <path d="M14,13 L14,17.041 L10,19 L6,17.041 L6,13 L10,14.8365 L14,13 Z M10,10 L14,12.0852339 L10,14 L6,12.0852339 L10,10 Z M10.9899912,1 L10.9899912,5.72256 L12.5999411,4.16117749 L14,5.51882251 L10.7000295,8.71882251 C10.3617408,9.04686292 9.83953975,9.08786797 9.455273,8.84183766 L9.37515866,8.78472348 L9.29997054,8.71882251 L6,5.51882251 L7.40005893,4.16117749 L9.01000884,5.72256 L9.01000884,1 L10.9899912,1 Z" id="path-1"></path>\n    </defs>\n    <g id="Icons" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">\n        <g id="Icon/notebook-mount/black">\n            <rect id="Bounding-Box"  class="jp-icon3" fill-opacity="0" fill="#FFFFFF" x="0" y="0" width="20" height="20"></rect>\n            <mask id="mask-2" fill="white">\n                <use xlink:href="#path-1"></use>\n            </mask>\n            <use id="Combined-Shape" fill="#926AA1" fill-rule="nonzero" xlink:href="#path-1"></use>\n            <g class="jp-icon3" id="Group" mask="url(#mask-2)" fill="#0F1012">\n                <g id="Color">\n                    <rect x="0" y="0" width="20" height="20"></rect>\n                </g>\n            </g>\n        </g>\n    </g>\n</svg>'
@@ -386,22 +386,23 @@
                                 command: e.command,
                                 category: "Pachyderm Examples",
                                 rank: e.rank
                             }))
                         })))(a, e, t))))
                     })))(e, t)
                 };
-            var C = a(6866),
-                z = a(5149),
-                M = a(3535),
-                S = a(1431),
-                L = a(1840),
-                B = a(3114);
+            var C = a(9239),
+                M = a(3619),
+                z = a(5643),
+                S = a(5679),
+                L = a(1431),
+                B = a(1840),
+                O = a(3114);
 
-            function O(e = "", t = "GET", a = null, r = "pachyderm/v2") {
+            function D(e = "", t = "GET", a = null, r = "pachyderm/v2") {
                 return n = this, l = void 0, i = function*() {
                     const n = _.ServerConnection.makeSettings(),
                         l = E.URLExt.join(n.baseUrl, r, e),
                         s = {
                             method: t,
                             body: a ? JSON.stringify(a) : void 0
                         };
@@ -448,15 +449,15 @@
                             e(n)
                         }))).then(a, r)
                     }
                     c((i = i.apply(n, l || [])).next())
                 }));
                 var n, l, s, i
             }
-            var D = function(e, t, a, r) {
+            var A = function(e, t, a, r) {
                 return new(a || (a = Promise))((function(n, l) {
                     function s(e) {
                         try {
                             c(r.next(e))
                         } catch (e) {
                             l(e)
                         }
@@ -475,33 +476,33 @@
                         e.done ? n(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                             e(t)
                         }))).then(s, i)
                     }
                     c((r = r.apply(e, t || [])).next())
                 }))
             };
-            class A {
+            class N {
                 constructor(e) {
                     this._rawData = {}, this._mounted = [], this._unmounted = [], this._status = {
                         code: 999,
                         message: ""
                     }, this._config = {
                         pachd_address: "",
                         cluster_status: "INVALID"
-                    }, this._mountedSignal = new L.Signal(this), this._unmountedSignal = new L.Signal(this), this._statusSignal = new L.Signal(this), this._configSignal = new L.Signal(this), this._dataPoll = new B.n_({
+                    }, this._mountedSignal = new B.Signal(this), this._unmountedSignal = new B.Signal(this), this._statusSignal = new B.Signal(this), this._configSignal = new B.Signal(this), this._dataPoll = new O.n_({
                         auto: !0,
-                        factory: () => D(this, void 0, void 0, (function*() {
+                        factory: () => A(this, void 0, void 0, (function*() {
                             return this.getData()
                         })),
                         frequency: {
                             interval: 2e3,
                             backoff: !0,
                             max: 5e3
                         }
-                    }), this.refresh = () => D(this, void 0, void 0, (function*() {
+                    }), this.refresh = () => A(this, void 0, void 0, (function*() {
                         yield this._dataPoll.refresh(), yield this._dataPoll.tick
                     })), this.updateData = e => {
                         JSON.stringify(e) !== JSON.stringify(this._rawData) && (this._rawData = e, this.mounted = Array.from(Object.values(e.mounted)), this.unmounted = Array.from(Object.values(e.unmounted)))
                     }, this.name = e
                 }
                 get mounted() {
                     return this._mounted
@@ -539,37 +540,37 @@
                 get configSignal() {
                     return this._configSignal
                 }
                 get poll() {
                     return this._dataPoll
                 }
                 getData() {
-                    return D(this, void 0, void 0, (function*() {
+                    return A(this, void 0, void 0, (function*() {
                         try {
-                            const e = yield O("config", "GET");
+                            const e = yield D("config", "GET");
                             if (this.config = e, "INVALID" !== e.cluster_status) {
-                                const e = yield O("mounts", "GET");
+                                const e = yield D("mounts", "GET");
                                 this.status = {
                                     code: 200
                                 }, this.updateData(e)
                             }
                         } catch (e) {
                             e instanceof _.ServerConnection.ResponseError && (this.status = {
                                 code: e.response.status,
                                 message: e.response.statusText
                             })
                         }
                     }))
                 }
             }
-            var N = a(6057),
-                F = a(8918);
-            class j {
+            var F = a(6057),
+                j = a(8918);
+            class H {
                 constructor(e) {
-                    this._fileChanged = new L.Signal(this), this._serverSettings = _.ServerConnection.makeSettings(), this._isDisposed = !1, this._registry = e
+                    this._fileChanged = new B.Signal(this), this._serverSettings = _.ServerConnection.makeSettings(), this._isDisposed = !1, this._registry = e
                 }
                 get name() {
                     return "mount-browser"
                 }
                 get fileChanged() {
                     return this._fileChanged
                 }
@@ -578,15 +579,15 @@
                 }
                 get isDisposed() {
                     return this._isDisposed
                 }
                 get(e, t) {
                     return a = this, r = void 0, l = function*() {
                         try {
-                            return yield O(E.URLExt.join("pfs", e), "GET")
+                            return yield D(E.URLExt.join("pfs", e), "GET")
                         } catch (e) {
                             return console.log("/pfs not found"), {
                                 name: "",
                                 path: "",
                                 last_modified: "2022-04-26T16:28:48.015858Z",
                                 created: "2022-04-26T16:28:48.015858Z",
                                 content: [],
@@ -654,18 +655,18 @@
                 restoreCheckpoint(e, t) {
                     return Promise.resolve()
                 }
                 deleteCheckpoint(e, t) {
                     return Promise.resolve()
                 }
                 dispose() {
-                    this.isDisposed || (this._isDisposed = !0, L.Signal.clearData(this))
+                    this.isDisposed || (this._isDisposed = !0, B.Signal.clearData(this))
                 }
             }
-            var H = function(e, t, a, r) {
+            var I = function(e, t, a, r) {
                 return new(a || (a = Promise))((function(n, l) {
                     function s(e) {
                         try {
                             c(r.next(e))
                         } catch (e) {
                             l(e)
                         }
@@ -684,15 +685,15 @@
                         e.done ? n(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                             e(t)
                         }))).then(s, i)
                     }
                     c((r = r.apply(e, t || [])).next())
                 }))
             };
-            const I = () => m().createElement("div", {
+            const P = () => m().createElement("div", {
                     className: "jp-dots-container"
                 }, m().createElement("div", {
                     className: "jp-dots-base",
                     role: "status",
                     "aria-label": "loading"
                 })),
                 W = e => o.createElement("svg", Object.assign({
@@ -2337,15 +2338,15 @@
                     fill: "#000",
                     filter: "url(#kubernetesElephant_svg__an)",
                     xlinkHref: "#kubernetesElephant_svg__ao"
                 }), o.createElement("use", {
                     fill: "#F69279",
                     xlinkHref: "#kubernetesElephant_svg__ao"
                 })))),
-                P = ({
+                U = ({
                     showConfig: e,
                     setShowConfig: t,
                     reposStatus: a,
                     updateConfig: r,
                     authConfig: n,
                     refresh: l
                 }) => {
@@ -2381,51 +2382,51 @@
                         }), [e, l]), {
                             addressField: c,
                             setAddressField: m,
                             errorMessage: d,
                             setErrorMessage: u,
                             shouldShowAddressInput: f,
                             setShouldShowAddressInput: E,
-                            updatePachdAddress: () => H(void 0, void 0, void 0, (function*() {
+                            updatePachdAddress: () => I(void 0, void 0, void 0, (function*() {
                                 i(!0);
                                 try {
                                     const e = c.trim();
                                     if (/^((grpc|grpcs|http|https|unix):\/\/)/.test(e)) {
-                                        const t = yield O("config", "PUT", v ? {
+                                        const t = yield D("config", "PUT", v ? {
                                             pachd_address: e,
                                             server_cas: v
                                         } : {
                                             pachd_address: e
                                         });
                                         "INVALID" === t.cluster_status ? u("Invalid address.") : (a(t), p("AUTH_ENABLED" === t.cluster_status))
                                     } else u("Cluster address should start with grpc://, grpcs://, http://, https:// or unix://")
                                 } catch (e) {
                                     u("Unable to connect to cluster."), console.log(e)
                                 }
                                 i(!1)
                             })),
-                            callLogin: () => H(void 0, void 0, void 0, (function*() {
+                            callLogin: () => I(void 0, void 0, void 0, (function*() {
                                 i(!0);
                                 try {
-                                    const e = yield O("auth/_login", "PUT");
+                                    const e = yield D("auth/_login", "PUT");
                                     if (e.auth_url) {
                                         const t = `width=500,height=500,left=${window.screenX+(window.outerWidth-500)/2},top=${window.screenY+(window.outerHeight-500)/2.5}`;
                                         window.open(e.auth_url, "", t)
                                     }
                                 } catch (e) {
                                     console.log(e)
                                 }
                                 setTimeout((() => {
                                     i(!1)
                                 }), 2e3)
                             })),
-                            callLogout: () => H(void 0, void 0, void 0, (function*() {
+                            callLogout: () => I(void 0, void 0, void 0, (function*() {
                                 i(!0);
                                 try {
-                                    yield O("auth/_logout", "PUT"), yield n()
+                                    yield D("auth/_logout", "PUT"), yield n()
                                 } catch (e) {
                                     console.log(e)
                                 }
                                 i(!1)
                             })),
                             shouldShowLogin: h,
                             loading: s,
@@ -2528,15 +2529,15 @@
                             paddingTop: "1rem"
                         }
                     }, v && m().createElement("div", {
                         className: "pachyderm-mount-list-item-status-icon",
                         style: {
                             position: "static"
                         }
-                    }, m().createElement(I, null)), m().createElement("span", {
+                    }, m().createElement(P, null)), m().createElement("span", {
                         className: "pachyderm-mount-config-address-error"
                     }, c)), m().createElement("div", {
                         className: "pachyderm-mount-config-advanced-settings-button"
                     }, m().createElement("button", {
                         "data-testid": "Config__advancedSettingsToggle",
                         className: "pachyderm-button-link",
                         onClick: () => {
@@ -2575,17 +2576,17 @@
                         className: "pachyderm-mount-config-graphic-container"
                     }, m().createElement(W, {
                         width: "230px",
                         height: "230px"
                     }))))
                 };
             var R = a(930),
-                U = a.n(R),
-                G = a(4439),
-                V = function(e, t, a, r) {
+                G = a.n(R),
+                V = a(4439),
+                $ = function(e, t, a, r) {
                     return new(a || (a = Promise))((function(n, l) {
                         function s(e) {
                             try {
                                 c(r.next(e))
                             } catch (e) {
                                 l(e)
                             }
@@ -2604,15 +2605,15 @@
                             e.done ? n(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                                 e(t)
                             }))).then(s, i)
                         }
                         c((r = r.apply(e, t || [])).next())
                     }))
                 };
-            const $ = ({
+            const T = ({
                 showDatum: e,
                 setShowDatum: t,
                 keepMounted: a,
                 setKeepMounted: r,
                 open: n,
                 pollRefresh: l,
                 currentDatumInfo: s,
@@ -2635,60 +2636,60 @@
                     } = ((e, t, a, r, n, l, s) => {
                         const [i, c] = (0, o.useState)(!1), [m, d] = (0, o.useState)(!1), [u, h] = (0, o.useState)(-1), [p, f] = (0, o.useState)({
                             id: "",
                             idx: -1,
                             num_datums: 0
                         }), [E, g] = (0, o.useState)(""), [v, k] = (0, o.useState)({}), [y, b] = (0, o.useState)(""), [w, x] = (0, o.useState)({});
                         (0, o.useEffect)((() => {
-                            e && -1 !== u && M()
+                            e && -1 !== u && z()
                         }), [u, e]), (0, o.useEffect)((() => {
                             if (e)
                                 if (t || S(), t && s) d(!0), h(s.curr_idx), f({
                                     id: "",
                                     idx: s.curr_idx,
                                     num_datums: s.num_datums
-                                }), g(z(s.input)), a(!1);
+                                }), g(M(s.input)), a(!1);
                                 else if ("string" == typeof w) g(w);
                             else {
                                 let e = {};
-                                e = 0 === Object.keys(w).length ? l : w, g(z(e)), k(e)
+                                e = 0 === Object.keys(w).length ? l : w, g(M(e)), k(e)
                             }
                         }), [e, l]);
                         const C = () => {
                                 let e = {};
                                 try {
                                     e = JSON.parse(E)
                                 } catch (t) {
                                     if (!(t instanceof SyntaxError)) throw t;
-                                    e = U().parse(E)
+                                    e = G().parse(E)
                                 }
                                 return e
                             },
-                            z = e => {
+                            M = e => {
                                 if (0 === Object.keys(e).length) return "";
                                 try {
                                     return JSON.parse(E), JSON.stringify(e, null, 2)
                                 } catch (t) {
-                                    return U().stringify(e, null, 2)
+                                    return G().stringify(e, null, 2)
                                 }
                             },
-                            M = () => V(void 0, void 0, void 0, (function*() {
+                            z = () => $(void 0, void 0, void 0, (function*() {
                                 c(!0);
                                 try {
-                                    const e = yield O(`_show_datum?idx=${u}`, "PUT");
+                                    const e = yield D(`_show_datum?idx=${u}`, "PUT");
                                     r(""), f(e)
                                 } catch (e) {
                                     console.log(e)
                                 }
                                 c(!1)
                             })),
-                            S = () => V(void 0, void 0, void 0, (function*() {
+                            S = () => $(void 0, void 0, void 0, (function*() {
                                 c(!0);
                                 try {
-                                    r(""), yield O("_unmount_all", "PUT"), r(""), yield n(), h(-1), f({
+                                    r(""), yield D("_unmount_all", "PUT"), r(""), yield n(), h(-1), f({
                                         id: "",
                                         idx: -1,
                                         num_datums: 0
                                     }), d(!1)
                                 } catch (e) {
                                     console.log(e)
                                 }
@@ -2698,35 +2699,35 @@
                             loading: i,
                             shouldShowCycler: m,
                             currDatum: p,
                             currIdx: u,
                             setCurrIdx: h,
                             inputSpec: E,
                             setInputSpec: g,
-                            callMountDatums: () => V(void 0, void 0, void 0, (function*() {
+                            callMountDatums: () => $(void 0, void 0, void 0, (function*() {
                                 c(!0), b("");
                                 try {
                                     const e = C(),
-                                        t = yield O("_mount_datums", "PUT", {
+                                        t = yield D("_mount_datums", "PUT", {
                                             input: e
                                         });
-                                    r(""), h(0), f(t), d(!0), g(z(e))
+                                    r(""), h(0), f(t), d(!0), g(M(e))
                                 } catch (e) {
-                                    console.log(e), e instanceof U().YAMLParseError ? b("Poorly formatted input spec- must be either YAML or JSON") : e instanceof _.ServerConnection.ResponseError ? b("Bad data in input spec") : b("Error mounting datums")
+                                    console.log(e), e instanceof G().YAMLParseError ? b("Poorly formatted input spec- must be either YAML or JSON") : e instanceof _.ServerConnection.ResponseError ? b("Bad data in input spec") : b("Error mounting datums")
                                 }
                                 c(!1)
                             })),
                             callUnmountAll: S,
                             errorMessage: y,
                             saveInputSpec: () => {
                                 try {
                                     const e = C();
-                                    (0, G.isEqual)(l, e) ? x({}): x(e || {})
+                                    (0, V.isEqual)(l, e) ? x({}): x(e || {})
                                 } catch (e) {
-                                    if (!(e instanceof U().YAMLParseError)) throw e;
+                                    if (!(e instanceof G().YAMLParseError)) throw e;
                                     x(E)
                                 }
                             },
                             initialInputSpec: v
                         }
                     })(e, a, r, n, l, i, s);
                 return m().createElement("div", {
@@ -2835,15 +2836,15 @@
                         p < h.num_datums - 1 && f(p + 1)
                     }
                 }, m().createElement(g.caretRightIcon.react, {
                     tag: "span",
                     className: "pachyderm-mount-datum-right"
                 }))))))
             };
-            var T = function(e, t, a, r) {
+            var Z = function(e, t, a, r) {
                 return new(a || (a = Promise))((function(n, l) {
                     function s(e) {
                         try {
                             c(r.next(e))
                         } catch (e) {
                             l(e)
                         }
@@ -2862,226 +2863,263 @@
                         e.done ? n(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                             e(t)
                         }))).then(s, i)
                     }
                     c((r = r.apply(e, t || [])).next())
                 }))
             };
-            const Z = ({
-                    setShowPipeline: e
+            const J = ({
+                    setShowPipeline: e,
+                    notebookPath: t,
+                    saveNotebookMetadata: a,
+                    metadata: r
                 }) => {
                     const {
-                        loading: t,
-                        pipelineName: a,
-                        setPipelineName: r,
-                        imageName: n,
-                        setImageName: l,
-                        inputSpec: s,
-                        setInputSpec: i,
-                        requirements: c,
-                        setRequirements: d,
-                        callCreatePipeline: u,
-                        errorMessage: h
-                    } = (() => {
-                        const [e, t] = (0, o.useState)(!1), [a, r] = (0, o.useState)(""), [n, l] = (0, o.useState)(""), [s, i] = (0, o.useState)(""), [c, m] = (0, o.useState)(""), [d, u] = (0, o.useState)("");
-                        return {
-                            loading: e,
-                            pipelineName: a,
-                            setPipelineName: r,
-                            imageName: n,
-                            setImageName: l,
-                            inputSpec: s,
-                            setInputSpec: i,
-                            requirements: c,
-                            setRequirements: m,
-                            callCreatePipeline: () => {
-                                return e = void 0, a = void 0, n = function*() {
-                                    let e, a;
-                                    t(!0), u("");
-                                    try {
-                                        e = U().parse(s)
-                                    } catch (t) {
-                                        if (!(t instanceof U().YAMLParseError)) throw t;
-                                        e = JSON.parse(s)
-                                    }
-                                    try {
-                                        a = U().parse(c)
-                                    } catch (e) {
-                                        if (!(e instanceof U().YAMLParseError)) throw e;
-                                        a = JSON.parse(c)
-                                    }
-                                    u("No action hooked up"), t(!1)
-                                }, new((r = void 0) || (r = Promise))((function(t, l) {
-                                    function s(e) {
-                                        try {
-                                            c(n.next(e))
-                                        } catch (e) {
-                                            l(e)
-                                        }
-                                    }
-
-                                    function i(e) {
-                                        try {
-                                            c(n.throw(e))
-                                        } catch (e) {
-                                            l(e)
-                                        }
-                                    }
-
-                                    function c(e) {
-                                        var a;
-                                        e.done ? t(e.value) : (a = e.value, a instanceof r ? a : new r((function(e) {
-                                            e(a)
-                                        }))).then(s, i)
+                        loading: n,
+                        pipelineName: l,
+                        setPipelineName: s,
+                        imageName: i,
+                        setImageName: c,
+                        inputSpec: d,
+                        setInputSpec: u,
+                        requirements: h,
+                        setRequirements: p,
+                        callCreatePipeline: f,
+                        callSavePipeline: E,
+                        errorMessage: v
+                    } = ((e, t, a) => {
+                        const [r, n] = (0, o.useState)(!1), [l, s] = (0, o.useState)(""), [i, c] = (0, o.useState)(""), [m, d] = (0, o.useState)(""), [u, h] = (0, o.useState)(""), [p, f] = (0, o.useState)("");
+                        (0, o.useEffect)((() => {
+                            var t, a, r;
+                            if (c(null !== (t = null == e ? void 0 : e.environments.default.image_tag) && void 0 !== t ? t : ""), s(null !== (a = null == e ? void 0 : e.metadata.name) && void 0 !== a ? a : ""), h(null !== (r = null == e ? void 0 : e.notebook.requirements) && void 0 !== r ? r : ""), null == e ? void 0 : e.run.input) {
+                                const t = JSON.parse(null == e ? void 0 : e.run.input);
+                                d(G().stringify(t))
+                            } else d("")
+                        }), [e]);
+                        const E = () => {
+                            let e;
+                            try {
+                                e = G().parse(m)
+                            } catch (t) {
+                                if (!(t instanceof G().YAMLParseError)) throw t;
+                                e = JSON.parse(m)
+                            }
+                            return {
+                                apiVersion: "sameproject.ml/v1alpha1",
+                                environments: {
+                                    default: {
+                                        image_tag: i
                                     }
-                                    c((n = n.apply(e, a || [])).next())
-                                }));
-                                var e, a, r, n
-                            },
-                            errorMessage: d
+                                },
+                                metadata: {
+                                    name: l,
+                                    version: "0.0.0"
+                                },
+                                notebook: {
+                                    requirements: u
+                                },
+                                run: {
+                                    name: l,
+                                    input: JSON.stringify(e)
+                                }
+                            }
+                        };
+                        return {
+                            loading: r,
+                            pipelineName: l,
+                            setPipelineName: s,
+                            imageName: i,
+                            setImageName: c,
+                            inputSpec: m,
+                            setInputSpec: d,
+                            requirements: u,
+                            setRequirements: h,
+                            callCreatePipeline: () => Z(void 0, void 0, void 0, (function*() {
+                                n(!0), f("");
+                                const e = E();
+                                try {
+                                    yield D(`pps/_create/${t}`, "PUT", e)
+                                } catch (e) {
+                                    if (!(e instanceof _.ServerConnection.ResponseError)) throw e;
+                                    f(e.message)
+                                }
+                                console.log("create pipeline called"), n(!1)
+                            })),
+                            callSavePipeline: () => Z(void 0, void 0, void 0, (function*() {
+                                const e = E();
+                                a(e), console.log("save pipeline called")
+                            })),
+                            errorMessage: p
                         }
-                    })();
+                    })(r, t, a);
                     return m().createElement("div", {
                         className: "pachyderm-mount-pipeline-base"
                     }, m().createElement("div", {
                         className: "pachyderm-mount-pipeline-back"
                     }, m().createElement("button", {
                         "data-testid": "Pipeline__back",
                         className: "pachyderm-button-link",
-                        onClick: () => T(void 0, void 0, void 0, (function*() {
-                            e(!1)
-                        }))
+                        onClick: () => {
+                            return t = void 0, a = void 0, n = function*() {
+                                e(!1)
+                            }, new((r = void 0) || (r = Promise))((function(e, l) {
+                                function s(e) {
+                                    try {
+                                        c(n.next(e))
+                                    } catch (e) {
+                                        l(e)
+                                    }
+                                }
+
+                                function i(e) {
+                                    try {
+                                        c(n.throw(e))
+                                    } catch (e) {
+                                        l(e)
+                                    }
+                                }
+
+                                function c(t) {
+                                    var a;
+                                    t.done ? e(t.value) : (a = t.value, a instanceof r ? a : new r((function(e) {
+                                        e(a)
+                                    }))).then(s, i)
+                                }
+                                c((n = n.apply(t, a || [])).next())
+                            }));
+                            var t, a, r, n
+                        }
                     }, "Back", " ", m().createElement(g.closeIcon.react, {
                         tag: "span",
                         className: "pachyderm-mount-icon-padding"
                     }))), m().createElement("span", {
                         className: "pachyderm-mount-pipeline-subheading"
                     }, "Notebook-to-Pipeline"), m().createElement("div", {
                         className: "pachyderm-pipeline-buttons"
                     }, m().createElement("button", {
                         "data-testid": "Pipeline__save",
                         className: "pachyderm-button-link",
-                        onClick: () => T(void 0, void 0, void 0, (function*() {}))
+                        onClick: E
                     }, "Save"), m().createElement("button", {
                         "data-testid": "Pipeline__create_pipeline",
                         className: "pachyderm-button-link",
-                        onClick: u
+                        onClick: f
                     }, "Create Pipeline")), m().createElement("span", {
                         className: "pachyderm-pipeline-error",
                         "data-testid": "Pipeline__errorMessage"
-                    }, h), m().createElement("div", {
+                    }, v), m().createElement("div", {
                         className: "pachyderm-pipeline-input-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-input-label",
                         htmlFor: "pipelineName"
                     }, "*Name:", "  "), m().createElement("input", {
                         className: "pachyderm-pipeline-input",
                         "data-testid": "Pipeline__inputPipelineName",
                         name: "pipelineName",
-                        value: a,
+                        value: l,
                         onChange: e => {
-                            r(e.target.value)
+                            s(e.target.value)
                         },
-                        disabled: t
+                        disabled: n
                     })), m().createElement("div", {
                         className: "pachyderm-pipeline-input-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-input-label",
                         htmlFor: "imageName"
                     }, "*Image:", "  "), m().createElement("input", {
                         className: "pachyderm-pipeline-input",
                         "data-testid": "Pipeline__inputImageName",
                         name: "imageName",
-                        value: n,
+                        value: i,
                         onChange: e => {
-                            l(e.target.value)
+                            c(e.target.value)
                         },
-                        disabled: t
+                        disabled: n
                     })), m().createElement("div", {
                         className: "pachyderm-pipeline-input-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-input-label",
                         htmlFor: "requirements"
                     }, "Requirements:", "  "), m().createElement("input", {
                         className: "pachyderm-pipeline-input",
                         "data-testid": "Pipeline__inputRequirements",
                         name: "requirements",
-                        value: c,
+                        value: h,
                         onChange: e => {
-                            d(e.target.value)
+                            p(e.target.value)
                         },
-                        disabled: t,
+                        disabled: n,
                         placeholder: "./requirements.txt"
                     })), m().createElement("div", {
                         className: "pachyderm-pipeline-textarea-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-textarea-label",
                         htmlFor: "inputSpec"
                     }, "Input Spec"), m().createElement("textarea", {
                         className: "pachyderm-pipeline-textarea pachyderm-input",
                         "data-testid": "Pipeline__inputSpecInput",
                         name: "inputSpec",
-                        value: s,
+                        value: d,
                         onChange: e => {
-                            i(e.target.value)
+                            u(e.target.value)
                         },
-                        disabled: t,
+                        disabled: n,
                         placeholder: "pfs:\n  repo: images\n  branch: dev\n  glob: /*\n"
                     })), m().createElement("div", {
                         className: "pachyderm-pipeline-spec-preview pachyderm-pipeline-textarea-wrapper"
                     }, m().createElement("label", {
                         className: "pachyderm-pipeline-preview-label"
                     }, "Pipeline Spec Preview: ", "  "), m().createElement("textarea", {
                         className: "pachyderm-pipeline-spec-preview-textarea",
                         style: {
                             backgroundColor: "#80808080"
                         },
                         "data-testid": "Pipeline__specPreview",
                         name: "specPreview",
-                        value: `name: ${a}\ntransform:\n  image: ${n}\ninput:\n${s.split("\n").map(((e,t,a)=>"  "+e)).join("\n")}\n`,
+                        value: `name: ${l}\ntransform:\n  image: ${i}\ninput:\n${d.split("\n").map(((e,t,a)=>"  "+e)).join("\n")}\n`,
                         readOnly: !0
                     })))
                 },
-                J = (e, t) => e > t ? 1 : e < t ? -1 : 0,
-                q = (e, t) => e - t;
-            var Y = a(4184),
-                X = a.n(Y);
-            const K = e => {
+                q = (e, t) => e > t ? 1 : e < t ? -1 : 0,
+                Y = (e, t) => e - t;
+            var X = a(4184),
+                K = a.n(X);
+            const Q = e => {
                 var {
                     children: t,
                     className: a,
                     color: r = "gray"
                 } = e, n = function(e, t) {
                     var a = {};
                     for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (a[r] = e[r]);
                     if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                         var n = 0;
                         for (r = Object.getOwnPropertySymbols(e); n < r.length; n++) t.indexOf(r[n]) < 0 && Object.prototype.propertyIsEnumerable.call(e, r[n]) && (a[r[n]] = e[r[n]])
                     }
                     return a
                 }(e, ["children", "className", "color"]);
-                const l = X()("jp-circle-base", a, {
+                const l = K()("jp-circle-base", a, {
                     "jp-circle-green": "green" === r,
                     "jp-circle-red": "red" === r,
                     "jp-circle-yellow": "yellow" === r,
                     "jp-circle-gray": "gray" === r
                 });
                 return m().createElement("div", Object.assign({
                     className: l
                 }, n), t)
             };
-            const Q = ["unmounting", "mounting", "error"],
-                ee = ({
+            const ee = ["unmounting", "mounting", "error"],
+                te = ({
                     item: e,
                     open: t,
                     updateData: a
                 }) => {
                     const [r, n] = (0, o.useState)(!1), l = e.branch, s = "Unmount", i = e.how_many_commits_behind;
                     return (0, o.useEffect)((() => {
-                        n(Q.includes(e.state))
+                        n(ee.includes(e.state))
                     }), [e]), m().createElement("li", {
                         className: "pachyderm-mount-sortableList-item",
                         "data-testid": "ListItem__repo"
                     }, m().createElement("span", {
                         className: "pachyderm-mount-list-item-name-branch-wrapper " + (r ? "pachyderm-mount-sortableList-disabled" : ""),
                         onClick: () => {
                             t(e.name)
@@ -3102,15 +3140,15 @@
                         className: "pachyderm-mount-list-item-action"
                     }, m().createElement("button", {
                         disabled: r,
                         onClick: () => {
                             return t = void 0, r = void 0, s = function*() {
                                 n(!0);
                                 try {
-                                    const t = yield O("_unmount", "PUT", {
+                                    const t = yield D("_unmount", "PUT", {
                                         mounts: [`${e.name}`]
                                     });
                                     a(t)
                                 } catch (e) {
                                     console.log("error unmounting repo")
                                 }
                             }, new((l = void 0) || (l = Promise))((function(e, a) {
@@ -3155,27 +3193,27 @@
                             case "unmounting":
                             case "mounting":
                                 a = "yellow";
                                 break;
                             case "error":
                                 a = "red"
                         }
-                        return r = t ? `${(0,G.capitalize)(e||"Unknown")}: ${t}` : (0, G.capitalize)(e || "Unknown"), m().createElement(m().Fragment, null, m().createElement(K, {
+                        return r = t ? `${(0,V.capitalize)(e||"Unknown")}: ${t}` : (0, V.capitalize)(e || "Unknown"), m().createElement(m().Fragment, null, m().createElement(Q, {
                             color: a,
                             className: "pachyderm-mount-list-item-status-circle"
                         }), m().createElement("div", {
                             "data-testid": "ListItem__statusIcon",
                             className: "pachyderm-mount-list-item-status-icon",
                             title: r
                         }, m().createElement(y.react, {
                             tag: "span"
                         })))
                     })(e.state, e.status))))
                 };
-            const te = ({
+            const ae = ({
                     item: e,
                     updateData: t,
                     mountedItems: a
                 }) => {
                     var r;
                     const [n, l] = (0, o.useState)(""), [s, i] = (0, o.useState)(!1), [c, d] = (0, o.useState)(!1), [u, h] = (0, o.useState)(!1), p = (null === (r = null == e ? void 0 : e.branches) || void 0 === r ? void 0 : r.length) > 0, f = "Mount";
                     return (0, o.useEffect)((() => {
@@ -3215,15 +3253,15 @@
                     }, m().createElement("button", {
                         disabled: c || s,
                         onClick: () => {
                             return a = void 0, r = void 0, s = function*() {
                                 d(!0);
                                 try {
                                     if (n) {
-                                        const a = yield O("_mount", "PUT", {
+                                        const a = yield D("_mount", "PUT", {
                                             mounts: [{
                                                 name: "master" === n ? `${e.project}_${e.repo}` : `${e.project}_${e.repo}_${n}`,
                                                 repo: e.repo,
                                                 branch: n,
                                                 project: e.project,
                                                 mode: "ro"
                                             }]
@@ -3285,20 +3323,20 @@
                     }, m().createElement("span", {
                         className: "pachyderm-mount-list-item-name",
                         title: `${e.project}_${e.repo}`
                     }, `${e.project}_${e.repo}`), m().createElement("span", {
                         className: "pachyderm-mount-list-item-branch"
                     }, "No read access")))
                 },
-                ae = {
+                re = {
                     name: "Name",
-                    func: J,
+                    func: q,
                     accessor: e => "name" in e ? e.name : `${e.project}_${e.repo}`
                 },
-                re = ({
+                ne = ({
                     open: e,
                     items: t,
                     updateData: a,
                     mountedItems: r,
                     type: n
                 }) => {
                     const l = "All projects",
@@ -3321,24 +3359,24 @@
                                 s((t => (e.name === t.name || e.reverse ? n(-1 * r) : n(1), e)))
                             }), [r]);
                             return {
                                 sortedData: (0, o.useMemo)((() => [...e].sort(((e, t) => r * l.func(l.accessor(e), l.accessor(t))))), [l, e, r]),
                                 reversed: -1 === r,
                                 setComparator: i,
                                 comparatorName: l.name,
-                                numberComparator: q,
-                                stringComparator: J
+                                numberComparator: Y,
+                                stringComparator: q
                             }
                         })({
                             data: t,
-                            initialSort: ae,
+                            initialSort: re,
                             initialDirection: 1
                         }),
                         p = (0, o.useCallback)((() => {
-                            u(ae)
+                            u(re)
                         }), [u]);
                     return m().createElement("div", {
                         className: "pachyderm-mount-sortableList"
                     }, "unmounted" === n && m().createElement("div", {
                         className: "pachyderm-mount-sortableList-projectFilter"
                     }, m().createElement("div", {
                         className: "pachyderm-mount-projectFilter-headerItem"
@@ -3359,27 +3397,27 @@
                     }, e)))))), m().createElement("div", {
                         className: "pachyderm-mount-sortableList-header"
                     }, m().createElement("div", {
                         className: "pachyderm-mount-sortableList-headerItem",
                         onClick: p
                     }, m().createElement("span", null, "Name"), m().createElement("span", null, h ? m().createElement(g.caretDownIcon.react, null) : m().createElement(g.caretUpIcon.react, null)))), m().createElement("ul", {
                         className: "pachyderm-mount-sortableList-content"
-                    }, d && d.map((t => "name" in t ? m().createElement(ee, {
+                    }, d && d.map((t => "name" in t ? m().createElement(te, {
                         item: t,
                         key: t.name,
                         open: e,
                         updateData: a
-                    }) : (i === t.project || i === l) && m().createElement(te, {
+                    }) : (i === t.project || i === l) && m().createElement(ae, {
                         item: t,
                         key: `${t.project}_${t.repo}`,
                         updateData: a,
                         mountedItems: r
                     })))))
                 },
-                ne = e => o.createElement("svg", Object.assign({
+                le = e => o.createElement("svg", Object.assign({
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 400,
                     height: 180,
                     viewBox: "320 -20 180 270",
                     xmlnsXlink: "http://www.w3.org/1999/xlink"
                 }, e), o.createElement("defs", null, o.createElement("path", {
                     id: "genericError_svg__b",
@@ -3894,56 +3932,56 @@
                     d: "M142.52 208.32 154 228.48h-22.96z"
                 }), o.createElement("path", {
                     d: "M607.04 74.706c1.237 0 2.24-1.12 2.24-2.501 0-.921-.747-2.7-2.24-5.34-1.493 2.64-2.24 4.419-2.24 5.34 0 1.381 1.003 2.5 2.24 2.5zm-5.6-11.2c1.237 0 2.24-1.12 2.24-2.501 0-.921-.747-2.7-2.24-5.34-1.493 2.64-2.24 4.419-2.24 5.34 0 1.381 1.003 2.5 2.24 2.5z",
                     stroke: "#26101A",
                     strokeWidth: 1.4,
                     fill: "#C3E5D7"
                 }))),
-                le = e => o.createElement("svg", Object.assign({
+                se = e => o.createElement("svg", Object.assign({
                     width: 20,
                     height: 20,
                     xmlns: "http://www.w3.org/2000/svg",
                     viewBox: "0 0 16 16"
                 }, e), o.createElement("g", {
                     fill: "none",
                     fillRule: "evenodd"
                 }, o.createElement("path", {
                     d: "M0 0h16v16H0z"
                 }), o.createElement("path", {
                     d: "M8 0a8 8 0 1 1 0 16A8 8 0 0 1 8 0Zm0 11.65a1.2 1.2 0 1 0 0 2.4 1.2 1.2 0 0 0 0-2.4Zm0-9.7a1.2 1.2 0 0 0-1.2 1.2v5.6a1.2 1.2 0 1 0 2.4 0v-5.6A1.2 1.2 0 0 0 8 1.95Z",
                     fill: "#BF444F"
                 }))),
-                se = ({
+                ie = ({
                     status: e
                 }) => m().createElement("div", {
                     className: "pachyderm-mount-base",
                     style: {
                         display: "flex",
                         flexDirection: "column",
                         alignItems: "center",
                         justifyContent: "center"
                     }
-                }, m().createElement("div", null, m().createElement(ne, {
+                }, m().createElement("div", null, m().createElement(le, {
                     width: "280px",
                     height: "130px"
                 })), m().createElement("div", {
                     style: {
                         display: "flex",
                         flexDirection: "row",
                         alignItems: "center",
                         paddingBottom: "1rem"
                     }
-                }, m().createElement(le, null), m().createElement("span", {
+                }, m().createElement(se, null), m().createElement("span", {
                     style: {
                         paddingLeft: ".5rem"
                     }
                 }, "Looks like there was an error")), m().createElement("div", {
                     "data-testid": "FullPageError__message"
                 }, e.message));
-            var ie = function(e, t, a, r) {
+            var ce = function(e, t, a, r) {
                 return new(a || (a = Promise))((function(n, l) {
                     function s(e) {
                         try {
                             c(r.next(e))
                         } catch (e) {
                             l(e)
                         }
@@ -3962,30 +4000,45 @@
                         e.done ? n(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                             e(t)
                         }))).then(s, i)
                     }
                     c((r = r.apply(e, t || [])).next())
                 }))
             };
-            const ce = "mount-browser:";
-            class oe {
-                constructor(e, t, a, r) {
-                    this._showConfig = !1, this._showConfigSignal = new L.Signal(this), this._readyPromise = Promise.resolve(), this._showDatum = !1, this._showPipeline = !1, this._keepMounted = !1, this._showDatumSignal = new L.Signal(this), this._repoViewInputSpec = {}, this._saveInputSpecSignal = new L.Signal(this), this._showPipelineSignal = new L.Signal(this), this.open = e => {
+            const oe = "mount-browser:",
+                me = "same_config";
+            class de {
+                constructor(e, t, a, r, n) {
+                    this._showConfig = !1, this._showConfigSignal = new B.Signal(this), this._readyPromise = Promise.resolve(), this._showDatum = !1, this._showPipeline = !1, this._keepMounted = !1, this._showDatumSignal = new B.Signal(this), this._repoViewInputSpec = {}, this._saveInputSpecSignal = new B.Signal(this), this._showPipelineSignal = new B.Signal(this), this._showMetadataSignal = new B.Signal(this), this.getActiveNotebook = () => this._tracker.currentWidget, this.handleNotebookChanged = (e, t) => ce(this, void 0, void 0, (function*() {
+                        var e;
+                        if (t) {
+                            yield t.sessionContext.ready;
+                            const a = null === (e = null == t ? void 0 : t.model) || void 0 === e ? void 0 : e.metadata.get(me);
+                            this._showMetadataSignal.emit(a), yield Promise.resolve()
+                        } else yield Promise.resolve()
+                    })), this.getNotebookMetadata = e => {
+                        var t;
+                        return null === (t = null == e ? void 0 : e.model) || void 0 === t ? void 0 : t.metadata.get(me)
+                    }, this.saveNotebookMetaData = e => {
+                        var t;
+                        const a = this.getActiveNotebook();
+                        null !== a ? (null === (t = null == a ? void 0 : a.model) || void 0 === t || t.metadata.set(me, e), console.log("notebook metadata saved")) : console.log("No active notebook")
+                    }, this.open = e => {
                         this._app.commands.execute("filebrowser:open-path", {
-                            path: ce + e
+                            path: oe + e
                         })
-                    }, this.refresh = (e, t) => ie(this, void 0, void 0, (function*() {
+                    }, this.refresh = (e, t) => ce(this, void 0, void 0, (function*() {
                         yield this._mountBrowser.model.refresh()
                     })), this.verifyBrowserPath = (e, t) => {
                         if (this._mountBrowser.model.path === this._mountBrowser.model.rootPath) return;
-                        const a = this._mountBrowser.model.path.split(ce)[1].split("/")[0];
+                        const a = this._mountBrowser.model.path.split(oe)[1].split("/")[0];
                         for (let e = 0; e < t.length; e++)
                             if (a === t[e].name) return;
                         this.open("")
-                    }, this.setShowDatum = e => ie(this, void 0, void 0, (function*() {
+                    }, this.setShowDatum = e => ce(this, void 0, void 0, (function*() {
                         e ? (this._datum.setHidden(!1), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this.saveMountedReposList()) : (this._datum.setHidden(!0), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), yield this.restoreMountedReposList()), this._mountBrowser.setHidden(!1), this._config.setHidden(!0), this._pipeline.setHidden(!0), this._fullPageError.setHidden(!0), this._showDatum = e, this._showDatumSignal.emit(e)
                     })), this.saveMountedReposList = () => {
                         const e = this._poller.mounted,
                             t = [];
                         for (let a = 0; a < e.length; a++) {
                             const r = {
                                 pfs: Object.assign(Object.assign(Object.assign(Object.assign(Object.assign({
@@ -4003,15 +4056,15 @@
                                 })
                             };
                             t.push(r)
                         }
                         0 === e.length ? this._repoViewInputSpec = {} : 1 === e.length ? this._repoViewInputSpec = t[0] : this._repoViewInputSpec = {
                             cross: t
                         }, this._saveInputSpecSignal.emit(this._repoViewInputSpec)
-                    }, this.restoreMountedReposList = () => ie(this, void 0, void 0, (function*() {
+                    }, this.restoreMountedReposList = () => ce(this, void 0, void 0, (function*() {
                         const e = [];
                         if (Object.prototype.hasOwnProperty.call(this._repoViewInputSpec, "cross") && Array.isArray(this._repoViewInputSpec.cross))
                             for (let t = 0; t < this._repoViewInputSpec.cross.length; t++) {
                                 const a = this._repoViewInputSpec.cross[t].pfs;
                                 e.push({
                                     name: a.name ? a.name : a.repo,
                                     repo: a.repo,
@@ -4025,15 +4078,15 @@
                                     name: t.name ? t.name : t.repo,
                                     repo: t.repo,
                                     project: t.project ? t.project : "default",
                                     branch: t.branch ? t.branch : "master",
                                     mode: "ro"
                                 })
                             } if (e.length > 0) {
-                            const t = yield O("_mount", "PUT", {
+                            const t = yield D("_mount", "PUT", {
                                 mounts: e
                             });
                             this._poller.updateData(t)
                         }
                         this.open("")
                     })), this.setShowPipeline = e => {
                         e ? (this._pipeline.setHidden(!1), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0)) : (this._pipeline.setHidden(!0), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1)), this._mountBrowser.setHidden(!0), this._config.setHidden(!0), this._datum.setHidden(!0), this._fullPageError.setHidden(!0), this._showPipeline = e, this._showPipelineSignal.emit(e)
@@ -4041,34 +4094,34 @@
                         this._keepMounted = e
                     }, this.setShowConfig = e => {
                         e ? (this._config.setHidden(!1), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._mountBrowser.setHidden(!0)) : (this._config.setHidden(!0), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), this._mountBrowser.setHidden(!1)), this._datum.setHidden(!0), this._pipeline.setHidden(!0), this._fullPageError.setHidden(!0), this._showConfig = e, this._showConfigSignal.emit(e)
                     }, this.setShowFullPageError = e => {
                         e ? (this._fullPageError.setHidden(!1), this._config.setHidden(!0), this._datum.setHidden(!0), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._mountBrowser.setHidden(!0), this._pipeline.setHidden(!0)) : (this._fullPageError.setHidden(!0), this._config.setHidden(!1), this._datum.setHidden(!1), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), this._mountBrowser.setHidden(!1), this._pipeline.setHidden(!1))
                     }, this.updateConfig = e => {
                         this._poller.config = e
-                    }, this.setup = () => ie(this, void 0, void 0, (function*() {
+                    }, this.setup = () => ce(this, void 0, void 0, (function*() {
                         if (yield this._poller.refresh(), 500 === this._poller.status.code) this.setShowFullPageError(!0);
                         else if (this.setShowConfig("INVALID" === this._poller.config.cluster_status || 200 !== this._poller.status.code), 200 === this._poller.status.code) try {
-                            const e = yield O("datums", "GET");
+                            const e = yield D("datums", "GET");
                             e.num_datums > 0 && (this._keepMounted = !0, this._currentDatumInfo = e, yield this.setShowDatum(!0))
                         } catch (e) {
                             console.log(e)
                         }
                         this._loader.setHidden(!0)
-                    })), this._app = e, this._poller = new A("PollMounts"), this._repoViewInputSpec = {}, this._poller.configSignal.connect(((e, t) => {
+                    })), this._app = e, this._poller = new N("PollMounts"), this._repoViewInputSpec = {}, this._tracker = n, this._poller.configSignal.connect(((e, t) => {
                         "INVALID" !== t.cluster_status || this._showConfig || this.setShowConfig(!0)
                     })), this._poller.statusSignal.connect(((e, t) => {
                         500 === t.code && this.setShowFullPageError(!0), 401 !== t.code || this._showConfig || this.setShowConfig(!0)
                     })), this._readyPromise = this.setup(), this._config = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._showConfigSignal
                     }, ((e, t) => m().createElement(d.UseSignal, {
                         signal: this._poller.configSignal
                     }, ((e, a) => m().createElement(d.UseSignal, {
                         signal: this._poller.statusSignal
-                    }, ((e, r) => m().createElement(P, {
+                    }, ((e, r) => m().createElement(U, {
                         showConfig: t || this._showConfig,
                         setShowConfig: this.setShowConfig,
                         reposStatus: r ? r.code : this._poller.status.code,
                         updateConfig: this.updateConfig,
                         authConfig: a || this._poller.config,
                         refresh: this._poller.refresh
                     })))))))), this._config.addClass("pachyderm-mount-config-wrapper"), this._mountedList = d.ReactWidget.create(m().createElement(d.UseSignal, {
@@ -4101,94 +4154,102 @@
                         className: "pachyderm-mount-icon-padding"
                     })), m().createElement("button", {
                         className: "pachyderm-button-link",
                         onClick: () => this.setShowConfig(!0)
                     }, "Config", " ", m().createElement(g.settingsIcon.react, {
                         tag: "span",
                         className: "pachyderm-mount-icon-padding"
-                    })))), m().createElement(re, {
+                    })))), m().createElement(ne, {
                         open: this.open,
                         items: t || this._poller.mounted,
                         updateData: this._poller.updateData,
                         mountedItems: [],
                         type: "mounted"
                     }))))), this._mountedList.addClass("pachyderm-mount-react-wrapper"), this._unmountedList = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._poller.unmountedSignal
                     }, ((e, t) => m().createElement("div", {
                         className: "pachyderm-mount-base"
                     }, m().createElement("div", {
                         className: "pachyderm-mount-base-title"
-                    }, "Unmounted Repositories"), m().createElement(re, {
+                    }, "Unmounted Repositories"), m().createElement(ne, {
                         open: this.open,
                         items: t || this._poller.unmounted,
                         updateData: this._poller.updateData,
                         mountedItems: this._poller.mounted,
                         type: "unmounted"
                     }))))), this._unmountedList.addClass("pachyderm-mount-react-wrapper"), this._datum = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._showDatumSignal
                     }, ((e, t) => m().createElement(d.UseSignal, {
                         signal: this._saveInputSpecSignal
-                    }, ((e, a) => m().createElement($, {
+                    }, ((e, a) => m().createElement(T, {
                         showDatum: t || this._showDatum,
                         setShowDatum: this.setShowDatum,
                         keepMounted: this._keepMounted,
                         setKeepMounted: this.setKeepMounted,
                         open: this.open,
                         pollRefresh: this._poller.refresh,
                         currentDatumInfo: this._currentDatumInfo,
                         repoViewInputSpec: a || this._repoViewInputSpec
-                    })))))), this._datum.addClass("pachyderm-mount-datum-wrapper"), this._pipeline = d.ReactWidget.create(m().createElement(Z, {
-                        setShowPipeline: this.setShowPipeline
-                    })), this._pipeline.addClass("pachyderm-mount-pipeline-wrapper"), this._loader = d.ReactWidget.create(m().createElement(I, null)), this._loader.addClass("pachyderm-mount-react-wrapper"), this._fullPageError = d.ReactWidget.create(m().createElement(d.UseSignal, {
+                    })))))), this._datum.addClass("pachyderm-mount-datum-wrapper"), this._pipeline = d.ReactWidget.create(m().createElement(d.UseSignal, {
+                        signal: this._showMetadataSignal
+                    }, ((e, t) => {
+                        var a, r, n;
+                        return m().createElement(m().Fragment, null, m().createElement(J, {
+                            setShowPipeline: this.setShowPipeline,
+                            notebookPath: null === (n = null === (r = null === (a = this.getActiveNotebook()) || void 0 === a ? void 0 : a.sessionContext) || void 0 === r ? void 0 : r.session) || void 0 === n ? void 0 : n.path,
+                            saveNotebookMetadata: this.saveNotebookMetaData,
+                            metadata: t
+                        }))
+                    }))), this._pipeline.addClass("pachyderm-mount-pipeline-wrapper"), this._loader = d.ReactWidget.create(m().createElement(P, null)), this._loader.addClass("pachyderm-mount-react-wrapper"), this._fullPageError = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._poller.statusSignal
-                    }, ((e, t) => m().createElement(se, {
+                    }, ((e, t) => m().createElement(ie, {
                         status: t || this._poller.status
                     })))), this._fullPageError.addClass("pachyderm-mount-react-wrapper"), this._mountBrowser = ((e, t, a) => {
                         var r;
-                        const n = new j(e.docRegistry);
+                        const n = new H(e.docRegistry);
                         t.services.contents.addDrive(n);
                         const l = a.createFileBrowser("jupyterlab-pachyderm-browser", {
                             driveName: n.name,
                             state: null,
                             refreshInterval: 1e4
                         });
                         try {
                             const e = l.toolbar.node.childNodes[0],
                                 a = l.toolbar.node.childNodes[1];
                             l.toolbar.node.removeChild(e), l.toolbar.node.removeChild(a);
                             const n = l.layout.widgets || [],
-                                s = n.find((e => e instanceof M.BreadCrumbs));
+                                s = n.find((e => e instanceof z.BreadCrumbs));
                             if (s) {
                                 null === (r = s.node.querySelector('svg[data-icon="ui-components:folder"]')) || void 0 === r || r.replaceWith("/ pfs");
                                 const e = s.node.querySelector('span[title="~/extension-wd"]');
                                 e && (e.className = "jp-BreadCrumbs-item")
                             }
-                            const i = n.find((e => e instanceof M.DirListing));
+                            const i = n.find((e => e instanceof z.DirListing));
                             if (i) {
-                                const e = new N.CommandRegistry;
+                                const e = new F.CommandRegistry;
                                 e.addCommand("file-open", {
                                     label: "Open",
                                     icon: "fa fa-folder",
                                     mnemonic: 0,
                                     execute: () => {
-                                        (0, F.each)(l.selectedItems(), (e => {
+                                        (0, j.each)(l.selectedItems(), (e => {
                                             t.openOrReveal(e.path)
                                         }))
                                     }
                                 }), e.addCommand("copy-path", {
                                     label: "Copy Path",
                                     icon: "fa fa-file",
                                     mnemonic: 0,
                                     execute: () => {
-                                        (0, F.each)(l.selectedItems(), (e => {
-                                            d.Clipboard.copyToSystem(e.path.replace(ce, "/pfs/"))
+                                        (0, j.each)(l.selectedItems(), (e => {
+                                            d.Clipboard.copyToSystem(e.path.replace(oe, "/pfs/"))
                                         }))
                                     }
                                 });
-                                const a = new S.Menu({
+                                const a = new L.Menu({
                                     commands: e
                                 });
                                 a.addItem({
                                     command: "file-open"
                                 }), a.addItem({
                                     command: "copy-path"
                                 }), i.node.getElementsByClassName("jp-DirListing-content")[0].addEventListener("contextmenu", (e => {
@@ -4198,15 +4259,15 @@
                                     a.open(t, r)
                                 }))
                             }
                         } catch (e) {
                             console.log("Failed to edit default browser.")
                         }
                         return l
-                    })(e, t, a), this._poller.mountedSignal.connect(this.verifyBrowserPath), this._poller.mountedSignal.connect(this.refresh), this._poller.unmountedSignal.connect(this.refresh), this._panel = new S.SplitPanel, this._panel.orientation = "vertical", this._panel.spacing = 0, this._panel.title.icon = k, this._panel.title.caption = "Pachyderm Mount", this._panel.id = "pachyderm-mount", this._panel.addWidget(this._mountedList), this._panel.addWidget(this._unmountedList), this._panel.addWidget(this._datum), this._panel.addWidget(this._pipeline), this._panel.addWidget(this._mountBrowser), this._panel.setRelativeSizes([1, 1, 3, 3]), this._panel.addWidget(this._loader), this._panel.addWidget(this._config), this._panel.addWidget(this._fullPageError), this._config.setHidden(!0), this._fullPageError.setHidden(!0), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._datum.setHidden(!0), this._pipeline.setHidden(!0), this._mountBrowser.setHidden(!0), window.addEventListener("resize", (() => {
+                    })(e, t, a), this._poller.mountedSignal.connect(this.verifyBrowserPath), this._poller.mountedSignal.connect(this.refresh), this._poller.unmountedSignal.connect(this.refresh), this._tracker.currentChanged.connect(this.handleNotebookChanged, this), this._panel = new L.SplitPanel, this._panel.orientation = "vertical", this._panel.spacing = 0, this._panel.title.icon = k, this._panel.title.caption = "Pachyderm Mount", this._panel.id = "pachyderm-mount", this._panel.addWidget(this._mountedList), this._panel.addWidget(this._unmountedList), this._panel.addWidget(this._datum), this._panel.addWidget(this._pipeline), this._panel.addWidget(this._mountBrowser), this._panel.setRelativeSizes([1, 1, 3, 3]), this._panel.addWidget(this._loader), this._panel.addWidget(this._config), this._panel.addWidget(this._fullPageError), this._config.setHidden(!0), this._fullPageError.setHidden(!0), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._datum.setHidden(!0), this._pipeline.setHidden(!0), this._mountBrowser.setHidden(!0), window.addEventListener("resize", (() => {
                         this._panel.update()
                     })), r.add(this._panel, "jupyterlab-pachyderm"), e.shell.add(this._panel, "left", {
                         rank: 100
                     })
                 }
                 get mountedRepos() {
                     return this._poller.poll.tick, this._poller.mounted
@@ -4217,16 +4278,16 @@
                 get layout() {
                     return this._panel
                 }
                 get ready() {
                     return this._readyPromise
                 }
             }
-            const me = [{
+            const ue = [{
                 id: "jupyterlab-pachyderm:mount",
                 autoStart: !0,
-                requires: [z.IDocumentManager, M.IFileBrowserFactory, C.ILayoutRestorer],
-                activate: (e, t, a, r) => new oe(e, t, a, r)
+                requires: [M.IDocumentManager, z.IFileBrowserFactory, C.ILayoutRestorer, S.INotebookTracker],
+                activate: (e, t, a, r, n) => new de(e, t, a, r, n)
             }, i, p, x]
         }
     }
 ]);
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/remoteEntry.052fe0d2650242075a28.js` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/remoteEntry.8cf7225b6da9d05077a7.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, l, i, u, d, f, s, p, c, h, v, m, b, y = {
+    var e, r, t, a, n, o, l, u, i, d, f, s, p, c, h, b, v, m, y = {
             6334: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(371), t.e(869)]).then((() => () => t(1979))),
                         "./extension": () => Promise.all([t.e(371), t.e(869)]).then((() => () => t(1979))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -49,52 +49,52 @@
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         67: "9d3e2934cfe0e102619e",
         371: "8ac933b7fbb0f688b6f4",
         486: "003d1d2cc9cc6927471e",
         676: "95f9b834e9f9b133c00b",
         747: "4bacb4613a4fbdd0e8a7",
-        869: "6da4802142bf08400b17"
+        869: "aa9313c5e001be51e97f"
     } [e] + ".js?v=" + {
         67: "9d3e2934cfe0e102619e",
         371: "8ac933b7fbb0f688b6f4",
         486: "003d1d2cc9cc6927471e",
         676: "95f9b834e9f9b133c00b",
         747: "4bacb4613a4fbdd0e8a7",
-        869: "6da4802142bf08400b17"
+        869: "aa9313c5e001be51e97f"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyterlab-pachyderm:", j.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
-            var l, i;
+            var l, u;
             if (void 0 !== n)
-                for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
-                    var f = u[d];
+                for (var i = document.getElementsByTagName("script"), d = 0; d < i.length; d++) {
+                    var f = i[d];
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
                         l = f;
                         break
                     }
                 }
-            l || (i = !0, (l = document.createElement("script")).charset = "utf-8", l.timeout = 120, j.nc && l.setAttribute("nonce", j.nc), l.setAttribute("data-webpack", r + n), l.src = t), e[t] = [a];
+            l || (u = !0, (l = document.createElement("script")).charset = "utf-8", l.timeout = 120, j.nc && l.setAttribute("nonce", j.nc), l.setAttribute("data-webpack", r + n), l.src = t), e[t] = [a];
             var s = (r, a) => {
                     l.onerror = l.onload = null, clearTimeout(p);
                     var n = e[t];
                     if (delete e[t], l.parentNode && l.parentNode.removeChild(l), n && n.forEach((e => e(a))), r) return r(a)
                 },
                 p = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: l
                 }), 12e4);
-            l.onerror = s.bind(null, l.onerror), l.onload = s.bind(null, l.onload), i && document.head.appendChild(l)
+            l.onerror = s.bind(null, l.onerror), l.onload = s.bind(null, l.onload), u && document.head.appendChild(l)
         }
     }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -106,25 +106,25 @@
             a || (a = []);
             var n = r[t];
             if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
                 if (a.push(n), e[t]) return e[t];
                 j.o(j.S, t) || (j.S[t] = {});
                 var o = j.S[t],
                     l = "jupyterlab-pachyderm",
-                    i = (e, r, t, a) => {
+                    u = (e, r, t, a) => {
                         var n = o[e] = o[e] || {},
-                            i = n[r];
-                        (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (n[r] = {
+                            u = n[r];
+                        (!u || !u.loaded && (!a != !u.eager ? a : l > u.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
-                    u = [];
-                return "default" === t && (i("jupyterlab-pachyderm", "2.6.0-alpha.2", (() => Promise.all([j.e(371), j.e(869)]).then((() => () => j(1979))))), i("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), i("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), i("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                    i = [];
+                return "default" === t && (u("jupyterlab-pachyderm", "2.6.0-alpha.3", (() => Promise.all([j.e(371), j.e(869)]).then((() => () => j(1979))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -142,129 +142,130 @@
         e = t(e), r = t(r);
         for (var a = 0;;) {
             if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
             var n = e[a],
                 o = (typeof n)[0];
             if (a >= r.length) return "u" == o;
             var l = r[a],
-                i = (typeof l)[0];
-            if (o != i) return "o" == o && "n" == i || "s" == i || "u" == o;
+                u = (typeof l)[0];
+            if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
             if ("o" != o && "u" != o && n != l) return n < l;
             a++
         }
     }, n = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(i = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, i);
+            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, u);
             return t
         }
         var l = [];
         for (o = 1; o < e.length; o++) {
-            var i = e[o];
-            l.push(0 === i ? "not(" + u() + ")" : 1 === i ? "(" + u() + " || " + u() + ")" : 2 === i ? l.pop() + " " + l.pop() : n(i))
+            var u = e[o];
+            l.push(0 === u ? "not(" + i() + ")" : 1 === u ? "(" + i() + " || " + i() + ")" : 2 === u ? l.pop() + " " + l.pop() : n(u))
         }
-        return u();
+        return i();
 
-        function u() {
+        function i() {
             return l.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
-            for (var l = 0, i = 1, u = !0;; i++, l++) {
-                var d, f, s = i < e.length ? (typeof e[i])[0] : "";
-                if (l >= r.length || "o" == (f = (typeof(d = r[l]))[0])) return !u || ("u" == s ? i > a && !n : "" == s != n);
+            for (var l = 0, u = 1, i = !0;; u++, l++) {
+                var d, f, s = u < e.length ? (typeof e[u])[0] : "";
+                if (l >= r.length || "o" == (f = (typeof(d = r[l]))[0])) return !i || ("u" == s ? u > a && !n : "" == s != n);
                 if ("u" == f) {
-                    if (!u || "u" != s) return !1
-                } else if (u)
+                    if (!i || "u" != s) return !1
+                } else if (i)
                     if (s == f)
-                        if (i <= a) {
-                            if (d != e[i]) return !1
+                        if (u <= a) {
+                            if (d != e[u]) return !1
                         } else {
-                            if (n ? d > e[i] : d < e[i]) return !1;
-                            d != e[i] && (u = !1)
+                            if (n ? d > e[u] : d < e[u]) return !1;
+                            d != e[u] && (i = !1)
                         }
                 else if ("s" != s && "n" != s) {
-                    if (n || i <= a) return !1;
-                    u = !1, i--
+                    if (n || u <= a) return !1;
+                    i = !1, u--
                 } else {
-                    if (i <= a || f < s != n) return !1;
-                    u = !1
-                } else "s" != s && "n" != s && (u = !1, i--)
+                    if (u <= a || f < s != n) return !1;
+                    i = !1
+                } else "s" != s && "n" != s && (i = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (l = 1; l < e.length; l++) {
             var h = e[l];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
     }, l = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, i = (e, r) => {
+    }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, u = (e, r, t) => "Unsatisfied version " + r + " of shared singleton module " + e + " (required " + n(t) + ")", d = (e, r, t, a) => {
-        var n = i(e, t);
-        return o(a, n) || "undefined" != typeof console && console.warn && console.warn(u(t, n, a)), s(e[t][n])
+    }, i = (e, r, t) => "Unsatisfied version " + r + " of shared singleton module " + e + " (required " + n(t) + ")", d = (e, r, t, a) => {
+        var n = u(e, t);
+        return o(a, n) || "undefined" != typeof console && console.warn && console.warn(i(t, n, a)), s(e[t][n])
     }, f = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, s = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, a, n) {
         var o = j.I(r);
         return o && o.then ? o.then(e.bind(e, r, j.S[r], t, a, n)) : e(r, j.S[r], t, a, n)
     })(((e, r, t, a) => (l(e, t), d(r, 0, t, a)))), h = p(((e, r, t, a, n) => {
         var o = r && j.o(r, t) && f(r, t, a);
         return o ? s(o) : n()
-    })), v = {}, m = {
+    })), b = {}, v = {
         930: () => h("default", "yaml", [1, 2, 1, 1], (() => j.e(676).then((() => () => j(5676))))),
-        1258: () => c("default", "@jupyterlab/services", [1, 6, 6, 1]),
-        1279: () => c("default", "@jupyterlab/launcher", [1, 3, 6, 1]),
         1431: () => c("default", "@lumino/widgets", [1, 1, 37, 1]),
         1526: () => c("default", "@lumino/coreutils", [1, 1, 11, 0]),
         1840: () => c("default", "@lumino/signaling", [1, 1, 10, 0]),
-        3535: () => c("default", "@jupyterlab/filebrowser", [1, 3, 6, 1]),
+        2884: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 2]),
+        3215: () => c("default", "@jupyterlab/ui-components", [1, 3, 6, 2]),
+        3619: () => c("default", "@jupyterlab/docmanager", [1, 3, 6, 2]),
         4234: () => h("default", "rudder-sdk-js", [1, 1, 2, 1], (() => j.e(67).then((() => () => j(3067))))),
         4439: () => h("default", "lodash", [1, 4, 17, 21], (() => j.e(486).then((() => () => j(6486))))),
-        4886: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 1]),
-        5149: () => c("default", "@jupyterlab/docmanager", [1, 3, 6, 1]),
-        5510: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 1]),
-        5705: () => c("default", "@jupyterlab/mainmenu", [1, 3, 6, 1]),
+        5613: () => c("default", "@jupyterlab/services", [1, 6, 6, 2]),
+        5643: () => c("default", "@jupyterlab/filebrowser", [1, 3, 6, 2]),
+        5679: () => c("default", "@jupyterlab/notebook", [1, 3, 6, 2]),
         6057: () => c("default", "@lumino/commands", [1, 1, 19, 0]),
         6271: () => c("default", "react", [1, 17, 0, 1]),
-        6591: () => c("default", "@jupyterlab/ui-components", [1, 3, 6, 1]),
-        6866: () => c("default", "@jupyterlab/application", [1, 3, 6, 1]),
-        8918: () => c("default", "@lumino/algorithm", [1, 1, 9, 0])
-    }, b = {
-        869: [930, 1258, 1279, 1431, 1526, 1840, 3535, 4234, 4439, 4886, 5149, 5510, 5705, 6057, 6271, 6591, 6866, 8918]
+        6848: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 2]),
+        8529: () => c("default", "@jupyterlab/launcher", [1, 3, 6, 2]),
+        8918: () => c("default", "@lumino/algorithm", [1, 1, 9, 0]),
+        9239: () => c("default", "@jupyterlab/application", [1, 3, 6, 2]),
+        9448: () => c("default", "@jupyterlab/mainmenu", [1, 3, 6, 2])
+    }, m = {
+        869: [930, 1431, 1526, 1840, 2884, 3215, 3619, 4234, 4439, 5613, 5643, 5679, 6057, 6271, 6848, 8529, 8918, 9239, 9448]
     }, j.f.consumes = (e, r) => {
-        j.o(b, e) && b[e].forEach((e => {
-            if (j.o(v, e)) return r.push(v[e]);
+        j.o(m, e) && m[e].forEach((e => {
+            if (j.o(b, e)) return r.push(b[e]);
             var t = r => {
-                    v[e] = 0, j.m[e] = t => {
+                    b[e] = 0, j.m[e] = t => {
                         delete j.c[e], t.exports = r()
                     }
                 },
                 a = r => {
-                    delete v[e], j.m[e] = t => {
+                    delete b[e], j.m[e] = t => {
                         throw delete j.c[e], r
                     }
                 };
             try {
-                var n = m[e]();
-                n.then ? r.push(v[e] = n.then(t).catch(a)) : t(n)
+                var n = v[e]();
+                n.then ? r.push(b[e] = n.then(t).catch(a)) : t(n)
             } catch (e) {
                 a(e)
             }
         }))
     }, (() => {
         var e = {
             815: 0
@@ -284,21 +285,21 @@
                                 o = t && t.target && t.target.src;
                             l.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", l.name = "ChunkLoadError", l.type = n, l.request = o, a[1](l)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var a, n, [o, l, i] = t,
-                    u = 0;
+                var a, n, [o, l, u] = t,
+                    i = 0;
                 if (o.some((r => 0 !== e[r]))) {
                     for (a in l) j.o(l, a) && (j.m[a] = l[a]);
-                    i && i(j)
+                    u && u(j)
                 }
-                for (r && r(t); u < o.length; u++) n = o[u], j.o(e, n) && e[n] && e[n][0](), e[o[u]] = 0
+                for (r && r(t); i < o.length; i++) n = o[i], j.o(e, n) && e[n] && e[n][0](), e[o[i]] = 0
             },
             t = self.webpackChunkjupyterlab_pachyderm = self.webpackChunkjupyterlab_pachyderm || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
     var w = j(6334);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["jupyterlab-pachyderm"] = w
 })();
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/labextension/static/third-party-licenses.json` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/mount_server_client.py` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/mount_server_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 
 from tornado.httpclient import AsyncHTTPClient, HTTPClientError
 from tornado import locks
 
 from .pachyderm import MountInterface
 from .log import get_logger
-from .env import SIDECAR_MODE
+from .env import SIDECAR_MODE, MOUNT_SERVER_LOG_DIR
 
 lock = locks.Lock()
 MOUNT_SERVER_PORT = 9002
 
 
 class MountServerClient(MountInterface):
     """Client interface for the mount-server backend."""
@@ -62,21 +62,25 @@
             get_logger().debug("Kubernetes is responsible for running mount server")
             return False
 
         get_logger().info("Starting mount server...")
         async with lock:
             if not await self._is_mount_server_running():
                 self._unmount()
+
+                mount_server_cmd = f"mount-server --mount-dir {self.mount_dir}"
+                if MOUNT_SERVER_LOG_DIR is not None and MOUNT_SERVER_LOG_DIR:
+                  mount_server_cmd += f" >> {MOUNT_SERVER_LOG_DIR} 2>&1"
+
                 subprocess.Popen(
                     [
                         "bash",
                         "-c",
                         "set -o pipefail; "
-                        + f"mount-server --mount-dir {self.mount_dir}"
-                        + " >> /tmp/mount-server.log 2>&1",
+                        + mount_server_cmd
                     ]
                 )
 
                 tries = 0
                 get_logger().debug("Waiting for mount server...")
                 while not await self._is_mount_server_running():
                     time.sleep(1)
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/pachyderm.py` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/pachyderm.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/tests/test_handlers.py` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/test_handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -532,7 +532,17 @@
 
 @pytest.mark.skipif(sys.version_info < (3, 7), reason="requires python3.7 or higher")
 @patch("jupyterlab_pachyderm.handlers.HealthHandler.mount_client", spec=MountInterface)
 async def test_health(mock_client, jp_fetch):
     mock_client.health.return_value = json.dumps({"status": "running"})
     r = await jp_fetch(f"/{NAMESPACE}/{VERSION}/health")
     assert json.loads(r.body) == {"status": "running"}
+
+
+@pytest.mark.skipif(sys.version_info < (3, 7), reason="requires python3.7 or higher")
+async def test_pps_get(jp_fetch):
+    response = await jp_fetch(f"/{NAMESPACE}/{VERSION}/pps/_create/NOT_REAL.ipynb")
+    assert response.code == 200
+    body = json.loads(response.body)
+    for expected_key in ("pipeline", "description", "transform", "input"):
+        assert expected_key in body
+
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm/tests/test_integrations.py` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/tests/test_integrations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import os
 import sys
 import subprocess
 import time
 import json
+from pathlib import Path
 
 import pytest
 import requests
 
 from jupyterlab_pachyderm.handlers import NAMESPACE, VERSION
 from jupyterlab_pachyderm.env import PFS_MOUNT_DIR
+from jupyterlab_pachyderm.pps_client import SAME_METADATA_FIELDS
 
 
 ADDRESS = "http://localhost:8888"
 BASE_URL = f"{ADDRESS}/{NAMESPACE}/{VERSION}"
 CONFIG_PATH = "~/.pachyderm/config.json"
 ROOT_TOKEN = "iamroot"
 DEFAULT_PROJECT = "default"
 
+TEST_NOTEBOOK = Path(__file__).parent.joinpath('data/TestNotebook.ipynb')
+
 
 @pytest.fixture()
 def pachyderm_resources():
     print("creating pachyderm resources")
     import python_pachyderm
     from python_pachyderm.pfs import Commit
 
@@ -373,7 +377,51 @@
     assert "30650" in endpoint_in_config
 
     # GET request
     r = requests.get(f"{BASE_URL}/config")
 
     assert r.status_code == 200
     assert r.json()["cluster_status"] != "INVALID"
+
+
+@pytest.fixture
+def simple_pachyderm_env():
+    from python_pachyderm import Client
+    client = Client()
+
+    repo_name = f"images_194837"
+    pipeline_name = f"test_pipeline_194837"
+    client.delete_repo(repo_name, force=True)
+    client.create_repo(repo_name)
+    yield client, repo_name, pipeline_name
+    client.delete_pipeline(pipeline_name, force=True)
+    client.delete_repo(repo_name, force=True)
+
+
+def test_pps(dev_server, simple_pachyderm_env):
+    client, repo_name, pipeline_name = simple_pachyderm_env
+    path = TEST_NOTEBOOK.relative_to(Path.cwd())
+    image = "combinatorml/jupyterlab-tensorflow-opencv:0.9"
+    input_spec = dict(pfs=dict(repo=repo_name, glob="/*"))
+    data = dict(
+        apiVersion='sameproject.ml/v1alpha1',
+        environments=dict(default=dict(image_tag=image)),
+        metadata=dict(name=pipeline_name, version='0.0.0'),
+        notebook=dict(requirements=''),
+        run=dict(name=pipeline_name, input=json.dumps(input_spec)),
+    )
+    r = requests.put(f"{BASE_URL}/pps/_create/{path}", data=json.dumps(data))
+    assert r.status_code == 200
+    assert next(client.inspect_pipeline(pipeline_name))
+
+
+@pytest.mark.parametrize('excluded_field', SAME_METADATA_FIELDS)
+def test_pps_validation_errors(dev_server, excluded_field):
+    path = TEST_NOTEBOOK.relative_to(Path.cwd())
+    data = dict()
+    for field in SAME_METADATA_FIELDS:
+        if field != excluded_field:
+            data[field] = dict()
+
+    r = requests.put(f"{BASE_URL}/pps/_create/{path}", data=json.dumps(data))
+    assert r.status_code == 500
+    assert r.json()['reason'] == f"Bad Request: field {excluded_field} not set"
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm.egg-info/PKG-INFO` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: jupyterlab-pachyderm
-Version: 2.6.0a2
+Version: 2.6.0a3
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: <4,>=3.7
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # jupyterlab-pachyderm
 
 [![CircleCI](https://circleci.com/gh/pachyderm/jupyterlab-pachyderm/tree/main.svg?style=shield&circle-token=23e1645bde6312d903e50be2dec7073bf0bcfbd0)](https://circleci.com/gh/pachyderm/jupyterlab-pachyderm/tree/main)
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/jupyterlab_pachyderm.egg-info/SOURCES.txt` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 jupyterlab_pachyderm/dev_server.py
 jupyterlab_pachyderm/env.py
 jupyterlab_pachyderm/filemanager.py
 jupyterlab_pachyderm/handlers.py
 jupyterlab_pachyderm/log.py
 jupyterlab_pachyderm/mount_server_client.py
 jupyterlab_pachyderm/pachyderm.py
+jupyterlab_pachyderm/pps_client.py
 jupyterlab_pachyderm.egg-info/PKG-INFO
 jupyterlab_pachyderm.egg-info/SOURCES.txt
 jupyterlab_pachyderm.egg-info/dependency_links.txt
 jupyterlab_pachyderm.egg-info/not-zip-safe
 jupyterlab_pachyderm.egg-info/requires.txt
 jupyterlab_pachyderm.egg-info/top_level.txt
 jupyterlab_pachyderm/labextension/package.json
@@ -35,21 +36,22 @@
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
 jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
 jupyterlab_pachyderm/labextension/static/747.4bacb4613a4fbdd0e8a7.js
-jupyterlab_pachyderm/labextension/static/869.6da4802142bf08400b17.js
-jupyterlab_pachyderm/labextension/static/remoteEntry.052fe0d2650242075a28.js
+jupyterlab_pachyderm/labextension/static/869.aa9313c5e001be51e97f.js
+jupyterlab_pachyderm/labextension/static/remoteEntry.8cf7225b6da9d05077a7.js
 jupyterlab_pachyderm/labextension/static/style.js
 jupyterlab_pachyderm/labextension/static/third-party-licenses.json
 jupyterlab_pachyderm/tests/__init__.py
 jupyterlab_pachyderm/tests/test_handlers.py
 jupyterlab_pachyderm/tests/test_integrations.py
+jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
 schema/examples.json
 schema/help.json
 schema/mount.json
 schema/telemetry.json
 src/global.d.ts
 src/handler.ts
 src/index.ts
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/package.json` & `jupyterlab_pachyderm-2.6.0a3/jupyterlab_pachyderm/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.8cf7225b6da9d05077a7.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'2.6.0-alpha.3'"}*

```diff
@@ -65,14 +65,19 @@
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "npm"
             ]
         }
     },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.8cf7225b6da9d05077a7.js",
+            "style": "./style"
+        },
         "disabledExtensions": [
             "jupyterlab-pachyderm:examples"
         ],
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_pachyderm"
@@ -127,9 +132,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.0-alpha.2"
+    "version": "2.6.0-alpha.3"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/pyproject.toml` & `jupyterlab_pachyderm-2.6.0a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/setup.cfg` & `jupyterlab_pachyderm-2.6.0a3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 platforms = Linux, Mac OS X, Windows
 classifiers = 
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Framework :: Jupyter
 	Framework :: Jupyter :: JupyterLab
 	Framework :: Jupyter :: JupyterLab :: 3
 	Framework :: Jupyter :: JupyterLab :: Extensions
 	Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 
 [options]
 packages = find:
 install_requires = 
 	jupyter_server>=1.6,<2
+	sameproject==0.2.5
 include_package_data = True
 zip_safe = False
-python_requires = >=3.7,<4
+python_requires = >=3.8,<4
 
 [options.extras_require]
 dev = 
 	black
 	jupyter_packaging~=0.10.0,<2
 	jupyterlab>=3.0.14
 	pre-commit
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/setup.py` & `jupyterlab_pachyderm-2.6.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/handler.ts` & `jupyterlab_pachyderm-2.6.0a3/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/examples/__test__/examples.test.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/examples/__test__/examples.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/examples/examples.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/examples/examples.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/help/__tests__/help.test.ts` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/help/__tests__/help.test.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/help/help.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/help/help.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/__tests__/mount.test.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/__tests__/mount.test.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import {StateDB} from '@jupyterlab/statedb';
 import {CommandRegistry} from '@lumino/commands';
 import {Widget} from '@lumino/widgets';
 import {mockedRequestAPI} from 'utils/testUtils';
 import {MountPlugin} from '../mount';
 import * as requestAPI from '../../../handler';
 import {waitFor} from '@testing-library/react';
+import {INotebookTracker, NotebookTracker} from '@jupyterlab/notebook';
 
 jest.mock('../../../handler');
 
 const items = {
   unmounted: [
     {
       repo: 'images',
@@ -39,14 +40,15 @@
   let app: JupyterLab;
   let docManager: IDocumentManager;
   let docRegistry: DocumentRegistry;
   let manager: ServiceManager;
   let factory: IFileBrowserFactory;
   let fileBrowser: FileBrowser;
   let restorer: ILayoutRestorer;
+  let tracker: INotebookTracker;
   const mockRequestAPI = requestAPI as jest.Mocked<typeof requestAPI>;
   beforeEach(() => {
     mockRequestAPI.requestAPI.mockImplementation(mockedRequestAPI(items));
 
     const opener = {
       open: (widget: Widget) => jest.fn(),
     };
@@ -64,15 +66,15 @@
 
     fileBrowser = new FileBrowser({id: 'test', model});
     factory = {
       createFileBrowser: () => fileBrowser,
       defaultBrowser: fileBrowser,
       tracker: new WidgetTracker<FileBrowser>({namespace: 'test'}),
     };
-
+    tracker = new NotebookTracker({namespace: 'test'});
     restorer = new LayoutRestorer({
       connector: new StateDB(),
       first: Promise.resolve<void>(void 0),
       registry: new CommandRegistry(),
     });
   });
 
@@ -98,15 +100,15 @@
                 repo: 'data',
                 branches: [],
               },
             },
           ],
         }),
       );
-    const plugin = new MountPlugin(app, docManager, factory, restorer);
+    const plugin = new MountPlugin(app, docManager, factory, restorer, tracker);
 
     await plugin.ready;
 
     jest.runAllTimers();
     await waitFor(() => {
       expect(plugin.unmountedRepos).toHaveLength(2);
       expect(plugin.unmountedRepos[0].repo).toBe('images');
@@ -120,15 +122,15 @@
       expect(plugin.mountedRepos).toHaveLength(1);
       expect(plugin.mountedRepos[0].name).toBe('images');
       expect(mockRequestAPI.requestAPI).toHaveBeenCalledTimes(3);
     });
   });
 
   it('should generate the correct layout', async () => {
-    const plugin = new MountPlugin(app, docManager, factory, restorer);
+    const plugin = new MountPlugin(app, docManager, factory, restorer, tracker);
     expect(plugin.layout.title.caption).toBe('Pachyderm Mount');
     expect(plugin.layout.id).toBe('pachyderm-mount');
     expect(plugin.layout.orientation).toBe('vertical');
     expect(plugin.layout.widgets).toHaveLength(8);
     expect(plugin.layout.widgets[0]).toBeInstanceOf(ReactWidget);
     expect(plugin.layout.widgets[1]).toBeInstanceOf(ReactWidget);
     expect(plugin.layout.widgets[2]).toBeInstanceOf(ReactWidget);
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Config/Config.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/Config.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Config/__tests__/Config.test.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/__tests__/Config.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Config/hooks/useConfig.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Config/hooks/useConfig.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Datum/Datum.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/Datum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Datum/hooks/useDatum.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Datum/hooks/useDatum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/FullPageError/FullPageError.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/FullPageError/FullPageError.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Pipeline/Pipeline.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/Pipeline.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 import React from 'react';
 import {closeIcon} from '@jupyterlab/ui-components';
 import {usePipeline} from './hooks/usePipeline';
+import {SameMetadata} from '../../types';
 
 type PipelineProps = {
   setShowPipeline: (shouldShow: boolean) => void;
+  notebookPath: string | undefined;
+  saveNotebookMetadata: (metadata: any) => void;
+  metadata: SameMetadata | undefined;
 };
 
 const placeholderInputSpec = `pfs:
   repo: images
   branch: dev
   glob: /*
 `;
 const placeholderRequirements = './requirements.txt';
 
-const Pipeline: React.FC<PipelineProps> = ({setShowPipeline}) => {
+const Pipeline: React.FC<PipelineProps> = ({
+  setShowPipeline,
+  notebookPath,
+  saveNotebookMetadata,
+  metadata,
+}) => {
   const {
     loading,
     pipelineName,
     setPipelineName,
     imageName,
     setImageName,
     inputSpec,
     setInputSpec,
     requirements,
     setRequirements,
     callCreatePipeline,
+    callSavePipeline,
     errorMessage,
-  } = usePipeline();
+  } = usePipeline(metadata, notebookPath, saveNotebookMetadata);
 
   return (
     <div className="pachyderm-mount-pipeline-base">
       <div className="pachyderm-mount-pipeline-back">
         <button
           data-testid="Pipeline__back"
           className="pachyderm-button-link"
@@ -49,17 +59,15 @@
         Notebook-to-Pipeline
       </span>
 
       <div className="pachyderm-pipeline-buttons">
         <button
           data-testid="Pipeline__save"
           className="pachyderm-button-link"
-          onClick={async () => {
-            return;
-          }}
+          onClick={callSavePipeline}
         >
           Save
         </button>
 
         <button
           data-testid="Pipeline__create_pipeline"
           className="pachyderm-button-link"
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx`

 * *Files 20% similar despite different names*

```diff
@@ -2,28 +2,53 @@
 import {render} from '@testing-library/react';
 import userEvent from '@testing-library/user-event';
 
 import * as requestAPI from '../../../../../handler';
 import {mockedRequestAPI} from 'utils/testUtils';
 import Pipeline from '../Pipeline';
 jest.mock('../../../../../handler');
+import {SameMetadata} from '../../../types';
 
 describe('PPS screen', () => {
   let setShowPipeline = jest.fn();
+  const saveNotebookMetaData = jest.fn();
+  const md: SameMetadata = {
+    apiVersion: '',
+    environments: {
+      default: {
+        image_tag: '',
+      },
+    },
+    metadata: {
+      name: '',
+    },
+    notebook: {
+      requirements: '',
+    },
+    run: {
+      name: '',
+    },
+  };
+
   const mockRequestAPI = requestAPI as jest.Mocked<typeof requestAPI>;
 
   beforeEach(() => {
     setShowPipeline = jest.fn();
     mockRequestAPI.requestAPI.mockImplementation(mockedRequestAPI({}));
   });
 
   describe('spec preview', () => {
     it('proper preview', async () => {
       const {getByTestId, findByTestId} = render(
-        <Pipeline setShowPipeline={setShowPipeline} />,
+        <Pipeline
+          metadata={md}
+          setShowPipeline={setShowPipeline}
+          notebookPath={'FakeNotebook.ipynb'}
+          saveNotebookMetadata={saveNotebookMetaData}
+        />,
       );
 
       const inputPipelineName = await findByTestId(
         'Pipeline__inputPipelineName',
       );
       userEvent.type(inputPipelineName, 'ThisPipelineIsNamedFred');
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/SortableList/ListMount.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/ListMount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/SortableList/ListUnmount.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/ListUnmount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/SortableList/SortableList.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/SortableList.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/customFileBrowser.ts` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/customFileBrowser.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/mount.css` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/mount.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/mount.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/mount.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import React from 'react';
 import {ILayoutRestorer, JupyterFrontEnd} from '@jupyterlab/application';
+import {INotebookTracker, NotebookPanel} from '@jupyterlab/notebook';
 import {IDocumentManager} from '@jupyterlab/docmanager';
 import {SplitPanel} from '@lumino/widgets';
 import {ReactWidget, UseSignal} from '@jupyterlab/apputils';
 import {FileBrowser, IFileBrowserFactory} from '@jupyterlab/filebrowser';
 import {settingsIcon, spreadsheetIcon} from '@jupyterlab/ui-components';
 import {Signal} from '@lumino/signaling';
 import {JSONObject} from '@lumino/coreutils';
@@ -16,37 +17,41 @@
   IMountPlugin,
   Repo,
   Mount,
   CurrentDatumResponse,
   PfsInput,
   ListMountsResponse,
   CrossInputSpec,
+  SameMetadata,
 } from './types';
 import Config from './components/Config/Config';
 import Datum from './components/Datum/Datum';
 import Pipeline from './components/Pipeline/Pipeline';
 import SortableList from './components/SortableList/SortableList';
 import LoadingDots from '../../utils/components/LoadingDots/LoadingDots';
 import FullPageError from './components/FullPageError/FullPageError';
 import {requestAPI} from '../../handler';
 
 export const MOUNT_BROWSER_NAME = 'mount-browser:';
 
+export const METADATA_KEY = 'same_config';
+
 export class MountPlugin implements IMountPlugin {
   private _app: JupyterFrontEnd<JupyterFrontEnd.IShell, 'desktop' | 'mobile'>;
   private _loader: ReactWidget;
   private _fullPageError: ReactWidget;
   private _config: ReactWidget;
   private _pipeline: ReactWidget;
   private _mountedList: ReactWidget;
   private _unmountedList: ReactWidget;
   private _datum: ReactWidget;
   private _mountBrowser: FileBrowser;
   private _poller: PollMounts;
   private _panel: SplitPanel;
+  private _tracker: INotebookTracker;
 
   private _showConfig = false;
   private _showConfigSignal = new Signal<this, boolean>(this);
   private _readyPromise: Promise<void> = Promise.resolve();
 
   private _showDatum = false;
   private _showPipeline = false;
@@ -54,24 +59,27 @@
   private _currentDatumInfo: CurrentDatumResponse | undefined;
   private _showDatumSignal = new Signal<this, boolean>(this);
   private _repoViewInputSpec: CrossInputSpec | PfsInput = {};
   private _saveInputSpecSignal = new Signal<this, CrossInputSpec | PfsInput>(
     this,
   );
   private _showPipelineSignal = new Signal<this, boolean>(this);
+  private _showMetadataSignal = new Signal<this, SameMetadata>(this);
 
   constructor(
     app: JupyterFrontEnd,
     manager: IDocumentManager,
     factory: IFileBrowserFactory,
     restorer: ILayoutRestorer,
+    tracker: INotebookTracker,
   ) {
     this._app = app;
     this._poller = new PollMounts('PollMounts');
     this._repoViewInputSpec = {};
+    this._tracker = tracker;
 
     // This is used to detect if the config goes bad (pachd address changes)
     this._poller.configSignal.connect((_, config) => {
       if (config.cluster_status === 'INVALID' && !this._showConfig) {
         this.setShowConfig(true);
       }
     });
@@ -214,15 +222,28 @@
           </UseSignal>
         )}
       </UseSignal>,
     );
     this._datum.addClass('pachyderm-mount-datum-wrapper');
 
     this._pipeline = ReactWidget.create(
-      <Pipeline setShowPipeline={this.setShowPipeline} />,
+      <UseSignal signal={this._showMetadataSignal}>
+        {(_, metadata) => (
+          <>
+            <Pipeline
+              setShowPipeline={this.setShowPipeline}
+              notebookPath={
+                this.getActiveNotebook()?.sessionContext?.session?.path
+              }
+              saveNotebookMetadata={this.saveNotebookMetaData}
+              metadata={metadata}
+            />
+          </>
+        )}
+      </UseSignal>,
     );
     this._pipeline.addClass('pachyderm-mount-pipeline-wrapper');
 
     this._loader = ReactWidget.create(<LoadingDots />);
 
     this._loader.addClass('pachyderm-mount-react-wrapper');
 
@@ -236,14 +257,16 @@
     this._fullPageError.addClass('pachyderm-mount-react-wrapper');
 
     this._mountBrowser = createCustomFileBrowser(app, manager, factory);
     this._poller.mountedSignal.connect(this.verifyBrowserPath);
     this._poller.mountedSignal.connect(this.refresh);
     this._poller.unmountedSignal.connect(this.refresh);
 
+    this._tracker.currentChanged.connect(this.handleNotebookChanged, this);
+
     this._panel = new SplitPanel();
     this._panel.orientation = 'vertical';
     this._panel.spacing = 0;
     this._panel.title.icon = mountLogoIcon;
     this._panel.title.caption = 'Pachyderm Mount';
     this._panel.id = 'pachyderm-mount';
     this._panel.addWidget(this._mountedList);
@@ -270,14 +293,53 @@
       this._panel.update();
     });
 
     restorer.add(this._panel, 'jupyterlab-pachyderm');
     app.shell.add(this._panel, 'left', {rank: 100});
   }
 
+  getActiveNotebook = (): NotebookPanel | null => {
+    return this._tracker.currentWidget;
+  };
+
+  /**
+   * This handles when a notebook is switched to another notebook.
+   * The parameters are automatically passed from the signal when a switch occurs.
+   */
+  handleNotebookChanged = async (
+    tracker: INotebookTracker,
+    notebook: NotebookPanel | null,
+  ): Promise<void> => {
+    // Set the current notebook and wait for the session to be ready
+    if (notebook) {
+      await notebook.sessionContext.ready;
+      const md = notebook?.model?.metadata.get(METADATA_KEY);
+
+      this._showMetadataSignal.emit(md as SameMetadata);
+      await Promise.resolve();
+    } else {
+      await Promise.resolve();
+    }
+  };
+
+  getNotebookMetadata = (notebook: NotebookPanel | null): any | null => {
+    return notebook?.model?.metadata.get(METADATA_KEY);
+  };
+
+  saveNotebookMetaData = (metadata: any): void => {
+    const currentNotebook = this.getActiveNotebook();
+
+    if (currentNotebook !== null) {
+      currentNotebook?.model?.metadata.set(METADATA_KEY, metadata);
+      console.log('notebook metadata saved');
+    } else {
+      console.log('No active notebook');
+    }
+  };
+
   open = (path: string): void => {
     this._app.commands.execute('filebrowser:open-path', {
       path: MOUNT_BROWSER_NAME + path,
     });
   };
 
   refresh = async (_: PollMounts, _data: Mount[] | Repo[]): Promise<void> => {
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/mountDrive.ts` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/mountDrive.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/pollMounts.ts` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/pollMounts.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/mount/types.ts` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/mount/types.ts`

 * *Files 22% similar despite different names*

```diff
@@ -81,7 +81,42 @@
 
 export interface IMountPlugin {
   mountedRepos: Mount[];
   unmountedRepos: Repo[];
   layout: SplitPanel;
   ready: Promise<void>;
 }
+
+export type SameMetadata = {
+  apiVersion: string;
+  environments: SameEnv;
+  metadata: SameMetaMetadata;
+  notebook: SameNotebookMetadata;
+  run: SameRunMetadata;
+};
+
+export type SameEnv = {
+  default: DefaultSameEnv;
+};
+
+export type DefaultSameEnv = {
+  image_tag: string;
+};
+export type SameMetaMetadata = {
+  labels?: string[];
+  name: string;
+  version?: string;
+};
+
+export type SameNotebookMetadata = {
+  // Note: name and path are filled in when you pass the notebook to SAME
+  requirements: string;
+};
+
+export type SameRunMetadata = {
+  name: string;
+  input?: string; //Note: SAME doesn't actually read this field when reading from the notebook and instead expects you to pass it on the command line
+};
+
+export type CreatePipelineResponse = {
+  message: string | null;
+};
```

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/telemetry/__tests__/telemetry.test.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/telemetry/__tests__/telemetry.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/plugins/telemetry/telemetry.ts` & `jupyterlab_pachyderm-2.6.0a3/src/plugins/telemetry/telemetry.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/utils/components/Circle/Circle.tsx` & `jupyterlab_pachyderm-2.6.0a3/src/utils/components/Circle/Circle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/utils/components/LoadingDots/loadingDots.css` & `jupyterlab_pachyderm-2.6.0a3/src/utils/components/LoadingDots/loadingDots.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/utils/components/Svgs/GenericError.js` & `jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/GenericError.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/utils/components/Svgs/KubernetesElephant.js` & `jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/KubernetesElephant.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/utils/components/Svgs/PachydermLogo.js` & `jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/PachydermLogo.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/utils/components/Svgs/StatusWarning.js` & `jupyterlab_pachyderm-2.6.0a3/src/utils/components/Svgs/StatusWarning.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/utils/hooks/useSort.ts` & `jupyterlab_pachyderm-2.6.0a3/src/utils/hooks/useSort.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/src/utils/icons.ts` & `jupyterlab_pachyderm-2.6.0a3/src/utils/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/style/base.css` & `jupyterlab_pachyderm-2.6.0a3/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/style/components/button.css` & `jupyterlab_pachyderm-2.6.0a3/style/components/button.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/style/icons/file.svg` & `jupyterlab_pachyderm-2.6.0a3/style/icons/file.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/style/icons/info.svg` & `jupyterlab_pachyderm-2.6.0a3/style/icons/info.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/style/icons/mount-logo.svg` & `jupyterlab_pachyderm-2.6.0a3/style/icons/mount-logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0a2/style/icons/repo.svg` & `jupyterlab_pachyderm-2.6.0a3/style/icons/repo.svg`

 * *Files identical despite different names*

