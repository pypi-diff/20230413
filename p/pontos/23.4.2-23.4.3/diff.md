# Comparing `tmp/pontos-23.4.2.tar.gz` & `tmp/pontos-23.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.4.2.tar", max compression
+gzip compressed data, was "pontos-23.4.3.tar", max compression
```

## Comparing `pontos-23.4.2.tar` & `pontos-23.4.3.tar`

### file list

```diff
@@ -1,248 +1,248 @@
--rw-r--r--   0        0        0    35149 2023-04-12 07:27:28.477329 pontos-23.4.2/LICENSE
--rw-r--r--   0        0        0     3349 2023-04-12 07:27:28.477329 pontos-23.4.2/README.md
--rw-r--r--   0        0        0    97724 2023-04-12 07:27:28.481329 pontos-23.4.2/poetry.lock
--rw-r--r--   0        0        0       32 2023-04-12 07:27:28.481329 pontos-23.4.2/poetry.toml
--rw-r--r--   0        0        0      791 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/__init__.py
--rw-r--r--   0        0        0      968 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/changelog/__init__.py
--rw-r--r--   0        0        0     9914 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4427 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/git/__init__.py
--rw-r--r--   0        0        0    16117 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/__init__.py
--rw-r--r--   0        0        0     1154 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     6158 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4173 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/api.py
--rw-r--r--   0        0        0     6196 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    10519 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    11942 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/search.py
--rw-r--r--   0        0        0     6004 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15207 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/main.py
--rw-r--r--   0        0        0     1114 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7508 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/organization.py
--rw-r--r--   0        0        0    12937 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/search.py
--rw-r--r--   0        0        0     4606 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3207 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/script/errors.py
--rw-r--r--   0        0        0     4854 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/script/parser.py
--rw-r--r--   0        0        0    14685 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/helper.py
--rw-r--r--   0        0        0     6211 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/models/__init__.py
--rw-r--r--   0        0        0      821 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4660 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/api.py
--rw-r--r--   0        0        0     2149 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     6708 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2618 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    10802 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3400 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/py.typed
--rw-r--r--   0        0        0     1164 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/release/main.py
--rw-r--r--   0        0        0     7491 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/release/parser.py
--rw-r--r--   0        0        0    12426 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/release/release.py
--rw-r--r--   0        0        0    12039 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/terminal/null.py
--rw-r--r--   0        0        0     4717 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/testing/__init__.py
--rw-r--r--   0        0        0      773 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      749 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0      757 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0      737 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0      753 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0      757 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0      757 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      871 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0      737 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0      737 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      747 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0      709 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      741 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      741 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0      733 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0      733 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      793 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0      802 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0      781 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0      802 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0      802 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      915 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0      781 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0      781 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0      791 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0      751 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      783 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      783 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      727 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0      735 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0      715 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0      731 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0      735 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0      735 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      849 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0      715 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0      715 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      725 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0      687 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      720 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      720 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12050 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1067 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1416 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     7752 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3792 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     6263 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     7786 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/errors.py
--rw-r--r--   0        0        0     2018 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/helper.py
--rw-r--r--   0        0        0     3692 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13117 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2145 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    14501 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5241 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/version.py
--rw-r--r--   0        0        0     2890 2023-04-12 07:27:28.485329 pontos-23.4.2/pyproject.toml
--rw-r--r--   0        0        0     1872 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/artifacts.py
--rw-r--r--   0        0        0     1605 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/create-repository.py
--rw-r--r--   0        0        0     2212 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/members.py
--rw-r--r--   0        0        0     2179 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/repositories.py
--rw-r--r--   0        0        0     6717 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/teams.py
--rw-r--r--   0        0        0     2789 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/workflow-runs.py
--rw-r--r--   0        0        0     1518 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    17750 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/git/__init__.py
--rw-r--r--   0        0        0    27772 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     4385 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    52500 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17774 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_search.py
--rw-r--r--   0        0        0     9471 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19874 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    76541 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3400 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3520 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6098 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11271 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3706 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25911 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/release/__init__.py
--rw-r--r--   0        0        0     3190 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/release/test_helper.py
--rw-r--r--   0        0        0     8223 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/release/test_parser.py
--rw-r--r--   0        0        0    59154 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/release/test_release.py
--rw-r--r--   0        0        0    21452 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    19355 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/test_helper.py
--rw-r--r--   0        0        0     1373 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/testing/__init__.py
--rw-r--r--   0        0        0     7785 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/testing/test_testing.py
--rw-r--r--   0        0        0      721 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15227 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/commands/__init__.py
--rw-r--r--   0        0        0    11322 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/commands/test_go.py
--rw-r--r--   0        0        0    15371 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16667 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    22817 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    25027 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/test_errors.py
--rw-r--r--   0        0        0     3385 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/test_version.py
--rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 pontos-23.4.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-13 08:30:47.399806 pontos-23.4.3/LICENSE
+-rw-r--r--   0        0        0     3349 2023-04-13 08:30:47.399806 pontos-23.4.3/README.md
+-rw-r--r--   0        0        0    97724 2023-04-13 08:30:47.403806 pontos-23.4.3/poetry.lock
+-rw-r--r--   0        0        0       32 2023-04-13 08:30:47.403806 pontos-23.4.3/poetry.toml
+-rw-r--r--   0        0        0      791 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/__init__.py
+-rw-r--r--   0        0        0      968 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0     9914 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4427 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/git/__init__.py
+-rw-r--r--   0        0        0    16117 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1154 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     6158 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4173 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6196 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    13121 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    11942 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21512 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15207 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/main.py
+-rw-r--r--   0        0        0     1114 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7508 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    14248 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-04-13 08:30:47.403806 pontos-23.4.3/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3207 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     4854 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/github/script/parser.py
+-rw-r--r--   0        0        0    14685 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/helper.py
+-rw-r--r--   0        0        0     6211 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/models/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4660 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2149 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     6708 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2618 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    10802 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3400 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/py.typed
+-rw-r--r--   0        0        0     1164 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/release/__init__.py
+-rw-r--r--   0        0        0     2472 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/release/helper.py
+-rw-r--r--   0        0        0     2127 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/release/main.py
+-rw-r--r--   0        0        0     7491 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/release/parser.py
+-rw-r--r--   0        0        0    14588 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/release/release.py
+-rw-r--r--   0        0        0    12039 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/terminal/null.py
+-rw-r--r--   0        0        0     4717 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      773 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      749 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0      757 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0      737 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0      753 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0      757 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0      757 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      871 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0      737 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0      737 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      747 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0      709 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      741 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      741 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0      733 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0      733 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      793 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0      802 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0      781 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0      802 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0      802 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      915 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0      781 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0      781 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0      791 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0      751 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      783 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      783 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      727 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0      735 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0      715 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0      731 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0      735 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0      735 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      849 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0      715 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0      715 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      725 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0      687 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      720 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      720 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12050 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1067 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1416 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     7752 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3792 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     6263 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     7786 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/errors.py
+-rw-r--r--   0        0        0     2809 2023-04-13 08:30:47.407806 pontos-23.4.3/pontos/version/helper.py
+-rw-r--r--   0        0        0     3692 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/project.py
+-rw-r--r--   0        0        0     2163 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    13419 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2145 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    16023 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5317 2023-04-13 08:30:47.411806 pontos-23.4.3/pontos/version/version.py
+-rw-r--r--   0        0        0     2890 2023-04-13 08:30:47.411806 pontos-23.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1872 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/artifacts-download.py
+-rw-r--r--   0        0        0     1862 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/artifacts.py
+-rw-r--r--   0        0        0     1605 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/branchprotection.py
+-rw-r--r--   0        0        0     5606 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/members.py
+-rw-r--r--   0        0        0     2179 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/repositories.py
+-rw-r--r--   0        0        0     6717 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/search-repositories.py
+-rw-r--r--   0        0        0     3689 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/teams.py
+-rw-r--r--   0        0        0     2789 2023-04-13 08:30:47.411806 pontos-23.4.3/scripts/github/workflow-runs.py
+-rw-r--r--   0        0        0     1518 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    17750 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/git/__init__.py
+-rw-r--r--   0        0        0    27772 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     4385 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    58514 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17774 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9471 2023-04-13 08:30:47.411806 pontos-23.4.3/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19874 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    80894 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3400 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3520 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6098 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11271 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3706 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25911 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/release/__init__.py
+-rw-r--r--   0        0        0     3190 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/release/test_helper.py
+-rw-r--r--   0        0        0     8223 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/release/test_parser.py
+-rw-r--r--   0        0        0    65783 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/release/test_release.py
+-rw-r--r--   0        0        0    21452 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0    19355 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/test_helper.py
+-rw-r--r--   0        0        0     1373 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/testing/__init__.py
+-rw-r--r--   0        0        0     7785 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15227 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0    11322 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0    15371 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16667 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    25525 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    27735 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/test_errors.py
+-rw-r--r--   0        0        0     5505 2023-04-13 08:30:47.415807 pontos-23.4.3/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-04-13 08:30:47.419807 pontos-23.4.3/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-04-13 08:30:47.419807 pontos-23.4.3/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-04-13 08:30:47.419807 pontos-23.4.3/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-04-13 08:30:47.419807 pontos-23.4.3/tests/version/test_version.py
+-rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 pontos-23.4.3/PKG-INFO
```

### Comparing `pontos-23.4.2/LICENSE` & `pontos-23.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/README.md` & `pontos-23.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/poetry.lock` & `pontos-23.4.3/poetry.lock`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/__init__.py` & `pontos-23.4.3/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/changelog/__init__.py` & `pontos-23.4.3/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/changelog/conventional_commits.py` & `pontos-23.4.3/pontos/changelog/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/changelog/errors.py` & `pontos-23.4.3/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/changelog/main.py` & `pontos-23.4.3/pontos/changelog/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/errors.py` & `pontos-23.4.3/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/git/__init__.py` & `pontos-23.4.3/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/git/git.py` & `pontos-23.4.3/pontos/git/git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/git/status.py` & `pontos-23.4.3/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/__init__.py` & `pontos-23.4.3/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/actions/__init__.py` & `pontos-23.4.3/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/actions/argparser.py` & `pontos-23.4.3/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/actions/cmds.py` & `pontos-23.4.3/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/actions/core.py` & `pontos-23.4.3/pontos/github/actions/core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/actions/env.py` & `pontos-23.4.3/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/actions/errors.py` & `pontos-23.4.3/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/actions/event.py` & `pontos-23.4.3/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/actions/main.py` & `pontos-23.4.3/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/__init__.py` & `pontos-23.4.3/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/api.py` & `pontos-23.4.3/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/artifacts.py` & `pontos-23.4.3/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/branch.py` & `pontos-23.4.3/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/client.py` & `pontos-23.4.3/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/contents.py` & `pontos-23.4.3/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/errors.py` & `pontos-23.4.3/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/helper.py` & `pontos-23.4.3/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/labels.py` & `pontos-23.4.3/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/organizations.py` & `pontos-23.4.3/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/pull_requests.py` & `pontos-23.4.3/pontos/github/api/pull_requests.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 from collections import defaultdict
 from pathlib import Path
 from typing import AsyncIterator, Dict, Iterable, List, Optional, Union
 
 from pontos.github.api.client import GitHubAsyncREST
 from pontos.github.api.helper import JSON_OBJECT
 from pontos.github.models.base import FileStatus
-from pontos.github.models.pull_request import PullRequest, PullRequestCommit
+from pontos.github.models.pull_request import (
+    Comment,
+    PullRequest,
+    PullRequestCommit,
+)
 
 
 class GitHubAsyncRESTPullRequests(GitHubAsyncREST):
     async def exists(self, repo: str, pull_request: Union[int, str]) -> bool:
         """
         Check if a single branch in a repository exists
 
@@ -223,18 +227,20 @@
 
         response = await self._client.post(api, data=data)
         response.raise_for_status()
         return PullRequest.from_dict(response.json())
 
     async def add_comment(
         self, repo: str, pull_request: Union[int, str], comment: str
-    ) -> None:
+    ) -> Comment:
         """
         Add a comment to a pull request on GitHub
 
+        https://docs.github.com/en/rest/issues/comments#create-an-issue-comment
+
         Args:
             repo: GitHub repository (owner/name) to use
             pull_request: Pull request number where to add a comment
             comment: The actual comment message. Can be formatted in Markdown.
 
         Raises:
             httpx.HTTPStatusError if the request was invalid
@@ -251,14 +257,86 @@
                         "A new comment for the pull request",
                     )
         """
         api = f"/repos/{repo}/issues/{pull_request}/comments"
         data: JSON_OBJECT = {"body": comment}
         response = await self._client.post(api, data=data)
         response.raise_for_status()
+        return Comment.from_dict(response.json())
+
+    async def update_comment(
+        self, repo: str, comment_id: Union[str, int], comment: str
+    ) -> Comment:
+        """
+        Update a comment to a pull request on GitHub
+
+        https://docs.github.com/en/rest/issues/comments#update-an-issue-comment
+
+        Args:
+            repo: GitHub repository (owner/name) to use
+            comment_id: The unique identifier of the comment
+            comment: The actual comment message. Can be formatted in Markdown.
+
+        Raises:
+            httpx.HTTPStatusError if the request was invalid
+
+        Example:
+            .. code-block:: python
+
+                from pontos.github.api import GitHubAsyncRESTApi
+
+                async with GitHubAsyncRESTApi(token) as api:
+                    await api.pull_requests.update_comment(
+                        "foo/bar",
+                        123,
+                        "A new comment for the pull request",
+                    )
+        """
+        api = f"/repos/{repo}/issues/comments/{comment_id}"
+        data: JSON_OBJECT = {"body": comment}
+        response = await self._client.post(api, data=data)
+        response.raise_for_status()
+        return Comment.from_dict(response.json())
+
+    async def comments(
+        self, repo: str, pull_request: Union[int, str]
+    ) -> AsyncIterator[Comment]:
+        """
+        Get all comments of a pull request on GitHub
+
+        https://docs.github.com/en/rest/issues/comments#list-issue-comments
+
+        Args:
+            repo: GitHub repository (owner/name) to use
+            pull_request: Pull request number where to add a comment
+
+        Raises:
+            httpx.HTTPStatusError if the request was invalid
+
+        Example:
+            .. code-block:: python
+
+                from pontos.github.api import GitHubAsyncRESTApi
+
+                async with GitHubAsyncRESTApi(token) as api:
+                    async for comment in api.pull_requests.comments(
+                        "foo/bar",
+                        123,
+                    ):
+                        print(comment)
+        """
+        params = {"per_page": "100"}
+        api = f"/repos/{repo}/issues/{pull_request}/comments"
+
+        async for response in self._client.get_all(api, params=params):
+            response.raise_for_status()
+
+            for comment in response.json():
+                print(comment)
+                yield Comment.from_dict(comment)
 
     async def files(
         self,
         repo: str,
         pull_request: Union[int, str],
         *,
         status_list: Optional[Iterable[FileStatus]] = None,
@@ -293,14 +371,16 @@
         # per default github only shows 35 files per page and at max it is only
         # possible to receive 100
         params = {"per_page": "100"}
         api = f"/repos/{repo}/pulls/{pull_request}/files"
         file_dict: Dict[FileStatus, List[Path]] = defaultdict(list)
 
         async for response in self._client.get_all(api, params=params):
+            response.raise_for_status()
+
             for f in response.json():
                 try:
                     status = FileStatus(f["status"])
                 except ValueError:
                     # unknown status
                     continue
```

