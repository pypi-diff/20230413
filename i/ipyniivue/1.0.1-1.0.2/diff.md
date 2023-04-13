# Comparing `tmp/ipyniivue-1.0.1.tar.gz` & `tmp/ipyniivue-1.0.2.tar.gz`

## Comparing `ipyniivue-1.0.1.tar` & `ipyniivue-1.0.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/.coveragerc
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/.eslintignore
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/.eslintrc.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/.npmignore
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/.prettierignore
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/.prettierrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/.yarnrc.yml
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/MANIFEST.in
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/babel.config.js
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/codecov.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/install.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue.json
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/jest.config.js
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/package.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/setup.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/tsconfig.eslint.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/tsconfig.json
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/webpack.config.js
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/css/widget.css
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/Makefile
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/environment.yml
--rw-r--r--   0        0        0   856986 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/example.png
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/make.bat
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/development-notes/attribute-docstrings.rst
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/development-notes/cell-syncing.rst
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/development-notes/py-ts-messaging.rst
--rw-r--r--   0        0        0   243278 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/development-notes/traceback.png
--rw-r--r--   0        0        0   150323 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/development-notes/ws.png
--rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/source/conf.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/source/develop-install.rst
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/source/index.rst
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/source/installing.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/source/introduction.rst
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/source/_static/embed-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/source/_static/helper.js
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/source/examples/index.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/docs/source/examples/introduction.nblink
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/examples/addobject.ipynb
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/examples/custom_code.ipynb
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/examples/draw.ipynb
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/examples/introduction.ipynb
--rw-r--r--   0        0        0   707836 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/examples/demo_images/CT_pitch.nii.gz
--rw-r--r--   0        0        0  4336029 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/examples/demo_images/mni152.nii.gz
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/_frontend.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/_version.py
--rw-r--r--   0        0        0    33670 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/niivue.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/traits.py
--rw-r--r--   0        0        0    20954 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/labextension/build_log.json
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/labextension/package.json
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/labextension/static/lib_index_js.6ffc91ccc740d1bae4db.js
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/labextension/static/lib_index_js.6ffc91ccc740d1bae4db.js.map
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/labextension/static/lib_plugin_js.4db7aec6cfaa2e3a5663.js
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/labextension/static/lib_plugin_js.4db7aec6cfaa2e3a5663.js.map
--rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/labextension/static/lib_widget_js.a86802843924a12afd11.js
--rw-r--r--   0        0        0    20971 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/labextension/static/lib_widget_js.a86802843924a12afd11.js.map
--rw-r--r--   0        0        0    27563 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/labextension/static/remoteEntry.f5a2a058628b49c62954.js
--rw-r--r--   0        0        0    26317 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/labextension/static/remoteEntry.f5a2a058628b49c62954.js.map
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/labextension/static/style.js
--rw-r--r--   0        0        0  3014460 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/labextension/static/vendors-node_modules_niivue_niivue_dist_niivue_es_js.2004dca03ee9fd191cd9.js
--rw-r--r--   0        0        0  3445145 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/labextension/static/vendors-node_modules_niivue_niivue_dist_niivue_es_js.2004dca03ee9fd191cd9.js.map
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/nbextension/extension.js
--rw-r--r--   0        0        0  1808568 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/nbextension/index.js
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0  2050655 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/nbextension/index.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/tests/__init__.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/tests/conftest.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/tests/test_example.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/ipyniivue/tests/test_nbextension_path.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/src/extension.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/src/index.ts
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/src/niivue.d.ts
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/src/plugin.ts
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/src/utils.ts
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/src/version.ts
--rw-r--r--   0        0        0     9733 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/src/widget.ts
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/src/__tests__/utils.ts
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/.gitignore
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/README.md
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 ipyniivue-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/.coveragerc
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/.eslintignore
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/.npmignore
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/.prettierignore
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/.prettierrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/.yarnrc.yml
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/MANIFEST.in
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/babel.config.js
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/codecov.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/install.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue.json
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/jest.config.js
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/package.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/setup.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/tsconfig.eslint.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/tsconfig.json
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/webpack.config.js
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/css/widget.css
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/environment.yml
+-rw-r--r--   0        0        0   856986 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/example.png
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/make.bat
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/development-notes/attribute-docstrings.rst
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/development-notes/cell-syncing.rst
+-rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/development-notes/py-ts-messaging.rst
+-rw-r--r--   0        0        0   243278 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/development-notes/traceback.png
+-rw-r--r--   0        0        0   150323 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/development-notes/ws.png
+-rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/source/conf.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/source/develop-install.rst
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/source/index.rst
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/source/installing.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/source/introduction.rst
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/source/_static/embed-bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/source/_static/helper.js
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/source/examples/index.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/docs/source/examples/introduction.nblink
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/examples/addobject.ipynb
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/examples/custom_code.ipynb
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/examples/draw.ipynb
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/examples/introduction.ipynb
+-rw-r--r--   0        0        0   707836 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/examples/demo_images/CT_pitch.nii.gz
+-rw-r--r--   0        0        0  4336029 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/examples/demo_images/mni152.nii.gz
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/_frontend.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/_version.py
+-rw-r--r--   0        0        0    33865 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/niivue.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/traits.py
+-rw-r--r--   0        0        0    20954 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/labextension/build_log.json
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/labextension/package.json
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/labextension/static/lib_index_js.6ffc91ccc740d1bae4db.js
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/labextension/static/lib_index_js.6ffc91ccc740d1bae4db.js.map
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/labextension/static/lib_plugin_js.4db7aec6cfaa2e3a5663.js
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/labextension/static/lib_plugin_js.4db7aec6cfaa2e3a5663.js.map
+-rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/labextension/static/lib_widget_js.dab26d8704b46bf7fde4.js
+-rw-r--r--   0        0        0    20971 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/labextension/static/lib_widget_js.dab26d8704b46bf7fde4.js.map
+-rw-r--r--   0        0        0    27563 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/labextension/static/remoteEntry.b043c37bb43deb442a61.js
+-rw-r--r--   0        0        0    26317 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/labextension/static/remoteEntry.b043c37bb43deb442a61.js.map
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/labextension/static/style.js
+-rw-r--r--   0        0        0  3014460 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/labextension/static/vendors-node_modules_niivue_niivue_dist_niivue_es_js.2004dca03ee9fd191cd9.js
+-rw-r--r--   0        0        0  3445145 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/labextension/static/vendors-node_modules_niivue_niivue_dist_niivue_es_js.2004dca03ee9fd191cd9.js.map
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/nbextension/extension.js
+-rw-r--r--   0        0        0  1808568 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/nbextension/index.js
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0  2050655 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/nbextension/index.js.map
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/tests/__init__.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/tests/conftest.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/tests/test_example.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/ipyniivue/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/src/extension.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/src/index.ts
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/src/niivue.d.ts
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/src/plugin.ts
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/src/utils.ts
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/src/version.ts
+-rw-r--r--   0        0        0     9733 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/src/widget.ts
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/src/__tests__/index.spec.ts
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/src/__tests__/utils.ts
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/README.md
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 ipyniivue-1.0.2/PKG-INFO
```

### Comparing `ipyniivue-1.0.1/.eslintrc.js` & `ipyniivue-1.0.2/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/MANIFEST.in` & `ipyniivue-1.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/package.json` & `ipyniivue-1.0.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'1.0.2'"}*

