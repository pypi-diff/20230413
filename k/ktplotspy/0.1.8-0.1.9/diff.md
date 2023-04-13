# Comparing `tmp/ktplotspy-0.1.8.tar.gz` & `tmp/ktplotspy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ktplotspy-0.1.8.tar", max compression
+gzip compressed data, was "ktplotspy-0.1.9.tar", max compression
```

## Comparing `ktplotspy-0.1.8.tar` & `ktplotspy-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1063 2023-02-02 11:02:48.465901 ktplotspy-0.1.8/LICENSE
--rw-r--r--   0        0        0     1856 2023-02-02 11:02:48.465901 ktplotspy-0.1.8/README.rst
--rw-r--r--   0        0        0      126 2023-02-02 11:02:48.693899 ktplotspy-0.1.8/ktplotspy/__init__.py
--rw-r--r--   0        0        0      256 2023-02-02 11:02:48.693899 ktplotspy-0.1.8/ktplotspy/plot/__init__.py
--rw-r--r--   0        0        0    15948 2023-02-02 11:02:48.693899 ktplotspy-0.1.8/ktplotspy/plot/plot_cpdb.py
--rw-r--r--   0        0        0    13857 2023-02-02 11:02:48.693899 ktplotspy-0.1.8/ktplotspy/plot/plot_cpdb_chord.py
--rw-r--r--   0        0        0     4962 2023-02-02 11:02:48.693899 ktplotspy-0.1.8/ktplotspy/plot/plot_cpdb_heatmap.py
--rw-r--r--   0        0        0      244 2023-02-02 11:02:48.693899 ktplotspy-0.1.8/ktplotspy/utils/settings.py
--rw-r--r--   0        0        0    22799 2023-02-02 11:02:48.693899 ktplotspy-0.1.8/ktplotspy/utils/support.py
--rw-r--r--   0        0        0     2285 2023-02-02 11:02:48.693899 ktplotspy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3004 1970-01-01 00:00:00.000000 ktplotspy-0.1.8/setup.py
--rw-r--r--   0        0        0     3376 1970-01-01 00:00:00.000000 ktplotspy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-01 22:59:39.033974 ktplotspy-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1856 2023-04-01 22:59:39.033974 ktplotspy-0.1.9/README.rst
+-rw-r--r--   0        0        0      126 2023-04-01 22:59:39.285985 ktplotspy-0.1.9/ktplotspy/__init__.py
+-rw-r--r--   0        0        0      256 2023-04-01 22:59:39.285985 ktplotspy-0.1.9/ktplotspy/plot/__init__.py
+-rw-r--r--   0        0        0    15948 2023-04-01 22:59:39.285985 ktplotspy-0.1.9/ktplotspy/plot/plot_cpdb.py
+-rw-r--r--   0        0        0    13857 2023-04-01 22:59:39.285985 ktplotspy-0.1.9/ktplotspy/plot/plot_cpdb_chord.py
+-rw-r--r--   0        0        0     5039 2023-04-01 22:59:39.285985 ktplotspy-0.1.9/ktplotspy/plot/plot_cpdb_heatmap.py
+-rw-r--r--   0        0        0      244 2023-04-01 22:59:39.285985 ktplotspy-0.1.9/ktplotspy/utils/settings.py
+-rw-r--r--   0        0        0    22799 2023-04-01 22:59:39.285985 ktplotspy-0.1.9/ktplotspy/utils/support.py
+-rw-r--r--   0        0        0     2285 2023-04-01 22:59:39.285985 ktplotspy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3376 1970-01-01 00:00:00.000000 ktplotspy-0.1.9/PKG-INFO
```

### Comparing `ktplotspy-0.1.8/LICENSE` & `ktplotspy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ktplotspy-0.1.8/README.rst` & `ktplotspy-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `ktplotspy-0.1.8/ktplotspy/plot/plot_cpdb.py` & `ktplotspy-0.1.9/ktplotspy/plot/plot_cpdb.py`

 * *Files identical despite different names*

### Comparing `ktplotspy-0.1.8/ktplotspy/plot/plot_cpdb_chord.py` & `ktplotspy-0.1.9/ktplotspy/plot/plot_cpdb_chord.py`

 * *Files identical despite different names*

### Comparing `ktplotspy-0.1.8/ktplotspy/plot/plot_cpdb_heatmap.py` & `ktplotspy-0.1.9/ktplotspy/plot/plot_cpdb_heatmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     col_cluster: bool = True,
     low_col: str = "#104e8b",
     mid_col: str = "#ffdab9",
     high_col: str = "#8b0a50",
     cmap: Optional[Union[str, ListedColormap]] = None,
     title: str = "",
     return_tables: bool = False,