### Comparing `pontos-23.4.2/pontos/github/api/release.py` & `pontos-23.4.3/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/repositories.py` & `pontos-23.4.3/pontos/github/api/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/search.py` & `pontos-23.4.3/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/tags.py` & `pontos-23.4.3/pontos/github/api/tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/teams.py` & `pontos-23.4.3/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/api/workflows.py` & `pontos-23.4.3/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/argparser.py` & `pontos-23.4.3/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/cmds.py` & `pontos-23.4.3/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/main.py` & `pontos-23.4.3/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/models/__init__.py` & `pontos-23.4.3/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/models/artifact.py` & `pontos-23.4.3/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/models/base.py` & `pontos-23.4.3/pontos/github/models/base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/models/branch.py` & `pontos-23.4.3/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/models/organization.py` & `pontos-23.4.3/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/models/pull_request.py` & `pontos-23.4.3/pontos/github/models/pull_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from pontos.github.models.base import FileStatus, GitHubModel, Team, User
 from pontos.github.models.organization import Repository
 
 __all__ = (
     "AuthorAssociation",
     "AutoMerge",
+    "Comment",
     "DiffEntry",
     "Label",
     "MergeMethod",
     "Milestone",
     "MilestoneState",
     "PullRequest",
     "PullRequestCommit",
@@ -345,14 +346,72 @@
     FIRST_TIME_CONTRIBUTOR = "FIRST_TIME_CONTRIBUTOR"
     MANNEQUIN = "MANNEQUIN"
     MEMBER = "MEMBER"
     NONE = "NONE"
     OWNER = "OWNER"
 
 
+@dataclass
+class Reactions(GitHubModel):
+    """
+    Reaction Rollup
+
+    Attributes:
+        url: URL to the reactions
+        total_count: int
+        laugh: int
+        confused: int
+        heart: int
+        hooray: int
+        eyes: int
+        rocket: int
+    """
+
+    url: str
+    total_count: int
+    laugh: int
+    confused: int
+    heart: int
+    hooray: int
+    eyes: int
+    rocket: int
+
+
+@dataclass
+class Comment(GitHubModel):
+    """
+    A single comment of a pull request/issue
+
+    Attributes:
+        id: Unique identifier of the comment
+        node_id: Node ID of the comment
+        url: URL for the issue comment
+        body: Contents of the issue comment
+        html_url: URL to the web page of the comment
+        created_at: Creation date
+        updated_at: Last modification date
+        issue_url: URL to the pull request
+        author_association: How the author is associated with the repository
+        user: Author of the comment
+        reactions: Reactions to the comment
+    """
+
+    id: int
+    node_id: str
+    url: str
+    html_url: str
+    issue_url: str
+    created_at: datetime
+    updated_at: datetime
+    author_association: AuthorAssociation
+    body: Optional[str] = None
+    user: Optional[User] = None
+    reactions: Optional[Reactions] = None
+
+
 class MergeMethod(Enum):
     """
     The (auto) merge method
 
     Attributes:
         MERGE: Create a merge commit
         SQUASH: Squash commits into a single commit
```

### Comparing `pontos-23.4.2/pontos/github/models/release.py` & `pontos-23.4.3/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/models/search.py` & `pontos-23.4.3/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/models/tag.py` & `pontos-23.4.3/pontos/github/models/tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/models/workflow.py` & `pontos-23.4.3/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/pr_template.md` & `pontos-23.4.3/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/script/__init__.py` & `pontos-23.4.3/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/script/errors.py` & `pontos-23.4.3/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/script/load.py` & `pontos-23.4.3/pontos/github/script/load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/github/script/parser.py` & `pontos-23.4.3/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/helper.py` & `pontos-23.4.3/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/models/__init__.py` & `pontos-23.4.3/pontos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/nvd/__init__.py` & `pontos-23.4.3/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/nvd/api.py` & `pontos-23.4.3/pontos/nvd/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/nvd/cpe/__init__.py` & `pontos-23.4.3/pontos/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/nvd/cpe/api.py` & `pontos-23.4.3/pontos/nvd/cpe/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/nvd/cve/__init__.py` & `pontos-23.4.3/pontos/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/nvd/cve/api.py` & `pontos-23.4.3/pontos/nvd/cve/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/nvd/models/__init__.py` & `pontos-23.4.3/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/nvd/models/cpe.py` & `pontos-23.4.3/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/nvd/models/cve.py` & `pontos-23.4.3/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/nvd/models/cvss_v2.py` & `pontos-23.4.3/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/nvd/models/cvss_v3.py` & `pontos-23.4.3/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/pontos.py` & `pontos-23.4.3/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/release/__init__.py` & `pontos-23.4.3/pontos/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/release/helper.py` & `pontos-23.4.3/pontos/release/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/release/main.py` & `pontos-23.4.3/pontos/release/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/release/parser.py` & `pontos-23.4.3/pontos/release/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/release/release.py` & `pontos-23.4.3/pontos/release/release.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 import asyncio
 from argparse import Namespace
 from enum import IntEnum, auto
 from pathlib import Path
-from typing import Optional
+from typing import Iterable, Optional
 
 import httpx
 
 from pontos.changelog.conventional_commits import ChangelogBuilder
 from pontos.errors import PontosError
 from pontos.git import Git
 from pontos.github.api import GitHubAsyncRESTApi
 from pontos.terminal import Terminal
 from pontos.version import Version, VersionCalculator, VersionError
-from pontos.version.helper import get_last_release_version
+from pontos.version.helper import get_last_release_versions
 from pontos.version.project import Project
 from pontos.version.schemes import VersioningScheme
 
 from .helper import ReleaseType, find_signing_key, get_git_repository_name
 
 
 class ReleaseReturnValue(IntEnum):
@@ -48,14 +48,24 @@
     NO_RELEASE_VERSION = auto()
     ALREADY_TAKEN = auto()
     CREATE_RELEASE_ERROR = auto()
     UPDATE_VERSION_ERROR = auto()
     UPDATE_VERSION_AFTER_RELEASE_ERROR = auto()
 
 
+def _get_version(
+    release_version: Version, last_release_versions: Iterable[Version]
+) -> Optional[Version]:
+    for version in last_release_versions:
+        if release_version > version:
+            return version
+
+    return None
+
+
 class ReleaseCommand:
     """
     A CLI command for creating a release
 
     Args:
         terminal: A Terminal for output
     """
@@ -131,14 +141,82 @@
             repo,
             git_version,
             name=f"{self.project} {release_version}",
             body=release_text,
             prerelease=release_version.is_pre_release,
         )
 
+    def _get_last_release(
+        self,
+        release_type: ReleaseType,
+        release_version: Version,
+        calculator: VersionCalculator,
+    ) -> Version:
+        # try to get last tag for the matching release series
+        if release_type in [
+            ReleaseType.PATCH,
+            ReleaseType.ALPHA,
+            ReleaseType.BETA,
+            ReleaseType.RELEASE_CANDIDATE,
+        ]:
+            tag_name = (
+                f"{self.git_tag_prefix}"
+                f"{release_version.major}.{release_version.minor}.*"
+            )
+        elif release_type == ReleaseType.MINOR:
+            tag_name = f"{self.git_tag_prefix}{release_version.major}.*"
+        else:
+            tag_name = None
+
+        last_release_versions = get_last_release_versions(
+            calculator.version_from_string,
+            git_tag_prefix=self.git_tag_prefix,
+            ignore_pre_releases=not release_version.is_pre_release,
+            tag_name=tag_name,
+        )
+
+        last_release_version = _get_version(
+            release_version, last_release_versions
+        )
+
+        if tag_name and not last_release_version:
+            if release_type in [
+                ReleaseType.PATCH,
+                ReleaseType.ALPHA,
+                ReleaseType.BETA,
+                ReleaseType.RELEASE_CANDIDATE,
+            ]:
+                tag_name = f"{self.git_tag_prefix}{release_version.major}.*"
+            else:
+                tag_name = None
+
+            last_release_versions = get_last_release_versions(
+                calculator.version_from_string,
+                git_tag_prefix=self.git_tag_prefix,
+                ignore_pre_releases=not release_version.is_pre_release,
+                tag_name=tag_name,
+            )
+
+            last_release_version = _get_version(
+                release_version, last_release_versions
+            )
+
+            if not last_release_version:
+                last_release_versions = get_last_release_versions(
+                    calculator.version_from_string,
+                    git_tag_prefix=self.git_tag_prefix,
+                    ignore_pre_releases=not release_version.is_pre_release,
+                )
+
+                last_release_version = _get_version(
+                    release_version, last_release_versions
+                )
+
+        return last_release_version
+
     async def run(
         self,
         *,
         token: str,
         space: str,
         project: Optional[str],
         versioning_scheme: VersioningScheme,
@@ -235,29 +313,18 @@
                 self.git.add(path)
         except VersionError as e:
             self.terminal.error(
                 f"Unable to update version to {release_version}. {e}"
             )
             return ReleaseReturnValue.UPDATE_VERSION_ERROR
 
-        if release_type == ReleaseType.PATCH:
-            tag_name = (
-                f"{self.git_tag_prefix}"
-                f"{release_version.major}.{release_version.minor}.*"
-            )
-        elif release_type == ReleaseType.MINOR:
-            tag_name = f"{self.git_tag_prefix}{release_version.major}.*"
-        else:
-            tag_name = None
-
-        last_release_version = get_last_release_version(
-            calculator.version_from_string,
-            git_tag_prefix=self.git_tag_prefix,
-            ignore_pre_releases=not release_version.is_pre_release,
-            tag_name=tag_name,
+        last_release_version = self._get_last_release(
+            release_type=release_type,
+            release_version=release_version,
+            calculator=calculator,
         )
 
         if not last_release_version:
             self.terminal.info(
                 f"No last release found. Creating changelog for the initial "
                 f"release {release_version}"
             )
```

### Comparing `pontos-23.4.2/pontos/release/sign.py` & `pontos-23.4.3/pontos/release/sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/terminal/__init__.py` & `pontos-23.4.3/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/terminal/null.py` & `pontos-23.4.3/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/terminal/rich.py` & `pontos-23.4.3/pontos/terminal/rich.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/terminal/terminal.py` & `pontos-23.4.3/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/testing/__init__.py` & `pontos-23.4.3/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/__init__.py` & `pontos-23.4.3/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/__main__.py` & `pontos-23.4.3/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash` & `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.c` & `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.c`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake` & `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.go` & `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.go`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.h` & `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.h`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.js` & `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.js`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl` & `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.po` & `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.po`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.py` & `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh` & `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt` & `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml` & `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl` & `pontos-23.4.3/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-only/template.c` & `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-only/template.c`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-only/template.h` & `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-only/template.h`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.bash` & `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.bash`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.c` & `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.c`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake` & `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.h` & `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.h`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.js` & `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.js`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl` & `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.po` & `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.po`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.py` & `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.sh` & `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.sh`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.txt` & `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.txt`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xml` & `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.xml`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl` & `pontos-23.4.3/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.bash` & `pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.bash`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.c` & `pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.c`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake` & `pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.go` & `pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.go`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.h` & `pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.h`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.js` & `pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.js`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl` & `pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.po` & `pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.po`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.py` & `pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.sh` & `pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.sh`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.txt` & `pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.txt`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xml` & `pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.xml`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl` & `pontos-23.4.3/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/updateheader/updateheader.py` & `pontos-23.4.3/pontos/updateheader/updateheader.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/__init__.py` & `pontos-23.4.3/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/__main__.py` & `pontos-23.4.3/pontos/version/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/_calculator.py` & `pontos-23.4.3/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/commands/__init__.py` & `pontos-23.4.3/pontos/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/commands/_cmake.py` & `pontos-23.4.3/pontos/version/commands/_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/commands/_command.py` & `pontos-23.4.3/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/commands/_go.py` & `pontos-23.4.3/pontos/version/commands/_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/commands/_javascript.py` & `pontos-23.4.3/pontos/version/commands/_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/commands/_python.py` & `pontos-23.4.3/pontos/version/commands/_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/errors.py` & `pontos-23.4.3/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/helper.py` & `pontos-23.4.3/pontos/version/helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,44 +21,75 @@
 
 from pontos.git import Git, TagSort
 from pontos.git.git import DEFAULT_TAG_SORT_SUFFIX
 
 from .version import ParseVersionFuncType, Version
 
 
-def get_last_release_version(
+def get_last_release_versions(
     parse_version: ParseVersionFuncType,
     *,
     git_tag_prefix: Optional[str] = "",
     ignore_pre_releases: Optional[bool] = False,
     tag_name: Optional[str] = None,
-) -> Optional[Version]:
-    """Get the last released Version from git.
+) -> list[Version]:
+    """Get the last released Versions from git.
 
     Args:
         git_tag_prefix: Git tag prefix to consider
         ignore_pre_release: Ignore pre releases and only consider non pre
             releases. Default is False.
         tag_name: A pattern for filtering the tags. For example: "1.2.*"
 
     Returns:
-        Last released git tag as Version if tags were found
-        or None
+        List of released versions
     """
 
     tag_list = Git().list_tags(
         sort=TagSort.VERSION,
         sort_suffix=DEFAULT_TAG_SORT_SUFFIX,
         tag_name=tag_name,
     )