```diff
@@ -89,9 +89,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.0.2"
 }
```

### Comparing `ipyniivue-1.0.1/tsconfig.json` & `ipyniivue-1.0.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/webpack.config.js` & `ipyniivue-1.0.2/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/docs/Makefile` & `ipyniivue-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/docs/example.png` & `ipyniivue-1.0.2/docs/example.png`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/docs/make.bat` & `ipyniivue-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/docs/development-notes/attribute-docstrings.rst` & `ipyniivue-1.0.2/docs/development-notes/attribute-docstrings.rst`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/docs/development-notes/py-ts-messaging.rst` & `ipyniivue-1.0.2/docs/development-notes/py-ts-messaging.rst`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/docs/development-notes/traceback.png` & `ipyniivue-1.0.2/docs/development-notes/traceback.png`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/docs/development-notes/ws.png` & `ipyniivue-1.0.2/docs/development-notes/ws.png`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/docs/source/conf.py` & `ipyniivue-1.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/docs/source/develop-install.rst` & `ipyniivue-1.0.2/docs/source/develop-install.rst`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/docs/source/index.rst` & `ipyniivue-1.0.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/docs/source/installing.rst` & `ipyniivue-1.0.2/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/docs/source/_static/embed-bundle.js.LICENSE.txt` & `ipyniivue-1.0.2/docs/source/_static/embed-bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/examples/addobject.ipynb` & `ipyniivue-1.0.2/examples/addobject.ipynb`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/examples/custom_code.ipynb` & `ipyniivue-1.0.2/examples/custom_code.ipynb`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/examples/draw.ipynb` & `ipyniivue-1.0.2/examples/draw.ipynb`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/examples/introduction.ipynb` & `ipyniivue-1.0.2/examples/introduction.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9610119047619048%*

 * *Differences: {"'cells'": "{1: {'execution_count': None}, 2: {'source': ['nv = "*

 * *            "ipyniivue.Niivue(crosshair_color=[0,1,0,1])\\n', "*

 * *            '"nv.add_volume(\'https://niivue.github.io/niivue/images/mni152.nii.gz\')\\n", '*

 * *            "'nv']}, delete: [2]}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.3'}}"}*

```diff
@@ -5,53 +5,31 @@
             "metadata": {},
             "source": [
                 "# Introduction"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import ipyniivue"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "0cb78531b52b44b18079b3b1e7e3d006",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "Niivue(back_color=[0.0, 0.0, 0.0, 1.0], clip_plane_color=[1.0, 1.0, 1.0, 0.5], crosshair_color=[0.0, 1.0, 0.0,\u2026"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                }
-            ],
+            "outputs": [],
             "source": [
                 "nv = ipyniivue.Niivue(crosshair_color=[0,1,0,1])\n",
                 "nv.add_volume('https://niivue.github.io/niivue/images/mni152.nii.gz')\n",
                 "nv"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -62,15 +40,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.11.3"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
                 "state": {},
                 "version_major": 2,
                 "version_minor": 0
             }
```

### Comparing `ipyniivue-1.0.1/examples/demo_images/CT_pitch.nii.gz` & `ipyniivue-1.0.2/examples/demo_images/CT_pitch.nii.gz`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/examples/demo_images/mni152.nii.gz` & `ipyniivue-1.0.2/examples/demo_images/mni152.nii.gz`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/ipyniivue/__init__.py` & `ipyniivue-1.0.2/ipyniivue/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/ipyniivue/niivue.py` & `ipyniivue-1.0.2/ipyniivue/niivue.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,24 @@
 	slice_type = SliceType
 
 	def __init__(self, *args, **kwargs):
 		'''Create an Niivue widget.'''
 		super(Niivue, self).__init__(*args, **kwargs)
 		self.on_msg(self._handle_frontend_msg)
 