-    symmetrical: bool = False,
+    symmetrical: bool = True,
     **kwargs
 ) -> Union[sns.matrix.ClusterGrid, Dict]:
     """Plot cellphonedb results as total counts of interactions.
 
     Parameters
     ----------
     adata : AnnData
@@ -79,27 +79,28 @@
     all_intr = pvals.copy()
     labels = metadata[celltype_key]
     intr_pairs = all_intr.interacting_pair
     all_int = all_intr.iloc[:, 11 : all_intr.shape[1]].T
     all_int.columns = intr_pairs
     all_count = all_int.melt(ignore_index=False).reset_index()
     if degs_analysis:
-        all_count['significant'] = all_count.value == 1
+        all_count["significant"] = all_count.value == 1
     else:
-        all_count['significant'] = all_count.value < alpha
+        all_count["significant"] = all_count.value < alpha
     count1x = all_count[["index", "significant"]].groupby("index").agg({"significant": "sum"})
     tmp = pd.DataFrame([x.split("|") for x in count1x.index])
     count_final = pd.concat([tmp, count1x.reset_index(drop=True)], axis=1)
     count_final.columns = ["SOURCE", "TARGET", "COUNT"]
     if any(count_final.COUNT > 0):
         count_mat = count_final.pivot_table(index="SOURCE", columns="TARGET", values="COUNT")
         count_mat.columns.name, count_mat.index.name = None, None
         count_mat[pd.isnull(count_mat)] = 0
         if symmetrical:
             count_matx = np.triu(count_mat) + np.tril(count_mat.T) + np.tril(count_mat) + np.triu(count_mat.T)
+            count_matx[np.diag_indices_from(count_matx)] = np.diag(count_mat)
             count_matx = pd.DataFrame(count_matx)
             count_matx.columns = count_mat.columns
             count_matx.index = count_mat.index
             count_mat = count_matx.copy()
             all_sum = pd.DataFrame(count_mat.apply(sum, axis=0), columns=["total_interactions"])
         else:
             all_sum = pd.DataFrame(count_mat.apply(sum, axis=0), columns=["total_interactions"]) + pd.DataFrame(
```

### Comparing `ktplotspy-0.1.8/ktplotspy/utils/support.py` & `ktplotspy-0.1.9/ktplotspy/utils/support.py`

 * *Files identical despite different names*

### Comparing `ktplotspy-0.1.8/pyproject.toml` & `ktplotspy-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ktplotspy"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python library for plotting Cellphonedb results. Ported from ktplots R package."
 authors = ["Kelvin Tuong <26215587+zktuong@users.noreply.github.com>"]
 license = "MIT"
 classifiers = [
     'License :: OSI Approved :: MIT License',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
```

### Comparing `ktplotspy-0.1.8/setup.py` & `ktplotspy-0.1.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,90 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ktplotspy
+Version: 0.1.9
+Summary: Python library for plotting Cellphonedb results. Ported from ktplots R package.
+Home-page: https://github.com/zktuong/ktplotspy
+License: MIT
+Keywords: cellphonedb,cpdb,plot_cpdb,ktplots,ligand-receptor,interaction
+Author: Kelvin Tuong
+Author-email: 26215587+zktuong@users.noreply.github.com
+Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Provides-Extra: docs
+Provides-Extra: test
+Requires-Dist: anndata (>=0.7.6,<0.8.0) ; extra == "test"
+Requires-Dist: black ; extra == "test"
+Requires-Dist: nbsphinx ; extra == "docs"
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: plotnine
+Requires-Dist: pytest-cov ; extra == "test"
+Requires-Dist: python-circos (>=0.3.0,<0.4.0)
+Requires-Dist: readthedocs-sphinx-ext ; extra == "docs"
+Requires-Dist: recommonmark ; extra == "docs"
+Requires-Dist: requests
+Requires-Dist: seaborn
+Requires-Dist: sphinx-autodoc-typehints ; extra == "docs"
+Requires-Dist: sphinx_rtd_theme ; extra == "docs"
+Project-URL: Repository, https://github.com/zktuong/ktplotspy
+Description-Content-Type: text/x-rst
+
+|Docs| |PyPI| |Master| |MasterTest| |CodeCov|
+
+ktplots-*py*
+------------
+
+|logo|
+
+Welcome! This is a super light-weight python library for plotting 
+`CellphoneDB <https://www.github.com/ventolab/CellphoneDB/>`__ results. Ported from 
+`ktplots <https://www.github.com/zktuong/ktplots/>`__ R package. For more options, 
+please check out the original R 
+`package <https://www.github.com/zktuong/ktplots/>`__.
+
+The documentation is
+`here <https://ktplotspy.readthedocs.io/>`__.
+
+Installation
+------------
+
+.. code:: bash
+
+    pip install ktplotspy
+
+
+Support
+-------
+
+Support is provided on a voluntary basis, as time permits.
+
+If there are any ideas, comments, suggestions, thing you would like to
+know more etc., please feel free to email me at z.tuong@uq.edu.au or
+post in the issue tracker and I will get back to you.
+
+Citation
+--------
+
+If you find this useful, please consider citing the github repositories. Also leave a star at the 
+`ktplotspy <https://www.github.com/zktuong/ktplotspy/>`__ and the original
+`ktplots <https://www.github.com/zktuong/ktplots/>`__ repositories!
+
+.. |Docs| image:: https://readthedocs.org/projects/ktplotspy/badge/?version=latest
+   :target: https://ktplotspy.readthedocs.io/en/latest/?badge=latest
+.. |PyPI| image:: https://img.shields.io/pypi/v/ktplotspy?logo=PyPI
+   :target: https://pypi.org/project/ktplotspy/
+.. |Master| image:: https://byob.yarr.is/zktuong/ktplotspy/version
+   :target: https://github.com/zktuong/ktplotspy/tree/master
+.. |MasterTest| image:: https://github.com/zktuong/ktplotspy/workflows/tests/badge.svg?branch=master
+   :target: https://github.com/zktuong/ktplotspy/actions/workflows/tests.yml
+.. |CodeCov| image:: https://codecov.io/gh/zktuong/ktplotspy/branch/master/graph/badge.svg?token=661BMU1FBO
+   :target: https://codecov.io/gh/zktuong/ktplotspy
+.. |logo| image:: docs/notebooks/logo.png
 
-packages = \
-['ktplotspy', 'ktplotspy.plot', 'ktplotspy.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['numpy',
- 'pandas',
- 'plotnine',
- 'python-circos>=0.3.0,<0.4.0',
- 'requests',
- 'seaborn']
-
-extras_require = \
-{'docs': ['nbsphinx',
-          'sphinx-autodoc-typehints',
-          'sphinx_rtd_theme',
-          'readthedocs-sphinx-ext',
-          'recommonmark'],
- 'test': ['anndata>=0.7.6,<0.8.0', 'black', 'pytest-cov']}
-
-setup_kwargs = {
-    'name': 'ktplotspy',
-    'version': '0.1.8',
-    'description': 'Python library for plotting Cellphonedb results. Ported from ktplots R package.',
-    'long_description': '|Docs| |PyPI| |Master| |MasterTest| |CodeCov|\n\nktplots-*py*\n------------\n\n|logo|\n\nWelcome! This is a super light-weight python library for plotting \n`CellphoneDB <https://www.github.com/ventolab/CellphoneDB/>`__ results. Ported from \n`ktplots <https://www.github.com/zktuong/ktplots/>`__ R package. For more options, \nplease check out the original R \n`package <https://www.github.com/zktuong/ktplots/>`__.\n\nThe documentation is\n`here <https://ktplotspy.readthedocs.io/>`__.\n\nInstallation\n------------\n\n.. code:: bash\n\n    pip install ktplotspy\n\n\nSupport\n-------\n\nSupport is provided on a voluntary basis, as time permits.\n\nIf there are any ideas, comments, suggestions, thing you would like to\nknow more etc., please feel free to email me at z.tuong@uq.edu.au or\npost in the issue tracker and I will get back to you.\n\nCitation\n--------\n\nIf you find this useful, please consider citing the github repositories. Also leave a star at the \n`ktplotspy <https://www.github.com/zktuong/ktplotspy/>`__ and the original\n`ktplots <https://www.github.com/zktuong/ktplots/>`__ repositories!\n\n.. |Docs| image:: https://readthedocs.org/projects/ktplotspy/badge/?version=latest\n   :target: https://ktplotspy.readthedocs.io/en/latest/?badge=latest\n.. |PyPI| image:: https://img.shields.io/pypi/v/ktplotspy?logo=PyPI\n   :target: https://pypi.org/project/ktplotspy/\n.. |Master| image:: https://byob.yarr.is/zktuong/ktplotspy/version\n   :target: https://github.com/zktuong/ktplotspy/tree/master\n.. |MasterTest| image:: https://github.com/zktuong/ktplotspy/workflows/tests/badge.svg?branch=master\n   :target: https://github.com/zktuong/ktplotspy/actions/workflows/tests.yml\n.. |CodeCov| image:: https://codecov.io/gh/zktuong/ktplotspy/branch/master/graph/badge.svg?token=661BMU1FBO\n   :target: https://codecov.io/gh/zktuong/ktplotspy\n.. |logo| image:: docs/notebooks/logo.png\n',
-    'author': 'Kelvin Tuong',
-    'author_email': '26215587+zktuong@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/zktuong/ktplotspy',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

