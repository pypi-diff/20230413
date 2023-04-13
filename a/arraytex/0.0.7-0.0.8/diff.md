# Comparing `tmp/arraytex-0.0.7.tar.gz` & `tmp/arraytex-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraytex-0.0.7.tar", max compression
+gzip compressed data, was "arraytex-0.0.8.tar", max compression
```

## Comparing `arraytex-0.0.7.tar` & `arraytex-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-04-11 16:41:58.785130 arraytex-0.0.7/LICENSE
--rw-r--r--   0        0        0     2982 2023-04-11 16:41:58.785130 arraytex-0.0.7/README.md
--rw-r--r--   0        0        0     2389 2023-04-11 16:42:15.609325 arraytex-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      112 2023-04-11 16:41:58.789131 arraytex-0.0.7/src/arraytex/__init__.py
--rw-r--r--   0        0        0      206 2023-04-11 16:41:58.789131 arraytex-0.0.7/src/arraytex/__main__.py
--rw-r--r--   0        0        0     4983 2023-04-11 16:42:15.609325 arraytex-0.0.7/src/arraytex/api.py
--rw-r--r--   0        0        0      243 2023-04-11 16:41:58.789131 arraytex-0.0.7/src/arraytex/errors.py
--rw-r--r--   0        0        0        0 2023-04-11 16:41:58.789131 arraytex-0.0.7/src/arraytex/py.typed
--rw-r--r--   0        0        0     1772 2023-04-11 16:41:58.789131 arraytex-0.0.7/src/arraytex/utils.py
--rw-r--r--   0        0        0     3970 1970-01-01 00:00:00.000000 arraytex-0.0.7/setup.py
--rw-r--r--   0        0        0     3945 1970-01-01 00:00:00.000000 arraytex-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-13 09:33:23.806359 arraytex-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2982 2023-04-13 09:33:23.806359 arraytex-0.0.8/README.md
+-rw-r--r--   0        0        0     2389 2023-04-13 09:33:49.310519 arraytex-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-04-13 09:33:23.806359 arraytex-0.0.8/src/arraytex/__init__.py
+-rw-r--r--   0        0        0      206 2023-04-13 09:33:23.806359 arraytex-0.0.8/src/arraytex/__main__.py
+-rw-r--r--   0        0        0     5033 2023-04-13 09:33:49.310519 arraytex-0.0.8/src/arraytex/api.py
+-rw-r--r--   0        0        0      243 2023-04-13 09:33:23.806359 arraytex-0.0.8/src/arraytex/errors.py
+-rw-r--r--   0        0        0        0 2023-04-13 09:33:23.806359 arraytex-0.0.8/src/arraytex/py.typed
+-rw-r--r--   0        0        0     1776 2023-04-13 09:33:49.314519 arraytex-0.0.8/src/arraytex/utils.py
+-rw-r--r--   0        0        0     3945 1970-01-01 00:00:00.000000 arraytex-0.0.8/PKG-INFO
```

### Comparing `arraytex-0.0.7/LICENSE` & `arraytex-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `arraytex-0.0.7/README.md` & `arraytex-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `arraytex-0.0.7/pyproject.toml` & `arraytex-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arraytex"
-version = "0.0.7"
+version = "0.0.8"
 description = "ArrayTeX"
 authors = ["Dom Batten <dominic.batten@googlemail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dbatten5/arraytex"
 repository = "https://github.com/dbatten5/arraytex"
 documentation = "https://arraytex.readthedocs.io"
```

### Comparing `arraytex-0.0.7/src/arraytex/api.py` & `arraytex-0.0.8/src/arraytex/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,16 @@
         to_clp: copy the output to the system clipboard
 
     Returns:
         the LaTeX tabular string representation of the array
 
     Raises:
         TooManyDimensionsError: when the supplied array has more than 2 dimensions
-        DimensionMismatchError: when there are mismatched column identifiers and
-            dimensions
+        DimensionMismatchError: when there is a mismatch between column items and number
+            of columns, or column index items and number of rows
     """
     n_dims = len(arr.shape)
 
     if n_dims == 0:
         n_cols = 1
     elif n_dims == 1:
         n_cols = arr.shape[0]
```

### Comparing `arraytex-0.0.7/src/arraytex/utils.py` & `arraytex-0.0.8/src/arraytex/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,14 @@
         )
         .replace("[", "")
         .replace("]", "")
         .replace(" &\n", "\n")
     )
 
     if num_format and "e" in num_format:
-        pattern = r"e(-?\d+)"
+        pattern = r"e([\+-]?\d+)"
         replace = r"\\mathrm{e}{\g<1>}"
         if scientific_notation:
             replace = r" \\times 10^{\g<1>}"
         lines = re.sub(pattern, replace, lines)
 
     return lines.splitlines()
```

### Comparing `arraytex-0.0.7/setup.py` & `arraytex-0.0.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,118 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: arraytex
+Version: 0.0.8
+Summary: ArrayTeX
+Home-page: https://github.com/dbatten5/arraytex
+License: MIT
+Author: Dom Batten
+Author-email: dominic.batten@googlemail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.0.1)
+Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Project-URL: Changelog, https://github.com/dbatten5/arraytex/releases
+Project-URL: Documentation, https://arraytex.readthedocs.io
+Project-URL: Repository, https://github.com/dbatten5/arraytex
+Description-Content-Type: text/markdown
+
+# ArrayTeX
+
+[![PyPI](https://img.shields.io/pypi/v/arraytex.svg)][pypi_]
+[![Status](https://img.shields.io/pypi/status/arraytex.svg)][status]
+[![Python Version](https://img.shields.io/pypi/pyversions/arraytex)][python version]
+[![License](https://img.shields.io/pypi/l/arraytex)][license]
+
+[![Read the documentation at https://arraytex.readthedocs.io/](https://img.shields.io/readthedocs/arraytex/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Tests](https://github.com/dbatten5/arraytex/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/dbatten5/arraytex/branch/main/graph/badge.svg)][codecov]
+
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+
+[pypi_]: https://pypi.org/project/arraytex/
+[status]: https://pypi.org/project/arraytex/
+[python version]: https://pypi.org/project/arraytex
+[read the docs]: https://arraytex.readthedocs.io/
+[tests]: https://github.com/dbatten5/arraytex/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/dbatten5/arraytex
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[black]: https://github.com/psf/black
+
+Convert a `numpy.NDArray` to various LaTeX forms.
+
+```python
+>>> import numpy as np
+>>> import arraytex as atx
+>>> A = np.array([[1, 2, 3], [4, 5, 6]])
+>>> print(atx.to_matrix(A))
+\begin{bmatrix}
+1 & 2 & 3 \\
+4 & 5 & 6 \\
+\end{bmatrix}
+```
+
+Inspired by [@josephcslater](https://github.com/josephcslater)'s
+[array_to_latex](https://github.com/josephcslater/array_to_latex).
+
+## Features
+
+- Support for different matrix environment delimiters, (`bmatrix`, `pmatrix`, etc.)
+- Support for tabular environments.
+- Support for builtin number formats (`:.2f`, `:.3e`, etc.).
+- Fully tested and typed.
+
+## Requirements
+
+- `python >= 3.8`
+
+## Installation
+
+You can install _ArrayTeX_ via [pip] from [PyPI]:
+
+```console
+$ pip install arraytex
+```
+
+## Usage
+
+Please see the [docs](https://arraytex.readthedocs.io/) for more information.
+
+## Contributing
+
+Contributions are very welcome.
+To learn more, see the [Contributor Guide].
+
+## License
+
+Distributed under the terms of the [MIT license][license],
+_ArrayTeX_ is free and open source software.
+
+## Issues
+
+If you encounter any problems,
+please [file an issue] along with a detailed description.
+
+## Credits
+
+This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
+
+[@cjolowicz]: https://github.com/cjolowicz
+[pypi]: https://pypi.org/
+[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+[file an issue]: https://github.com/dbatten5/arraytex/issues
+[pip]: https://pip.pypa.io/
+
+<!-- github-only -->
+
+[license]: https://github.com/dbatten5/arraytex/blob/main/LICENSE
+[contributor guide]: https://github.com/dbatten5/arraytex/blob/main/CONTRIBUTING.md
+[command-line reference]: https://arraytex.readthedocs.io/en/latest/usage.html
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['arraytex']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.0.1',
- 'numpy>=1.24.2,<2.0.0',
- 'pyperclip>=1.8.2,<2.0.0',
- 'typing-extensions>=4.5.0,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['arraytex = arraytex.__main__:main']}
-
-setup_kwargs = {
-    'name': 'arraytex',
-    'version': '0.0.7',
-    'description': 'ArrayTeX',
-    'long_description': "# ArrayTeX\n\n[![PyPI](https://img.shields.io/pypi/v/arraytex.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/arraytex.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/arraytex)][python version]\n[![License](https://img.shields.io/pypi/l/arraytex)][license]\n\n[![Read the documentation at https://arraytex.readthedocs.io/](https://img.shields.io/readthedocs/arraytex/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/dbatten5/arraytex/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/dbatten5/arraytex/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/arraytex/\n[status]: https://pypi.org/project/arraytex/\n[python version]: https://pypi.org/project/arraytex\n[read the docs]: https://arraytex.readthedocs.io/\n[tests]: https://github.com/dbatten5/arraytex/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/dbatten5/arraytex\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\nConvert a `numpy.NDArray` to various LaTeX forms.\n\n```python\n>>> import numpy as np\n>>> import arraytex as atx\n>>> A = np.array([[1, 2, 3], [4, 5, 6]])\n>>> print(atx.to_matrix(A))\n\\begin{bmatrix}\n1 & 2 & 3 \\\\\n4 & 5 & 6 \\\\\n\\end{bmatrix}\n```\n\nInspired by [@josephcslater](https://github.com/josephcslater)'s\n[array_to_latex](https://github.com/josephcslater/array_to_latex).\n\n## Features\n\n- Support for different matrix environment delimiters, (`bmatrix`, `pmatrix`, etc.)\n- Support for tabular environments.\n- Support for builtin number formats (`:.2f`, `:.3e`, etc.).\n- Fully tested and typed.\n\n## Requirements\n\n- `python >= 3.8`\n\n## Installation\n\nYou can install _ArrayTeX_ via [pip] from [PyPI]:\n\n```console\n$ pip install arraytex\n```\n\n## Usage\n\nPlease see the [docs](https://arraytex.readthedocs.io/) for more information.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_ArrayTeX_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/dbatten5/arraytex/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/dbatten5/arraytex/blob/main/LICENSE\n[contributor guide]: https://github.com/dbatten5/arraytex/blob/main/CONTRIBUTING.md\n[command-line reference]: https://arraytex.readthedocs.io/en/latest/usage.html\n",
-    'author': 'Dom Batten',
-    'author_email': 'dominic.batten@googlemail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/dbatten5/arraytex',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

