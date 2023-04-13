# Comparing `tmp/mrchef-0.2.3.tar.gz` & `tmp/mrchef-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrchef-0.2.3.tar", max compression
+gzip compressed data, was "mrchef-0.4.0.tar", max compression
```

## Comparing `mrchef-0.2.3.tar` & `mrchef-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2022-04-28 11:57:36.516478 mrchef-0.2.3/LICENSE
--rw-r--r--   0        0        0     4738 2022-04-28 11:57:36.516478 mrchef-0.2.3/README.md
--rw-r--r--   0        0        0       55 2022-04-28 11:57:36.516478 mrchef-0.2.3/mrchef/__init__.py
--rw-r--r--   0        0        0      177 2022-04-28 11:57:36.516478 mrchef-0.2.3/mrchef/__main__.py
--rw-r--r--   0        0        0     4857 2022-04-28 11:57:36.516478 mrchef-0.2.3/mrchef/cli.py
--rw-r--r--   0        0        0    25061 2022-04-28 11:57:36.516478 mrchef-0.2.3/mrchef/lib.py
--rw-r--r--   0        0        0     1439 2022-04-28 11:57:36.517478 mrchef-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5781 2022-04-28 12:01:37.545615 mrchef-0.2.3/setup.py
--rw-r--r--   0        0        0     5713 2022-04-28 12:01:37.546260 mrchef-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-13 10:27:17.428131 mrchef-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5000 2023-04-13 10:27:17.428131 mrchef-0.4.0/README.md
+-rw-r--r--   0        0        0       55 2023-04-13 10:27:17.428131 mrchef-0.4.0/mrchef/__init__.py
+-rw-r--r--   0        0        0      177 2023-04-13 10:27:17.428131 mrchef-0.4.0/mrchef/__main__.py
+-rw-r--r--   0        0        0     4857 2023-04-13 10:27:17.428131 mrchef-0.4.0/mrchef/cli.py
+-rw-r--r--   0        0        0    25083 2023-04-13 10:27:17.428131 mrchef-0.4.0/mrchef/lib.py
+-rw-r--r--   0        0        0      964 2023-04-13 10:27:17.429048 mrchef-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6029 1970-01-01 00:00:00.000000 mrchef-0.4.0/setup.py
+-rw-r--r--   0        0        0     5989 1970-01-01 00:00:00.000000 mrchef-0.4.0/PKG-INFO
```

### Comparing `mrchef-0.2.3/LICENSE` & `mrchef-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mrchef-0.2.3/README.md` & `mrchef-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,66 +2,66 @@
 
 👨‍🍳 Meta-Repo Chef. Culinary git helper to work with code buffets.
 
 ## Why
 
 It has features that no other meta-repo manager has:
 
-- Code is 100% reproducible.
-- Full freeze-warmup-freeze coding cycle.
-- Upstream patching supported.
-- Downstream patching supported.
-- Mixed and multi-patching repo supported.
-- Automated updates.
-- Automatic disk space economization with [git-autoshare][].
-- Food! 🥘
+-   Code is 100% reproducible.
+-   Full freeze-warmup-freeze coding cycle.
+-   Upstream patching supported.
+-   Downstream patching supported.
+-   Mixed and multi-patching repo supported.
+-   Automated updates.
+-   Automatic disk space economization with [git-autoshare][].
+-   Food! 🥘
 
 Let's dive in. Imagine you need to create an app that requires many unrelated modules to
 be properly glued together. How would you organize your source code?
 
 There are multiple answers to that question:
 
