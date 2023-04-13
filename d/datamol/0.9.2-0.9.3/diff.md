# Comparing `tmp/datamol-0.9.2.tar.gz` & `tmp/datamol-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamol-0.9.2.tar", last modified: Fri Mar 31 11:44:48 2023, max compression
+gzip compressed data, was "datamol-0.9.3.tar", last modified: Thu Apr 13 19:29:15 2023, max compression
```

## Comparing `datamol-0.9.2.tar` & `datamol-0.9.3.tar`

### file list

```diff
@@ -1,204 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.462443 datamol-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-03-31 11:42:58.000000 datamol-0.9.2/.authors.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.430442 datamol-0.9.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-31 11:42:58.000000 datamol-0.9.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-31 11:42:58.000000 datamol-0.9.2/.devcontainer/bashrc
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-03-31 11:42:58.000000 datamol-0.9.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.430442 datamol-0.9.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 11:42:58.000000 datamol-0.9.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-03-31 11:42:58.000000 datamol-0.9.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-31 11:42:58.000000 datamol-0.9.2/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-31 11:42:58.000000 datamol-0.9.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 11:42:58.000000 datamol-0.9.2/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.430442 datamol-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-31 11:42:58.000000 datamol-0.9.2/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-03-31 11:42:58.000000 datamol-0.9.2/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-31 11:42:58.000000 datamol-0.9.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-03-31 11:42:58.000000 datamol-0.9.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-31 11:42:58.000000 datamol-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-31 11:42:58.000000 datamol-0.9.2/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-31 11:42:58.000000 datamol-0.9.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25336 2023-03-31 11:42:58.000000 datamol-0.9.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-03-31 11:42:58.000000 datamol-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-03-31 11:44:48.462443 datamol-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-03-31 11:42:58.000000 datamol-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.430442 datamol-0.9.2/binder/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-31 11:42:58.000000 datamol-0.9.2/binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-31 11:42:58.000000 datamol-0.9.2/binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-31 11:42:58.000000 datamol-0.9.2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.434442 datamol-0.9.2/datamol/
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/_sanifix4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.434442 datamol-0.9.2/datamol/conformers/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/conformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/conformers/_conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/conformers/_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.438443 datamol-0.9.2/datamol/data/
--rw-r--r--   0 runner    (1001) docker     (123)   160134 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/data/cdk2.sdf
--rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/data/freesolv.csv
--rw-r--r--   0 runner    (1001) docker     (123)   124841 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/data/reactions.json
--rw-r--r--   0 runner    (1001) docker     (123)   245735 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/data/solubility.test.sdf
--rw-r--r--   0 runner    (1001) docker     (123)  1376487 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/data/solubility.train.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.438443 datamol-0.9.2/datamol/descriptors/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/descriptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/descriptors/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/descriptors/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/fp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.438443 datamol-0.9.2/datamol/fragment/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/fragment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/fragment/_assemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/fragment/_fragment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    18365 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.438443 datamol-0.9.2/datamol/isomers/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/isomers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/isomers/_enumerate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/isomers/_structural.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/mcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43876 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/mol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/molar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.438443 datamol-0.9.2/datamol/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/predictors/esol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.442443 datamol-0.9.2/datamol/reactions/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/reactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/reactions/_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/reactions/_reactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.442443 datamol-0.9.2/datamol/scaffold/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/scaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/scaffold/_fuzzy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.442443 datamol-0.9.2/datamol/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/utils/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/utils/perf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.442443 datamol-0.9.2/datamol/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/viz/_circle_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/viz/_conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/viz/_substructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/viz/_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-03-31 11:42:58.000000 datamol-0.9.2/datamol/viz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.434442 datamol-0.9.2/datamol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-03-31 11:44:48.000000 datamol-0.9.2/datamol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-03-31 11:44:48.000000 datamol-0.9.2/datamol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 11:44:48.000000 datamol-0.9.2/datamol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-31 11:44:48.000000 datamol-0.9.2/datamol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-31 11:44:48.000000 datamol-0.9.2/datamol.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.442443 datamol-0.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.446443 datamol-0.9.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.align.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.cluster.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.conformers.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.convert.md
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.data.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.descriptors.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.fp.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.fragment.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.graph.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.io.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.isomers.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.log.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.mol.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.molar.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.reactions.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.scaffold.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.similarity.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/api/datamol.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.426442 datamol-0.9.2/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.446443 datamol-0.9.2/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/assets/css/custom-datamol.css
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/assets/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/assets/css/tweak-width.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.446443 datamol-0.9.2/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/assets/js/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/contribute.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.446443 datamol-0.9.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/images/logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/images/logo-title.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.450443 datamol-0.9.2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)   298565 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/Aligning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   174933 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/Clustering.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    94833 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/Conformers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   180458 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/Descriptors.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/Filesystem.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   297941 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/Fragment.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   210862 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/Fuzzy_Scaffolds.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    42846 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/Preprocessing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    89360 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/Reactions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   151601 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/Scaffolds.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   521054 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/The_Basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    84855 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/Visualization.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.454443 datamol-0.9.2/docs/tutorials/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1345316 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/data/ReactionBlock.rxn
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.454443 datamol-0.9.2/docs/tutorials/images/
--rw-r--r--   0 runner    (1001) docker     (123)   141008 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/images/Aligning_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    76455 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/images/Aligning_2.png
--rw-r--r--   0 runner    (1001) docker     (123)   310889 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/images/Conformers_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    40925 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/images/Descriptors_1.png
--rw-r--r--   0 runner    (1001) docker     (123)   422734 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/images/Fragment_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    67840 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/images/Fragment_2.png
--rw-r--r--   0 runner    (1001) docker     (123)    34879 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/images/Fragment_3.png
--rw-r--r--   0 runner    (1001) docker     (123)   333241 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/images/Preprocess_1.png
--rw-r--r--   0 runner    (1001) docker     (123)   102167 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/tutorials/images/Scaffolds_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-31 11:42:58.000000 datamol-0.9.2/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-31 11:42:58.000000 datamol-0.9.2/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-03-31 11:42:58.000000 datamol-0.9.2/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.458443 datamol-0.9.2/news/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-31 11:42:58.000000 datamol-0.9.2/news/TEMPLATE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-03-31 11:42:58.000000 datamol-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-31 11:42:58.000000 datamol-0.9.2/rever.xsh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 11:44:48.462443 datamol-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.462443 datamol-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:44:48.462443 datamol-0.9.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    30130 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/data/TUBB3-observations-last-broken.sdf
--rw-r--r--   0 runner    (1001) docker     (123)    30331 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/data/TUBB3-observations.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/data/TUBB3-observations.sdf.gz
--rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/data/freesolv.csv
--rw-r--r--   0 runner    (1001) docker     (123)    28227 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/data/freesolv.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/data/test.mol2
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_datamol_import_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_fragment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_isomers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_mcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_mol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_molar.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_predictors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_utils_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_utils_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_utils_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-31 11:42:58.000000 datamol-0.9.2/tests/test_viz_substrcture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.653833 datamol-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-13 19:27:46.000000 datamol-0.9.3/.authors.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.609833 datamol-0.9.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-13 19:27:46.000000 datamol-0.9.3/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 19:27:46.000000 datamol-0.9.3/.devcontainer/bashrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-13 19:27:46.000000 datamol-0.9.3/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.613833 datamol-0.9.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.613833 datamol-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-13 19:27:46.000000 datamol-0.9.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-13 19:27:46.000000 datamol-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-13 19:27:46.000000 datamol-0.9.3/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-13 19:27:46.000000 datamol-0.9.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25863 2023-04-13 19:27:46.000000 datamol-0.9.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-04-13 19:27:46.000000 datamol-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-13 19:29:15.649833 datamol-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-04-13 19:27:46.000000 datamol-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.613833 datamol-0.9.3/binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 19:27:46.000000 datamol-0.9.3/binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 19:27:46.000000 datamol-0.9.3/binder/postBuild
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-13 19:27:46.000000 datamol-0.9.3/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.617833 datamol-0.9.3/datamol/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/_sanifix4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.617833 datamol-0.9.3/datamol/conformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/conformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/conformers/_conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/conformers/_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.617833 datamol-0.9.3/datamol/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160134 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/data/cdk2.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/data/freesolv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   124841 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/data/reactions.json
+-rw-r--r--   0 runner    (1001) docker     (123)   245735 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/data/solubility.test.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)  1376487 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/data/solubility.train.sdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/descriptors/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/descriptors/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/fp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/fragment/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/fragment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/fragment/_assemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/fragment/_fragment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18365 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/isomers/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/isomers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/isomers/_enumerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/isomers/_structural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/mcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43876 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/molar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/predictors/esol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/reactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/reactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/reactions/_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/reactions/_reactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/scaffold/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/scaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/scaffold/_fuzzy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/utils/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/utils/perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.621833 datamol-0.9.3/datamol/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/viz/_circle_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/viz/_conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19122 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/viz/_lasso_highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/viz/_substructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/viz/_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-13 19:27:46.000000 datamol-0.9.3/datamol/viz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.617833 datamol-0.9.3/datamol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-13 19:29:15.000000 datamol-0.9.3/datamol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-13 19:29:15.000000 datamol-0.9.3/datamol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:29:15.000000 datamol-0.9.3/datamol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-13 19:29:15.000000 datamol-0.9.3/datamol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 19:29:15.000000 datamol-0.9.3/datamol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.625833 datamol-0.9.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.629833 datamol-0.9.3/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.align.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.cluster.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.conformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.convert.md
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.data.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.descriptors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.fp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.fragment.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.graph.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.io.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.isomers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.log.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.mol.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.molar.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.reactions.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.scaffold.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.similarity.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/api/datamol.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.609833 datamol-0.9.3/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.629833 datamol-0.9.3/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/assets/css/custom-datamol.css
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/assets/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/assets/css/tweak-width.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.629833 datamol-0.9.3/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/contribute.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.633833 datamol-0.9.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/images/logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/images/logo-title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.641833 datamol-0.9.3/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)   298565 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Aligning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   174933 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Clustering.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    94833 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Conformers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   180458 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Descriptors.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Filesystem.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   297941 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Fragment.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   210862 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Fuzzy_Scaffolds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42846 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Preprocessing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    89360 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Reactions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   151601 2023-04-13 19:27:46.000000 datamol-0.9.3/docs/tutorials/Scaffolds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   521054 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/The_Basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   181122 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/Visualization.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.645833 datamol-0.9.3/docs/tutorials/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1345316 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/data/ReactionBlock.rxn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.645833 datamol-0.9.3/docs/tutorials/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   141008 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Aligning_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76455 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Aligning_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   310889 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Conformers_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40925 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Descriptors_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   422734 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Fragment_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    67840 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Fragment_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34879 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Fragment_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   333241 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Preprocess_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   102167 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/tutorials/images/Scaffolds_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-13 19:27:47.000000 datamol-0.9.3/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-13 19:27:47.000000 datamol-0.9.3/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-13 19:27:47.000000 datamol-0.9.3/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.645833 datamol-0.9.3/news/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-13 19:27:47.000000 datamol-0.9.3/news/TEMPLATE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-13 19:27:47.000000 datamol-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-13 19:27:47.000000 datamol-0.9.3/rever.xsh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:29:15.653833 datamol-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.649833 datamol-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:29:15.649833 datamol-0.9.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    30130 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/data/TUBB3-observations-last-broken.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)    30331 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/data/TUBB3-observations.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/data/TUBB3-observations.sdf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/data/freesolv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    28227 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/data/freesolv.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/data/test.mol2
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_datamol_import_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_fragment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_isomers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_mcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_molar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_predictors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_utils_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_utils_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_utils_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_viz_lasso_highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-13 19:27:47.000000 datamol-0.9.3/tests/test_viz_substrcture.py
```

### Comparing `datamol-0.9.2/.authors.yml` & `datamol-0.9.3/.authors.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 - name: Emmanuel Noutahi
   email: emmanuel.noutahi@hotmail.ca
   aliases:
   - maclandrol