+    tag_list.reverse()
+
+    tags = []
 
-    while tag_list:
-        last_release_version = tag_list[-1]
-        last_release_version = last_release_version.strip(git_tag_prefix)
+    for tag in tag_list:
+        last_release_version = tag.strip(git_tag_prefix)
 
         version = parse_version(last_release_version)
-        if not version.is_pre_release or not ignore_pre_releases:
-            return version
+        if version.is_pre_release and ignore_pre_releases:
+            continue
+
+        tags.append(version)
+
+    return tags
 
-        tag_list = tag_list[:-1]
 
-    return None
+def get_last_release_version(
+    parse_version: ParseVersionFuncType,
+    *,
+    git_tag_prefix: Optional[str] = "",
+    ignore_pre_releases: Optional[bool] = False,
+    tag_name: Optional[str] = None,
+) -> Optional[Version]:
+    """Get the last released Version from git.
+
+    Args:
+        git_tag_prefix: Git tag prefix to consider
+        ignore_pre_release: Ignore pre releases and only consider non pre
+            releases. Default is False.
+        tag_name: A pattern for filtering the tags. For example: "1.2.*"
+
+    Returns:
+        Last released git tag as Version if tags were found
+        or None
+    """
+
+    versions = get_last_release_versions(
+        parse_version=parse_version,
+        git_tag_prefix=git_tag_prefix,
+        ignore_pre_releases=ignore_pre_releases,
+        tag_name=tag_name,
+    )
+
+    return versions[0] if versions else None
```

### Comparing `pontos-23.4.2/pontos/version/main.py` & `pontos-23.4.3/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/parser.py` & `pontos-23.4.3/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/project.py` & `pontos-23.4.3/pontos/version/project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/schemes/__init__.py` & `pontos-23.4.3/pontos/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/schemes/_pep440.py` & `pontos-23.4.3/pontos/version/schemes/_pep440.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,21 @@
             return True
         if not isinstance(other, Version):
             raise ValueError(f"Can't compare {type(self)} with {type(other)}")
         if not isinstance(other, type(self)):
             other = self.from_version(other)
         return self._version != other._version
 