-- Use separate repos and glue them together through packaging. But what if some code you
-  need isn't properly packaged? What if some dependencies need more than 1 patch to
-  work?
-- Use [a monorepo](https://en.wikipedia.org/wiki/Monorepo). However, what happens if
-  some parts are open source and you need to upstream or review changes?
-- Use [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules). However,
-  that requires that every time you do a `git checkout`... or almost any git command...,
-  you need to use some `--recurse-submodules` flag. Also it gives _a lot_ of headaches
-  when you move files around and perform basically any operation. And what if you need
-  to merge 2 upstream patches?
-- Use [git subtrees](https://www.atlassian.com/git/tutorials/git-subtree). But then, you
-  need even more deep knowledge than with submodules to be able to review or publish
-  patches. And again, how to merge more than one patch?
-- Use [Pijul](https://pijul.org/posts/2022-01-07-monorepos/). But the world isn't ready
-  for it yet. Still we need Git.
+-   Use separate repos and glue them together through packaging. But what if some code
+    you need isn't properly packaged? What if some dependencies need more than 1 patch
+    to work?
+-   Use [a monorepo](https://en.wikipedia.org/wiki/Monorepo). However, what happens if
+    some parts are open source and you need to upstream or review changes?
+-   Use [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules). However,
+    that requires that every time you do a `git checkout`... or almost any git
+    command..., you need to use some `--recurse-submodules` flag. Also it gives _a lot_
+    of headaches when you move files around and perform basically any operation. And
+    what if you need to merge 2 upstream patches?
+-   Use [git subtrees](https://www.atlassian.com/git/tutorials/git-subtree). But then,
+    you need even more deep knowledge than with submodules to be able to review or
+    publish patches. And again, how to merge more than one patch?
+-   Use [Pijul](https://pijul.org/posts/2022-01-07-monorepos/). But the world isn't
+    ready for it yet. Still we need Git.
 
 The solution is to [use a meta-repo](https://notes.burke.libbey.me/metarepo/). There are
 many meta-repo managers out there, but none of them has all the features that I already
 told you about Mr. Chef.
 
 ## Glossary
 
 Mr. Chef introduces a new code management concept based on the metaphor of a buffet. Use
 this glossary to understand the rest of the recipe... readme! Sorry...
 
-- _Buffet_ is the main git repository that contains all the instructions to build it.
-- The _config file_ is a file named `mrchef.toml` that stands in the root of your
-  _buffet_ and configures what Mr. Chef should do.
-- The _kitchen_ is the root folder, inside the _buffet_, where you can find the _meals_.
-  It's configured inside the _config file_.
-- A _meal_ is like a git submodule: another git repo inside your _kitchen_.
-- A _spice_ is a patch that is added to a _meal_.
-- The _freezer_ is where we store the gory details needed to make the kitchen 100%
-  reproducible. Mr. Chef saves it in a file called `.mrchef.freezer.toml`.
-- _Warming up_ means getting meals outside of the _freezer_ and putting them in the
-  _kitchen_, ready to cook!
-- _Freezing_ means writing a new _freezer_ that can reproduce what's currently _warmed
-  up_ in the _kitchen_.
+-   _Buffet_ is the main git repository that contains all the instructions to build it.
+-   The _config file_ is a file named `mrchef.toml` that stands in the root of your
+    _buffet_ and configures what Mr. Chef should do.
+-   The _kitchen_ is the root folder, inside the _buffet_, where you can find the
+    _meals_. It's configured inside the _config file_.
+-   A _meal_ is like a git submodule: another git repo inside your _kitchen_.
+-   A _spice_ is a patch that is added to a _meal_.
+-   The _freezer_ is where we store the gory details needed to make the kitchen 100%
+    reproducible. Mr. Chef saves it in a file called `.mrchef.freezer.toml`.
+-   _Warming up_ means getting meals outside of the _freezer_ and putting them in the
+    _kitchen_, ready to cook!
+-   _Freezing_ means writing a new _freezer_ that can reproduce what's currently _warmed
+    up_ in the _kitchen_.
 
 ## How
 
 ### Using CLI
 
 Install it:
 
@@ -126,21 +126,26 @@
 
 Install it:
 
 ```sh
 nix profile install gitlab:moduon/mrchef
 ```
 
-Go read [that flake](https://gitlab.com/moduon/mrchef/-/blob/main/flake.nix). Ugly?
-Maybe, but awesome! You'll find derivations ready to convert a buffet into aggregated
-source code. Ready to replace git submodules?
-
 Did I say buffets are 100% reproducible? Nothing better than [Nix](https://nixos.org/)
 for that job.
 
+Go read [the flake](./flake.nix). You'll find helpers ready to convert a buffet into
+aggregated source code. Read [the minimal test](./tests/nix/testMinimal.nix) to
+understand how to use them. Ready to replace git submodules?
+
+Keep in mind this if using nix:
+
+-   You should enable flakes. At least, until https://github.com/NixOS/nix/issues/5541
+    or https://github.com/NixOS/nix/issues/5119 are fixed.
+
 ## Who
 
 Created and maintained by [Moduon Team](https://www.moduon.team/).
 
 Original idea by [Jairo Llopis](https://www.recallstack.icu/).
 
 ## Where
```

### Comparing `mrchef-0.2.3/mrchef/cli.py` & `mrchef-0.4.0/mrchef/cli.py`

 * *Files identical despite different names*

### Comparing `mrchef-0.2.3/mrchef/lib.py` & `mrchef-0.4.0/mrchef/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -343,16 +343,15 @@
                 continue
             if hot == cold:
                 logger.info("Matches frozen status, skipping meal: %s", key)
                 continue
             # Clone if meal is not in the kitchen
             if not hot:
                 logger.info("Cloning %s", key)
-                git()(
-                    "autoshare-clone",
+                local["git-autoshare-clone"](
                     "--recursive",
                     "--filter",
                     "blob:none",
                     "--branch",
                     cold.branch,
                     cold.url,
                     cold.path,
@@ -645,18 +644,20 @@
 
     Args:
         folder: Path to git repo.
         remote_url: Absolute URL to remote.
         remote_ref: Branch or revision to fetch from remote.
     """
     _git = git(folder)
-    _git("remote", "add", "_mrchef", remote_url)
-    _git("fetch", "--write-fetch-head", "_mrchef", remote_ref)
-    result = _git("rev-parse", "FETCH_HEAD").strip()
-    _git("remote", "rm", "_mrchef")
+    try:
+        _git("remote", "add", "_mrchef", remote_url)
+        _git("fetch", "--write-fetch-head", "_mrchef", remote_ref)
+        result = _git("rev-parse", "FETCH_HEAD").strip()
+    finally:
+        _git("remote", "rm", "_mrchef")
     return result
 
 
 def git_rev(folder: Path) -> str:
     """Know the commit where a git repository is currently checked out."""
     return git(folder)("rev-parse", "--verify", "HEAD").strip()
```

### Comparing `mrchef-0.2.3/pyproject.toml` & `mrchef-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mrchef"
-version = "0.2.3"
+version = "0.4.0"
 description = "Metarepo Chef"
 authors = ["Moduon <info@moduon.team>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://gitlab.com/moduon/mrchef"
 
 [tool.poetry.scripts]
@@ -18,43 +18,25 @@
 git-autoshare = ">=1.0.0-beta.6"
 mergedeep = ">=1.3.4"
 plumbum = ">=1.7.2"
 requests = ">=2.27.1"
 tomlkit = ">=0.10.0"
 xdg = ">=5.1.1"
 
-# Indirect dependencies
-platformdirs = "<2.5.2" # HACK https://github.com/nix-community/poetry2nix/pull/600
-
-[tool.poetry.dev-dependencies]
-autoflake = ">=1.4"
-black = ">=22.1.0"
-blacken-docs = ">=1.12.1"
-commitizen = ">=2.21.2"
-flake8 = ">=4.0.1"
-flake8-bugbear = ">=22.1.11"
-isort = ">=5.10.1"
-pre-commit = "^2.17.0"
-pydocstyle = {extras = ["toml"], version = ">=6.1.1"}
-pytest = ">=7.0.1"
-pytest-xdist = "^2.5.0"
-pyupgrade = ">=2.31.0"
-
-[tool.commitizen]
-annotated_tag = true
-changelog_incremental = true
-tag_format = "v$version"
-update_changelog_on_bump = true
-version = "0.2.3"
-version_files = ["mrchef/__init__.py", "pyproject.toml"]
+[tool.poetry.group.dev.dependencies]
+pytest = ">=7.2.1"
+pytest-xdist = ">=3.2.1"
 
 [tool.pydocstyle]
 convention = "google"
 ignore_decorators = "handle_error"
 
 [tool.pytest.ini_options]
 addopts = "-n auto -ra"
 testpaths = ["tests"]
+markers = [
+    "impure: tests that depend on network access or external sources"
+]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mrchef-0.2.3/setup.py` & `mrchef-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,32 +8,31 @@
 {'': ['*']}
 
 install_requires = \
 ['coloredlogs>=15.0.1',
  'decorator>=5.1.1',
  'git-autoshare>=1.0.0-beta.6',
  'mergedeep>=1.3.4',
- 'platformdirs<2.5.2',
  'plumbum>=1.7.2',
  'requests>=2.27.1',
  'tomlkit>=0.10.0',
  'xdg>=5.1.1']
 
 entry_points = \
 {'console_scripts': ['mrchef = mrchef.__main__:run']}
 
 setup_kwargs = {
     'name': 'mrchef',
-    'version': '0.2.3',
+    'version': '0.4.0',
     'description': 'Metarepo Chef',
-    'long_description': "# Mr. Chef\n\n👨\u200d🍳 Meta-Repo Chef. Culinary git helper to work with code buffets.\n\n## Why\n\nIt has features that no other meta-repo manager has:\n\n- Code is 100% reproducible.\n- Full freeze-warmup-freeze coding cycle.\n- Upstream patching supported.\n- Downstream patching supported.\n- Mixed and multi-patching repo supported.\n- Automated updates.\n- Automatic disk space economization with [git-autoshare][].\n- Food! 🥘\n\nLet's dive in. Imagine you need to create an app that requires many unrelated modules to\nbe properly glued together. How would you organize your source code?\n\nThere are multiple answers to that question:\n\n- Use separate repos and glue them together through packaging. But what if some code you\n  need isn't properly packaged? What if some dependencies need more than 1 patch to\n  work?\n- Use [a monorepo](https://en.wikipedia.org/wiki/Monorepo). However, what happens if\n  some parts are open source and you need to upstream or review changes?\n- Use [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules). However,\n  that requires that every time you do a `git checkout`... or almost any git command...,\n  you need to use some `--recurse-submodules` flag. Also it gives _a lot_ of headaches\n  when you move files around and perform basically any operation. And what if you need\n  to merge 2 upstream patches?\n- Use [git subtrees](https://www.atlassian.com/git/tutorials/git-subtree). But then, you\n  need even more deep knowledge than with submodules to be able to review or publish\n  patches. And again, how to merge more than one patch?\n- Use [Pijul](https://pijul.org/posts/2022-01-07-monorepos/). But the world isn't ready\n  for it yet. Still we need Git.\n\nThe solution is to [use a meta-repo](https://notes.burke.libbey.me/metarepo/). There are\nmany meta-repo managers out there, but none of them has all the features that I already\ntold you about Mr. Chef.\n\n## Glossary\n\nMr. Chef introduces a new code management concept based on the metaphor of a buffet. Use\nthis glossary to understand the rest of the recipe... readme! Sorry...\n\n- _Buffet_ is the main git repository that contains all the instructions to build it.\n- The _config file_ is a file named `mrchef.toml` that stands in the root of your\n  _buffet_ and configures what Mr. Chef should do.\n- The _kitchen_ is the root folder, inside the _buffet_, where you can find the _meals_.\n  It's configured inside the _config file_.\n- A _meal_ is like a git submodule: another git repo inside your _kitchen_.\n- A _spice_ is a patch that is added to a _meal_.\n- The _freezer_ is where we store the gory details needed to make the kitchen 100%\n  reproducible. Mr. Chef saves it in a file called `.mrchef.freezer.toml`.\n- _Warming up_ means getting meals outside of the _freezer_ and putting them in the\n  _kitchen_, ready to cook!\n- _Freezing_ means writing a new _freezer_ that can reproduce what's currently _warmed\n  up_ in the _kitchen_.\n\n## How\n\n### Using CLI\n\nInstall it:\n\n```sh\npipx install mrchef\n```\n\nUsually you start by creating a new configuration file:\n\n```sh\nmrchef init\n```\n\nIt will create a new `mrchef.toml` file with some comments about how to use it. You can\ndelete them once you know how to do it.\n\nNow, you will need to add a meal:\n\n```sh\nmrchef meal-add kitchen/hello https://github.com/octocat/Hello-World master\n```\n\n💡 Mr. Chef uses [git-autoshare][] automatically. It will help you if you need to clone\nhuge repos! But you have to configure it before adding the meals.\n\nYou can add more meals just like that.\n\nMaybe you need to apply a couple of spices to the meal? OK:\n\n```sh\nmrchef spice-add kitchen/hello https://github.com/octocat/Hello-World/pull/2256\nmrchef spice-add kitchen/hello https://github.com/octocat/Hello-World/pull/34\n```\n\nDid `master` get new commits? Or did those PRs get updated? Update everything:\n\n```sh\nmrchef update\n```\n\nCool, huh? 😏 Mr. Chef can do more things! To see all commands and what they do:\n\n```sh\nmrchef --help-all\n```\n\n### Using Python\n\nInstall it:\n\n```sh\npip install mrchef\n```\n\nUse it:\n\n```python\nimport mrchef\n```\n\n### Using Nix\n\nInstall it:\n\n```sh\nnix profile install gitlab:moduon/mrchef\n```\n\nGo read [that flake](https://gitlab.com/moduon/mrchef/-/blob/main/flake.nix). Ugly?\nMaybe, but awesome! You'll find derivations ready to convert a buffet into aggregated\nsource code. Ready to replace git submodules?\n\nDid I say buffets are 100% reproducible? Nothing better than [Nix](https://nixos.org/)\nfor that job.\n\n## Who\n\nCreated and maintained by [Moduon Team](https://www.moduon.team/).\n\nOriginal idea by [Jairo Llopis](https://www.recallstack.icu/).\n\n## Where\n\nAnywhere you want! 🎁 It's [GPL 3.0+](./LICENSE).\n\n[git-autoshare]: https://github.com/acsone/git-autoshare\n",
+    'long_description': "# Mr. Chef\n\n👨\u200d🍳 Meta-Repo Chef. Culinary git helper to work with code buffets.\n\n## Why\n\nIt has features that no other meta-repo manager has:\n\n-   Code is 100% reproducible.\n-   Full freeze-warmup-freeze coding cycle.\n-   Upstream patching supported.\n-   Downstream patching supported.\n-   Mixed and multi-patching repo supported.\n-   Automated updates.\n-   Automatic disk space economization with [git-autoshare][].\n-   Food! 🥘\n\nLet's dive in. Imagine you need to create an app that requires many unrelated modules to\nbe properly glued together. How would you organize your source code?\n\nThere are multiple answers to that question:\n\n-   Use separate repos and glue them together through packaging. But what if some code\n    you need isn't properly packaged? What if some dependencies need more than 1 patch\n    to work?\n-   Use [a monorepo](https://en.wikipedia.org/wiki/Monorepo). However, what happens if\n    some parts are open source and you need to upstream or review changes?\n-   Use [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules). However,\n    that requires that every time you do a `git checkout`... or almost any git\n    command..., you need to use some `--recurse-submodules` flag. Also it gives _a lot_\n    of headaches when you move files around and perform basically any operation. And\n    what if you need to merge 2 upstream patches?\n-   Use [git subtrees](https://www.atlassian.com/git/tutorials/git-subtree). But then,\n    you need even more deep knowledge than with submodules to be able to review or\n    publish patches. And again, how to merge more than one patch?\n-   Use [Pijul](https://pijul.org/posts/2022-01-07-monorepos/). But the world isn't\n    ready for it yet. Still we need Git.\n\nThe solution is to [use a meta-repo](https://notes.burke.libbey.me/metarepo/). There are\nmany meta-repo managers out there, but none of them has all the features that I already\ntold you about Mr. Chef.\n\n## Glossary\n\nMr. Chef introduces a new code management concept based on the metaphor of a buffet. Use\nthis glossary to understand the rest of the recipe... readme! Sorry...\n\n-   _Buffet_ is the main git repository that contains all the instructions to build it.\n-   The _config file_ is a file named `mrchef.toml` that stands in the root of your\n    _buffet_ and configures what Mr. Chef should do.\n-   The _kitchen_ is the root folder, inside the _buffet_, where you can find the\n    _meals_. It's configured inside the _config file_.\n-   A _meal_ is like a git submodule: another git repo inside your _kitchen_.\n-   A _spice_ is a patch that is added to a _meal_.\n-   The _freezer_ is where we store the gory details needed to make the kitchen 100%\n    reproducible. Mr. Chef saves it in a file called `.mrchef.freezer.toml`.\n-   _Warming up_ means getting meals outside of the _freezer_ and putting them in the\n    _kitchen_, ready to cook!\n-   _Freezing_ means writing a new _freezer_ that can reproduce what's currently _warmed\n    up_ in the _kitchen_.\n\n## How\n\n### Using CLI\n\nInstall it:\n\n```sh\npipx install mrchef\n```\n\nUsually you start by creating a new configuration file:\n\n```sh\nmrchef init\n```\n\nIt will create a new `mrchef.toml` file with some comments about how to use it. You can\ndelete them once you know how to do it.\n\nNow, you will need to add a meal:\n\n```sh\nmrchef meal-add kitchen/hello https://github.com/octocat/Hello-World master\n```\n\n💡 Mr. Chef uses [git-autoshare][] automatically. It will help you if you need to clone\nhuge repos! But you have to configure it before adding the meals.\n\nYou can add more meals just like that.\n\nMaybe you need to apply a couple of spices to the meal? OK:\n\n```sh\nmrchef spice-add kitchen/hello https://github.com/octocat/Hello-World/pull/2256\nmrchef spice-add kitchen/hello https://github.com/octocat/Hello-World/pull/34\n```\n\nDid `master` get new commits? Or did those PRs get updated? Update everything:\n\n```sh\nmrchef update\n```\n\nCool, huh? 😏 Mr. Chef can do more things! To see all commands and what they do:\n\n```sh\nmrchef --help-all\n```\n\n### Using Python\n\nInstall it:\n\n```sh\npip install mrchef\n```\n\nUse it:\n\n```python\nimport mrchef\n```\n\n### Using Nix\n\nInstall it:\n\n```sh\nnix profile install gitlab:moduon/mrchef\n```\n\nDid I say buffets are 100% reproducible? Nothing better than [Nix](https://nixos.org/)\nfor that job.\n\nGo read [the flake](./flake.nix). You'll find helpers ready to convert a buffet into\naggregated source code. Read [the minimal test](./tests/nix/testMinimal.nix) to\nunderstand how to use them. Ready to replace git submodules?\n\nKeep in mind this if using nix:\n\n-   You should enable flakes. At least, until https://github.com/NixOS/nix/issues/5541\n    or https://github.com/NixOS/nix/issues/5119 are fixed.\n\n## Who\n\nCreated and maintained by [Moduon Team](https://www.moduon.team/).\n\nOriginal idea by [Jairo Llopis](https://www.recallstack.icu/).\n\n## Where\n\nAnywhere you want! 🎁 It's [GPL 3.0+](./LICENSE).\n\n[git-autoshare]: https://github.com/acsone/git-autoshare\n",
     'author': 'Moduon',
     'author_email': 'info@moduon.team',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://gitlab.com/moduon/mrchef',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `mrchef-0.2.3/PKG-INFO` & `mrchef-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mrchef
-Version: 0.2.3
+Version: 0.4.0
 Summary: Metarepo Chef
 Home-page: https://gitlab.com/moduon/mrchef
 License: GPL-3.0-or-later
 Author: Moduon
 Author-email: info@moduon.team
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: coloredlogs (>=15.0.1)
 Requires-Dist: decorator (>=5.1.1)
 Requires-Dist: git-autoshare (>=1.0.0-beta.6)
 Requires-Dist: mergedeep (>=1.3.4)
-Requires-Dist: platformdirs (<2.5.2)
 Requires-Dist: plumbum (>=1.7.2)
 Requires-Dist: requests (>=2.27.1)
 Requires-Dist: tomlkit (>=0.10.0)
 Requires-Dist: xdg (>=5.1.1)
 Project-URL: Repository, https://gitlab.com/moduon/mrchef
 Description-Content-Type: text/markdown
 
@@ -29,66 +29,66 @@
 
 👨‍🍳 Meta-Repo Chef. Culinary git helper to work with code buffets.
 
 ## Why
 
 It has features that no other meta-repo manager has:
 
-- Code is 100% reproducible.
-- Full freeze-warmup-freeze coding cycle.
-- Upstream patching supported.
-- Downstream patching supported.
-- Mixed and multi-patching repo supported.
-- Automated updates.
-- Automatic disk space economization with [git-autoshare][].
-- Food! 🥘
+-   Code is 100% reproducible.
+-   Full freeze-warmup-freeze coding cycle.
+-   Upstream patching supported.
+-   Downstream patching supported.
+-   Mixed and multi-patching repo supported.
+-   Automated updates.
+-   Automatic disk space economization with [git-autoshare][].
+-   Food! 🥘
 
 Let's dive in. Imagine you need to create an app that requires many unrelated modules to
 be properly glued together. How would you organize your source code?
 
 There are multiple answers to that question:
 
-- Use separate repos and glue them together through packaging. But what if some code you
-  need isn't properly packaged? What if some dependencies need more than 1 patch to
-  work?
-- Use [a monorepo](https://en.wikipedia.org/wiki/Monorepo). However, what happens if
-  some parts are open source and you need to upstream or review changes?
-- Use [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules). However,
-  that requires that every time you do a `git checkout`... or almost any git command...,
-  you need to use some `--recurse-submodules` flag. Also it gives _a lot_ of headaches
-  when you move files around and perform basically any operation. And what if you need
-  to merge 2 upstream patches?
-- Use [git subtrees](https://www.atlassian.com/git/tutorials/git-subtree). But then, you
-  need even more deep knowledge than with submodules to be able to review or publish
-  patches. And again, how to merge more than one patch?
-- Use [Pijul](https://pijul.org/posts/2022-01-07-monorepos/). But the world isn't ready
-  for it yet. Still we need Git.
+-   Use separate repos and glue them together through packaging. But what if some code
+    you need isn't properly packaged? What if some dependencies need more than 1 patch
+    to work?
+-   Use [a monorepo](https://en.wikipedia.org/wiki/Monorepo). However, what happens if
+    some parts are open source and you need to upstream or review changes?
+-   Use [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules). However,
+    that requires that every time you do a `git checkout`... or almost any git
+    command..., you need to use some `--recurse-submodules` flag. Also it gives _a lot_
+    of headaches when you move files around and perform basically any operation. And
+    what if you need to merge 2 upstream patches?
+-   Use [git subtrees](https://www.atlassian.com/git/tutorials/git-subtree). But then,
+    you need even more deep knowledge than with submodules to be able to review or
+    publish patches. And again, how to merge more than one patch?
+-   Use [Pijul](https://pijul.org/posts/2022-01-07-monorepos/). But the world isn't
+    ready for it yet. Still we need Git.
 
 The solution is to [use a meta-repo](https://notes.burke.libbey.me/metarepo/). There are
 many meta-repo managers out there, but none of them has all the features that I already
 told you about Mr. Chef.
 
 ## Glossary
 
 Mr. Chef introduces a new code management concept based on the metaphor of a buffet. Use
 this glossary to understand the rest of the recipe... readme! Sorry...
 
-- _Buffet_ is the main git repository that contains all the instructions to build it.
-- The _config file_ is a file named `mrchef.toml` that stands in the root of your
-  _buffet_ and configures what Mr. Chef should do.
-- The _kitchen_ is the root folder, inside the _buffet_, where you can find the _meals_.
-  It's configured inside the _config file_.
-- A _meal_ is like a git submodule: another git repo inside your _kitchen_.
-- A _spice_ is a patch that is added to a _meal_.
-- The _freezer_ is where we store the gory details needed to make the kitchen 100%
-  reproducible. Mr. Chef saves it in a file called `.mrchef.freezer.toml`.
-- _Warming up_ means getting meals outside of the _freezer_ and putting them in the
-  _kitchen_, ready to cook!
-- _Freezing_ means writing a new _freezer_ that can reproduce what's currently _warmed
-  up_ in the _kitchen_.
+-   _Buffet_ is the main git repository that contains all the instructions to build it.
+-   The _config file_ is a file named `mrchef.toml` that stands in the root of your
+    _buffet_ and configures what Mr. Chef should do.
+-   The _kitchen_ is the root folder, inside the _buffet_, where you can find the
+    _meals_. It's configured inside the _config file_.
+-   A _meal_ is like a git submodule: another git repo inside your _kitchen_.
+-   A _spice_ is a patch that is added to a _meal_.
+-   The _freezer_ is where we store the gory details needed to make the kitchen 100%
+    reproducible. Mr. Chef saves it in a file called `.mrchef.freezer.toml`.
+-   _Warming up_ means getting meals outside of the _freezer_ and putting them in the
+    _kitchen_, ready to cook!
+-   _Freezing_ means writing a new _freezer_ that can reproduce what's currently _warmed
+    up_ in the _kitchen_.
 
 ## How
 
 ### Using CLI
 
 Install it:
 
@@ -153,21 +153,26 @@
 
 Install it:
 
 ```sh
 nix profile install gitlab:moduon/mrchef
 ```
 
-Go read [that flake](https://gitlab.com/moduon/mrchef/-/blob/main/flake.nix). Ugly?
-Maybe, but awesome! You'll find derivations ready to convert a buffet into aggregated
-source code. Ready to replace git submodules?
-
 Did I say buffets are 100% reproducible? Nothing better than [Nix](https://nixos.org/)
 for that job.
 
+Go read [the flake](./flake.nix). You'll find helpers ready to convert a buffet into
+aggregated source code. Read [the minimal test](./tests/nix/testMinimal.nix) to
+understand how to use them. Ready to replace git submodules?
+
+Keep in mind this if using nix:
+
+-   You should enable flakes. At least, until https://github.com/NixOS/nix/issues/5541
+    or https://github.com/NixOS/nix/issues/5119 are fixed.
+
 ## Who
 
 Created and maintained by [Moduon Team](https://www.moduon.team/).
 
 Original idea by [Jairo Llopis](https://www.recallstack.icu/).
 
 ## Where
```