-  num_commits: 33
+  num_commits: 34
   first_commit: 2020-10-25 10:15:22
   github: DomInvivo
 - name: Hadrien Mary
   email: hadrien.mary@gmail.com
   aliases:
   - hadim
   alternate_emails:
   - hadim@users.noreply.github.com
-  num_commits: 38
+  num_commits: 39
   first_commit: 2020-10-24 11:46:22
   github: matudor
 - name: michelml
   email: michmoreau.l@gmail.com
   num_commits: 26
   first_commit: 2021-02-25 15:48:52
 - name: Honoré Hounwanou
   email: mercuryseries@gmail.com
-  num_commits: 1
+  num_commits: 3
   first_commit: 2021-02-12 17:01:32
 - name: Therence1
   email: 38595485+Therence1@users.noreply.github.com
   num_commits: 13
   first_commit: 2021-04-03 17:31:09
 - name: mike
   email: michael@invivoai.com
@@ -79,7 +79,11 @@
   first_commit: 2023-03-07 16:59:47
   github: SauravMaheshkar
 - name: Pakman450
   email: steven.pak10@gmail.com
   num_commits: 10
   first_commit: 2023-03-30 00:37:39
   github: Pakman450
+- name: dessygil
+  email: desmondgilmour@gmail.com
+  num_commits: 6
+  first_commit: 2023-04-05 17:40:19
```

### Comparing `datamol-0.9.2/.devcontainer/Dockerfile` & `datamol-0.9.3/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/.devcontainer/devcontainer.json` & `datamol-0.9.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/.github/CODE_OF_CONDUCT.md` & `datamol-0.9.3/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/.github/workflows/code-check.yml` & `datamol-0.9.3/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/.github/workflows/doc.yml` & `datamol-0.9.3/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/.github/workflows/release.yml` & `datamol-0.9.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/.github/workflows/test.yml` & `datamol-0.9.3/.github/workflows/test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,20 @@
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.9", "3.10"]
         os: ["ubuntu-latest", "macos-latest", "windows-latest"]
         rdkit-version: ["2022.03", "2022.09"]
 
+        # just enable python 3.11 on ubuntu to not blow up the CI time.
+        include:
+          - os: ubuntu-latest
+            python-version: "3.11"
+            rdkit-version: "2022.09"
+
     runs-on: ${{ matrix.os }}
     timeout-minutes: 30
 
     defaults:
       run:
         shell: bash -l {0}
```

### Comparing `datamol-0.9.2/.gitignore` & `datamol-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/.mailmap` & `datamol-0.9.3/.mailmap`

 * *Files 6% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 Lu Zhu <lu@valencediscovery.com>
 Matt <mtudor@proteovant.com>
 Pakman450 <steven.pak10@gmail.com>
 Saurav Maheshkar <sauravvmaheshkar@gmail.com>
 Therence1 <38595485+Therence1@users.noreply.github.com>
 Valence-JonnyHsu <104230580+Valence-JonnyHsu@users.noreply.github.com>
 deepsource-autofix[bot] <62050782+deepsource-autofix[bot]@users.noreply.github.com>
+dessygil <desmondgilmour@gmail.com>
 michelml <michmoreau.l@gmail.com>
 mike <michael@invivoai.com>
```