+    def __gt__(self, other: Any) -> bool:
+        if not isinstance(other, Version):
+            raise ValueError(f"Can't compare {type(self)} with {type(other)}")
+        if not isinstance(other, type(self)):
+            other = self.from_version(other)
+        return self._version > other._version
+
     def __str__(self) -> str:
         return str(self._version)
 
 
 class PEP440VersionCalculator(VersionCalculator):
     version_cls = PEP440Version
```

### Comparing `pontos-23.4.2/pontos/version/schemes/_scheme.py` & `pontos-23.4.3/pontos/version/schemes/_scheme.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/pontos/version/schemes/_semantic.py` & `pontos-23.4.3/pontos/version/schemes/_semantic.py`

 * *Files 12% similar despite different names*

```diff
@@ -174,14 +174,58 @@
             other = self.from_version(other)
 
         return (
             self._version_info != other._version_info
             or self._version_info.build != other._version_info.build
         )
 
+    def __gt__(self, other: Any) -> bool:
+        if not isinstance(other, Version):
+            raise ValueError(f"Can't compare {type(self)} with {type(other)}")
+        if not isinstance(other, type(self)):
+            other = self.from_version(other)
+
+        if self._version_info.to_tuple()[:3] > other._version_info[:3]:
+            return True
+        if self._version_info.to_tuple()[:3] < other._version_info[:3]:
+            return False
+
+        # major, minor and patch are equal
+        if self.is_dev_release:
+            if not other.is_pre_release and not other.is_dev_release:
+                return False
+            if not self.is_pre_release and other.is_pre_release:
+                return False
+            if not self.is_pre_release:
+                return self.dev > other.dev
+
+            if self.is_pre_release:
+                if other.is_dev_release and self.pre == other.pre:
+                    return self.dev > other.dev
+                return self.pre > other.pre
+
+        # not a dev release
+        if self.is_pre_release:
+            if not other.is_pre_release and not other.is_dev_release:
+                return False
+
+            if other.is_pre_release:
+                if other.is_dev_release:
+                    return self.pre >= other.pre
+                return self.pre > other.pre
+
+            # other is a dev release
+            return True
+
+        if other.is_dev_release or other.is_pre_release:
+            return True
+
+        # both are equal
+        return False
+
     def __str__(self) -> str:
         """A string representation of the version"""
         return str(self._version_info)
 
     @classmethod
     def from_string(cls, version: str) -> "SemanticVersion":
         """
```

### Comparing `pontos-23.4.2/pontos/version/version.py` & `pontos-23.4.3/pontos/version/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,18 @@
         pass
 
     @abstractmethod
     def __ne__(self, other: Any) -> bool:
         pass
 
     @abstractmethod
+    def __gt__(self, other: Any) -> bool:
+        pass
+
+    @abstractmethod
     def __str__(self) -> str:
         """A string representation of the version"""
 
     def __repr__(self) -> str:
         """A representation of the Version"""
         return f"<{self.__class__.__name__}('{self}')>"
```

### Comparing `pontos-23.4.2/pyproject.toml` & `pontos-23.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.4.2"
+version = "23.4.3"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
```

### Comparing `pontos-23.4.2/scripts/github/artifacts-download.py` & `pontos-23.4.3/scripts/github/artifacts-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/scripts/github/artifacts.py` & `pontos-23.4.3/scripts/github/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/scripts/github/branchprotection.py` & `pontos-23.4.3/scripts/github/branchprotection.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/scripts/github/create-repository.py` & `pontos-23.4.3/scripts/github/create-repository.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/scripts/github/enforce-admins.py` & `pontos-23.4.3/scripts/github/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/scripts/github/lock-branch.py` & `pontos-23.4.3/scripts/github/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/scripts/github/members.py` & `pontos-23.4.3/scripts/github/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/scripts/github/release-assets-download.py` & `pontos-23.4.3/scripts/github/release-assets-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/scripts/github/repositories.py` & `pontos-23.4.3/scripts/github/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/scripts/github/search-repositories.py` & `pontos-23.4.3/scripts/github/search-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/scripts/github/team-repositories.py` & `pontos-23.4.3/scripts/github/team-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/scripts/github/teams.py` & `pontos-23.4.3/scripts/github/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/scripts/github/workflow-runs.py` & `pontos-23.4.3/scripts/github/workflow-runs.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/__init__.py` & `pontos-23.4.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/changelog/__init__.py` & `pontos-23.4.3/tests/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/changelog/test_conventional_commits.py` & `pontos-23.4.3/tests/changelog/test_conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/changelog/test_parser.py` & `pontos-23.4.3/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/git/__init__.py` & `pontos-23.4.3/tests/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/git/test_git.py` & `pontos-23.4.3/tests/git/test_git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/git/test_status.py` & `pontos-23.4.3/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/__init__.py` & `pontos-23.4.3/tests/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/actions/__init__.py` & `pontos-23.4.3/tests/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/actions/test-pull-request-event.json` & `pontos-23.4.3/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/actions/test_core.py` & `pontos-23.4.3/tests/github/actions/test_core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/actions/test_env.py` & `pontos-23.4.3/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/actions/test_event.py` & `pontos-23.4.3/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/__init__.py` & `pontos-23.4.3/tests/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/pr-files.json` & `pontos-23.4.3/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/release-response.json` & `pontos-23.4.3/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/test_artifacts.py` & `pontos-23.4.3/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/test_branch.py` & `pontos-23.4.3/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/test_client.py` & `pontos-23.4.3/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/test_contents.py` & `pontos-23.4.3/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/test_labels.py` & `pontos-23.4.3/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/test_organizations.py` & `pontos-23.4.3/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/test_pull_requests.py` & `pontos-23.4.3/tests/github/api/test_pull_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Greenbone AG
+# Copyright (C) 2022-2023 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -549,14 +549,46 @@
     "maintainer_can_modify": True,
     "commits": 3,
     "additions": 100,
     "deletions": 3,
     "changed_files": 5,
 }
 
+COMMENT_JSON = {
+    "id": 1,
+    "node_id": "MDEyOklzc3VlQ29tbWVudDE=",
+    "url": "https://api.github.com/repos/octocat/Hello-World/issues/comments/1",
+    "html_url": "https://github.com/octocat/Hello-World/issues/1347#issuecomment-1",
+    "body": "Me too",
+    "user": {
+        "login": "octocat",
+        "id": 1,
+        "node_id": "MDQ6VXNlcjE=",
+        "avatar_url": "https://github.com/images/error/octocat_happy.gif",
+        "gravatar_id": "",
+        "url": "https://api.github.com/users/octocat",
+        "html_url": "https://github.com/octocat",
+        "followers_url": "https://api.github.com/users/octocat/followers",
+        "following_url": "https://api.github.com/users/octocat/following{/other_user}",
+        "gists_url": "https://api.github.com/users/octocat/gists{/gist_id}",
+        "starred_url": "https://api.github.com/users/octocat/starred{/owner}{/repo}",
+        "subscriptions_url": "https://api.github.com/users/octocat/subscriptions",
+        "organizations_url": "https://api.github.com/users/octocat/orgs",
+        "repos_url": "https://api.github.com/users/octocat/repos",
+        "events_url": "https://api.github.com/users/octocat/events{/privacy}",
+        "received_events_url": "https://api.github.com/users/octocat/received_events",
+        "type": "User",
+        "site_admin": False,
+    },
+    "created_at": "2011-04-14T16:00:49Z",
+    "updated_at": "2011-04-14T16:00:49Z",
+    "issue_url": "https://api.github.com/repos/octocat/Hello-World/issues/1347",
+    "author_association": "COLLABORATOR",
+}
+
 
 class GitHubAsyncRESTPullRequestsTestCase(GitHubAsyncRESTTestCase):
     api_cls = GitHubAsyncRESTPullRequests
 
     async def test_exists(self):
         response = create_response(is_success=True)
         self.client.get.return_value = response
@@ -947,29 +979,32 @@
                 "title": "Lorem",
                 "body": "Ipsum",
             },
         )
 
     async def test_add_comment(self):
         response = create_response()
+        response.json.return_value = COMMENT_JSON
         self.client.post.return_value = response
 
-        await self.api.add_comment(
+        comment = await self.api.add_comment(
             "foo/bar",
             123,
             "Lorem Ipsum",
         )
 
         self.client.post.assert_awaited_once_with(
             "/repos/foo/bar/issues/123/comments",
             data={
                 "body": "Lorem Ipsum",
             },
         )
 
+        self.assertEqual(comment.id, 1)
+
     async def test_add_comment_failure(self):
         response = create_response()
         self.client.post.side_effect = HTTPStatusError(
             "404", request=MagicMock(), response=response
         )
 
         with self.assertRaises(HTTPStatusError):
@@ -982,14 +1017,128 @@
         self.client.post.assert_awaited_once_with(
             "/repos/foo/bar/issues/123/comments",
             data={
                 "body": "Lorem Ipsum",
             },
         )
 
+    async def test_update_comment(self):
+        response = create_response()
+        response.json.return_value = COMMENT_JSON
+        self.client.post.return_value = response
+
+        comment = await self.api.update_comment(
+            "foo/bar",
+            123,
+            "Lorem Ipsum",
+        )
+
+        self.client.post.assert_awaited_once_with(
+            "/repos/foo/bar/issues/comments/123",
+            data={
+                "body": "Lorem Ipsum",
+            },
+        )
+
+        self.assertEqual(comment.id, 1)
+
+    async def test_update_comment_failure(self):
+        response = create_response()
+        self.client.post.side_effect = HTTPStatusError(
+            "404", request=MagicMock(), response=response
+        )
+
+        with self.assertRaises(HTTPStatusError):
+            await self.api.update_comment(
+                "foo/bar",
+                123,
+                "Lorem Ipsum",
+            )
+
+        self.client.post.assert_awaited_once_with(
+            "/repos/foo/bar/issues/comments/123",
+            data={
+                "body": "Lorem Ipsum",
+            },
+        )
+
+    async def test_comments(self):
+        response1 = create_response()
+        response1.json.return_value = [
+            {
+                "id": 1,
+                "node_id": "MDEyOklzc3VlQ29tbWVudDE=",
+                "url": "https://api.github.com/repos/octocat/Hello-World/issues/comments/1",
+                "html_url": "https://github.com/octocat/Hello-World/issues/1347#issuecomment-1",
+                "body": "Me too",
+                "created_at": "2011-04-14T16:00:49Z",
+                "updated_at": "2011-04-14T16:00:49Z",
+                "issue_url": "https://api.github.com/repos/octocat/Hello-World/issues/1347",
+                "author_association": "COLLABORATOR",
+            },
+            {
+                "id": 2,
+                "node_id": "MDEyOklzc3VlQ29tbWVudDE=",
+                "url": "https://api.github.com/repos/octocat/Hello-World/issues/comments/2",
+                "html_url": "https://github.com/octocat/Hello-World/issues/1347#issuecomment-2",
+                "body": "Me too",
+                "created_at": "2011-04-14T16:00:49Z",
+                "updated_at": "2011-04-14T16:00:49Z",
+                "issue_url": "https://api.github.com/repos/octocat/Hello-World/issues/1347",
+                "author_association": "COLLABORATOR",
+            },
+        ]
+        response2 = create_response()
+        response2.json.return_value = [
+            {
+                "id": 3,
+                "node_id": "MDEyOklzc3VlQ29tbWVudDE=",
+                "url": "https://api.github.com/repos/octocat/Hello-World/issues/comments/3",
+                "html_url": "https://github.com/octocat/Hello-World/issues/1347#issuecomment-3",
+                "body": "Me too",
+                "created_at": "2011-04-14T16:00:49Z",
+                "updated_at": "2011-04-14T16:00:49Z",
+                "issue_url": "https://api.github.com/repos/octocat/Hello-World/issues/1347",
+                "author_association": "COLLABORATOR",
+            },
+        ]
+
+        self.client.get_all.return_value = AsyncIteratorMock(
+            [response1, response2]
+        )
+
+        it = aiter(self.api.comments("foo/bar", 123))
+
+        comment = await anext(it)
+        self.assertEqual(comment.id, 1)
+
+        comment = await anext(it)
+        self.assertEqual(comment.id, 2)
+
+        comment = await anext(it)
+        self.assertEqual(comment.id, 3)
+
+        with self.assertRaises(StopAsyncIteration):
+            await anext(it)
+
+        self.client.get_all.assert_called_once_with(
+            "/repos/foo/bar/issues/123/comments",
+            params={"per_page": "100"},
+        )
+
+    async def test_comments_failure(self):
+        response = create_response()
+        self.client.get_all.side_effect = [
+            HTTPStatusError("404", request=MagicMock(), response=response)
+        ]
+
+        it = aiter(self.api.comments("foo/bar", 123))
+        with self.assertRaises(HTTPStatusError):
+            await anext(it)
+
     async def test_files(self):
         response1 = create_response()
         response1.json.return_value = [
             {"filename": "baz", "status": FileStatus.MODIFIED.value}
         ]
         response2 = create_response()
         response2.json.return_value = [
@@ -1009,14 +1158,23 @@
         self.assertEqual(len(files[FileStatus.ADDED]), 0)
 
         self.client.get_all.assert_called_once_with(
             "/repos/foo/bar/pulls/123/files",
             params={"per_page": "100"},
         )
 
+    async def test_files_failure(self):
+        response = create_response()
+        self.client.get_all.side_effect = [
+            HTTPStatusError("404", request=MagicMock(), response=response)
+        ]
+
+        with self.assertRaises(HTTPStatusError):
+            await self.api.files("foo/bar", 123)
+
     async def test_files_with_status_list(self):
         response1 = create_response()
         response1.json.return_value = [
             {"filename": "baz", "status": FileStatus.MODIFIED.value}
         ]
         response2 = create_response()
         response2.json.return_value = [
```

### Comparing `pontos-23.4.2/tests/github/api/test_release.py` & `pontos-23.4.3/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/test_repositories.py` & `pontos-23.4.3/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/test_search.py` & `pontos-23.4.3/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/test_tags.py` & `pontos-23.4.3/tests/github/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/test_teams.py` & `pontos-23.4.3/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/api/test_workflows.py` & `pontos-23.4.3/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/models/__init__.py` & `pontos-23.4.3/tests/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/models/test_artifact.py` & `pontos-23.4.3/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/models/test_base.py` & `pontos-23.4.3/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/models/test_branch.py` & `pontos-23.4.3/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/models/test_organization.py` & `pontos-23.4.3/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/models/test_pull_request.py` & `pontos-23.4.3/tests/github/models/test_pull_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 import unittest
 from datetime import datetime, timezone
 
 from pontos.github.models.base import Permission, TeamPrivacy
 from pontos.github.models.pull_request import (
     AuthorAssociation,
+    Comment,
     MilestoneState,
     PullRequest,
     PullRequestState,
 )
 
 
 class PullRequestTestCase(unittest.TestCase):
@@ -1605,7 +1606,109 @@
         )
         self.assertEqual(
             user.received_events_url,
             "https://api.github.com/users/octocat/received_events",
         )
         self.assertEqual(user.type, "User")
         self.assertFalse(user.site_admin)
+
+
+class CommentTestCase(unittest.TestCase):
+    def test_from_dict(self):
+        data = {
+            "id": 1,
+            "node_id": "MDEyOklzc3VlQ29tbWVudDE=",
+            "url": "https://api.github.com/repos/octocat/Hello-World/issues/comments/1",
+            "html_url": "https://github.com/octocat/Hello-World/issues/1347#issuecomment-1",
+            "body": "Me too",
+            "user": {
+                "login": "octocat",
+                "id": 1,
+                "node_id": "MDQ6VXNlcjE=",
+                "avatar_url": "https://github.com/images/error/octocat_happy.gif",
+                "gravatar_id": "",
+                "url": "https://api.github.com/users/octocat",
+                "html_url": "https://github.com/octocat",
+                "followers_url": "https://api.github.com/users/octocat/followers",
+                "following_url": "https://api.github.com/users/octocat/following{/other_user}",
+                "gists_url": "https://api.github.com/users/octocat/gists{/gist_id}",
+                "starred_url": "https://api.github.com/users/octocat/starred{/owner}{/repo}",
+                "subscriptions_url": "https://api.github.com/users/octocat/subscriptions",
+                "organizations_url": "https://api.github.com/users/octocat/orgs",
+                "repos_url": "https://api.github.com/users/octocat/repos",
+                "events_url": "https://api.github.com/users/octocat/events{/privacy}",
+                "received_events_url": "https://api.github.com/users/octocat/received_events",
+                "type": "User",
+                "site_admin": False,
+            },
+            "created_at": "2011-04-14T16:00:49Z",
+            "updated_at": "2011-04-14T16:00:49Z",
+            "issue_url": "https://api.github.com/repos/octocat/Hello-World/issues/1347",
+            "author_association": "COLLABORATOR",
+        }
+        comment = Comment.from_dict(data)
+
+        self.assertEqual(comment.id, 1)
+        self.assertEqual(comment.node_id, "MDEyOklzc3VlQ29tbWVudDE=")
+        self.assertEqual(
+            comment.url,
+            "https://api.github.com/repos/octocat/Hello-World/issues/comments/1",
+        )
+        self.assertEqual(
+            comment.html_url,
+            "https://github.com/octocat/Hello-World/issues/1347#issuecomment-1",
+        )
+        self.assertEqual(comment.body, "Me too")
+
+        user = comment.user
+        self.assertEqual(user.login, "octocat")
+        self.assertEqual(user.id, 1)
+        self.assertEqual(user.node_id, "MDQ6VXNlcjE=")
+        self.assertEqual(
+            user.avatar_url, "https://github.com/images/error/octocat_happy.gif"
+        )
+        self.assertEqual(user.gravatar_id, "")
+        self.assertEqual(user.url, "https://api.github.com/users/octocat")
+        self.assertEqual(user.html_url, "https://github.com/octocat")
+        self.assertEqual(
+            user.followers_url, "https://api.github.com/users/octocat/followers"
+        )
+        self.assertEqual(
+            user.following_url,
+            "https://api.github.com/users/octocat/following{/other_user}",
+        )
+        self.assertEqual(
+            user.gists_url,
+            "https://api.github.com/users/octocat/gists{/gist_id}",
+        )
+        self.assertEqual(
+            user.starred_url,
+            "https://api.github.com/users/octocat/starred{/owner}{/repo}",
+        )
+        self.assertEqual(
+            user.subscriptions_url,
+            "https://api.github.com/users/octocat/subscriptions",
+        )
+        self.assertEqual(
+            user.organizations_url, "https://api.github.com/users/octocat/orgs"
+        )
+        self.assertEqual(
+            user.repos_url, "https://api.github.com/users/octocat/repos"
+        )
+        self.assertEqual(
+            user.events_url,
+            "https://api.github.com/users/octocat/events{/privacy}",
+        )
+        self.assertEqual(
+            user.received_events_url,
+            "https://api.github.com/users/octocat/received_events",
+        )
+        self.assertEqual(user.type, "User")
+        self.assertFalse(user.site_admin)
+
+        self.assertEqual(
+            comment.issue_url,
+            "https://api.github.com/repos/octocat/Hello-World/issues/1347",
+        )
+        self.assertEqual(
+            comment.author_association, AuthorAssociation.COLLABORATOR
+        )
```

### Comparing `pontos-23.4.2/tests/github/models/test_release.py` & `pontos-23.4.3/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/models/test_search.py` & `pontos-23.4.3/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/models/test_tag.py` & `pontos-23.4.3/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/models/test_workflow.py` & `pontos-23.4.3/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/script/__init__.py` & `pontos-23.4.3/tests/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/script/test_load.py` & `pontos-23.4.3/tests/github/script/test_load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/script/test_parser.py` & `pontos-23.4.3/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/test_argparser.py` & `pontos-23.4.3/tests/github/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/github/test_cmds.py` & `pontos-23.4.3/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/models/__init__.py` & `pontos-23.4.3/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/models/test_models.py` & `pontos-23.4.3/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/nvd/__init__.py` & `pontos-23.4.3/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/nvd/cpe/__init__.py` & `pontos-23.4.3/tests/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/nvd/cpe/test_api.py` & `pontos-23.4.3/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/nvd/cve/__init__.py` & `pontos-23.4.3/tests/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/nvd/cve/test_api.py` & `pontos-23.4.3/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/nvd/models/__init__.py` & `pontos-23.4.3/tests/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/nvd/models/test_cpe.py` & `pontos-23.4.3/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/nvd/models/test_cve.py` & `pontos-23.4.3/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/nvd/test_api.py` & `pontos-23.4.3/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/release/__init__.py` & `pontos-23.4.3/tests/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/release/test_helper.py` & `pontos-23.4.3/tests/release/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/release/test_parser.py` & `pontos-23.4.3/tests/release/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/release/test_release.py` & `pontos-23.4.3/tests/release/test_release.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,37 +11,74 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-# pylint: disable=too-many-lines, line-too-long
+# pylint: disable=too-many-lines, line-too-long, invalid-name
 
 import unittest
+from contextlib import contextmanager
+from dataclasses import dataclass, field
 from datetime import datetime
+from pathlib import Path
+from typing import Optional
 from unittest.mock import AsyncMock, MagicMock, call, patch
 
 from httpx import HTTPStatusError, Request, Response
 
 from pontos.git.git import ConfigScope, Git
 from pontos.release.main import parse_args
 from pontos.release.release import ReleaseReturnValue, release
 from pontos.terminal.terminal import Terminal
 from pontos.testing import temp_git_repository
 from pontos.version import VersionError, VersionUpdate
 from pontos.version.commands import GoVersionCommand
-from pontos.version.schemes._pep440 import PEP440Version
+from pontos.version.schemes._pep440 import PEP440Version, PEP440VersioningScheme
 
 
 def mock_terminal() -> MagicMock:
     return MagicMock(spec=Terminal)
 
 
-@patch.dict("os.environ", {"GITHUB_TOKEN": "foo", "GITHUB_USER": "user"})
+@contextmanager
+def setup_go_project(*, current_version: str, tags: list[str] = None) -> Path:
+    with temp_git_repository() as tmp_git:
+        git = Git(tmp_git)
+
+        git.config("commit.gpgSign", "false", scope=ConfigScope.LOCAL)
+        git.config("tag.gpgSign", "false", scope=ConfigScope.LOCAL)
+        git.config("tag.sort", "refname", scope=ConfigScope.LOCAL)
+
+        git.add_remote("origin", "http://foo/bar.git")
+
+        go = GoVersionCommand(PEP440VersioningScheme)
+        go.project_file_path.touch()
+        update = go.update_version(new_version=PEP440Version(current_version))
+
+        git.add(update.changed_files)
+        git.add(go.project_file_path)
+        git.commit("Create initial release")
+
+        if tags:
+            for tag in tags:
+                git.tag(f"v{tag}")
+
+        yield tmp_git
+
+
+@patch.dict(
+    "os.environ",
+    {
+        "GITHUB_TOKEN": "foo",
+        "GITHUB_USER": "user",
+        "GPG_SIGNING_KEY": "1234",
+    },
+)
 class ReleaseTestCase(unittest.TestCase):
     @patch("pontos.release.release.Git", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog",
@@ -1068,14 +1105,16 @@
         with temp_git_repository():
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
+        self.assertEqual(released, ReleaseReturnValue.CREATE_RELEASE_ERROR)
+
         git_mock.return_value.push.assert_called_once_with(
             follow_tags=True, remote=None
         )
         git_mock.return_value.add.assert_called_once_with("MyProject.conf")
         git_mock.return_value.commit.assert_called_once_with(
             "Automatic release to 0.0.1", verify=False, gpg_signing_key="123"
         )
@@ -1084,16 +1123,14 @@
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
-        self.assertEqual(released, ReleaseReturnValue.CREATE_RELEASE_ERROR)
-
     @patch("pontos.release.release.Git", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch(
         "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
     )
@@ -1552,24 +1589,15 @@
         git_mock,
     ):
         release_version = PEP440Version("0.0.2")
 
         create_changelog_mock.return_value = "A Changelog"
         _, token, args = parse_args(["release", "--release-type", "patch"])
 
-        with temp_git_repository() as temp_dir:
-            git = Git()
-            git.config("user.signingkey", "1234", scope=ConfigScope.LOCAL)
-            git.add_remote("origin", "http://foo/bar.git")
-
-            go_mod = temp_dir / GoVersionCommand.project_file_name
-            go_mod.touch()
-            version_file = temp_dir / GoVersionCommand.version_file_path
-            version_file.write_text('var version = "0.0.1"', encoding="utf8")
-
+        with setup_go_project(current_version="0.0.1"):
             released = release(
                 terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
@@ -1595,24 +1623,24 @@
             (release_version, "foo", "A Changelog"),
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
 
     @patch("pontos.release.release.Git", autospec=True)
     @patch("pontos.changelog.conventional_commits.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.release.get_last_release_versions", autospec=True)
     @patch(
         "pontos.release.release.ReleaseCommand._create_release", autospec=True
     )
     @patch("pontos.release.release.Project._gather_commands", autospec=True)
     def test_release_with_changelog(
         self,
         gather_commands_mock: MagicMock,
         create_release_mock: AsyncMock,
-        get_last_release_version_mock: MagicMock,
+        get_last_release_versions_mock: MagicMock,
         cc_git_mock: MagicMock,
         git_mock: MagicMock,
     ):
         current_version = PEP440Version("0.0.1")
         release_version = PEP440Version("0.0.2")
         next_version = PEP440Version("1.0.0.dev1")
         command_mock = MagicMock(spec=GoVersionCommand)
@@ -1625,15 +1653,15 @@
             ),
             VersionUpdate(
                 previous=release_version,
                 new=next_version,
                 changed_files=["project.conf", "version.lang"],
             ),
         ]
-        get_last_release_version_mock.return_value = current_version
+        get_last_release_versions_mock.return_value = [current_version]
         cc_git_mock.return_value.log.return_value = [
             "1234567 Add: foo bar",
             "8abcdef Add: bar baz",
             "8abcd3f Add bar baz",
             "8abcd3d Adding bar baz",
             "1337abc Change: bar to baz",
             "42a42a4 Remove: foo bar again",
@@ -1805,7 +1833,189 @@
             gpg_signing_key="1234",
         )
         git_mock.return_value.tag.assert_called_once_with(
             "v0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
         self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+
+
+@dataclass
+class Release:
+    release_type: str
+    current_version: str
+    expected_release_version: str
+    expected_last_release_version: Optional[str] = None
+    tags: list[str] = field(default_factory=list)
+
+
+@patch.dict(
+    "os.environ",
+    {"GITHUB_TOKEN": "foo", "GITHUB_USER": "user", "GPG_SIGNING_KEY": ""},
+)
+class ReleaseGoProjectTestCase(unittest.TestCase):
+    @patch("pontos.release.release.Git.push", autospec=True)
+    @patch(
+        "pontos.release.release.GitHubAsyncRESTApi",
+        autospec=True,
+    )
+    def test_release(
+        self, github_api_mock: AsyncMock, _git_push_mock: MagicMock
+    ):
+        create_api_mock = AsyncMock()
+        github_api_mock.return_value.releases.create = create_api_mock
+
+        releases = [
+            Release("major", "1.0.0", "2.0.0"),
+            Release("minor", "1.0.0", "1.1.0"),
+            Release("patch", "1.0.0", "1.0.1"),
+            Release("patch", "1.0.5", "1.0.6"),
+            Release("alpha", "1.0.0", "1.0.1a1"),
+            Release("alpha", "1.0.0a3", "1.0.0a4"),
+            Release("beta", "1.0.0", "1.0.1b1"),
+            Release("beta", "1.0.0b2", "1.0.0b3"),
+            Release("release-candidate", "1.0.0", "1.0.1rc1"),
+            Release("release-candidate", "1.0.0rc1", "1.0.0rc2"),
+        ]
+
+        for r in releases:
+            with setup_go_project(current_version=r.current_version):
+                _, token, args = parse_args(
+                    ["release", "--release-type", r.release_type]
+                )
+                released = release(
+                    terminal=mock_terminal(),
+                    args=args,
+                    token=token,
+                )
+
+            self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+            self.assertEqual(
+                create_api_mock.call_args.args[1],
+                f"v{r.expected_release_version}",
+            )
+
+            create_api_mock.reset_mock()
+
+    @patch(
+        "pontos.release.release.ReleaseCommand._create_changelog",
+        autospec=True,
+    )
+    @patch("pontos.release.release.Git.push", autospec=True)
+    @patch(
+        "pontos.release.release.GitHubAsyncRESTApi",
+        autospec=True,
+    )
+    def test_release_series(
+        self,
+        github_api_mock: AsyncMock,
+        _git_push_mock: MagicMock,
+        create_changelog_mock: MagicMock,
+    ):
+        create_api_mock = AsyncMock()
+        github_api_mock.return_value.releases.create = create_api_mock
+
+        create_changelog_mock.return_value = "A Changelog"
+
+        releases = [
+            Release("major", "1.0.0", "2.0.0", "1.0.0", ["1.0.0", "3.0.0"]),
+            Release("major", "1.0.0rc1", "1.0.0", None, ["3.0.0"]),
+            Release("minor", "1.0.0", "1.1.0", "1.0.0", ["1.0.0", "2.0.0"]),
+            Release(
+                "minor", "1.1.0", "1.2.0", "1.1.0", ["1.0.0", "1.1.0", "2.0.0"]
+            ),
+            Release(
+                "patch", "1.0.0", "1.0.1", "1.0.0", ["1.0.0", "1.1.0", "2.0.0"]
+            ),
+            Release(
+                "patch", "1.0.5", "1.0.6", "1.0.5", ["1.0.5", "1.1.0", "2.0.0"]
+            ),
+            Release(
+                "patch", "1.0.5", "1.0.6", "1.0.3", ["1.0.3", "1.1.0", "2.0.0"]
+            ),
+            Release(
+                "patch",
+                "1.1.0rc1",
+                "1.1.0",
+                "1.0.0",
+                ["1.0.0", "1.2.0", "2.0.0"],
+            ),
+            Release(
+                "alpha",
+                "1.0.0",
+                "1.0.1a1",
+                "1.0.0",
+                ["1.0.0", "2.0.0", "1.1.0"],
+            ),
+            Release(
+                "alpha",
+                "1.0.0a3",
+                "1.0.0a4",
+                "1.0.0a3",
+                ["1.0.0a3", "2.0.0", "1.1.0"],
+            ),
+            Release(
+                "beta",
+                "1.0.0",
+                "1.0.1b1",
+                "1.0.0",
+                ["1.0.0", "2.0.0", "1.1.0"],
+            ),
+            Release(
+                "beta",
+                "1.0.0b2",
+                "1.0.0b3",
+                "1.0.0b2",
+                ["1.0.0b2", "2.0.0", "1.1.0"],
+            ),
+            Release(
+                "release-candidate",
+                "1.0.0",
+                "1.0.1rc1",
+                "1.0.0",
+                ["1.0.0", "2.0.0", "1.1.0"],
+            ),
+            Release(
+                "release-candidate",
+                "1.0.0rc1",
+                "1.0.0rc2",
+                "1.0.0rc1",
+                ["1.0.0rc1", "2.0.0", "1.1.0"],
+            ),
+        ]
+
+        for r in releases:
+            with setup_go_project(
+                current_version=r.current_version, tags=r.tags
+            ):
+                _, token, args = parse_args(
+                    ["release", "--release-type", r.release_type]
+                )
+                released = release(
+                    terminal=mock_terminal(),
+                    args=args,
+                    token=token,
+                )
+
+            self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+            self.assertEqual(
+                create_api_mock.call_args.args[1],
+                f"v{r.expected_release_version}",
+            )
+
+            self.assertEqual(
+                create_changelog_mock.call_args.args[1],
+                PEP440Version.from_string(r.expected_release_version),
+                f"Unexpected current release version {r}",
+            )
+
+            if r.expected_last_release_version is None:
+                self.assertIsNone(create_changelog_mock.call_args.args[2])
+            else:
+                self.assertEqual(
+                    create_changelog_mock.call_args.args[2],
+                    PEP440Version.from_string(r.expected_last_release_version),
+                    f"Unexpected last release version for {r}",
+                )
+
+            create_api_mock.reset_mock()
+            create_changelog_mock.reset_mock()
```

### Comparing `pontos-23.4.2/tests/release/test_sign.py` & `pontos-23.4.3/tests/release/test_sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/terminal/__init__.py` & `pontos-23.4.3/tests/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/terminal/test_terminal.py` & `pontos-23.4.3/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/test_helper.py` & `pontos-23.4.3/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/test_pontos.py` & `pontos-23.4.3/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/testing/__init__.py` & `pontos-23.4.3/tests/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/testing/test_testing.py` & `pontos-23.4.3/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/updateheader/__init__.py` & `pontos-23.4.3/tests/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/updateheader/test_header.py` & `pontos-23.4.3/tests/updateheader/test_header.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/version/__init__.py` & `pontos-23.4.3/tests/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/version/commands/__init__.py` & `pontos-23.4.3/tests/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/version/commands/test_cmake.py` & `pontos-23.4.3/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/version/commands/test_go.py` & `pontos-23.4.3/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/version/commands/test_javascript.py` & `pontos-23.4.3/tests/version/commands/test_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/version/commands/test_python.py` & `pontos-23.4.3/tests/version/commands/test_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/version/schemes/__init__.py` & `pontos-23.4.3/tests/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/version/schemes/test_pep440.py` & `pontos-23.4.3/tests/version/schemes/test_pep440.py`

 * *Files 16% similar despite different names*

```diff
@@ -230,14 +230,80 @@
             ("1.0.0", 1),
             ("1.0.0", True),
         ]
         for version1, version2 in versions:
             with self.assertRaisesRegex(ValueError, "Can't compare"):
                 self.assertFalse(Version.from_string(version1) != version2)
 
+    def test_greater_then(self):
+        versions = [
+            ("1.0.0", "0.9.9999"),
+            ("1.0.1", "1.0.0"),
+            ("1.0.0", "1.0.0.dev1"),
+            ("1.0.0", "1.0.0-alpha1"),
+            ("1.0.0", "1.0.0-alpha1"),
+            ("1.0.0", "1.0.0-beta1"),
+            ("1.0.0", "1.0.0-rc1"),
+            ("1.0.0-alpha1", "1.0.0-dev1"),
+            ("1.0.0-alpha1", "1.0.0-alpha1.dev1"),
+            ("1.0.0-alpha2", "1.0.0-alpha1"),
+            ("1.0.0-beta1", "1.0.0-dev1"),
+            ("1.0.0-beta1", "1.0.0-alpha1"),
+            ("1.0.0-beta1", "1.0.0-beta1.dev1"),
+            ("1.0.0-beta2", "1.0.0-beta1"),
+            ("1.0.0-rc1", "1.0.0-dev1"),
+            ("1.0.0-rc1", "1.0.0-alpha1"),
+            ("1.0.0-rc1", "1.0.0-beta1"),
+            ("1.0.0-rc1", "1.0.0-rc1.dev1"),
+            ("1.0.0-rc2", "1.0.0-rc1"),
+        ]
+        for version1, version2 in versions:
+            self.assertTrue(
+                Version.from_string(version1) > Version.from_string(version2),
+                f"{version1} should be greater then {version2}",
+            )
+
+        versions = [
+            ("1.0.0", "1.0.0"),
+            ("1.0.0", "1.0.0+dev1"),
+            ("1.0.0.dev1", "1.0.0.dev1"),
+            ("1.0.0.dev1", "1.0.0.dev2"),
+            ("1.0.0", "1.0.1"),
+            ("1.0.0-dev1", "1.0.0"),
+            ("1.0.0-dev1", "1.0.0-alpha1"),
+            ("1.0.0-dev1", "1.0.0-beta1"),
+            ("1.0.0-dev1", "1.0.0-rc1"),
+            ("1.0.0+dev1", "1.0.0+dev1"),
+            ("1.0.0+dev1", "1.0.0+dev2"),
+            ("1.0.0-alpha1", "1.0.0-alpha1"),
+            ("1.0.0-alpha1", "1.0.0-beta1"),
+            ("1.0.0-alpha1", "1.0.0-rc1"),
+            ("1.0.0-alpha1", "1.0.0-alpha1+dev1"),
+            ("1.0.0-alpha1.dev1", "1.0.0-alpha1.dev1"),
+            ("1.0.0-alpha1.dev1", "1.0.0-alpha1.dev2"),
+            ("1.0.0-alpha1+dev1", "1.0.0-alpha1+dev2"),
+            ("1.0.0-beta1", "1.0.0-rc1"),
+            ("1.0.0-beta1", "1.0.0-beta1"),
+            ("1.0.0-beta1", "1.0.0-beta1+dev1"),
+            ("1.0.0-beta1.dev1", "1.0.0-beta1.dev1"),
+            ("1.0.0-beta1.dev1", "1.0.0-beta1.dev2"),
+            ("1.0.0-beta1+dev1", "1.0.0-beta1+dev2"),
+            ("1.0.0-rc1", "1.0.0"),
+            ("1.0.0-rc1", "1.0.0-rc1"),
+            ("1.0.0-rc1", "1.0.0-rc1+dev1"),
+            ("1.0.0-rc1.dev1", "1.0.0-rc1.dev1"),
+            ("1.0.0-rc1.dev1", "1.0.0-rc1.dev2"),
+            ("1.0.0-rc1+dev1", "1.0.0-rc1+dev2"),
+        ]
+        for version1, version2 in versions:
+            self.assertFalse(
+                Version.from_string(version1) > Version.from_string(version2),
+                f"{version1} should not be greater then {version2}",
+            )
+
     def test_is_dev_release(self):
         versions = [
             "1.0.0.dev1",
             "1.0.0dev1",
             "1.0.0-alpha1.dev1",
             "1.0.0-beta1.dev1",
             "1.0.0-rc1.dev1",
```

### Comparing `pontos-23.4.2/tests/version/test_commands.py` & `pontos-23.4.3/tests/version/test_commands.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/version/test_errors.py` & `pontos-23.4.3/tests/version/test_errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/version/test_main.py` & `pontos-23.4.3/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/version/test_parser.py` & `pontos-23.4.3/tests/version/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/version/test_project.py` & `pontos-23.4.3/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/tests/version/test_version.py` & `pontos-23.4.3/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.2/PKG-INFO` & `pontos-23.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.4.2
+Version: 23.4.3
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

