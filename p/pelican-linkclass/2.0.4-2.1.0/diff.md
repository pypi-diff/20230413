# Comparing `tmp/pelican-linkclass-2.0.4.tar.gz` & `tmp/pelican_linkclass-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican-linkclass-2.0.4.tar", max compression
+gzip compressed data, was "pelican_linkclass-2.1.0.tar", max compression
```

## Comparing `pelican-linkclass-2.0.4.tar` & `pelican_linkclass-2.1.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    34523 2022-10-01 20:32:46.491329 pelican-linkclass-2.0.4/LICENSE
--rw-r--r--   0        0        0     3850 2022-10-01 20:32:46.491329 pelican-linkclass-2.0.4/README.md
--rw-r--r--   0        0        0       33 2022-10-01 20:32:46.491329 pelican-linkclass-2.0.4/pelican/plugins/linkclass/__init__.py
--rw-r--r--   0        0        0     1811 2022-10-01 20:32:46.491329 pelican-linkclass-2.0.4/pelican/plugins/linkclass/linkclass.py
--rw-r--r--   0        0        0     3896 2022-10-01 20:32:46.491329 pelican-linkclass-2.0.4/pelican/plugins/linkclass/mdx_linkclass.py
--rw-r--r--   0        0        0     6898 2022-10-01 20:32:46.491329 pelican-linkclass-2.0.4/pelican/plugins/linkclass/test_linkclass.py
--rw-r--r--   0        0        0     1977 2022-10-01 20:32:58.615275 pelican-linkclass-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 pelican-linkclass-2.0.4/setup.py
--rw-r--r--   0        0        0     5343 1970-01-01 00:00:00.000000 pelican-linkclass-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-13 12:41:10.743584 pelican_linkclass-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3871 2023-04-13 12:41:10.747584 pelican_linkclass-2.1.0/README.md
+-rw-r--r--   0        0        0       33 2023-04-13 12:41:10.747584 pelican_linkclass-2.1.0/pelican/plugins/linkclass/__init__.py
+-rw-r--r--   0        0        0     1757 2023-04-13 12:41:10.747584 pelican_linkclass-2.1.0/pelican/plugins/linkclass/linkclass.py
+-rw-r--r--   0        0        0     3896 2023-04-13 12:41:10.747584 pelican_linkclass-2.1.0/pelican/plugins/linkclass/mdx_linkclass.py
+-rw-r--r--   0        0        0     6889 2023-04-13 12:41:10.747584 pelican_linkclass-2.1.0/pelican/plugins/linkclass/test_linkclass.py
+-rw-r--r--   0        0        0     1964 2023-04-13 12:41:29.911784 pelican_linkclass-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5316 1970-01-01 00:00:00.000000 pelican_linkclass-2.1.0/PKG-INFO
```

### Comparing `pelican-linkclass-2.0.4/LICENSE` & `pelican_linkclass-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican-linkclass-2.0.4/README.md` & `pelican_linkclass-2.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Link Class: A Plugin for Pelican
 ================================
 