+	def __str__(self):
+		return f'Niivue {self._model_id}'
+	
+	def __repr__(self):
+		return f'ipyniivue.{super().__repr__()}'
+
+	def __dir__(self):
+		default = super().__dir__()
+		return [d for d in default if d not in dir(DOMWidget)]
+
 	def _handle_frontend_msg(self, _, content, buffers):
 		event_data = content.get('event', [None])
 		if event_data[0] == 'customCodeResult':
 			code_id = event_data[1]
 			chunks_left = event_data[2]
 			if code_id not in self._custom_code_results:
 				self._custom_code_results[code_id] = {
@@ -975,15 +985,15 @@
 	def get_frame_4D(self, ID):
 		'''
 		determine active 3D volume from 4D time series
 
 		Parameters:
 		-----------
 		ID: str
-            the ID of the 4D image
+			the ID of the 4D image
 
 		Returns:
 		--------
 		int
 		'''
 		return self.run_custom_code(f'this.nv.getFrame4D({ID})')
 
@@ -1004,15 +1014,15 @@
 	def get_overlay_index_by_ID(self, ID):
 		'''
 		get the index of an overlay by its unique id. unique ids are assigned to the NVImage.id property when a new NVImage is created.
 
 		Parameters:
 		-----------
 		ID: str
-            the ID of the overlay
+			the ID of the overlay
 
 		Returns:
 		--------
 		int
 		'''
 		return self.run_custom_code(f'this.nv.getOverlayIndexByID({ID})')
 
@@ -1029,29 +1039,29 @@
 	def get_volume_index_by_ID(self, ID):
 		'''
 		get the index of a volume by its unique id. unique ids are assigned to the NVImage.id property when a new NVImage is created.
 
 		Parameters:
 		-----------
 		ID: str
-            the ID of the volume
+			the ID of the volume
 
 		Returns:
 		--------
 		int
 		'''
 		return self.run_custom_code(f'this.nv.getVolumeIndexByID({ID})')
 
 	def is_mesh_ext(self, url):
 		'''
 		Returns boolean: true if filename ends with mesh extension (TRK, pial, etc)
 
 		Parameters:
 		-----------
 		url: str
-            the url or filepath of the mesh
+			the url or filepath of the mesh
 
 		Returns:
 		--------
 		bool
 		'''
 		return self.run_custom_code(f'this.nv.isMeshExt({url})')
```

### Comparing `ipyniivue-1.0.1/ipyniivue/traits.py` & `ipyniivue-1.0.2/ipyniivue/traits.py`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/ipyniivue/labextension/build_log.json` & `ipyniivue-1.0.2/ipyniivue/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999999304860416%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'ipyniivue': {'version': '1.0.2'}}}}}}"}*

```diff
@@ -591,15 +591,15 @@
                             "requiredVersion": "^1.33.0",
                             "singleton": true
                         },
                         "@niivue/niivue": {},
                         "ipyniivue": {
                             "import": "/Users/rorden/Documents/GitHub/ipyniivue/lib/index.js",
                             "singleton": true,
-                            "version": "1.0.1"
+                            "version": "1.0.2"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "react-dom": {
```

### Comparing `ipyniivue-1.0.1/ipyniivue/labextension/package.json` & `ipyniivue-1.0.2/ipyniivue/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9677734375%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b043c37bb43deb442a61.js'}}",*

 * * "'version'": "'1.0.2'"}*

```diff
@@ -48,15 +48,15 @@
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/niivue/ipyniivue",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f5a2a058628b49c62954.js"
+            "load": "static/remoteEntry.b043c37bb43deb442a61.js"
         },
         "extension": "lib/plugin",
         "outputDir": "ipyniivue/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -93,9 +93,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.0.2"
 }
```

### Comparing `ipyniivue-1.0.1/ipyniivue/labextension/static/lib_index_js.6ffc91ccc740d1bae4db.js` & `ipyniivue-1.0.2/ipyniivue/labextension/static/lib_index_js.6ffc91ccc740d1bae4db.js`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/ipyniivue/labextension/static/lib_plugin_js.4db7aec6cfaa2e3a5663.js` & `ipyniivue-1.0.2/ipyniivue/labextension/static/lib_plugin_js.4db7aec6cfaa2e3a5663.js`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/ipyniivue/labextension/static/lib_plugin_js.4db7aec6cfaa2e3a5663.js.map` & `ipyniivue-1.0.2/ipyniivue/labextension/static/lib_plugin_js.4db7aec6cfaa2e3a5663.js.map`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/ipyniivue/labextension/static/lib_widget_js.a86802843924a12afd11.js` & `ipyniivue-1.0.2/ipyniivue/labextension/static/lib_widget_js.dab26d8704b46bf7fde4.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -397,15 +397,15 @@
         "./package.json":
             /*!**********************!*\
               !*** ./package.json ***!
               \**********************/
             /***/
             ((module) => {
 
-                module.exports = JSON.parse('{"name":"ipyniivue","version":"1.0.1","description":"Jupyter-Niivue bridge","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/niivue/ipyniivue","bugs":{"url":"https://github.com/niivue/ipyniivue/issues"},"license":"BSD-3-Clause","author":{"name":"Niivue"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/niivue/ipyniivue"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyniivue/labextension","clean:nbextension":"rimraf ipyniivue/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","@niivue/niivue":"^0.33.1"},"devDependencies":{"@babel/core":"^7.21.4","@babel/preset-env":"^7.21.4","@babel/preset-typescript":"^7.21.4","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","babel-jest":"^29.5.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.6.3","mkdirp":"^0.5.1","npm-run-all":"^4.1.5","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.5.6","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyniivue/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
+                module.exports = JSON.parse('{"name":"ipyniivue","version":"1.0.2","description":"Jupyter-Niivue bridge","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/niivue/ipyniivue","bugs":{"url":"https://github.com/niivue/ipyniivue/issues"},"license":"BSD-3-Clause","author":{"name":"Niivue"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/niivue/ipyniivue"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyniivue/labextension","clean:nbextension":"rimraf ipyniivue/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","@niivue/niivue":"^0.33.1"},"devDependencies":{"@babel/core":"^7.21.4","@babel/preset-env":"^7.21.4","@babel/preset-typescript":"^7.21.4","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","babel-jest":"^29.5.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.6.3","mkdirp":"^0.5.1","npm-run-all":"^4.1.5","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.5.6","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyniivue/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_widget_js.a86802843924a12afd11.js.map
+//# sourceMappingURL=lib_widget_js.dab26d8704b46bf7fde4.js.map
```

### Comparing `ipyniivue-1.0.1/ipyniivue/labextension/static/lib_widget_js.a86802843924a12afd11.js.map` & `ipyniivue-1.0.2/ipyniivue/labextension/static/lib_widget_js.dab26d8704b46bf7fde4.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'file'": "'lib_widget_js.dab26d8704b46bf7fde4.js'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "lib_widget_js.a86802843924a12afd11.js",
+    "file": "lib_widget_js.dab26d8704b46bf7fde4.js",
     "mappings": ";;;;;;;;;;;;AAAA,qCAAqC;AACrC,SAAgB,mBAAmB,CAAC,MAAmB;IACrD,IAAI,MAAM,GAAG,EAAE,CAAC;IAChB,MAAM,KAAK,GAAG,IAAI,UAAU,CAAC,MAAM,CAAC,CAAC;IACrC,MAAM,GAAG,GAAG,KAAK,CAAC,UAAU,CAAC;IAC7B,KAAK,IAAI,CAAC,GAAG,CAAC,EAAE,CAAC,GAAG,GAAG,EAAE,CAAC,EAAE,EAAE;QAC5B,MAAM,IAAI,MAAM,CAAC,YAAY,CAAC,KAAK,CAAC,CAAC,CAAC,CAAC,CAAC;KACzC;IACD,OAAO,IAAI,CAAC,MAAM,CAAC,CAAC;AACtB,CAAC;AARD,kDAQC;AAED,kFAAkF;AAClF,SAAgB,mBAAmB,CAAC,MAAmB;IACrD,MAAM,KAAK,GAAG,IAAI,UAAU,CAAC,MAAM,CAAC,CAAC;IACrC,OAAO,MAAM,CAAC,YAAY,CAAC,KAAK,CAAC,IAAI,EAAE,CAAC,GAAG,KAAK,CAAC,CAAC,CAAC;AACrD,CAAC;AAHD,kDAGC;AAED,SAAgB,mBAAmB,CAAC,GAAW;IAC7C,MAAM,GAAG,GAAG,IAAI,WAAW,CAAC,GAAG,CAAC,MAAM,CAAC,CAAC;IACxC,MAAM,OAAO,GAAG,IAAI,UAAU,CAAC,GAAG,CAAC,CAAC;IACpC,KAAK,IAAI,CAAC,GAAG,CAAC,EAAE,MAAM,GAAG,GAAG,CAAC,MAAM,EAAE,CAAC,GAAG,MAAM,EAAE,CAAC,EAAE,EAAE;QACpD,OAAO,CAAC,CAAC,CAAC,GAAG,GAAG,CAAC,UAAU,CAAC,CAAC,CAAC,CAAC;KAChC;IACD,OAAO,GAAG,CAAC;AACb,CAAC;AAPD,kDAOC;;;;;;;;;;;;ACxBD,uBAAuB;AACvB,2DAA2D;;;AAE3D,6DAA6D;AAC7D,aAAa;AACb,8DAA8D;AAC9D,MAAM,IAAI,GAAG,mBAAO,CAAC,uCAAiB,CAAC,CAAC;AAExC;;;;;GAKG;AACU,sBAAc,GAAG,IAAI,CAAC,OAAO,CAAC;AAE3C;;GAEG;AACU,mBAAW,GAAG,IAAI,CAAC,IAAI,CAAC;;;;;;;;;;;;ACnBrC,uBAAuB;AACvB,2DAA2D;;;;;;;;;;;;;;;;;;;;;;AAE3D,uEAAuE;AACvE,yIAAyI;AAEzI,yHAI+B;AAE/B,2EAAwD;AAExD,wIAAyC;AAEzC,qEAIiB;AAEjB,MAAM,OAAO,GAAa;IACxB,WAAW;IACX,kBAAkB;IAClB,mBAAmB;IACnB,0BAA0B;IAC1B,2BAA2B;IAC3B,sBAAsB;IACtB,sBAAsB;IACtB,YAAY;IACZ,0BAA0B;IAC1B,WAAW;IACX,SAAS;IACT,UAAU;IACV,oBAAoB;IACpB,UAAU;IACV,YAAY;IACZ,WAAW;IACX,iBAAiB;IACjB,cAAc;IACd,sBAAsB;IACtB,eAAe;IACf,2BAA2B;IAC3B,WAAW;IACX,cAAc;IACd,qBAAqB;IACrB,YAAY;IACZ,iBAAiB;IACjB,oBAAoB;IACpB,cAAc;IACd,gBAAgB;IAChB,iBAAiB;IACjB,cAAc;IACd,mBAAmB;IACnB,mBAAmB;IACnB,mBAAmB;IACnB,aAAa;IACb,gBAAgB;IAChB,sBAAsB;IACtB,cAAc;IACd,YAAY;IACZ,UAAU;IACV,mBAAmB;IACnB,qBAAqB;IACrB,aAAa;IACb,gBAAgB;IAChB,YAAY;IACZ,gBAAgB;IAChB,oBAAoB;IACpB,aAAa;IACb,eAAe;IACf,qBAAqB;IACrB,gBAAgB;IAChB,aAAa;IACb,qBAAqB;IACrB,oBAAoB;IACpB,YAAY;IACZ,kBAAkB;IAClB,oBAAoB;IACpB,YAAY;CACb,CAAC;AAEF,MAAa,WAAY,SAAQ,qBAAc;IAA/C;;QA4KU,sBAAiB,GAAkB,OAAO,CAAC,OAAO,EAAE,CAAC;IAS/D,CAAC;IApLC,QAAQ;QACN,uCACK,KAAK,CAAC,QAAQ,EAAE,KACnB,WAAW,EAAE,WAAW,CAAC,UAAU,EACnC,aAAa,EAAE,WAAW,CAAC,YAAY,EACvC,qBAAqB,EAAE,WAAW,CAAC,oBAAoB,EACvD,UAAU,EAAE,WAAW,CAAC,SAAS,EACjC,YAAY,EAAE,WAAW,CAAC,WAAW,EACrC,oBAAoB,EAAE,WAAW,CAAC,mBAAmB,IACrD;IACJ,CAAC;IAOD,UAAU,CAAC,UAAe,EAAE,OAAY;QACtC,KAAK,CAAC,UAAU,CAAC,UAAU,EAAE,OAAO,CAAC,CAAC;QAEtC,IAAI,CAAC,EAAE,CAAC,YAAY,EAAE,CAAC,OAAY,EAAE,OAAY,EAAE,EAAE;YACnD,IAAI,CAAC,iBAAiB,GAAG,IAAI,CAAC,iBAAiB,CAAC,IAAI,CAAC,KAAK,IAAI,EAAE;gBAC9D,MAAM,IAAI,CAAC,SAAS,CAAC,OAAO,EAAE,OAAO,CAAC,CAAC;YACzC,CAAC,CAAC,CAAC;QACL,CAAC,CAAC,CAAC;QAEH,IAAI,CAAC,QAAQ,EAAE,CAAC;IAClB,CAAC;IAEO,KAAK,CAAC,oBAAoB,CAAC,YAAoB,EAAE,QAAe;QACtE,MAAM,OAAO,GAAG,IAAI,CAAC,EAAE,CAAC,YAAY,CAAC,CAAC,WAAW,CAAC,IAAI,KAAK,eAAe,CAAC;QAE3E,wCAAwC;QACxC,IAAI,OAAO,EAAE;YACX,MAAM,IAAI,CAAC,EAAE,CAAC,YAAY,CAAC,CAAC,GAAG,QAAQ,CAAC,CAAC;SAC1C;aAAM;YACL,IAAI,CAAC,EAAE,CAAC,YAAY,CAAC,CAAC,GAAG,QAAQ,CAAC,CAAC;SACpC;IACH,CAAC;IAEO,KAAK,CAAC,SAAS,CAAC,OAAY,EAAE,OAAmB;QACvD,MAAM,IAAI,GAAW,OAAO,CAAC,CAAC,CAAC,CAAC;QAChC,MAAM,IAAI,GAAU,OAAO,CAAC,CAAC,CAAC,CAAC;QAC/B,IAAI;YACF,MAAM,IAAI,CAAC,cAAc,CAAC,IAAI,EAAE,IAAI,EAAE,OAAO,CAAC,CAAC;SAChD;QAAC,OAAO,CAAC,EAAE;YACV,IAAI,CAAC,YAAY,KAAK,EAAE;gBACtB,IACE,CAAC,CAAC,IAAI,KAAK,WAAW;oBACtB,CAAC,CAAC,OAAO;wBACP,0DAA0D,EAC5D;oBACA,OAAO,CAAC,IAAI,CACV,sFAAsF,CACvF,CAAC;oBACF,OAAO;iBACR;gBACD,OAAO,CAAC,KAAK,CAAC,CAAC,CAAC,CAAC;aAClB;SACF;IACH,CAAC;IAEO,KAAK,CAAC,cAAc,CAAC,IAAY,EAAE,IAAW,EAAE,OAAmB;QACzE,IAAI,OAAO,CAAC,QAAQ,CAAC,IAAI,CAAC,EAAE;YAC1B,IAAI,CAAC,oBAAoB,CAAC,IAAI,EAAE,IAAI,CAAC,CAAC;SACvC;QACD,QAAQ,IAAI,EAAE;YACZ,KAAK,qBAAqB;gBACxB,IAAI,CAAC,EAAE,CAAC,SAAS,CACf,MAAM,CAAC,OAAO,CAAC,cAAc,CAAC;oBAC5B,IAAI,EAAE,IAAI,CAAC,CAAC,CAAC;oBACb,MAAM,EAAE,2BAAmB,CAAC,OAAO,CAAC,CAAC,CAAC,CAAC,MAAM,CAAC;iBAC/C,CAAC,CACH,CAAC;gBACF,MAAM;YACR,KAAK,eAAe,CAAC,CAAC;gBACpB,IAAI,MAAM,EACR,SAAS,GAAG,KAAK,CAAC;gBACpB,MAAM,IAAI,GAAG,2BAAmB,CAAC,OAAO,CAAC,CAAC,CAAC,CAAC,MAAM,CAAC,CAAC;gBACpD,IAAI;oBACF,MAAM,GAAG,IAAI,CAAC,IAAI,CAAC,CAAC;oBACpB,SAAS,GAAG,IAAI,CAAC;iBAClB;gBAAC,OAAO,CAAC,EAAE;oBACV,IAAI,CAAC,YAAY,KAAK,EAAE;wBACtB,OAAO,CAAC,KAAK,CAAC,CAAC,CAAC,KAAK,CAAC,CAAC;qBACxB;iBACF;gBACD,IAAI,CAAC,oBAAoB,CAAC,IAAI,CAAC,CAAC,CAAC,EAAE,SAAS,EAAE,MAAM,CAAC,CAAC;gBACtD,MAAM;aACP;SACF;IACH,CAAC;IAEO,oBAAoB,CAAC,EAAU,EAAE,SAAkB,EAAE,MAAW;QACtE,IAAI,IAAI,GAAgB,IAAI,WAAW,CAAC,CAAC,CAAC,CAAC;QAC3C,IAAI,SAAS,EAAE;YACb,MAAM,GAAG,GAAG,MAAM,KAAK,SAAS,CAAC,CAAC,CAAC,WAAW,CAAC,CAAC,CAAC,IAAI,CAAC,SAAS,CAAC,MAAM,CAAC,CAAC;YACxE,IAAI,GAAG,2BAAmB,CAAC,GAAG,CAAC,CAAC;SACjC;QAED,4BAA4B;QAC5B,MAAM,SAAS,GAAG,CAAC,GAAG,IAAI,GAAG,IAAI,CAAC;QAClC,MAAM,SAAS,GAAG,IAAI,CAAC,IAAI,CAAC,IAAI,CAAC,UAAU,GAAG,SAAS,CAAC,CAAC;QACzD,KAAK,IAAI,CAAC,GAAG,CAAC,EAAE,CAAC,GAAG,SAAS,EAAE,EAAE,CAAC,EAAE;YAClC,MAAM,KAAK,GAAG,CAAC,GAAG,SAAS,CAAC;YAC5B,MAAM,GAAG,GAAG,IAAI,CAAC,GAAG,CAAC,KAAK,GAAG,SAAS,EAAE,IAAI,CAAC,UAAU,CAAC,CAAC;YACzD,MAAM,KAAK,GAAG,IAAI,CAAC,KAAK,CAAC,KAAK,EAAE,GAAG,CAAC,CAAC;YACrC,IAAI,CAAC,IAAI,CAAC,EAAE,KAAK,EAAE,CAAC,kBAAkB,EAAE,EAAE,EAAE,SAAS,GAAG,CAAC,GAAG,CAAC,CAAC,EAAE,EAAE,EAAE,EAAE;gBACpE,KAAK;aACN,CAAC,CAAC;SACJ;QACD,IAAI,SAAS,KAAK,CAAC,EAAE;YACnB,IAAI,CAAC,IAAI,CAAC,EAAE,KAAK,EAAE,CAAC,kBAAkB,EAAE,EAAE,EAAE,CAAC,CAAC,EAAE,EAAE,EAAE,CAAC,CAAC;SACvD;IACH,CAAC;IAEO,KAAK,CAAC,QAAQ;QACpB,IAAI,CAAC,EAAE,GAAG,IAAI,MAAM,CAAC,MAAM,CAAC;YAC1B,cAAc,EAAE,KAAK;YACrB,OAAO,EAAE,IAAI;YAEb,UAAU,EAAE,IAAI,CAAC,GAAG,CAAC,aAAa,CAAC;YACnC,cAAc,EAAE,IAAI,CAAC,GAAG,CAAC,iBAAiB,CAAC;YAC3C,cAAc,EAAE,IAAI,CAAC,GAAG,CAAC,iBAAiB,CAAC;YAC3C,cAAc,EAAE,IAAI,CAAC,GAAG,CAAC,iBAAiB,CAAC;YAC3C,UAAU,EAAE,IAAI,CAAC,GAAG,CAAC,aAAa,CAAC;YACnC,SAAS,EAAE,IAAI,CAAC,GAAG,CAAC,YAAY,CAAC;YACjC,cAAc,EAAE,IAAI,CAAC,GAAG,CAAC,iBAAiB,CAAC;YAC3C,SAAS,EAAE,IAAI,CAAC,GAAG,CAAC,YAAY,CAAC;YACjC,iBAAiB,EAAE,IAAI,CAAC,GAAG,CAAC,qBAAqB,CAAC;YAClD,cAAc,EAAE,IAAI,CAAC,GAAG,CAAC,kBAAkB,CAAC;YAC5C,UAAU,EAAE,IAAI,CAAC,GAAG,CAAC,aAAa,CAAC;YACnC,eAAe,EAAE,IAAI,CAAC,GAAG,CAAC,mBAAmB,CAAC;YAC9C,cAAc,EAAE,IAAI,CAAC,GAAG,CAAC,mBAAmB,CAAC;YAC7C,eAAe,EAAE,IAAI,CAAC,GAAG,CAAC,oBAAoB,CAAC;YAC/C,cAAc,EAAE,IAAI,CAAC,GAAG,CAAC,mBAAmB,CAAC;YAC7C,eAAe,EAAE,IAAI,CAAC,GAAG,CAAC,mBAAmB,CAAC;YAC9C,kBAAkB,EAAE,IAAI,CAAC,GAAG,CAAC,sBAAsB,CAAC;YACpD,gBAAgB,EAAE,IAAI,CAAC,GAAG,CAAC,oBAAoB,CAAC;YAChD,wBAAwB,EAAE,IAAI,CAAC,GAAG,CAAC,4BAA4B,CAAC;YAChE,WAAW,EAAE,IAAI,CAAC,GAAG,CAAC,cAAc,CAAC;YACrC,kBAAkB,EAAE,IAAI,CAAC,GAAG,CAAC,uBAAuB,CAAC;YACrD,sBAAsB,EAAE,IAAI,CAAC,GAAG,CAAC,0BAA0B,CAAC;YAC5D,cAAc,EAAE,IAAI,CAAC,GAAG,CAAC,kBAAkB,CAAC;YAC5C,OAAO,EAAE,IAAI,CAAC,GAAG,CAAC,UAAU,CAAC;YAC7B,UAAU,EAAE,IAAI,CAAC,GAAG,CAAC,aAAa,CAAC;YACnC,YAAY,EAAE,IAAI,CAAC,GAAG,CAAC,gBAAgB,CAAC;YACxC,oBAAoB,EAAE,IAAI,CAAC,GAAG,CAAC,wBAAwB,CAAC;YACxD,sBAAsB,EAAE,IAAI,CAAC,GAAG,CAAC,0BAA0B,CAAC;YAC5D,iBAAiB,EACf,IAAI,CAAC,GAAG,CAAC,sBAAsB,CAAC,KAAK,sBAAsB;gBACzD,CAAC,CAAC,SAAS;gBACX,CAAC,CAAC,IAAI,CAAC,GAAG,CAAC,sBAAsB,CAAC;YACtC,QAAQ,EAAE,IAAI,CAAC,GAAG,CAAC,WAAW,CAAC;YAC/B,eAAe,EAAE,IAAI,CAAC,GAAG,CAAC,oBAAoB,CAAC;YAC/C,uBAAuB,EAAE,IAAI,CAAC,GAAG,CAAC,4BAA4B,CAAC;YAC/D,gBAAgB,EAAE,IAAI,CAAC,GAAG,CAAC,oBAAoB,CAAC;YAChD,SAAS,EAAE,IAAI,CAAC,GAAG,CAAC,aAAa,CAAC;YAClC,uBAAuB,EAAE,IAAI,CAAC,GAAG,CAAC,4BAA4B,CAAC;YAC/D,cAAc,EAAE,IAAI,CAAC,GAAG,CAAC,iBAAiB,CAAC;YAC3C,QAAQ,EACN,IAAI,CAAC,GAAG,CAAC,WAAW,CAAC,KAAK,sBAAsB;gBAC9C,CAAC,CAAC,SAAS;gBACX,CAAC,CAAC,IAAI,CAAC,GAAG,CAAC,WAAW,CAAC;YAC3B,WAAW,EAAE,IAAI,CAAC,GAAG,CAAC,eAAe,CAAC;YACtC,kBAAkB,EAAE,IAAI,CAAC,GAAG,CAAC,uBAAuB,CAAC;YACrD,SAAS,EAAE,IAAI,CAAC,GAAG,CAAC,WAAW,CAAC,IAAI,EAAE;SACvC,CAAC,CAAC;QACH,OAAO,CAAC,GAAG,CAAC,IAAI,CAAC,EAAE,CAAC,QAAQ,CAAC,CAAC;IAChC,CAAC;;AA1KH,kCAqLC;AAxKQ,uBAAW,qBACb,qBAAc,CAAC,WAAW,EAE7B;AA+JK,sBAAU,GAAG,aAAa,CAAC;AAC3B,wBAAY,GAAG,qBAAW,CAAC;AAC3B,gCAAoB,GAAG,wBAAc,CAAC;AACtC,qBAAS,GAAG,YAAY,CAAC,CAAC,yBAAyB;AACnD,uBAAW,GAAG,qBAAW,CAAC,CAAC,yBAAyB;AACpD,+BAAmB,GAAG,wBAAc,CAAC;AAG9C,MAAa,UAAW,SAAQ,oBAAa;IAC3C,8CAA8C;IAC9C,MAAM;QACJ,oDAAoD;QACpD,eAAe;QACf,mGAAmG;QACnG,mJAAmJ;QACnJ,IAAI,CAAC,MAAM,GAAG,QAAQ,CAAC,aAAa,CAAC,QAAQ,CAAC,CAAC;QAC/C,IAAI,CAAC,MAAM,CAAC,SAAS,CAAC,GAAG,CAAC,eAAe,CAAC,CAAC;QAE3C,IAAI,CAAC,MAAM,EAAE,CAAC;QACd,IAAI,CAAC,YAAY,EAAE,CAAC;QACpB,uBAAuB;QAEvB,IAAI,CAAC,KAAK,CAAC,cAAc,CAAC,CAAC,OAAO,EAAE,QAAQ,CAAC,EAAE,IAAI,CAAC,MAAM,EAAE,IAAI,CAAC,CAAC;QAClE,0DAA0D;IAC5D,CAAC;IAES,MAAM;QACd,YAAY;QACZ,IAAI,CAAC,EAAE,CAAC,YAAY,CAAC,OAAO,EAAE,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,OAAO,CAAC,CAAC,CAAC;QACvD,IAAI,CAAC,EAAE,CAAC,YAAY,CAAC,QAAQ,EAAE,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,QAAQ,CAAC,CAAC,CAAC;QACzD,IAAI,CAAC,EAAE,CAAC,YAAY,CAClB,OAAO,EACP,UAAU,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,OAAO,CAAC,eAAe,IAAI,CAAC,KAAK,CAAC,GAAG,CAC5D,QAAQ,CACT,KAAK,CACP,CAAC;QACF,eAAe;QACf,IAAI,CAAC,MAAM,CAAC,YAAY,CAAC,OAAO,EAAE,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,OAAO,CAAC,CAAC,CAAC;QAC3D,IAAI,CAAC,MAAM,CAAC,YAAY,CAAC,QAAQ,EAAE,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,QAAQ,CAAC,CAAC,CAAC;QAC7D,IAAI,CAAC,MAAM,CAAC,YAAY,CACtB,OAAO,EACP,UAAU,IAAI,CAAC,KAAK,CAAC,GAAG,CAAC,OAAO,CAAC,eAAe,IAAI,CAAC,KAAK,CAAC,GAAG,CAC5D,QAAQ,CACT,GAAG,CACL,CAAC;QACF,QAAQ;QACR,IAAI,CAAC,KAAK,CAAC,EAAE,CAAC,SAAS,EAAE,CAAC;IAC5B,CAAC;IAED,YAAY;QACV,IAAI,CAAC,EAAE,CAAC,WAAW,CAAC,IAAI,CAAC,MAAM,CAAC,CAAC;QACjC,IAAI,CAAC,KAAK,CAAC,EAAE,CAAC,cAAc,CAAC,IAAI,CAAC,MAAM,CAAC,CAAC;QAC1C,IAAI,CAAC,EAAE,CAAC,KAAK,CAAC,eAAe,GAAG,aAAa,CAAC;IAChD,CAAC;CAKF;AAlDD,gCAkDC",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://ipyniivue/./src/utils.ts",
         "webpack://ipyniivue/./src/version.ts",
         "webpack://ipyniivue/./src/widget.ts"
```

### Comparing `ipyniivue-1.0.1/ipyniivue/labextension/static/remoteEntry.f5a2a058628b49c62954.js` & `ipyniivue-1.0.2/ipyniivue/labextension/static/remoteEntry.b043c37bb43deb442a61.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -154,15 +154,15 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_widget_js": "a86802843924a12afd11",
+                "lib_widget_js": "dab26d8704b46bf7fde4",
                 "lib_index_js": "6ffc91ccc740d1bae4db",
                 "lib_plugin_js": "4db7aec6cfaa2e3a5663",
                 "vendors-node_modules_niivue_niivue_dist_niivue_es_js": "2004dca03ee9fd191cd9"
             } [chunkId] + ".js";
             /******/
         };
         /******/
@@ -398,15 +398,15 @@
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
                     register("@niivue/niivue", "0.33.1", () => (__webpack_require__.e("vendors-node_modules_niivue_niivue_dist_niivue_es_js").then(() => (() => (__webpack_require__( /*! ./node_modules/@niivue/niivue/dist/niivue.es.js */ "./node_modules/@niivue/niivue/dist/niivue.es.js"))))));
                     /******/
-                    register("ipyniivue", "1.0.1", () => (Promise.all([__webpack_require__.e("lib_widget_js"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("ipyniivue", "1.0.2", () => (Promise.all([__webpack_require__.e("lib_widget_js"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -1032,8 +1032,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/ipyniivue");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).ipyniivue = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.f5a2a058628b49c62954.js.map
+//# sourceMappingURL=remoteEntry.b043c37bb43deb442a61.js.map
```

### Comparing `ipyniivue-1.0.1/ipyniivue/labextension/static/remoteEntry.f5a2a058628b49c62954.js.map` & `ipyniivue-1.0.2/ipyniivue/labextension/static/remoteEntry.b043c37bb43deb442a61.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9126984126984128%*

 * *Differences: {"'file'": "'remoteEntry.b043c37bb43deb442a61.js'",*

 * * "'sourcesContent'": "{insert: [(4, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"lib_widget_js":"dab26d8704b46bf7fde4","lib_index_js":"6ffc91ccc740d1bae4db","lib_plugin_js":"4db7aec6cfaa2e3a5663","vendors-node_modules_niivue_niivue_dist_niivue_es_js":"2004 […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.f5a2a058628b49c62954.js",
+    "file": "remoteEntry.b043c37bb43deb442a61.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCjCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,kMAAkM;WAChO;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC5CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCzKA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;UErFA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://ipyniivue/webpack/container-entry",
         "webpack://ipyniivue/webpack/bootstrap",
         "webpack://ipyniivue/webpack/runtime/define property getters",
@@ -22,20 +22,20 @@
         "webpack://ipyniivue/webpack/after-startup"
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_plugin_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/plugin */ \"./lib/plugin.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\t// no module.id needed\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_widget_js\":\"a86802843924a12afd11\",\"lib_index_js\":\"6ffc91ccc740d1bae4db\",\"lib_plugin_js\":\"4db7aec6cfaa2e3a5663\",\"vendors-node_modules_niivue_niivue_dist_niivue_es_js\":\"2004dca03ee9fd191cd9\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_widget_js\":\"dab26d8704b46bf7fde4\",\"lib_index_js\":\"6ffc91ccc740d1bae4db\",\"lib_plugin_js\":\"4db7aec6cfaa2e3a5663\",\"vendors-node_modules_niivue_niivue_dist_niivue_es_js\":\"2004dca03ee9fd191cd9\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"ipyniivue:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"ipyniivue\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@niivue/niivue\", \"0.33.1\", () => (__webpack_require__.e(\"vendors-node_modules_niivue_niivue_dist_niivue_es_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/@niivue/niivue/dist/niivue.es.js */ \"./node_modules/@niivue/niivue/dist/niivue.es.js\"))))));\n\t\t\tregister(\"ipyniivue\", \"1.0.1\", () => (Promise.all([__webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"ipyniivue\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"@niivue/niivue\", \"0.33.1\", () => (__webpack_require__.e(\"vendors-node_modules_niivue_niivue_dist_niivue_es_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/@niivue/niivue/dist/niivue.es.js */ \"./node_modules/@niivue/niivue/dist/niivue.es.js\"))))));\n\t\t\tregister(\"ipyniivue\", \"1.0.2\", () => (Promise.all([__webpack_require__.e(\"lib_widget_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyter-widgets/base\": () => (loadSingletonVersionCheck(\"default\", \"@jupyter-widgets/base\", [,[1,6],[1,5],[1,4],[1,3],[1,2],[1,1,1,10],1,1,1,1,1])),\n\t\"webpack/sharing/consume/default/@niivue/niivue/@niivue/niivue\": () => (loadStrictVersionCheckFallback(\"default\", \"@niivue/niivue\", [2,0,33,1], () => (__webpack_require__.e(\"vendors-node_modules_niivue_niivue_dist_niivue_es_js\").then(() => (() => (__webpack_require__(/*! @niivue/niivue */ \"./node_modules/@niivue/niivue/dist/niivue.es.js\")))))))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_widget_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyter-widgets/base\",\n\t\t\"webpack/sharing/consume/default/@niivue/niivue/@niivue/niivue\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"ipyniivue\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkipyniivue\"] = self[\"webpackChunkipyniivue\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/ipyniivue\");\n",
         ""
     ],
```

### Comparing `ipyniivue-1.0.1/ipyniivue/labextension/static/vendors-node_modules_niivue_niivue_dist_niivue_es_js.2004dca03ee9fd191cd9.js` & `ipyniivue-1.0.2/ipyniivue/labextension/static/vendors-node_modules_niivue_niivue_dist_niivue_es_js.2004dca03ee9fd191cd9.js`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/ipyniivue/labextension/static/vendors-node_modules_niivue_niivue_dist_niivue_es_js.2004dca03ee9fd191cd9.js.map` & `ipyniivue-1.0.2/ipyniivue/labextension/static/vendors-node_modules_niivue_niivue_dist_niivue_es_js.2004dca03ee9fd191cd9.js.map`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/ipyniivue/nbextension/index.js` & `ipyniivue-1.0.2/ipyniivue/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -55625,15 +55625,15 @@
                 /*!**********************!*\
                   !*** ./package.json ***!
                   \**********************/
                 /***/
                 ((module) => {
 
                     "use strict";
-                    module.exports = JSON.parse('{"name":"ipyniivue","version":"1.0.1","description":"Jupyter-Niivue bridge","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/niivue/ipyniivue","bugs":{"url":"https://github.com/niivue/ipyniivue/issues"},"license":"BSD-3-Clause","author":{"name":"Niivue"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/niivue/ipyniivue"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyniivue/labextension","clean:nbextension":"rimraf ipyniivue/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","@niivue/niivue":"^0.33.1"},"devDependencies":{"@babel/core":"^7.21.4","@babel/preset-env":"^7.21.4","@babel/preset-typescript":"^7.21.4","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","babel-jest":"^29.5.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.6.3","mkdirp":"^0.5.1","npm-run-all":"^4.1.5","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.5.6","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyniivue/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
+                    module.exports = JSON.parse('{"name":"ipyniivue","version":"1.0.2","description":"Jupyter-Niivue bridge","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/niivue/ipyniivue","bugs":{"url":"https://github.com/niivue/ipyniivue/issues"},"license":"BSD-3-Clause","author":{"name":"Niivue"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/niivue/ipyniivue"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyniivue/labextension","clean:nbextension":"rimraf ipyniivue/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","@niivue/niivue":"^0.33.1"},"devDependencies":{"@babel/core":"^7.21.4","@babel/preset-env":"^7.21.4","@babel/preset-typescript":"^7.21.4","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","babel-jest":"^29.5.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.6.3","mkdirp":"^0.5.1","npm-run-all":"^4.1.5","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.5.6","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyniivue/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}');
 
                     /***/
                 })
 
             /******/
         });
         /************************************************************************/
```

### Comparing `ipyniivue-1.0.1/ipyniivue/nbextension/index.js.LICENSE.txt` & `ipyniivue-1.0.2/ipyniivue/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/ipyniivue/nbextension/index.js.map` & `ipyniivue-1.0.2/ipyniivue/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/ipyniivue/tests/conftest.py` & `ipyniivue-1.0.2/ipyniivue/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/src/extension.ts` & `ipyniivue-1.0.2/src/extension.ts`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/src/plugin.ts` & `ipyniivue-1.0.2/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/src/utils.ts` & `ipyniivue-1.0.2/src/utils.ts`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/src/version.ts` & `ipyniivue-1.0.2/src/version.ts`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/src/widget.ts` & `ipyniivue-1.0.2/src/widget.ts`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/src/__tests__/index.spec.ts` & `ipyniivue-1.0.2/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/src/__tests__/utils.ts` & `ipyniivue-1.0.2/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/.gitignore` & `ipyniivue-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/LICENSE.txt` & `ipyniivue-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/README.md` & `ipyniivue-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ipyniivue-1.0.1/pyproject.toml` & `ipyniivue-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.0.0",
     "jupyter_ui_poll>=0.2.2"
 ]
-version = "1.0.1"
+version = "1.0.2"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
@@ -101,13 +101,13 @@
 ]
 file = [
     { src = "pyproject.toml", version_template = "version = \"{major}.{minor}.{patch}{channel}{release}\"" },
     { src = "ipyniivue/_version.py" },
 ]
 
 [tool.tbump.version]
-current = "1.0.1"
+current = "1.0.2"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
```

### Comparing `ipyniivue-1.0.1/PKG-INFO` & `ipyniivue-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyniivue
-Version: 1.0.1
+Version: 1.0.2
 Summary: Jupyter-Niivue bridge
 Project-URL: Homepage, https://github.com/niivue/ipyniivue
 Author: Niivue
 License: Copyright (c) 2023 Niivue
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