### Comparing `datamol-0.9.2/CHANGELOG.rst` & `datamol-0.9.3/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,41 @@
 ==================
 Datamol Changelogs
 ==================
 
 .. current developments
 
+v0.9.3
+====================
+
+**Added:**
+
+* added a feature that highlights substructures of 2D molecular images
+
+**Changed:**
+
+* Update CNAME to docs.datamol.io
+* Replace all occurrences of doc.datamol.io by docs.datamol.io
+* Switch from `pkg_resources` to `importlib.resources` for loading resources.
+* Enable python 3.11 on the CI.
+* Relocatem `datamol/data.py` to `datamol/data/__init__.py`.
+
+**Fixed:**
+
+* Color bug of the search input bar
+
+**Authors:**
+
+* Emmanuel Noutahi
+* Hadrien Mary
+* Honoré Hounwanou
+* dessygil
+
+
+
 v0.9.2
 ====================
 
 **Added:**
 
 * A multi-mol2 file reader that converts into rdkit objects
```

### Comparing `datamol-0.9.2/LICENSE` & `datamol-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/PKG-INFO` & `datamol-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: datamol
-Version: 0.9.2
+Version: 0.9.3
 Summary: A python library to work with molecules. Built on top of RDKit.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol
 Project-URL: Bug Tracker, https://github.com/datamol-io/datamol/issues
-Project-URL: Documentation, https://doc.datamol.io
+Project-URL: Documentation, https://docs.datamol.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
@@ -33,15 +33,15 @@
     <img src="docs/images/logo-title.svg" width="100%">
 </div>
 
 <p align="center">
     <b>datamol - molecular processing made easy</b> <br />
 </p>
 <p align="center">
-  <a href="https://doc.datamol.io/stable/" target="_blank">
+  <a href="https://docs.datamol.io/stable/" target="_blank">
       Docs
   </a> |
   <a href="https://datamol.io/" target="_blank">
       Homepage
   </a>
 </p>
 
@@ -69,15 +69,15 @@
 
 ## Try Online
 
 Visit [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/datamol-io/datamol/main?urlpath=lab/tree/docs/tutorials/The_Basics.ipynb) and try Datamol online.
 
 ## Documentation
 
-Visit https://doc.datamol.io.
+Visit https://docs.datamol.io.
 
 ## Installation
 
 Use conda:
 
 ```bash
 mamba install -c conda-forge datamol
@@ -130,23 +130,23 @@
 
 ## Compatibilities
 
 Version compatibilities are an essential topic for production-software stacks. We are cautious about documenting compatibility between `datamol`, `python` and `rdkit`.
 
 See below the associated versions of Python and RDKit, for which a minor version of Datamol **has been tested** during its whole lifecycle. _It does not mean other combinations does not work but that those are not tested._
 
-| `datamol` | `python`           | `rdkit`                       |
-| --------- | ------------------ | ----------------------------- |
-| `0.9`     | `[3.9, 3.10]`      | `[2022.03, 2022.09]`          |
-| `0.8`     | `[3.8, 3.9, 3.10]` | `[2021.09, 2022.03, 2022.09]` |
-| `0.7`     | `[3.8, 3.9]`       | `[2021.09, 2022.03]`          |
-| `0.6`     | `[3.8, 3.9]`       | `[2021.09]`                   |
-| `0.5`     | `[3.8, 3.9]`       | `[2021.03, 2021.09]`          |
-| `0.4`     | `[3.8, 3.9]`       | `[2020.09, 2021.03]`          |
-| `0.3`     | `[3.8, 3.9]`       | `[2020.09, 2021.03]`          |
+| `datamol` | `python`            | `rdkit`                       |
+| --------- | ------------------- | ----------------------------- |
+| `0.9`     | `[3.9, 3.10, 3.11]` | `[2022.03, 2022.09]`          |
+| `0.8`     | `[3.8, 3.9, 3.10]`  | `[2021.09, 2022.03, 2022.09]` |
+| `0.7`     | `[3.8, 3.9]`        | `[2021.09, 2022.03]`          |
+| `0.6`     | `[3.8, 3.9]`        | `[2021.09]`                   |
+| `0.5`     | `[3.8, 3.9]`        | `[2021.03, 2021.09]`          |
+| `0.4`     | `[3.8, 3.9]`        | `[2020.09, 2021.03]`          |
+| `0.3`     | `[3.8, 3.9]`        | `[2020.09, 2021.03]`          |
 
 ## CI Status
 
 The CI runs tests and performs code quality checks for the following combinations:
 
 - The three major platforms: Windows, OSX and Linux.
 - The two latest Python versions.
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: datamol Version: 0.9.2 Summary: A python library to
+Metadata-Version: 2.1 Name: datamol Version: 0.9.3 Summary: A python library to
 work with molecules. Built on top of RDKit. Author-email: Hadrien Mary
 valencediscovery.com> License: Apache Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol Project-URL:
 Bug Tracker, https://github.com/datamol-io/datamol/issues Project-URL:
-Documentation, https://doc.datamol.io Classifier: Development Status :: 5 -
+Documentation, https://docs.datamol.io Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Healthcare Industry Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis Classifier:
 Topic :: Scientific/Engineering :: Medical Science Apps. Classifier: Natural
 Language :: English Classifier: Operating System :: OS Independent Classifier:
@@ -44,15 +44,15 @@
 molecules often relies on many options; Datamol provides good defaults by
 design. - ð§  Performance matters: built-in efficient parallelization when
 possible with an optional progress bar. - ð¹ï¸ Modern IO: out-of-the-box
 support for remote paths using `fsspec` to read and write multiple formats
 (sdf, xlsx, csv, etc). ## Try Online Visit [![Binder](http://mybinder.org/
 badge_logo.svg)](https://mybinder.org/v2/gh/datamol-io/datamol/
 main?urlpath=lab/tree/docs/tutorials/The_Basics.ipynb) and try Datamol online.
-## Documentation Visit https://doc.datamol.io. ## Installation Use conda:
+## Documentation Visit https://docs.datamol.io. ## Installation Use conda:
 ```bash mamba install -c conda-forge datamol ``` ## Quick API Tour ```python
 import datamol as dm # Common functions mol = dm.to_mol("O=C(C)Oc1ccccc1C
 (=O)O", sanitize=True) fp = dm.to_fp(mol) selfies = dm.to_selfies(mol) inchi =
 dm.to_inchi(mol) # Standardize and sanitize mol = dm.to_mol("O=C(C)Oc1ccccc1C
 (=O)O") mol = dm.fix_mol(mol) mol = dm.sanitize_mol(mol) mol =
 dm.standardize_mol(mol) # Dataframe manipulation df = dm.data.freesolv() mols =
 dm.from_df(df) # 2D viz legends = [dm.to_smiles(mol) for mol in mols[:10]]
@@ -66,16 +66,16 @@
 /zenodo.org/badge/341603042.svg)](https://zenodo.org/badge/latestdoi/
 341603042). ## Compatibilities Version compatibilities are an essential topic
 for production-software stacks. We are cautious about documenting compatibility
 between `datamol`, `python` and `rdkit`. See below the associated versions of
 Python and RDKit, for which a minor version of Datamol **has been tested**
 during its whole lifecycle. _It does not mean other combinations does not work
 but that those are not tested._ | `datamol` | `python` | `rdkit` | | --------