-[![Build Status](https://img.shields.io/github/workflow/status/pelican-plugins/linkclass/build)](https://github.com/pelican-plugins/linkclass/actions)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pelican-plugins/linkclass/main.yml?branch=main)](https://github.com/pelican-plugins/linkclass/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/pelican-linkclass)](https://pypi.org/project/pelican-linkclass/)
 ![License](https://img.shields.io/pypi/l/pelican-linkclass?color=blue)
 
 This Pelican plugin allows you to set the class attribute of `<a>` elements
 (generated in Markdown by `[ext](link)`) according to whether the link is
 external (i.e., starts with `http://` or `https://`) or internal to the
 Pelican-generated site.
@@ -28,16 +28,16 @@
 
 In order to avoid clashes with already-defined classes in the user CSS
 style sheets, it is possible to specify the name of the classes that will
 be used. They can be specified in the Pelican setting file with the
 `LINKCLASS` variable, which must be defined as a list of tuples, like this:
 
 ```python
-'LINKCLASS' = (('EXTERNAL_CLASS', 'name-of-the-class-for-external-links')
-                'INTERNAL_CLASS', 'name-of-the-class-for-internal-links'))
+'LINKCLASS' = (('EXTERNAL_CLASS', 'name-of-the-class-for-external-links'),
+               ('INTERNAL_CLASS', 'name-of-the-class-for-internal-links'))
 ```
 
 The default values for `EXTERNAL_CLASS` and `INTERNAL_CLASS` are,
 respectively, `'external'` and `'internal'`.
 
 Styling Hyperlinks
 ------------------
@@ -99,10 +99,10 @@
 [Lucas Cimon]: https://github.com/Lucas-C
 [pytest]: https://pytest.org/
 [Justin Mayer]: https://github.com/justinmayer
 
 Author
 ------
 
-Copyright (C) 2015, 2017, 2019, 2021, 2022  Rafael Laboissière (<rafael@laboissiere.net>)
+Copyright © 2015, 2017, 2019, 2021-2023 Rafael Laboissière (<rafael@laboissiere.net>)
 
 Released under the GNU Affero Public License, version 3 or later. No warranties.
```

### Comparing `pelican-linkclass-2.0.4/pelican/plugins/linkclass/linkclass.py` & `pelican_linkclass-2.1.0/pelican/plugins/linkclass/linkclass.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Link Class Plugin for Pelican"""
 
-# Copyright (C) 2015, 2019  Rafael Laboissière
+# Copyright (C) 2015, 2019, 2023  Rafael Laboissière
 #
 # This program is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Affero Public License as published by
 # the Free Software Foundation, either version 3 of the License, or (at
 # your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but
@@ -14,39 +14,37 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see http://www.gnu.org/licenses/.
 
 
 from pelican import signals
 
-from .mdx_linkclass import LC_CONFIG, LC_HELP, LinkClassExtension
+from .mdx_linkclass import LC_CONFIG, LinkClassExtension
 
 
 def addLinkClass(gen):
-
     if not gen.settings.get("MARKDOWN"):
         from pelican.settings import DEFAULT_CONFIG
 
         gen.settings["MARKDOWN"] = DEFAULT_CONFIG["MARKDOWN"]
 
     if gen.settings.get("LINKCLASS"):
-        for param, default, helptext in gen.settings.get("LINKCLASS"):
+        for param, default in gen.settings.get("LINKCLASS"):
             LC_CONFIG[param] = default
-            LC_HELP[param] = helptext
 
     if LinkClassExtension not in gen.settings["MARKDOWN"]:
         config = dict()
         for key, value in LC_CONFIG.items():
             config[key] = value
         for key, value in gen.settings.items():
             if key in LC_CONFIG:
                 config[key] = value
         lcobj = LinkClassExtension(config)
         try:
             gen.settings["MARKDOWN"]["extensions"].append(lcobj)
-        except (KeyError):
+        except KeyError:
             gen.settings["MARKDOWN"]["extensions"] = [lcobj]
 
 
 def register():
     """Register the Link Class plugin with Pelican"""
     signals.initialized.connect(addLinkClass)
```

### Comparing `pelican-linkclass-2.0.4/pelican/plugins/linkclass/mdx_linkclass.py` & `pelican_linkclass-2.1.0/pelican/plugins/linkclass/mdx_linkclass.py`

 * *Files identical despite different names*

### Comparing `pelican-linkclass-2.0.4/pelican/plugins/linkclass/test_linkclass.py` & `pelican_linkclass-2.1.0/pelican/plugins/linkclass/test_linkclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Unit testing suite for the Link Class Plugin"""
 
-# Copyright (C) 2015, 2017, 2019, 2021, 2022  Rafael Laboissière <rafael@laboissiere.net>  # noqa: E501
+# Copyright (C) 2015, 2017, 2019, 2021-2023  Rafael Laboissière <rafael@laboissiere.net>  # noqa: E501
 #
 # This program is free software: you can redistribute it and/or modify it
 # under the terms of the GNU General Affero Public License as published by
 # the Free Software Foundation, either version 3 of the License, or (at
 # your option) any later version.
 #
 # This program is distributed in the hope that it will be useful, but
@@ -71,16 +71,16 @@
             "PATH": self.content_path,
             "OUTPUT_PATH": self.output_path,
             "PLUGINS": [linkclass],
             "CACHE_CONTENT": False,
             "SITEURL": "http://example.org",
             "TIMEZONE": "UTC",
             "LINKCLASS": (
-                ("INTERNAL_CLASS", INTERNAL_CLASS, ""),
-                ("EXTERNAL_CLASS", EXTERNAL_CLASS, ""),
+                ("INTERNAL_CLASS", INTERNAL_CLASS),
+                ("EXTERNAL_CLASS", EXTERNAL_CLASS),
             ),
         }
         if override:
             settings.update(override)
 
         # Generate the test Markdown source file
         fid = open(
```

### Comparing `pelican-linkclass-2.0.4/pyproject.toml` & `pelican_linkclass-2.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pelican-linkclass"
-version = "2.0.4"
+version = "2.1.0"
 description = "Pelican plugin to set anchor tag's class attribute to differentiate between internal and external links"
 authors = ["Rafael Laboissière <rafael@laboissiere.net>"]
 license = "AGPL-3.0"
 readme = "README.md"
 keywords = ["pelican", "plugin", "markdown"]
 repository = "https://github.com/pelican-plugins/linkclass"
 documentation = "https://docs.getpelican.com"
@@ -24,24 +24,24 @@
 ]
 
 [tool.poetry.urls]
 "Funding" = "https://donate.getpelican.com/"
 "Issue Tracker" = "https://github.com/pelican-plugins/linkclass/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.6.2,<4.0"
+python = ">=3.8.1,<4.0"
 pelican = ">=4.5"
 markdown = {version = ">=3.2", optional = true}
 
 [tool.poetry.dev-dependencies]
-black = {version = "^22.1.0"}
+black = "^23"
 flake8 = "^3.8"
 flake8-black = "^0.2"
-invoke = "^1.3"
-isort = "^5.4"
+invoke = "^2.0"
+isort = "^5.12.0"
 livereload = "^2.6"
 markdown = "^3.2"
 pytest = "^6.0"
 pytest-cov = "^3.0"
 pytest-pythonpath = "^0.7.3"
 pytest-sugar = "^0.9.4"
 Werkzeug = "^1.0"
```

### Comparing `pelican-linkclass-2.0.4/setup.py` & `pelican_linkclass-2.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,141 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pelican-linkclass
+Version: 2.1.0
+Summary: Pelican plugin to set anchor tag's class attribute to differentiate between internal and external links
+Home-page: https://github.com/pelican-plugins/linkclass
+License: AGPL-3.0
+Keywords: pelican,plugin,markdown
+Author: Rafael Laboissière
+Author-email: rafael@laboissiere.net
+Requires-Python: >=3.8.1,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Framework :: Pelican
+Classifier: Framework :: Pelican :: Plugins
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: markdown
+Requires-Dist: markdown (>=3.2) ; extra == "markdown"
+Requires-Dist: pelican (>=4.5)
+Project-URL: Documentation, https://docs.getpelican.com
+Project-URL: Funding, https://donate.getpelican.com/
+Project-URL: Issue Tracker, https://github.com/pelican-plugins/linkclass/issues
+Project-URL: Repository, https://github.com/pelican-plugins/linkclass
+Description-Content-Type: text/markdown
+
+Link Class: A Plugin for Pelican
+================================
+
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pelican-plugins/linkclass/main.yml?branch=main)](https://github.com/pelican-plugins/linkclass/actions)
+[![PyPI Version](https://img.shields.io/pypi/v/pelican-linkclass)](https://pypi.org/project/pelican-linkclass/)
+![License](https://img.shields.io/pypi/l/pelican-linkclass?color=blue)
+
+This Pelican plugin allows you to set the class attribute of `<a>` elements
+(generated in Markdown by `[ext](link)`) according to whether the link is
+external (i.e., starts with `http://` or `https://`) or internal to the
+Pelican-generated site.
+
+For now, this plugin only works with Markdown. It has been tested with version
+3.0+ of the Python-Markdown module and may not work with previous versions.
+
+Installation
+------------
+
+This plugin [is available as a package](https://pypi.org/project/pelican-linkclass/)
+at PyPI and can be installed via:
+
+```
+python -m pip install pelican-linkclass
+```
+
+Configuration
+-------------
+
+In order to avoid clashes with already-defined classes in the user CSS
+style sheets, it is possible to specify the name of the classes that will
+be used. They can be specified in the Pelican setting file with the
+`LINKCLASS` variable, which must be defined as a list of tuples, like this:
+
+```python
+'LINKCLASS' = (('EXTERNAL_CLASS', 'name-of-the-class-for-external-links'),
+               ('INTERNAL_CLASS', 'name-of-the-class-for-internal-links'))
+```
+
+The default values for `EXTERNAL_CLASS` and `INTERNAL_CLASS` are,
+respectively, `'external'` and `'internal'`.
+
+Styling Hyperlinks
+------------------
+
+One of the possible uses of this plugins is for styling. Suppose that we
+have the following Markdown content in your article:
+
+```markdown
+This is an [internal](internal) link and this is an
+[external](http://external.com) link.
+```
+
+If the default configuration variable values are used, then one possible
+CSS setting could be:
+
+```css
+a.external:before {
+    content: url('../images/external-link.png');
+    margin-right: 0.2em;
+}
+```
 
-packages = \
-['pelican', 'pelican.plugins.linkclass']
+(The file `external-link.png` is also distributed with this plugin. To use it,
+copy it to the appropriate place in your web site source tree, for instance
+in `theme/static/images/`.)
 
-package_data = \
-{'': ['*']}
+Then, the result will look like the following:
 
-install_requires = \
-['pelican>=4.5']
-
-extras_require = \
-{'markdown': ['markdown>=3.2']}
-
-setup_kwargs = {
-    'name': 'pelican-linkclass',
-    'version': '2.0.4',
-    'description': "Pelican plugin to set anchor tag's class attribute to differentiate between internal and external links",
-    'long_description': "Link Class: A Plugin for Pelican\n================================\n\n[![Build Status](https://img.shields.io/github/workflow/status/pelican-plugins/linkclass/build)](https://github.com/pelican-plugins/linkclass/actions)\n[![PyPI Version](https://img.shields.io/pypi/v/pelican-linkclass)](https://pypi.org/project/pelican-linkclass/)\n![License](https://img.shields.io/pypi/l/pelican-linkclass?color=blue)\n\nThis Pelican plugin allows you to set the class attribute of `<a>` elements\n(generated in Markdown by `[ext](link)`) according to whether the link is\nexternal (i.e., starts with `http://` or `https://`) or internal to the\nPelican-generated site.\n\nFor now, this plugin only works with Markdown. It has been tested with version\n3.0+ of the Python-Markdown module and may not work with previous versions.\n\nInstallation\n------------\n\nThis plugin [is available as a package](https://pypi.org/project/pelican-linkclass/)\nat PyPI and can be installed via:\n\n```\npython -m pip install pelican-linkclass\n```\n\nConfiguration\n-------------\n\nIn order to avoid clashes with already-defined classes in the user CSS\nstyle sheets, it is possible to specify the name of the classes that will\nbe used. They can be specified in the Pelican setting file with the\n`LINKCLASS` variable, which must be defined as a list of tuples, like this:\n\n```python\n'LINKCLASS' = (('EXTERNAL_CLASS', 'name-of-the-class-for-external-links')\n                'INTERNAL_CLASS', 'name-of-the-class-for-internal-links'))\n```\n\nThe default values for `EXTERNAL_CLASS` and `INTERNAL_CLASS` are,\nrespectively, `'external'` and `'internal'`.\n\nStyling Hyperlinks\n------------------\n\nOne of the possible uses of this plugins is for styling. Suppose that we\nhave the following Markdown content in your article:\n\n```markdown\nThis is an [internal](internal) link and this is an\n[external](http://external.com) link.\n```\n\nIf the default configuration variable values are used, then one possible\nCSS setting could be:\n\n```css\na.external:before {\n    content: url('../images/external-link.png');\n    margin-right: 0.2em;\n}\n```\n\n(The file `external-link.png` is also distributed with this plugin. To use it,\ncopy it to the appropriate place in your web site source tree, for instance\nin `theme/static/images/`.)\n\nThen, the result will look like the following:\n\n![figure](https://github.com/pelican-plugins/linkclass/raw/main/linkclass-example.png)\n\nNote that this plugin also works with reference-style links, as in the\nfollowing example:\n\n```markdown\nThis is an [internal][internal] link and this is an\n[external][external] link.\n\n [internal]: internal\n [external]: http://external.com\n```\n\nContributing\n------------\n\nContributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].\n\nTo start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.\n\n[existing issues]: https://github.com/pelican-plugins/linkclass/issues\n[Contributing to Pelican]: https://docs.getpelican.com/en/latest/contribute.html\n\nAcknowledgments\n---------------\n\nMany thanks to [Yuliya Bagriy][] for setting up the package for [PyPI][], to [Lucas Cimon][] for fixing the issues with [pytest][], and to [Justin Mayer][] for helping with migration of this plugin under the Pelican Plugins organization.\n\n[Yuliya Bagriy]: https://github.com/aviskase\n[PyPI]: https://pypi.org/\n[Lucas Cimon]: https://github.com/Lucas-C\n[pytest]: https://pytest.org/\n[Justin Mayer]: https://github.com/justinmayer\n\nAuthor\n------\n\nCopyright (C) 2015, 2017, 2019, 2021, 2022  Rafael Laboissière (<rafael@laboissiere.net>)\n\nReleased under the GNU Affero Public License, version 3 or later. No warranties.\n",
-    'author': 'Rafael Laboissière',
-    'author_email': 'rafael@laboissiere.net',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/pelican-plugins/linkclass',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6.2,<4.0',
-}
+![figure](https://github.com/pelican-plugins/linkclass/raw/main/linkclass-example.png)
+
+Note that this plugin also works with reference-style links, as in the
+following example:
+
+```markdown
+This is an [internal][internal] link and this is an
+[external][external] link.
+
+ [internal]: internal
+ [external]: http://external.com
+```
+
+Contributing
+------------
+
+Contributions are welcome and much appreciated. Every little bit helps. You can contribute by improving the documentation, adding missing features, and fixing bugs. You can also help out by reviewing and commenting on [existing issues][].
+
+To start contributing to this plugin, review the [Contributing to Pelican][] documentation, beginning with the **Contributing Code** section.
+
+[existing issues]: https://github.com/pelican-plugins/linkclass/issues
+[Contributing to Pelican]: https://docs.getpelican.com/en/latest/contribute.html
+
+Acknowledgments
+---------------
+
+Many thanks to [Yuliya Bagriy][] for setting up the package for [PyPI][], to [Lucas Cimon][] for fixing the issues with [pytest][], and to [Justin Mayer][] for helping with migration of this plugin under the Pelican Plugins organization.
+
+[Yuliya Bagriy]: https://github.com/aviskase
+[PyPI]: https://pypi.org/
+[Lucas Cimon]: https://github.com/Lucas-C
+[pytest]: https://pytest.org/
+[Justin Mayer]: https://github.com/justinmayer
+
+Author
+------
+
+Copyright © 2015, 2017, 2019, 2021-2023 Rafael Laboissière (<rafael@laboissiere.net>)
 
+Released under the GNU Affero Public License, version 3 or later. No warranties.
 
-setup(**setup_kwargs)
```