-- | ------------------ | ----------------------------- | | `0.9` | `[3.9,
-3.10]` | `[2022.03, 2022.09]` | | `0.8` | `[3.8, 3.9, 3.10]` | `[2021.09,
+- | ------------------- | ----------------------------- | | `0.9` | `[3.9,
+3.10, 3.11]` | `[2022.03, 2022.09]` | | `0.8` | `[3.8, 3.9, 3.10]` | `[2021.09,
 2022.03, 2022.09]` | | `0.7` | `[3.8, 3.9]` | `[2021.09, 2022.03]` | | `0.6` |
 `[3.8, 3.9]` | `[2021.09]` | | `0.5` | `[3.8, 3.9]` | `[2021.03, 2021.09]` | |
 `0.4` | `[3.8, 3.9]` | `[2020.09, 2021.03]` | | `0.3` | `[3.8, 3.9]` | `
 [2020.09, 2021.03]` | ## CI Status The CI runs tests and performs code quality
 checks for the following combinations: - The three major platforms: Windows,
 OSX and Linux. - The two latest Python versions. - The two latest RDKit
 versions. | | `main` | | --------------------------------------- | ------------
```

### Comparing `datamol-0.9.2/README.md` & `datamol-0.9.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     <img src="docs/images/logo-title.svg" width="100%">
 </div>
 
 <p align="center">
     <b>datamol - molecular processing made easy</b> <br />
 </p>
 <p align="center">
-  <a href="https://doc.datamol.io/stable/" target="_blank">
+  <a href="https://docs.datamol.io/stable/" target="_blank">
       Docs
   </a> |
   <a href="https://datamol.io/" target="_blank">
       Homepage
   </a>
 </p>
 
@@ -38,15 +38,15 @@
 
 ## Try Online
 
 Visit [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/datamol-io/datamol/main?urlpath=lab/tree/docs/tutorials/The_Basics.ipynb) and try Datamol online.
 
 ## Documentation
 
-Visit https://doc.datamol.io.
+Visit https://docs.datamol.io.
 
 ## Installation
 
 Use conda:
 
 ```bash
 mamba install -c conda-forge datamol
@@ -99,23 +99,23 @@
 
 ## Compatibilities
 
 Version compatibilities are an essential topic for production-software stacks. We are cautious about documenting compatibility between `datamol`, `python` and `rdkit`.
 
 See below the associated versions of Python and RDKit, for which a minor version of Datamol **has been tested** during its whole lifecycle. _It does not mean other combinations does not work but that those are not tested._
 
-| `datamol` | `python`           | `rdkit`                       |
-| --------- | ------------------ | ----------------------------- |
-| `0.9`     | `[3.9, 3.10]`      | `[2022.03, 2022.09]`          |
-| `0.8`     | `[3.8, 3.9, 3.10]` | `[2021.09, 2022.03, 2022.09]` |
-| `0.7`     | `[3.8, 3.9]`       | `[2021.09, 2022.03]`          |
-| `0.6`     | `[3.8, 3.9]`       | `[2021.09]`                   |
-| `0.5`     | `[3.8, 3.9]`       | `[2021.03, 2021.09]`          |
-| `0.4`     | `[3.8, 3.9]`       | `[2020.09, 2021.03]`          |
-| `0.3`     | `[3.8, 3.9]`       | `[2020.09, 2021.03]`          |
+| `datamol` | `python`            | `rdkit`                       |
+| --------- | ------------------- | ----------------------------- |
+| `0.9`     | `[3.9, 3.10, 3.11]` | `[2022.03, 2022.09]`          |
+| `0.8`     | `[3.8, 3.9, 3.10]`  | `[2021.09, 2022.03, 2022.09]` |
+| `0.7`     | `[3.8, 3.9]`        | `[2021.09, 2022.03]`          |
+| `0.6`     | `[3.8, 3.9]`        | `[2021.09]`                   |
+| `0.5`     | `[3.8, 3.9]`        | `[2021.03, 2021.09]`          |
+| `0.4`     | `[3.8, 3.9]`        | `[2020.09, 2021.03]`          |
+| `0.3`     | `[3.8, 3.9]`        | `[2020.09, 2021.03]`          |
 
 ## CI Status
 
 The CI runs tests and performs code quality checks for the following combinations:
 
 - The three major platforms: Windows, OSX and Linux.
 - The two latest Python versions.
```

#### html2text {}

```diff
@@ -25,15 +25,15 @@
 molecules often relies on many options; Datamol provides good defaults by
 design. - ð§  Performance matters: built-in efficient parallelization when
 possible with an optional progress bar. - ð¹ï¸ Modern IO: out-of-the-box
 support for remote paths using `fsspec` to read and write multiple formats
 (sdf, xlsx, csv, etc). ## Try Online Visit [![Binder](http://mybinder.org/
 badge_logo.svg)](https://mybinder.org/v2/gh/datamol-io/datamol/
 main?urlpath=lab/tree/docs/tutorials/The_Basics.ipynb) and try Datamol online.
-## Documentation Visit https://doc.datamol.io. ## Installation Use conda:
+## Documentation Visit https://docs.datamol.io. ## Installation Use conda:
 ```bash mamba install -c conda-forge datamol ``` ## Quick API Tour ```python
 import datamol as dm # Common functions mol = dm.to_mol("O=C(C)Oc1ccccc1C
 (=O)O", sanitize=True) fp = dm.to_fp(mol) selfies = dm.to_selfies(mol) inchi =
 dm.to_inchi(mol) # Standardize and sanitize mol = dm.to_mol("O=C(C)Oc1ccccc1C
 (=O)O") mol = dm.fix_mol(mol) mol = dm.sanitize_mol(mol) mol =
 dm.standardize_mol(mol) # Dataframe manipulation df = dm.data.freesolv() mols =
 dm.from_df(df) # 2D viz legends = [dm.to_smiles(mol) for mol in mols[:10]]
@@ -47,16 +47,16 @@
 /zenodo.org/badge/341603042.svg)](https://zenodo.org/badge/latestdoi/
 341603042). ## Compatibilities Version compatibilities are an essential topic
 for production-software stacks. We are cautious about documenting compatibility
 between `datamol`, `python` and `rdkit`. See below the associated versions of
 Python and RDKit, for which a minor version of Datamol **has been tested**
 during its whole lifecycle. _It does not mean other combinations does not work
 but that those are not tested._ | `datamol` | `python` | `rdkit` | | --------
-- | ------------------ | ----------------------------- | | `0.9` | `[3.9,
-3.10]` | `[2022.03, 2022.09]` | | `0.8` | `[3.8, 3.9, 3.10]` | `[2021.09,
+- | ------------------- | ----------------------------- | | `0.9` | `[3.9,
+3.10, 3.11]` | `[2022.03, 2022.09]` | | `0.8` | `[3.8, 3.9, 3.10]` | `[2021.09,
 2022.03, 2022.09]` | | `0.7` | `[3.8, 3.9]` | `[2021.09, 2022.03]` | | `0.6` |
 `[3.8, 3.9]` | `[2021.09]` | | `0.5` | `[3.8, 3.9]` | `[2021.03, 2021.09]` | |
 `0.4` | `[3.8, 3.9]` | `[2020.09, 2021.03]` | | `0.3` | `[3.8, 3.9]` | `
 [2020.09, 2021.03]` | ## CI Status The CI runs tests and performs code quality
 checks for the following combinations: - The three major platforms: Windows,
 OSX and Linux. - The two latest Python versions. - The two latest RDKit
 versions. | | `main` | | --------------------------------------- | ------------
```

### Comparing `datamol-0.9.2/binder/environment.yml` & `datamol-0.9.3/binder/environment.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/__init__.py` & `datamol-0.9.3/datamol/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 from .isomers import remove_stereochemistry
 
 from . import align
 from . import conformers
 from . import viz
 
 from .viz import to_image
+from .viz import lasso_highlight_image
 
 from .mcs import find_mcs
 
 from .graph import to_graph
 from .graph import get_all_path_between
 from .graph import match_molecular_graphs
 from .graph import reorder_mol_from_template
```

### Comparing `datamol-0.9.2/datamol/_sanifix4.py` & `datamol-0.9.3/datamol/_sanifix4.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/_version.py` & `datamol-0.9.3/datamol/_version.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/align.py` & `datamol-0.9.3/datamol/align.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/cluster.py` & `datamol-0.9.3/datamol/cluster.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/conformers/_conformers.py` & `datamol-0.9.3/datamol/conformers/_conformers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/conformers/_features.py` & `datamol-0.9.3/datamol/conformers/_features.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/convert.py` & `datamol-0.9.3/datamol/convert.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/data/cdk2.sdf` & `datamol-0.9.3/datamol/data/cdk2.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/data/freesolv.csv` & `datamol-0.9.3/datamol/data/freesolv.csv`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/data/reactions.json` & `datamol-0.9.3/datamol/data/reactions.json`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/data/solubility.test.sdf` & `datamol-0.9.3/datamol/data/solubility.test.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/data/solubility.train.sdf` & `datamol-0.9.3/datamol/data/solubility.train.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/data.py` & `datamol-0.9.3/datamol/data/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,23 +6,56 @@
 
 from typing import Optional
 from typing import cast
 from typing import Union
 from typing import List
 from typing import overload
 from typing import Literal
+from typing import cast
+
+import sys
+import io
 
-import pkg_resources
+try:
+    import importlib.resources as importlib_resources
+except:
+    import importlib_resources
 
 import pandas as pd
 
-from .types import Mol
-from .io import read_sdf
-from .convert import from_df
-from .convert import render_mol_df
+from ..types import Mol
+from ..io import read_sdf
+from ..convert import from_df
+from ..convert import render_mol_df
+
+
+def open_datamol_data_file(
+    filename: str,
+    open_binary: bool = False,
+    dm_module: str = "datamol.data",
+):
+    if sys.version_info < (3, 9, 0):
+        if open_binary:
+            file_context_manager = importlib_resources.open_binary(dm_module, filename)
+        else:
+            file_context_manager = importlib_resources.open_text(dm_module, filename)
+    else:
+        if open_binary:
+            mode = "rb"
+        else:
+            mode = "r"
+
+        file_context_manager = (
+            importlib_resources.files(dm_module).joinpath(filename).open(mode=mode)
+        )
+
+    # NOTE(hadim): we assume the file always exists
+    file_context_manager = cast(io.TextIOWrapper, file_context_manager)
+
+    return file_context_manager
 
 
 @overload
 def freesolv(as_df: Literal[True] = True) -> pd.DataFrame:
     ...
 
 
@@ -44,15 +77,15 @@
 
     Warning:
         This dataset is only meant to be used as a toy dataset for pedagogic and
         testing purposes. **It is not** a dataset for benchmarking, analysis or
         model training.
     """
 
-    with pkg_resources.resource_stream("datamol", "data/freesolv.csv") as f:
+    with open_datamol_data_file("freesolv.csv") as f:
         data = pd.read_csv(f)
 
     if not as_df:
         data = from_df(data)
 
     return data
 
@@ -76,15 +109,15 @@
     """Return the RDKit CDK2 dataset from `RDConfig.RDDocsDir, 'Book/data/cdk2.sdf'`.
 
     Args:
         as_df: Whether to return a list mol or a pandas DataFrame.
         mol_column: Name of the mol column. Only relevant if `as_df` is True.
     """
 
-    with pkg_resources.resource_stream("datamol", "data/cdk2.sdf") as f:
+    with open_datamol_data_file("cdk2.sdf", open_binary=True) as f:
         data = read_sdf(f, as_df=as_df, mol_column=mol_column)
     return data
 
 
 @overload
 def solubility(as_df: Literal[True] = True, mol_column: Optional[str] = "mol") -> pd.DataFrame:
     ...
@@ -108,18 +141,18 @@
     The dataframe or the list of molecules with contain a `split` column, either `train` or `test`.
 
     Args:
         as_df: Whether to return a list mol or a pandas DataFrame.
         mol_column: Name of the mol column. Only relevant if `as_df` is True.
     """
 
-    with pkg_resources.resource_stream("datamol", "data/solubility.train.sdf") as f:
+    with open_datamol_data_file("solubility.train.sdf", open_binary=True) as f:
         train = read_sdf(f, as_df=True, mol_column="mol", smiles_column=None)
 
-    with pkg_resources.resource_stream("datamol", "data/solubility.test.sdf") as f:
+    with open_datamol_data_file("solubility.test.sdf", open_binary=True) as f:
         test = read_sdf(f, as_df=True, mol_column="mol", smiles_column=None)
 
     train = cast(pd.DataFrame, train)
     test = cast(pd.DataFrame, test)
 
     train["split"] = "train"
     test["split"] = "test"
```

### Comparing `datamol-0.9.2/datamol/descriptors/__init__.py` & `datamol-0.9.3/datamol/descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/descriptors/compute.py` & `datamol-0.9.3/datamol/descriptors/compute.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/descriptors/descriptors.py` & `datamol-0.9.3/datamol/descriptors/descriptors.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/fp.py` & `datamol-0.9.3/datamol/fp.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/fragment/_assemble.py` & `datamol-0.9.3/datamol/fragment/_assemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 from typing import Optional
 
 import copy
 import json
 import itertools
 import random
 import re
-import pkg_resources
 
 from functools import lru_cache
 
 import numpy as np
 
 from rdkit import Chem
 from rdkit.Chem import rdChemReactions
 
 import datamol as dm
+
 from ..types import Mol
+from ..data import open_datamol_data_file
 
 CCQ = "[$([#6][!#6;!#1]):1]!@[#6;!a:2]>>[*:1].[*:2]"
 CCQ_RETRO = "[$([#6;!H0][!#6;!#1]):1].[#6;!a;!H0:2]>>[*:1][*:2]"
 
 BRICS_ENVIRONS = {
     "L1": "[C;D3]([#0,#6,#7,#8])(=O)",
     "L3": "[O;D2]-;!@[#0,#6,#1]",
@@ -203,15 +204,16 @@
 
 
 @lru_cache(maxsize=None)
 def get_reactions_list():
     all_rxns = []
     all_rxns_retro = []
     all_rxns_type = []
-    with pkg_resources.resource_stream("datamol", "data/reactions.json") as IN:
+
+    with open_datamol_data_file("reactions.json") as IN:
         rxns = json.load(IN)
         for k, data in rxns.items():
             try:
                 rxn = data.get("syn_smarts")
                 retro_rxn = data.get("retro_smarts")
                 retro_rxn = rdChemReactions.ReactionFromSmarts(retro_rxn)
                 rxn = rdChemReactions.ReactionFromSmarts(rxn)
```

### Comparing `datamol-0.9.2/datamol/fragment/_fragment.py` & `datamol-0.9.3/datamol/fragment/_fragment.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/graph.py` & `datamol-0.9.3/datamol/graph.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/io.py` & `datamol-0.9.3/datamol/io.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/isomers/_enumerate.py` & `datamol-0.9.3/datamol/isomers/_enumerate.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/isomers/_structural.py` & `datamol-0.9.3/datamol/isomers/_structural.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/log.py` & `datamol-0.9.3/datamol/log.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/mcs.py` & `datamol-0.9.3/datamol/mcs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/mol.py` & `datamol-0.9.3/datamol/mol.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/molar.py` & `datamol-0.9.3/datamol/molar.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/predictors/esol.py` & `datamol-0.9.3/datamol/predictors/esol.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/reactions/__init__.py` & `datamol-0.9.3/datamol/reactions/__init__.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/reactions/_attachments.py` & `datamol-0.9.3/datamol/reactions/_attachments.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/reactions/_reactions.py` & `datamol-0.9.3/datamol/reactions/_reactions.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/scaffold/_fuzzy.py` & `datamol-0.9.3/datamol/scaffold/_fuzzy.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/similarity.py` & `datamol-0.9.3/datamol/similarity.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/utils/decorators.py` & `datamol-0.9.3/datamol/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/utils/fs.py` & `datamol-0.9.3/datamol/utils/fs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/utils/jobs.py` & `datamol-0.9.3/datamol/utils/jobs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/utils/perf.py` & `datamol-0.9.3/datamol/utils/perf.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/utils/testing.py` & `datamol-0.9.3/datamol/utils/testing.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/viz/_circle_grid.py` & `datamol-0.9.3/datamol/viz/_circle_grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,20 +81,22 @@
         """Create circles and slices in-memory"""
         draw = ImageDraw.Draw(self.image)
         self.draw = draw
         all_radius = self._draw_circles(draw)
         self._draw_center_mol()
         self._draw_ring_mols(all_radius)
         font = None
-        w, h = draw.textsize(self.legend)
+        left, top, right, bottom = draw.textbbox((0, 0), self.legend)
+        w, h = right - left, bottom - top
         try:
             fn = FontManager()
             fontpath = fn.findfont("Droid sans")
             font = ImageFont.truetype(fontpath, 12 * self.size // 800)
-            w, h = font.getsize(self.legend)
+            left, top, right, bottom = font.getbbox(self.legend)
+            w, h = right - left, bottom - top
         except:
             pass
         draw.text(
             ((self.size // 2 - w) - 2, self.size - 2 * h),
             self.legend,
             fill="black",
             font=font,
```

### Comparing `datamol-0.9.2/datamol/viz/_conformers.py` & `datamol-0.9.3/datamol/viz/_conformers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/viz/_substructure.py` & `datamol-0.9.3/datamol/viz/_substructure.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/viz/_viz.py` & `datamol-0.9.3/datamol/viz/_viz.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol/viz/utils.py` & `datamol-0.9.3/datamol/viz/utils.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/datamol.egg-info/PKG-INFO` & `datamol-0.9.3/datamol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: datamol
-Version: 0.9.2
+Version: 0.9.3
 Summary: A python library to work with molecules. Built on top of RDKit.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol
 Project-URL: Bug Tracker, https://github.com/datamol-io/datamol/issues
-Project-URL: Documentation, https://doc.datamol.io
+Project-URL: Documentation, https://docs.datamol.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
@@ -33,15 +33,15 @@
     <img src="docs/images/logo-title.svg" width="100%">
 </div>
 
 <p align="center">
     <b>datamol - molecular processing made easy</b> <br />
 </p>
 <p align="center">
-  <a href="https://doc.datamol.io/stable/" target="_blank">
+  <a href="https://docs.datamol.io/stable/" target="_blank">
       Docs
   </a> |
   <a href="https://datamol.io/" target="_blank">
       Homepage
   </a>
 </p>
 
@@ -69,15 +69,15 @@
 
 ## Try Online
 
 Visit [![Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/datamol-io/datamol/main?urlpath=lab/tree/docs/tutorials/The_Basics.ipynb) and try Datamol online.
 
 ## Documentation
 
-Visit https://doc.datamol.io.
+Visit https://docs.datamol.io.
 
 ## Installation
 
 Use conda:
 
 ```bash
 mamba install -c conda-forge datamol
@@ -130,23 +130,23 @@
 
 ## Compatibilities
 
 Version compatibilities are an essential topic for production-software stacks. We are cautious about documenting compatibility between `datamol`, `python` and `rdkit`.
 
 See below the associated versions of Python and RDKit, for which a minor version of Datamol **has been tested** during its whole lifecycle. _It does not mean other combinations does not work but that those are not tested._
 
-| `datamol` | `python`           | `rdkit`                       |
-| --------- | ------------------ | ----------------------------- |
-| `0.9`     | `[3.9, 3.10]`      | `[2022.03, 2022.09]`          |
-| `0.8`     | `[3.8, 3.9, 3.10]` | `[2021.09, 2022.03, 2022.09]` |
-| `0.7`     | `[3.8, 3.9]`       | `[2021.09, 2022.03]`          |
-| `0.6`     | `[3.8, 3.9]`       | `[2021.09]`                   |
-| `0.5`     | `[3.8, 3.9]`       | `[2021.03, 2021.09]`          |
-| `0.4`     | `[3.8, 3.9]`       | `[2020.09, 2021.03]`          |
-| `0.3`     | `[3.8, 3.9]`       | `[2020.09, 2021.03]`          |
+| `datamol` | `python`            | `rdkit`                       |
+| --------- | ------------------- | ----------------------------- |
+| `0.9`     | `[3.9, 3.10, 3.11]` | `[2022.03, 2022.09]`          |
+| `0.8`     | `[3.8, 3.9, 3.10]`  | `[2021.09, 2022.03, 2022.09]` |
+| `0.7`     | `[3.8, 3.9]`        | `[2021.09, 2022.03]`          |
+| `0.6`     | `[3.8, 3.9]`        | `[2021.09]`                   |
+| `0.5`     | `[3.8, 3.9]`        | `[2021.03, 2021.09]`          |
+| `0.4`     | `[3.8, 3.9]`        | `[2020.09, 2021.03]`          |
+| `0.3`     | `[3.8, 3.9]`        | `[2020.09, 2021.03]`          |
 
 ## CI Status
 
 The CI runs tests and performs code quality checks for the following combinations:
 
 - The three major platforms: Windows, OSX and Linux.
 - The two latest Python versions.
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: datamol Version: 0.9.2 Summary: A python library to
+Metadata-Version: 2.1 Name: datamol Version: 0.9.3 Summary: A python library to
 work with molecules. Built on top of RDKit. Author-email: Hadrien Mary
 valencediscovery.com> License: Apache Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol Project-URL:
 Bug Tracker, https://github.com/datamol-io/datamol/issues Project-URL:
-Documentation, https://doc.datamol.io Classifier: Development Status :: 5 -
+Documentation, https://docs.datamol.io Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Healthcare Industry Classifier: Intended Audience ::
 Science/Research Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis Classifier:
 Topic :: Scientific/Engineering :: Medical Science Apps. Classifier: Natural
 Language :: English Classifier: Operating System :: OS Independent Classifier:
@@ -44,15 +44,15 @@
 molecules often relies on many options; Datamol provides good defaults by
 design. - ð§  Performance matters: built-in efficient parallelization when
 possible with an optional progress bar. - ð¹ï¸ Modern IO: out-of-the-box
 support for remote paths using `fsspec` to read and write multiple formats
 (sdf, xlsx, csv, etc). ## Try Online Visit [![Binder](http://mybinder.org/
 badge_logo.svg)](https://mybinder.org/v2/gh/datamol-io/datamol/
 main?urlpath=lab/tree/docs/tutorials/The_Basics.ipynb) and try Datamol online.
-## Documentation Visit https://doc.datamol.io. ## Installation Use conda:
+## Documentation Visit https://docs.datamol.io. ## Installation Use conda:
 ```bash mamba install -c conda-forge datamol ``` ## Quick API Tour ```python
 import datamol as dm # Common functions mol = dm.to_mol("O=C(C)Oc1ccccc1C
 (=O)O", sanitize=True) fp = dm.to_fp(mol) selfies = dm.to_selfies(mol) inchi =
 dm.to_inchi(mol) # Standardize and sanitize mol = dm.to_mol("O=C(C)Oc1ccccc1C
 (=O)O") mol = dm.fix_mol(mol) mol = dm.sanitize_mol(mol) mol =
 dm.standardize_mol(mol) # Dataframe manipulation df = dm.data.freesolv() mols =
 dm.from_df(df) # 2D viz legends = [dm.to_smiles(mol) for mol in mols[:10]]
@@ -66,16 +66,16 @@
 /zenodo.org/badge/341603042.svg)](https://zenodo.org/badge/latestdoi/
 341603042). ## Compatibilities Version compatibilities are an essential topic
 for production-software stacks. We are cautious about documenting compatibility
 between `datamol`, `python` and `rdkit`. See below the associated versions of
 Python and RDKit, for which a minor version of Datamol **has been tested**
 during its whole lifecycle. _It does not mean other combinations does not work
 but that those are not tested._ | `datamol` | `python` | `rdkit` | | --------
-- | ------------------ | ----------------------------- | | `0.9` | `[3.9,
-3.10]` | `[2022.03, 2022.09]` | | `0.8` | `[3.8, 3.9, 3.10]` | `[2021.09,
+- | ------------------- | ----------------------------- | | `0.9` | `[3.9,
+3.10, 3.11]` | `[2022.03, 2022.09]` | | `0.8` | `[3.8, 3.9, 3.10]` | `[2021.09,
 2022.03, 2022.09]` | | `0.7` | `[3.8, 3.9]` | `[2021.09, 2022.03]` | | `0.6` |
 `[3.8, 3.9]` | `[2021.09]` | | `0.5` | `[3.8, 3.9]` | `[2021.03, 2021.09]` | |
 `0.4` | `[3.8, 3.9]` | `[2020.09, 2021.03]` | | `0.3` | `[3.8, 3.9]` | `
 [2020.09, 2021.03]` | ## CI Status The CI runs tests and performs code quality
 checks for the following combinations: - The three major platforms: Windows,
 OSX and Linux. - The two latest Python versions. - The two latest RDKit
 versions. | | `main` | | --------------------------------------- | ------------
```

### Comparing `datamol-0.9.2/datamol.egg-info/SOURCES.txt` & `datamol-0.9.3/datamol.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 binder/postBuild
 datamol/__init__.py
 datamol/_sanifix4.py
 datamol/_version.py
 datamol/align.py
 datamol/cluster.py
 datamol/convert.py
-datamol/data.py
 datamol/fp.py
 datamol/graph.py
 datamol/io.py
 datamol/log.py
 datamol/mcs.py
 datamol/mol.py
 datamol/molar.py
@@ -44,14 +43,15 @@
 datamol.egg-info/SOURCES.txt
 datamol.egg-info/dependency_links.txt
 datamol.egg-info/requires.txt
 datamol.egg-info/top_level.txt
 datamol/conformers/__init__.py
 datamol/conformers/_conformers.py
 datamol/conformers/_features.py
+datamol/data/__init__.py
 datamol/data/cdk2.sdf
 datamol/data/freesolv.csv
 datamol/data/reactions.json
 datamol/data/solubility.test.sdf
 datamol/data/solubility.train.sdf
 datamol/descriptors/__init__.py
 datamol/descriptors/compute.py
@@ -74,14 +74,15 @@
 datamol/utils/fs.py
 datamol/utils/jobs.py
 datamol/utils/perf.py
 datamol/utils/testing.py
 datamol/viz/__init__.py
 datamol/viz/_circle_grid.py
 datamol/viz/_conformers.py
+datamol/viz/_lasso_highlight.py
 datamol/viz/_substructure.py
 datamol/viz/_viz.py
 datamol/viz/utils.py
 docs/CNAME
 docs/contribute.md
 docs/index.md
 docs/license.md
@@ -160,14 +161,15 @@
 tests/test_reactions.py
 tests/test_scaffold.py
 tests/test_similarity.py
 tests/test_utils_fs.py
 tests/test_utils_jobs.py
 tests/test_utils_perf.py
 tests/test_viz.py
+tests/test_viz_lasso_highlight.py
 tests/test_viz_substrcture.py
 tests/data/TUBB3-observations-last-broken.sdf
 tests/data/TUBB3-observations.sdf
 tests/data/TUBB3-observations.sdf.gz
 tests/data/freesolv.csv
 tests/data/freesolv.xlsx
 tests/data/test.mol2
```

### Comparing `datamol-0.9.2/docs/assets/css/custom-datamol.css` & `datamol-0.9.3/docs/assets/css/custom-datamol.css`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,18 @@
   color: rgb(255, 255, 255) !important;
 }
 
 .md-search__form {
   background-color: rgba(255, 255, 255, 0.2);
 }
 
+.md-search__input {
+  color: #222222 !important;
+}
+
 .md-header__topic {
   color: rgb(255, 255, 255);
   font-size: 1.4em;
 }
 
 /* Increase the size of the logo */
 .md-header__button.md-logo img,
@@ -77,8 +81,8 @@
   padding: 0.4em;
 }
 
 /* Remove the `In` and `Out` block in rendered Jupyter notebooks */
 .md-container .jp-Cell-outputWrapper .jp-OutputPrompt.jp-OutputArea-prompt,
 .md-container .jp-Cell-inputWrapper .jp-InputPrompt.jp-InputArea-prompt {
   display: none !important;
-}
+}
```

### Comparing `datamol-0.9.2/docs/assets/css/custom.css` & `datamol-0.9.3/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/contribute.md` & `datamol-0.9.3/docs/contribute.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/images/logo-black.png` & `datamol-0.9.3/docs/images/logo-black.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/images/logo-black.svg` & `datamol-0.9.3/docs/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/images/logo-title.svg` & `datamol-0.9.3/docs/images/logo-title.svg`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/images/logo.png` & `datamol-0.9.3/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/images/logo.svg` & `datamol-0.9.3/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/index.md` & `datamol-0.9.3/docs/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -69,16 +69,16 @@
 
 ## Compatibilities
 
 Version compatibilities are an essential topic for production-software stacks. We are cautious about documenting compatibility between `datamol`, `python` and `rdkit`.
 
 See below the associated versions of Python and RDKit, for which a minor version of Datamol **has been tested** during its whole lifecycle. _It does not mean other combinations does not work but that those are not tested._
 
-| `datamol` | `python`           | `rdkit`                       |
-| --------- | ------------------ | ----------------------------- |
-| `0.9`     | `[3.9, 3.10]`      | `[2022.03, 2022.09]`          |
-| `0.8`     | `[3.8, 3.9, 3.10]` | `[2021.09, 2022.03, 2022.09]` |
-| `0.7`     | `[3.8, 3.9]`       | `[2021.09, 2022.03]`          |
-| `0.6`     | `[3.8, 3.9]`       | `[2021.09]`                   |
-| `0.5`     | `[3.8, 3.9]`       | `[2021.03, 2021.09]`          |
-| `0.4`     | `[3.8, 3.9]`       | `[2020.09, 2021.03]`          |
-| `0.3`     | `[3.8, 3.9]`       | `[2020.09, 2021.03]`          |
+| `datamol` | `python`            | `rdkit`                       |
+| --------- | ------------------- | ----------------------------- |
+| `0.9`     | `[3.9, 3.10, 3.11]` | `[2022.03, 2022.09]`          |
+| `0.8`     | `[3.8, 3.9, 3.10]`  | `[2021.09, 2022.03, 2022.09]` |
+| `0.7`     | `[3.8, 3.9]`        | `[2021.09, 2022.03]`          |
+| `0.6`     | `[3.8, 3.9]`        | `[2021.09]`                   |
+| `0.5`     | `[3.8, 3.9]`        | `[2021.03, 2021.09]`          |
+| `0.4`     | `[3.8, 3.9]`        | `[2020.09, 2021.03]`          |
+| `0.3`     | `[3.8, 3.9]`        | `[2020.09, 2021.03]`          |
```

### Comparing `datamol-0.9.2/docs/tutorials/Aligning.ipynb` & `datamol-0.9.3/docs/tutorials/Aligning.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/Clustering.ipynb` & `datamol-0.9.3/docs/tutorials/Clustering.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/Conformers.ipynb` & `datamol-0.9.3/docs/tutorials/Conformers.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/Descriptors.ipynb` & `datamol-0.9.3/docs/tutorials/Descriptors.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/Filesystem.ipynb` & `datamol-0.9.3/docs/tutorials/Filesystem.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/Fragment.ipynb` & `datamol-0.9.3/docs/tutorials/Fragment.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/Fuzzy_Scaffolds.ipynb` & `datamol-0.9.3/docs/tutorials/Fuzzy_Scaffolds.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/Preprocessing.ipynb` & `datamol-0.9.3/docs/tutorials/Preprocessing.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/Reactions.ipynb` & `datamol-0.9.3/docs/tutorials/Reactions.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/Scaffolds.ipynb` & `datamol-0.9.3/docs/tutorials/Scaffolds.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/The_Basics.ipynb` & `datamol-0.9.3/docs/tutorials/The_Basics.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf` & `datamol-0.9.3/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/data/ReactionBlock.rxn` & `datamol-0.9.3/docs/tutorials/data/ReactionBlock.rxn`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/images/Aligning_1.png` & `datamol-0.9.3/docs/tutorials/images/Aligning_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/images/Aligning_2.png` & `datamol-0.9.3/docs/tutorials/images/Aligning_2.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/images/Conformers_1.png` & `datamol-0.9.3/docs/tutorials/images/Conformers_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/images/Descriptors_1.png` & `datamol-0.9.3/docs/tutorials/images/Descriptors_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/images/Fragment_1.png` & `datamol-0.9.3/docs/tutorials/images/Fragment_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/images/Fragment_2.png` & `datamol-0.9.3/docs/tutorials/images/Fragment_2.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/images/Fragment_3.png` & `datamol-0.9.3/docs/tutorials/images/Fragment_3.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/images/Preprocess_1.png` & `datamol-0.9.3/docs/tutorials/images/Preprocess_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/tutorials/images/Scaffolds_1.png` & `datamol-0.9.3/docs/tutorials/images/Scaffolds_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/docs/usage.md` & `datamol-0.9.3/docs/usage.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/env.yml` & `datamol-0.9.3/env.yml`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
   - joblib
   - fsspec >=2021.9
   - s3fs >=2021.9
   - gcsfs >=2021.9
   - platformdirs
   - packaging
   - typing_extensions
+  - importlib_resources
 
   # Scientific
   - pandas
   - numpy
   - scipy
   - pillow
   - matplotlib
```

### Comparing `datamol-0.9.2/mkdocs.yml` & `datamol-0.9.3/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -80,20 +80,21 @@
   # For `tab_length=2` in the markdown extension
   # See https://github.com/mkdocs/mkdocs/issues/545
   - mdx_truly_sane_lists
   - toc:
       permalink: true
       toc_depth: 4
 
+watch:
+  - datamol/
+
 plugins:
   - search
 
   - mkdocstrings:
-      watch:
-        - datamol/
       handlers:
         python:
           setup_commands:
             - import sys
             - sys.path.append("docs")
             - sys.path.append("datamol")
           selection:
```

### Comparing `datamol-0.9.2/pyproject.toml` & `datamol-0.9.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     # "rdkit",
 ]
 
 [project.urls]
 Website = "https://datamol.io"
 "Source Code" = "https://github.com/datamol-io/datamol"
 "Bug Tracker" = "https://github.com/datamol-io/datamol/issues"
-Documentation = "https://doc.datamol.io"
+Documentation = "https://docs.datamol.io"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools_scm]
 fallback_version = "dev"
 
@@ -77,15 +77,19 @@
 target-version = ['py39', 'py310']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--verbose --cov=datamol --cov-fail-under=85 --cov-report xml --cov-report term --durations=10 -n auto"
 testpaths = ["tests"]
-filterwarnings = ["ignore::DeprecationWarning:rdkit.*:"]
+filterwarnings = [
+    "ignore::DeprecationWarning:rdkit.*:",
+    "ignore::DeprecationWarning:jupyter_client.*:",
+    "ignore::DeprecationWarning:pkg_resources.*:",
+]
 
 [tool.coverage.run]
 omit = ["setup.py", "tests/*", "SA_Score/*"]
 disable_warnings = ["no-data-collected"]
 
 [tool.coverage.xml]
 output = "coverage.xml"
```

### Comparing `datamol-0.9.2/tests/conftest.py` & `datamol-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/data/TUBB3-observations-last-broken.sdf` & `datamol-0.9.3/tests/data/TUBB3-observations-last-broken.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/data/TUBB3-observations.sdf` & `datamol-0.9.3/tests/data/TUBB3-observations.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/data/TUBB3-observations.sdf.gz` & `datamol-0.9.3/tests/data/TUBB3-observations.sdf.gz`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/data/freesolv.csv` & `datamol-0.9.3/tests/data/freesolv.csv`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/data/freesolv.xlsx` & `datamol-0.9.3/tests/data/freesolv.xlsx`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/data/test.mol2` & `datamol-0.9.3/tests/data/test.mol2`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_align.py` & `datamol-0.9.3/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_cluster.py` & `datamol-0.9.3/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_conformers.py` & `datamol-0.9.3/tests/test_conformers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_convert.py` & `datamol-0.9.3/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_data.py` & `datamol-0.9.3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_datamol_import_time.py` & `datamol-0.9.3/tests/test_datamol_import_time.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_descriptors.py` & `datamol-0.9.3/tests/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_fp.py` & `datamol-0.9.3/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_fragment.py` & `datamol-0.9.3/tests/test_fragment.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_graph.py` & `datamol-0.9.3/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_io.py` & `datamol-0.9.3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_isomers.py` & `datamol-0.9.3/tests/test_isomers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_log.py` & `datamol-0.9.3/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_mcs.py` & `datamol-0.9.3/tests/test_mcs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_mol.py` & `datamol-0.9.3/tests/test_mol.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_molar.py` & `datamol-0.9.3/tests/test_molar.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_notebooks.py` & `datamol-0.9.3/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_predictors.py` & `datamol-0.9.3/tests/test_predictors.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_reactions.py` & `datamol-0.9.3/tests/test_reactions.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_scaffold.py` & `datamol-0.9.3/tests/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_similarity.py` & `datamol-0.9.3/tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_utils_fs.py` & `datamol-0.9.3/tests/test_utils_fs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_utils_jobs.py` & `datamol-0.9.3/tests/test_utils_jobs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_viz.py` & `datamol-0.9.3/tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.2/tests/test_viz_substrcture.py` & `datamol-0.9.3/tests/test_viz_substrcture.py`

 * *Files identical despite different names*

