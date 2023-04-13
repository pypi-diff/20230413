# Comparing `tmp/spectrochempy-0.5.5.tar.gz` & `tmp/spectrochempy-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrochempy-0.5.5.tar", last modified: Wed Mar 22 08:57:51 2023, max compression
+gzip compressed data, was "spectrochempy-0.6.1.tar", last modified: Thu Apr 13 09:17:25 2023, max compression
```

## Comparing `spectrochempy-0.5.5.tar` & `spectrochempy-0.6.1.tar`

### file list

```diff
@@ -1,215 +1,226 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.676251 spectrochempy-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/.codespellrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.636251 spectrochempy-0.5.5/.conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/.conda/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.636251 spectrochempy-0.5.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/LICENSES/NMRGLUE_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/LICENSES/NNMF_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/LICENSES/PACKAGING_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/LICENSES/PANDAS_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/LICENSES/TRAITTYPES_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-03-22 08:57:51.676251 spectrochempy-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-03-22 08:57:28.000000 spectrochempy-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/environment_dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.636251 spectrochempy-0.5.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/requirements/requirements_dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.636251 spectrochempy-0.5.5/scp_data/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.636251 spectrochempy-0.5.5/scp_data/databases/
--rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/databases/isotopes.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.648251 spectrochempy-0.5.5/scp_data/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    38040 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/Felipa-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/Humor-Sans.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/LICENSE_felipa.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/LICENSE_victormono.txt
--rw-r--r--   0 runner    (1001) docker     (123)   157048 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   164392 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-BoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150324 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   184764 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156852 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-ExtraLightOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188172 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150888 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188268 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   157596 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-LightOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   153808 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   194336 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-MediumOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158228 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   151576 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   193176 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161200 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-SemiBoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150284 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188288 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   157184 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/VictorMono-ThinOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105316 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/fonts/comic-sans-ms.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.648251 spectrochempy-0.5.5/scp_data/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/stylesheets/grayscale.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/stylesheets/notebook.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/stylesheets/paper.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/stylesheets/poster.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/stylesheets/sans.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/stylesheets/scpy.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/stylesheets/serif.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scp_data/stylesheets/talk.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.648251 spectrochempy-0.5.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scripts/checkindex.py
--rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/scripts/validate_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-22 08:57:51.680251 spectrochempy-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.652251 spectrochempy-0.5.5/spectrochempy/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.656251 spectrochempy-0.5.5/spectrochempy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/analysis/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34330 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/analysis/cantera_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/analysis/efa.py
--rw-r--r--   0 runner    (1001) docker     (123)    42371 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/analysis/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    29252 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/analysis/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/analysis/lstsq.py
--rw-r--r--   0 runner    (1001) docker     (123)    28967 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/analysis/mcrals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10008 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/analysis/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/analysis/nnmf.py
--rw-r--r--   0 runner    (1001) docker     (123)    20551 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/analysis/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    13066 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/analysis/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)    19206 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/analysis/simplisma.py
--rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/analysis/svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    48310 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.656251 spectrochempy-0.5.5/spectrochempy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.656251 spectrochempy-0.5.5/spectrochempy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/common/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.656251 spectrochempy-0.5.5/spectrochempy/core/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/dataset/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.660251 spectrochempy-0.5.5/spectrochempy/core/dataset/arraymixins/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/dataset/arraymixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15832 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/dataset/arraymixins/ndio.py
--rw-r--r--   0 runner    (1001) docker     (123)   120698 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/dataset/arraymixins/ndmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/dataset/arraymixins/ndplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/dataset/arraymixins/npy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.660251 spectrochempy-0.5.5/spectrochempy/core/dataset/baseobjects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/dataset/baseobjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/dataset/baseobjects/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    73888 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/dataset/baseobjects/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    22749 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/dataset/baseobjects/ndcomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)    34088 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/dataset/coord.py
--rw-r--r--   0 runner    (1001) docker     (123)    37941 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/dataset/coordset.py
--rw-r--r--   0 runner    (1001) docker     (123)    53690 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/dataset/nddataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.660251 spectrochempy-0.5.5/spectrochempy/core/plotters/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/plotters/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/plotters/multiplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    19749 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/plotters/plot1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    26288 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/plotters/plot2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/plotters/plot3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    19058 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/plotters/plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.664251 spectrochempy-0.5.5/spectrochempy/core/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/align.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24457 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/autosub.py
--rw-r--r--   0 runner    (1001) docker     (123)    28343 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19447 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/phasing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/processors/zero_filling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.664251 spectrochempy-0.5.5/spectrochempy/core/project/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/project/abstractproject.py
--rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/project/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.668251 spectrochempy-0.5.5/spectrochempy/core/readers/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    25752 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/read_carroucell.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/read_jcamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/read_labspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/read_matlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    49920 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/read_omnic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/read_opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/read_quadera.py
--rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/read_soc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19504 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/read_spc.py
--rw-r--r--   0 runner    (1001) docker     (123)    48102 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/read_topspin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/readers/read_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.668251 spectrochempy-0.5.5/spectrochempy/core/script/
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.668251 spectrochempy-0.5.5/spectrochempy/core/units/
--rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.672251 spectrochempy-0.5.5/spectrochempy/core/writers/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/writers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/writers/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/writers/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/writers/write_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/writers/write_jcamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/core/writers/write_matlab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.672251 spectrochempy-0.5.5/spectrochempy/extern/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64431 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/extern/nmrglue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/extern/traittypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/extern/traittypes_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.672251 spectrochempy-0.5.5/spectrochempy/ipython/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/ipython/magics.py
--rw-r--r--   0 runner    (1001) docker     (123)    47047 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/plot_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.676251 spectrochempy-0.5.5/spectrochempy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/citation.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/coordrange.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14071 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/jsonutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/optional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/orderedset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    16784 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/print.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    34449 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.676251 spectrochempy-0.5.5/spectrochempy/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/widgets/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/widgets/baselinecorrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-03-22 08:57:29.000000 spectrochempy-0.5.5/spectrochempy/widgets/fileselector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 08:57:51.652251 spectrochempy-0.5.5/spectrochempy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-03-22 08:57:51.000000 spectrochempy-0.5.5/spectrochempy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-03-22 08:57:51.000000 spectrochempy-0.5.5/spectrochempy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 08:57:51.000000 spectrochempy-0.5.5/spectrochempy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 08:57:51.000000 spectrochempy-0.5.5/spectrochempy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-22 08:57:51.000000 spectrochempy-0.5.5/spectrochempy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-22 08:57:51.000000 spectrochempy-0.5.5/spectrochempy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.561840 spectrochempy-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/.codespellrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.513840 spectrochempy-0.6.1/.conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/.conda/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.513840 spectrochempy-0.6.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/LICENSES/NMRGLUE_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/LICENSES/NNMF_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/LICENSES/PACKAGING_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/LICENSES/PANDAS_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/LICENSES/TRAITTYPES_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-13 09:17:25.561840 spectrochempy-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/environment_dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.513840 spectrochempy-0.6.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/requirements/requirements_dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.513840 spectrochempy-0.6.1/scp_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.513840 spectrochempy-0.6.1/scp_data/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/databases/isotopes.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.525840 spectrochempy-0.6.1/scp_data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    38040 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/Felipa-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/Humor-Sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/LICENSE_felipa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/LICENSE_victormono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   157048 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   164392 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-BoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150324 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   184764 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156852 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-ExtraLightOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188172 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150888 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188268 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   157596 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-LightOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   153808 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   194336 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-MediumOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158228 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   151576 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   193176 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161200 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-SemiBoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150284 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188288 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   157184 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-ThinOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105316 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/comic-sans-ms.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.525840 spectrochempy-0.6.1/scp_data/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/grayscale.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/notebook.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/paper.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/poster.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/sans.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/scpy.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/serif.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/talk.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.525840 spectrochempy-0.6.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scripts/checkindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scripts/validate_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-13 09:17:25.561840 spectrochempy-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.525840 spectrochempy-0.6.1/spectrochempy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.533840 spectrochempy-0.6.1/spectrochempy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52625 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/efa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35689 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/kinetic_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/linearregression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43620 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/mcrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/nnmf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.533840 spectrochempy-0.6.1/spectrochempy/analysis/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/optimize/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9988 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/optimize/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/optimize/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36844 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/optimize/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22702 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/simplisma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.533840 spectrochempy-0.6.1/spectrochempy/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43480 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/application/general_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/application/metaconfigurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47047 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/application/plot_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.533840 spectrochempy-0.6.1/spectrochempy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.533840 spectrochempy-0.6.1/spectrochempy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/common/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.537840 spectrochempy-0.6.1/spectrochempy/core/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.537840 spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/ndio.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120723 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/ndmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27693 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/ndplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/npy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.537840 spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74573 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/ndcomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34168 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37998 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/coordset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53899 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/nddataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.541840 spectrochempy-0.6.1/spectrochempy/core/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/plotters/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/plotters/multiplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/plotters/plot1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26279 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/plotters/plot2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/plotters/plot3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/plotters/plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.541840 spectrochempy-0.6.1/spectrochempy/core/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/autosub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28435 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19449 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/phasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/zero_filling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.541840 spectrochempy-0.6.1/spectrochempy/core/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/project/abstractproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18331 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/project/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.549840 spectrochempy-0.6.1/spectrochempy/core/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26561 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_carroucell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_jcamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_labspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_matlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50613 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_omnic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_quadera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_soc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19509 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_spc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48164 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_topspin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.549840 spectrochempy-0.6.1/spectrochempy/core/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.549840 spectrochempy-0.6.1/spectrochempy/core/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.549840 spectrochempy-0.6.1/spectrochempy/core/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/writers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/writers/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/writers/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/writers/write_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/writers/write_jcamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/writers/write_matlab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.553840 spectrochempy-0.6.1/spectrochempy/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64415 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/extern/nmrglue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/extern/traittypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/extern/traittypes_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.553840 spectrochempy-0.6.1/spectrochempy/ipython/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/ipython/magics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.557840 spectrochempy-0.6.1/spectrochempy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/citation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/coordrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14176 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23056 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/jsonutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/print.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33935 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.557840 spectrochempy-0.6.1/spectrochempy/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/widgets/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/widgets/baselinecorrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/widgets/fileselector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.529840 spectrochempy-0.6.1/spectrochempy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-13 09:17:25.000000 spectrochempy-0.6.1/spectrochempy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-13 09:17:25.000000 spectrochempy-0.6.1/spectrochempy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:17:25.000000 spectrochempy-0.6.1/spectrochempy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:17:25.000000 spectrochempy-0.6.1/spectrochempy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 09:17:25.000000 spectrochempy-0.6.1/spectrochempy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 09:17:25.000000 spectrochempy-0.6.1/spectrochempy.egg-info/top_level.txt
```

### Comparing `spectrochempy-0.5.5/.codeclimate.yml` & `spectrochempy-0.6.1/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/.conda/meta.yaml` & `spectrochempy-0.6.1/.conda/meta.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   script:
     - export SETUPTOOLS_SCM_PRETEND_VERSION={{ version }}
     - {{ PYTHON }} -m pip install .
 
 requirements:
   host:
     - pip
-    - python >=3.7
+    - python >=3.8
     - setuptools
     - setuptools_scm
   run:
     - python
 
     # specific dependencies
     - quadprog
```

### Comparing `spectrochempy-0.5.5/.gitignore` & `spectrochempy-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/.pre-commit-config.yaml` & `spectrochempy-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/.pylintrc` & `spectrochempy-0.6.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/.zenodo.json` & `spectrochempy-0.6.1/.zenodo.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'publication_date'": "'2023-04-13'", "'version'": "'0.6.1'"}*

```diff
@@ -50,12 +50,12 @@
         "raman",
         "raman-spectra",
         "raman-spectroscopy",
         "spectroscopy",
         "uv-vis"
     ],
     "license": "CECILL-B",
-    "publication_date": "2023-03-22",
+    "publication_date": "2023-04-13",
     "title": "SpectroChemPy",
     "upload_type": "software",
-    "version": "0.5.5"
+    "version": "0.6.1"
 }
```

### Comparing `spectrochempy-0.5.5/CITATION.cff` & `spectrochempy-0.6.1/CITATION.cff`

 * *Files 22% similar despite different names*

```diff
@@ -11,20 +11,20 @@
   orcid: https://orcid.org/0000-0002-9579-8910
 - affiliation: "ENSICAEN, Universit\xE9 de Caen, CNRS (Laboratoire Catalyse et Spectrochimie)"
   email: christian.fernandez@ensicaen.fr
   family-names: Fernandez
   given-names: Christian
   orcid: https://orcid.org/0000-0002-5476-3148
 cff-version: 1.2.0
-date-released: '2023-03-22'
+date-released: '2023-04-13'
 identifiers:
 - description: Persistent identifier for all versions of SpectroChemPy
   type: doi
   value: 10.5281/zenodo.3823841
 license: CECILL-B
 message: If you use this software, please cite it using the metadata from this file.
 repository-code: https://github.com/spectrochempy/spectrochempy
 title: SpectroChemPy, a framework for processing, analyzing and modeling spectroscopic
   data for chemistry with Python
 type: software
 url: https://www.spectrochempy.fr
-version: 0.5.5
+version: 0.6.1
```

### Comparing `spectrochempy-0.5.5/Dockerfile` & `spectrochempy-0.6.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/LICENSE` & `spectrochempy-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/LICENSES/NMRGLUE_LICENSE.rst` & `spectrochempy-0.6.1/LICENSES/NMRGLUE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/LICENSES/NNMF_LICENSE.rst` & `spectrochempy-0.6.1/LICENSES/NNMF_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/LICENSES/PACKAGING_LICENSE.rst` & `spectrochempy-0.6.1/LICENSES/PACKAGING_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/LICENSES/PANDAS_LICENSE.rst` & `spectrochempy-0.6.1/LICENSES/PANDAS_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/LICENSES/TRAITTYPES_LICENSE.rst` & `spectrochempy-0.6.1/LICENSES/TRAITTYPES_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/PKG-INFO` & `spectrochempy-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrochempy
-Version: 0.5.5
+Version: 0.6.1
 Summary: Processing, analysis and modelling Spectroscopic data for Chemistry with Python
 Home-page: https://www.spectrochempy.fr
 Author: Arnaud Travert & Christian Fernandez
 Author-email: contact@spectrochempy.fr
 Maintainer: C. Fernandez
 Maintainer-email: christian.fernandez@ensicaen.fr
 License: CECILL-B
@@ -14,18 +14,18 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align ="center">
 <img src='https://github.com/spectrochempy/spectrochempy/raw/master/docs/_static/scpy.png' width="150">
 <br>
 SpectroChemPy
```

### Comparing `spectrochempy-0.5.5/README.md` & `spectrochempy-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/environment.yml` & `spectrochempy-0.6.1/environment.yml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/environment_dev.yml` & `spectrochempy-0.6.1/environment_dev.yml`

 * *Files 11% similar despite different names*

```diff
@@ -80,13 +80,14 @@
     - sphinx_rtd_theme=1.1
     - autodocsumm
     - sphinx-gallery
     - nbsphinx
     - jupyter_sphinx
     - json5
     - sphinx-copybutton
-    - pandoc
+    - sphinxcontrib-bibtex
+    - pandoc=2.19
     - conda-build
     - conda-verify
     - anaconda-client
 
 #EOF
```

### Comparing `spectrochempy-0.5.5/requirements/requirements.txt` & `spectrochempy-0.6.1/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/requirements/requirements_dev.txt` & `spectrochempy-0.6.1/requirements/requirements_dev.txt`

 * *Files 14% similar despite different names*

```diff
@@ -55,8 +55,9 @@
 sphinx_rtd_theme==1.1
 autodocsumm
 sphinx-gallery
 nbsphinx
 jupyter_sphinx
 json5
 sphinx-copybutton
-pandoc
+sphinxcontrib-bibtex
+pandoc==2.19
```

### Comparing `spectrochempy-0.5.5/scp_data/databases/isotopes.csv` & `spectrochempy-0.6.1/scp_data/databases/isotopes.csv`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/Felipa-Regular.ttf` & `spectrochempy-0.6.1/scp_data/fonts/Felipa-Regular.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/Humor-Sans.ttf` & `spectrochempy-0.6.1/scp_data/fonts/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/LICENSE_felipa.txt` & `spectrochempy-0.6.1/scp_data/fonts/LICENSE_felipa.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/LICENSE_victormono.txt` & `spectrochempy-0.6.1/scp_data/fonts/LICENSE_victormono.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-Bold.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-BoldItalic.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-BoldOblique.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-ExtraLight.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-ExtraLightItalic.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-ExtraLightOblique.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-ExtraLightOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-Italic.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-Light.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-LightItalic.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-LightOblique.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-LightOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-Medium.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-MediumItalic.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-MediumOblique.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-MediumOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-Oblique.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-Regular.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-SemiBold.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-SemiBoldItalic.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-SemiBoldOblique.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-SemiBoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-Thin.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-ThinItalic.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/VictorMono-ThinOblique.ttf` & `spectrochempy-0.6.1/scp_data/fonts/VictorMono-ThinOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/fonts/comic-sans-ms.ttf` & `spectrochempy-0.6.1/scp_data/fonts/comic-sans-ms.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/stylesheets/grayscale.mplstyle` & `spectrochempy-0.6.1/scp_data/stylesheets/grayscale.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/stylesheets/notebook.mplstyle` & `spectrochempy-0.6.1/scp_data/stylesheets/notebook.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/stylesheets/sans.mplstyle` & `spectrochempy-0.6.1/scp_data/stylesheets/sans.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/stylesheets/scpy.mplstyle` & `spectrochempy-0.6.1/scp_data/stylesheets/scpy.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scp_data/stylesheets/serif.mplstyle` & `spectrochempy-0.6.1/scp_data/stylesheets/serif.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scripts/checkindex.py` & `spectrochempy-0.6.1/scripts/checkindex.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/scripts/validate_docstrings.py` & `spectrochempy-0.6.1/scripts/validate_docstrings.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     Parameters
     ----------
     func_name : str
         Name of the object of the docstring to validate.
 
     Returns
     -------
-    dict
+    `dict`
         Information about the docstring and the errors found.
     """
     func_obj = Validator._load_obj(func_name)
     # Some objects are instances, e.g. IndexSlice, which numpydoc can't validate
     doc_obj = get_doc_object(func_obj, doc=func_obj.__doc__)
     doc = spectrochempyDocstring(func_name, doc_obj)
     result = validate(doc_obj)
@@ -299,27 +299,30 @@
         If provided, only the docstrings that start with this pattern will be
         validated. If None, all docstrings will be validated.
     ignore_deprecated: bool, default False
         If True, deprecated objects are ignored when validating docstrings.
 
     Returns
     -------
-    dict
+    `dict`
         A dictionary with an item for every function/method... containing
         all the validation information.
     """
     result = {}
     seen = {}
 
     base_path = pathlib.Path(__file__).parent.parent
-    api_doc_fnames = pathlib.Path(base_path, "docs", "userguide", "reference")
+    api_doc_fnames = pathlib.Path(base_path, "docs", "reference")
     api_items = []
     for api_doc_fname in api_doc_fnames.glob("*.rst"):
         with open(api_doc_fname) as f:
-            api_items += list(get_api_items(f))
+            try:
+                api_items += list(get_api_items(f))
+            except AttributeError:
+                continue
 
     for func_name, _, section, subsection in api_items:
         if prefix and not func_name.startswith(prefix):
             continue
         doc_info = spectrochempy_validate(func_name)
         if ignore_deprecated and doc_info["deprecated"]:
             continue
@@ -413,15 +416,15 @@
         print_validate_one_results(func_name)
         return 0
 
 
 if __name__ == "__main__":
     format_opts = "default", "json", "actions"
     func_help = (
-        "function or method to validate (e.g. spectrochempy.DataFrame.head) "
+        "function or method to validate (e.g. spectrochempy.NDDataset.read) "
         "if not provided, all docstrings are validated and returned "
         "as JSON"
     )
     argparser = argparse.ArgumentParser(description="validate spectrochempy docstrings")
     argparser.add_argument("function", nargs="?", default=None, help=func_help)
     argparser.add_argument(
         "--format",
```

### Comparing `spectrochempy-0.5.5/setup.cfg` & `spectrochempy-0.6.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,25 @@
 	N802,
 	N803,
 	N805,
 	N806,
 	N812,
 	N815,
 	N816
+rst-roles = 
+	class,
+	meth,
+	func,
+	ref,
+	term,
+	attr,
+	const,
+	cite:t
+rst-directives = 
+	plot
 per-file-ignores = 
 	docs/**/*.py:E501
 max-line-length = 88
 max-complexity = 100
 select = 
 	C,
 	E,
```

### Comparing `spectrochempy-0.5.5/setup.py` & `spectrochempy-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,24 +138,24 @@
         "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
         "Topic :: Scientific/Engineering",
         "Topic :: Software Development :: Libraries",
         "Intended Audience :: Science/Research",
         "License :: CeCILL-B Free Software License Agreement (CECILL-B)",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     platforms=["Windows", "Mac OS X", "Linux"],
     # packages discovery
     zip_safe=False,
     packages=find_packages() + packages,
     include_package_data=True,  # requirements
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     setup_requires=["setuptools_scm>=6.3.2", "matplotlib>=3.5.1"],
     install_requires=read_requirements(),
     # post-commands
     cmdclass={
         "develop": PostDevelopCommand,
         "install": PostInstallCommand,
     },
```

### Comparing `spectrochempy-0.5.5/spectrochempy/__init__.py` & `spectrochempy-0.6.1/spectrochempy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,33 +46,32 @@
 SpectroChemPy is a framework for processing, analyzing and modeling Spectroscopic data
 for Chemistry with Python.
 It is a cross-platform software, running on Linux, Windows or OS X.
 """
 
 import warnings
 
+import numpy as np
+
 # warnings.filterwarnings(action="error", category=DeprecationWarning)
-# warnings.filterwarnings(action="ignore", module="matplotlib")  # , category=UserWarning)
 warnings.filterwarnings(
     action="once", module="spectrochempy", category=DeprecationWarning
 )
-import numpy as np
 
 warnings.filterwarnings(
     action="error", module="spectrochempy", category=np.VisibleDeprecationWarning
 )
 
 warnings.filterwarnings(action="ignore", module="jupyter")  # , category=UserWarning)
 warnings.filterwarnings(action="ignore", module="pykwalify")  # , category=UserWarning)
-warnings.filterwarnings(
-    action="error", category=FutureWarning
-)  # , category=UserWarning)
+warnings.filterwarnings(action="ignore", module="matplotlib")
+warnings.filterwarnings(action="ignore", category=FutureWarning)
 
 from spectrochempy import api
-from spectrochempy.api import *  # noqa: F401
+from spectrochempy.api import *
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.dataset.coordset import CoordSet
 from spectrochempy.core.dataset.nddataset import NDDataset
 
 __all__ = api.__all__
```

### Comparing `spectrochempy-0.5.5/spectrochempy/analysis/fitting.py` & `spectrochempy-0.6.1/spectrochempy/analysis/optimize/optimize.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,395 +1,315 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
-"""
-Module to perform fitting of 1D or n-D spectral data.
-"""
-__all__ = ["Fit", "FitParameters", "ParameterScript"]
 
-__dataset_methods__ = []
+__all__ = ["Optimize"]
+__configurables__ = __all__
 
 import re
 import sys
-from collections import UserDict
-from warnings import warn
 
 import numpy as np
 import scipy.optimize
+import traitlets as tr
 from IPython import display
-from traitlets import Any, Bool, HasTraits, Instance, List, Unicode, observe
 
-from spectrochempy.analysis import models as models_
-from spectrochempy.core import INFO, info_, preferences, warning_
-from spectrochempy.utils.docstrings import htmldoc
+from spectrochempy.analysis._base import DecompositionAnalysis
+from spectrochempy.analysis.optimize import _models as models_
+from spectrochempy.analysis.optimize._parameters import FitParameters
+from spectrochempy.application import info_, warning_
+from spectrochempy.extern.traittypes import Array
+from spectrochempy.utils.decorators import signature_has_configurable_traits
+from spectrochempy.utils.docstrings import _docstring
 
 
 # ======================================================================================
-def getmodel(x, y=None, modelname=None, par=None, **kargs):
-    """
-    Get the model for a given x vector.
-
-    Parameters
-    -----------
-    x : ndarray
-        Array of frequency where to evaluate the model values returned by the
-        f function.
-    y : ndarray or None
-        None for 1D, or index for the second dimension.
-    modelname : str
-        Name of the model class to use.
-    par : :class:`Parameters` instance
-        Parameter to pass to the f function.
-    kargs : any
-        Keywords arguments to pass to the f function.
-
-    Returns
-    -------
-    ndarray : float
-        An array containing the calculated model.
-    """
-    model = par.model[modelname]
-    modelcls = getattr(models_, model)
-
-    # take an instance of the model
-    a = modelcls()
-
-    # get the parameters for the given model
-    args = []
-    for p in a.args:
-        try:
-            args.append(par[f"{p}_{modelname}"])
-        except KeyError as e:
-            if p.startswith("c_"):
-                # probably the end of the list
-                # due to a limited polynomial degree
-                pass
-            else:
-                raise ValueError(e)
-
-    x = np.array(x, dtype=np.float64)
-    if y is not None:
-        y = np.array(y, dtype=np.float64)
+@signature_has_configurable_traits
+class Optimize(DecompositionAnalysis):
+    __doc__ = _docstring.dedent(
+        """
+    Non-linear Least-Square Optimization and Curve-Fitting.
 
-    if y is None:
-        return a.f(x, *args, **kargs)
-    else:
-        return a.f(x, y, *args, **kargs)
+    Works on a 1D or 2D dataset.
 
+    # TODO: complete this description
 
-# =============================================================================
-class FitParameters(UserDict):
-    """
-    Allow passing a dictionary of parameters with additional properties
-    to the fit function. Check if the parameter is between the specified bounds
-    if any.
+    Parameters
+    ----------
+    %(AnalysisConfigurable.parameters)s
     """
+    )
 
-    # ----------------------------------------------------------------------------------
-    def __init__(self):
-        UserDict.__init__(self)  # Create a dictionary class
-        self.lob = {}  # Lower bound
-        self.upb = {}  # Upper bound
-        self.fixed = {}  # true for non-variable parameter
-        self.reference = {}  #
-        self.common = {}  # indicates if a parameters belong to a common block
-        self.model = {}  # model to use
-        self.models = []  # list of models
-        self.sequence = ""  # sequence used in the experiment
-        self.expvars = []  # list of parameters which are experiment dependent
-        self.expnumber = 1  # number of experiments
+    name = "Optimize"
+    description = "Non-linear Least-Squares Optimization"
 
     # ----------------------------------------------------------------------------------
-    def __setitem__(self, key, value):
-        key = str(key)
-        if key not in self.reference:
-            self.reference[key] = False
-        if self.reference[key]:
-            # we get a reference to another parameter
-            self.data[key] = str(value)
-            self.fixed[key] = True
-        elif isinstance(value, tuple) or isinstance(value, list):
-            self.data[key] = self._evaluate(value[0])
-            self.lob[key] = None
-            self.upb[key] = None
-            try:
-                if len(value) > 2:
-                    self.lob[key] = self._evaluate(value[1])
-                    self.upb[key] = self._evaluate(value[2])
-                    self._checkerror(key)
-            except Exception:
-                pass
-            self.fixed[key] = False
-            if isinstance(value[-1], bool):
-                self.fixed[key] = value[-1]
-        else:
-            self.data[key] = self._evaluate(value)
-            self.lob[key] = None
-            self.upb[key] = None
-            self.fixed[key] = False
-
+    # Configuration parameters (mostly defined in subclass
+    # as they depend on the model estimator)
     # ----------------------------------------------------------------------------------
-    def __getitem__(self, key):
-        key = str(key)
-        if key in self.data:
-            return self.data[key]
-        raise KeyError(f"parameter `{key}` is not found")
+    max_iter = tr.Integer(
+        default_value=500, help="Maximum number of fitting iteration."
+    ).tag(config=True)
+
+    max_fun_calls = tr.Integer(
+        allow_none=True, help="Maximum number of function calls at each iteration."
+    ).tag(config=True)
+
+    callback_every = tr.Integer(
+        default_value=10,
+        help="Number of iteration between each callback report. "
+        "Used for printing or display intermediate results.",
+    ).tag(config=True)
+
+    method = tr.CaselessStrEnum(
+        ["SIMPLEX", "HOPPING"], default_value="SIMPLEX", help="Optimization method."
+    ).tag(config=True)
+
+    script = tr.Unicode(help="Script defining models and parameters for fitting.").tag(
+        config=True
+    )
+
+    constraints = tr.Any(allow_none=True, help="Constraints.").tag(
+        config=True
+    )  # TODO: adjust this
+
+    dry = tr.Bool(
+        default_value=False,
+        help="If True perform a dry run. "
+        "Mainly used to check the validity of the input parameters.",
+    ).tag(config=True)
+
+    autobase = tr.Bool(
+        default_value=False, help="Whether to apply an automatic baseline correction."
+    ).tag(config=True)
+
+    autoampl = tr.Bool(
+        default_value=False, help="Whether to apply an automatic amplitude correction."
+    ).tag(config=True)
+
+    amplitude_mode = tr.CaselessStrEnum(
+        ["area", "height"],
+        default_value="height",
+        help="Initial amplitude setting mode.",
+    ).tag(config=True)
 
     # ----------------------------------------------------------------------------------
-    def iteritems(self):
-        return iter(self.data.items())
-
+    # Runtime Parameters (in addition to those of AnalysisConfigurable)
     # ----------------------------------------------------------------------------------
-    def _checkerror(self, key):
-        key = str(key)
-        if self.lob[key] is None and self.upb[key] is None:
-            return False
-        elif (self.lob[key] is not None and self.data[key] < self.lob[key]) or (
-            self.upb[key] is not None and self.data[key] > self.upb[key]
-        ):
-            raise ValueError(f"`{key}` value ({self.data[key]}) is out of bounds")
+    fp = tr.Instance(FitParameters, allow_none=True)
+    modeldata = tr.List(Array())
 
     # ----------------------------------------------------------------------------------
-    def __str__(self):
-        def makestr(key):
-
-            keystring = key.split("_")[0]
-            if self.reference[key]:
-                return f"\t> {keystring}:{self.data[key]}\n"
-            else:
-                if self.fixed[key]:
-                    keystring = f"\t* {keystring}"
-                else:
-                    keystring = f"\t$ {keystring}"
-                lob = self.lob[key]
-                upb = self.upb[key]
-                if lob <= -0.1 / sys.float_info.epsilon:
-                    lob = "none"
-                if upb >= +0.1 / sys.float_info.epsilon:
-                    upb = "none"
-                val = str(self.data[key])
-
-                return f"{keystring}: {float(val):10.4f}, {lob}, {upb}\n"
-
-        message = "#PARAMETER SCRIPT\n\nCOMMON:\n"
-
-        var = ""
-        for item in self.expvars:
-            var += f" {item}"
-
-        if var:
-            message += f"\texperiment_number: {self.expnumber}\n"
-            message += f"\texperiment_variables: {var}\n"
-
-        # look for common parameters
-        for key in list(self.keys()):
-            keysp = key.split("_")[0]
-            if self.common[keysp]:
-                message += makestr(key)
-
-        # model parameters
-        models = self.models
-        for model in models:
-            message += f"\nMODEL: {model}\n"
-            message += f"shape: {self.model[model]}\n"
-            for key in sorted(self.keys()):
-                keyspl = key.split("_")
-                if model not in "_".join(keyspl[1:]):
-                    continue
-                message += makestr(key)
-        return message
-
+    # Initialization
     # ----------------------------------------------------------------------------------
-    @staticmethod
-    def _evaluate(strg):
-        """
-        Allow the evaluation of strings containing some operations
-
-        Parameters
-        ----------
-        strg : string
-            A string to evaluate containing multiplier,
-            e.g., '10 k' evaluate to 10 000.
-
-        Return
-        ------
-        value : float or bool
-            Value of the string, or False, if there is an error
-        """
-        res = False
-
-        if isinstance(strg, str):
-            # strg=string.upper(strg)
-            p = re.compile(r"\s+")
-            m = p.split(strg.strip())
-
-            for i in range(len(m)):
-                try:
-                    res = eval(m[i])
-                except NameError:
-                    message = f"Cannot evaluate '{strg}' >> {m[i]} is not defined"
-                    raise NameError(message)
-                except SyntaxError:
-                    message = f"Syntax error in '{strg}'"
-                    raise SyntaxError(message)
-        else:
-            # not a string (probably a scalar that can be return as it is)
-            res = strg
-
-        return res
+    def __init__(
+        self,
+        *,
+        log_level="WARNING",
+        warm_start=False,
+        copy=True,
+        **kwargs,
+    ):
+        """ """
+        # An empty __doc__ must be placed here, else Configurable.__doc__ will appear
+
+        # call the super class for initialisation of the configuration parameters
+        # to do before anything else!
+        super().__init__(
+            log_level=log_level,
+            warm_start=warm_start,
+            copy=copy,
+            **kwargs,
+        )
 
     # ----------------------------------------------------------------------------------
-    def to_internal(self, key, expi=None):
-        """
-        If expi is not none, several parameters to create.
-        """
-        key = str(key)
-        if key not in self.data:
-            raise KeyError(f"parameter `{key}` is not found")
-
-        if expi is not None:
-            pe = self.data[key][expi]
-        else:
-            pe = self.data[key]
-        lob = self.lob[key]
-        upb = self.upb[key]
-
-        is_lob = (
-            lob is not None and lob > -0.1 / sys.float_info.epsilon
-        )  # lob is not None
-        is_upb = (
-            lob is not None and upb < +0.1 / sys.float_info.epsilon
-        )  # upb is not None
-
-        if is_lob and is_upb:
-            lob = min(pe, lob)
-            upb = max(pe, upb)
-            # With min and max bounds defined
-            pi = np.arcsin((2 * (pe - lob) / (upb - lob)) - 1.0)
-        elif is_upb:
-            upb = max(pe, upb)
-            # With only max defined
-            pi = np.sqrt((upb - pe + 1.0) ** 2 - 1.0)
-        elif is_lob:
-            lob = min(pe, lob)
-            # With only min defined
-            pi = np.sqrt((pe - lob + 1.0) ** 2 - 1.0)
-        else:
-            pi = pe
-        return pi
-
+    # Private methods ( overriding abstract methods)
     # ----------------------------------------------------------------------------------
-    def to_external(self, key, pi):
+    def _fit(self, X, Y=None):
 
-        key = str(key)
-        if key not in self.data:
-            raise KeyError(f"parameter `{key}` is not found")
-
-        lob = self.lob[key]
-        upb = self.upb[key]
-
-        is_lob = (
-            lob is not None and lob > -0.1 / sys.float_info.epsilon
-        )  # lob is not None
-        is_upb = (
-            lob is not None and upb < +0.1 / sys.float_info.epsilon
-        )  # upb is not None
-
-        if not isinstance(pi, list):
-            pi = [
-                pi,
-            ]  # make a list
-
-        pe = []
-        for item in pi:
-            if is_lob and is_upb:
-                #  With min and max bounds defined
-                pei = lob + ((upb - lob) / 2.0) * (np.sin(item) + 1.0)
-            elif is_upb:
-                # With only max defined
-                pei = upb + 1.0 - np.sqrt(item**2 + 1.0)
-            elif is_lob:
-                # With only min defined
-                pei = lob - 1.0 + np.sqrt(item**2 + 1.0)
-            else:
-                pei = pi
-            pe.append(pei)
+        # NMR
+        # sequence = kargs.get('sequence', 'ideal_pulse')
+        # self.sequence = PulseSequence(type=sequence)
 
-        if len(pe) == 1:
-            pe = pe[0]
+        # create model data
+        modeldata, modelnames, model_A, model_a, model_b = self._get_modeldata(X)
 
-        self.data[key] = pe
+        info_("*" * 50)
+        info_("  Entering fitting procedure")
+        info_("*" * 50)
 
-        return pe
+        global niter, chi2, everyiter, ncalls
+        ncalls = 0
+        everyiter = self.callback_every
+        niter = 0
 
-    def copy(self):
+        # # internally defined function chi2
+        # def funchi2(params, datasets, *constraints):
+        #     """
+        #     Return sum((y - x)**2)
+        #     """
+        #     global chi2, ncalls
+        #     # model spectrum
+        #
+        #     chi2 = 0
+        #     som = 0
+        #     ncalls += 1
+        #
+        #     for exp_idx, dataset in enumerate(datasets):
+        #         modeldata = self._get_modeldata(dataset, exp_idx)[0]
+        #         # baseline is already summed with modeldata[-1]
+        #
+        #         # important to work with the real component of dataset
+        #         # not the complex number
+        #         data = dataset.real.data.squeeze()
+        #
+        #         # if not dataset.is_2d:
+        #         mdata = modeldata[-1]  # modelsum
+        #
+        #         # else:
+        #         #    mdata = modeldata.values
+        #
+        #         merror = 1.0
+        #         # if dataset.is_2d:
+        #         #     if constraints:
+        #         #
+        #         #         # Case of SQ-DQ experiments
+        #         #         if self.kind == 'SQ-DQ' and \
+        #         #                         'max_connections' in constraints[0]:
+        #         #             # check connectivity numbers
+        #         #             nbconnections = {}
+        #         #             for key in params.keys():
+        #         #                 if 'pos1' in key:
+        #         #                     connect = key[-2:]
+        #         #                     key = 'ampl_line_' + connect  # get amplitude
+        #         #                     ki = connect[0].upper()
+        #         #                     if ki not in nbconnections.keys():
+        #         #                         nbconnections[ki] = 0
+        #         #                     if int(params[key]) > 0:
+        #         #                         nbconnections[ki] += 1
+        #         #             for k, v in nbconnections.iteritems():
+        #         #                 if v > constraints[0]['max_connections']:
+        #         #                     merror *= v * 10.
+        #
+        #         diff = data - mdata
+        #         chi2 += np.sum(diff**2) * merror
+        #         som += np.sum(data[0] ** 2)
+        #
+        #     chi2 = np.sqrt(chi2 / som)
+        #     # reset log_level
+        #     return chi2
+        # internally defined function chi2
+        def funchi2(params, X, *constraints):
+            """
+            Return sum((y - x)**2)
+            """
+            global chi2, ncalls
+            # model spectrum
+
+            chi2 = 0
+            ncalls += 1
 
-        import copy as cpy
+            # model
+            modeldata = self._get_modeldata(X)[0]
+            # baseline is already summed with modeldata[-1]
+            mdata = modeldata[-1]  # modelsum
+
+            # important to work with the real component of dataset
+            # not the complex number
+            data = X.real.squeeze()
 
-        data = cpy.copy(self.data)
-        lob = cpy.copy(self.lob)
-        upb = cpy.copy(self.upb)
-        fixed = cpy.copy(self.fixed)
-        reference = cpy.copy(self.reference)
+            diff = data - mdata
+            chi2 += np.sum(diff**2)  # * merror
+            return chi2
 
-        c = cpy.copy(self)
+        # end chi2 function ---------------------------------------------------
 
-        c.data = data
-        c.lob = lob
-        c.upb = upb
-        c.fixed = fixed
-        c.reference = reference
+        # callback function--------------------------------------------------------
+        def callback(*args, **kwargs):
+            """
+            callback log.info function
+            """
+            global niter, chi2, everyiter, ncalls
+            niter += 1
 
-        return c
+            if niter % everyiter != 0:
+                return
 
+            display.clear_output(wait=True)
+            info_(f"Iterations: {niter}, Calls: {ncalls} (chi2: {chi2:.5f})")
+            sys.stdout.flush()
 
-# =============================================================================
-class ParameterScript(HasTraits):
-    """
-    This class allow some manipulation of the parameter list for modelling.
-    """
+        # end callback function ---------------------------------------------------
 
-    fp = Instance(FitParameters)
+        fp = self.fp  # starting parameters
 
-    script = Unicode("")
+        if not self.dry:
+            fp, fopt = _optimize(
+                funchi2,
+                fp,
+                args=(X,),
+                maxfun=self.max_fun_calls,
+                maxiter=self.max_iter,
+                method=self.method,
+                constraints=self.constraints,
+                callback=callback,
+            )
 
-    datasets = List(Instance("spectrochempy.core.dataset.nddataset.NDDataset"))
+        # replace the previous script with new fp parameters
+        self.script = str(fp)
 
-    # ==================================================================================
-    # properties
-    # ==================================================================================
-    @observe("script")
-    def _check_parameters(self, change):
-        """
-        Check the validity of the parameters.
-        """
-        self.fp = self._interpret(self.script)
+        # log.info the results
+        info_("\n")
+        info_("*" * 50)
+        if not self.dry:
+            info_("  Result:")
+        else:
+            info_("  Starting parameters:")
+        info_("*" * 50)
+        info_(self.script)
+
+        # reset dry and continue to show starting model
+        self.dry = False
+
+        # return fit results
+        modeldata, names, A, a, b = self._get_modeldata(X)
+        if X.squeeze().ndim == 1:
+            # C in this case is just the A for all species
+            # (not very useful here but it will be necessary for 2D
+            # we eventually add baseline to the components
+            start = 0 if self.autobase else 1
+            C = np.ones((start, self._n_components)) * A
+            components = modeldata[start:-1]
+            total = modeldata[-1]
+        else:
+            # todo
+            pass
+        _outfit = C, components, total, A, a, b
+        return _outfit
 
     # ----------------------------------------------------------------------------------
-    def _interpret(self, script):
-        """
-        Interpreter of the script content.
-        """
+    # Private methods for validation
+    # ----------------------------------------------------------------------------------
+    @tr.validate("script")
+    def _script_validate(self, proposal):
+        script = proposal.value
+
         # init some flags
         modlabel = None
         common = False
         fixed = False
         reference = False
 
         # create a new FitParameters instance
         fp = FitParameters()
 
-        # set the number of experiments
-        fp.expnumber = len(self.datasets)
-        info_(f"The number of experiment(s) is set to {fp.expnumber}")
-
-        # start interpreting ------------------------------------------------------
+        # start interpreting -----------------------------------------------------------
         lines = script.split("\n")
         lc = 0
 
         for item in lines:
             lc += 1  # -------------- count the lines
             line = item.strip()
             if line == "" or line.startswith("#"):
@@ -412,38 +332,40 @@
                 continue
             elif key.startswith("common") or key.startswith("vars"):
                 common = True
                 modlabel = "common"
                 continue
             elif key.startswith("shape"):
                 shape = values.lower().strip()
-                if (
-                    shape is None
-                ):  # or (shape not in self._list_of_models and shape not in self._list_of_baselines):
+                if shape is None:  # or (shape not in self._list_of_models and shape not
+                    # in self._list_of_baselines):
                     raise ValueError(
-                        f"Shape of this model `{shape}` was not specified or is not implemented"
+                        f"Shape of this model `{shape}` was not specified"
+                        f" or is not implemented"
                     )
                 fp.model[modlabel] = shape
                 common = False
                 continue
-            elif key.startswith("experiment"):  # must be in common
-                if not common:
-                    raise ValueError(
-                        "'experiment_...' specification was found outside the common block."
-                    )
-                if "variables" in key:
-                    expvars = values.lower().strip()
-                    expvars = expvars.replace(",", " ").replace(";", " ")
-                    expvars = expvars.split()
-                    fp.expvars.extend(expvars)
-                continue
+            # elif key.startswith("experiment"):  # must be in common
+            #     if not common:
+            #         raise ValueError(
+            #             "'experiment_...' specification was found outside the common
+            #             block."
+            #         )
+            #     if "variables" in key:
+            #         expvars = values.lower().strip()
+            #         expvars = expvars.replace(",", " ").replace(";", " ")
+            #         expvars = expvars.split()
+            #         fp.expvars.extend(expvars)
+            #     continue
             else:
                 if modlabel is None and not common:
                     raise ValueError(
-                        "The first definition should be a label for a model or a block of variables or constants."
+                        "The first definition should be a label for a model or a block "
+                        "of variables or constants."
                     )
                 # get the parameters
                 if key.startswith("*"):
                     fixed = True
                     reference = False
                     key = key[1:].strip()
                 elif key.startswith("$"):
@@ -452,15 +374,16 @@
                     key = key[1:].strip()
                 elif key.startswith(">"):
                     fixed = True
                     reference = True
                     key = key[1:].strip()
                 else:
                     raise ValueError(
-                        f"Cannot interpret line {lc}: A parameter definition must start with *,$ or >"
+                        f"Cannot interpret line {lc}: A parameter definition must start"
+                        f" with *,$ or >"
                     )
 
                 # store this parameter
                 s = values.split(",")
                 s = [ss.strip() for ss in s]
                 if len(s) > 1 and ("[" in s[0]) and ("]" in s[1]):  # list
                     s[0] = "%s, %s" % (s[0], s[1])
@@ -486,345 +409,110 @@
                 else:
                     ks = f"{key}"
                     fp.common[key] = True
                 fp.reference[ks] = reference
                 if not reference:
                     val = value.strip()
                     val = eval(val)
-                    if isinstance(val, list):
-                        # if the parameter is already a list, that's ok if the number of parameters is ok
-                        if len(val) != fp.expnumber:
-                            raise ValueError(
-                                f"the number of parameters {len(val)} is not the number of experiments."
-                            )
-                        if key not in fp.expvars:
-                            raise ValueError(
-                                f"parameter {key} is not declared as variable"
-                            )
-                    else:
-                        if key in fp.expvars:
-                            # we create a list of parameters corresponding
-                            val = [val] * fp.expnumber
+                    # if isinstance(val, list):
+                    #     # if the parameter is already a list, that's ok if the number
+                    #     # of parameters is ok
+                    #     if len(val) != fp.expnumber:
+                    #         raise ValueError(
+                    #             f"the number of parameters {len(val)} is not the number "
+                    #             f"of experiments."
+                    #         )
+                    #     if key not in fp.expvars:
+                    #         raise ValueError(
+                    #             f"parameter {key} is not declared as variable"
+                    #         )
+                    # else:
+                    #     if key in fp.expvars:
+                    #         # we create a list of parameters corresponding
+                    #         val = [val] * fp.expnumber
                     fp[ks] = val, mini.strip(), maxi.strip(), fixed
                 else:
                     fp[ks] = value.strip()
 
-        return fp
-
-
-# ======================================================================================
-class Fit(HasTraits):
-    """
-    Fit a 1D or 2D dataset, or a list of datasets.
-
-
-    Parameters
-    ----------
-    dataset : Dataset or list of Dataset instance
-        The data to fit.
-
-    mode : Unicode, optional
-        Reserved - not used for now.
-
-    Attributes
-    ----------
-    fp : Dict
-        Fit parameters dictionary (read-only, but individual elements of the dict
-        can be changed)
-
-    script : Unicode
-        A string representation of the fp dict,
-        which can be used as input for other a fit (read-only)
-    """
-
-    silent = Bool(False)
-
-    _ = Any()
-
-    datasets = List(Instance("spectrochempy.core.dataset.nddataset.NDDataset"))
-
-    parameterscript = Instance(ParameterScript)
+        # update global fp
+        self.fp = fp
 
-    # *******************************************************************************
-    # initialisation
-    # *******************************************************************************
+        # return validated script
+        return script
 
-    def __init__(self, *args, **kwargs):
-
-        if args:
-            # look in args
-            if not isinstance(args[0], list):
-                self.datasets = [
-                    args[0],
-                ]
-            else:
-                self.datasets = args[0]
-                # we create a list of dataset in all case
-            script = args[1]
-
-        else:
-            return
-
-        # get parameters from script
-        self.parameterscript = ParameterScript(datasets=self.datasets, script=script)
-        if self.fp is None:  # pragma: no cover
-            # for unknown reason for now, this sometimes happens during tests
-            warn("error with fp")
-
-        # sequence = kargs.get('sequence', 'ideal_pulse')
-        # self.sequence = PulseSequence(type=sequence)
-
-        self.mode = kwargs.pop("mode", None)
-        self.method = kwargs.pop("method", None)
-        self.silent = kwargs.pop("silent", False)
-
-        for exp_idx, dataset in enumerate(self.datasets):
-            (
-                dataset.modeldata,
-                dataset.modelnames,
-                dataset.model_A,
-                dataset.model_a,
-                dataset.model_b,
-            ) = self._get_modeldata(
-                dataset, exp_idx
-            )  # lgtm[py/mismatched-multiple-assignment]
-
-    # *******************************************************************************
-    # public methods
-    # *******************************************************************************
-
-    @staticmethod
-    def script_default():
+    # ----------------------------------------------------------------------------------
+    # Private methods
+    # ----------------------------------------------------------------------------------
+    @tr.default("_script")
+    def _script_default(self):
         """
         Return a default script.
         """
         return """
-        #-----------------------------------------------------------
+        # -----------------------------------------------------------
         # syntax for parameters definition:
         # name: value, low_bound,  high_bound
+        # prefix:
+        #  # for comments
         #  * for fixed parameters
         #  $ for variable parameters
         #  > for reference to a parameter in the COMMON block
         #    (> is forbidden in the COMMON block)
         # common block parameters should not have a _ in their names
-        #-----------------------------------------------------------
+        # -----------------------------------------------------------
         #
 
         COMMON:
-        # common parameters ex.
-        experiment_variables: ampl
-
+        # common parameters
         # $ gwidth: 1.0, 0.0, none
           $ gratio: 0.5, 0.0, 1.0
 
         MODEL: LINE_1
         shape: voigtmodel
             $ ampl:  1.0, 0.0, none
             $ pos:   0.0, -100.0, 100.0
             > ratio: gratio
             $ width: 1.0, 0, 100
         """
 
-    def dry_run(self):
-        return self.run(dry=True)
-
-    def run(self, maxiter=100, maxfun=None, every=10, method="simplex", **kwargs):
-        """
-        Main fitting procedure.
-
-        Parameters
-        ----------
-        maxiter : int, maximum number of iteration
-        maxfun : int, maximum number of function calls
-        every : int, number of function call between two displays
-        method : str, ether 'simplex' or 'hopping'
-        dryrun : bool
-        """
-
-        if not self.silent:
-            level = preferences.log_level
-            if level > INFO:
-                preferences.log_level = INFO
-            info_("*" * 50)
-            info_("  Entering fitting procedure")
-            info_("*" * 50)
-
-        global niter, chi2, everyiter, ncalls
-        ncalls = 0
-        everyiter = every
-        niter = 0
-
-        # internally defined function chi2
-        def funchi2(params, datasets, *constraints):
-            """
-            Return sum((y - x)**2)
-            """
-            global chi2, ncalls
-            # model spectrum
-
-            chi2 = 0
-            som = 0
-            ncalls += 1
-
-            for exp_idx, dataset in enumerate(datasets):
-                modeldata = self._get_modeldata(dataset, exp_idx)[0]
-                # baseline is already summed with modeldata[-1]
-
-                # important to work with the real component of dataset
-                # not the complex number
-                data = dataset.real.data.squeeze()
-
-                # if not dataset.is_2d:
-                mdata = modeldata[-1]  # modelsum
-
-                # else:
-                #    mdata = modeldata.values
-
-                merror = 1.0
-                # if dataset.is_2d:
-                #     if constraints:
-                #
-                #         # Case of SQ-DQ experiments
-                #         if self.kind == 'SQ-DQ' and \
-                #                         'max_connections' in constraints[0]:
-                #             # check connectivity numbers
-                #             nbconnections = {}
-                #             for key in params.keys():
-                #                 if 'pos1' in key:
-                #                     connect = key[-2:]
-                #                     key = 'ampl_line_' + connect  # get amplitude
-                #                     ki = connect[0].upper()
-                #                     if ki not in nbconnections.keys():
-                #                         nbconnections[ki] = 0
-                #                     if int(params[key]) > 0:
-                #                         nbconnections[ki] += 1
-                #             for k, v in nbconnections.iteritems():
-                #                 if v > constraints[0]['max_connections']:
-                #                     merror *= v * 10.
-
-                diff = data - mdata
-                chi2 += np.sum(diff**2) * merror
-                som += np.sum(data[0] ** 2)
-
-            chi2 = np.sqrt(chi2 / som)
-            # reset log_level
-            return chi2
-
-        # end chi2 function ---------------------------------------------------
-
-        # callback function--------------------------------------------------------
-        def callback(*args, **kwargs):
-            """
-            callback log.info function
-            """
-            global niter, chi2, everyiter, ncalls
-            niter += 1
-
-            if niter % everyiter != 0:
-                return
-
-            if not self.silent:
-                display.clear_output(wait=True)
-                info_(
-                    ("Iterations: %d, Calls: %d (chi2: %.5f)" % (niter, ncalls, chi2))
-                )
-                sys.stdout.flush()
-
-        # end callback function ---------------------------------------------------
-
-        fp = self.fp  # starting parameters
-
-        dry = kwargs.get("dry", False)
-
-        if not dry:
-            fp, fopt = optimize(
-                funchi2,
-                fp,
-                args=(self.datasets,),
-                maxfun=maxfun,
-                maxiter=maxiter,
-                method=method,
-                constraints=kwargs.get("constraints", None),
-                callback=callback,
-            )
-
-        # replace the previous script with new fp parameters
-        self.parameterscript.script = str(fp)
-
-        if not self.silent:
-            # log.info the results
-            info_("\n")
-            info_("*" * 50)
-            if not dry:
-                info_("  Result:")
-            else:
-                info_("  Starting parameters:")
-            info_("*" * 50)
-            info_(self.parameterscript.script)
-
-        # store the models
-        for exp_idx, dataset in enumerate(self.datasets):
-            (
-                dataset.modeldata,
-                dataset.modelnames,
-                dataset.model_A,
-                dataset.model_a,
-                dataset.model_b,
-            ) = self._get_modeldata(dataset, exp_idx)
-
-        # Reset Log_level
-        if not self.silent:
-            preferences.log_level = level
-
-        return
-
-    # *******************************************************************************
-    # properties
-    # *******************************************************************************
-
-    @property
-    def fp(self):
-        return self.parameterscript.fp
-
-    @property
-    def script(self):
-        return self.parameterscript.script
-
-    # *******************************************************************************
-    # Private functions
-    # *******************************************************************************
-
-    def _repr_html_(self):
-        if not self.datasets:
-            return htmldoc(self.__init__.__doc__)
-        else:
-            return self.message
-
-    def _get_modeldata(self, dataset, exp_idx):
+    # def _repr_html_(self):
+    #     if not self.datasets:
+    #         return htmldoc(self.script)
+    #     else:
+    #         return self.message
+
+    def _get_modeldata(self, X, exp_idx=1):
+        # exp_idx is not used for the moment, but will be necessary for multidataset
+        # fitting
 
         # Prepare parameters
         parameters = self._prepare(self.fp, exp_idx)
 
         # Get the list of models
         models = self.fp.models
-        nbmodels = len(models)
+        self._n_components = nbmodels = len(models)
 
         # Make an array 'modeldata' with the size of the dataset of data
         # which will contains the data produced by the models
         # This name must always be 'modeldata'
         # which will be returned to the main program.
 
-        expedata = dataset.real.data.squeeze()
-        axis, dim = dataset.get_axis(-1)
-        x = dataset.coordset[dim].data
+        expedata = X.real.squeeze()
+
+        # we need to calculate the model with the full unmasked coordinates
 
         if expedata.ndim > 1:
             # nD data
             raise NotImplementedError("Fit not implemented for nD data yet!")
 
+        # we need to keep track of the x axis before masking
+        axis, dim = self._X.get_axis(-1)
+        _xaxis = self._X_coordset[dim].data
+
+        x = _xaxis
         modeldata = np.zeros((nbmodels + 2, x.size), dtype=np.float64)
 
         if nbmodels < 1:
             names = ["baseline", "modelsum"]
             return modeldata, names
 
         # Calculates model data
@@ -832,36 +520,47 @@
         # so we fill the array starting at row 1
         row = 0
         names = [
             "baseline",
         ]
 
         for model in models:
-            calc = getmodel(x, modelname=model, par=parameters)  # , dataset=dataset)
+            calc = getmodel(
+                x, modelname=model, par=parameters, amplitude_mode=self.amplitude_mode
+            )
             if not model.startswith("baseline"):
                 row += 1
                 modeldata[row] = calc
                 names.append(model)
             else:
                 modeldata[0] += calc
 
         # make the sum
         modeldata[row + 1] = modeldata.sum(axis=0)
         names.append("modelsum")
 
         # remove unused column
         modeldata = modeldata[: row + 2]
 
-        xi = np.arange(float(x.size))
-        A, a, b = self._ampbas(xi, expedata, modeldata[-1])
+        # remove masked column
+        if np.any(self._X_mask):
+            masked_columns = np.all(self._X_mask, axis=-2)
+            modeldata = modeldata[:, ~masked_columns]
+            x = x[~masked_columns]
+
+        if self.autobase:
+            A, a, b = self._ampbas(x, expedata, modeldata[-1])
+        else:
+            A, a, b = 1.0, 0.0, 0.0
+
         # (fitzone-fitzone[0], data.take(fitzone),
         # modeldata[-1].take(fitzone))
 
         modeldata = A * modeldata
-        baseline = a * xi + b  # a*(xi-fitzone[0]) + b
+        baseline = a * x + b  # a*(xi-fitzone[0]) + b
 
         # update the modeldata
         modeldata[0] += baseline
         modeldata[-1] += baseline
 
         # return modeldata
         return modeldata, names, A, a, b
@@ -874,15 +573,15 @@
         for kw in mo:
             if kw in param:
                 expr = expr.replace(kw, str(param[kw]))
             elif kw in np.__dict__:  # check if it is a recognized math function
                 expr = expr.replace(kw, "np.%s" % kw)
         return expr
 
-    def _prepare(self, param, exp_idx):
+    def _prepare(self, param, exp_idx=1):
         # This function is needed for the script related to modelfunction
         #
         # exp_idx: int, contains the index of the experiment
 
         new_param = param.copy()
 
         for key in param:
@@ -904,16 +603,16 @@
                     raise ValueError(
                         "Cannot evaluate the expression %s: %s" % (key, param[refpar])
                     )
 
                 new_param.fixed[key] = True
                 new_param.reference[key] = True  # restore it for the next call
 
-            if isinstance(new_param[key], list):
-                new_param.data[key] = new_param.data[key][exp_idx]
+            # if isinstance(new_param[key], list):
+            #     new_param.data[key] = new_param.data[key][exp_idx]
 
         return new_param
 
     # ==================================================================================
     # automatic calculation of amplitude and baseline
     # ==================================================================================
     @staticmethod
@@ -1172,50 +871,90 @@
             a = 0.0
         if np.isnan(b):
             b = 0.0
         if np.isnan(c):
             c = 0.0
         return A, a, b, c
 
+    # ----------------------------------------------------------------------------------
+    # Public methods and properties
+    # ----------------------------------------------------------------------------------
+    def _transform(self, X=None):
+        # X is ignored for Optimize
+        # this method is present for coherence with other decomposition methods
+        return self._outfit[0]
+
+    def _inverse_transform(self, X_transform=None):
+        # X_transform is ignored for Optimize
+        # this method is present for coherence with other decomposition methods
+        X_transform = self._outfit[2]
+        if X_transform.ndim == 1:
+            # we need a seconddimension of size 1 for the restoration of masks
+            X_transform = X_transform[np.newaxis]
+        return X_transform
+
+    def _get_components(self):
+        return self._outfit[1]  # the first is the baseline, the last is the sum
+
+    # ----------------------------------------------------------------------------------
+    # Public methods/properties
+    # ----------------------------------------------------------------------------------
+    @_docstring.dedent
+    def fit(self, X):
+        """
+        Perform a non-linear optimization of the ``X`` dataset.
+
+        Parameters
+        ----------
+        %(analysis_fit.parameters.X)s
+
+        Returns
+        -------
+        %(analysis_fit.returns)s
+
+        See Also
+        --------
+        %(analysis_fit.see_also)s
+        """
+        return super().fit(X, Y=None)
+
 
 # ======================================================================================
-def optimize(
+def _optimize(
     func,
     fp0,
     args=(),
     constraints={},
     method="SIMPLEX",
     maxfun=None,
     maxiter=1000,
     ftol=1e-8,
     xtol=1e-8,
     callback=None,
 ):
-    """
-    Parameters
-    ----------
-    func
-    fp0
-    args
-    constraints
-    method
-    maxfun
-    maxiter
-    ftol
-    xtol
-    callback
-
-
-    #  Internal/external transformation
-    #  These transformations are used in the MINUIT package,
-    #  and described in detail
-    #  in the section 1.3.1 of the MINUIT User's Guide.
-
-
-    """
+    # """
+    # Parameters
+    # ----------
+    # func
+    # fp0
+    # args
+    # constraints
+    # method
+    # maxfun
+    # maxiter
+    # ftol
+    # xtol
+    # callback
+    #
+    #
+    # #  Internal/external transformation
+    # #  These transformations are used in the MINUIT package,
+    # #  and described in detail
+    # #  in the section 1.3.1 of the MINUIT User's Guide.
+    # """
 
     global keys
 
     def restore_external(fp, p, keys):
         # restore external parameters
         for key in list(fp.keys()):
             keysp = key.split("_")
@@ -1321,7 +1060,69 @@
 
     if warnmess == 1:
         warning_("Maximum number of function evaluations made.")
     if warnmess == 2:
         warning_("Maximum number of iterations reached.")
 
     return fpe, fopt
+
+
+# ======================================================================================
+def getmodel(x, y=None, modelname=None, par=None, **kwargs):
+    """
+    Get the model for a given x vector.
+
+    Parameters
+    -----------
+    x : ndarray
+        Array of frequency where to evaluate the model values returned by the
+        f function.
+    y : ndarray or None
+        None for 1D, or index for the second dimension.
+    modelname : str
+        Name of the model class to use.
+    par : :class:`Parameters` instance
+        Parameter to pass to the f function.
+    kargs : any
+        Keywords arguments to pass to the f function.
+
+    Returns
+    -------
+    `~numpy.ndarray`
+        Array containing the calculated model.
+    """
+    model = par.model[modelname]
+    modelcls = getattr(models_, model)
+
+    # take an instance of the model
+    a = modelcls()
+
+    # get the parameters for the given model
+    args = []
+    for p in a.args:
+        try:
+            args.append(par[f"{p}_{modelname}"])
+        except KeyError as e:
+            if p.startswith("c_"):
+                # probably the end of the list
+                # due to a limited polynomial degree
+                pass
+            else:
+                raise ValueError(e)
+
+    x = np.array(x, dtype=np.float64)
+    if y is not None:
+        y = np.array(y, dtype=np.float64)
+
+    if y is None:
+        val = a.f(x, *args, **kwargs)
+    else:
+        val = a.f(x, y, *args, **kwargs)
+
+    # Return amplitude or area ? return calc is scaled by area by default
+    amplitude_mode = kwargs.pop("amplitude_mode")
+    if amplitude_mode.lower() == "height":
+        # in this case ampl parameter is the height, so we need to rescale
+        # calc
+        ampl = args[0]
+        val = ampl * val / val.max()
+    return val
```

### Comparing `spectrochempy-0.5.5/spectrochempy/analysis/iris.py` & `spectrochempy-0.6.1/spectrochempy/analysis/iris.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,497 +3,639 @@
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 This module implements the IRIS class.
 """
-__all__ = ["IRIS", "kern"]
-__dataset_methods__ = []
+__all__ = ["IrisKernel", "IRIS"]
+__configurables__ = ["IRIS"]
 
-from collections.abc import Iterable
+# from collections.abc import Iterable
 
 import numpy as np
 import quadprog
+import traitlets as tr
 from matplotlib import pyplot as plt
 from scipy import optimize
 
+from spectrochempy.analysis._base import DecompositionAnalysis, NotFittedError
 from spectrochempy.core import info_, warning_
 from spectrochempy.core.dataset.coord import Coord
+from spectrochempy.core.dataset.coordset import CoordSet
 from spectrochempy.core.dataset.nddataset import NDDataset
+from spectrochempy.extern.traittypes import Array
+from spectrochempy.utils.constants import EPSILON
+from spectrochempy.utils.decorators import signature_has_configurable_traits
+from spectrochempy.utils.docstrings import _docstring
+from spectrochempy.utils.traits import CoordType, NDDatasetType
 
 
-def kern(K, p, q):
+@tr.signature_has_traits
+class IrisKernel(tr.HasTraits):
     """
-    Compute kernel of Fredholm equation of the 1st kind.
+    Define a kernel matrix of Fredholm equation of the 1st kind.
 
-    This function computes a kernel matrix and returns it as NDDataset. Pre-defined kernels can be chosen among:
-    {'langmuir', 'ca', 'reactant-first-order', 'product-first-order', diffusion} A custom kernel fucntion - a
-    2-variable lambda function `ker(p, q)` or a function returning a ndarray can be passed. `p` and `q` contain
-    the values of an external experimental variable and an internal physico-chemical parameter, respectively.
+    This class define a kernel matrix as a `NDDataset` compatible
+    with the `X` input `NDDataset`\ .
 
-    Parameters
-    ----------
-    K : str or callable
-        Kernel type.
-    p : Coord or ndadarray
-        External variable.
-    q : Coord or ndadarray
-        Internal variable.
-
-    Returns
-    -------
-    NDDataset
-        The kernel.
-
-    See Also
-    --------
-    IRIS : Integral inversion solver for spectroscopic data.
+    Pre-defined kernels can be chosen among: {``'langmuir'``\ , ``'ca'``\ ,
+    ``'reactant-first-order'``\ , ``'product-first-order'``\ , ``'diffusion'``\ },
+    a custom kernel function - a 2-variable lambda
+    function `K`\ ``(p, q)`` or a function returning a `~numpy.ndarray` can be passed.
+    `p` and `q` contain the values of an external experimental variable and an internal
+    physico-chemical parameter, respectively.
 
-    Examples
-    --------
-    # the three examples below are equivalents:
-    >>> scp.kern('langmuir', np.linspace(0, 1, 100), np.logspace(-10, 1, 10))
-    NDDataset: [float64] unitless (shape: (y:100, x:10))
-
-    >>> F = lambda p, q : np.exp(-q) * p[:, None] / (1 + np.exp(-q) * p[:, None])
-    >>> scp.kern(F, np.linspace(0, 1, 100), np.logspace(-10, 1, 10))
-    NDDataset: [float64] unitless (shape: (y:100, x:10))
-
-    >>> def F(p,q):
-    ...    return np.exp(-q) * p[:, None] / (1 + np.exp(-q) * p[:, None])
-    >>>
-    >>> scp.kern(F, np.linspace(0, 1, 100), np.logspace(-10, 1, 10))
-    NDDataset: [float64] unitless (shape: (y:100, x:10))
-
-    # p and q can also be passed as coordinates:
-    >>> p = scp.Coord(np.linspace(0, 1, 100), name="pressure", title="p", units="torr")
-    >>> q = scp.Coord(np.logspace(-10, 1, 10), name="reduced adsorption energy",
-    ...              title="$\Delta_{ads}G^{0}/RT$", units="")
-    >>> scp.kern('langmuir', p, q)
-    NDDataset: [float64] unitless (shape: (y:100, x:10))
+    Parameters
+    -----------
+    X : `NDDataset`
+        The 1D or 2D dataset for the kernel is defined.
+    K : any of [ ``'langmuir'`` , ``'ca'`` , ``'reactant-first-order'`` , ``'product-first-order'`` , ``'diffusion'`` ] or `callable` or `NDDataset`
+        Predefined or user-defined Kernel for the integral equation.
+    p :  `Coord` or ``iterable``
+        External variable. Must be provided if the kernel `K` is passed as a `str` or
+        `callable` .
+    q :  `Coord` or ``iterable`` of 3 values
+        Internal variable. Must be provided if the kernel `K` is passed as a `str` or
+        `callable`.
     """
 
-    if not isinstance(q, Coord):  # q was passed as a ndarray
-        q = Coord(data=q, name="internal variable", title="$q$", units="")
-        q_was_array = True
-    else:
-        q_was_array = False
-    if not isinstance(p, Coord):  # p was passed as a ndarray
-        p = Coord(data=p, name="external variable", title="$p$", units="")
-        p_was_array = True
-    else:
-        p_was_array = False
-
-    if isinstance(K, str):
-        _adsorption = {"langmuir", "ca"}
-        _kinetics = {"reactant-first-order", "product-first-order"}
-        _diffusion = {"diffusion"}
-
-        if K.lower() in _adsorption:
-            if q_was_array:  # change default values and units
-                q.name = "reduced adsorption energy"
-                q.title = "$\Delta_{ads}G^{0}/RT$"
-            if p_was_array:  # change default values and units
-                p.name = "relative pressure"
-                p.title = "$p_/p_^{0}$"
-
-            if K.lower() == "langmuir":
-                K_ = (
-                    np.exp(-q.data)
-                    * p.data[:, None]
-                    / (1 + np.exp(-q.data) * p.data[:, None])
-                )
+    _X = NDDatasetType(allow_none=True)
+    _K = (
+        tr.Union(
+            (
+                tr.Enum(
+                    [
+                        "langmuir",
+                        "ca",
+                        "reactant-first-order",
+                        "product-first-order",
+                        "diffusion",
+                    ]
+                ),
+                tr.Callable(),
+                NDDatasetType(),
+            ),
+            default_value=None,
+            allow_none=True,
+        ),
+    )
+
+    _p = CoordType(
+        # CoordType include array-like iterables
+    )
+    _q = tr.Union(
+        (
+            tr.List(),
+            CoordType(),
+            # CoordType include array-like iterables
+        ),
+    )
+
+    # ----------------------------------------------------------------------------------
+    # Initialization
+    # ----------------------------------------------------------------------------------
+    def __init__(self, X, K, p=None, q=None, **kwargs):
+
+        info_("Creating Kernel...")
+
+        self._X = X
+        self._K = K
+        if p is not None:
+            self._p = p
+        if q is not None:
+            self._q = q
+
+        info_("Kernel now ready as IrisKernel().kernel!")
+
+    # ----------------------------------------------------------------------------------
+    # default values
+    # ----------------------------------------------------------------------------------
+    @tr.default("_p")
+    def _p_default(self):
+        return self._X.coordset[self._X.dims[0]].default
+
+    @tr.default("_q")
+    def _q_default(self):
+        q = None
+        if isinstance(self._K, NDDataset):
+            q = self._K.coordset[self._K.dims[-1]]
+        return q
+
+    # ----------------------------------------------------------------------------------
+    # Validation
+    # ----------------------------------------------------------------------------------
+    @tr.validate("_p")
+    def _p_validate(self, proposal):
+        p = proposal.value
+        # as p belong CoordType, it is necessarily a Coord at this point.
+        if len(p) != self._X.shape[0]:
+            raise ValueError(
+                "'p' size should be consistent with the y coordinate of the dataset"
+            )
+        # change its default metadata if necessary
+        # (i.e. if p was not provided as already a Coord).
+        if p.name == p.id:
+            p.name = "external variable"
+        if p.title == "<untitled>":
+            p.title = "$p$"
+        if p.units is None:
+            p.units = ""
+        return p
+
+    @tr.validate("_q")
+    def _q_validate(self, proposal):
+        q = proposal.value
+        if isinstance(self._K, str) or callable(self._K):
+            # case of a list
+            if isinstance(q, list):
+                if len(q) == 3:
+                    q = np.linspace(q[0], q[1], q[2])
+                else:
+                    warning_(
+                        "Provided q is a list a {len(q)} items. "
+                        "It will be converted to a Coord object. "
+                        "If this is not what you wanted, remember that only list "
+                        "of strictly 3 items are treated differently."
+                    )
+                # Transform the list or array-like to Coord
+                q = Coord(q)
 
-            else:  # this is 'ca'
-                K_ = np.ones((len(p.data), len(q.data)))
-                K_[p.data[:, None] < q.data] = 0
-
-            title = "coverage"
-
-        elif K.lower() in _kinetics:
-            if q_was_array:  # change default values and units
-                q.name = "Ln of rate constant"
-                q.title = "$\Ln k$"
-            if p_was_array:  # change default values and units
-                p.name = "time"
-                p.title = "$t$"
-                p.units = "s"
-
-            if K.lower() == "reactant-first-order":
-                K_ = np.exp(-1 * np.exp(q.data) * p.data[:, None])
-
-            else:  # 'product-first-order'
-                K_ = 1 - np.exp(-1 * np.exp(q.data) * p.data[:, None])
-
-            title = "coverage"
-
-        elif K.lower() in _diffusion:
-            if q_was_array:  # change default values and units
-                q.name = "Diffusion rate constant"
-                q.title = "$\\tau^{-1}$"
-                # q.to('1/s', force=True)
-            if p_was_array:  # change default values and units
-                p.name = "time"
-                p.title = "$t$"
-                # p.to('s', force=True)
-
-            title = "fractional uptake"
-
-            K_ = np.zeros((p.size, q.size))
-            for n in np.arange(1, 100):
-                K_ += (1 / n**2) * np.exp(
-                    -(1 / 9) * n**2 * np.pi**2 * q.data * p.data[:, None]
+            # q should now be a Coord in all cases
+            if not isinstance(q, Coord):
+                raise ValueError(
+                    "q must be provided as a list of 3 items or a array-like object "
+                    "that can be casted to a Coord object"
                 )
-            K_ = 1 - (6 / np.pi**2) * K_
 
+            # At this point, q is surely a Coord.
+            # change its default metadata if necessary.
+            # (i.e. if q was not provided as already a Coord).
+            if q.name == q.id:
+                q.name = "internal variable"
+            if q.title == "<untitled>":
+                q.title = "$q$"
+            if q.units is None:
+                q.units = ""
         else:
-            raise NameError(f"This kernel: <{K}> is not implemented")
+            pass
+            # K was probably defined as a NDDataset, so q will be provided
+            # as the default
+        return q
+
+    # ----------------------------------------------------------------------------------
+    # Kernel property
+    # ----------------------------------------------------------------------------------
+    @property
+    def kernel(self):
+
+        _adsorption = ["langmuir", "ca"]
+        _kinetics = ["reactant-first-order", "product-first-order"]
+        _diffusion = ["diffusion"]
+
+        K = self._K
+        p = self._p.copy()
+        q = self._q.copy()
+
+        qdefault = q.name == "internal variable" and q.title == "$q$"
+        pdefault = p.name == "external variable" and p.title == "$p$"
+
+        if isinstance(K, str):
+
+            if K.lower() not in _adsorption + _kinetics + _diffusion:
+                raise NotImplementedError(
+                    f"Kernel type `{K.lower()}` is not implemented"
+                )
 
-    elif callable(K):
-        K_ = K(p.data, q.data)
-        title = ""
-
-    else:
-        raise ValueError("K must be a str or a callable")
-
-    # weighting coefficients for the numerical quadrature of the Fredholm integral
-    w = np.zeros((q.size))
-    w[0] = 0.5 * (q.data[-1] - q.data[0]) / (q.size - 1)
-    w[1:-1] = 2 * w[0]
-    w[-1] = w[0]
-
-    out = NDDataset(K_ * w)
-    if isinstance(K, str):
-        out.name = K + " kernel matrix"
-    else:
-        out.name = "kernel matrix"
-    out.dims = ["y", "x"]
-    out.y = p
-    out.x = q
-    out.title = title
+            elif K.lower() in _adsorption:
+                title = "coverage"
 
-    return out
+                # change default metadata
+                if qdefault:
+                    q.name = "reduced adsorption energy"
+                    q.title = "$\Delta_{ads}G^{0}/RT$"
+
+                if pdefault:
+                    p.name = "relative pressure"
+                    p.title = "$p_/p_^{0}$"
+
+                if K.lower() == "langmuir":
+                    kernel = (
+                        np.exp(-q.data)
+                        * p.data[:, None]
+                        / (1 + np.exp(-q.data) * p.data[:, None])
+                    )
 
+                else:  # 'ca'
+                    kernel = np.ones((len(p.data), len(q.data)))
+                    kernel[p.data[:, None] < q.data] = 0
+
+            elif K.lower() in _kinetics:
+                title = "coverage"
+
+                # change default metadata
+                if qdefault:
+                    q.name = "Ln of rate constant"
+                    q.title = "$\Ln k$"
+                if pdefault:
+                    # change default values and units
+                    p.name = "time"
+                    p.title = "$t$"
+                    p.units = "s"
+
+                if K.lower() == "reactant-first-order":
+                    kernel = np.exp(-1 * np.exp(q.data) * p.data[:, None])
+
+                else:  # 'product-first-order'
+                    kernel = 1 - np.exp(-1 * np.exp(q.data) * p.data[:, None])
+
+            elif K.lower() in _diffusion:
+                title = "fractional uptake"
+
+                # change default metadata
+                if qdefault:
+                    q.name = "Diffusion rate constant"
+                    q.title = "$\\tau^{-1}$"
+                    # q.to('1/s', force=True)
+                if pdefault:
+                    p.name = "time"
+                    p.title = "$t$"
+                    # p.to('s', force=True)
+
+                kernel = np.zeros((p.size, q.size))
+                for n in np.arange(1, 100):
+                    kernel += (1 / n**2) * np.exp(
+                        -(1 / 9) * n**2 * np.pi**2 * q.data * p.data[:, None]
+                    )
+                kernel = 1 - (6 / np.pi**2) * kernel
 
-class IRIS:
-    """
-    Integral inversion solver for spectroscopic data.
+        elif callable(K):
+            kernel = K(p.data, q.data)
+            title = ""
 
-    Solves integral equations of the first kind of 1 or 2 dimensions, i.e. returns a
-    distribution f of contributions to 1D ou 2D datasets.
+        else:
+            raise ValueError("K must be a str or a callable")
 
-    Parameters
-    -----------
-    X : NDDataset
-        The 1D or 2D dataset on which to perform the IRIS analysis.
-    K : str or callable or NDDataset
-        Kernel of the integral equation. Pre-defined kernels can be chosen among
-        `["langmuir", "ca", "reactant-first-order", "product-first-order", "diffusion"]`.
-    p : Coord or Iterable
-        External variable. Must be provided if the kernel is passed as a str or callable.
-    q : Coord or Iterable of 3 values
-        Internal variable. Must be provided if the kernel is passed as a str or callable.
-    reg_par : None or array_like of two values `[min, max]` or three values `[start, stop, num]`
-        Regularization parameter.
+        # weighting coefficients for the numerical quadrature of the Fredholm integral
+        w = np.zeros((q.size))
+        w[0] = 0.5 * (q.data[-1] - q.data[0]) / (q.size - 1)
+        w[1:-1] = 2 * w[0]
+        w[-1] = w[0]
+
+        kernel = kernel * w
+        if isinstance(K, str):
+            name = K + " kernel matrix"
+        else:
+            name = "kernel matrix"
+        dims = ["y", "x"]
+        out = NDDataset(
+            kernel, dims=dims, coordset=CoordSet(y=p, x=q), title=title, name=name
+        )
 
-    Attributes
-    ----------
-    f : NDDataset
-        A 3D/2D dataset containing the solutions (one per regularization parameter).
-    RSS: array of float
-        Residual sums of squares (one per regularization parameter).
-    SM : array of float
-        Values of the regularization constraint (one per regularization parameter).
-    reg_par : None or array of float
-        Values of the regularization parameters.
-    log : str
-        Log of the optimization.
-    K : NDDataset
-        Kernel matrix.
-    X : NDDataset
-        The original dataset.
+        return out
 
-    See Also
-    --------
-        ker : Compute kernel of Fredholm equation of the 1st kind.
 
-    Notes
-    -----
-    IRIS solves integral equation of the first kind of 1 or 2 dimensions, i.e. finds a distribution
-    function :math:`f(p)` or :math:`f(c,p)` of contributions to univariate data :math:`a(p)` or multivariate
-    :math:`a(c, p)` data evolving with an external experimental variable :math:`p` (time, pressure,
-    temperature, concentration, ...) according to the integral transform:
+@signature_has_configurable_traits
+class IRIS(DecompositionAnalysis):
+
+    _docstring.delete_params("DecompositionAnalysis.see_also", "IRIS")
+
+    __doc__ = _docstring.dedent(
+        """
+    Integral inversion solver for spectroscopic data (IRIS).
+
+    `IRIS`, a model developed by :cite:t:`stelmachowski:2013`\ , solves integral
+    equation of the first kind of 1 or 2 dimensions, *i.e.,*
+    finds a distribution function :math:`f(p)` or :math:`f(c,p)` of contributions to
+    univariate data :math:`a(p)` or multivariate :math:`a(c, p)` data evolving with an
+    external experimental variable :math:`p` (time, pressure, temperature,
+    concentration, ...) according to the integral transform:
 
     .. math:: a(c, p) = \int_{min}^{max} k(q, p) f(c, q) dq
 
     .. math:: a(p) = \int_{min}^{max} k(q, p) f(q) dq
 
-    where the kernel :math:`k(q, p)` expresses the functional dependence of a single contribution
-    with respect to the experimental variable :math:`p` and and 'internal' physico-chemical variable :math:`q`
-    Regularization is triggered when 'reg_param' is set to an array of two or three values.
-    If 'reg_param' has two values [min, max], the optimum regularization parameter is searched between
-    :math:`10^{min}` and :math:`10^{max}`. Automatic search of the regularization is made using the
-    Cultrera_Callegaro algorithm (arXiv:1608.04571v2) which involves the Menger curvature of a circumcircle
-    and the golden section search method.
-    If three values are given (`[min, max, num]`), then the inversion will be made for num values
-    evenly spaced on a log scale between :math:`10^{min}` and :math:`10^{max}`
+    where the kernel :math:`k(q, p)` expresses the functional dependence of a single
+    contribution with respect to the experimental variable :math:`p` and 'internal'
+    physico-chemical variable :math:`q` .
+
+    Regularization is triggered when `reg_par` is set to an array of two or three
+    values.
+
+    If `reg_par` has two values [``min``\ , ``max``\ ], the optimum regularization
+    parameter is searched between :math:`10^{min}` and :math:`10^{max}`\ .
+    Automatic search of the regularization is made using the Cultrera_Callegaro
+    algorithm (:cite:p:cultrera:2020) which involves the Menger curvature of a
+    circumcircle and the golden section search method.
+
+    If three values are given ([``min``\ , ``max``\ , ``num``\ ]), then the inversion
+    will be made for ``num`` values evenly spaced on a log scale between
+    :math:`10^{min}` and :math:`10^{max}`\ .
+
+    Parameters
+    ----------
+    %(AnalysisConfigurable.parameters)s
+
+    See Also
+    --------
+    %(DecompositionAnalysis.see_also.no_IRIS)s
 
     Examples
     --------
     >>> X = scp.read("irdata/CO@Mo_Al2O3.SPG")
     >>> p = [0.003, 0.004, 0.009, 0.014, 0.021, 0.026, 0.036, 0.051, 0.093, 0.150,
     ...      0.203, 0.300, 0.404, 0.503, 0.602, 0.702, 0.801, 0.905, 1.004]
     >>> iris = scp.IRIS(X[:,2250.0:1960.0], "langmuir", q = [-8, -1, 10])
     >>> iris.f
     NDDataset: [float64] unitless (shape: (z:1, y:10, x:301))
     """
+    )
 
-    def __init__(self, X, K, p=None, q=None, reg_par=None):
-        global _log
-        _log = ""
-
-        # check if x dimension exists
-        if "x" in X.dims:
-            # if multiple coords for a given dimension, take the default ones:
-            channels = X.x.default
-        else:
-            # else, set a single channel:
-            channels = Coord([0])
-
-        if p is not None:  # supersedes the default
-            if isinstance(p, Coord):
-                if p.shape[1] != X.shape[0]:
-                    raise ValueError(
-                        "'p' should be consistent with the y coordinate of the dataset"
-                    )
-            else:
-                if len(p) != X.shape[0]:
-                    raise ValueError(
-                        "'p' should be consistent with the y coordinate of the dataset"
-                    )
-                p = Coord(p, title="External variable")
-        else:
-            p = X.y.default
-
-        # check options
-        # defines the kernel
-
-        if isinstance(K, NDDataset) and q is None:
-            q = K.x
-        elif isinstance(K, str) or callable(K):
-            if isinstance(q, Coord):
-                pass
-            elif isinstance(q, Iterable):
-                if len(q) == 3:
-                    q = np.linspace(q[0], q[1], q[2])
-            else:
-                raise ValueError(
-                    "q must be provided as a Coord, a NDarray or an iterable of 3 items"
-                )
-
-            msg = f"Build kernel matrix with: {K}\n"
-            info_(msg)
-            _log += msg
-            K = kern(K, p, q)
-            q = K.x  # q is now a Coord
-
-        # defines regularization parameter values
-
-        if reg_par is None:
-            regularization = False
-            search_reg = False
-            reg_par = [0]
+    # ----------------------------------------------------------------------------------
+    # Runtime Parameters (in addition to those of AnalysisConfigurable)
+    # ----------------------------------------------------------------------------------
+    _Y = tr.Union(
+        (
+            tr.Instance(IrisKernel),
+            NDDatasetType(),
+        ),
+        default_value=None,
+        allow_none=True,
+        help="Target/profiles taken into account to fit a model",
+    )
+    _Y_preprocessed = Array(help="preprocessed Y")
+    _q = CoordType()
+    _channels = CoordType()
+    _lambdas = CoordType()
+    _regularization = tr.Bool(False)
+    _search_reg = tr.Bool(False)
+
+    # ----------------------------------------------------------------------------------
+    # Configuration parameters
+    # ----------------------------------------------------------------------------------
+    reg_par = tr.List(
+        minlen=2,
+        maxlen=3,
+        default_value=None,
+        allow_none=True,
+        help="Regularization parameter (two values [ ``min`` , ``max`` ] "
+        "or three values [ ``start`` , ``stop`` , ``num`` ]. "
+        "If `reg_par` is None, no :term:`regularization` is applied.",
+    ).tag(config=True)
+
+    # ----------------------------------------------------------------------------------
+    # Initialization
+    # ----------------------------------------------------------------------------------
+    def __init__(
+        self,
+        log_level="WARNING",
+        warm_start=False,
+        copy=True,
+        **kwargs,
+    ):
+        # call the super class for initialisation of the configuration parameters
+        # to do before anything else!
+        super().__init__(
+            log_level=log_level,
+            warm_start=warm_start,
+            copy=copy,
+            **kwargs,
+        )
+        # no validation of reg_par triggred when it is None
+        # so we need to init self._lambdas manually else itt will not be inited
+        if self.reg_par is None:
+            self._lambdas = Coord([0], title="lambda")
+
+    # ----------------------------------------------------------------------------------
+    # Private validation and default getter methods
+    # ----------------------------------------------------------------------------------
+    @tr.validate("reg_par")
+    def _reg_par_validate(self, proposal):
+        reg_par = proposal.value
+        if reg_par is None or len(reg_par) == 1:
+            self._regularization = False
+            self._search_reg = False
+            _lambdas = [0]
         elif len(reg_par) == 2:
-            regularization = True
-            search_reg = True
+            self._regularization = True
+            self._search_reg = True
+            _lambdas = reg_par
         elif len(reg_par) == 3:
-            regularization = True
-            search_reg = False
-            reg_par = np.logspace(reg_par[0], reg_par[1], reg_par[2])
+            self._regularization = True
+            self._search_reg = False
+            _lambdas = np.logspace(reg_par[0], reg_par[1], reg_par[2])
         else:
             raise ValueError(
                 "reg_par should be either None or a set of 2 or 3 integers"
             )
 
+        # create the lambdas coordinate
+        self._lambdas = Coord(_lambdas, title="lambda")
+
+        # return the validated reg_par with no transformation
+        return reg_par
+
+    @tr.validate("_Y")
+    def _Y_validate(self, proposal):
+        # validation of the _Y attribute: fired when self._Y is assigned
+        # In this IRIS model, we can have either a IrisKernel object or a NDDataset
+        Y = proposal.value
+        # we need a dataset
+        if isinstance(Y, IrisKernel):
+            Y = Y.kernel
+        return Y
+
+    @tr.observe("_Y")
+    def _preprocess_as_Y_changed(self, change):
+        Y = change.new
+        # store the coordinate q
+        self._q = Y.coordset[Y.dims[-1]]
+        # use data only
+        self._Y_preprocessed = Y.data
+
+    @tr.observe("_X")
+    def _preprocess_as_X_changed(self, change):
+        # we need the X.x axis (called channels) later in the IRIS calculation
+        # get it from the self._X nddataset (where masked data have been removed)
+        X = change.new
+        self._channels = X.coordset[X.dims[-1]]
+        # use data only
+        self._X_preprocessed = X.data
+
+    # ----------------------------------------------------------------------------------
+    # Private methods (overloading abstract classes)
+    # ----------------------------------------------------------------------------------
+    def _fit(self, X, K):
+        # X is the data array to fit
+        # K is the kernel data array
+
+        q = self._q.data
+        lambdas = self._lambdas.data
+
         # define containers for outputs
-        if not regularization:
-            f = np.zeros((1, len(q), len(channels.data)))
-            RSS = np.zeros((1))
-            SM = np.zeros((1))
-
-        if regularization and not search_reg:
-            f = np.zeros((len(reg_par), len(q), len(channels.data)))
-            RSS = np.zeros((len(reg_par)))
-            SM = np.zeros((len(reg_par)))
-
-        if regularization and search_reg:
-            f = np.zeros((4, len(q), len(channels.data)))
-            RSS = np.zeros((4))
-            SM = np.zeros((4))
+        M, N, W = K.shape[-1], X.shape[-1], X.shape[0]  # noqa: F475
+        L = len(lambdas) if not self._search_reg else 4
+        f = np.zeros((L, M, N))
+        RSS = np.zeros((L))
+        SM = np.zeros((L))
 
         # Define S matrix (sharpness), see function _Smat() below
-        msg = "Build S matrix (sharpness)\n"
-        info_(msg)
-        _log += msg
+        info_("Build S matrix (sharpness)")
         S = _Smat(q)
-        msg = "... done\n"
-        info_(msg)
-        _log += msg
-
-        # Solve unregularized problem
-        if not regularization:
-            msg = "Solving for {} channels and {} observations, no regularization\n".format(
-                X.shape[1], X.shape[0]
-            )
-            _log += msg
+        info_("... done")
+
+        # Solve non-regularized problem
+        if not self._regularization:
+            msg = f"Solving for {N} channels and {W} observations, no regularization"
             info_(msg)
 
             # use scipy.nnls() to solve the linear problem: X = K f
-            for j, _ in enumerate(channels.data):
-                f[0, :, j] = optimize.nnls(K.data, X[:, j].data.squeeze())[0]
-            res = X.data - np.dot(K.data, f[0].data)
+            for j in range(N):
+                f[0, :, j] = optimize.nnls(K, X[:, j].squeeze())[0]
+            res = X - np.dot(K, f[0])
             RSS[0] = np.sum(res**2)
             SM[0] = np.linalg.norm(np.dot(np.dot(np.transpose(f[0]), S), f[0]))
 
-            msg = "-->  residuals = {:.2e}    curvature = {:.2e}".format(RSS[0], SM[0])
-            _log += msg
+            msg = f"-->  residuals = {RSS[0]:.2e}    curvature = {SM[0]:.2e}"
             info_(msg)
 
         else:  # regularization
             # some matrices used for QP optimization do not depend on lambdaR
             # and are computed here. The standard form used by quadprog() is
             # minimize (1/2) xT G x - aT x ; subject to: C.T x >= b
 
-            # The first part of the G matrix is independent of lambda:  G = G0 + 2 * lambdaR S
-            G0 = 2 * np.dot(K.data.T, K.data)
-            a = 2 * np.dot(X.data.T, K.data)
-            C = np.eye(len(q))
-            b = np.zeros(len(q))
+            # The first part of the G matrix is independent of lambda:
+            #     G = G0 + 2 * lambdaR S
+            G0 = 2 * np.dot(K.T, K)
+            a = 2 * np.dot(X.T, K)
+            C = np.eye(M)
+            b = np.zeros(M)
 
-            def solve_for_reg_par(X, K, G0, reg_par, S):
+            # --------------------------------------------------------------------------
+            def solve_for_lambda(X, K, G0, lamda, S):
                 """
                 QP optimization
 
                 parameters:
                 -----------
                 X: NDDataset of experimental spectra
                 K: NDDataset, kernel datase
                 G0: the lambda independent part of G
-                reg_par: regularization parameter
+                lamda: regularization parameter
                 S: penalty function (shaprness)
                 verbose: print info
 
                 returns:
                 --------
                 f, RSS and SM for a given regularization parameter
                 """
-                global _log
-
-                fi = np.zeros((len(q), len(channels.data)))
-
+                M, N, _ = K.shape[-1], X.shape[-1], X.shape[0]
+                fi = np.zeros((M, N))
+                channels = self._channels
                 for j, channel in enumerate(channels.data):
                     try:
-                        G = G0 + 2 * reg_par * S
+                        G = G0 + 2 * lamda * S
                         fi[:, j] = quadprog.solve_qp(G, a[j].squeeze(), C, b)[0]
                     except ValueError:  # pragma: no cover
-                        msg = f"Warning:G is not positive definite for log10(lambda)={np.log10(reg_par):.2f} at {channel:.2f} {channels.units}, find nearest PD matrix"
+                        msg = (
+                            f"Warning:G is not positive definite for log10(lambda)="
+                            f"{np.log10(lamda):.2f} at {channel:.2f} "
+                            f"{channels.units}, find nearest PD matrix"
+                        )
                         warning_(msg)
-                        _log += msg
                         try:
-                            G = _nearestPD(G0 + 2 * reg_par * S, 0)
+                            G = _nearestPD(G0 + 2 * lamda * S, 0)
                             fi[:, j] = quadprog.solve_qp(G, a[j].squeeze(), C, b)[0]
                         except ValueError:
                             msg = (
                                 "... G matrix is still ill-conditioned, "
                                 "try with a small shift of diagonal elements..."
                             )
                             warning_(msg)
-                            _log += msg
-                            G = _nearestPD(G0 + 2 * reg_par * S, 1e-3)
+                            G = _nearestPD(G0 + 2 * lamda * S, 1e-3)
                             fi[:, j] = quadprog.solve_qp(G, a[j].squeeze(), C, b)[0]
 
                 resi = X.data - np.dot(K.data, fi)
                 RSSi = np.sum(resi**2)
                 SMi = np.linalg.norm(np.dot(np.dot(np.transpose(fi), S), fi))
 
                 msg = (
-                    f"log10(lambda)={np.log10(reg_par):.3f} -->  residuals = {RSSi:.3e}    "
-                    f"regularization constraint  = {SMi:.3e}\n"
+                    f"log10(lambda)={np.log10(lamda):.3f} -->  "
+                    f"residuals = {RSSi:.3e}    "
+                    f"regularization constraint  = {SMi:.3e}"
                 )
                 info_(msg)
-                _log += msg
 
                 return fi, RSSi, SMi
 
-            if not search_reg:
+            # --------------------------------------------------------------------------
+
+            if not self._search_reg:
                 msg = (
                     f"Solving for {X.shape[1]} channels, {X.shape[0]} observations and "
-                    f"{len(reg_par)} regularization parameters \n"
+                    f"{len(lambdas)} regularization parameters"
                 )
                 info_(msg)
-                _log += msg
 
-                for i, lamda_ in enumerate(reg_par):
-                    f[i], RSS[i], SM[i] = solve_for_reg_par(X, K, G0, lamda_, S)
+                for i, lamda_ in enumerate(lambdas):
+                    f[i], RSS[i], SM[i] = solve_for_lambda(X, K, G0, lamda_, S)
 
             else:
                 msg = (
-                    f"Solving for {X.shape[1]} channel(s) and {X.shape[0]} observations, search "
-                    f"optimum regularization parameter in the range: [10**{min(reg_par)}, 10**{max(reg_par)}]\n"
+                    f"Solving for {X.shape[1]} channel(s) and {X.shape[0]} "
+                    f"observations, search optimum regularization parameter "
+                    f"in the range: [10**{min(lambdas)}, 10**{max(lambdas)}]"
                 )
                 info_(msg)
-                _log += msg
 
                 x = np.zeros(4)
                 epsilon = 0.1
                 phi = (1 + np.sqrt(5)) / 2
 
-                x[0] = min(reg_par)
-                x[3] = max(reg_par)
+                x[0] = min(lambdas)
+                x[3] = max(lambdas)
                 x[1] = (x[3] + phi * x[0]) / (1 + phi)
                 x[2] = x[0] + x[3] - x[1]
-                reg_par = 10**x
+                lambdas = 10**x
                 msg = "Initial Log(lambda) values = " + str(x)
                 info_(msg)
-                _log += msg
 
                 for i, xi in enumerate(x):
-                    f[i], RSS[i], SM[i] = solve_for_reg_par(X, K, G0, 10**xi, S)
+                    f[i], RSS[i], SM[i] = solve_for_lambda(X, K, G0, 10**xi, S)
 
                 Rx = np.copy(RSS)
                 Sy = np.copy(SM)
                 while "convergence not reached":
                     C1 = _menger(np.log10(Rx[0:3]), np.log10(Sy[0:3]))
                     C2 = _menger(np.log10(Rx[1:4]), np.log10(Sy[1:4]))
-                    msg = f"Curvatures of the inner points: C1 = {C1:.3f} ; C2 = {C2:.3f} \n"
+                    msg = (
+                        f"Curvatures of the inner points: C1 = {C1:.3f} ;"
+                        f" C2 = {C2:.3f}"
+                    )
                     info_(msg)
-                    _log += msg
 
                     while "convergence not reached":
                         x[3] = x[2]
                         Rx[3] = Rx[2]
                         Sy[3] = Sy[2]
                         x[2] = x[1]
                         Rx[2] = Rx[1]
                         Sy[2] = Sy[1]
                         x[1] = (x[3] + phi * x[0]) / (1 + phi)
                         msg = "New range of Log(lambda) values: " + str(x)
                         info_(msg)
-                        _log += msg
 
-                        f_, Rx[1], Sy[1] = solve_for_reg_par(X, K, G0, 10 ** x[1], S)
-                        reg_par = np.append(reg_par, np.array(10 ** x[1]))
+                        f_, Rx[1], Sy[1] = solve_for_lambda(X, K, G0, 10 ** x[1], S)
+                        lambdas = np.append(lambdas, np.array(10 ** x[1]))
                         f = np.concatenate((f, np.atleast_3d(f_.T).T))
                         RSS = np.concatenate((RSS, np.array(Rx[1:2])))
                         SM = np.concatenate((SM, np.array(Sy[1:2])))
                         C2 = _menger(np.log10(Rx[1:4]), np.log10(Sy[1:4]))
                         msg = f"new curvature: C2 = {C2:.3f}"
                         info_(msg)
-                        _log += msg
 
                         if C2 > 0:
                             break
 
                     if C1 > C2:
                         x_ = x[1]
                         C_ = C1
@@ -502,196 +644,234 @@
                         Sy[3] = Sy[2]
                         x[2] = x[1]
                         Rx[2] = Rx[1]
                         Sy[2] = Sy[1]
                         x[1] = (x[3] + phi * x[0]) / (1 + phi)
                         msg = "New range (Log lambda): " + str(x)
                         info_(msg)
-                        _log += msg
-                        f_, Rx[1], Sy[1] = solve_for_reg_par(X, K, G0, 10 ** x[1], S)
+                        f_, Rx[1], Sy[1] = solve_for_lambda(X, K, G0, 10 ** x[1], S)
                         f = np.concatenate((f, np.atleast_3d(f_.T).T))
-                        reg_par = np.append(reg_par, np.array(10 ** x[1]))
+                        lambdas = np.append(lambdas, np.array(10 ** x[1]))
                         RSS = np.concatenate((RSS, np.array(Rx[1:2])))
                         SM = np.concatenate((SM, np.array(Sy[1:2])))
                     else:
                         x_ = x[2]
                         C_ = C2
                         x[0] = x[1]
                         Rx[0] = Rx[1]
                         Sy[0] = Sy[1]
                         x[1] = x[2]
                         Rx[1] = Rx[2]
                         Sy[1] = Sy[2]
                         x[2] = x[0] - (x[1] - x[3])
                         msg = "New range (Log lambda):" + str(x)
                         info_(msg)
-                        _log += msg
-                        f_, Rx[2], Sy[2] = solve_for_reg_par(X, K, G0, 10 ** x[2], S)
+                        f_, Rx[2], Sy[2] = solve_for_lambda(X, K, G0, 10 ** x[2], S)
                         f = np.concatenate((f, np.atleast_3d(f_.T).T))
-                        reg_par = np.append(reg_par, np.array(10 ** x[2]))
+                        lambdas = np.append(lambdas, np.array(10 ** x[2]))
                         RSS = np.concatenate((RSS, np.array(Rx[1:2])))
                         SM = np.concatenate((SM, np.array(Sy[1:2])))
                     if (10 ** x[3] - 10 ** x[0]) / 10 ** x[3] < epsilon:
                         break
-                id_opt = np.argmin(np.abs(reg_par - np.power(10, x_)))
-                id_opt_ranked = np.argmin(np.abs(np.argsort(reg_par) - id_opt))
-                msg = f"\n optimum found: index = {id_opt_ranked} ; Log(lambda) = {x_:.3f} ; lambda = {np.power(10, x_):.5e} ; curvature = {C_:.3f}"
+                id_opt = np.argmin(np.abs(lambdas - np.power(10, x_)))
+                id_opt_ranked = np.argmin(np.abs(np.argsort(lambdas) - id_opt))
+                msg = (
+                    f" optimum found: index = {id_opt_ranked} ; "
+                    f"Log(lambda) = {x_:.3f} ; "
+                    f"lambda = {np.power(10, x_):.5e} ; curvature = {C_:.3f}"
+                )
                 info_(msg)
-                _log += msg
 
             # sort by lamba values
-            argsort = np.argsort(reg_par)
-            reg_par = reg_par[argsort]
+            argsort = np.argsort(lambdas)
+            lambdas = lambdas[argsort]
             RSS = RSS[argsort]
             SM = SM[argsort]
             f = f[argsort]
 
-        msg = "\n Done."
-        info_(msg)
-        _log += msg
-
-        f = NDDataset(f)
-        f.name = "2D distribution functions"
-        f.title = "density"
-        f.history = "2D IRIS analysis of {} dataset".format(X.name)
-        f.set_coordset(z=Coord(data=reg_par, title="lambda"), y=q.copy(), x=channels)
-        self.f = f
-        self.K = K
-        self.X = X
-        self.reg_par = reg_par
-        self.RSS = RSS
-        self.SM = SM
-        self.log = _log
+        info_("Done.")
+
+        self._lambdas.data = lambdas
+        _outfit = f, RSS, SM
+        return _outfit
+
+    # ----------------------------------------------------------------------------------
+    # Public methods and property
+    # ----------------------------------------------------------------------------------
+    @property
+    def f(self):
+        if self._X_is_missing:
+            raise NotFittedError
+
+        f = self._outfit[0]
+        f = NDDataset(f, name="2D distribution functions", title="density")
+        f.history = "2D IRIS analysis of {X.name} dataset"
+        f.set_coordset(z=self._lambdas, y=self._q, x=self._channels)
+        if np.any(self._X_mask):
+            # restore masked column if necessary
+            f = self._restore_masked_data(f, axis=-1)
+        return f
+
+    @property
+    def K(self):
+        return self._Y  # Todo: eventuallly restore row mask
+
+    @property
+    def q(self):
+        return self._q
+
+    @property
+    def lambdas(self):
+        return self._lambdas
+
+    @property
+    def RSS(self):
+        return self._outfit[1]
+
+    @property
+    def SM(self):
+        return self._outfit[2]
 
-    def reconstruct(self):
+    def inverse_transform(self):  # override the decomposition method
         """
         Transform data back to the original space.
 
-        The following matrix operation is performed : :math:`\\hat{X} = K.f[i]`
+        The following matrix operation is performed : :math:`\hat{X} = K.f[i]`
         for each value of the regularization parameter.
 
         Returns
         -------
-            NDDataset
-                The reconstructed dataset.
+        `~spectrochempy.core.dataset.nddataset.NDDataset`
+            The reconstructed dataset.
         """
+        if not self._fitted:
+            raise NotFittedError("The fit method must be used before using this method")
 
-        if len(self.reg_par) == 1:  # no regularization or single lambda
-            X_hat = NDDataset(
-                np.zeros((self.X.shape)), title=self.X.title, units=self.X.units
-            )
-            X_hat.set_coordset(y=self.X.y, x=self.X.x)
-            X_hat.data = np.dot(self.K.data, self.f.data.squeeze(axis=0))
+        lambdas = self._lambdas.data
+        X = self.X
+        K = self._Y
+        f = self.f
+
+        if len(lambdas) == 1:  # no regularization or single lambda
+            X_hat = NDDataset(np.zeros((X.shape)), title=X.title, units=X.units)
+            X_hat.set_coordset(y=X.y, x=X.x)
+            X_hat.data = np.dot(K.data, f.data.squeeze(axis=0))
         else:
             X_hat = NDDataset(
-                np.zeros((self.f.z.size, *self.X.shape)),
-                title=self.X.title,
-                units=self.X.units,
+                np.zeros((f.z.size, *X.shape)),
+                title=X.title,
+                units=X.units,
             )
-            X_hat.set_coordset(z=self.f.z, y=self.X.y, x=self.X.x)
+            X_hat.set_coordset(z=f.z, y=X.y, x=X.x)
             for i in range(X_hat.z.size):
-                X_hat.data[i] = np.dot(self.K.data, self.f[i].data.squeeze(axis=0))
+                X_hat.data[i] = np.dot(K.data, f[i].data.squeeze(axis=0))
 
         X_hat.name = "2D-IRIS Reconstructed datasets"
         return X_hat
 
     def plotlcurve(self, scale="ll", title="L curve"):
         """
-        Plot the L Curve.
+        Plot the ``L-Curve``\ .
 
         Parameters
         ----------
-        scale : str, optional, default='ll'
-            String of 2 letters among 'l' (log) or 'n' (non-log) indicating whether the y and x
-            axes should be log scales.
-        title : str, optional, default='L curve'
+        scale : `str`\ , optional, default: ``'ll'``
+            String of 2 letters among ``'l'``\ (log) or ``'n'``\ (non-log) indicating
+            whether the ``y`` and ``x`` axes should be log scales.
+        title : `str`, optional, default: ``'L-curve'``
             Plot title.
 
         Returns
         -------
-            matplotlib.pyplot.axes
-                The axes.
+        `~matplotlib.axes.Axes`
+                The matplotlib axe.
         """
+        if not self._fitted:
+            raise NotFittedError("The fit method must be used before using this method")
 
         fig = plt.figure()
         ax = fig.add_subplot(111)
-        ax.set_title("L curve")
+        ax.set_title(title)
         plt.plot(self.RSS, self.SM, "o")
         ax.set_xlabel("Residuals")
         ax.set_ylabel("Curvature")
         if scale[1] == "l":
             ax.set_xscale("log")
         if scale[0] == "l":
             ax.set_yscale("log")
         return ax
 
+    @_docstring.dedent
     def plotmerit(self, index=None, **kwargs):
         """
         Plot the input dataset, reconstructed dataset and residuals.
 
         Parameters
         ----------
-        index : int, list or tuple of int, optional, default: None
-            Index(es) of the inversions (i.e. of the lambda values) to consider.
-            If 'None': plots for all indices.
-
-        **kwargs
-            Keywords arguments passed to the plot() function.
+        index : `int`\ , `list` or `tuple` of `int`\ , optional, default: `None`
+            Index(es) of the inversions (*i.e.,* of the lambda values) to consider.
+            If `None` plots for all indices.
+        %(kwargs)s
+
+        Other Parameters
+        ----------------
+        %(plotmerit.other_parameters)s
 
         Returns
         -------
-            list of axes
-                The axes.
+        `list` of `~matplotlib.axes.Axes`
+            Subplots.
         """
-
-        colX, colXhat, colRes = kwargs.get("colors", ["blue", "green", "red"])
-
-        X_hat = self.reconstruct()
+        X = self.X
+        X_hat = self.inverse_transform()
         axeslist = []
         if index is None:
-            index = range(len(self.reg_par))
+            index = range(len(self._lambdas))
         if type(index) is int:
             index = [index]
 
         for i in index:
             if X_hat.ndim == 3:  # if several lambda
                 X_hat_ = X_hat[i].squeeze()
             else:
                 X_hat_ = X_hat  # if single lambda or no regularization
-            res = self.X - X_hat_
-            ax = self.X.plot()
-            ax.plot(self.X.x.data, X_hat_.squeeze().T.data, "-", color=colXhat)
-            ax.plot(self.X.x.data, res.T.data, "-", color=colRes)
-            ax.set_title(f"2D IRIS merit plot, $\lambda$ = {self.reg_par[i]:.2e}")
+
+            ax = super().plotmerit(X, X_hat_, **kwargs)
+
+            ax.set_title(
+                f"2D IRIS merit plot, $\lambda$ = {self._lambdas[i].value:.2e}"
+            )
             axeslist.append(ax)
+
         return axeslist
 
     def plotdistribution(self, index=None, **kwargs):
         """
         Plot the distribution function.
 
-        This fucntion plots the distribution function f of the IRIS object.
+        This function plots the distribution function f of the `IRIS` object.
 
         Parameters
         ----------
-        index : optional, int, list or tuple of int. default: None
-            Index(es) of the inversions (i.e. of the regularization parameter) to consider.
-            If 'None': plots for all indices.
+        index : `int` , `list` or `tuple` of `int`, optional, default: `None`
+            Index(es) of the inversions (i.e. of the :term:`regularization` parameter)
+            to consider.
+            If `None`, plots for all indices.
         **kwargs
             Other optional arguments are passed in the plots.
 
         Returns
         -------
-            List of axes
-                The axes.
+        `list` of `~matplotlib.axes.Axes`
+            Subplots.
         """
 
         axeslist = []
         if index is None:
-            index = range(len(self.reg_par))
+            index = range(len(self._lambdas))
         if type(index) is int:
             index = [index]
         for i in index:
             axeslist.append(self.f[i].plot(method="map", **kwargs))
         return axeslist
 
 
@@ -701,14 +881,17 @@
 
 def _menger(x, y):
     """
     returns the Menger curvature of a triplet of
     points. x, y = sets of 3 cartesian coordinates
     """
     numerator = 2 * (((x[1] - x[0]) * (y[2] - y[1])) - ((y[1] - y[0]) * (x[2] - x[1])))
+    if abs(numerator) <= EPSILON:
+        return 0.0
+
     # euclidian distances
     r01 = (x[1] - x[0]) ** 2 + (y[1] - y[0]) ** 2
     r12 = (x[2] - x[1]) ** 2 + (y[2] - y[1]) ** 2
     r02 = (x[2] - x[0]) ** 2 + (y[2] - y[0]) ** 2
 
     denominator = np.sqrt(r01 * r12 * r02)
     return numerator / denominator
@@ -737,15 +920,15 @@
     S[m - 2, m - 3] = -4
     S[m - 2, m - 2] = 6
     S[m - 2, m - 1] = -4
     S[m - 1, m - 3] = 1
     S[m - 1, m - 2] = -4
     S[m - 1, m - 1] = 6
 
-    S = ((q.data[m - 1] - q.data[0]) / (m - 1)) ** (-3) * S
+    S = ((q[m - 1] - q[0]) / (m - 1)) ** (-3) * S
     return S
 
 
 def _nearestPD(A, shift):  # pragma: no cover
     """
     Find the nearest positive-definite matrix to input.
 
@@ -773,16 +956,16 @@
     if _isPD(A3):
         return A3
 
     spacing = np.spacing(np.linalg.norm(A))
     # The above is different from [1]. It appears that MATLAB's `chol` Cholesky
     # decomposition will accept matrices with exactly 0-eigenvalue, whereas
     # Numpy's will not. So where [1] uses `eps(mineig)` (where `eps` is Matlab
-    # for `np.spacing`), we use the above definition. CAVEAT: our `spacing`
-    # will be much larger than [1]'s `eps(mineig)`, since `mineig` is usually on
+    # for `np.spacing` ), we use the above definition. CAVEAT: our `spacing`
+    # will be much larger than [1]'s `eps(mineig)` , since `mineig` is usually on
     # the order of 1e-16, and `eps(1e-16)` is on the order of 1e-34, whereas
     # `spacing` will, for Gaussian random matrices of small dimension, be on
     # the order of 1e-16. In practice, both ways converge, as the unit test
     # below suggests.
     Ie = np.eye(A.shape[0])
     k = 1
     while not _isPD(A3):
@@ -801,7 +984,12 @@
     """
 
     try:
         _ = np.linalg.cholesky(B)
         return True
     except np.linalg.LinAlgError:
         return False
+
+
+# ======================================================================================
+if __name__ == "__main__":
+    pass
```

### Comparing `spectrochempy-0.5.5/spectrochempy/analysis/lstsq.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/filter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,351 +1,234 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
-# TODO: create tests
+__all__ = ["savgol_filter", "detrend"]
 
-__all__ = ["CurveFit", "LSTSQ", "NNLS"]
+__dataset_methods__ = __all__
 
-import numpy as np
-import scipy.linalg as lng
-import scipy.optimize as sopt
-from traitlets import HasTraits, Instance
+import scipy.signal
 
-from spectrochempy.core.dataset.baseobjects.ndarray import NDArray
-from spectrochempy.core.dataset.nddataset import NDDataset
-from spectrochempy.core.units import Quantity
-from spectrochempy.utils.traits import NDDatasetType
+"""wrappers of scipy.signal filters, """
 
 
-class LSTSQ(HasTraits):
-    """
-    Least-squares solution to a linear matrix equation.
-
-    Given a vector `X` and a vector Y, the equation `A.X + B = Y` is solved by
-    computing  ``A``, and ``B`` that minimizes the Euclidean 2-norm
-    `|| Y - (A.X + B) ||^2`.
-
-    Parameters
-    ----------
-    *datasets : one or two |NDDataset|'s or array-like objects
-        If a single dataset `Y` is provided, the `X` data will be the `x`
-        coordinates of the `Y` dataset, or the index of the data if not
-        coordinates exists.
-        If two datasets `X`, and `Y` are given, the `x` coordinates of `Y`
-        are ignored and replaced by the `X` data.
-    """
-
-    X = Instance(NDArray)
-    Y = NDDatasetType()
-
-    def __init__(self, *datasets):
-
-        super().__init__()
-
-        if len(datasets) > 2 or len(datasets) < 1:
-            raise ValueError("one or two dataset at max are expected")
-
-        if len(datasets) == 2:
-            X, Y = datasets
-
-        else:  # nb dataset ==1
-            # abscissa coordinates are the X
-            dim = datasets[0].dims[-1]
-            X = getattr(datasets[0], dim)
-
-            Y = datasets[0]
-
-        self.X = X
-        self.Y = Y
-
-        Xdata = np.vstack([X.data, np.ones(len(X.data))]).T
-        Ydata = Y.data
-
-        P, res, rank, s = lng.lstsq(Xdata, Ydata)
-
-        self._P = P
-        self._res = res
-        self._rank = rank
-        self._s = s
-
-    def transform(self):
-        """
-        Return the least square coefficients A and B.
-
-        Returns
-        -------
-        Quantity or NDDataset, depending on the dimension of the linear system.
-        """
-        P = self._P
-        X = self.X
-        Y = self.Y
-
-        if P.shape == (2,):
-            # this is the result of the single equation, so only one value
-            # should be returned
-            A = P[0] * Y.units / X.units
-            B = P[1] * Y.units
-
-        else:
-            A = NDDataset(
-                data=P[0],
-                units=Y.units / X.units,
-                title="%s/%s" % (Y.title, X.title),
-            )
-            B = NDDataset(
-                data=P[1] * np.ones(X.size),
-                units=Y.units,
-                title="%s at origin" % Y.title,
-            )
-
-            A.history = "Computed by spectrochempy.lstsq \n"
-            B.history = "Computed by spectrochempy.lstsq \n"
-
-        return A, B
-
-    trans = transform  # short-cut
-
-    def inverse_transform(self):
-        """
-        Return the reconstructed data from the A and B least-square
-        coefficients.
-
-        Returns
-        -------
-        |NDDataset|
-        """
-        A, B = self.transform()
-
-        if isinstance(A, Quantity):
-            Yp = self.Y.copy()
-            Yp.data = (self.X * A + B).data
-        else:
-            Yp = A * self.X + B
-        return Yp
+# Todo:
+# find_peaks_cwt(vector, widths[, wavelet, ...]) Attempt to find the peaks in a 1-D array.
+# argrelmin(data[, axis, order, mode]) 	Calculate the relative minima of data.
+# argrelmax(data[, axis, order, mode]) 	Calculate the relative maxima of data.
+# argrelextrema(data, comparator[, axis, ...]) 	Calculate the relative extrema of data.
 
-    itrans = inverse_transform
 
-
-class NNLS(HasTraits):
+def savgol_filter(
+    dataset,
+    window_length=5,
+    polyorder=0,
+    deriv=0,
+    delta=1.0,
+    mode="interp",
+    cval=0.0,
+    **kwargs,
+):
     """
-    Least-squares solution to a linear matrix equation with non-negativity constraints.
+    Apply a Savitzky-Golay filter to a NDDataset.
 
-    This is a wrapper to the `scipy.optimize.nnls`` function.
+    Wrapper of scpy.signal.savgol(). If dataset has dimension greater than 1,
+    dim determines the axis along which the filter is applied.
 
     Parameters
     ----------
-    *datasets : one or two |NDDataset|'s or array-like objects
-        If a single dataset `Y` is provided, the `X` data will be the `x`
-        coordinates of the `Y` dataset, or the index of the data if not
-        coordinates exists.
-        If two datasets `X`, and `Y` are given, the `x` coordinates of `Y`
-        are ignored and replaced by the `X` data.
-    maxiter: int, optional
-        Maximum number of iterations, optional.
-        Default is ``3 * X.shape``.
-    """
-
-    X = Instance(NDArray)
-    Y = NDDatasetType()
-
-    def __init__(self, *datasets):
-
-        super().__init__()
+    dataset : `NDDataset`
+        The dataset to be filtered. If dataset.data is not a single or double precision
+        floating point array, it will be converted to type numpy.float64 before
+        filtering.
+    window_length : int
+        The length of the filter window (i.e. the number of coefficients).
+        window_length must be a positive odd integer.
+    polyorder : int
+        The order of the polynomial used to fit the NDDataset. `polyorder` must be less
+        than window_length.
+    deriv : int, optional
+        The order of the derivative to compute. This must be a non-negative integer.
+        The default is 0, which means to filter the data without differentiating.
+    delta : float, optional
+        The spacing of the samples to which the filter will be applied. This is only
+        used if deriv > 0. Default is 1.0.
+    mode : str, optional
+        Must be ‘mirror’, ‘constant’, ‘nearest’, ‘wrap’ or ‘interp’. This determines
+        the type of extension to use for
+        the padded signal to which the filter is applied. When mode is ‘constant’,
+        the padding value is given by cval.
+        See :py:scipy.signal.savgol_filter: for more details on ‘mirror’, ‘constant’,
+        ‘wrap’, and ‘nearest’.
+        When the ‘interp’ mode is selected (the default), no extension is used.
+        Instead, a degree polyorder polynomial is fit to the last window_length values
+        of the edges, and this polynomial is used to evaluate the
+        last window_length // 2 output values.
+    cval : scalar, optional
+        Value to fill past the edges of the input if mode is ‘constant’. Default is 0.0.
+    **kwargs
+        Optional keyword parameters (see Other Parameters).
+
+    Returns
+    -------
+    NDDataset
+        The filtered data with same shape as x. data units are removed when deriv > 1.
+
+    Other Parameters
+    ----------------
+    dim : str or int, optional, default='x'
+        Specify on which dimension to apply this method. If `dim` is specified as an
+        integer it is equivalent to the usual `axis` numpy parameter.
+    inplace : bool, optional, default=False
+        True if we make the transform inplace.  If False, the function return a new
+        object.
+
+    Notes
+    -----
+    Even spacing of the axis coordinates is NOT checked. Be aware that Savitzky-Golay
+    algorithm is based on indexes, not on coordinates.
+
+    Details on the `mode` options:
+
+    * `mirror` :
+      Repeats the values at the edges in reverse order.  The value
+      closest to the edge is not included.
+    * `nearest` :
+      The extension contains the nearest input value.
+    * `constant` :
+      The extension contains the value given by the `cval` argument.
+    * `wrap` :
+      The extension contains the values from the other end of the array.
+
+    For example, if the input is [1, 2, 3, 4, 5, 6, 7, 8], and
+    `window_length` is 7, the following shows the extended data for
+    the various `mode` options (assuming `cval` is 0)
+
+    +------------+----------+------------------------+---------+
+    | Mode       |   Ext    |         Input          |   Ext   |
+    +============+==========+========================+=========+
+    | 'mirror'   | 4  3  2  | 1  2  3  4  5  6  7  8 | 7  6  5 |
+    +------------+----------+------------------------+---------+
+    | 'nearest'  | 1  1  1  | 1  2  3  4  5  6  7  8 | 8  8  8 |
+    +------------+----------+------------------------+---------+
+    | 'constant' | 0  0  0  | 1  2  3  4  5  6  7  8 | 0  0  0 |
+    +------------+----------+------------------------+---------+
+    | 'wrap'     | 6  7  8  | 1  2  3  4  5  6  7  8 | 1  2  3 |
+    +------------+----------+------------------------+---------+
+
+
+    See Also
+    ---------
+    smooth : Smooth the data using a window with requested size.
+
+    Examples
+    --------
+
+    >>> dataset = scp.read('irdata/nh4y-activation.spg')
+    >>> dataset.savgol_filter(window_length=5, polyorder=0)
+    NDDataset: [float64] a.u. (shape: (y:55, x:5549))
+    """
+
+    new = dataset.copy() if not kwargs.pop("inplace", False) else dataset
+
+    is_ndarray = False
+    axis = kwargs.pop("dim", kwargs.pop("axis", -1))
+    if hasattr(new, "get_axis"):
+        axis, dim = new.get_axis(axis, negative_axis=True)
+        data = new.data
+    else:
+        is_ndarray = True
+        data = new
+
+    data = scipy.signal.savgol_filter(
+        data, window_length, polyorder, deriv, delta, axis, mode, cval
+    )
+
+    if not is_ndarray:
+        if deriv != 0 and dataset.coord(dim).reversed:
+            data = data * (-1) ** deriv
+        new.data = data
+    else:
+        new = data
+
+    if not is_ndarray:
+        new.history = (
+            f"savgol_filter applied (window_length={window_length}, "
+            f"polyorder={polyorder}, deriv={deriv}, delta={delta}, mode={mode}, "
+            f"cval={cval}"
+        )
+    return new
 
-        if len(datasets) > 2 or len(datasets) < 1:
-            raise ValueError("one or two dataset at max are expected")
-
-        if len(datasets) == 2:
-            X, Y = datasets
-
-        else:  # nb dataset ==1
-            # abscissa coordinates are the X
-            dim = datasets[0].dims[-1]
-            X = getattr(datasets[0], dim)
-
-            Y = datasets[0]
-
-        self.X = X
-        self.Y = Y
-
-        Xdata = np.vstack([X.data, np.ones(len(X.data))]).T
-        Ydata = Y.data
-
-        P, res = sopt.nnls(Xdata, Ydata, maxiter=None)
-
-        self._P = P
-        self._res = res
-
-    def transform(self):
-        """
-        Return the least square coefficients A and B.
-
-        Returns
-        -------
-        Coefficient
-            Quantity or NDDataset, depending on the dimension of the linear system.
-        """
-        P = self._P
-        X = self.X
-        Y = self.Y
-
-        if P.shape == (2,):
-            # this is the result of the single equation, so only one value
-            # should be returned
-            A = P[0] * Y.units / X.units
-            B = P[1] * Y.units
-
-        else:
-            A = NDDataset(
-                data=P[0],
-                units=Y.units / X.units,
-                title="%s/%s" % (Y.title, X.title),
-            )
-            B = NDDataset(
-                data=P[1] * np.ones(X.size),
-                units=Y.units,
-                title="%s at origin" % Y.title,
-            )
-
-            A.history = "Computed by spectrochempy.lstsq \n"
-            B.history = "Computed by spectrochempy.lstsq \n"
-
-        return A, B
-
-    trans = transform  # short-cut
-
-    def inverse_transform(self):
-        """
-        Return the reconstructed data from the A and B least-square
-        coefficients.
-
-        Returns
-        -------
-        dataset
-            |NDDataset| .
-        """
-        A, B = self.transform()
-
-        if isinstance(A, Quantity):
-            Yp = self.Y.copy()
-            Yp.data = (self.X * A + B).data
-        else:
-            Yp = A * self.X + B
-        return Yp
 
-    itrans = inverse_transform
-
-
-class CurveFit(HasTraits):
+def detrend(dataset, type="linear", bp=0, **kwargs):
     """
-    Use non-linear least squares to fit a function, ``f``, to data.
-
-    It assumes Y = f(X, *params) + eps.
+    Remove linear trend along dim from dataset.
 
-    This is a wrapper to the `scipy.optimize.curve_fit`` function
+    Wrapper of scpy.signal.detrend().
 
     Parameters
     ----------
-    *datasets : one or two |NDDataset|'s or array-like objects
-        If a single dataset `Y` is provided, the `X` data will be the `x`
-        coordinates of the `Y` dataset, or the index of the data if not
-        coordinates exists.
-        If two datasets `X`, and `Y` are given, the `x` coordinates of `Y`
-        are ignored and replaced by the `X` data.
-    maxiter: int, optional
-        Maximum number of iterations, optional.
-        Default is ``3 * X.shape``.
-    """
-
-    # TODO: Something wrong here! This is exactly the same code as NNLS.
-    # Probably a mistake to correct...
+    dataset :  `NDDataset`
+        The input data.
+    type : str among ['linear', 'constant'}, optional, default='linear'
+        The type of detrending. If `type == 'linear'` (default),
+        the result of a linear least-squares fit to `data` is subtracted from `data` .
+        If `type == 'constant'` , only the mean of `data` is subtracted.
+    bp : array_like of ints, optional
+        A sequence of break points. If given, an individual linear fit is
+        performed for each part of `data` between two break points.
+        Break points are specified as indices into `data` .
+    **kwargs
+        Optional keyword parameters (see Other Parameters).
+
+    Returns
+    -------
+    detrended
+        The detrended `NDDataset` .
+
+    Other Parameters
+    ----------------
+    dim : str or int, optional, default='x'.
+        Specify on which dimension to apply this method. If `dim` is specified as an
+        integer it is equivalent to the usual `axis` numpy parameter.
+    inplace : bool, optional, default=False.
+        True if we make the transform inplace.  If False, the function return a new
+        object
+
+    See Also
+    --------
+    BaselineCorrection : Manual baseline correction.
+    abs : Automatic baseline correction.
+    autosub : Subtraction of reference.
+
+    Examples
+    --------
+
+    >>> dataset = scp.read("irdata/nh4y-activation.spg")
+    >>> dataset.detrend(type='constant')
+    NDDataset: [float64] a.u. (shape: (y:55, x:5549))
+    """
+    if not kwargs.pop("inplace", False):
+        # default
+        new = dataset.copy()
+    else:
+        new = dataset
+
+    is_ndarray = False
+    axis = kwargs.pop("dim", kwargs.pop("axis", -1))
+    if hasattr(new, "get_axis"):
+        axis, dim = new.get_axis(axis, negative_axis=True)
+        data = new.data
+    else:
+        is_ndarray = True
+        data = new
 
-    X = Instance(NDArray)
-    Y = NDDatasetType()
+    data = scipy.signal.detrend(data, axis=axis, type=type, bp=bp)
 
-    def __init__(self, *datasets):
+    if is_ndarray:
+        return data
 
-        super().__init__()
-
-        if len(datasets) > 2 or len(datasets) < 1:
-            raise ValueError("one or two dataset at max are expected")
-
-        if len(datasets) == 2:
-            X, Y = datasets
-
-        else:  # nb dataset ==1
-            # abscissa coordinates are the X
-            dim = datasets[0].dims[-1]
-            X = getattr(datasets[0], dim)
-
-            Y = datasets[0]
-
-        self.X = X
-        self.Y = Y
-
-        Xdata = np.vstack([X.data, np.ones(len(X.data))]).T
-        Ydata = Y.data
-
-        P, res = sopt.nnls(Xdata, Ydata, maxiter=None)
-
-        self._P = P
-        self._res = res
-
-    def transform(self):
-        """
-        Return the least square coefficients A and B.
-
-        Returns
-        -------
-        Quantity or NDDataset, depending on the dimension of the linear system.
-        """
-        P = self._P
-        X = self.X
-        Y = self.Y
-
-        if P.shape == (2,):
-            # this is the result of the single equation, so only one value
-            # should be returned
-            A = P[0] * Y.units / X.units
-            B = P[1] * Y.units
-
-        else:
-            A = NDDataset(
-                data=P[0],
-                units=Y.units / X.units,
-                title="%s/%s" % (Y.title, X.title),
-            )
-            B = NDDataset(
-                data=P[1] * np.ones(X.size),
-                units=Y.units,
-                title="%s at origin" % Y.title,
-            )
-
-            A.history = "Computed by spectrochempy.lstsq \n"
-            B.history = "Computed by spectrochempy.lstsq \n"
-
-        return A, B
-
-    trans = transform  # short-cut
-
-    def inverse_transform(self):
-        """
-        Return the reconstructed data from the A and B least-square
-        coefficients.
-
-        Returns
-        -------
-        |NDDataset|
-        """
-        A, B = self.transform()
-
-        if isinstance(A, Quantity):
-            Yp = self.Y.copy()
-            Yp.data = (self.X * A + B).data
-        else:
-            Yp = A * self.X + B
-        return Yp
+    new.data = data
 
-    itrans = inverse_transform
+    return new
```

### Comparing `spectrochempy-0.5.5/spectrochempy/analysis/mcrals.py` & `spectrochempy-0.6.1/spectrochempy/core/dataset/coord.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,775 +1,1082 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
-This module implements the MCRALS class.
+This module implements the class  `Coord` .
 """
 
-__all__ = ["MCRALS"]
+__all__ = ["Coord", "LinearCoord"]
 
-__dataset_methods__ = []
+import copy as cpy
+import textwrap
 
 import numpy as np
-from traitlets import Dict, HasTraits, Unicode
+from traitlets import All, Bool, CFloat, CInt, Instance, Integer, Unicode, Union
+from traitlets import default as traitdefault
+from traitlets import observe, signature_has_traits
+
+from spectrochempy.core import error_
+from spectrochempy.core.dataset.arraymixins.ndmath import NDMath, _set_operators
+from spectrochempy.core.dataset.baseobjects.ndarray import NDArray
+from spectrochempy.core.units import Quantity, ur
+from spectrochempy.utils.constants import INPLACE, NOMASK
+from spectrochempy.utils.misc import spacing_
+from spectrochempy.utils.print import colored_output
 
-from spectrochempy.analysis.pca import PCA
-from spectrochempy.core import INFO, info_, set_loglevel
-from spectrochempy.core.dataset.arraymixins.npy import dot
-from spectrochempy.core.dataset.nddataset import NDDataset
-from spectrochempy.utils import exceptions
-from spectrochempy.utils.traits import NDDatasetType
 
-
-class MCRALS(HasTraits):
+# ======================================================================================
+# Coord
+# ======================================================================================
+@signature_has_traits
+class Coord(NDMath, NDArray):
     """
-    Performs MCR-ALS of a dataset knowing the initial C or St matrix.
+    Explicit coordinates for a dataset along a given axis.
 
-    MCR-ALS (Multivariate Curve Resolution - Alternating Least Squares) resolve"s a set (or several sets) of
-    spectra X of an evolving mixture (or a set of mixtures) into the spectra St of ‘pure’ species and their
-    concentration profiles C. In terms of matrix equation:
-    .. math::`X = CS^T + E`
-    where :math:`E` is the lmatrix of residuals.
+    The coordinates of a `NDDataset` can be created using the  `Coord`
+    object.
+    This is a single dimension array with either numerical (float)
+    values or labels (str, `Datetime` objects, or any other kind of objects) to
+    represent the coordinates. Only a one numerical axis can be defined,
+    but labels can be multiple.
 
     Parameters
     ----------
-    dataset : NDDataset
-        The dataset on which to perform the MCR-ALS analysis.
-
-    guess : NDDataset
-        Initial concentration or spectra.
-
+    data : ndarray, tuple or list
+        The actual data array contained in the  `Coord` object.
+        The given array (with a single dimension) can be a list,
+        a tuple, a `~numpy.ndarray` , or a :term:`array-like` object.
+        If an object is passed that contains labels, or units,
+        these elements will be used to accordingly set those of the
+        created object.
+        If possible, the provided data will not be copied for `data` input,
+        but will be passed by reference, so you should make a copy the
+        `data` before passing it in the object constructor if that's the
+        desired behavior or set the `copy` argument to True.
     **kwargs
-        Optional parameters, see Other parameters below.
+        Optional keywords parameters. See other parameters.
 
     Other Parameters
     ----------------
-    tol : float, optional, default 0.1
-        Convergence criterion on the change of residuals (percent change of standard deviation of residuals).
-
-    maxit : int, optional, default=50
-        Maximum number of ALS minimizations.
-
-    maxdiv : int, optional, default=5
-        Maximum number of successive non-converging iterations.
-
-    nonnegConc : str or array of indexes or `None`, default `"all"`
-        Non negativity constraint on concentrations. If set to `'all'` (default) all concentrations profiles are
-        considered non-negative. If an array of indexes is passed, the corresponding profiles are considered
-        non-negative, not the others. For instance `[0, 2]` indicates that profile #0 and #2 are non-negative while
-         profile #1 *can* be negative. If set to `None` or `[]`, all profiles can be negative.
-
-    unimodConc : str or array of indexes, default `"all"`
-        Unimodality constraint on concentrations. If set to `'all'` (default) all concentrations profiles are
-        considered unimodal. If an array of indexes is passed, the corresponding profiles are considered
-        unimodal, not the others. For instance `[0, 2]` indicates that profile #0 and #2 are unimodal while
-         profile #1 *can* be multimodal. If set to `"None"` or `[]`, all profiles can be multimodal.
-
-    unimodConcMod : str, default "strict"
-        When set to `"strict"`, values deviating from unimodality are reset to the value of the previous point.
-        When set to `"smooth"`, both values (deviating point and previous point) are modified to avoid ="steps"
-        in the concentration profile.
-
-    unimodTol : float, default 1.1
-        Tolerance parameter for unimodality. Correction is applied only if:
-        ```C[i,j] > C[i-1,j] * unimodTol```  on the decreasing branch of profile #j,
-        ```C[i,j] < C[i-1,j] * unimodTol```  on the increasing branch of profile  #j.
-
-    monoDecConc : `None` or array of indexes
-        Monotonic decrease constraint on concentrations.  If set to `None` (default) or `[]` no constraint is applied.
-        If an array of indexes is passed, the corresponding profiles are considered do decrease monotonically, not
-         the others. For instance `[0, 2]` indicates that profile #0 and #2 are decreasing while profile #1 *can*
-         increase.
-
-    monoDecTol : float, default 1.1
-         Tolerance parameter for monotonic decrease. Correction is applied only if:
-        ```C[i,j] > C[i-1,j] * unimodTol```  along profile #j.
-
-    monoIncConc : `None` or array of indexes
-        Monotonic increase constraint on concentrations.  If set to `None` (default) or `[]` no constraint is applied.
-        If an array of indexes is passed, the corresponding profiles are considered to increase monotonically, not
-         the others. For instance `[0, 2]` indicates that profile #0 and #2 are increasing while profile #1 *can*
-         decrease.
-
-    monoIncTol : float, default 1.1
-            Tolerance parameter for monotonic decrease. Correction is applied only if:
-        ```C[i,j] < C[i-1,j] * unimodTol``` along profile  #j.
-
-    closureConc : None or array of indexes, default `None`
-        Defines the concentration profiles subjected to closure constraint. If set to `None` or `[]`, no constraint is
-        applied. If an array of indexes is passed, the corresponding profile will be constrained so that their weighted
-        sum equals the `closureTarget`.
-
-    closureTarget : str or array of float, default `"default"`
-        The value of the sum of concentrations profiles subjected to closure.  If set to `default`, the total
-        concentration is set to 1.0 for all observations. If an array is passed: the values of concentration for each
-        observation. Hence,`np.ones[X.shape[0]` would be equivalent to "default".
-
-    closureMethod : str, `"scaling"` or `"constantSum"`, default `"scaling"`
-        The method used to enforce Closure. "scaling" recompute the concentration profiles using linear algebra:
-        ```
-        C.data[:, closureConc] = np.dot(C.data[:, closureConc],
-                                        np.diag(np.linalg.lstsq(C.data[:, closureConc], closureTarget.T, rcond=None)[0]))
-        ```
-        "constantSum"` normalize the sum of concentration profiles to `closureTarget`.
-
-    hardConc : None or or array of indexes, default `None`
-        Defines hard constraints obn the concentration profiles. If set to `None` or `[]`, no constraint is
-        applied. If an array of indexes is passed, the corresponding profiles will set by `getC` (see below).
-
-    getC : Callable
-        An external function that will provide `len(hardConc)` concentration profiles:
-        ```
-        getC(Ccurr, *argsGetC, **kwargsGetC) -> hardC
-        ```
-        or:
-        ```
-        getC(Ccurr, *argsGetC, **kwargsGetC) -> hardC, newArgsGetC
-        ```
-        or:
-        ```
-        getC(Ccurr, *argsGetCn, **kargsGetC) -> hardC, newArgsGetC, extOutput
-        ```
-        where Ccurr  is the current C martrix, *argsGetC are the parameters needed to completely specify the function. `hardC` is a nadarray or NDDataset
-        of shape `(C.y, len(hardConc)`, newArgsGetC are the updated parameters for the next iteration (can be None), and
-        extOutput can be any relevant output to be kept in extOutput attribute (only the last iteration extOutput is
-        kept)
-
-    argsGetConc : tuple, optional
-        supplementary positional arguments passed to the external function.
-
-    kwargsGetConc: tuple, optional
-        supplementary keyword arguments passed to the external function
-
-    hardC_to_C_idx : None or list or tuple, default None
-        Indicates the correspondence between the indexes of the columns of hardC and of the C matrix. [1, None, 0]
-        indicates that the first profile in hardC (index O) corrsponds to the second profile of C (index 1).
-
-    nonnegSpec : str, list or tuple or `None`, default `"all"`
-        Indicates non-negative spectral profile. If set to `'all'` (default) all spectral profiles are
-        considered non-negative. If an array of indexes is passed, the corresponding profiles are considered
-        non-negative, not the others. For instance `[0, 2]` indicates that profile #0 and #2 are non-negative while
-        profile #1 *can* be negative. If set to `None` or `[]`, all profiles can be negative.
-
-    normSpec : None or str, default None
-        Defines whether the spectral profiles should be normalized. If set to `None` no normalization is applied.
-        when set to "euclid", spectra are normalized with respect to their total area, when set to "max", spectra are
-        normalized with respect to the maximum af their value.
-
-     unimodSpec : str or array of indexes, default `None`
-        Unimodality constraint on Spectra. If set to `None` (default) none of spectral profiles is
-        considered unimodal. If an array of indexes is passed, the corresponding profiles are considered
-        unimodal, not the others. For instance `[0, 2]` indicates that profile #0 and #2 are unimodal while
-        profile #1 *can* be multimodal. If set to `"None"` or `[]`, all profiles can be multimodal.
-
-    unimodSpecMod : str, default "strict"
-        When set to `"strict"`, values deviating from unimodality are reset to the value of the previous point.
-        When set to `"smooth"`, both values (deviating point and previous point) are modified to avoid ="steps"
-        in the concentration profile.
-
-    unimodSpecTol : float, default 1.1
-        Tolerance parameter for unimodality. Correction is applied only if the deviating point is larger/lower than
-        ```St[j,i] > St[j, i-1] * unimodSpecTol```  on the decreasing branch of profile #j,
-        ```St[j,i] < St[j, i-1] * unimodTol```  on the increasing branch of profile  #j.
-
+    dtype : str or dtype, optional, default=np.float64
+        If specified, the data will be casted to this dtype, else the
+        type of the data will be used.
+    dims : list of chars, optional.
+        if specified the list must have a length equal to the number od
+        data dimensions (ndim) and the chars must be
+        taken among among x,y,z,u,v,w or t. If not specified,
+        the dimension names are automatically attributed in
+        this order.
+    name : str, optional
+        A user friendly name for this object. If not given,
+        the automatic `id` given at the object creation will be
+        used as a name..
+    labels : array of objects, optional
+        Labels for the `data` . labels can be used only for 1D-datasets.
+        The labels array may have an additional dimension, meaning
+        several series of labels for the same data.
+        The given array can be a list, a tuple, a `~numpy.ndarray` ,
+        a ndarray-like, a  `NDArray` or any subclass of `NDArray` .
+    units : `Unit` instance or str, optional
+        Units of the data. If data is a `Quantity` then `units` is set
+        to the unit of the `data`; if a unit is also
+        explicitly provided an error is raised. Handling of units use
+        the `pint <https://pint.readthedocs.org/>`_
+        package.
+    title : str, optional
+        The title of the dimension. It will later be used for instance
+        for labelling plots of the data.
+        It is optional but recommended to give a title to each ndarray.
+    dlabel :  str, optional
+        Alias of `title` .
+    copy : bool, optional
+        Perform a copy of the passed object. Default is False.
+    linear : bool, optional
+        If set to True, the coordinate is considered as a
+        `LinearCoord` object.
+    offset : float, optional
+        Only used is linear is True.
+        If omitted a value of 0.0 is taken for the coordinate offset.
+    increment : float, optional
+        Only used if linear is true.
+        If omitted a value of 1.0 is taken for the coordinate increment.
 
     See Also
     --------
-    PCA
-       Performs MCR-ALS of a |NDDataset| knowing the initial C or St matrix.
-    NNMF
-       Performs a Non Negative Matrix Factorization of a |NDDataset| .
-    EFA
-       Perform an Evolving Factor Analysis (forward and reverse) of the input |NDDataset| .
+    NDDataset : Main SpectroChemPy object: an array with masks, units and coordinates.
+    LinearCoord : linear coordinates.
 
     Examples
     --------
-    >>> data = scp.read("matlabdata/als2004dataset.MAT")
-    >>> X, guess = data[-1], data[3]
-    >>> mcr = scp.MCRALS(X, guess)
-    >>> mcr.St, mcr.St
-    (NDDataset: [float64] unitless (shape: (y:4, x:96)), NDDataset: [float64] unitless (shape: (y:4, x:96)))
-    """
 
-    _X = NDDatasetType()
-    _C = NDDatasetType(allow_none=True)
-    _St = NDDatasetType(allow_none=True)
-    _log = Unicode()
-    _params = Dict()
-
-    def __init__(self, dataset, guess, **kwargs):
-        # list all default arguments:
-
-        tol = kwargs.get("tol", 0.1)
-        maxit = kwargs.get("maxit", 50)
-        maxdiv = kwargs.get("maxdiv", 5)
-
-        nonnegConc = kwargs.get("nonnegConc", "all")
-
-        unimodConc = kwargs.get("unimodConc", "all")
-        unimodConcTol = kwargs.get("unimodConcTol", 1.1)
-        unimodConcMod = kwargs.get("unimodMod", "strict")
-        if "unimodTol" in kwargs:
-            exceptions.deprecated("unimodTol", replace="unimodConcTol")
-            unimodConcTol = kwargs.get("unimodTol", 1.1)
-        if "unimodMod" in kwargs.keys():
-            exceptions.deprecated("unimodMod", replace="unimodConcMod")
-            unimodConcMod = kwargs.get("unimodConcMod", "strict")
-
-        monoDecConc = kwargs.get("monoDecConc", None)
-        monoIncTol = kwargs.get("monoIncTol", 1.1)
-        monoIncConc = kwargs.get("monoIncConc", None)
-        monoDecTol = kwargs.get("monoDecTol", 1.1)
-
-        closureConc = kwargs.get("closureConc", None)
-        closureTarget = kwargs.get("closureTarget", "default")
-        closureMethod = kwargs.get("closureMethod", "scaling")
-
-        hardConc = kwargs.get("hardConc", None)
-        getConc = kwargs.get("getConc", None)
-        argsGetConc = kwargs.get("argsGetConc", None)
-        kwargsGetConc = kwargs.get("kwargsGetConc", None)
-        hardC_to_C_idx = kwargs.get("hardC_to_C_idx", "default")
-
-        unimodSpec = kwargs.get("unimodSpec", None)
-        unimodSpecTol = kwargs.get("unimodSpecTol", 1.1)
-        unimodSpecMod = kwargs.get("unimodSpecMod", "strict")
-
-        nonnegSpec = kwargs.get("nonnegSpec", "all")
-
-        normSpec = kwargs.get("normSpec", None)
-
-        if "verbose" in kwargs.keys():
-            exceptions.deprecated(
-                "verbose", replace="set_loglevel('INFO') before launching MCRALS"
-            )
-            set_loglevel(INFO)
-
-        # Check initial data
-        # ------------------------------------------------------------------------------
-        initConc, initSpec = False, False
+    We first import the object from the api :
 
-        if type(guess) is np.ndarray:
-            guess = NDDataset(guess)
+    >>> from spectrochempy import Coord
 
-        X = dataset
+    We then create a numpy `~numpy.ndarray` and use it as the numerical `data`
+    axis of our new  `Coord` object :
 
-        if X.shape[0] == guess.shape[0]:
-            initConc = True
-            C = guess.copy()
-            C.name = "Pure conc. profile, mcs-als of " + X.name
-            nspecies = C.shape[1]
+    >>> c0 = Coord.arange(1., 12., 2., title='frequency', units='Hz')
+    >>> c0
+    Coord: [float64] Hz (size: 6)
 
-        elif X.shape[1] == guess.shape[1]:
-            initSpec = True
-            St = guess.copy()
-            St.name = "Pure spectra profile, mcs-als of " + X.name
-            nspecies = St.shape[0]
+    We can take a series of str to create a non numerical but labelled
+    axis :
 
-        else:
-            raise ValueError("the dimensions of guess do not match the data")
+    >>> tarr = list('abcdef')
+    >>> tarr
+    ['a', 'b', 'c', 'd', 'e', 'f']
 
-        ny, _ = X.shape
+    >>> c1 = Coord(labels=tarr, title='mylabels')
+    >>> c1
+    Coord: [labels] [  a   b   c   d   e   f] (size: 6)
+    """
 
-        # makes a PCA with same number of species for further comparison
-        Xpca = PCA(X).reconstruct(n_pc=nspecies)
+    _copy = Bool()
 
-        # reset default text to indexes
-        # ------------------------------
-        if nonnegConc == "all":
-            nonnegConc = np.arange(nspecies)
-        elif nonnegConc is None:
-            nonnegConc = []
-        elif nonnegConc != [] and (
-            len(nonnegConc) > nspecies or max(nonnegConc) + 1 > nspecies
-        ):
-            raise ValueError(
-                f"The guess has only {nspecies} species, please check nonnegConc"
-            )
+    _html_output = False
+    _parent_dim = Unicode(allow_none=True)
 
-        if unimodConc == "all":
-            unimodConc = np.arange(nspecies)
-        elif unimodConc is None:
-            unimodConc = []
-        elif unimodConc != [] and (
-            len(unimodConc) > nspecies or max(unimodConc) + 1 > nspecies
-        ):
-            raise ValueError(
-                f"The guess has only {nspecies} species, please check unimodConc"
-            )
+    # For linear data generation
+    _offset = Union((CFloat(), CInt(), Instance(Quantity)))
+    _increment = Union((CFloat(), CInt(), Instance(Quantity)))
+    _size = Integer(0)
+    _linear = Bool(False)
+
+    # ----------------------------------------------------------------------------------
+    # initialization
+    # ----------------------------------------------------------------------------------
+    def __init__(self, data=None, **kwargs):
+
+        super().__init__(data=data, **kwargs)
+
+        if len(self.shape) > 1:
+            raise ValueError("Only one 1D arrays can be used to define coordinates")
+
+        self._linear = kwargs.pop("linear", False)
+        self._increment = kwargs.pop("increment", 1.0)
+        self._offset = kwargs.pop("offset", 0.0)
+        self._size = kwargs.pop("size", 0)
+        # self._accuracy = kwargs.pop('accuracy', None)
+
+    # ----------------------------------------------------------------------------------
+    # readonly property
+    # ----------------------------------------------------------------------------------
+    @property
+    def reversed(self):
+        """bool - Whether the axis is reversed (readonly
+        property).
+        """
+        if self.units == "ppm":
+            return True
+        elif self.units == "1 / centimeter" and "raman" not in self.title.lower():
+            return True
+        return False
 
-        if closureTarget == "default":
-            closureTarget = np.ones(ny)
-        elif len(closureTarget) != ny:
-            raise ValueError(
-                f"The data contain only {ny} observations, please check closureTarget"
-            )
+        # Return a correct result only if the data are sorted  # return  # bool(self.data[0] > self.data[-1])
 
-        if hardC_to_C_idx == "default":
-            hardC_to_C_idx = np.arange(nspecies)
-        elif len(hardC_to_C_idx) > nspecies or max(hardC_to_C_idx) + 1 > nspecies:
-            raise ValueError(
-                f"The guess has only {nspecies} species, please check hardC_to_C_idx"
-            )
+    @property
+    def data(self):
+        """
+        The `data` array (`~numpy.ndarray`).
 
-        # constraints on spectra
+        If there is no data but labels, then the labels are returned instead of data.
+        """
+        if self.linear:
+            data = np.arange(self.size) * self._increment + self._offset
+            # if hasattr(data, "units"):
+            #    data = data.m
+        else:
+            data = self._data
 
-        if unimodSpec == "all":
-            unimodSpec = np.arange(nspecies)
-        elif unimodSpec is None:
-            unimodSpec = []
-        elif unimodSpec != [] and (
-            len(unimodSpec) > nspecies or max(unimodSpec) + 1 > nspecies
-        ):
-            raise ValueError(
-                f"The guess has only {nspecies} species, please check unimodSpec"
-            )
+        return data
 
-        if nonnegSpec == "all":
-            nonnegSpec = np.arange(nspecies)
-        elif nonnegSpec is None:
-            nonnegSpec = []
-        elif nonnegSpec != [] and (
-            len(nonnegSpec) > nspecies or max(nonnegSpec) + 1 > nspecies
-        ):
-            raise ValueError(
-                f"The guess has only {nspecies} species, please check nonnegSpec"
-            )
+    @data.setter
+    def data(self, data):
 
-        # Compute initial spectra or concentrations   (first iteration...)
-        # ------------------------------------------------------------------------------
-        if initConc:
-            if C.coordset is None:
-                C.set_coordset(y=X.y, x=C.x)
-            St = NDDataset(np.linalg.lstsq(C.data, X.data, rcond=None)[0])
-            St.name = "Pure spectra profile, mcs-als of " + X.name
-            St.title = X.title
-            cy = C.x.copy() if C.x else None
-            cx = X.x.copy() if X.x else None
-            St.set_coordset(y=cy, x=cx)
-
-        if initSpec:
-            if St.coordset is None:
-                St.set_coordset(y=St.y, x=X.x)
-            Ct = np.linalg.lstsq(St.data.T, X.data.T, rcond=None)[0]
-            C = NDDataset(Ct.T)
-            C.name = "Pure conc. profile, mcs-als of " + X.name
-            C.title = "concentration"
-            cx = St.y.copy() if St.y else None
-            cy = X.y.copy() if X.y else None
-            C.set_coordset(y=cy, x=cx)
-
-        change = tol + 1
-        stdev = np.std(X.data)
-        niter = 0
-        ndiv = 0
-
-        log = "*** ALS optimisation log*** \n"
-        info_(log)
-        logentry = "#iter     RSE / PCA        RSE / Exp      %change \n"
-        log += logentry
-        info_(logentry)
-        logentry = "------------------------------------------------- \n"
-        log += logentry
-        info_(logentry)
-
-        while change >= tol and niter < maxit and ndiv < maxdiv:
-            C.data = np.linalg.lstsq(St.data.T, X.data.T, rcond=None)[0].T
-            niter += 1
-
-            # Force non-negative concentration
-            # --------------------------------
-            if nonnegConc is not None:
-                for s in nonnegConc:
-                    C.data[:, s] = C.data[:, s].clip(min=0)
-
-            # Force unimodal concentration
-            # ----------------------------
-            if len(unimodConc) > 0:
-                C.data = _unimodal_2D(
-                    C.data,
-                    idxes=unimodConc,
-                    axis=0,
-                    tol=unimodConcTol,
-                    mod=unimodConcMod,
-                )
-
-            # Force monotonic increase
-            # ------------------------
-            if monoIncConc is not None:
-                for s in monoIncConc:
-                    for curid in np.arange(ny - 1):
-                        if C.data[curid + 1, s] < C.data[curid, s] / monoIncTol:
-                            C.data[curid + 1, s] = C.data[curid, s]
-
-            # Force monotonic decrease
-            # ----------------------------------------------
-            if monoDecConc is not None:
-                for s in monoDecConc:
-                    for curid in np.arange(ny - 1):
-                        if C.data[curid + 1, s] > C.data[curid, s] * monoDecTol:
-                            C.data[curid + 1, s] = C.data[curid, s]
-
-            # Closure
-            # ------------------------------------------
-            if closureConc is not None:
-                if closureMethod == "scaling":
-                    Q = np.linalg.lstsq(
-                        C.data[:, closureConc], closureTarget.T, rcond=None
-                    )[0]
-                    C.data[:, closureConc] = np.dot(C.data[:, closureConc], np.diag(Q))
-                elif closureMethod == "constantSum":
-                    totalConc = np.sum(C.data[:, closureConc], axis=1)
-                    C.data[:, closureConc] = (
-                        C.data[:, closureConc]
-                        * closureTarget[:, None]
-                        / totalConc[:, None]
-                    )
-
-            # external concentration profiles
-            # ------------------------------------------
-            if hardConc is not None:
-                if kwargsGetConc is not None and argsGetConc is not None:
-                    output = getConc(C, *argsGetConc, **kwargsGetConc)
-                elif kwargsGetConc is None and argsGetConc is not None:
-                    output = getConc(C, *argsGetConc)
-                elif kwargsGetConc is not None and argsGetConc is None:
-                    output = getConc(C, **kwargsGetConc)
-                else:
-                    output = getConc(C)
+        self._set_data(data)
 
-                if isinstance(output, tuple):
-                    fixedC = output[0]
-                    argsGetConc = output[1]
-                    if len(output) == 3:
-                        extOutput = output[2]
-                    else:
-                        extOutput = None
-                else:
-                    fixedC = output
-                    extOutput = None
+    @property
+    def default(self):
+        # this is in case default is called on a coord, while it is a coordset property
+        return self
+
+    # ----------------------------------------------------------------------------------
+    # hidden properties (for the documentation, only - we remove the docstring)
+    # some of the property of NDArray has to be hidden because they
+    # are not useful for this Coord class
+    # ----------------------------------------------------------------------------------
+    # NDarray methods
 
-                C.data[:, hardConc] = fixedC[:, hardC_to_C_idx]
+    @property
+    def is_complex(self):
+        return False  # always real
 
-            # stores C in Chard
-            Chard = C.copy()
+    @property
+    def is_empty(self):
+        """
+        True if the `data` array is empty or size=0, and if no label are present
+        - Readonly property (bool).
+        """
+        if not self.linear:
+            return super().is_empty
 
-            # compute St
-            St.data = np.linalg.lstsq(C.data, X.data, rcond=None)[0]
-
-            # stores St in Stsoft
-            Stsoft = St.copy()
-
-            # Force non-negative spectra
-            # --------------------------
-            if nonnegSpec is not None:
-                St.data[nonnegSpec, :] = St.data[nonnegSpec, :].clip(min=0)
-
-            # Force unimodal spectra
-            # ----------------------------
-            if unimodSpec != []:
-                St.data = _unimodal_2D(
-                    St.data,
-                    idxes=unimodSpec,
-                    axis=1,
-                    tol=unimodSpecTol,
-                    mod=unimodSpecMod,
-                )
-
-            # recompute C for consistency(soft modeling)
-            C.data = np.linalg.lstsq(St.data.T, X.data.T, rcond=-1)[0].T
-
-            # rescale spectra & concentrations
-            if normSpec == "max":
-                alpha = np.max(St.data, axis=1).reshape(nspecies, 1)
-                St.data = St.data / alpha
-                C.data = C.data * alpha.T
-            elif normSpec == "euclid":
-                alpha = np.linalg.norm(St.data, axis=1).reshape(nspecies, 1)
-                St.data = St.data / alpha
-                C.data = C.data * alpha.T
-
-            # compute residuals
-            # -----------------
-            X_hat = dot(C, St)
-            stdev2 = np.std(X_hat.data - X.data)
-            change = 100 * (stdev2 - stdev) / stdev
-            stdev = stdev2
+        return False
 
-            stdev_PCA = np.std(X_hat.data - Xpca.data)  #
+    @property
+    def ndim(self):
+        if self.linear:
+            return 1
+        ndim = super().ndim
+        if ndim > 1:
+            raise ValueError("Coordinate's array should be 1-dimensional!")
+        return ndim
 
-            logentry = "{:3d}      {:10f}      {:10f}      {:10f}".format(
-                niter, stdev_PCA, stdev2, change
-            )
-            log += logentry + "\n"
-            info_(logentry)
+    @property
+    def T(self):  # no transpose
+        return self
 
-            if change > 0:
-                ndiv += 1
+    # @property
+    # def values(self):
+    #    return super().values
+
+    def to(self, other, inplace=False, force=False):
+
+        new = super().to(other, force=force)
+
+        if inplace:
+            self._units = new._units
+            self._title = new._title
+            self._roi = new._roi
+            if not self.linear:
+                self._data = new._data
             else:
-                ndiv = 0
-                change = -change
+                self._offset = new._offset
+                self._increment = new._increment
+                self._linear = new._linear
 
-            if change < tol:
-                logentry = "converged !"
-                log += logentry + "\n"
-                info_(logentry)
-
-            if ndiv == maxdiv:
-                logline = (
-                    f"Optimization not improved since {maxdiv} iterations... unconverged "
-                    f"or 'tol' set too small ?\n"
-                )
-                logline += "Stop ALS optimization"
-                log += logline + "\n"
-                info_(logline)
-
-            if niter == maxit:
-                logline = "Convergence criterion ('tol') not reached after {:d} iterations.".format(
-                    maxit
-                )
-                logline += "Stop ALS optimization"
-                log += logline + "\n"
-                info_(logline)
-
-        self._X = X
-        self._params = {
-            "tol": tol,
-            "maxit": maxit,
-            "maxdiv": maxdiv,
-            "nonnegConc": nonnegConc,
-            "unimodConc": unimodConc,
-            "unimodConcTol": unimodConcTol,
-            "unimodConcMod": unimodConcMod,
-            "closureConc": closureConc,
-            "closureTarget ": closureTarget,
-            "closureMethod": closureMethod,
-            "monoDecConc": monoDecConc,
-            "monoDecTol": monoDecTol,
-            "monoIncConc": monoIncConc,
-            "monoIncTol": monoIncTol,
-            "hardConc": hardConc,
-            "getConc": getConc,
-            "argsGetConc": argsGetConc,
-            "hardC_to_C_idx": hardC_to_C_idx,
-            "nonnegSpec": nonnegSpec,
-            "unimodSpec": unimodConc,
-            "unimodSpecTol": unimodSpecTol,
-            "unimodSpecMod": unimodSpecMod,
-            "normSpec": normSpec,
-        }
-
-        self._C = C
-        if hardConc is not None:
-            self._extOutput = extOutput
         else:
-            self._extOutput = None
+            return new
 
-        self._St = St
-        self._log = log
+    to.__doc__ = NDArray.to.__doc__
 
-        self._Stsoft = Stsoft
-        self._Chard = Chard
+    @property
+    def masked_data(self):
+        return super().masked_data
 
     @property
-    def X(self):
-        """
-        The original dataset.
-        """
-        return self._X
+    def is_masked(self):
+        return False
 
     @property
-    def extOutput(self):
+    def linear(self):
         """
-        The last output of the external function used to get concentrations.
+        Flag to specify if the data can be constructed using a linear variation (bool).
         """
-        return self._extOutput
+        return self._linear
+
+    @linear.setter
+    def linear(self, val):
+
+        self._linear = (
+            val  # it val is true this provoque the linearization (  # see observe)
+        )
+
+        # if val and self._data is not None:  #     # linearisation of the data, if possible  #     self._linearize()
 
     @property
-    def C(self):
+    def offset(self):
         """
-        The final concentration profiles.
+        Starting value for linear array
         """
-        return self._C
+        return self._offset
+
+    @offset.setter
+    def offset(self, val):
+        if isinstance(val, Quantity):
+            if self.has_units:
+                val.ito(self.units)
+                val = val.m
+            else:
+                self.units = val.units
+                val = val.m
+        self._offset = val
 
     @property
-    def St(self):
-        """
-        The final spectra profiles.
-        """
-        return self._St
+    def offset_value(self):
+        offset = self.offset
+        if self.units:
+            return Quantity(offset, self._units)
+        else:
+            return offset
 
     @property
-    def Stsoft(self):
-        """
-        The soft spectra profiles.
-        """
-        return self._Stsoft
+    def mask(self):
+        return NOMASK
+
+    @mask.setter
+    def mask(self, val):
+        # Coordinates cannot be masked. Set mask always to NOMASK
+        self._mask = NOMASK
+
+    # NDmath methods
+
+    def cumsum(self, **kwargs):
+        raise NotImplementedError
+
+    def mean(self, **kwargs):
+        raise NotImplementedError
+
+    def pipe(self, func=None, *args, **kwargs):
+        raise NotImplementedError
+
+    def remove_masks(self, **kwargs):
+        raise NotImplementedError
 
     @property
-    def Chard(self):
+    def size(self):
         """
-        The hard concentration profiles.
+        Size of the underlying `data` array - Readonly property (int).
         """
-        return self._Chard
+
+        if self.linear:
+            # the provided size is returned i or its default
+            return self._size
+        else:
+            return super().size
 
     @property
-    def params(self):
-        """
-        The parameters used to perform the MCR als.
-        """
-        return self._params
+    def shape(self):
+        if self.linear:
+            return (self._size,)
+        return super().shape
+
+    def std(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def sum(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def swapdims(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def swapaxes(self, *args, **kwargs):
+        raise NotImplementedError
 
     @property
-    def log(self):
-        """
-        Logs output.
+    def spacing(self):
         """
-        return self._log
+        Return coordinates spacing.
 
-    @property
-    @exceptions.deprecated(replace="log")
-    def logs(self):
+        It will be a scalar if the coordinates are uniformly spaced,
+        else an array of the different spacings
         """
-        Logs output.
+        if self.linear:
+            return self.increment * self.units
+        return spacing_(self.data) * self.units
+
+    def squeeze(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def random(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def empty(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def empty_like(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def var(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def ones(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def ones_like(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def full(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def diag(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def diagonal(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def full_like(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def identity(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def eye(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def zeros(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def zeros_like(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def coordmin(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def coordmax(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def conjugate(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def conj(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def abs(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def absolute(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def all(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def any(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def argmax(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def argmin(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def asfortranarray(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def astype(self, dtype=None, **kwargs):
         """
-        return self._log
+        Cast the data to a specified type.
 
-    def reconstruct(self):
+        Parameters
+        ----------
+        dtype : str or dtype
+            Typecode or data-type to which the array is cast.
         """
-        Transform data back to the original space.
+        if not self.linear:
+            self._data = self._data.astype(dtype, **kwargs)
+        else:
+            self._increment = np.array(self._increment).astype(dtype, **kwargs)[()]
+            self._offset = np.array(self._offset).astype(dtype, **kwargs)[()]
+        return self
 
-        The following matrice operation is performed : :math:`X'_{hat} = C'.S'^t`.
+    def average(self, *args, **kwargs):
+        raise NotImplementedError
 
-        Returns
-        -------
-        X_hat : |NDDataset|
-            The reconstructed dataset based on the MCS-ALS optimization.
-        """
+    def clip(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def get_axis(self, *args, **kwargs):
+        return super().get_axis(*args, **kwargs)
+
+    @property
+    def origin(self, *args, **kwargs):
+        raise NotImplementedError
+
+    @property
+    def author(self):
+        return None
 
-        # reconstruct from concentration and spectra profiles
-        C = self.C
-        St = self.St
+    @property
+    def descendant(self):
+        return (self.data[-1] - self.data[0]) < 0
+
+    @property
+    def dims(self):
+        return ["x"]
 
-        X_hat = dot(C, St)
+    @property
+    def is_1d(self):
+        return True
 
-        X_hat.history = "Dataset reconstructed by MCS ALS optimization"
-        X_hat.title = "X_hat: " + self.X.title
-        return X_hat
+    def transpose(self, **kwargs):
+        return self
 
-    def plotmerit(self, **kwargs):
+    # ----------------------------------------------------------------------------------
+    # public methods
+    # ----------------------------------------------------------------------------------
+    def loc2index(self, loc):
         """
-        Plots the input dataset, reconstructed dataset and residuals.
+        Return the index corresponding to a given location.
 
         Parameters
         ----------
-        **kwargs
-            optional "colors" argument: tuple or array of 3 colors for :math:`X`, :math:`\hat X` and :math:`E`.
+        loc : float.
+            Value corresponding to a given location on the coordinates axis.
 
         Returns
         -------
-        ax
-            subplot.
-        """
-        colX, colXhat, colRes = kwargs.get("colors", ["blue", "green", "red"])
+        index : int.
+            The corresponding index.
 
-        X_hat = self.reconstruct()
-        res = self.X - X_hat
-        ax = self.X.plot()
-        if self.X.x is not None:
-            ax.plot(self.X.x.data, X_hat.T.data, color=colXhat)
-            ax.plot(self.X.x.data, res.T.data, color=colRes)
-        else:
-            ax.plot(X_hat.T.data, color=colXhat)
-            ax.plot(res.T.data, color=colRes)
-        ax.autoscale(enable=True)
-        ax.set_title("MCR ALS merit plot")
-        return ax
-
-
-# ---------------------------------
-def _unimodal_2D(a, axis, idxes, tol, mod):
-    """Force unimodality on given lines or or columnns od a 2D ndarray
-
-    a: ndarray
-
-    axis: int
-        axis along which the correction is applied
-
-    idxes: list of int
-        indexes at which the correction is applied
-
-    mod : str
-        When set to `"strict"`, values deviating from unimodality are reset to the value of the previous point.
-        When set to `"smooth"`, both values (deviating point and previous point) are modified to avoid "steps"
-        in the profile.
-
-    tol: float
-        Tolerance parameter for unimodality. Correction is applied only if:
-        `a[i] > a[i-1] * unimodTol`  on a decreasing branch of profile,
-        `a[i] < a[i-1] * unimodTol`  on an increasing branch of profile.
-    """
+        Examples
+        --------
+
+        >>> dataset = scp.NDDataset.read("irdata/nh4y-activation.spg")
+        >>> dataset.x.loc2index(1644.0)
+        4517
+        """
+        return self._loc2index(loc)
+
+    # ----------------------------------------------------------------------------------
+    # special methods
+    # ----------------------------------------------------------------------------------
+    def __copy__(self):
+        res = self.copy(deep=False)  # we keep name of the coordinate by default
+        res.name = self.name
+        return res
+
+    def __deepcopy__(self, memo=None):
+        res = self.copy(deep=True, memo=memo)
+        res.name = self.name
+        return res
+
+    def __dir__(self):
+        # remove some methods with respect to the full NDArray
+        # as they are not useful for Coord.
+        return [
+            "data",
+            "labels",
+            "units",
+            "title",
+            "name",
+            "offset",
+            "increment",
+            "linear",
+            "roi",
+        ]
+
+    def __getitem__(self, items, **kwargs):
+
+        if isinstance(items, list):
+            # Special case of fancy indexing
+            items = (items,)
+
+        # choose, if we keep the same or create new object
+        inplace = False
+        if isinstance(items, tuple) and items[-1] == INPLACE:
+            items = items[:-1]
+            inplace = True
+
+        # Eventually get a better representation of the indexes
+        keys = self._make_index(items)
+
+        # init returned object
+        if inplace:
+            new = self
+        else:
+            new = self.copy()
+
+        # slicing by index of all internal array
+        if new.data is not None:
+            udata = new.data[keys]
+
+            if new.linear:
+                # if self.increment > 0:
+                #     new._offset = udata.min()
+                # else:
+                #     new._offset = udata.max()
+                new._size = udata.size
+                if new._size > 1:
+                    inc = np.diff(udata)
+                    variation = (inc.max() - inc.min()) / udata.ptp()
+                    if variation < 1.0e-5:
+                        new._increment = np.mean(inc)  # np.round(np.mean(
+                        # inc), 5)
+                        new._offset = udata[0]
+                        new._data = None
+                        new._linear = True
+                    else:
+                        new._linear = False
+                else:
+                    new._linear = False
+
+            if not new.linear:
+                new._data = np.asarray(udata)
+
+        if self.is_labeled:
+            # case only of 1D dataset such as Coord
+            new._labels = np.array(self._labels[keys])
+
+        if new.is_empty:
+            error_(
+                IndexError,
+                f"Empty array of shape {new._data.shape} resulted from slicing.\n"
+                f"Check the indexes and make sure to use floats for location slicing",
+            )
+            new = None
+
+        new._mask = NOMASK
+
+        # we need to keep the names when copying coordinates to avoid later
+        # problems
+        new.name = self.name
+        return new
+
+    def __setitem__(self, items, value):
+
+        if self.linear:
+            error_(Exception, "Linearly defined array are readonly")
+            return
+
+        super().__setitem__(items, value)
+
+    def __str__(self):
+        return repr(self)
+
+    def _cstr(self, header="  coordinates: ... \n", print_size=True, **kwargs):
+
+        indent = kwargs.get("indent", 0)
+
+        out = ""
+        if not self.is_empty and print_size:
+            out += f"{self._str_shape().rstrip()}\n"
+        out += f"        title: {self.title}\n" if self.title else ""
+        if self.has_data:
+            out += "{}\n".format(self._str_value(header=header))
+        elif self.is_empty and not self.is_labeled:
+            out += header.replace("...", "\0Undefined\0")
+
+        if self.is_labeled:
+            header = "       labels: ... \n"
+            text = str(self.labels.T).strip()
+            if "\n" not in text:  # single line!
+                out += header.replace("...", "\0\0{}\0\0".format(text))
+            else:
+                out += header
+                out += "\0\0{}\0\0".format(textwrap.indent(text.strip(), " " * 9))
+
+        if out[-1] == "\n":
+            out = out[:-1]
 
-    if axis == 0:
-        a_ = a
-    elif axis == 1:
-        a_ = a.T
+        if indent:
+            out = "{}".format(textwrap.indent(out, " " * indent))
 
-    for col, idx in zip(a_[:, idxes].T, idxes):
-        a_[:, idx] = _unimodal_1D(col, tol, mod)
+        first_indent = kwargs.get("first_indent", 0)
+        if first_indent < indent:
+            out = out[indent - first_indent :]
 
-    return a
+        if not self._html_output:
+            return colored_output(out)
+        else:
+            return out
 
+    def __repr__(self):
+        out = self._repr_value().rstrip()
+        return out
+
+    # ----------------------------------------------------------------------------------
+    # Private properties and methods
+    # ----------------------------------------------------------------------------------
+    @traitdefault("_increment")
+    def _increment_default(self):
+        return 1.0
+
+    def _linearize(self):
+
+        if not self.linear or self._data is None:
+            return
+
+        self._linear = False  # to avoid action of the observer
+
+        if self._squeeze_ndim > 1:
+            error_(NotImplementedError, "Linearization is only implemented for 1D data")
+            return
+
+        data = self._data.squeeze()
+
+        # try to find an increment
+        if data.size > 1:
+            inc = np.diff(data)
+            variation = (inc.max() - inc.min()) / data.ptp()
+            if variation < 1.0e-5:
+                self._increment = (
+                    data.ptp() / (data.size - 1) * np.sign(inc[0])
+                )  # np.mean(inc)  # np.round(np.mean(inc), 5)
+                self._offset = data[0]
+                self._size = data.size
+                self._data = None
+                self._linear = True
+            else:
+                self._linear = False
+        else:
+            self._linear = False
 
-def _unimodal_1D(a: np.ndarray, tol: str, mod: str) -> np.ndarray:
-    """force unimodal concentration
+    @traitdefault("_offset")
+    def _offset_default(self):
+        return 0
+
+    def _set_data(self, data):
+
+        if data is None:
+            return
+
+        elif isinstance(data, Coord) and data.linear:
+            # Case of LinearCoord
+            for attr in self.__dir__():
+                try:
+                    if attr in ["linear", "offset", "increment"]:
+                        continue
+                    if attr == "data":
+                        val = data.data
+                    else:
+                        val = getattr(data, f"_{attr}")
+                    if self._copy:
+                        val = cpy.deepcopy(val)
+                    setattr(self, f"_{attr}", val)
+                except AttributeError:
+                    # some attribute of NDDataset are missing in NDArray
+                    pass
+
+        elif isinstance(data, NDArray):
+            # init data with data from another NDArray or NDArray's subclass
+            # No need to check the validity of the data
+            # because the data must have been already
+            # successfully initialized for the passed NDArray.data
+            for attr in self.__dir__():
+                try:
+                    val = getattr(data, f"_{attr}")
+                    if self._copy:
+                        val = cpy.deepcopy(val)
+                    setattr(self, f"_{attr}", val)
+                except AttributeError:
+                    # some attribute of NDDataset are missing in NDArray
+                    pass
+
+        elif isinstance(data, Quantity):
+            self._data = np.array(data.magnitude, subok=True, copy=self._copy)
+            self._units = data.units
+
+        elif hasattr(data, "mask"):
+            # an object with data and mask attributes
+            self._data = np.array(data.data, subok=True, copy=self._copy)
+            if isinstance(data.mask, np.ndarray) and data.mask.shape == data.data.shape:
+                self.mask = np.array(data.mask, dtype=np.bool_, copy=False)
+
+        elif (
+            not hasattr(data, "shape")
+            or not hasattr(data, "__getitem__")
+            or not hasattr(data, "__array_struct__")
+        ):
+            # Data doesn't look like a numpy array, try converting it to
+            # one. Non-numerical input are converted to an array of objects.
+            self._data = np.array(data, subok=True, copy=False)
 
-    makes a vector unimodal
+        else:
+            data = np.array(data, subok=True, copy=self._copy)
+            if data.dtype == np.object_:  # likely None value
+                data = data.astype(float)
+            self._data = data
+
+        if self.linear:
+            # we try to replace data by only an offset and an increment
+            self._linearize()
+
+    @staticmethod
+    def _unittransform(new, units):
+        oldunits = new.units
+        if not new.linear:
+            udata = (new.data * oldunits).to(units)
+            new._data = udata.m
+            new._units = udata.units
+        else:
+            offset = (new.offset * oldunits).to(units)
+            increment = (new.increment * oldunits).to(units)
+            new._offset = offset.m
+            new._increment = increment.m
+            new._units = increment.units
+
+        if new._roi is not None:
+            roi = (np.array(new._roi) * oldunits).to(units)
+            new._roi = list(roi)
+
+        # if new._linear:
+        #     # try to make it linear as well
+        #     new._linearize()
+        #     if not new._linear and new._implements("LinearCoord"):
+        #         # can't be linearized -> Coord
+        #         if inplace:
+        #             raise Exception(
+        #                     "A LinearCoord object cannot be transformed to a non linear coordinate "
+        #                     "`inplace` . "
+        #                     "Use to() instead of ito() and leave the `inplace` attribute to False"
+        #             )
+        #         else:
+        #             from spectrochempy import Coord
+        #
+        #             new = Coord(new)
+        return new
+
+    # ----------------------------------------------------------------------------------
+    # Events
+    # ----------------------------------------------------------------------------------
+    @observe(All)
+    def _anytrait_changed(self, change):
+        # ex: change {
+        #   'owner': object, # The HasTraits instance
+        #   'new': 6, # The new value
+        #   'old': 5, # The old value
+        #   'name': "foo", # The name of the changed trait
+        #   'type': 'change', # The event type of the notification, usually
+        #   'change'
+        # }
+
+        if change.name in ["_linear", "_increment", "_offset", "_size"]:
+            if self._linear:
+                self._linearize()
+            return
 
-    parameters:
+    @property
+    def increment(self):
+        return self._increment
+
+    @increment.setter
+    def increment(self, val):
+        if isinstance(val, Quantity):
+            if self.has_units:
+                val.ito(self.units)
+                val = val.m
+            else:
+                self.units = val.units
+                val = val.m
+        self._increment = val
+
+    @property
+    def increment_value(self):
+        increment = self.increment
+        if self.units:
+            return Quantity(increment, self._units)
+        else:
+            return increment
+
+
+@signature_has_traits
+class LinearCoord(Coord):
+    """
+    Linear coordinates.
+
+    Such coordinates correspond to a ascending or descending linear
+    sequence of values, fully determined by two parameters, i.e., an offset (off) and an increment (inc) :
+
+    .. math::
+
+        \\mathrm{data} = i*\\mathrm{inc} + \\mathrm{off}.
+
+    Parameters
     ----------
-    a : 1D ndarray
+    data : a 1D array-like object, optional
+        WWen provided, the `size` parameters is adjusted to the size of
+        the array, and a linearization of the
+        array is performed (only if it is possible: regular spacing in
+        the 1.e5 relative accuracy).
+    offset : float, optional
+        If omitted a value of 0.0 is taken for the coordinate offset.
+    increment : float, optional
+        If omitted a value of 1.0 is taken for the coordinate increment.
+    **kwargs
+        Optional keywords parameters. See other parameters.
+
+    Other Parameters
+    ----------------
+    dtype : str or dtype, optional, default=np.float64
+        If specified, the data will be casted to this dtype, else the
+        type of the data will be used
+    dims : list of chars, optional.
+        if specified the list must have a length equal to the number od
+        data dimensions (ndim) and the chars must be
+        taken among x,y,z,u,v,w or t. If not specified,
+        the dimension names are automatically attributed in
+        this order.
+    name : str, optional
+        A user-friendly name for this object. If not given,
+        the automatic `id` given at the object creation will be
+        used as a name.
+    labels : array of objects, optional
+        Labels for the `data` . labels can be used only for 1D-datasets.
+        The labels array may have an additional dimension, meaning
+        several series of labels for the same data.
+        The given array can be a list, a tuple, a `~numpy.ndarray` ,
+        a ndarray-like, a  `NDArray` or any subclass of `NDArray` .
+    units : `Unit` instance or str, optional
+        Units of the data. If data is a `Quantity` then `units` is set
+        to the unit of the `data`; if a unit is also
+        explicitly provided an error is raised. Handling of units use
+        the `pint <https://pint.readthedocs.org/>`_
+        package.
+    title : str, optional
+        The title of the dimension. It will later be used for instance
+        for labelling plots of the data.
+        It is optional but recommended to give a title to each ndarray.
+    dlabel : str, optional.
+        Alias of `title` .
+    meta : dict-like object, optional.
+        Additional metadata for this object. Must be dict-like but no
+        further restriction is placed on meta.
+    copy : bool, optional
+        Perform a copy of the passed object. Default is False.
+    fill_missing : bool
+        Create a linear coordinate array where missing data are masked.
+
+    See Also
+    --------
+    NDDataset : Main SpectroChemPy object: an array with masks, units and
+    coordinates.
+    Coord : Explicit coordinates.
+
+    Examples
+    --------
+    >>> from spectrochempy import LinearCoord, Coord
+
+    To create a linear coordinate, we need to specify an offset,
+    an increment and
+    the size of the data
+
+    >>> c1 = LinearCoord(offset=2.0, increment=2.0, size=10)
 
-    mod : str
-        When set to `"strict"`, values deviating from unimodality are reset to the value of the previous point.
-        When set to `"smooth"`, both values (deviating point and previous point) are modified to avoid "steps"
-        in the profile.
-
-    tol: float
-        Tolerance parameter for unimodality. Correction is applied only if:
-        `a[i] > a[i-1] * unimodTol`  on a decreasing branch of profile,
-        `a[i] < a[i-1] * unimodTol`  on an increasing branch of profile.
+    Alternatively, linear coordinates can be created using the
+    `linear` keyword
+
+    >>> c2 = Coord(linear=True, offset=2.0, increment=2.0, size=10)
     """
 
-    maxid = np.argmax(a)
-    curmax = max(a)
-    curid = maxid
-
-    while curid > 0:
-        # run backward
-        curid -= 1
-        if a[curid] > curmax * tol:
-            if mod == "strict":
-                a[curid] = a[curid + 1]
-            if mod == "smooth":
-                a[curid] = (a[curid] + a[curid + 1]) / 2
-                a[curid + 1] = a[curid]
-                curid = curid + 2
-        curmax = a[curid]
-
-    curid = maxid
-    curmax = a[maxid]
-    while curid < len(a) - 1:
-        curid += 1
-        if a[curid] > curmax * tol:
-            if mod == "strict":
-                a[curid] = a[curid - 1]
-            if mod == "smooth":
-                a[curid] = (a[curid] + a[curid - 1]) / 2
-                a[curid - 1] = a[curid]
-                curid = curid - 2
-        curmax = a[curid]
+    _use_time = Bool(False)
+    _show_datapoints = Bool(True)
+    _zpd = Integer()
+
+    def __init__(self, data=None, offset=0.0, increment=1.0, **kwargs):
+
+        if data is not None and isinstance(data, Coord) and not data.linear:
+            raise ValueError(
+                "Only linear Coord (with attribute linear set to True, can be transformed into "
+                "LinearCoord class"
+            )
+
+        super().__init__(data, **kwargs)
 
-    return a
+        # when data is present, we don't need offset and increment, nor size,
+        # we just do linear=True and these parameters are ignored
+
+        if self._data is not None:
+            self._linear = True
+
+        elif not self.linear:
+            # in case it was not already a linear array
+            self.offset = offset
+            self.increment = increment
+            self._linear = True
+
+    @property  # read only
+    def linear(self):
+        return self._linear
+
+    def __dir__(self):
+        # remove some methods with respect to the full NDArray
+        # as they are not useful for Coord.
+
+        return [
+            "data",
+            "labels",
+            "units",
+            "meta",
+            "title",
+            "name",
+            "offset",
+            "increment",
+            "linear",
+            "size",
+            "roi",
+            "show_datapoints",
+        ]
+
+    def set_laser_frequency(self, frequency=15798.26 * ur("cm^-1")):
+
+        if not isinstance(frequency, Quantity):
+            frequency = frequency * ur("cm^-1")
+
+        frequency.ito("Hz")
+        self.meta.laser_frequency = frequency
+
+        if self._use_time:
+            spacing = 1.0 / frequency
+            spacing.ito("picoseconds")
+
+            self.increment = spacing.m
+            self.offset = 0
+            self._units = ur.picoseconds
+            self.title = "time"
+
+        else:
+            frequency.ito("cm^-1")
+            spacing = 1.0 / frequency
+            spacing.ito("mm")
+
+            self.increment = spacing.m
+            self.offset = -self.increment * self._zpd
+            self._units = ur.mm
+            self.title = "optical path difference"
+
+    @property
+    def _use_time_axis(self):
+        # private property
+        # True if time scale must be used for interferogram axis. Else it
+        # will be set to optical path difference.
+        return self._use_time
+
+    @_use_time_axis.setter
+    def _use_time_axis(self, val):
+
+        self._use_time = val
+        if "laser_frequency" in self.meta:
+            self.set_laser_frequency(self.meta.laser_frequency)
+
+    @property
+    def show_datapoints(self):
+        """
+        Bool : True if axis must discard values and show only datapoints.
+
+        """
+        if "laser_frequency" not in self.meta or self.units.dimensionality not in [
+            "[time]",
+            "[length]",
+        ]:
+            return False
+
+        return self._show_datapoints
+
+    @show_datapoints.setter
+    def show_datapoints(self, val):
+
+        self._show_datapoints = val
+
+    @property
+    def laser_frequency(self):
+        """
+        Laser frequency if needed (Quantity).
+        """
+        return self.meta.laser_frequency
+
+    @laser_frequency.setter
+    def laser_frequency(self, val):
+        self.meta.aser_frequency = val
+
+
+# ======================================================================================
+# Set the operators
+# ======================================================================================
+_set_operators(Coord, priority=50)
+_set_operators(LinearCoord, priority=50)
+
+# ======================================================================================
+if __name__ == "__main__":
+    pass
```

### Comparing `spectrochempy-0.5.5/spectrochempy/analysis/models.py` & `spectrochempy-0.6.1/spectrochempy/analysis/optimize/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,14 @@
                 newargs[index] = _convert_to_units(arg, x_units)
 
         ampl_units = None
         if hasattr(newargs[0], "units"):
             ampl_units = newargs[0].units
             newargs[0] = newargs[0].m
 
-        print(newargs)
         _data = func(cls, x, *newargs)
 
         if returntype == "NDDataset":
             res = NDDataset(_data, units=ampl_units)
             res.x = LinearCoord(xinput)
             res.name = cls.__class__.__name__.split("model")[0]
             res.title = "intensity"
@@ -165,15 +164,15 @@
 class gaussianmodel(object):
     """
     Normalized 1D gaussian function.
 
     .. math::
         f(x) = \\frac{ampl}{\\sqrt{2 \\pi \\sigma^2} } \\exp({\\frac{-(x-pos)^2}{2 \\sigma^2}})
 
-    where :math:`\\sigma = \\frac{width}{2.3548}`.
+    where :math:`\\sigma = \\frac{width}{2.3548}` .
     """
 
     type = "1D"
     args = ["ampl", "pos", "width"]
 
     script = """
     MODEL: line%(id)d\nshape: gaussianmodel
@@ -197,15 +196,15 @@
 class lorentzianmodel(object):
     """
     A standard Lorentzian function (also known as the Cauchy distribution).
 
     .. math::
         f(x) = \\frac{ampl * \\lambda}{\\pi [(x-pos)^2+ \\lambda^2]}
 
-    where :math:`\\lambda = \\frac{width}{2}`.
+    where :math:`\\lambda = \\frac{width}{2}` .
     """
 
     type = "1D"
     args = ["ampl", "pos", "width"]
 
     script = """
     MODEL: line%(id)d\nshape: lorentzianmodel
@@ -224,15 +223,15 @@
 
 # ======================================================================================
 # VoigtModel
 # ======================================================================================
 class voigtmodel(object):
     """
     A Voigt model constructed as the convolution of a :class:`GaussianModel` and
-    a :class:`LorentzianModel`.
+    a :class:`LorentzianModel` .
 
     Commonly used for spectral line fitting.
     """
 
     type = "1D"
     args = ["ampl", "pos", "width", "ratio"]
```

### Comparing `spectrochempy-0.5.5/spectrochempy/analysis/pca.py` & `spectrochempy-0.6.1/spectrochempy/analysis/pca.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,504 +1,523 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
-This module implement the PCA (Principal Component Analysis) class.
+Implementation of Principal Component Analysis (using scikit-learn library)
 """
-
-__all__ = ["PCA"]
-
-__dataset_methods__ = []
-
+import matplotlib.pyplot as plt
 import numpy as np
-from matplotlib import pyplot as plt
+import traitlets as tr
 from matplotlib.ticker import MaxNLocator, ScalarFormatter
-from scipy import special
-from traitlets import HasTraits
+from numpy.random import RandomState
+from sklearn import decomposition
 
-from spectrochempy.analysis.svd import SVD
-from spectrochempy.core import info_
-from spectrochempy.core.dataset.arraymixins.npy import dot
-from spectrochempy.core.dataset.coord import Coord
+from spectrochempy.analysis._base import (
+    DecompositionAnalysis,
+    NotFittedError,
+    _wrap_ndarray_output_to_nddataset,
+)
+from spectrochempy.utils.decorators import signature_has_configurable_traits
+from spectrochempy.utils.docstrings import _docstring
 from spectrochempy.utils.plots import NBlue, NRed
-from spectrochempy.utils.traits import NDDatasetType
+
+__all__ = ["PCA"]
+__configurables__ = ["PCA"]
 
 
 # ======================================================================================
 # class PCA
 # ======================================================================================
-class PCA(HasTraits):
-    """
-    Principal Component Analysis.
+@signature_has_configurable_traits
+class PCA(DecompositionAnalysis):
+    _docstring.delete_params("DecompositionAnalysis.see_also", "PCA")
 
-    This class performs a Principal Component Analysis of a |NDDataset|,
-    *i.e.*, a linear dimensionality reduction using Singular Value
-    Decomposition (`SVD`)
-    of the data to perform its projection to a lower dimensional space.
-
-    The reduction of a dataset :math:`X` with shape (`M`,`N`) is achieved
-    using the decomposition : :math:`X = S.L^T`, where
-    :math:`S` is the score's matrix with shape (`M`, `n_pc`) and :math:`L^T` is
-    the transposed loading's matrix with shape (`n_pc`, `N`).
+    __doc__ = _docstring.dedent(
+        """
+    Principal Component Anamysis (PCA).
 
-    If the dataset `X` contains masked values, these values are silently
-    ignored in the calculation.
+    The Principal Component Analysis analysis is using the
+    `sklearn.decomposition.PCA` model.
 
     Parameters
     ----------
-    dataset : |NDDataset| object
-        The input dataset has shape (M, N). M is the number of
-        observations (for examples a series of IR spectra) while N
-        is the number of features (for example the wavenumbers measured
-        in each IR spectrum).
-    centered : bool, optional, default:True
-        If True the data are centered around the mean values: :math:`X' = X
-        - mean(X)`.
-    standardized : bool, optional, default:False
-        If True the data are scaled to unit standard deviation: :math:`X' =
-        X / \\sigma`.
-    scaled : bool, optional, default:False
-        If True the data are scaled in the interval [0-1]: :math:`X' = (X -
-        min(X)) / (max(X)-min(X))`.
+    %(AnalysisConfigurable.parameters)s
 
     See Also
     --------
-    EFA
-       Perform an Evolving Factor Analysis (forward and reverse) of the input |NDDataset| .
-    NNMF
-       Performs a Non Negative Matrix Factorization of a |NDDataset| .
-    MCRALS
-       Performs MCR-ALS of a |NDDataset| knowing the initial C or St matrix.
+    %(DecompositionAnalysis.see_also.no_PCA)s
     """
+    )
 
-    _LT = NDDatasetType()
-    _S = NDDatasetType()
-    _X = NDDatasetType()
-
-    _ev = NDDatasetType()
-    """|NDDataset| - Explained variances (The eigenvalues of the covariance matrix)."""
-
-    _ev_ratio = NDDatasetType()
-    """|NDDataset| - Explained variance per singular values."""
-
-    _ev_cum = NDDatasetType()
-    """|NDDataset| - Cumulative Explained Variances."""
+    # ----------------------------------------------------------------------------------
+    # Runtime Parameters,
+    # only those specific to PCA, the other being defined in AnalysisConfigurable.
+    # ----------------------------------------------------------------------------------
+    # define here only the variable that you use in fit or transform functions
+    _pca = tr.Instance(
+        decomposition.PCA,
+        help="The instance of sklearn.decomposition.PCA used in this model",
+    )
 
-    def __init__(self, dataset, centered=True, standardized=False, scaled=False):
+    # ----------------------------------------------------------------------------------
+    # Configuration parameters
+    # ----------------------------------------------------------------------------------
+    # sklearn PCA is always on centered data
+    standardized = tr.Bool(
+        default_value=False,
+        help="If True the data are scaled to unit standard deviation: "
+        ":math:`X' = X / \\sigma`",
+    ).tag(config=True)
+
+    scaled = tr.Bool(
+        default_value=False,
+        help="If True the data are scaled in the interval ``[0-1]`` : "
+        ":math:`X' = (X - min(X)) / (max(X)-min(X))``",
+    ).tag(config=True)
+
+    used_components = tr.Union(
+        (tr.Enum(["mle"]), tr.Int(), tr.Float()),
+        allow_none=True,
+        default_value=None,
+        help="""Number of components to keep.
+if `used_components` is not set all components are kept::
+
+    used_components == min(n_observations, n_features)
+
+If ``used_components == 'mle'`` and ``svd_solver == 'full'`` , Minka's MLE is used to guess
+the dimension. Use of ``used_components == 'mle'`` will interpret `svd_solver == 'auto'`
+as ``svd_solver == 'full'`` .
+If `0 < used_components < 1` and `svd_solver == 'full'` , select the number of
+components such that the amount of variance that needs to be explained is greater than
+the percentage specified by used_components.
+If `svd_solver == 'arpack'` , the number of components must be strictly less than the
+minimum of n_features and n_observations. Hence, the None case results in::
+
+    used_components == min(n_observations, n_features) - 1""",
+    ).tag(config=True)
+
+    whiten = tr.Bool(
+        default_value=False,
+        help="""When True (False by default) the `components_` vectors are multiplied
+by the square root of n_observations and then divided by the singular values to ensure
+uncorrelated outputs with unit component-wise variances. Whitening will remove some
+information from the transformed signal (the relative variance scales of the components)
+but can sometime improve the predictive accuracy of the downstream estimators by making
+their data respect some hard-wired assumptions.""",
+    ).tag(config=True)
+
+    svd_solver = tr.Enum(
+        ["auto", "full", "arpack", "randomized"],
+        default_value="auto",
+        help="""If auto :
+The solver is selected by a default policy based on `X.shape`
+and `used_components`: if the input data is larger than 500x500 and the number of
+components to extract is lower than 80% of the smallest dimension of the data, then the
+more efficient 'randomized' method is enabled. Otherwise the exact full SVD is computed
+and optionally truncated afterwards.
+If full :
+run exact full SVD calling the standard LAPACK solver via `scipy.linalg.svd` and select
+the components by postprocessing
+If arpack :
+run SVD truncated to used_components calling ARPACK solver via `scipy.sparse.linalg.svds` .
+It requires strictly 0 < used_components < min(X.shape)
+If randomized :
+run randomized SVD by the method of Halko et al.""",
+    ).tag(config=True)
+
+    tol = tr.Float(
+        default_value=0.0,
+        help="""Tolerance for singular values computed by svd_solver == 'arpack'.
+Must be of range [0.0, infinity).""",
+    ).tag(config=True)
+
+    iterated_power = tr.Union(
+        (tr.Int(), tr.Enum(["auto"])),
+        default_value="auto",
+        help="""Number of iterations for the power method computed by
+svd_solver == 'randomized'. Must be of range [0, infinity).""",
+    ).tag(config=True)
+
+    n_oversamples = tr.Int(
+        default_value=10,
+        help="""This parameter is only relevant when `svd_solver="randomized"` .
+It corresponds to the additional number of random vectors to sample the range of `X` so
+as to ensure proper conditioning. See :func:`~sklearn.utils.extmath.randomized_svd`
+for more details.""",
+    ).tag(config=True)
+
+    power_iteration_normalizer = tr.Enum(
+        ["auto", "QR", "LU", "none"],
+        default_value="auto",
+        help="""Power iteration normalizer for randomized SVD solver. Not used by
+ARPACK. See :func:`~sklearn.utils.extmath.randomized_svd` for more details.""",
+    ).tag(config=True)
+
+    random_state = tr.Union(
+        (tr.Int(), tr.Instance(RandomState)),
+        allow_none=True,
+        default_value=None,
+        help="""Used when the 'arpack' or 'randomized' solvers are used. Pass an int
+for reproducible results across multiple function calls.""",
+    ).tag(config=True)
 
-        super().__init__()
+    # ----------------------------------------------------------------------------------
+    # Initialization
+    # ----------------------------------------------------------------------------------
+    def __init__(
+        self,
+        *,
+        log_level="WARNING",
+        warm_start=False,
+        copy=True,
+        **kwargs,
+    ):
+        # we have changed the name n_components use in sklearn by
+        # used_components (in order  to avoid conflict with the rest of the program)
+        # warn th user:
+        if "n_components" in kwargs:
+            raise KeyError(
+                "`n_components` is not a valid parameter. Did-you mean "
+                "`used_components`?"
+            )
 
-        self.prefs = dataset.preferences
+        # call the super class for initialisation of the configuration parameters
+        # to do before anything else!
+        super().__init__(
+            log_level=log_level,
+            warm_start=warm_start,
+            copy=copy,
+            **kwargs,
+        )
 
-        self._X = X = dataset
+        # initialize sklearn PCA
+        self._pca = decomposition.PCA(
+            n_components=self.used_components,
+            whiten=self.whiten,
+            copy=copy,
+            svd_solver=self.svd_solver,
+            tol=self.tol,
+            iterated_power=self.iterated_power,
+            n_oversamples=self.n_oversamples,
+            power_iteration_normalizer=self.power_iteration_normalizer,
+            random_state=self.random_state,
+        )
 
-        Xsc = X.copy()
+    # ----------------------------------------------------------------------------------
+    # Private methods (overloading abstract classes)
+    # ----------------------------------------------------------------------------------
+    @tr.observe("_X")
+    def _preprocess_as_X_changed(self, change):
 
-        # mean center the dataset
-        # -----------------------
-        self._centered = centered
-        if centered:
-            self._center = center = X.mean(dim=0)
-            Xsc = X - center
-            Xsc.name = f"centered {X.name}"
+        X = change.new
 
         # Standardization
         # ---------------
-        self._standardized = standardized
-        if standardized:
-            self._std = Xsc.std(dim=0)
-            Xsc /= self._std
-            Xsc.name = f"standardized {Xsc.name}"
+        if self.standardized:
+            self._std = X.std(dim=0)
+            X /= self._std
+            X.name = f"standardized {X.name}"
 
         # Scaling
         # -------
-        self._scaled = scaled
-        if scaled:
-            self._min = Xsc.min(dim=0)
-            self._ampl = Xsc.ptp(dim=0)
-            Xsc -= self._min
-            Xsc /= self._ampl
-            Xsc.name = "scaled %s" % Xsc.name
-
-        self._Xscaled = Xsc
-
-        # perform SVD
-        # -----------
-        svd = SVD(Xsc)
-        sigma = svd.s.diag()
-        U = svd.U
-        VT = svd.VT
-
-        # select n_pc loadings & compute scores
-        # ------------------------------------------------------------------------------
-        # loadings
-
-        LT = VT
-        LT.title = "loadings (L^T) of " + X.name
-        LT.history = "Created by PCA"
-
-        # scores
-
-        S = dot(U, sigma)
-        S.title = "scores (S) of " + X.name
-        S.set_coordset(
-            y=X.y,
-            x=Coord(
-                None,
-                labels=["#%d" % (i + 1) for i in range(svd.s.size)],
-                title="principal component",
-            ),
-        )
-
-        S.description = "scores (S) of " + X.name
-        S.history = "Created by PCA"
-
-        self._LT = LT
-        self._S = S
-
-        # other attributes
-        # ----------------
-        self._sv = svd.sv
-        self._sv.x.title = "PC #"
-
-        self._ev = svd.ev
-        self._ev.x.title = "PC #"
-
-        self._ev_ratio = svd.ev_ratio
-        self._ev_ratio.x.title = "PC #"
-
-        self._ev_cum = svd.ev_cum
-        self._ev_cum.x.title = "PC #"
-
-        return
-
-    # ----------------------------------------------------------------------------------
-    # Special methods
-    # ----------------------------------------------------------------------------------
-    def __str__(self, n_pc=5):
-
-        s = "\n"
-        s += "PC\tEigenvalue\t\t%variance\t\t%cumulative\n"
-        s += "  \t of cov(X)\t\t   per PC\t\t   variance\n"
-
-        n_pc = min(n_pc, len(self.ev.data))
-        for i in range(n_pc):
-            tup = (
-                i + 1,
-                np.sqrt(self.ev.data[i]),
-                self.ev_ratio.data[i],
-                self.ev_cum.data[i],
+        if self.scaled:
+            self._min = X.min(dim=0)
+            self._ampl = X.ptp(dim=0)
+            X -= self._min
+            X /= self._ampl
+            X.name = "scaled %s" % X.name
+
+        self._X_preprocessed = X.data
+
+        # final check on the configuration used_components parameter
+        # (which can be done only when X is defined in fit arguments)
+        n_observations, n_features = X.shape
+
+        n_components = self.used_components
+        if n_components is None:
+            pass
+        elif n_components == "mle":
+            if n_observations < n_features:
+                raise ValueError(
+                    "used_components='mle' is only supported if n_observations >= n_features"
+                )
+        elif not 0 <= n_components <= min(n_observations, n_features):
+            raise ValueError(
+                "used_components=%r must be between 0 and "
+                "min(n_observations, n_features)=%r with "
+                "svd_solver='full'" % (n_components, min(n_observations, n_features))
             )
-            s += "#{}\t{:10.3e}\t\t{:9.3f}\t\t{:11.3f}\n".format(*tup)
 
-        return s
+    def _fit(self, X, Y=None):
+        # this method is called by the abstract class fit.
+        # Input X is a np.ndarray
+        # Y is ignored in this model
+
+        # call the sklearn _fit function on data (it outputs SVD results)
+        # _outfit is a tuple handle the eventual output of _fit for further processing.
+
+        # The _outfit members are np.ndarrays
+        _outfit = self._pca.fit(X)
+
+        # get the calculated attribute
+        self._components = self._pca.components_
+
+        self._noise_variance = self._pca.noise_variance_
+        self._n_observations = self._pca.n_samples_
+        self._explained_variance = self._pca.explained_variance_
+        self._explained_variance_ratio = self._pca.explained_variance_ratio_
+        self._singular_values = self._pca.singular_values_
+
+        # unlike to sklearn, we will update the n_components value here with the
+        # eventually calculated ones: this will simplify further process
+        # indeed in sklearn, the value after processing is n_components_
+        # with an underscore at the end
+
+        self._n_components = int(
+            self._pca.n_components_
+        )  # cast the returned int64 to int
+        return _outfit
+
+    def _transform(self, X):
+        return self._pca.transform(X)
+
+    def _inverse_transform(self, X_transform):
+        # we need to  set self._pca.components_ to a compatible size but without
+        # destroying the full matrix:
+        store_components_ = self._pca.components_
+        self._pca.components_ = self._pca.components_[: X_transform.shape[1]]
+        X = self._pca.inverse_transform(X_transform)
+        # restore
+        self._pca.components_ = store_components_
+        return X
+
+    def _get_components(self):
+        self._components = self._pca.components_
+        return self._components
 
     # ----------------------------------------------------------------------------------
-    # Private methods
+    # Public methods and properties specific to PCA
     # ----------------------------------------------------------------------------------
-    def _get_n_pc(self, n_pc=None):
-
-        max_n_pc = self.ev.size
-        if n_pc is None:
-            n_pc = max_n_pc
-            return n_pc
-        elif isinstance(n_pc, int):
-            n_pc = min(n_pc, max_n_pc)
-            return n_pc
-        elif n_pc == "auto":
-            M, N = self.X.shape
-            if M >= N:
-                n_pc = self._infer_pc_()
-                return n_pc
-            else:
-                info_(
-                    "Cannot use `auto` if n_observations < "
-                    "n_features. Try with threshold 0.9999"
-                )
-                n_pc = 0.9999
+    _docstring.keep_params("analysis_fit.parameters", "X")
 
-        if 0 < n_pc < 1.0:
-            # number of PC for which the cumulated explained variance is
-            # less than a given ratio
-            n_pc = np.searchsorted(self.ev_cum.data / 100.0, n_pc) + 1
-            return n_pc
-        else:
-            raise ValueError("could not get a valid number of components")
-
-    def _assess_dimension_(self, rank):
-        """Compute the likelihood of a rank ``rank`` dataset
-        The dataset is assumed to be embedded in gaussian noise having
-        spectrum ``spectrum`` (here, the explained variances `ev` ).
+    @_docstring.dedent
+    def fit(self, X):
+        """
+        Fit the PCA model on X.
 
         Parameters
         ----------
-        rank : int
-            Tested rank value.
+        %(analysis_fit.parameters.X)s
 
         Returns
         -------
-        float
-            The log-likelihood.
-
-        Notes
-        -----
-        This implements the method of Thomas P. Minka :
-        Automatic Choice of Dimensionality for PCA. NIPS 2000 : 598-604.
-        Copied and modified from scikit-learn.decomposition.pca (BSD-3 license)
-        """
-        spectrum = self._ev.data
-        M, N = self._X.shape
-
-        if rank > len(spectrum):
-            raise ValueError("The tested rank cannot exceed the rank of the dataset")
-
-        pu = -rank * np.log(2.0)
-        for i in range(rank):
-            pu += special.gammaln((N - i) / 2.0) - np.log(np.pi) * (N - i) / 2.0
-
-        pl = np.sum(np.log(spectrum[:rank]))
-        pl = -pl * M / 2.0
-
-        if rank == N:
-            pv = 0
-            v = 1
-        else:
-            v = np.sum(spectrum[rank:]) / (N - rank)
-            pv = -np.log(v) * M * (N - rank) / 2.0
-
-        m = N * rank - rank * (rank + 1.0) / 2.0
-        pp = np.log(2.0 * np.pi) * (m + rank + 1.0) / 2.0
-
-        pa = 0.0
-        spectrum_ = spectrum.copy()
-        spectrum_[rank:N] = v
-        for i in range(rank):
-            for j in range(i + 1, len(spectrum)):
-                pa += np.log(
-                    (spectrum[i] - spectrum[j])
-                    * (1.0 / spectrum_[j] - 1.0 / spectrum_[i])
-                ) + np.log(M)
-
-        ll = pu + pl + pv + pp - pa / 2.0 - rank * np.log(M) / 2.0
-
-        return ll
+        %(analysis_fit.returns)s
 
-    def _infer_pc_(self):
-        """Infers the number of principal components.
-
-        Notes
-        -----
-        Copied and modified from _infer_dimensions in
-        scikit-learn.decomposition.pca (BSD-3 license).
+        See Also
+        --------
+        %(analysis_fit.see_also)s
         """
-        n_ev = self._ev.size
-        ll = np.empty(n_ev)
-        for rank in range(n_ev):
-            ll[rank] = self._assess_dimension_(rank)
-        return ll.argmax()
+        return super().fit(X, Y=None)
 
-    # ----------------------------------------------------------------------------------
-    # Public methods
-    # ----------------------------------------------------------------------------------
-    def reduce(self, n_pc=None):
+    @property
+    def loadings(self):
         """
-        Apply a dimensionality reduction to the X dataset of shape [M, N].
-
-        Loadings `L` with shape [``n_pc``, `N`] and scores `S`
-        with shape [`M`, `n_pc`] are obtained using the following
-        decomposition : :math:`X = S.L^T`.
-
-        Parameters
-        ----------
-        n_pc : int, optional
-            The number of principal components to compute. If not set all
-            components are returned, except if n_pc is set to ``auto`` for
-            an automatic determination of the number of components.
-
-        Returns
-        -------
-        S, LT : |NDDataset| objects.
-            n_pc loadings and their corresponding scores for each observations.
+        Return PCA loadings.
         """
+        return self.get_components()
 
-        # get n_pc (automatic or determined by the n_pc arguments)
-        n_pc = self._get_n_pc(n_pc)
-
-        # scores (S) and loading (L^T) matrices
-        # ------------------------------------
-        S = self._S[:, :n_pc]
-        LT = self._LT[:n_pc]
+    @property
+    def scores(self):
+        """
+        Returns PCA scores.
+        """
+        return self.transform(self.X)
 
-        return S, LT
+    @property
+    @_wrap_ndarray_output_to_nddataset(
+        units=None, title="explained variance", typesingle="components"
+    )
+    def explained_variance(self):
+        return self._pca.explained_variance_
 
-    def reconstruct(self, n_pc=None):
-        """
-        Transform data back to the original space using `n_pc` PC's.
+    ev = explained_variance
 
-        The following matrice operation is performed : :math:`X' = S'.L'^T`
-        where S'=S[:, n_pc] and L=L[:, n_pc].
+    @property
+    @_wrap_ndarray_output_to_nddataset(
+        units="percent", title="explained variance ratio", typesingle="components"
+    )
+    def explained_variance_ratio(self):
+        return self._pca.explained_variance_ratio_ * 100.0
 
-        Parameters
-        ----------
-        n_pc : int, optional
-            The number of PC to use for the reconstruction.
+    ev_ratio = explained_variance_ratio
 
-        Returns
-        -------
-        |NDDataset|
-            The reconstructed dataset based on n_pc principal components.
-        """
+    @property
+    @_wrap_ndarray_output_to_nddataset(
+        units="percent", title="cumulative explained variance", typesingle="components"
+    )
+    def cumulative_explained_variance(self):
+        return np.cumsum(self._pca.explained_variance_ratio_) * 100.0
 
-        # get n_pc (automatic or determined by the n_pc arguments)
-        n_pc = self._get_n_pc(n_pc)
+    ev_cum = cumulative_explained_variance
 
-        # reconstruct from scores and loadings using n_pc components
-        S = self._S[:, :n_pc]
-        LT = self._LT[:n_pc]
-
-        X = dot(S, LT)
-
-        # try to reconstruct something close to the original scaled, standardized or centered data
-        if self._scaled:
-            X *= self._ampl
-            X += self._min
-        if self._standardized:
-            X *= self._std
-        if self._centered:
-            X += self._center
-
-        X.history = f"PCA reconstructed Dataset with {n_pc} principal components"
-        X.name = self._X.name
-        X.title = self._X.title
-        return X
+    # ----------------------------------------------------------------------------------
+    # Reporting specific to PCA
+    # ----------------------------------------------------------------------------------
+    def __str__(self, n_components=5):
 
-    def plotmerit(self, n_pc=None, **kwargs):
-        """
-        Plots the input dataset, reconstructed dataset and residuals.
+        if not self._fitted:
+            raise NotFittedError(
+                f"The fit method must be used prior using the {self.name} model"
+            )
 
-        Parameters
-        ----------
-        **kwargs
-            optional "colors" argument: tuple or array of 3 colors for :math:`X`, :math:`\hat X` and :math:`E`.
+        s = "\n"
+        s += "PC\tEigenvalue\t\t%variance\t\t%cumulative\n"
+        s += "  \t of cov(X)\t\t   per PC\t\t   variance\n"
 
-        Returns
-        -------
-        ax
-            subplot.
-        """
-        colX, colXhat, colRes = kwargs.get("colors", ["blue", "green", "red"])
+        if n_components is None or n_components > self.n_components:
+            n_components = self.n_components
+        for i in range(n_components):
+            tup = (
+                i + 1,
+                np.sqrt(self.ev.data[i]),
+                self.ev_ratio.data[i],
+                self.ev_cum.data[i],
+            )
+            s += "#{}\t{:10.3e}\t\t{:9.3f}\t\t{:11.3f}\n".format(*tup)
 
-        X_hat = self.reconstruct(n_pc=n_pc)
-        res = self.X - X_hat
-        ax = self.X.plot()
-        if self.X.x is not None:
-            ax.plot(self.X.x.data, X_hat.T.data, color=colXhat)
-            ax.plot(self.X.x.data, res.T.data, color=colRes)
-        else:
-            ax.plot(X_hat.T.data, color=colXhat)
-            ax.plot(res.T.data, color=colRes)
-        ax.autoscale(enable=True)
-        ax.set_title("PCA merit plot")
-        return ax
+        return s
 
-    def printev(self, n_pc=None):
+    def printev(self, n_components=None):
         """
         Print PCA figures of merit.
 
         Prints eigenvalues and explained variance for all or first n_pc PC's.
 
         Parameters
         ----------
         n_pc : int, optional
             The number of components to print.
         """
-        # get n_pc (automatic or determined by the n_pc arguments)
-        n_pc = self._get_n_pc(n_pc)
+        if not self._fitted:
+            raise NotFittedError(
+                "The fit method must be used " "before using this method"
+            )
 
-        print((self.__str__(n_pc)))
+        if n_components is None or n_components > self.n_components:
+            n_components = self.n_components
+        print((self.__str__(n_components)))
 
-    def screeplot(self, n_pc=None, **kwargs):
+    # ----------------------------------------------------------------------------------
+    # Plot methods specific to PCA
+    # ----------------------------------------------------------------------------------
+    def screeplot(self, n_components=None, **kwargs):
         """
         Scree plot of explained variance + cumulative variance by PCA.
 
         Explained variance by each PC is plot as a bar graph (left y axis)
         and cumulative explained variance is plot as a scatter plot with lines
         (right y axis).
 
         Parameters
         ----------
-        n_pc : int
+        n_components : int
             Number of components to plot.
-
         **kwargs
-            Extra arguments: `colors` (default: `[NBlue, NRed]`) to set the colors
-            of the bar plot and scatter plot; `ylims` (default `[(0, 100), "auto"]`).
+            Extra arguments: `colors` (default: ``[NBlue, NRed]`` ) to set the colors
+            of the bar plot and scatter plot; ``ylims`` (default ``[(0, 100), "auto"]``\ ).
 
         Returns
         -------
-            list of axes
-                The list of axes.
+        `list` of `~matplotlib.axes.Axes`
+            The list of axes.
         """
-        # get n_pc (automatic or determined by the n_pc arguments) - min = 3
-        n_pc = max(self._get_n_pc(n_pc), 3)
+        # get n_components
+        if n_components is None:
+            n_components = self.n_components
+        else:
+            n_components = min(self.n_components, n_components)
 
         color1, color2 = kwargs.get("colors", [NBlue, NRed])
         # pen = kwargs.get('pen', True)
         ylim1, ylim2 = kwargs.get("ylims", [(0, 100), "auto"])
 
         if ylim2 == "auto":
-            y1 = np.around(self._ev_ratio.data[0] * 0.95, -1)
+            y1 = np.around(self.ev_ratio.data[0] * 0.95, -1)
             y2 = 101.0
             ylim2 = (y1, y2)
 
-        ax1 = self._ev_ratio[:n_pc].plot_bar(
+        ax1 = self.ev_ratio[:n_components].plot_bar(
             ylim=ylim1, color=color1, title="Scree plot"
         )
-        ax2 = self._ev_cum[:n_pc].plot_scatter(
+        ax2 = self.ev_cum[:n_components].plot_scatter(
             ylim=ylim2, color=color2, pen=True, markersize=7.0, twinx=ax1
         )
         ax1.set_title("Scree plot")
         return ax1, ax2
 
     def scoreplot(
         self,
-        *pcs,
+        *args,
         colormap="viridis",
         color_mapping="index",
         show_labels=False,
         labels_column=0,
         labels_every=1,
         **kwargs,
     ):
         """
-        2D or 3D scoreplot of samples.
+        2D or 3D scoreplot of observations.
+
+        Plots the projection of each observation/spectrum onto the span of two or
+        three selected principal components.
 
         Parameters
         ----------
-        *pcs : a series of int argument or a list/tuple
-            Must contain 2 or 3 elements.
+        *args : `NDDataset` and/or series of 2 or 3 ints or iterabble of 2 or 3 int, optional
+            The `NDDataset` contains the sores to plot. If not provided `PCA.scores`
+            is used. The 2 or 3 int are the PC on which the projection is shown. If not
+            provided, default to [1,2], i.e. bidimensional plot on PCs #1 and #2.
         colormap : str
             A matplotlib colormap.
         color_mapping : 'index' or 'labels'
             If 'index', then the colors of each n_scores is mapped sequentially
             on the colormap. If labels, the labels of the n_observations are
             used for color mapping.
         show_labels : bool, optional, default: False
             If True each observation will be annotated with its label.
         labels_column : int, optional, default:0
             If several columns of labels are present indicates which column has to be
             used to show labels.
         labels_every : int, optional, default: 1
         `   Do not label all points, but only every value indicated by this parameter.
+
+        Returns
+        -------
+        `~matplotlib.axes.Axes`
+            The axes
         """
         self.prefs = self.X.preferences
-        scores = self._S
+
+        # checks args
+        if len(args) > 0:
+            scores = args[0]
+            if hasattr(scores, "_implements") and scores._implements("NDDataset"):
+                if len(args) > 1:
+                    pcs = args[1:]
+                else:
+                    pcs = 1, 2
+            else:
+                scores = self.scores
+                pcs = args
+        else:
+            scores = self.scores
+            pcs = 1, 2
 
         if isinstance(pcs[0], (list, tuple, set)):
             pcs = pcs[0]
 
         # transform to internal index of component's index (1->0 etc...)
         pcs = np.array(pcs) - 1
 
@@ -515,15 +534,20 @@
             else:
                 labels = list(set(scores.y.labels[:, labels_column]))
             colors = [labels.index(lab) for lab in scores.y.labels]
 
         # labels
         scatterlabels = None
         if show_labels:
-            scatterlabels = scores.y.labels[:, labels_column]
+            if scores.y.labels is None:
+                raise ValueError("You set show_label to true but score.y has no label")
+            elif scores.y.labels.ndim == 1:
+                scatterlabels = scores.y.labels
+            else:
+                scatterlabels = scores.y.labels[:, labels_column]
 
         if len(pcs) == 2:
             # bidimensional score plot
 
             fig = plt.figure(**kwargs)
             ax = fig.add_subplot(111)
             ax.set_title("Score plot")
@@ -562,21 +586,21 @@
 
         if len(pcs) == 3:
             # tridimensional score plot
             plt.figure(**kwargs)
             ax = plt.axes(projection="3d")
             ax.set_title("Score plot")
             ax.set_xlabel(
-                "PC# {} ({:.3f}%)".format(pcs[0] + 1, self._ev_ratio.data[pcs[0]])
+                "PC# {} ({:.3f}%)".format(pcs[0] + 1, self.ev_ratio.data[pcs[0]])
             )
             ax.set_ylabel(
-                "PC# {} ({:.3f}%)".format(pcs[1] + 1, self._ev_ratio.data[pcs[1]])
+                "PC# {} ({:.3f}%)".format(pcs[1] + 1, self.ev_ratio.data[pcs[1]])
             )
             ax.set_zlabel(
-                "PC# {} ({:.3f}%)".format(pcs[2] + 1, self._ev_ratio.data[pcs[2]])
+                "PC# {} ({:.3f}%)".format(pcs[2] + 1, self.ev_ratio.data[pcs[2]])
             )
             axsc = ax.scatter(
                 scores.masked_data[:, pcs[0]],
                 scores.masked_data[:, pcs[1]],
                 scores.masked_data[:, pcs[2]],
                 zdir="z",
                 s=30,
@@ -594,58 +618,10 @@
                 c = axsc.get_cmap().colors[int(255 / (len(labels) - 1) * i)]
                 leg.append(mpatches.Patch(color=c, label=lab))
 
             ax.legend(handles=leg, loc="best")
 
         return ax
 
-    @property
-    def LT(self):
-        """
-        LT.
-        """
-        return self._LT
-
-    @property
-    def S(self):
-        """
-        S.
-        """
-        return self._S
-
-    def labels(self, value):
-        self._S.y.labels = value
-
-    @property
-    def X(self):
-        """
-        X.
-        """
-        return self._X
-
-    @property
-    def ev(self):
-        """
-        Explained variances (|NDDataset|).
-
-        (The eigenvalues of the covariance matrix).
-        """
-        return self._ev
-
-    @property
-    def ev_ratio(self):
-        """
-        Explained variance per singular values (|NDDataset|).
-        """
-        return self._ev_ratio
-
-    @property
-    def ev_cum(self):
-        """
-        Cumulative Explained Variances (|NDDataset|).
-        """
-        return self._ev_cum
-
 
-# ============================================================================
 if __name__ == "__main__":
     pass
```

### Comparing `spectrochempy-0.5.5/spectrochempy/analysis/peakfinding.py` & `spectrochempy-0.6.1/spectrochempy/analysis/peakfinding.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 Peak finding module.
 
-Contains wrappers of scipy.signal peak finding functions.
+Contains wrappers of `scipy.signal` peak finding functions.
 """
 
 __all__ = ["find_peaks"]
 
 __dataset_methods__ = ["find_peaks"]
 
 from datetime import datetime, timezone
 
 import numpy as np
-from scipy import signal
+import scipy
 
 from spectrochempy.core.dataset.coord import Coord
 
 # Todo:
-# find_peaks_cwt(vector, widths[, wavelet, ...]) 	Attempt to find the peaks in a 1-D array.
+# find_peaks_cwt(vector, widths[, wavelet, ...]) Attempt to find the peaks in a 1-D array.
 # argrelmin(data[, axis, order, mode]) 	Calculate the relative minima of data.
 # argrelmax(data[, axis, order, mode]) 	Calculate the relative maxima of data.
 # argrelextrema(data, comparator[, axis, ...]) 	Calculate the relative extrema of data.
 
 
 def find_peaks(
     dataset,
@@ -38,154 +38,158 @@
     width=None,
     wlen=None,
     rel_height=0.5,
     plateau_size=None,
     use_coord=True,
 ):
     """
-    Wrapper and extension of scpy.signal.find_peaks().
+    Wrapper and extension of `scpy.signal.find_peaks`\ .
 
-    Find peaks inside a 1D NDDataset based on peak properties.
-    This function finds all local maxima by simple comparison of neighbouring values. Optionally, a subset of these
+    Find peaks inside a 1D `NDDataset` based on peak properties.
+    This function finds all local maxima by simple comparison of neighbouring values.
+    Optionally, a subset of these
     peaks can be selected by specifying conditions for a peak's properties.
 
-    ..warning::
+    .. warning::
 
-      This function may return unexpected results for data containing NaNs.
-      To avoid this, NaNs should either be removed or replaced.
+        This function may return unexpected results for data containing NaNs.
+        To avoid this, NaNs should either be removed or replaced.
 
     Parameters
     ----------
-    dataset : |NDDataset|
-        A 1D NDDataset or a 2D NDdataset with `len(X.y) == 1`.
-    height : number or ndarray or sequence, optional
-        Required height of peaks. Either a number, ``None``, an array matching
+    dataset : `NDDataset`
+        A 1D NDDataset or a 2D NDdataset with `len(X.y) == 1` .
+    height : `float` or :term:`array-like`\ , optional, default: `None`
+        Required height of peaks. Either a number, `None` , an array matching
         `x` or a 2-element sequence of the former. The first element is
-        always interpreted as the  minimal and the second, if supplied, as the
+        always interpreted as the minimal and the second, if supplied, as the
         maximal required height.
-    window_length : int, default: 5
-        The length of the filter window used to interpolate the maximum. window_length must be a positive odd integer.
+    window_length : `int`, default: 5
+        The length of the filter window used to interpolate the maximum. window_length
+        must be a positive odd integer.
         If set to one, the actual maximum is returned.
-    threshold : number or ndarray or sequence, optional
+    threshold : `float` or :term:`array-like`\ , optional
         Required threshold of peaks, the vertical distance to its neighbouring
-        samples. Either a number, ``None``, an array matching `x` or a
+        samples. Either a number, `None` , an array matching `x` or a
         2-element sequence of the former. The first element is always
         interpreted as the  minimal and the second, if supplied, as the maximal
         required threshold.
-    distance : number, optional
+    distance : `float`\ , optional
         Required minimal horizontal distance in samples between
         neighbouring peaks. Smaller peaks are removed first until the condition
         is fulfilled for all remaining peaks.
-    prominence : number or ndarray or sequence, optional
-        Required prominence of peaks. Either a number, ``None``, an array
+    prominence : `float` or :term:`array-like`\ , optional
+        Required prominence of peaks. Either a number, `None` , an array
         matching `x` or a 2-element sequence of the former. The first
         element is always interpreted as the  minimal and the second, if
         supplied, as the maximal required prominence.
-    width : number or ndarray or sequence, optional
-        Required width of peaks in samples. Either a number, ``None``, an array
+    width : `float` or :term:`array-like`\ , optional
+        Required width of peaks in samples. Either a number, `None` , an array
         matching `x` or a 2-element sequence of the former. The first
         element is always interpreted as the  minimal and the second, if
         supplied, as the maximal required width. Floats are interpreted as width
         measured along the 'x' Coord; ints are interpreted as a number of points.
-    wlen : int or float, optional
+    wlen : `int` or `float`, optional
         Used for calculation of the peaks prominences, thus it is only used if
         one of the arguments `prominence` or `width` is given. Floats are interpreted
         as measured along the 'x' Coord; ints are interpreted as a number of points.
         See argument len` in `peak_prominences` of the scipy documentation for a full
         description of its effects.
-    rel_height : float, optional,
+    rel_height : `float`, optional,
         Used for calculation of the peaks width, thus it is only used if `width`
         is given. See argument  `rel_height` in `peak_widths` of the scipy documentation
         for a full description of its effects.
-    plateau_size : number or ndarray or sequence, optional
+    plateau_size : `float` or :term:`array-like`\ , optional
         Required size of the flat top of peaks in samples. Either a number,
-        ``None``, an array matching `x` or a 2-element sequence of the former.
+        `None` , an array matching `x` or a 2-element sequence of the former.
         The first element is always interpreted as the minimal and the second,
         if supplied as the maximal required plateau size. Floats are interpreted
         as measured along the 'x' Coord; ints are interpreted as a number of points.
-    use_coord : bool, optional
+    use_coord : `bool`\ , optional
         Set whether the x Coord (when it exists) should be used instead of indices
         for the positions and width. If True, the units of the other parameters
         are interpreted according to the coordinates.
 
     Returns
     -------
-    peaks : ndarray
-        Indices of peaks in `x` that satisfy all given conditions.
+    peaks : `~numpy.ndarray`
+        Indices of peaks in `dataset` that satisfy all given conditions.
 
-    properties : dict
+    properties : `dict`
         A dictionary containing properties of the returned peaks which were
         calculated as intermediate results during evaluation of the specified
         conditions:
 
-        * peak_heights
-              If `height` is given, the height of each peak in `x`.
-        * left_thresholds, right_thresholds
-              If `threshold` is given, these keys contain a peaks vertical
-              distance to its neighbouring samples.
-        * prominences, right_bases, left_bases
-              If `prominence` is given, these keys are accessible. See
-              `peak_prominences` in scipy documentation for a description of their content.
-        * width_heights, left_ips, right_ips
-              If `width` is given, these keys are accessible. See `peak_widths`
-              in scipy documentation for a description of their content.
+        * ``peak_heights``
+            If `height` is given, the height of each peak in `dataset`\  .
+        * ``left_thresholds``\ , ``right_thresholds``
+            If `threshold` is given, these keys contain a peaks vertical
+            distance to its neighbouring samples.
+        * ``prominences``\ , ``right_bases``\ , ``left_bases``
+            If `prominence` is given, these keys are accessible. See
+            `scipy.signal.peak_prominences` for a
+            full description of their content.
+        * ``width_heights``\ , ``left_ips``\ , ``right_ips``
+            If `width` is given, these keys are accessible. See
+            `scipy.signal.peak_widths` for a full description of their content.
         * plateau_sizes, left_edges', 'right_edges'
-              If `plateau_size` is given, these keys are accessible and contain
-              the indices of a peak's edges (edges are still part of the
-              plateau) and the calculated plateau sizes.
+            If `plateau_size` is given, these keys are accessible and contain
+            the indices of a peak's edges (edges are still part of the
+            plateau) and the calculated plateau sizes.
 
         To calculate and return properties without excluding peaks, provide the
-        open interval ``(None, None)`` as a value to the appropriate argument
-        (excluding `distance`).
+        open interval `(None, None)` as a value to the appropriate argument
+        (excluding `distance`\ ).
 
     Warns
     -----
     PeakPropertyWarning
         Raised if a peak's properties have unexpected values (see
-        `peak_prominences` and `peak_widths`).
+        `peak_prominences` and `peak_widths` ).
 
     See Also
     --------
     find_peaks_cwt:
-        In scipy.signal: Find peaks using the wavelet transformation.
+        In `scipy.signal`: Find peaks using the wavelet transformation.
     peak_prominences:
-        In scipy.signal: Directly calculate the prominence of peaks.
+        In `scipy.signal`: Directly calculate the prominence of peaks.
     peak_widths:
-        In scipy.signal: Directly calculate the width of peaks.
+        In `scipy.signal`: Directly calculate the width of peaks.
 
     Notes
     -----
     In the context of this function, a peak or local maximum is defined as any
     sample whose two direct neighbours have a smaller amplitude. For flat peaks
     (more than one sample of equal amplitude wide) the index of the middle
     sample is returned (rounded down in case the number of samples is even).
     For noisy signals the peak locations can be off because the noise might
     change the position of local maxima. In those cases consider smoothing the
     signal before searching for peaks or use other peak finding and fitting
-    methods (like `find_peaks_cwt`).
+    methods (like `scipy.signal.find_peaks_cwt` ).
+
     Some additional comments on specifying conditions:
 
-    * Almost all conditions (excluding `distance`) can be given as half-open or
-      closed intervals, e.g ``1`` or ``(1, None)`` defines the half-open
-      interval :math:`[1, \\infty]` while ``(None, 1)`` defines the interval
-      :math:`[-\\infty, 1]`. The open interval ``(None, None)`` can be specified
+    * Almost all conditions (excluding `distance`\ ) can be given as half-open or
+      closed intervals, e.g `1` or `(1, None)` defines the half-open
+      interval :math:`[1, \\infty]` while `(None, 1)` defines the interval
+      :math:`[-\\infty, 1]`\ . The open interval `(None, None)` can be specified
       as well, which returns the matching properties without exclusion of peaks.
     * The border is always included in the interval used to select valid peaks.
     * For several conditions the interval borders can be specified with
-      arrays matching `x` in shape which enables dynamic constrains based on
+      arrays matching `dataset` in shape which enables dynamic constrains based on
       the sample position.
-    * The conditions are evaluated in the following order: `plateau_size`,
-      `height`, `threshold`, `distance`, `prominence`, `width`. In most cases
+    * The conditions are evaluated in the following order: `plateau_size` ,
+      `height` , `threshold` , `distance` , `prominence` , `width` . In most cases
       this order is the fastest one because faster operations are applied first
       to reduce the number of peaks that need to be evaluated later.
     * While indices in `peaks` are guaranteed to be at least `distance` samples
-      apart, edges of flat peaks may be closer than the allowed `distance`.
+      apart, edges of flat peaks may be closer than the allowed `distance` .
     * Use `wlen` to reduce the time it takes to evaluate the conditions for
-      `prominence` or `width` if `x` is large or has many local maxima
-      (see `peak_prominences`).
+      `prominence` or `width` if `dataset` is large or has many local maxima
+      (see `scipy.signal.peak_prominences`\ ).
 
     Examples
     --------
 
     >>> dataset = scp.NDDataset.read("irdata/nh4y-activation.spg")
     >>> X = dataset[0, 1800.0:1300.0]
     >>> peaks, properties = X.find_peaks(height=1.5, distance=50.0, width=0.0)
@@ -223,15 +227,15 @@
     # transform coord (if exists) to index
     distance = int(round(distance / step)) if distance is not None else None
     width = int(round(width / step)) if width is not None else None
     wlen = int(round(wlen / step)) if wlen is not None else None
     plateau_size = int(round(plateau_size / step)) if plateau_size is not None else None
 
     # now the distance, width ... parameters are given in data points
-    peaks, properties = signal.find_peaks(
+    peaks, properties = scipy.signal.find_peaks(
         X.data,
         height=height,
         threshold=threshold,
         distance=distance,
         prominence=prominence,
         width=width,
         wlen=wlen,
```

### Comparing `spectrochempy-0.5.5/spectrochempy/analysis/simplisma.py` & `spectrochempy-0.6.1/spectrochempy/analysis/simplisma.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,223 +5,293 @@
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 This module implement the SIMPLISMA class.
 """
 
 __all__ = ["SIMPLISMA"]
+__configurables__ = ["SIMPLISMA"]
 
-__dataset_methods__ = []
-
-import warnings
+from warnings import warn
 
 import numpy as np
-from traitlets import HasTraits, Unicode
+import traitlets as tr
 
-from spectrochempy.core import INFO, info_, set_loglevel
-from spectrochempy.core.dataset.arraymixins.npy import dot
-from spectrochempy.core.dataset.nddataset import NDDataset
+from spectrochempy.analysis._base import DecompositionAnalysis
+from spectrochempy.core import info_
 from spectrochempy.utils import exceptions
-from spectrochempy.utils.traits import NDDatasetType
+from spectrochempy.utils.decorators import deprecated, signature_has_configurable_traits
+from spectrochempy.utils.docstrings import _docstring
 
 
 # ======================================================================================
 # class SIMPLISMA
 # ======================================================================================
-class SIMPLISMA(HasTraits):
-    """
-    SIMPLe to use Interactive Self-modeling Mixture Analysis.
+@signature_has_configurable_traits
+class SIMPLISMA(DecompositionAnalysis):
+    _docstring.delete_params("DecompositionAnalysis.see_also", "SIMPLISMA")
 
-    This class performs a SIMPLISMA analysis of a 2D |NDDataset| . The algorithm is adapted from Windig's paper,
-    Chemometrics and Intelligent Laboratory Systems, 36, 1997, 3-16.
+    __doc__ = _docstring.dedent(
+        """
+    SIMPLe to use Interactive Self-modeling Mixture Analysis (SIMPLISMA).
 
-    TODO : adapt to 3DDataset ?
+    This class performs a SIMPLISMA analysis of a 2D `NDDataset` .
+    The algorithm is adapted from :cite:t:`windig:1997`\ .
 
     Parameters
     ----------
-    dataset : |NDDataset|
-        A 2D dataset containing the data matrix (spectra in rows).
-    interactive : bool, optional, default=False
-        If True, the determination of purest variables is carried out
-        interactively
-    n_pc : int, optional, default=2 in non-interactive mode; 100 in
-    interactive mode
-        The maximum number of pure compounds. Used only for non interactive
-        analysis
-        (the default in interactive mode (100) will never be reached in
-        practice).
-    tol : float, optional, default=0.1
-        The convergence criterion on the percent of unexplained variance.
-    noise : float or int, optional, default=5
-        A correction factor (%) for low intensity variables (0 - no offset,
-        15 - large offset).
-    """
-
-    _St = NDDatasetType()
-    _C = NDDatasetType()
-    _X = NDDatasetType()
-    _Pt = NDDatasetType()
-    _s = NDDatasetType()
-    _logs = Unicode()
-
-    def __init__(self, dataset, **kwargs):
+    %(AnalysisConfigurable.parameters)s
 
-        super().__init__()
+    See Also
+    --------
+    %(DecompositionAnalysis.see_also.no_SIMPLISMA)s
+    """
+    )
 
-        # ------------------------------------------------------------------------------
-        # Utility functions
-        # ------------------------------------------------------------------------------
-        def figures_of_merit(X, maxPIndex, C, St, j):
-            # return %explained variance and stdev of residuals when the jth compound is added
-            C[:, j] = X[:, maxPIndex[j]]
-            St[0 : j + 1, :] = np.linalg.lstsq(
-                C.data[:, 0 : j + 1], X.data, rcond=None
-            )[0]
-            Xhat = dot(C[:, 0 : j + 1], St[0 : j + 1, :])
-            res = Xhat - X
-            stdev_res = np.std(res)
-            rsquare = 1 - np.linalg.norm(res) ** 2 / np.linalg.norm(X) ** 2
-            return rsquare, stdev_res
+    # TODO : adapt to 3DDataset ?
 
-        def str_iter_summary(j, index, coord, rsquare, stdev_res, diff):
-            # return formatted list of figure of merits at a given iteration
+    # ----------------------------------------------------------------------------------
+    # Runtime Parameters,
+    # only those specific to PCA, the other being defined in AnalysisConfigurable.
+    # ----------------------------------------------------------------------------------
+    # define here only the variable that you use in fit or transform functions
+
+    # ----------------------------------------------------------------------------------
+    # Configuration parameters
+    # They will be written in a file from which the default can be modified)
+    # Obviously, the parameters can also be modified at runtime as usual by assignment.
+    # ----------------------------------------------------------------------------------
+    interactive = tr.Bool(
+        default_value=False,
+        help=(
+            "If True, the determination of purest variables is carried out "
+            "interactively"
+        ),
+    ).tag(config=True)
+    max_components = tr.Integer(
+        default_value=2,
+        help=(
+            "The maximum number of pure compounds. Used only for non interactive"
+            "analysis"
+        ),
+    ).tag(config=True)
+    tol = tr.Float(
+        default_value=0.1,
+        help="The convergence criterion on the percent of unexplained variance.",
+    ).tag(config=True)
+    noise = tr.Float(
+        default_value=3,
+        help=(
+            "A correction factor (%) for low intensity variables (0 - no offset, "
+            "15 - large offset"
+        ),
+    ).tag(config=True)
+
+    # ----------------------------------------------------------------------------------
+    # Initialization
+    # ----------------------------------------------------------------------------------
+    def __init__(
+        self,
+        *args,
+        log_level="WARNING",
+        warm_start=False,
+        copy=True,
+        **kwargs,
+    ):
+        if len(args) > 0:
+            raise ValueError(
+                "Passing arguments such as SIMPLISMA(X) is now deprecated. "
+                "Instead, use SIMPLISMA() followed by SIMPLISMA.fit(X). "
+                "See the documentation and exemples"
+            )
 
-            string = "{:4}  {:5}  {:8.1f} {:10.4f} {:10.4f} ".format(
-                j + 1, index, coord, stdev_res, rsquare
+        # warn about deprecations
+        # -----------------------
+        if "verbose" in kwargs:
+            deprecated("verbose", replace="log_level='INFO'", removed="0.6.5")
+            verbose = kwargs.pop("verbose")
+            if verbose:
+                log_level = "INFO"
+
+        # unimodMod deprecation
+        if "n_pc" in kwargs:
+            deprecated("n_pc", replace="max_components", removed="0.6.5")
+            kwargs["max_components"] = kwargs.pop("n_pc")
+
+        # call the super class for initialisation
+        super().__init__(
+            log_level=log_level,
+            warm_start=warm_start,
+            copy=copy,
+            **kwargs,
+        )
+
+    # ----------------------------------------------------------------------------------
+    # Private validation methods and default getter
+    # ----------------------------------------------------------------------------------
+    @tr.validate("max_components")
+    def _max_components_validate(self, proposal):
+        n = proposal.value
+        if n < 2:
+            raise ValueError(
+                "Oh you did not just... 'MA' in simplisMA stands for Mixture Analysis. "
+                "The number of pure compounds should be an integer larger than 2"
             )
-            return string
+        return n  # <-- do not forget this, or the returned value
+        # for max_components is None
 
-        def get_x_data(X):
-            if X.x is not None and not X.x.is_empty:  # TODO what about labels?
-                return X.x.data
-            else:
-                return np.arange(X.shape[-1])
+    @tr.default("_components")
+    def _components_default(self):
+        if self._fitted:
+            return self._outfit[1]
+        else:
+            raise exceptions.NotFittedError(
+                "The model was not yet fitted. Execute `fit` first!"
+            )
 
-        # ------------------------------------------------------------------------------
-        # Check data
-        # ------------------------------------------------------------------------------
-        X = dataset
+    # ------------------------------------------------------------------------------
+    # Utility functions
+    # ------------------------------------------------------------------------------
+    @staticmethod
+    def _figures_of_merit(X, maxPIndex, C, St, j):
+        # return %explained variance and stdev of residuals when the jth compound
+        # is added
+        C[:, j] = X[:, maxPIndex[j]]
+        St[0 : j + 1, :] = np.linalg.lstsq(C[:, 0 : j + 1], X, rcond=None)[0]
+        Xhat = np.dot(C[:, 0 : j + 1], St[0 : j + 1, :])
+        res = Xhat - X
+        stdev_res = np.std(res)
+        rsquare = 1 - np.linalg.norm(res) ** 2 / np.linalg.norm(X) ** 2
+        return rsquare, stdev_res
+
+    @staticmethod
+    def _str_iter_summary(j, index, coord, rsquare, stdev_res, diff):
+        # return formatted list of figure of merits at a given iteration
+
+        string = "{:4}  {:5}  {:8.1f} {:10.4f} {:10.4f} ".format(
+            j + 1, index, coord, stdev_res, rsquare
+        )
+        return string
+
+    # ----------------------------------------------------------------------------------
+    # Private methods (overloading abstract classes)
+    # ----------------------------------------------------------------------------------
+    @tr.observe("_X")
+    def _preprocess_as_X_changed(self, change):
+        X = change.new
 
+        # add some validation
         if len(X.shape) != 2:
             raise ValueError("For now, SIMPLISMA only handles 2D Datasets")
 
-        if np.min(X.data) < 0:
-            warnings.warn("SIMPLISMA does not handle easily negative values.")
+        if np.min(X) < 0:
+            warn("SIMPLISMA does not handle easily negative values.")
             # TODO: check whether negative values should be set to zero or not.
 
-        if "verbose" in kwargs.keys():
-            exceptions.deprecated(
-                "verbose", replace="use set_loglevel(INFO) before launching SIMPLISMA"
-            )
-            set_loglevel(INFO)
+        self._X_preprocessed = X.data
+        # also store the name for future display
+        self._Xname = X.name
+
+    def _fit(self, X, Y=None):
+        # remember most of the treatments is done in the abstract method
+        # X is _X_preprocessed, so just a np.ndarray
+        # Y is ignored
+
+        interactive = self.interactive
+        tol = self.tol
+        noise = self.noise
+        n_components = self.max_components
+        M, N = X.shape
+        xdata = np.arange(N)
 
-        interactive = kwargs.get("interactive", False)
-        tol = kwargs.get("tol", 0.1)
-        noise = kwargs.get("noise", 3)
-        n_pc = kwargs.get("n_pc", 2)
-        if n_pc < 2 or not isinstance(n_pc, int):
-            raise ValueError(
-                "Oh you did not just... 'MA' in simplisMA stands for Mixture Analysis. "
-                "The number of pure compounds should be an integer larger than 2"
-            )
         if interactive:
-            n_pc = 100
+            n_components = 100
 
         # ------------------------------------------------------------------------------
         # Core
         # ------------------------------------------------------------------------------
         if not interactive:
-            logs = "*** Automatic SIMPL(I)SMA analysis *** \n"
+            info_("*** Automatic SIMPL(I)SMA analysis ***")
         else:
-            logs = "*** Interactive SIMPLISMA analysis *** \n"
-        logs += "dataset: {}\n".format(X.name)
-        logs += "  noise: {:2} %\n".format(noise)
+            info_("*** Interactive SIMPLISMA analysis ***")
+
+        info_(f"     dataset: {self._Xname}")
+        info_(f"       noise: {noise:2} %")
         if not interactive:
-            logs += "    tol: {:2} %\n".format(tol)
-            logs += "   n_pc: {:2}\n".format(n_pc)
-        logs += "\n"
-        logs += "#iter index_pc  coord_pc   Std(res)   R^2   \n"
-        logs += "---------------------------------------------"
-        info_(logs)
-        logs += "\n"
+            info_(f"         tol: {tol:2} %")
+            info_(f"n_components: {n_components:2}")
+        info_("\n")
+        info_("#iter index_pc  coord_pc   Std(res)   R^2    ")
+        info_("---------------------------------------------")
 
         # Containers for returned objects and intermediate data
         # ---------------------------------------------------
         # purity 'spectra' (generally spectra if X is passed,
         # but could also be concentrations if X.T is passed)
-        Pt = NDDataset.zeros((n_pc, X.shape[-1]))
-        Pt.name = "Purity spectra"
-        Pt.set_coordset(y=Pt.y, x=X.x)
-        Pt.y.title = "# pure compound"
+        Pt = np.zeros((n_components, N))
+        # Pt.name = "Purity spectra"
+        # Pt.set_coordset(y=Pt.y, x=X.x)
+        # Pt.y.title = "# pure compound"
 
         # weight matrix
-        w = NDDataset.zeros((n_pc, X.shape[-1]))
-        w.set_coordset(y=Pt.y, x=X.x)
+        w = np.zeros((n_components, N))
 
         # Stdev spectrum
-        s = NDDataset.zeros((n_pc, X.shape[-1]))
-        s.name = "Standard deviation spectra"
-        s.set_coordset(y=Pt.y, x=X.x)
+        s = np.zeros((n_components, N))
 
         # maximum purity indexes and coordinates
-        maxPIndex = [0] * n_pc
-        maxPCoordinate = [0] * n_pc
+        maxPIndex = [0] * n_components
+        maxPCoordinate = [0] * n_components
 
         # Concentration matrix
-        C = NDDataset.zeros((X.shape[-2], n_pc))
-        C.name = "Relative Concentrations"
-        C.set_coordset(y=X.y, x=C.x)
-        C.x.title = "# pure compound"
+        C = np.zeros((M, n_components))
 
         # Pure component spectral profiles
-        St = NDDataset.zeros((n_pc, X.shape[-1]))
-        St.name = "Pure compound spectra"
-        St.set_coordset(y=Pt.y, x=X.x)
+        St = np.zeros((n_components, N))
 
         # Compute Statistics
         # ------------------
-        sigma = np.std(X.data, axis=0)
-        mu = np.mean(X.data, axis=0)
-        alpha = (noise / 100) * np.max(mu.data)
+        sigma = np.std(X, axis=0)
+        mu = np.mean(X, axis=0)
+        alpha = (noise / 100) * np.max(mu)
         lamda = np.sqrt(mu**2 + sigma**2)
         p = sigma / (mu + alpha)
 
         # scale dataset
-        Xscaled = X.data / np.sqrt(mu**2 + (sigma + alpha) ** 2)
+        Xscaled = X / np.sqrt(mu**2 + (sigma + alpha) ** 2)
 
         # COO dispersion matrix
-        COO = (1 / X.shape[-2]) * np.dot(Xscaled.T, Xscaled)
+        COO = (1 / M) * np.dot(Xscaled.T, Xscaled)
 
         # Determine the purest variables
         j = 0
         finished = False
         while not finished:
             # compute first purest variable and weights
             if j == 0:
                 w[j, :] = lamda**2 / (mu**2 + (sigma + alpha) ** 2)
                 s[j, :] = sigma * w[j, :]
                 Pt[j, :] = p * w[j, :]
 
                 # get index and coordinate of pure variable
-                maxPIndex[j] = np.argmax(Pt[j, :].data)
-                maxPCoordinate[j] = get_x_data(X)[maxPIndex[j]]
+                maxPIndex[j] = np.argmax(Pt[j, :])
+                maxPCoordinate[j] = xdata[maxPIndex[j]]
 
                 # compute figures of merit
-                rsquare0, stdev_res0 = figures_of_merit(X, maxPIndex, C, St, j)
+                rsquare0, stdev_res0 = self._figures_of_merit(X, maxPIndex, C, St, j)
 
                 # add summary to log
-                llog = str_iter_summary(
+                llog = self._str_iter_summary(
                     j, maxPIndex[j], maxPCoordinate[j], rsquare0, stdev_res0, ""
                 )
-                logs += llog + "\n"
+                info_(llog)
 
                 if interactive:
                     print(llog)
 
-                if interactive:
                     # should plot purity and stdev, does not work for the moment
                     # TODO: fix the code below
                     # fig1, (ax1, ax2) = plt.subplots(2,1)
                     # Pt[j, :].plot(ax=ax1)
                     # ax1.set_title('Purity spectrum #{}'.format(j+1))
                     # ax1.axvline(maxPCoordinate[j], color='r')
                     # s[j, :].plot(ax=ax2)
@@ -236,36 +306,37 @@
                     while ans.lower() != "a":
                         new = input(
                             "   |--> enter the new index (int) or variable value (float): "
                         )
                         try:
                             new = int(new)
                             maxPIndex[j] = new
-                            maxPCoordinate[j] = get_x_data(X)[maxPIndex[j]]
+                            maxPCoordinate[j] = xdata[maxPIndex[j]]
                         except ValueError:
                             try:
                                 new = float(new)
-                                maxPIndex[j] = np.argmin(abs(get_x_data(X) - new))
-                                maxPCoordinate[j] = get_x_data(X)[maxPIndex[j]]
+                                maxPIndex[j] = np.argmin(abs(xdata - new))
+                                maxPCoordinate[j] = xdata[maxPIndex[j]]
                             except ValueError:
                                 print(
                                     "Incorrect answer. Please enter a valid index or value"
                                 )
 
-                        rsquare0, stdev_res0 = figures_of_merit(X, maxPIndex, C, St, j)
+                        rsquare0, stdev_res0 = self._figures_of_merit(
+                            X, maxPIndex, C, St, j
+                        )
 
-                        llog = str_iter_summary(
+                        llog = self._str_iter_summary(
                             j, maxPIndex[j], maxPCoordinate[j], rsquare0, stdev_res0, ""
                         )
-                        logs += "   |--> changed pure variable #1"
-                        logs += llog + "\n"
+                        info_("   |--> changed pure variable #1")
                         info_(llog)
 
                         ans = input("   |--> (a) Accept, (c) Change: ")
-                    # ans was [a]ccept
+                    # and was [a]ccept
                     j += 1
                 if not interactive:
                     j += 1
 
                 prev_stdev_res = stdev_res0
 
             else:
@@ -277,34 +348,30 @@
                         for col in range(j + 1):
                             Mji[line, col] = COO[idx[line], idx[col]]
                     w[j, i] = np.linalg.det(Mji)
                 Pt[j:] = p * w[j, :]
                 s[j, :] = sigma * w[j, :]
 
                 # get index and coordinate of jth pure variable
-                maxPIndex[j] = np.argmax(Pt[j, :].data)
-                maxPCoordinate[j] = get_x_data(X)[maxPIndex[j]]
+                maxPIndex[j] = np.argmax(Pt[j, :])
+                maxPCoordinate[j] = xdata[maxPIndex[j]]
 
                 # compute figures of merit
-                rsquarej, stdev_resj = figures_of_merit(X, maxPIndex, C, St, j)
+                rsquarej, stdev_resj = self._figures_of_merit(X, maxPIndex, C, St, j)
                 diff = 100 * (stdev_resj - prev_stdev_res) / prev_stdev_res
                 prev_stdev_res = stdev_resj
 
                 # add summary to log
-                llog = str_iter_summary(
+                llog = self._str_iter_summary(
                     j, maxPIndex[j], maxPCoordinate[j], rsquarej, stdev_resj, diff
                 )
-                logs += llog + "\n"
+                info_(llog)
 
                 if interactive:
-                    info_(llog)
-
-                if (
-                    interactive
-                ):  # TODO: I suggest to use jupyter widgets for the interactivity!
+                    # TODO: I suggest to use jupyter widgets for the interactivity!
                     # should plot purity and stdev, does not work for the moment
                     # TODO: fix the code below
                     # ax1.clear()
                     # ax1.set_title('Purity spectrum #{}'.format(j+1))
                     # Pt[j, :].plot(ax=ax1)
                     # for coord in maxPCoordinate[:-1]:
                     #     ax1.axvline(coord, color='g')
@@ -316,203 +383,183 @@
                     #     ax2.axvline(coord, color='g')
                     # ax2.axvline(maxPCoordinate[j], color='r')
                     # plt.show()
 
                     ans = ""
                     while ans.lower() not in ["a", "c", "r", "f"]:
                         ans = input(
-                            "   |--> (a) Accept and continue, (c) Change, (r) Reject, (f) Accept and finish: "
+                            "   |--> (a) Accept and continue, (c) Change, (r) Reject, "
+                            "(f) Accept and finish: "
                         )
 
                     while ans.lower() == "c":
                         new = input(
                             "   |--> enter the new index (int) or variable value (float): "
                         )
                         try:
                             new = int(new)
                             maxPIndex[j] = new
-                            maxPCoordinate[j] = get_x_data(X)[maxPIndex[j]]
+                            maxPCoordinate[j] = xdata[maxPIndex[j]]
                         except ValueError:
                             try:
                                 new = float(new)
-                                maxPIndex[j] = np.argmin(abs(get_x_data(X) - new))
-                                maxPCoordinate[j] = get_x_data(X)[maxPIndex[j]]
+                                maxPIndex[j] = np.argmin(abs(xdata - new))
+                                maxPCoordinate[j] = xdata[maxPIndex[j]]
                             except ValueError:
                                 print(
                                     "   |--> Incorrect answer. Please enter a valid index or value"
                                 )
 
-                        rsquarej, stdev_resj = figures_of_merit(X, maxPIndex, C, St, j)
+                        rsquarej, stdev_resj = self._figures_of_merit(
+                            X, maxPIndex, C, St, j
+                        )
                         diff = 100 * (stdev_resj - prev_stdev_res) / prev_stdev_res
                         prev_stdev_res + stdev_resj
 
-                        logs += f"   |--> changed pure variable #{j + 1}\n"
-                        llog = str_iter_summary(
+                        info_(f"   |--> changed pure variable #{j + 1}")
+                        llog = self._str_iter_summary(
                             j,
                             maxPIndex[j],
                             maxPCoordinate[j],
                             rsquarej,
                             stdev_resj,
                             "diff",
                         )
-                        logs += llog + "\n"
                         info_(llog)
 
                         info_(
                             f"purest variable #{j + 1} set at index = {maxPIndex[j]} ; x = {maxPCoordinate[j]}"
                         )
                         ans = input(
                             "   |--> (a) Accept and continue, (c) Change, (r) Reject, (f) Accept and stop: "
                         )
 
                     if ans.lower() == "r":
                         maxPCoordinate[j] = 0
                         maxPIndex[j] = 0
-                        logs += f"   |--> rejected pure variable #{j + 1}\n"
+                        info_(f"   |--> rejected pure variable #{j + 1}\n")
                         j = j - 1
 
                     elif ans.lower() == "a":
                         j = j + 1
 
                     elif ans.lower() == "f":
                         finished = True
                         j = j + 1
-                        llog = f"\n**** Interrupted by user at compound # {j} \n**** End of SIMPL(I)SMA analysis."
-                        logs += llog + "\n"
+                        info_("**** Interrupted by user at compound # {j}")
+                        info_("**** End of SIMPL(I)SMA analysis.")
                         Pt = Pt[0:j, :]
                         St = St[0:j, :]
                         s = s[0:j, :]
                         C = C[:, 0:j]
+
                 # not interactive
                 else:
                     j = j + 1
                     if (1 - rsquarej) < tol / 100:
-                        llog = (
-                            f"\n**** Unexplained variance lower than 'tol' ({tol}%) \n"
-                            "**** End of SIMPL(I)SMA analysis."
-                        )
-                        logs += llog + "\n"
+                        info_(f"**** Unexplained variance lower than 'tol' ({tol} %)")
+                        info_("**** End of SIMPL(I)SMA analysis.")
                         Pt = Pt[0:j, :]
                         St = St[0:j, :]
                         s = s[0:j, :]
                         C = C[:, 0:j]
-
-                        info_(llog)
                         finished = True
-            if j == n_pc:
+
+            if j == n_components:
                 if not interactive:
-                    llog = (
-                        f"\n**** Reached maximum number of pure compounds 'n_pc' ({n_pc}) \n"
-                        "**** End of SIMPL(I)SMA analysis."
+                    info_(
+                        f"**** Reached maximum number of pure compounds 'n_components' "
+                        f"({n_components})"
                     )
-                    logs += llog + "\n"
-                    info_(llog)
+                    info_("**** End of SIMPL(I)SMA analysis.")
                     finished = True
 
-        Pt.description = "Purity spectra from SIMPLISMA:\n" + logs
-        C.description = "Concentration/contribution matrix from SIMPLISMA:\n" + logs
-        St.description = "Pure compound spectra matrix from SIMPLISMA:\n" + logs
-        s.description = "Standard deviation spectra matrix from SIMPLISMA:\n" + logs
-
-        self._logs = logs
-        self._X = X
-        self._Pt = Pt
-        self._C = C
-        self._St = St
-        self._s = s
+        # found components
+        self._n_components = Pt.shape[0]
 
-    @property
-    def X(self):
+        # results
+        _outfit = (C, St, Pt, s)
+        return _outfit
+
+    def _transform(self, X=None):
+        # X is ignored for SIMPLISMA
+        return self._outfit[0]
+
+    def _inverse_transform(self, X_transform=None):
+        # X_transform is ignored for MCRALS
+        return np.dot(self._transform(), self._components)
+
+    def _get_components(self):
+        return self._components
+
+    # ----------------------------------------------------------------------------------
+    # Public methods and properties
+    # ----------------------------------------------------------------------------------
+    _docstring.keep_params("analysis_fit.parameters", "X")
+
+    @_docstring.dedent
+    def fit(self, X):
         """
-        The original dataset.
+        Fit the SIMPLISMA model on X.
+
+        Parameters
+        ----------
+        %(analysis_fit.parameters.X)s
+
+        Returns
+        -------
+        %(analysis_fit.returns)s
+
+        See Also
+        --------
+        %(analysis_fit.see_also)s
         """
-        return self._X
+        return super().fit(X, Y=None)
 
     @property
-    def St(self):
+    def C(self):
         """
-        Spectra of pure compounds.
+        Intensities ('concentrations') of pure compounds in spectra.
         """
-        return self._St
+        C = self.transform()
+        C.name = "Relative Concentrations"
+        C.x.title = "# pure compound"
+        C.description = "Concentration/contribution matrix from SIMPLISMA:"  # + logs
+        return C
 
     @property
-    def C(self):
+    def St(self):
         """
-        Intensities ('concentrations') of pure compounds in spectra.
+        Spectra of pure compounds.
         """
-        return self._C
+        St = self.components
+        St.name = "Pure compound spectra"
+        St.description = "Pure compound spectra matrix from SIMPLISMA:"  # + logs
+        return St
 
     @property
     def Pt(self):
         """
         Purity spectra.
         """
-        return self._Pt
+        Pt = self.St.copy()  # get a container
+        Pt.data = self._outfit[2]
+        Pt.name = "Purity spectra"
+        Pt.y.title = "# pure compound"
+        Pt.description = "Purity spectra from SIMPLISMA:"  # + logs
+        return Pt
 
     @property
     def s(self):
         """
         Standard deviation spectra.
         """
-        return self._s
-
-    @property
-    def logs(self):
-        """
-        Logs output.
-        """
-        return self._logs
-
-    def reconstruct(self):
-        """
-        Transform data back to the original space.
-
-        The following matrix operation is performed: :math:`X'_{hat} = C'.S'^t`
-
-        Returns
-        -------
-        X_hat
-            The reconstructed dataset based on the SIMPLISMA Analysis.
-        """
-
-        # reconstruct from concentration and spectra profiles
-
-        X_hat = dot(self.C, self.St)
-        X_hat.description = "Dataset reconstructed by SIMPLISMA\n" + self.logs
-        X_hat.title = "X_hat: " + self.X.title
-        return X_hat
-
-    def plotmerit(self, **kwargs):
-        """
-        Plots the input dataset, reconstructed dataset and residuals.
-
-        Parameters
-        ----------
-        **kwargs
-            Optional keyword parameters (see Other Parameters).
-
-        Other Parameters
-        ----------------
-
-        Returns
-        -------
-        ax
-            subplot.
-        """
-
-        colX, colXhat, colRes = kwargs.get("colors", ["blue", "green", "red"])
-
-        X_hat = self.reconstruct()
-
-        res = self.X - X_hat
-
-        ax = self.X.plot(label="$X$")
-        ax.plot(X_hat.data.T, color=colXhat, label=r"$\hat{X}")
-        ax.plot(res.data.T, color=colRes, label="Residual")
-        ax.set_title("SIMPLISMA plot: " + self.X.name)
-
-        return ax
+        s = self.St.copy()  # get a container
+        s.data = self._outfit[3]
+        s.name = "Standard deviation spectra"
+        s.description = "Standard deviation spectra matrix from SIMPLISMA:"  # + logs
+        return s
 
 
-# ============================================================================
+# ======================================================================================
 if __name__ == "__main__":
     pass
```

### Comparing `spectrochempy-0.5.5/spectrochempy/analysis/svd.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/read_csv.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,300 +1,291 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
-"""
-This module implements the Singular Value Decomposition (SVD) class.
-"""
+__all__ = ["read_csv"]
+__dataset_methods__ = __all__
 
-__all__ = ["SVD"]
-
-__dataset_methods__ = []
+# --------------------------------------------------------------------------------------
+# standard and other imports
+# --------------------------------------------------------------------------------------
+import io
+import locale
+import warnings
+from datetime import datetime
 
 import numpy as np
-from traitlets import HasTraits
 
+from spectrochempy.core import preferences as prefs
 from spectrochempy.core.dataset.coord import Coord
-from spectrochempy.core.dataset.nddataset import NDDataset
-from spectrochempy.utils.constants import MASKED
-from spectrochempy.utils.traits import NDDatasetType
+from spectrochempy.core.readers.importer import Importer, _importer_method
 
+try:
+    locale.setlocale(locale.LC_ALL, "en_US")  # to avoid problems with date format
+except Exception:  # pragma: no cover
+    try:
+        locale.setlocale(
+            locale.LC_ALL, "en_US.utf8"
+        )  # to avoid problems with date format
+    except Exception:
+        warnings.warn("Could not set locale: en_US or en_US.utf8")
 
-def _svd_flip(U, VT, u_based_decision=True):
-    """
-    Sign correction to ensure deterministic output from SVD.
-    Adjusts the columns of u and the rows of v such that the loadings in the
-    columns in u that are largest in absolute value are always positive.
 
-    Parameters
-    ----------
-    u_based_decision : boolean, (default=True)
-        If True, use the columns of u as the basis for sign flipping.
-        Otherwise, use the rows of v.
-
-    Notes
-    -----
-    Copied and modified from scikit-learn.utils.extmath (BSD 3 Licence)
+# ======================================================================================
+# Public functions
+# ======================================================================================
+def read_csv(*paths, **kwargs):
     """
+    Open a \*.csv file or a list of \*.csv files.
 
-    if u_based_decision:
-        # columns of U, rows of VT
-        max_abs_cols = np.argmax(np.abs(U), axis=0)
-        signs = np.sign(U[max_abs_cols, range(U.shape[1])])
-        U *= signs
-        VT *= signs[:, np.newaxis]
-    else:
-        # rows of V, columns of U
-        max_abs_rows = np.argmax(np.abs(VT), axis=1)
-        signs = np.sign(VT[range(VT.shape[0]), max_abs_rows])
-        U *= signs
-        VT *= signs[:, np.newaxis]
+    This is limited to 1D array - csv file must have two columns [index, data]
+    without header.
 
-    return U, VT
+    Parameters
+    ----------
+    *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
+        The data source(s) can be specified by the name or a list of name for the file(s) to be loaded:
 
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
-# --------------------------------------------------------------------------------------
-class SVD(HasTraits):
-    """
-    Performs a Singular Value Decomposition of a dataset.
+        If the list of filenames are enclosed into brackets:
 
-    The SVD is commonly written as :math:`X = U \\Sigma V^{T}`.
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
-    This class has the attributes : U, s = diag(S) and VT=V :math:`^T`.
+        The returned datasets are merged to form a single dataset,
+        except if `merge` is set to False. If a source is not provided (i.e. no `filename` , nor `content` ),
+        a dialog box will be opened to select files.
+    **kwargs
+        Optional keyword parameters (see Other Parameters).
 
-    If the dataset contains masked values, the corresponding ranges are
-    ignored in the calculation.
+    Returns
+    --------
+    read_csv
+        `NDDataset` or list of `NDDataset` .
 
-    Parameters
-    -----------
-    dataset : |NDDataset| object
-        The input dataset has shape (M, N). M is the number of
-        observations (for examples a series of IR spectra) while N
-        is the number of features (for example the wavenumbers measured
-        in each IR spectrum).
-    full_matrices : bool, optional, default=False.
-        If False , U and VT have the shapes (M,  k) and
-        (k, N), respectively, where k = min(M, N).
-        Otherwise the shapes will be (M, M) and (N, N),
-        respectively.
-    compute_uv : bool, optional, default: True.
-        Whether or not to compute U and VT in addition to s.
+    Other Parameters
+    ----------------
+    directory : str, optional
+        From where to read the specified `filename` . If not specified, read in the default `datadir` specified in
+        SpectroChemPy Preferences.
+    merge : bool, optional
+        Default value is False. If True, and several filenames have been provided as arguments,
+        then a single dataset with merged (stacked along the first
+        dimension) is returned (default=False).
+    sortbydate : bool, optional
+        Sort multiple spectra by acquisition date (default=True).
+    description: str, optional
+        A Custom description.
+    origin : {'omnic', 'tga'}, optional
+        in order to properly interpret CSV file it can be necessary to set the origin of the spectra.
+        Up to now only 'omnic' and 'tga' have been implemented.
+    csv_delimiter : str, optional
+        Set the column delimiter in CSV file.
+        By default it is the one set in SpectroChemPy `Preferences` .
+    content : bytes object, optional
+        Instead of passing a filename for further reading, a bytes content can be directly provided as bytes objects.
+        The most convenient way is to use a dictionary. This feature is particularly useful for a GUI Dash application
+        to handle drag and drop of files into a Browser.
+        For examples on how to use this feature, one can look in the `tests/tests_readers` directory.
+    listdir : bool, optional
+        If True and filename is None, all files present in the provided `directory` are returned (and merged if `merge`
+        is True. It is assumed that all the files correspond to current reading protocol (default=True).
+    recursive : bool, optional
+        Read also in subfolders. (default=False).
 
-    Examples
+    See Also
     --------
+    read_topspin : Read TopSpin Bruker NMR spectra.
+    read_omnic : Read Omnic spectra.
+    read_opus : Read OPUS spectra.
+    read_spg : Read Omnic \*.spg grouped spectra.
+    read_spa : Read Omnic \*.Spa single spectra.
+    read_srs : Read Omnic series.
+    read_zip : Read Zip files.
+    read_matlab : Read Matlab files.
+    read : Generic file reading.
 
-    >>> dataset = scp.read('irdata/nh4y-activation.spg')
-    >>> svd = scp.SVD(dataset)
-    >>> print(svd.ev.data)
-    [1.185e+04      634 ... 0.001089 0.000975]
-    >>> print(svd.ev_cum.data)
-    [   94.54     99.6 ...      100      100]
-    >>> print(svd.ev_ratio.data)
-    [   94.54    5.059 ... 8.687e-06 7.779e-06]
-    """
+    Examples
+    ---------
 
-    U = NDDatasetType(allow_none=True)
-    """|NDDataset| - Contains the left unitary matrix. Its shape depends on `full_matrices`"""
+    >>> scp.read_csv('agirdata/P350/TGA/tg.csv')
+    NDDataset: [float64] unitless (shape: (y:1, x:3247))
 
-    s = NDDatasetType()
-    """|NDDataset| - Vector of singular values"""
+    Additional information can be stored in the dataset if the origin is given
+    (known origin for now : tga or omnic)
+    # TODO: define some template to allow adding new origins
 
-    VT = NDDatasetType(allow_none=True)
-    """|NDDataset| - Contains a transpose matrix of the Loadings. Its shape depends on `full_matrices`"""
+    >>> scp.read_csv('agirdata/P350/TGA/tg.csv', origin='tga')
+    NDDataset: [float64] wt.% (shape: (y:1, x:3247))
 
-    def __init__(self, dataset, full_matrices=False, compute_uv=True):
-
-        super().__init__()
-
-        self._compute_uv = compute_uv
-
-        # check if we have the correct input
-        # ----------------------------------
-        X = dataset
-
-        if isinstance(X, NDDataset):
-            # As seen below, we cannot performs SVD on the masked array
-            # so let's take the ndarray only.
-            # Warning: we need to take the hidden values, to handle the
-            # case of dim 1 axis. Of course, svd will work only for real
-            # data, not complex or hypercomplex.
-            data = X._data
-            M, N = X._data.shape
-            units = X.units
+    Sometimes the delimiteur needs to be adjusted
 
-        else:
-            raise TypeError(
-                f"A dataset of type NDDataset is expected as a dataset of data, but an object of type"
-                f" {type(X).__name__} has been provided"
-            )
-
-        # Retains only valid rows and columns
-        # -----------------------------------
-        # unfortunately, the present SVD implementation in linalg library
-        # doesn't support numpy masked arrays as input. So we will have to
-        # remove the masked values ourselves
-
-        # the following however assumes that entire rows or columns are masked,
-        # not only some individual data (if this is what you wanted, this
-        # will fail)
-
-        if np.any(X._mask):
-            masked_columns = np.all(X._mask, axis=-2)
-            masked_rows = np.all(X._mask, axis=-1)
-        else:
-            masked_columns = np.zeros(X._data.shape[-1], dtype=bool)
-            masked_rows = np.zeros(X._data.shape[-2], dtype=bool)
+    >>> prefs = scp.preferences
+    >>> scp.read_csv('irdata/IR.CSV', directory=prefs.datadir, origin='omnic', csv_delimiter=',')
+    NDDataset: [float64] a.u. (shape: (y:1, x:3736))
+    """
+    kwargs["filetypes"] = ["CSV files (*.csv)"]
+    kwargs["protocol"] = ["csv"]
+    importer = Importer()
+    return importer(*paths, **kwargs)
 
-        data = data[:, ~masked_columns]
-        data = data[~masked_rows]
 
-        # Performs the SVD
-        # ----------------
-        if data.size == 0 and np.product(data.shape[-2:]) == 0:
-            raise np.linalg.LinAlgError(
-                "Arrays cannot be empty. You may " "want to check the masked data. "
-            )
-
-        res = np.linalg.svd(data, full_matrices, compute_uv)
-        if compute_uv:
-            U, s, VT = res
+# ======================================================================================
+# Private functions
+# ======================================================================================
+@_importer_method
+def _read_csv(*args, **kwargs):
+    # read csv file
+    dataset, filename = args
+    content = kwargs.get("content", None)
+    delimiter = kwargs.get("csv_delimiter", prefs.csv_delimiter)
+
+    def _open():
+        if content is not None:
+            f = io.StringIO(content.decode("utf-8"))
         else:
-            s = res
+            f = open(filename, "r")
+        return f
 
-        # Returns the diagonal sigma matrix as a NDDataset object
-        # -------------------------------------------------------
-        s = NDDataset(s)
-        s.title = "singular values of " + X.name
-        s.name = "sigma"
-        s.history = "Created by SVD \n"
-        s.description = (
-            "Vector of singular values obtained  by SVD " "decomposition of " + X.name
+    try:
+        fid = _open()
+        d = np.loadtxt(fid, unpack=True, delimiter=delimiter)
+        fid.close()
+    except ValueError:
+        # it might be that the delimiter is not correct (default is ','), but
+        # french excel export with the french locale for instance, use ";".
+        _delimiter = ";"
+        try:
+            fid = _open()
+            if fid:
+                fid.close()
+            fid = _open()
+            d = np.loadtxt(fid, unpack=True, delimiter=_delimiter)
+            fid.close()
+
+        except Exception:  # pragma: no cover
+            # in french, very often the decimal '.' is replaced by a
+            # comma:  Let's try to correct this
+            if fid:
+                fid.close()
+            if not isinstance(fid, io.StringIO):
+                with open(fid, "r") as fid_:
+                    txt = fid_.read()
+            else:
+                txt = fid.read()
+            txt = txt.replace(",", ".")
+            fil = io.StringIO(txt)
+            try:
+                d = np.loadtxt(fil, unpack=True, delimiter=delimiter)
+            except Exception:
+                raise IOError(
+                    "{} is not a .csv file or its structure cannot be recognized"
+                )
+
+    # First column is the x coordinates
+    coordx = Coord(d[0])
+
+    # create a second coordinate for dimension y of size 1
+    coordy = Coord([0])
+
+    # and data is the second column -  we make it a vector
+    data = d[1].reshape((1, coordx.size))
+
+    # update the dataset
+    dataset.data = data
+    dataset.set_coordset(y=coordy, x=coordx)
+
+    # set the additional attributes
+    name = filename.stem
+    dataset.filename = filename
+    dataset.name = kwargs.get("name", name)
+    dataset.title = kwargs.get("title", None)
+    dataset.units = kwargs.get("units", None)
+    dataset.description = kwargs.get("description", '"name" ' + "read from .csv file")
+    dataset.history = "Read from .csv file"
+
+    # here we can check some particular format
+    origin = kwargs.get("origin", "")
+    if "omnic" in origin:
+        # this will be treated as csv export from omnic (IR data)
+        dataset = _add_omnic_info(dataset, **kwargs)
+    elif "tga" in origin:
+        # this will be treated as csv export from tga analysis
+        dataset = _add_tga_info(dataset, **kwargs)
+    elif origin:
+        raise NotImplementedError(
+            f"Sorry, but reading a csv file with '{origin}' origin is not implemented. "
+            "Please, remove or set the keyword 'origin'\n "
+            "(Up to now implemented csv files are: `omnic` , `tga` )"
         )
-        self.s = s
 
-        if compute_uv:
-            # Put back masked columns in  VT
-            # ------------------------------
-            # Note that it is very important to use here the ma version of zeros
-            # array constructor
-            KV = VT.shape[0]
-            if np.any(masked_columns):
-                Vtemp = np.ma.zeros((KV, N))  # note np.ma, not np.
-                Vtemp[:, ~masked_columns] = VT
-                Vtemp[:, masked_columns] = MASKED
-                VT = Vtemp
-
-            # Put back masked rows in U
-            # -------------------------
-            KU = U.shape[1]
-            if np.any(masked_rows):
-                Utemp = np.ma.zeros((M, KU))
-                Utemp[~masked_rows] = U
-                Utemp[masked_rows] = MASKED
-                U = Utemp
-
-            # Sign correction to ensure deterministic output from SVD.
-            # This doesn't work will full_matrices=True.
-            if not full_matrices:
-                U, VT = _svd_flip(U, VT)
-
-            # Returns U as a NDDataset object
-            # --------------------------------
-            U = NDDataset(U)
-            U.name = "U"
-            U.title = "left singular vectors of " + X.name
-            U.set_coordset(
-                x=Coord(labels=[f"#{i + 1}" for i in range(KU)], title="Components"),
-                y=X.y,
-            )
-            U.description = "left singular vectors of " + X.name
-            U.history = "Created by SVD \n"
-
-            # Returns the loadings (VT) as a NDDataset object
-            # ------------------------------------------------
-            VT = NDDataset(VT)
-            VT.name = "V.T"
-            VT.title = "loadings (V.t) of " + X.name
-            VT.set_coordset(
-                x=X.x,
-                y=Coord(labels=[f"#{i + 1}" for i in range(KV)], title="Components"),
-            )
-            VT.description = (
-                "Loadings obtained by singular value decomposition of " + X.name
-            )
-            VT.history = str(VT.modified) + ": Created by SVD \n"
-            # loadings keep the units of the original data
-            VT.units = units
+    # reset modification date to cretion date
+    dataset._modified = dataset._created
 
-            self.U = U
-            self.VT = VT
-        else:
-            self.U = None
-            self.VT = None
+    return dataset
 
-    # ----------------------------------------------------------------------------------
-    # special methods
-    # ----------------------------------------------------------------------------------
-    def __repr__(self):
-        if self._compute_uv:
-            return f"<svd: U{self.U.shape}, s({self.s.size}), VT{self.VT.shape}>"
-        return f"<svd: s({self.s.size}), U, VT:not computed>"
-
-    # ----------------------------------------------------------------------------------
-    #  Properties
-    # ----------------------------------------------------------------------------------
-    @property
-    def sv(self):
-        """
-        Singular values (|NDDataset|).
-        """
-        size = self.s.size
-        sv = self.s.copy()
-        sv.name = "sv"
-        sv.title = "singular values"
-        sv.set_coordset(
-            Coord(None, labels=[f"#{(i + 1)}" for i in range(size)], title="Components")
-        )
-        return sv
 
-    @property
-    def ev(self):
-        """
-        Explained variance (|NDDataset|).
-        """
-        size = self.s.size
-        ev = self.s**2 / (size - 1)
-        ev.name = "ev"
-        ev.title = "explained variance"
-        ev.set_coordset(
-            Coord(None, labels=[f"#{(i + 1)}" for i in range(size)], title="Components")
-        )
-        return ev
+def _add_omnic_info(dataset, **kwargs):
+    # get the time and name
+    name = desc = dataset.name
+
+    # modify the dataset metadata
+    dataset.units = "absorbance"
+    dataset.title = "absorbance"
+    dataset.name = name
+    dataset.description = "Dataset from .csv file: {}\n".format(desc)
+    dataset.history = "Read from omnic exported csv file."
+    dataset.origin = "omnic"
+
+    # x axis
+    dataset.x.units = "cm^-1"
+
+    # y axis ?
+    if "_" in name:
+        name, dat = name.split("_")
+        # if needed convert weekday name to English
+        dat = dat.replace("Lun", "Mon")
+        dat = dat[:3].replace("Mar", "Tue") + dat[3:]
+        dat = dat.replace("Mer", "Wed")
+        dat = dat.replace("Jeu", "Thu")
+        dat = dat.replace("Ven", "Fri")
+        dat = dat.replace("Sam", "Sat")
+        dat = dat.replace("Dim", "Sun")
+        # convert month name to English
+        dat = dat.replace("Aout", "Aug")
+
+        # get the dates
+        acqdate = datetime.strptime(dat, "%a %b %d %H-%M-%S %Y")
+
+        # Transform back to timestamp for storage in the Coord object
+        # use datetime.fromtimestamp(d, timezone.utc))
+        # to transform back to datetime obkct
+        timestamp = acqdate.timestamp()
+
+        dataset.y = Coord(np.array([timestamp]), name="y")
+        dataset.set_coordtitles(y="acquisition timestamp (GMT)", x="wavenumbers")
+        dataset.y.labels = np.array([[acqdate], [name]])
+        dataset.y.units = "s"
+
+    # reset modification date to cretion date
+    dataset._modified = dataset._created
+
+    return dataset
+
+
+def _add_tga_info(dataset, **kwargs):
+    # for TGA, some information are needed.
+    # we add them here
+    dataset.x.units = "hour"
+    dataset.units = "weight_percent"
+    dataset.x.title = "time-on-stream"
+    dataset.title = "mass change"
+    dataset.origin = "tga"
 
-    @property
-    def ev_cum(self):
-        """
-        Cumulative Explained Variance (|NDDataset|).
-        """
-        ev_cum = np.cumsum(self.ev_ratio)
-        ev_cum.name = "ev_cum"
-        ev_cum.title = "cumulative explained variance"
-        ev_cum.units = "percent"
-        return ev_cum
-
-    @property
-    def ev_ratio(self):
-        """
-        Explained Variance per singular values |NDDataset|).
-        """
-        ratio = self.ev * 100.0 / np.sum(self.ev)
-        ratio.name = "ev_ratio"
-        ratio.title = "explained variance"
-        ratio.units = "percent"
-        return ratio
+    return dataset
 
 
-# ======================================================================================
+# --------------------------------------------------------------------------------------
 if __name__ == "__main__":
     pass
```

### Comparing `spectrochempy-0.5.5/spectrochempy/api.py` & `spectrochempy-0.6.1/spectrochempy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 # import the core api
 from spectrochempy import core
 from spectrochempy.core import *  # noqa: F403, F401, E402
 
 ALL += core.__all__
 
 if not IN_IPYTHON:
-    # needed in Windows terminal - but must not be inited in Jupyter notebook
+    # needed in terminal - but must not in Jupyter notebook
     from colorama import init as initcolor
 
     initcolor()
 
 RUNNING_IN_COLAB = "google.colab" in str(get_ipython())
 
 if IN_IPYTHON and KERNEL and not NO_DISPLAY:  # pragma: no cover
```

### Comparing `spectrochempy-0.5.5/spectrochempy/application.py` & `spectrochempy-0.6.1/spectrochempy/application/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 from jinja2 import Template
 from pkg_resources import DistributionNotFound, get_distribution, parse_version
 from setuptools_scm import get_version
 from traitlets.config.application import Application
 from traitlets.config.configurable import Config
 from traitlets.config.manager import BaseJSONConfigManager
 
+from spectrochempy.application.general_preferences import GeneralPreferences
 from spectrochempy.utils.file import pathclean
-from spectrochempy.utils.traits import MetaConfigurable
 from spectrochempy.utils.version import Version
 
 # ======================================================================================
 # Setup
 # ======================================================================================
 
 # --------------------------------------------------------------------------------------
@@ -130,43 +130,43 @@
     publish_display_data(data={"text/html": html})
 
 
 # --------------------------------------------------------------------------------------
 # Version
 # --------------------------------------------------------------------------------------
 try:
-    __release__ = get_distribution("spectrochempy").version.split("+")[0]
+    release = get_distribution("spectrochempy").version.split("+")[0]
     "Release version string of this package"
 except DistributionNotFound:  # pragma: no cover
     # package is not installed
-    __release__ = "--not set--"
+    release = "--not set--"
 
 try:
-    __version__ = get_version(root="..", relative_to=__file__)
+    version = get_version(root="..", relative_to=__file__)
     "Version string of this package"
 except LookupError:  # pragma: no cover
-    __version__ = __release__
+    version = release
 
 
 def _get_copyright():
     current_year = np.datetime64("now", "Y")
     right = f"2014-{current_year}"
     right += " - A.Travert & C.Fernandez @ LCS"
     return right
 
 
-__copyright__ = _get_copyright()
+copyright = _get_copyright()
 "Copyright string of this package"
 
 
 def _get_release_date():
     return subprocess.getoutput("git log -1 --tags --date=short --format='%ad'")
 
 
-__release_date__ = _get_release_date()
+release_date = _get_release_date()
 "Last release date of this package"
 
 
 def _get_pypi_version():
     """
     Get the last released pypi version
     """
@@ -195,38 +195,40 @@
         releases[last_version][0]["upload_time_iso_8601"].split("T")[0]
     )
     return Version(last_version), release_date
 
 
 def _check_for_updates(*args):
 
-    old = Version(__version__)
+    old = Version(version)
     res = _get_pypi_version()
     if res is not None:
-        version, release_date = res
+        _version, _release_date = res
     else:
         # probably a ConnectionError
         return
 
     new_release = None
 
-    if version > old:  # pragma: no cover  # TODO: change back the comparison sign
-        new_version = version.public
-        if not version.is_devrelease:
+    if _version > old:  # pragma: no cover  # TODO: change back the comparison sign
+        new_version = _version.public
+        if not _version.is_devrelease:
             new_release = new_version
 
     fil = Path.home() / ".scpy_update"
     if new_release and environ.get("DOC_BUILDING") is None:  # pragma: no cover
         if not fil.exists():  # This new version is checked for the first time
             # write the information: date of writing, status, message
             fil.write_text(
                 f"{date.isoformat(date.today())}%%NOT_YET_DISPLAYED%%"
                 f"SpectroChemPy v.{new_release} is available.\n"
                 f"Please consider updating, using pip or conda, for bug fixes and new "
-                f"features! "
+                f"features! \n"
+                f"WARNING: Version 0.6 has made some important changes "
+                f"that may require modification of existing scripts."
             )
     else:  # pragma: no cover
         if fil.exists():
             fil.unlink()
 
 
 def _display_needs_update_message():
@@ -261,29 +263,29 @@
 
 CHECK_UPDATE = threading.Thread(target=_check_for_updates, args=(1,))
 CHECK_UPDATE.start()
 
 # --------------------------------------------------------------------------------------
 # Other info
 # --------------------------------------------------------------------------------------
-__url__ = "https://www.spectrochempy.fr"
+url = "https://www.spectrochempy.fr"
 "URL for the documentation of this package"
 
-__author__ = "C. Fernandez & A. Travert"
+authors = "C. Fernandez & A. Travert"
 "First authors(s) of this package"
 
-__contributor__ = "A. Ait Blal, W. Guérin, M. Mailänder"
+contributors = "A. Ait Blal, W. Guérin, M. Mailänder"
 "contributor(s) to this package"
 
-__license__ = "CeCILL-B license"
+license = "CeCILL-B license"
 "License of this package"
 
-__cite__ = (
+cite = (
     f"Arnaud Travert & Christian Fernandez (2021) SpectroChemPy (version"
-    f" {'.'.join(__version__.split('.')[0:2])}). "
+    f" {'.'.join(version.split('.')[0:2])}). "
     f"Zenodo. https://doi.org/10.5281/zenodo.3823841"
 )
 "How to cite this package"
 
 
 # Directories
 
@@ -301,18 +303,18 @@
 
 
 def _get_config_dir():
     """
     Determines the SpectroChemPy configuration directory name and
     creates the directory if it doesn't exist.
 
-    This directory is typically ``$HOME/.spectrochempy/config``,
+    This directory is typically `$HOME/.spectrochempy/config` ,
     but if the
     SCP_CONFIG_HOME environment variable is set and the
-    ``$SCP_CONFIG_HOME`` directory exists, it will be that
+    `$SCP_CONFIG_HOME` directory exists, it will be that
     directory.
 
     If neither exists, the former will be created.
 
     Returns
     -------
     config_dir : str
@@ -512,15 +514,15 @@
 
     def listing(self):
         """
         Create a str representing a listing of the testdata folder.
 
         Returns
         -------
-        listing : str
+        `str`
             Display of the datadir content
         """
         strg = f"{self.path.name}\n"  # os.path.basename(self.path) + "\n"
 
         def _listdir(strg, initial, nst):
             nst += 1
             for fil in pathclean(initial).glob(
@@ -551,208 +553,58 @@
 
     def _repr_html_(self):  # pragma: no cover
         # _repr_html is needed to output in notebooks
         return self.listing().replace("\n", "<br/>").replace(" ", "&nbsp;")
 
 
 # ======================================================================================
-# General Preferences
-# ======================================================================================
-class GeneralPreferences(MetaConfigurable):
-    """
-    Preferences that apply to the |scpy| application in general.
-
-    They should be accessible from the main API.
-    """
-
-    name = tr.Unicode("GeneralPreferences")
-    description = tr.Unicode("General options for the SpectroChemPy application")
-    updated = tr.Bool(False)
-
-    # ----------------------------------------------------------------------------------
-    # Configuration entries
-    # ----------------------------------------------------------------------------------
-    # NON GUI
-    show_info_on_loading = tr.Bool(True, help="Display info on loading").tag(
-        config=True
-    )
-    use_qt = tr.Bool(
-        False,
-        help="Use QT for dialog instead of TK which is the default. "
-        "If True the PyQt libraries must be installed",
-    ).tag(config=True)
-
-    # GUI
-    # databases_directory = tr.Union(
-    #     (tr.Instance(Path), tr.Unicode()),
-    #     help="Directory where to look for database files such as csv",
-    # ).tag(config=True, gui=True, kind="folder")
-
-    datadir = tr.Union(
-        (tr.Instance(Path), tr.Unicode()),
-        help="Directory where to look for data by default",
-    ).tag(config=True, gui=True, kind="folder")
-
-    workspace = tr.Union(
-        (tr.Instance(Path), tr.Unicode()), help="Workspace directory by default"
-    ).tag(config=True, gui=True, kind="folder")
-
-    autoload_project = tr.Bool(
-        True, help="Automatic loading of the last project at startup"
-    ).tag(config=True, gui=True)
-
-    autosave_project = tr.Bool(
-        True, help="Automatic saving of the current project"
-    ).tag(config=True, gui=True)
-
-    project_directory = tr.Union(
-        (tr.Instance(Path), tr.Unicode()),
-        help="Directory where projects are stored by default",
-    ).tag(config=True, kind="folder")
-
-    last_project = tr.Union(
-        (tr.Instance(Path, allow_none=True), tr.Unicode()), help="Last used project"
-    ).tag(config=True, gui=True, kind="file")
-
-    show_close_dialog = tr.Bool(
-        True,
-        help="Display the close project dialog project changing or on application exit",
-    ).tag(config=True, gui=True)
-
-    csv_delimiter = tr.Enum(
-        [",", ";", r"\t", " "], default_value=",", help="CSV data delimiter"
-    ).tag(config=True, gui=True)
-
-    check_update_frequency = tr.Enum(
-        ["day", "week", "month"],
-        default_value="day",
-        help="Frequency of checking for update",
-    )
-
-    @tr.default("project_directory")
-    def _get_default_project_directory(self):
-        # Determines the SpectroChemPy project directory name and creates the directory
-        # if it doesn't exist.
-        # This directory is typically ``$HOME/spectrochempy/projects``, but if the
-        # SCP_PROJECTS_HOME environment
-        # variable is set and the `$SCP_PROJECTS_HOME` directory exists, it will be
-        # that directory.
-        # If neither exists, the former will be created.
-
-        # first look for SCP_PROJECTS_HOME
-        pscp = environ.get("SCP_PROJECTS_HOME")
-        if pscp is not None and Path(pscp).exists():
-            return Path(pscp)
-
-        pscp = Path.home() / ".spectrochempy" / "projects"
-
-        pscp.mkdir(exist_ok=True)
-
-        if pscp.is_file():
-            raise IOError("Intended Projects directory is actually a file.")
-
-        return pscp
-
-    @tr.default("workspace")
-    def _get_workspace_default(self):
-        # the spectra path in package data
-        return Path.home()
-
-    # @tr.default("databases_directory")
-    # def _get_databases_directory_default(self):
-    #     # the spectra path in package data
-    #     return pathclean(get_pkg_path("databases", "scp_data"))
-
-    @tr.default("datadir")
-    def _get_default_datadir(self):
-        return pathclean(self.parent.datadir.path)
-
-    @tr.observe("datadir")
-    def _datadir_changed(self, change):
-        self.parent.datadir.path = pathclean(change["new"])
-
-    @tr.validate("datadir")
-    def _data_validate(self, proposal):
-        # validation of the datadir attribute
-        datadir = proposal["value"]
-        if isinstance(datadir, str):
-            datadir = pathclean(datadir)
-        return datadir
-
-    @property
-    def log_level(self):
-        """
-        Logging level (int).
-        """
-        return self.parent.log_level
-
-    @log_level.setter
-    def log_level(self, value):
-        if isinstance(value, str):
-            value = getattr(logging, value, None)
-            if value is None:  # pragma: no cover
-                warnings.warn(
-                    "Log level not changed: invalid value given\n"
-                    "string values must be DEBUG, INFO, WARNING, "
-                    "or ERROR"
-                )
-        self.parent.log_level = value
-
-    # ----------------------------------------------------------------------------------
-    # Class Initialisation
-    # ----------------------------------------------------------------------------------
-    def __init__(self, **kwargs):
-        super().__init__(section="GeneralPreferences", **kwargs)
-
-
-# ======================================================================================
 # Application
 # ======================================================================================
 class SpectroChemPy(Application):
     """
     This class SpectroChemPy is the main class, containing most of the setup,
     configuration and more.
     """
 
     icon = tr.Unicode("scpy.png")
     "Icon for the application"
 
     running = tr.Bool(False)
-    "Running status of the |scpy| application"
+    "Running status of the  `SpectroChemPy` application"
 
     name = tr.Unicode("SpectroChemPy")
     "Running name of the application"
 
     description = tr.Unicode(
         "SpectroChemPy is a framework for processing, analysing and modelling "
         "Spectroscopic data for Chemistry with Python."
     )
-    "Short description of the |scpy| application"
+    "Short description of the  `SpectroChemPy` application"
 
     long_description = tr.Unicode()
-    "Long description of the |scpy| application"
+    "Long description of the  `SpectroChemPy` application"
 
     @tr.default("long_description")
     def _get_long_description(self):
         desc = f"""
 <p><strong>SpectroChemPy</strong> is a framework for processing, analysing and modelling
  <strong>Spectro</>scopic data for <strong>Chem</strong>istry with
  <strong>Py</strong>thon.
  It is a cross platform software, running on Linux, Windows or OS X.</p><br><br>
-<strong>Version:</strong> {__release__}<br>
-<strong>Authors:</strong> {__author__}<br>
-<strong>License:</strong> {__license__}<br>
+<strong>Version:</strong> {release}<br>
+<strong>Authors:</strong> {authors}<br>
+<strong>License:</strong> {license}<br>
 <div class='warning'> SpectroChemPy is still experimental and under active development.
 Its current design and
  functionalities are subject to major changes, reorganizations, bugs and crashes!!!.
  Please report any issues
 to the <a url='https://github.com/spectrochempy/spectrochempy/issues'>Issue Tracker<a>
 </div><br><br>
 When using <strong>SpectroChemPy</strong> for your own work,
-you are kindly requested to cite it this way: <pre>{__cite__}</pre></p>.
+you are kindly requested to cite it this way: <pre>{cite}</pre></p>.
 """
 
         return desc
 
     # ----------------------------------------------------------------------------------
     # Configuration parameters
     # ----------------------------------------------------------------------------------
@@ -927,15 +779,15 @@
         self.debug_("*" * 40)
         self.initialize()
 
     # ----------------------------------------------------------------------------------
     # Error/warning capture
     # ----------------------------------------------------------------------------------
     def _ipython_catch_exceptions(self, shell, etype, evalue, tb, tb_offset=None):
-        # output the full traceback only in DEBUG mode
+        # output the full traceback only in DEBUG mode or when under pytest
         if self.log_level == logging.DEBUG:
             shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
         else:
             self.log.error(f"{etype.__name__}: {evalue}")
 
     def _catch_exceptions(self, etype, evalue, tb=None):
         # output the full traceback only in DEBUG mode
@@ -981,15 +833,15 @@
                 if fil.suffix == ".py":
                     pyname = self.config_dir / fil
                     if self.reset_config:
                         # remove the py file to reset to defaults
                         pyname.unlink()
                     else:
                         configfiles.append(pyname)
-                elif fil.suffix == ".jso":
+                elif fil.suffix == ".json":
                     jsonname = self.config_dir / fil
                     if self.reset_config or fil == "PlotPreferences.json":
                         # remove the user json file to reset to defaults
                         jsonname.unlink()
                     else:
                         # check integrity of the file
                         with jsonname.open() as f:
@@ -1004,20 +856,20 @@
                 self.load_config_file(cfgname)
                 if cfgname not in self._loaded_config_files:
                     self._loaded_config_files.append(cfgname)
 
         self.datadir = (
             DataDir()
         )  # config=self.config)  -- passing args deprecated in traitlets 4.2
-        self.preferences = GeneralPreferences(config=self.config, parent=self)
-        from spectrochempy.plot_preferences import (
+        self.preferences = GeneralPreferences(parent=self)
+        from spectrochempy.application.plot_preferences import (
             PlotPreferences,  # slow : delayed import
         )
 
-        self.plot_preferences = PlotPreferences(config=self.config, parent=self)
+        self.plot_preferences = PlotPreferences(parent=self)
         self.classes.extend(
             [
                 GeneralPreferences,
                 PlotPreferences,
             ]
         )
 
@@ -1080,15 +932,16 @@
         # (such that those from jupyter which cause problems here)
 
         ipy = get_ipython() if InteractiveShell.initialized() else None
 
         if ipy is None:
             # remove argument not known by spectrochempy
             if (
-                "make.py" in sys.argv[0]
+                "sphinx-build" in sys.argv[0]
+                or "make.py" in sys.argv[0]
                 or "pytest" in sys.argv[0]
                 or "validate_docstrings" in sys.argv[0]
             ):  # building docs
                 options = []
                 for item in sys.argv[:]:
                     for k in list(self.flags.keys()):
                         if item.startswith("--" + k) or k in ["--help", "--help-all"]:
@@ -1097,15 +950,16 @@
                     for k in list(self.aliases.keys()):
                         if item.startswith("-" + k) or k in [
                             "h",
                         ]:
                             options.append(item)
                 self.parse_command_line(options)
             else:  # pragma: no cover
-                self.parse_command_line(sys.argv)
+                pass  # print("args", sys.argv)
+                # self.parse_command_line(sys.argv)
 
         # Get preferences from the config file and init everything
         # ---------------------------------------------------------------------
         self._init_all_preferences()
 
         # we catch warnings and error for a lighter display to the end-user.
         # except if we are in debugging mode
@@ -1143,26 +997,24 @@
         self.reset_config = False
 
     # ----------------------------------------------------------------------------------
     # start the application
     # ----------------------------------------------------------------------------------
     def start(self):
         """
-        Start the |scpy| API.
+        Start the  `SpectroChemPy` API.
 
         All configuration must have been done before calling this function.
         """
         if self.running:
             # API already started. Nothing done!
             return True
 
         if self.preferences.show_info_on_loading:
-            info_string = (
-                f"SpectroChemPy's API - v.{__version__}\n© Copyright {__copyright__}"
-            )
+            info_string = f"SpectroChemPy's API - v.{version}\n© Copyright {copyright}"
             ipy = get_ipython()
             if ipy is not None and "TerminalInteractiveShell" not in str(ipy):
                 _display_info_string(message=info_string.strip())
 
             else:
                 if "/bin/scpy" not in sys.argv[0]:  # deactivate for console scripts
                     print(info_string.strip())
@@ -1281,30 +1133,34 @@
         )
         self.log.handlers[1].setFormatter(formatter)
 
     # ----------------------------------------------------------------------------------
     # Private methods
     # ----------------------------------------------------------------------------------
     def _make_default_config_file(self):
-        """auto generate default config file."""
-
-        # first we will complete self.classes with a list of configurable in analysis
-        from spectrochempy.analysis.api import __configurables__
+        # auto generate default config file.
 
         # remove old configuration file spectrochempy_cfg.py
+        # --------------------------------------------------
         fname = self.config_dir / "spectrochempy_cfg.py"  # Old configuration file
-        if fname.exists():
-            fname.unlink()
+        fname2 = self.config_dir / "SpectroChemPy.cfg.py"
+        if fname.exists() or fname2.exists():
+            for file in list(self.config_dir.iterdir()):
+                file.unlink()
 
         # create a configuration file for each configurables
+        # --------------------------------------------------
+        from spectrochempy.analysis.api import __configurables__
+
+        # first we will complete self.classes with a list of configurable in analysis
         self.classes.extend(__configurables__)
         config_classes = list(self._classes_with_config_traits(self.classes))
         for cls in config_classes:
             name = cls.__name__
-            fname = self.config_dir / f"{name}.cfg.py"
+            fname = self.config_dir / f"{name}.py"
             if fname.exists() and not self.reset_config:
                 continue
             """generate default config file from Configurables"""
             lines = [f"# Configuration file for SpectroChemPy::{name}"]
             lines.append("")
             lines.append("c = get_config()  # noqa")
             lines.append("")
@@ -1312,15 +1168,15 @@
             sfil = "\n".join(lines)
             self.log.info(f"Generating default config file: {fname}")
             with open(fname, "w") as fil:
                 fil.write(sfil)
 
 
 # ======================================================================================
-# Start instance od Spectrochempy and expose public members in all
+# Start instance of Spectrochempy and expose public members in all
 # ======================================================================================
 app = SpectroChemPy()
 preferences = app.preferences
 error_ = app.error_
 warning_ = app.warning_
 info_ = app.info_
 debug_ = app.debug_
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/__init__.py` & `spectrochempy-0.6.1/spectrochempy/core/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
-Package defining the *core* methods of the |scpy| API.
+Package defining the *core* methods of the  `SpectroChemPy` API.
 
 Most the API methods such as plotting, processing, analysis, etc...
 
 isort:skip_file
 """
 # flake8: noqa
 
@@ -28,37 +28,38 @@
     def __enter__(self):
         self.time = perf_counter()
         return self
 
     def __exit__(self, type, value, traceback):
         self.time = perf_counter() - self.time
         self.readout = f"Elapsed Time for {self.msg}: {self.time:.6f} seconds\n"
-        # print(self.readout)
+        if "pytest" in sys.argv[0] or "py.test" in sys.argv[0]:
+            print(self.readout)
 
 
 # ======================================================================================
 # loading module libraries
 # here we also construct the __all__ list automatically
 # ======================================================================================
 
 with timeit("app"):
     from spectrochempy.application import app  # noqa: E402
 
     __all__ += ["app"]
 
 with timeit("application"):
     from spectrochempy.application import (
-        __version__ as version,
-        __release__ as release,
-        __copyright__ as copyright,
-        __license__ as license,
-        __release_date__ as release_date,
-        __author__ as authors,
-        __contributor__ as contributors,
-        __url__ as url,
+        version,
+        release,
+        copyright,
+        license,
+        release_date,
+        authors,
+        contributors,
+        url,
         DEBUG,
         WARNING,
         ERROR,
         CRITICAL,
         INFO,
         error_,
         warning_,
@@ -212,12 +213,13 @@
         "Quantity",
         "ur",
         "set_nmr_context",
         "DimensionalityError",
     ]
 
 # START THE app
-_started = app.start()
+with timeit("start app"):
+    _started = app.start()
 
 # ======================================================================================
 if __name__ == "__main__":
     pass
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/common/dialogs.py` & `spectrochempy-0.6.1/spectrochempy/core/common/dialogs.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/core/dataset/api.py` & `spectrochempy-0.6.1/spectrochempy/core/dataset/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/core/dataset/arraymixins/__init__.py` & `spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/core/dataset/arraymixins/ndio.py` & `spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/ndio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
-This module define the class |NDIO| in which input/output standard
-methods for a |NDDataset| are defined.
+This module define the class  `NDIO` in which input/output standard
+methods for a `NDDataset` are defined.
 """
 
 __all__ = ["load"]
 
 import io
 import json
 import pathlib
@@ -35,17 +35,17 @@
 # Utilities
 # --------------------------------------------------------------------------------------
 # ======================================================================================
 # Class NDIO to handle I/O of datasets
 # ======================================================================================
 class NDIO(HasTraits):
     """
-    Import/export interface from |NDDataset| .
+    Import/export interface from `NDDataset` .
 
-    This class is used as basic import/export interface of the |NDDataset| .
+    This class is used as basic import/export interface of the `NDDataset` .
     """
 
     _filename = Union((Instance(pathlib.Path), Unicode()), allow_none=True)
 
     @property
     def directory(self):
         """
@@ -107,16 +107,16 @@
     # ----------------------------------------------------------------------------------
     # Public methods
     # ----------------------------------------------------------------------------------
     def save(self, **kwargs):
         """
         Save the current object in SpectroChemPy format.
 
-        Default extension is *.scp for |NDDataset|'s and *.pscp for
-        |Project|'s.
+        Default extension is .scp for `NDDataset`\'s and .pscp for
+         `Project`'s.
 
         Parameters
         ----------
         **kwargs
             Optional keyword parameters (see Other Parameters).
 
         Other Parameters
@@ -128,26 +128,30 @@
         save_as : Save current object with a different name and/or directory.
         write : Export current object to different format.
 
         Examples
         ---------
 
         Read some data from an OMNIC file
+
         >>> nd = scp.read_omnic('wodger.spg')
         >>> assert nd.name == 'wodger'
 
         Write it in SpectroChemPy format (.scp)
         (return a `pathlib` object)
+
         >>> filename = nd.save()
 
         Check the existence of the scp fie
+
         >>> assert filename.is_file()
         >>> assert filename.name == 'wodger.scp'
 
         Remove this file
+
         >>> filename.unlink()
         """
 
         # By default we save the file in the self.directory and with the
         # name + suffix depending
         # on the current object type
         if self.directory is None:
@@ -167,15 +171,15 @@
         # in this case we do not display a dialog and overwrite the same file
 
         self.name = filename.stem
         return self.dump(filename, **kwargs)
 
     def save_as(self, filename="", **kwargs):
         """
-        Save the current |NDDataset| in SpectroChemPy format (*.scp).
+        Save the current `NDDataset` in SpectroChemPy format (\*.scp).
 
         Parameters
         ----------
         filename : str
             The filename of the file where to save the current dataset.
         **kwargs
             Optional keyword parameters (see Other Parameters).
@@ -189,32 +193,35 @@
         See Also
         ---------
         save : Save current dataset.
         write : Export current dataset to different format.
 
         Notes
         -----
-        Adapted from :class:`numpy.savez`.
+        Adapted from :class:`numpy.savez` .
 
         Examples
         --------
-
         Read some data from an OMNIC file
+
         >>> nd = scp.read_omnic('wodger.spg')
         >>> assert nd.name == 'wodger'
 
         Write it in SpectroChemPy format (.scp)
         (return a `pathlib` object)
+
         >>> filename = nd.save_as('new_wodger')
 
-        Check the existence of the scp fie
+        Check the existence of the scp file
+
         >>> assert filename.is_file()
         >>> assert filename.name == 'new_wodger.scp'
 
         Remove this file
+
         >>> filename.unlink()
         """
         if filename:
             # we have a filename
             # by default it use the saved directory
             filename = pathclean(filename)
             if self.directory and self.directory != filename.parent:
@@ -241,15 +248,15 @@
     @classmethod
     def load(cls, filename, **kwargs):
         """
         Open data from a '*.scp' (NDDataset) or '.pscp' (Project) file.
 
         Parameters
         ----------
-        filename :  `str`, `pathlib` or `file` objects
+        filename :  `str` , `pathlib` or `file` objects
             The name of the file to read (or a file objects.
         **kwargs
             Optional keyword parameters (see Other Parameters).
 
         Other Parameters
         ----------------
         content : str, optional
@@ -258,15 +265,15 @@
         See Also
         --------
         read : Import dataset from various orgines.
         save : Save the current dataset.
 
         Notes
         -----
-        Adapted from `numpy.load`.
+        Adapted from `numpy.load` .
 
         Examples
         --------
 
         >>> nd1 = scp.read('irdata/nh4y-activation.spg')
         >>> f = nd1.save()
         >>> f.name
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/dataset/arraymixins/ndmath.py` & `spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/ndmath.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,27 +350,27 @@
 
 def _logical_binary_ufuncs():
     return _extract_ufuncs(LOGICAL_BINARY_STR)
 
 
 class NDMath(object):
     """
-    This class provides the math and some other array manipulation functionalities to |NDArray| or |Coord| .
+    This class provides the math and some other array manipulation functionalities to  `NDArray` or  `Coord` .
 
     Below is a list of mathematical functions (numpy) implemented (or
     planned for implementation).
 
     **Ufuncs**
 
     These functions should work like for numpy-ndarray, except that they
     may be units-aware.
 
-    For instance, `ds`  being a |NDDataset| , just call the np functions like
+    For instance, `ds`  being a `NDDataset` , just call the np functions like
     this. Most of the time it returns a new NDDataset, while in some cases
-    noted below, one get a |ndarray| .
+    noted below, one get a `~numpy.ndarray` .
 
     >>> ds = scp.NDDataset([1., 2., 3.])
     >>> np.sin(ds)
     NDDataset: [float64] unitless (size: 3)
 
     In this particular case (*i.e.*, `np.sin` ufuncs) , the `ds` units must be
     `unitless` , `dimensionless` or angle-units : `radians` or `degrees` ,
@@ -552,28 +552,28 @@
     @_from_numpy_method
     def absolute(cls, dataset, dtype=None):
         """
         Calculate the absolute value of the given NDDataset element-wise.
 
         `abs` is a shorthand for this function. For complex input, a + ib, the absolute
         value is
-        :math:`\\sqrt{ a^2 + b^2}`.
+        :math:`\\sqrt{ a^2 + b^2}` .
 
         Parameters
         ----------
-        dataset : array_like
+        dataset : `NDDataset` or :term:`array-like`
             Input array or object that can be converted to an array.
         dtype : dtype
             The type of the output array. If dtype is not given, infer the data type
             from the other input arguments.
 
         Returns
         -------
-        absolute
-            An ndarray containing the absolute value of each element in dataset.
+        `~spectrochempy.core.dataset.nddataset.NDDataset`
+            The absolute value of each element in dataset.
         """
 
         if not cls.has_complex_dims:
             data = np.ma.fabs(
                 dataset, dtype=dtype
             )  # not a complex, return fabs should be faster
 
@@ -611,15 +611,15 @@
             Input array or object that can be converted to an array.
         dim : int, str, optional, default=(0,)
             Dimension names or indexes along which the method should be applied.
 
         Returns
         -------
         conjugated
-            Same object or a copy depending on the ``inplace`` flag.
+            Same object or a copy depending on the `inplace` flag.
 
         See Also
         --------
         conj, real, imag, RR, RI, IR, II, part, set_complex, is_complex
         """
 
         axis, dim = cls.get_axis(dim, allows_none=True)
@@ -646,15 +646,15 @@
     @_from_numpy_method
     def around(cls, dataset, decimals=0):
         """
         Evenly round to the given number of decimals.
 
         Parameters
         ----------
-        dataset : |NDDataset|
+        dataset : `NDDataset`
             Input dataset.
         decimals : int, optional
             Number of decimal places to round to (default: 0).  If
             decimals is negative, it specifies the number of positions to
             the left of the decimal point.
 
         Returns
@@ -699,24 +699,24 @@
 
         Parameters
         ----------
         dataset : array_like
             Input array or object that can be converted to an array.
         dim : None or int or str, optional
             Axis or axes along which a logical AND reduction is performed.
-            The default (``axis=None``) is to perform a logical AND over all
+            The default (`axis=None` ) is to perform a logical AND over all
             the dimensions of the input array. `axis` may be negative, in
             which case it counts from the last to the first axis.
         keepdims : bool, optional
             If this is set to True, the axes which are reduced are left
             in the result as dimensions with size one. With this option,
             the result will broadcast correctly against the input array.
             If the default value is passed, then `keepdims` will not be
             passed through to the `all` method of sub-classes of
-            `ndarray`, however any non-default value will be.  If the
+            `~numpy.ndarray` , however any non-default value will be.  If the
             sub-class' method does not implement `keepdims` any
             exceptions will be raised.
 
         Returns
         -------
         all
             A new boolean or array is returned unless `out` is specified,
@@ -755,15 +755,15 @@
             in the result as dimensions with size one. With this option,
             the result will broadcast correctly against the input array.
 
         Returns
         -------
         amax
             Maximum of the data. If `dim` is None, the result is a scalar value.
-            If `dim` is given, the result is an array of dimension ``ndim - 1``.
+            If `dim` is given, the result is an array of dimension `ndim - 1` .
 
         See Also
         --------
         amin : The minimum value of a dataset along a given dimension, propagating NaNs.
         minimum : Element-wise minimum of two datasets, propagating any NaNs.
         maximum : Element-wise maximum of two datasets, propagating any NaNs.
         fmax : Element-wise maximum of two datasets, ignoring any NaNs.
@@ -859,15 +859,15 @@
             in the result as dimensions with size one. With this option,
             the result will broadcast correctly against the input array.
 
         Returns
         -------
         amin
             Minimum of the data. If `dim` is None, the result is a scalar value.
-            If `dim` is given, the result is an array of dimension ``ndim - 1``.
+            If `dim` is given, the result is an array of dimension `ndim - 1` .
 
         See Also
         --------
         amax : The maximum value of a dataset along a given dimension, propagating NaNs.
         minimum : Element-wise minimum of two datasets, propagating any NaNs.
         maximum : Element-wise maximum of two datasets, propagating any NaNs.
         fmax : Element-wise maximum of two datasets, ignoring any NaNs.
@@ -940,39 +940,39 @@
 
     @_reduce_method
     @_from_numpy_method
     def any(cls, dataset, dim=None, keepdims=False):
         """
         Test whether any array element along a given axis evaluates to True.
 
-        Returns single boolean unless `dim` is not ``None``
+        Returns single boolean unless `dim` is not `None`
 
         Parameters
         ----------
         dataset : array_like
             Input array or object that can be converted to an array.
         dim : None or int or tuple of ints, optional
             Axis or axes along which a logical OR reduction is performed.
-            The default (``axis=None``) is to perform a logical OR over all
+            The default (`axis=None` ) is to perform a logical OR over all
             the dimensions of the input array. `axis` may be negative, in
             which case it counts from the last to the first axis.
         keepdims : bool, optional
             If this is set to True, the axes which are reduced are left
             in the result as dimensions with size one. With this option,
             the result will broadcast correctly against the input array.
             If the default value is passed, then `keepdims` will not be
             passed through to the `any` method of sub-classes of
-            `ndarray`, however any non-default value will be.  If the
+            `~numpy.ndarray` , however any non-default value will be.  If the
             sub-class' method does not implement `keepdims` any
             exceptions will be raised.
 
         Returns
         -------
         any
-            A new boolean or `ndarray` is returned.
+            A new boolean or `~numpy.ndarray` is returned.
 
         See Also
         --------
         all : Test whether all array elements along a given axis evaluate to True.
         """
 
         axis, dim = cls.get_axis(dim, allows_none=True)
@@ -1066,20 +1066,20 @@
             Array containing data to be averaged.
         dim : None or int or dimension name or tuple of int or dimensions, optional
             Dimension or dimensions along which to operate.  By default, flattened
             input is used.
             If this is a tuple, the minimum is selected over multiple dimensions,
             instead of a single dimension or all the dimensions as before.
         weights : array_like, optional
-            An array of weights associated with the values in `dataset`. Each value in
+            An array of weights associated with the values in `dataset` . Each value in
             `a` contributes to the average according to its associated weight.
             The weights array can either be 1-D (in which case its length must be
             the size of `dataset` along the given axis) or of the same shape as
-            `dataset`.
-            If `weights=None`, then all data in `dataset` are assumed to have a
+            `dataset` .
+            If `weights=None` , then all data in `dataset` are assumed to have a
             weight equal to one.  The 1-D calculation is::
 
                 avg = sum(a * weights) / sum(weights)
 
             The only constraint on `weights` is that `sum(weights)` must not be 0.
 
         Returns
@@ -1136,19 +1136,19 @@
 
     @_from_numpy_method
     def clip(cls, dataset, a_min=None, a_max=None, **kwargs):
         """
         Clip (limit) the values in a dataset.
 
         Given an interval, values outside the interval are clipped to
-        the interval edges.  For example, if an interval of ``[0, 1]``
+        the interval edges.  For example, if an interval of `[0, 1]`
         is specified, values smaller than 0 become 0, and values larger
         than 1 become 1.
 
-        No check is performed to ensure ``a_min < a_max``.
+        No check is performed to ensure `a_min < a_max` .
 
         Parameters
         ----------
         dataset : array_like
             Input array or object that can be converted to an array.
         a_min : scalar or array_like or None
             Minimum value. If None, clipping is not performed on lower
@@ -1159,17 +1159,17 @@
             interval edge. Not more than one of `a_min` and `a_max` may be
             None. If `a_min` or `a_max` are array_like, then the three
             arrays will be broadcasted to match their shapes.
 
         Returns
         -------
         clip
-            An array with the elements of `a`, but where values
-            < `a_min` are replaced with `a_min`, and those > `a_max`
-            with `a_max`.
+            An array with the elements of `a` , but where values
+            < `a_min` are replaced with `a_min` , and those > `a_max`
+            with `a_max` .
         """
         # if len(args) > 2 or len(args) == 0:
         #     raise ValueError('Clip requires at least one argument or at most two
         #     arguments')
         # amax = kwargs.pop('a_max', args[0] if len(args) == 1 else args[1])
         # amin = kwargs.pop('a_min', self.min() if len(args) == 1 else args[0])
         # amin, amax = np.minimum(amin, amax), max(amin, amax)
@@ -1310,15 +1310,15 @@
         return cls
 
     @_from_numpy_method
     def diag(cls, dataset, offset=0, **kwargs):
         """
         Extract a diagonal or construct a diagonal array.
 
-        See the more detailed documentation for ``numpy.diagonal`` if you use this
+        See the more detailed documentation for `numpy.diagonal` if you use this
         function to extract a diagonal and wish to write to the resulting array;
         whether it returns a copy or a view depends on what version of numpy you
         are using.
 
         Parameters
         ----------
         dataset : array_like
@@ -1376,15 +1376,15 @@
         Return the diagonal of a 2D array.
 
         As we reduce a 2D to a 1D we must specified which is the dimension for the
         coordinates to keep!.
 
         Parameters
         ----------
-        dataset : |NDDataset| or array-like
+        dataset : `NDDataset` or array-like
             Object from which to extract the diagonal.
         offset : int, optional
             Offset of the diagonal from the main diagonal.  Can be positive or
             negative.  Defaults to main diagonal (0).
         dim : str, optional
             Dimension to keep for coordinates. By default it is the last (-1, `x` or
             another name if the default
@@ -1432,15 +1432,15 @@
             cls.dims = [dim]
 
         return cls
 
     @_from_numpy_method
     def empty(cls, shape, dtype=None, **kwargs):
         """
-        Return a new |NDDataset| of given shape and type, without initializing entries.
+        Return a new `NDDataset` of given shape and type, without initializing entries.
 
         Parameters
         ----------
         shape : int or tuple of int
             Shape of the empty array.
         dtype : data-type, optional
             Desired output data-type.
@@ -1470,15 +1470,15 @@
         full_like : Fill an array with shape and type of input.
         zeros : Return a new array setting values to zero.
         ones : Return a new array setting values to 1.
         full : Fill a new array.
 
         Notes
         -----
-        `empty`, unlike `zeros`, does not set the array values to zero,
+        `empty` , unlike `zeros` , does not set the array values to zero,
         and may therefore be marginally faster.  On the other hand, it requires
         the user to manually set all the values in the array, and should be
         used with caution.
 
         Examples
         --------
 
@@ -1487,33 +1487,33 @@
         """
 
         return cls(np.empty(shape, dtype), dtype=dtype, **kwargs)
 
     @_from_numpy_method
     def empty_like(cls, dataset, dtype=None, **kwargs):
         """
-        Return a new uninitialized |NDDataset| .
+        Return a new uninitialized `NDDataset` .
 
-        The returned |NDDataset| have the same shape and type as a given array. Units,
+        The returned `NDDataset` have the same shape and type as a given array. Units,
         coordset, ... can be added in
         kwargs.
 
         Parameters
         ----------
-        dataset : |NDDataset| or array-like
+        dataset : `NDDataset` or array-like
             Object from which to copy the array structure.
         dtype : data-type, optional
             Overrides the data type of the result.
         **kwargs
             Optional keyword parameters (see Other Parameters).
 
         Returns
         -------
         emptylike
-            Array of `fill_value` with the same shape and type as `dataset`.
+            Array of `fill_value` with the same shape and type as `dataset` .
 
         Other Parameters
         ----------------
         units : str or ur instance
             Units of the returned object. If not provided, try to copy from the input
             object.
         coordset : list or Coordset object
@@ -1530,15 +1530,15 @@
         ones : Return a new array setting values to one.
         zeros : Return a new array setting values to zero.
         full : Fill a new array.
 
         Notes
         -----
         This function does *not* initialize the returned array; to do that use
-        for instance `zeros_like`, `ones_like` or `full_like` instead.  It may be
+        for instance `zeros_like` , `ones_like` or `full_like` instead.  It may be
         marginally faster than the functions that do set the array values.
         """
 
         cls._data = np.empty_like(dataset, dtype)
         cls._dtype = np.dtype(dtype)
 
         return cls
@@ -1549,15 +1549,15 @@
         Return a 2-D array with ones on the diagonal and zeros elsewhere.
 
         Parameters
         ----------
         N : int
             Number of rows in the output.
         M : int, optional
-            Number of columns in the output. If None, defaults to `N`.
+            Number of columns in the output. If None, defaults to `N` .
         k : int, optional
             Index of the diagonal: 0 (the default) refers to the main diagonal,
             a positive value refers to an upper diagonal, and a negative value
             to a lower diagonal.
         dtype : data-type, optional
             Data-type of the returned array.
         **kwargs
@@ -1592,44 +1592,44 @@
     @_from_numpy_method
     def fromfunction(
         cls, function, shape=None, dtype=float, units=None, coordset=None, **kwargs
     ):
         """
         Construct a nddataset by executing a function over each coordinate.
 
-        The resulting array therefore has a value ``fn(x, y, z)`` at coordinate
-        ``(x, y, z)`` .
+        The resulting array therefore has a value `fn(x, y, z)` at coordinate
+        `(x, y, z)` .
 
         Parameters
         ----------
         function : callable
             The function is called with N parameters, where N is the rank of
-            `shape` or from the provided `coordset`.
+            `shape` or from the provided `CoordSet` .
         shape : (N,) tuple of ints, optional
             Shape of the output array, which also determines the shape of
-            the coordinate arrays passed to `function`. It is optional only if
-            `coordset` is None.
+            the coordinate arrays passed to `function` . It is optional only if
+            `CoordSet` is None.
         dtype : data-type, optional
-            Data-type of the coordinate arrays passed to `function`.
+            Data-type of the coordinate arrays passed to `function` .
             By default, `dtype` is float.
         units : str, optional
             Dataset units.
             When None, units will be determined from the function results.
-        coordset : |Coordset| instance, optional
+        coordset : `CoordSet` instance, optional
             If provided, this determine the shape and coordinates of each dimension of
-            the returned |NDDataset| . If shape is also passed it will be ignored.
+            the returned `NDDataset` . If shape is also passed it will be ignored.
         **kwargs
             Other kwargs are passed to the final object constructor.
 
         Returns
         -------
         fromfunction
             The result of the call to `function` is passed back directly.
             Therefore the shape of `fromfunction` is completely determined by
-            `function`.
+            `function` .
 
         See Also
         --------
         fromiter : Make a dataset from an iterable.
 
         Examples
         --------
@@ -1676,35 +1676,33 @@
 
         Parameters
         ----------
         iterable : iterable object
             An iterable object providing data for the array.
         dtype : data-type
             The data-type of the returned array.
-        count : int, optional
+        count : `int`, optional
             The number of items to read from iterable. The default is -1, which means
             all data is read.
         **kwargs
             Other kwargs are passed to the final object constructor.
 
         Returns
         -------
         fromiter
             The output nddataset.
 
         See Also
         --------
-        fromfunction : Construct a nddataset by executing a function over each
-        coordinate.
+        fromfunction : Construct a nddataset by executing a function over each coordinate.
 
         Notes
         -----
             Specify count to improve performance. It allows fromiter to pre-allocate the
-             output array,
-            instead of resizing it on demand.
+             output array, instead of resizing it on demand.
 
         Examples
         --------
 
         >>> iterable = (x * x for x in range(5))
         >>> d = scp.fromiter(iterable, float, units='km')
         >>> d
@@ -1714,32 +1712,32 @@
         """
 
         return cls(np.fromiter(iterable, dtype=dtype, count=count), **kwargs)
 
     @_from_numpy_method
     def full(cls, shape, fill_value=0.0, dtype=None, **kwargs):
         """
-        Return a new |NDDataset| of given shape and type, filled with `fill_value`.
+        Return a new `NDDataset` of given shape and type, filled with `fill_value` .
 
         Parameters
         ----------
         shape : int or sequence of ints
-            Shape of the new array, e.g., ``(2, 3)`` or ``2``.
+            Shape of the new array, e.g., `(2, 3)` or `2` .
         fill_value : scalar
             Fill value.
         dtype : data-type, optional
-            The desired data-type for the array, e.g., `np.int8`.  Default is
+            The desired data-type for the array, e.g., `np.int8` .  Default is
             fill_value.dtype.
         **kwargs
             Optional keyword parameters (see Other Parameters).
 
         Returns
         -------
         full
-            Array of `fill_value`.
+            Array of `fill_value` .
 
         Other Parameters
         ----------------
         units : str or ur instance
             Units of the returned object. If not provided, try to copy from the input
             object.
         coordset : list or Coordset object
@@ -1766,35 +1764,35 @@
         """
 
         return cls(np.full(shape, fill_value, dtype), dtype=dtype, **kwargs)
 
     @_from_numpy_method
     def full_like(cls, dataset, fill_value=0.0, dtype=None, **kwargs):
         """
-        Return a |NDDataset| of fill_value.
+        Return a `NDDataset` of fill_value.
 
-        The returned |NDDataset| have the same shape and type as a given array. Units,
+        The returned `NDDataset` have the same shape and type as a given array. Units,
         coordset, ... can be added in
         kwargs
 
         Parameters
         ----------
-        dataset : |NDDataset| or array-like
+        dataset : `NDDataset` or array-like
             Object from which to copy the array structure.
         fill_value : scalar
             Fill value.
         dtype : data-type, optional
             Overrides the data type of the result.
         **kwargs
             Optional keyword parameters (see Other Parameters).
 
         Returns
         -------
         fulllike
-            Array of `fill_value` with the same shape and type as `dataset`.
+            Array of `fill_value` with the same shape and type as `dataset` .
 
         Other Parameters
         ----------------
         units : str or ur instance
             Units of the returned object. If not provided, try to copy from the input
             object.
         coordset : list or Coordset object
@@ -1839,26 +1837,26 @@
         return cls
 
     @_from_numpy_method
     def geomspace(cls, start, stop, num=50, endpoint=True, dtype=None, **kwargs):
         """
         Return numbers spaced evenly on a log scale (a geometric progression).
 
-        This is similar to `logspace`, but with endpoints specified directly.
+        This is similar to `logspace` , but with endpoints specified directly.
         Each output sample is a constant multiple of the previous.
 
         Parameters
         ----------
         start : number
             The starting value of the sequence.
         stop : number
             The final value of the sequence, unless `endpoint` is False.
-            In that case, ``num + 1`` values are spaced over the
+            In that case, `num + 1` values are spaced over the
             interval in log-space, of which all but the last (a sequence of
-            length `num`) are returned.
+            length `num` ) are returned.
         num : int, optional
             Number of samples to generate.  Default is 50.
         endpoint : bool, optional
             If true, `stop` is the last sample. Otherwise, it is not included.
             Default is True.
         dtype : dtype
             The type of the output array.  If `dtype` is not given, infer the data
@@ -1883,25 +1881,25 @@
         """
 
         return cls(np.geomspace(start, stop, num, endpoint, dtype), **kwargs)
 
     @_from_numpy_method
     def identity(cls, n, dtype=None, **kwargs):
         """
-        Return the identity |NDDataset| of a given shape.
+        Return the identity `NDDataset` of a given shape.
 
         The identity array is a square array with ones on
         the main diagonal.
 
         Parameters
         ----------
         n : int
             Number of rows (and columns) in `n` x `n` output.
         dtype : data-type, optional
-            Data-type of the output.  Defaults to ``float``.
+            Data-type of the output.  Defaults to `float` .
         **kwargs
             Other parameters to be passed to the object constructor (units, coordset,
             mask ...).
 
         Returns
         -------
         identity
@@ -1975,35 +1973,35 @@
     @_from_numpy_method
     def logspace(
         cls, start, stop, num=50, endpoint=True, base=10.0, dtype=None, **kwargs
     ):
         """
         Return numbers spaced evenly on a log scale.
 
-        In linear space, the sequence starts at ``base ** start``
-        (`base` to the power of `start`) and ends with ``base ** stop``
+        In linear space, the sequence starts at `base ** start`
+        (`base` to the power of `start` ) and ends with `base ** stop`
         (see `endpoint` below).
 
         Parameters
         ----------
         start : array_like
-            ``base ** start`` is the starting value of the sequence.
+            `base ** start` is the starting value of the sequence.
         stop : array_like
-            ``base ** stop`` is the final value of the sequence, unless `endpoint`
-            is False.  In that case, ``num + 1`` values are spaced over the
+            `base ** stop` is the final value of the sequence, unless `endpoint`
+            is False.  In that case, `num + 1` values are spaced over the
             interval in log-space, of which all but the last (a sequence of
-            length `num`) are returned.
+            length `num` ) are returned.
         num : int, optional
             Number of samples to generate.  Default is 50.
         endpoint : bool, optional
             If true, `stop` is the last sample. Otherwise, it is not included.
             Default is True.
         base : float, optional
             The base of the log space. The step size between the elements in
-            ``ln(samples) / ln(base)`` (or ``log_base(samples)``) is uniform.
+            `ln(samples) / ln(base)` (or `log_base(samples)` ) is uniform.
             Default is 10.0.
         dtype : dtype
             The type of the output array.  If `dtype` is not given, infer the data
             type from the other input arguments.
         **kwargs
             Keywords argument used when creating the returned object, such as units,
             name, title, ...
@@ -2094,29 +2092,29 @@
         cls.dims = dims
 
         return cls
 
     @_from_numpy_method
     def ones(cls, shape, dtype=None, **kwargs):
         """
-        Return a new |NDDataset| of given shape and type, filled with ones.
+        Return a new `NDDataset` of given shape and type, filled with ones.
 
         Parameters
         ----------
         shape : int or sequence of ints
-            Shape of the new array, e.g., ``(2, 3)`` or ``2``.
+            Shape of the new array, e.g., `(2, 3)` or `2` .
         dtype : data-type, optional
-            The desired data-type for the array, e.g., `numpy.int8`.  Default is
+            The desired data-type for the array, e.g., `numpy.int8` .  Default is
         **kwargs
             Optional keyword parameters (see Other Parameters).
 
         Returns
         -------
         ones
-            Array of `ones`.
+            Array of `ones` .
 
         Other Parameters
         ----------------
         units : str or ur instance
             Units of the returned object. If not provided, try to copy from the input
             object.
         coordset : list or Coordset object
@@ -2159,33 +2157,33 @@
         """
 
         return cls(np.ones(shape), dtype=dtype, **kwargs)
 
     @_from_numpy_method
     def ones_like(cls, dataset, dtype=None, **kwargs):
         """
-        Return |NDDataset| of ones.
+        Return `NDDataset` of ones.
 
-        The returned |NDDataset| have the same shape and type as a given array. Units,
+        The returned `NDDataset` have the same shape and type as a given array. Units,
         coordset, ... can be added in
         kwargs.
 
         Parameters
         ----------
-        dataset : |NDDataset| or array-like
+        dataset : `NDDataset` or array-like
             Object from which to copy the array structure.
         dtype : data-type, optional
             Overrides the data type of the result.
         **kwargs
             Optional keyword parameters (see Other Parameters).
 
         Returns
         -------
         oneslike
-            Array of `1` with the same shape and type as `dataset`.
+            Array of `1` with the same shape and type as `dataset` .
 
         Other Parameters
         ----------------
         units : str or ur instance
             Units of the returned object. If not provided, try to copy from the input
             object.
         coordset : list or Coordset object
@@ -2218,38 +2216,38 @@
         cls._data = np.ones_like(dataset, dtype)
         cls._dtype = np.dtype(dtype)
 
         return cls
 
     def pipe(self, func, *args, **kwargs):
         """
-        Apply func(self, *args, **kwargs).
+        Apply func(self, \*args, \*\*kwargs).
 
         Parameters
         ----------
         func : function
-            Function to apply to the |NDDataset| .
-            `*args`, and `**kwargs` are passed into `func`.
+            Function to apply to the `NDDataset` .
+            \*args` , and `\*\*kwargs` are passed into `func` .
             Alternatively a `(callable, data_keyword)` tuple where
             `data_keyword` is a string indicating the keyword of
             `callable` that expects the array object.
         *args
-            Positional arguments passed into `func`.
+            Positional arguments passed into `func` .
         **kwargs
-            Keyword arguments passed into `func`.
+            Keyword arguments passed into `func` .
 
         Returns
         -------
         pipe
-           The return type of `func`.
+           The return type of `func` .
 
         Notes
         -----
-        Use ``.pipe`` when chaining together functions that expect
-        a |NDDataset| .
+        Use `pipe` when chaining together functions that expect
+        a `NDDataset` .
         """
         if isinstance(func, tuple):
             func, target = func
             if target in kwargs:
                 error_(
                     Exception,
                     f"{target} is both the pipe target and a keyword argument. "
@@ -2263,15 +2261,15 @@
 
     @_reduce_method
     @_from_numpy_method
     def ptp(cls, dataset, dim=None, keepdims=False):
         """
         Range of values (maximum - minimum) along a dimension.
 
-        The name of the function comes from the acronym for 'peak to peak'.
+        The name of the function comes from the acronym for 'peak to peak' .
 
         Parameters
         ----------
         dim : None or int or dimension name, optional
             Dimension along which to find the peaks.
             If None, the operation is made on the first dimension.
         keepdims : bool, optional
@@ -2353,15 +2351,15 @@
              is used.
         dtype : dtype, optional
             Type to use in computing the standard deviation. For arrays of
             integer type the default is float64, for arrays of float types it is
             the same as the array type.
         ddof : int, optional
             Means Delta Degrees of Freedom.  The divisor used in calculations
-            is ``N - ddof``, where ``N`` represents the number of elements.
+            is `N - ddof` , where `N` represents the number of elements.
             By default `ddof` is zero.
         keepdims : bool, optional
             If this is set to True, the dimensions which are reduced are left
             in the result as dimensions with size one. With this option,
             the result will broadcast correctly against the input array.
 
         Returns
@@ -2373,24 +2371,24 @@
         --------
         var : Variance values along axis.
         mean : Compute the arithmetic mean along the specified axis.
 
         Notes
         -----
         The standard deviation is the square root of the average of the squared
-        deviations from the mean, i.e., ``std = sqrt(mean(abs(x - x.mean())**2))``.
+        deviations from the mean, i.e., `std = sqrt(mean(abs(x - x.mean())**2))` .
 
         The average squared deviation is normally calculated as
-        ``x.sum() / N``, where ``N = len(x)``.  If, however, `ddof` is specified,
-        the divisor ``N - ddof`` is used instead. In standard statistical
-        practice, ``ddof=1`` provides an unbiased estimator of the variance
-        of the infinite population. ``ddof=0`` provides a maximum likelihood
+        `x.sum() / N` , where `N = len(x)` .  If, however, `ddof` is specified,
+        the divisor `N - ddof` is used instead. In standard statistical
+        practice, `ddof=1` provides an unbiased estimator of the variance
+        of the infinite population. `ddof=0` provides a maximum likelihood
         estimate of the variance for normally distributed variables. The
         standard deviation computed in this function is the square root of
-        the estimated variance, so even with ``ddof=1``, it will not be an
+        the estimated variance, so even with `ddof=1` , it will not be an
         unbiased estimate of the standard deviation per se.
 
         Note that, for complex numbers, `std` takes the absolute
         value before squaring, so that the result is always real and nonnegative.
         For floating-point input, the *std* is computed using the same
         precision the input has. Depending on the input data, this can cause
         the results to be inaccurate, especially for float32 (see example below).
@@ -2508,15 +2506,15 @@
             input is used.
         dtype : dtype, optional
             Type to use in computing the standard deviation. For arrays of
             integer type the default is float64, for arrays of float types it is
             the same as the array type.
         ddof : int, optional
             Means Delta Degrees of Freedom.  The divisor used in calculations
-            is ``N - ddof``, where ``N`` represents the number of elements.
+            is `N - ddof` , where `N` represents the number of elements.
             By default `ddof` is zero.
         keepdims : bool, optional
             If this is set to True, the dimensions which are reduced are left
             in the result as dimensions with size one. With this option,
             the result will broadcast correctly against the input array.
 
         Returns
@@ -2528,30 +2526,30 @@
         --------
         std : Standard deviation values along axis.
         mean : Compute the arithmetic mean along the specified axis.
 
         Notes
         -----
         The variance is the average of the squared deviations from the mean,
-        i.e.,  ``var = mean(abs(x - x.mean())**2)``.
+        i.e.,  `var = mean(abs(x - x.mean())**2)` .
 
-        The mean is normally calculated as ``x.sum() / N``, where ``N = len(x)``.
-        If, however, `ddof` is specified, the divisor ``N - ddof`` is used
-        instead.  In standard statistical practice, ``ddof=1`` provides an
+        The mean is normally calculated as `x.sum() / N` , where `N = len(x)` .
+        If, however, `ddof` is specified, the divisor `N - ddof` is used
+        instead.  In standard statistical practice, `ddof=1` provides an
         unbiased estimator of the variance of a hypothetical infinite population.
-        ``ddof=0`` provides a maximum likelihood estimate of the variance for
+        `ddof=0` provides a maximum likelihood estimate of the variance for
         normally distributed variables.
 
         Note that for complex numbers, the absolute value is taken before
         squaring, so that the result is always real and nonnegative.
 
         For floating-point input, the variance is computed using the same
         precision the input has.  Depending on the input data, this can cause
         the results to be inaccurate, especially for `float32` (see example
-        below).  Specifying a higher-accuracy accumulator using the ``dtype``
+        below).  Specifying a higher-accuracy accumulator using the `dtype`
         keyword can alleviate this issue.
 
         Examples
         --------
 
         >>> nd = scp.read('irdata/nh4y-activation.spg')
         >>> nd
@@ -2579,23 +2577,23 @@
         cls.dims = dims
 
         return cls
 
     @_from_numpy_method
     def zeros(cls, shape, dtype=None, **kwargs):
         """
-        Return a new |NDDataset| of given shape and type, filled with zeros.
+        Return a new `NDDataset` of given shape and type, filled with zeros.
 
         Parameters
         ----------
         shape : int or sequence of ints
-            Shape of the new array, e.g., ``(2, 3)`` or ``2``.
+            Shape of the new array, e.g., `(2, 3)` or `2` .
         dtype : data-type, optional
-            The desired data-type for the array, e.g., `numpy.int8`.  Default is
-            `numpy.float64`.
+            The desired data-type for the array, e.g., `numpy.int8` .  Default is
+            `numpy.float64` .
         **kwargs
             Optional keyword parameters (see Other Parameters).
 
         Returns
         -------
         zeros
             Array of zeros.
@@ -2636,33 +2634,33 @@
         """
 
         return cls(np.zeros(shape), dtype=dtype, **kwargs)
 
     @_from_numpy_method
     def zeros_like(cls, dataset, dtype=None, **kwargs):
         """
-        Return a |NDDataset| of zeros.
+        Return a `NDDataset` of zeros.
 
-        The returned |NDDataset| have the same shape and type as a given array. Units,
+        The returned `NDDataset` have the same shape and type as a given array. Units,
         coordset, ... can be added in kwargs.
 
         Parameters
         ----------
-        dataset : |NDDataset| or array-like
+        dataset : `NDDataset` or array-like
             Object from which to copy the array structure.
         dtype : data-type, optional
             Overrides the data type of the result.
         **kwargs
             Optional keyword parameters (see Other Parameters).
 
 
         Returns
         -------
         zeorslike
-            Array of `fill_value` with the same shape and type as `dataset`.
+            Array of `fill_value` with the same shape and type as `dataset` .
 
         Other Parameters
         ----------------
         units : str or ur instance
             Units of the returned object. If not provided, try to copy from the input
             object.
         coordset : list or Coordset object
@@ -3279,34 +3277,34 @@
         return self.ufunc(*args, **kwargs)
 
     @property
     def __doc__(self):
         doc = f"""
             {_unary_ufuncs()[self.name].split('->')[-1].strip()}
 
-            Wrapper of the numpy.ufunc function ``np.{self.name}(dataset)``.
+            Wrapper of the numpy.ufunc function `np.{self.name}(dataset)` .
 
             Parameters
             ----------
             dataset : array-like
                 Object to pass to the numpy function.
 
             Returns
             -------
             out
-                |NDDataset|
+                `NDDataset`
 
             See Also
             --------
             numpy.{self.name} : Corresponding numpy Ufunc.
 
             Notes
             -----
             Numpy Ufuncs referenced in our documentation can be directly applied to
-            |NDDataset| or |Coord| type
+            `NDDataset` or  `Coord` type
             of SpectrochemPy objects.
             Most of these Ufuncs, however, instead of returning a numpy array, will
             return the same type of object.
 
             Examples
             --------
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/dataset/arraymixins/ndplot.py` & `spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/ndplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
-This module defines the |NDPlot| class in which generic |NDDataset| plot methods are defined.
+This module defines the `NDPlot` class in which generic `NDDataset` plot methods are defined.
 """
 
 __all__ = ["plot"]
 
 import re
 import textwrap
 
@@ -28,15 +28,15 @@
 from spectrochempy.utils.file import pathclean
 from spectrochempy.utils.optional import import_optional_dependency
 from spectrochempy.utils.plots import _Axes, _Axes3D, get_figure
 
 go = import_optional_dependency("plotly.graph_objects", errors="ignore")
 HAS_PLOTLY = go is not None
 
-# from spectrochempy.utils import deprecated
+# from spectrochempy.utils.decorators import deprecated
 
 
 # ======================================================================================
 # Management of the preferences for datasets
 # ======================================================================================
 class PreferencesSet(Meta):
     """
@@ -337,17 +337,17 @@
 
 
 # ======================================================================================
 # Class NDPlot to handle plotting of datasets
 # ======================================================================================
 class NDPlot(HasTraits):
     """
-    Plotting interface for |NDDataset| .
+    Plotting interface for `NDDataset` .
 
-    This class is used as basic plotting interface of the |NDDataset| .
+    This class is used as basic plotting interface of the `NDDataset` .
     """
 
     # Instance of the current matplotlib axis defined for a NDArray object.
     # The _Axes class subclass matplotlib axes in order to allow methods with
     # Quantities as arguments
     _ax = Instance(_Axes, allow_none=True)
 
@@ -367,24 +367,24 @@
     # ----------------------------------------------------------------------------------
     # Generic plotter and plot related methods or properties
     # ----------------------------------------------------------------------------------
     def plot(self, method=None, **kwargs):
         """
         Generic plot function.
 
-        This apply to a |NDDataset| but actually delegate the work to a plotter defined by the keyword parameter
-        ``method``.
+        This apply to a `NDDataset` but actually delegate the work to a plotter defined
+        by the keyword parameter `method` .
 
         Parameters
         ----------
         method : str, optional, default: "generic"
             Specify with plot method to use.
         **kwargs
             Any optional parameters to pass to the plot method.
-            See plot_1D, plot_2D and plot_3D for a  liste of possible arguments.
+            See plot_1D, plot_2D and plot_3D for a list of possible arguments.
 
         Returns
         -------
         axe
             The axe instance on which the plot has bee performed.
 
         See Also
@@ -720,15 +720,15 @@
         # Reset all preferences
         prefs = PreferencesSet()
         return prefs
 
     @property
     def preferences(self):
         """
-        |Meta| instance object - Additional metadata.
+        `Meta` instance object - Additional metadata.
         """
         return self._preferences
 
     @preferences.setter
     def preferences(self, preferences):
         # property.setter for preferences
         if preferences is not None:
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/dataset/arraymixins/npy.py` & `spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/npy.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         the computation. Default is False.  Propagating the mask means that
         if a masked value appears in a row or column, the whole row or
         column is considered masked.
     out : masked_array, optional
         Output argument. This must have the exact kind that would be returned
         if it was not used. In particular, it must have the right type, must be
         C-contiguous, and its dtype must be the dtype that would be returned
-        for `dot(a,b)`. This is a performance feature. Therefore, if these
+        for `dot(a,b)` . This is a performance feature. Therefore, if these
         conditions are not met, an exception is raised, instead of attempting
         to be flexible.
 
     See Also
     --------
     numpy.dot : Equivalent function for ndarrays.
     numpy.ma.dot : Equivalent function for masked ndarrays.
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/dataset/baseobjects/meta.py` & `spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 This module mainly contains the definition of a Meta class object.
 
-Such object is particularly used in `SpectrochemPy` by the |NDDataset| object
+Such object is particularly used in `SpectrochemPy` by the `NDDataset` object
 to store metadata. Like a regular dictionary, the
 elements can be accessed by key, but also by attributes, *e.g.*
-``a = meta['key']`` give the same results as ``a = meta.key``.
+`a = meta['key']` give the same results as `a = meta.key` .
 """
 
 # from traitlets import HasTraits, Dict, Bool, default
 
 # import sys
 import copy
 import json
 
 import numpy as np
 
-__all__ = ["Meta"]
+__all__ = []
 
 
 # ======================================================================================
 # Class Meta
 # ======================================================================================
-class Meta(object):  # HasTraits):
+class Meta(object):
     """
     A dictionary to store metadata.
 
     The metadata are accessible by item or by attributes, and
     the dictionary can be made read-only if necessary.
 
     Parameters
     ----------
-    **data : keywords
+    \**data : keywords
         The dictionary can be already inited with some keywords.
 
     Examples
     --------
 
     First we initialise a metadata object
 
@@ -192,29 +192,32 @@
             A regular dictionary.
         """
 
         return self._data
 
     def get(self, key, default=None):
         """
+        Dictionary get method.
+
         Parameters
         ----------
-        key
+        key : str
+            key to retrieve.
         """
         return self._data.get(key, default)
 
     def update(self, d):
         """
         Feed a metadata dictionary with the content of an another
         dictionary.
 
         Parameters
         ----------
         d : dict-like object
-            Any dict-like object can be used, such as `dict`, traits `Dict` or
+            Any dict-like object can be used, such as `dict` , traits `Dict` or
             another `Meta` object.
         """
 
         if isinstance(d, Meta) or hasattr(d, "_data"):
             d = d.to_dict()
         if d:
             self._data.update(d)
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/dataset/baseobjects/ndarray.py` & `spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/ndarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
-This module implements the |NDArray| base class.
+This module implements the  `NDArray` base class.
 """
 
 __all__ = []
 
 import copy as cpy
 import itertools
 import pathlib
@@ -70,82 +70,103 @@
 
 
 # ======================================================================================
 # The basic NDArray class
 # ======================================================================================
 class NDArray(HasTraits):
     """
-    The basic |NDArray| object.
+    The basic  `NDArray` object.
 
-    The |NDArray| class is an array (numpy |ndarray|-like) container, usually not intended to be used directly,
+    The  `NDArray` class is an array (numpy :term:`array-like`) container, usually not
+    intended to be used directly,
     as its basic functionalities may be quite limited, but to be subclassed.
 
-    Indeed, both the classes |NDDataset| and |Coord| which respectively implement a full dataset (with
-    coordinates) and the coordinates in a given dimension, are derived from |NDArray| in |scpy| .
+    Indeed, both the classes `NDDataset` and  `Coord` which respectively implement a
+    full dataset (with
+    coordinates) and the coordinates in a given dimension, are derived from  `NDArray`
+    in  `SpectroChemPy` .
 
-    The key distinction from raw numpy |ndarray| is the presence of optional properties such as dimension names,
+    The key distinction from raw numpy `~numpy.ndarray` is the presence of optional
+    properties such as dimension names,
     labels, masks, units and/or extensible metadata dictionary.
 
     Parameters
     ----------
     data : array of floats
-        Data array contained in the object. The data can be a list, a tuple, a |ndarray| , a ndarray-like,
-        a |NDArray| or any subclass of |NDArray| . Any size or shape of data is accepted. If not given, an empty
-        |NDArray| will be inited.
-        At the initialisation the provided data will be eventually cast to a numpy-ndarray.
-        If a subclass of |NDArray| is passed which already contains some mask, labels, or units, these elements
+        Data array contained in the object. The data can be a list, a tuple, a
+        `~numpy.ndarray` , a ndarray-like,
+        a  `NDArray` or any subclass of  `NDArray` . Any size or shape of data is
+        accepted. If not given, an empty `NDArray` will be inited.
+        At the initialisation the provided data will be eventually cast to a
+        `numpy.ndarray`\ .
+        If a subclass of  `NDArray` is passed which already contains some mask, labels,
+        or units, these elements
         will
-        be used to accordingly set those of the created object. If possible, the provided data will not be copied
-        for `data` input, but will be passed by reference, so you should make a copy of the `data` before passing
+        be used to accordingly set those of the created object. If possible, the
+        provided data will not be copied
+        for `data` input, but will be passed by reference, so you should make a copy of
+        the `data` before passing
         them if that's the desired behavior or set the `copy` argument to True.
     **kwargs
         Optional keywords parameters. See Other Parameters.
 
     Other Parameters
     ----------------
     dtype : str or dtype, optional, default=np.float64
-        If specified, the data will be cast to this dtype, else the data will be cast to float64.
+        If specified, the data will be cast to this dtype, else the data will be cast
+        to float64.
     dims : list of chars, optional
-        If specified the list must have a length equal to the number of data dimensions (ndim).
-        If not specified, dimension names are automatically attributed in the order given by
-        `DEFAULT_DIM_NAME`.
+        If specified the list must have a length equal to the number of data dimensions
+        (ndim).
+        If not specified, dimension names are automatically attributed in the order
+        given by
+        `DEFAULT_DIM_NAME` .
     name : str, optional
-        A user-friendly name for this object. If not given, the automatic `id` given at the object creation will be
+        A user-friendly name for this object. If not given, the automatic `id` given at
+        the object creation will be
         used as a name.
     labels : array of objects, optional
-        Labels for the `data`. Note that the labels can be used only for 1D-datasets.
-        The labels array may have an additional dimension, meaning several series of labels for the same data.
-        The given array can be a list, a tuple, a |ndarray| , a ndarray-like, a |NDArray| or any subclass of
-        |NDArray| .
-    mask : array of bool or `NOMASK`, optional
-        Mask for the data. The mask array must have the same shape as the data. The given array can be a list,
-        a tuple, or a |ndarray| . Each values in the array must be `False` where the data are *valid* and True when
-        they are not (like in numpy masked arrays). If `data` is already a :class:`~numpy.ma.MaskedArray`, or any
-        array object (such as a |NDArray| or subclass of it), providing a `mask` here will cause the mask from the
+        Labels for the `data` . Note that the labels can be used only for 1D-datasets.
+        The labels array may have an additional dimension, meaning several series of
+        labels for the same data.
+        The given array can be a list, a tuple, a `~numpy.ndarray` , a ndarray-like, a
+        `NDArray` or any subclass of `NDArray` .
+    mask : array of bool or `NOMASK` , optional
+        Mask for the data. The mask array must have the same shape as the data. The
+        given array can be a list,
+        a tuple, or a `~numpy.ndarray` . Each values in the array must be `False` where
+        the data are *valid* and True when
+        they are not (like in numpy masked arrays). If `data` is already a
+        :class:`~numpy.ma.MaskedArray` , or any
+        array object (such as a  `NDArray` or subclass of it), providing a `mask` here
+        will cause the mask from the
         masked array to be ignored.
-    units : |Unit| instance or str, optional
-        Units of the data. If data is a |Quantity| then `units` is set to the unit of the `data`; if a unit is also
-        explicitly provided an error is raised. Handling of units use the `pint <https://pint.readthedocs.org/>`_
+    units : `Unit` instance or str, optional
+        Units of the data. If data is a `Quantity` then `units` is set to the unit of
+        the `data`; if a unit is also
+        explicitly provided an error is raised. Handling of units use the
+        `pint <https://pint.readthedocs.org/>`_
         package.
     title : str, optional
-        The title of the dimension. It will later be used for instance for labelling plots of the data.
+        The title of the dimension. It will later be used for instance for labelling
+        plots of the data.
         It is optional but recommended giving a title to each ndarray.
     dlabel :  str, optional
-        Alias of `title`.
+        Alias of `title` .
     meta : dict-like object, optional
         Additional metadata for this object. Must be dict-like but no
         further restriction is placed on meta.
     copy : bool, optional, Default:False
         If True, a deep copy of the passed object is performed.
 
     See Also
     --------
-    NDDataset : Object which subclass |NDArray| with the addition of coordinates.
-    Coord : Object which subclass |NDArray| (coordinates object).
-    LinearCoord : Object which subclass |NDArray| (Linear coordinates object).
+    NDDataset : Object which subclass  `NDArray` with the addition of coordinates.
+    Coord : Object which subclass  `NDArray` (coordinates object).
+    LinearCoord : Object which subclass  `NDArray` (Linear coordinates object).
 
     Examples
     --------
 
     >>> myarray = scp.NDArray([1., 2., 3.], name='myarray')
     >>> assert myarray.name == 'myarray'
     """
@@ -457,15 +478,16 @@
     # Private methods and properties
     # ----------------------------------------------------------------------------------
     def _argsort(self, by=None, pos=None, descend=False):
         # found the indices sorted by values or labels
 
         if by is None:
             warnings.warn(
-                "parameter `by` should be set to `value` or `label`, use `value` by default"
+                "parameter `by` should be set to `value` or `label` , use `value` "
+                "by default"
             )
             by = "value"
 
         if by == "value":
             args = np.argsort(self.data)
         elif "label" in by and not self.is_labeled:
             # by = 'value'
@@ -516,29 +538,31 @@
 
     @default("_dims")
     def _dims_default(self):
         return DEFAULT_DIM_NAME[-self.ndim :]
 
     def _get_dims_from_args(self, *dims, **kwargs):
         # utility function to read dims args and kwargs
-        # sequence of dims or axis, or `dim`, `dims` or `axis` keyword are accepted
+        # sequence of dims or axis, or `dim` , `dims` or `axis` keyword are accepted
 
         # check if we have arguments
         if not dims:
             dims = None
 
         # Check if keyword dims (or synonym axis) exists
         axis = kwargs.pop("axis", None)
 
         kdims = kwargs.pop("dims", kwargs.pop("dim", axis))  # dim or dims keyword
         if kdims is not None:
             if dims is not None:
                 warnings.warn(
-                    "the unnamed arguments are interpreted as `dims`. But a named argument `dims` or `axis`"
-                    "(DEPRECATED) has been specified. \nThe unnamed arguments will thus be ignored.",
+                    "the unnamed arguments are interpreted as `dims` . But a named "
+                    "argument `dims` or `axis`"
+                    "(DEPRECATED) has been specified. \nThe unnamed arguments will "
+                    "thus be ignored.",
                     UserWarning,
                 )
             dims = kdims
 
         if dims is not None and not isinstance(dims, list):
             if isinstance(dims, tuple):
                 dims = list(dims)
@@ -553,15 +577,16 @@
 
         if dims is not None and len(dims) == 1:
             dims = dims[0]
 
         return dims
 
     def _get_dims_index(self, dims):
-        # get the index(es) corresponding to the given dim(s) which can be expressed as integer or string
+        # get the index(es) corresponding to the given dim(s) which can be expressed
+        # as integer or string
 
         if dims is None:
             return
 
         if is_sequence(dims):
             if np.all([d is None for d in dims]):
                 return
@@ -580,15 +605,16 @@
                         f"(not in the dimension's list: {self.dims})."
                     )
                 idx = self.dims.index(dim)
                 axis.append(idx)
 
             else:
                 raise TypeError(
-                    f"Dimensions must be specified as string or integer index, but a value of type "
+                    f"Dimensions must be specified as string or integer index, but a "
+                    f"value of type "
                     f"{type(dim)} has been passed (value:{dim})!"
                 )
 
         for i, item in enumerate(axis):
             # convert to positive index
             if item < 0:
                 axis[i] = self.ndim + item
@@ -673,45 +699,49 @@
         return f"{type(self).__name__}_{str(uuid.uuid1()).split('-')[0]}"
 
     @default("_labels")
     def _labels_default(self):
         return None
 
     def _loc2index(self, loc, dim=None, *, units=None):
-        # Return the index of a location (label or values such as coordinates) along a 1D array.
+        # Return the index of a location (label or values such as coordinates) along a
+        # 1D array.
         # Do not apply for multidimensional arrays (ndim>1)
         if self.ndim > 1:
             raise NotImplementedError(
-                f"not implemented for {type(self).__name__} objects which are not 1-dimensional "
+                f"not implemented for {type(self).__name__} objects which are "
+                f"not 1-dimensional "
                 f"(current ndim:{self.ndim})"
             )
 
         # check units compatibility
         if (
             units is not None
             and (is_number(loc) or is_sequence(loc))
             and units != self.units
         ):
             raise ValueError(
-                f"Units of the location {loc} {units} are not compatible with those of this array:"
+                f"Units of the location {loc} {units} are not compatible with those of"
+                f" this array:"
                 f" {self.units}"
             )
 
         if self.is_empty and not self.is_labeled:
             raise IndexError(f"Could not find this location {loc} on an empty array")
 
         else:
             data = self.data
 
             if is_number(loc):
                 # get the index of a given values
                 error = None
                 if np.all(loc > data.max()) or np.all(loc < data.min()):
                     info_(
-                        f"This coordinate ({loc}) is outside the axis limits ({data.min()}-{data.max()}).\n"
+                        f"This coordinate ({loc}) is outside the axis limits "
+                        f"({data.min()}-{data.max()}).\n"
                         f"The closest limit index is returned"
                     )
                     error = "out_of_limits"
                 index = (np.abs(data - loc)).argmin()
                 # TODO: add some precision to this result
                 if not error:
                     return index
@@ -764,15 +794,16 @@
             try:
                 # Ellipsis
                 if isinstance(_keys[0], np.ndarray):
                     return False
                 test = Ellipsis in _keys
             except ValueError as e:
                 if e.args[0].startswith("The truth "):
-                    # probably an array of index (Fancy indexing)  # should not happen anymore with the test above
+                    # probably an array of index (Fancy indexing)
+                    # should not happen anymore with the test above
                     test = False
             return test
 
         while ellipsisinkeys(keys):
             i = keys.index(Ellipsis)
             keys.pop(i)
             for j in range(self.ndim - len(keys)):
@@ -1158,15 +1189,15 @@
             new.name = ""  # default
 
         return new
 
     @property
     def data(self):
         """
-        The `data` array (|ndarray|).
+        The `data` array (`~numpy.ndarray`).
 
         If there is no data but labels, then the labels are returned instead of data.
         """
         return self._data
 
     @data.setter
     def data(self, data):
@@ -1187,28 +1218,29 @@
         True if the `data` array is dimensionless - Readonly property (bool).
 
         See Also
         --------
         unitless : True if data has no units.
         has_units : True if data has units.
 
-         Notes
+        Notes
         -----
         `Dimensionless` is different of `unitless` which means no unit.
         """
         if self.unitless:
             return False
         return self._units.dimensionless
 
     @property
     def dims(self):
         """
         Names of the dimensions (list).
 
-        The name of the dimensions are 'x', 'y', 'z'.... depending on the number of dimension.
+        The name of the dimensions are 'x', 'y', 'z'....
+        depending on the number of dimension.
         """
         ndim = self.ndim
         if ndim > 0:
             # if len(self._dims)< ndim:
             #    self._dims = self._dims_default()
             dims = self._dims[:ndim]
             return dims
@@ -1218,15 +1250,16 @@
     @dims.setter
     def dims(self, values):
         if isinstance(values, str) and len(values) == 1:
             values = [values]
 
         if not is_sequence(values) or len(values) != self.ndim:
             raise ValueError(
-                f"a sequence of chars with a length of {self.ndim} is expected, but `{values}` "
+                f"a sequence of chars with a length of {self.ndim} is expected, "
+                f"but `{values}` "
                 f"has been provided"
             )
 
         for value in values:
             if value not in DEFAULT_DIM_NAME:
                 raise ValueError(
                     f"{value} value is not admitted. Dimension's name must be among "
@@ -1258,23 +1291,26 @@
 
     @filename.setter
     def filename(self, val):
         self._filename = pathclean(val)
 
     def get_axis(self, *args, **kwargs):
         """
-        Helper function to determine an axis index whatever the syntax used (axis index or dimension names).
+        Helper function to determine an axis index whatever the syntax used (axis index
+        or dimension names).
 
         Parameters
         ----------
         dim, axis, dims : str, int, or list of str or index
-            The axis indexes or dimensions names - they can be specified as argument or using keyword 'axis', 'dim'
+            The axis indexes or dimensions names - they can be specified as argument or
+            using keyword 'axis', 'dim'
             or 'dims'.
         negative_axis : bool, optional, default=False
-            If True a negative index is returned for the axis value (-1 for the last dimension, etc...).
+            If True a negative index is returned for the axis value (-1 for the last
+            dimension, etc...).
         allows_none : bool, optional, default=False
             If True, if input is none then None is returned.
         only_first : bool, optional, default: True
             By default return only information on the first axis if dim is a list.
             Else, return a list for axis and dims information.
 
         Returns
@@ -1327,15 +1363,15 @@
         Parameters
         ----------
         level : int, optional, default:0
             Label level.
 
         Returns
         -------
-        |ndarray|
+        `~numpy.ndarray`
             The labels at the desired level or None.
         """
         if not self.is_labeled:
             return None
 
         if level > self.labels.ndim - 1:
             warnings.warn("There is no such level in the existing labels")
@@ -1486,15 +1522,15 @@
 
     def is_units_compatible(self, other):
         """
         Check the compatibility of units with another object.
 
         Parameters
         ----------
-        other : |ndarray|
+        other : `~numpy.ndarray`
             The ndarray object for which we want to compare units compatibility.
 
         Returns
         -------
         result
             True if units are compatible.
 
@@ -1520,15 +1556,15 @@
 
     def ito(self, other, force=False):
         """
         Inplace scaling to different units. (same as `to` with inplace= True).
 
         Parameters
         ----------
-        other : |Unit| , |Quantity| or str
+        other : `Unit` , `Quantity` or str
             Destination units.
         force : bool, optional, default=`False`
             If True the change of units is forced, even for incompatible units.
 
         See Also
         --------
         to : Rescaling of the current object data to different units.
@@ -1570,55 +1606,62 @@
         to_reduced_units : Rescaling to reduced units.
         """
         self.to_reduced_units(inplace=True)
 
     @property
     def labels(self):
         """
-        An array of labels for `data` (|ndarray| of str).
+        An array of labels for `data` (`~numpy.ndarray` of str).
 
-        An array of objects of any type (but most generally string), with the last dimension size equal to that of the
-        dimension of data. Note that's labelling is possible only for 1D data. One classical application is
-        the labelling of coordinates to display informative strings instead of numerical values.
+        An array of objects of any type (but most generally string), with the last
+        dimension size equal to that of the
+        dimension of data. Note that's labelling is possible only for 1D data. One
+        classical application is
+        the labelling of coordinates to display informative strings instead of
+        numerical values.
         """
         return self._labels
 
     @labels.setter
     def labels(self, labels):
         if labels is None:
             return
 
         if self.ndim > 1:
             warnings.warn(
-                "We cannot set the labels for multidimentional data - Thus, these labels are ignored"
+                "We cannot set the labels for multidimentional data - Thus, these "
+                "labels are ignored"
             )
         else:
             # make sure labels array is of type np.ndarray or Quantity arrays
             if not isinstance(labels, np.ndarray):
                 labels = np.array(labels, subok=True, copy=True).astype(
                     object, copy=False
                 )
 
             if not np.any(labels):
                 # no labels
                 return
 
             else:
                 if (self.data is not None) and (labels.shape[0] != self.shape[0]):
-                    # allow the fact that the labels may have been passed in a transposed array
+                    # allow the fact that the labels may have been passed in a
+                    # transposed array
                     if labels.ndim > 1 and (labels.shape[-1] == self.shape[0]):
                         labels = labels.T
                     else:
                         raise ValueError(
-                            f"labels {labels.shape} and data {self.shape} shape mismatch!"
+                            f"labels {labels.shape} and data {self.shape} "
+                            f"shape mismatch!"
                         )
 
                 if np.any(self._labels):
                     info_(
-                        f"{type(self).__name__} is already a labeled array.\nThe explicitly provided labels will "
+                        f"{type(self).__name__} is already a labeled array.\nThe "
+                        f"explicitly provided labels will "
                         f"be appended to the current labels"
                     )
 
                     labels = labels.squeeze()
                     self._labels = self._labels.squeeze()
                     if self._labels.ndim > 1:
                         self._labels = self._labels.T
@@ -1639,15 +1682,15 @@
             return None
 
         return [self.data.min(), self.data.max()]
 
     @property
     def mask(self):
         """
-        Mask for the data (|ndarray| of bool).
+        Mask for the data (`~numpy.ndarray` of bool).
         """
         if not self.is_masked:
             return NOMASK
 
         return self._mask
 
     @mask.setter
@@ -1677,38 +1720,39 @@
                 NOMASK if self.data is None else np.ones(self.shape).astype(bool)
             )
         else:
             if np.any(self._mask):
                 # this should happen when a new mask is added to an existing one
                 # mask to be combined to an existing one
                 info_(
-                    f"{type(self).__name__} is already a masked array.\n The new mask will be combined with the "
+                    f"{type(self).__name__} is already a masked array.\n The new "
+                    f"mask will be combined with the "
                     f"current array's mask."
                 )
                 self._mask |= mask  # combine (is a copy!)
             else:
                 if self._copy:
                     self._mask = mask.copy()
                 else:
                     self._mask = mask
 
     @property
     def masked_data(self):
         """
-        The actual masked `data` array - Readonly property (|ma.ndarray|).
+        The actual masked `data` array - Readonly property (`numpy.ma.ndarray`).
         """
         if self.is_masked and not self.is_empty:
             return self._umasked(self.data, self.mask)
         else:
             return self.data
 
     @property
     def meta(self):
         """
-        Additional metadata (|Meta|).
+        Additional metadata (`Meta`).
         """
         return self._meta
 
     @meta.setter
     def meta(self, meta):
         if meta is not None:
             self._meta.update(meta)
@@ -1777,15 +1821,16 @@
 
     @property
     def shape(self):
         """
         A tuple with the size of each dimension - Readonly property.
 
         The number of `data` element on each dimension (possibly complex).
-        For only labelled array, there is no data, so it is the 1D and the size is the size of the array of labels.
+        For only labelled array, there is no data, so it is the 1D and the size is the
+        size of the array of labels.
         """
         if self.data is None and self.is_labeled:
             return (self.labels.shape[0],)
 
         elif self.data is None:
             return ()
 
@@ -1825,15 +1870,15 @@
         squeezed : same object type
             The input array, but with all or a subset of the
             dimensions of length 1 removed.
 
         Raises
         ------
         ValueError
-            If `dims` is not `None`, and the dimension being squeezed is not
+            If `dims` is not `None` , and the dimension being squeezed is not
             of length 1
         """
         if inplace:
             new = self
         else:
             new = self.copy()
 
@@ -1859,15 +1904,15 @@
         if return_axis:  # in case we need to know which axis has been squeezed
             return new, axis
 
         return new
 
     def swapdims(self, dim1, dim2, inplace=False):
         """
-        Interchange a two dims of a |NDArray| .
+        Interchange a two dims of a  `NDArray` .
 
         Parameters
         ----------
         dim1 : int or str
             First dimension index.
         dim2 : int
             Second dimension index.
@@ -1900,20 +1945,20 @@
         if self.is_masked:
             new._mask = np.swapaxes(new._mask, *axis)
 
         new._meta = new._meta.swap(*axis, inplace=False)
         return new
 
     swapaxes = swapdims
-    swapaxes.__doc__ = "Alias of `swapdims`."
+    swapaxes.__doc__ = "Alias of `swapdims` ."
 
     @property
     def T(self):
         """
-        Transposed array (|NDArray|).
+        Transposed array ( `NDArray`).
 
         The same object is returned if `ndim` is less than 2.
 
         See Also
         --------
         transpose: Permute the dimensions of an array.
         """
@@ -1939,15 +1984,15 @@
 
     def to(self, other, inplace=False, force=False):
         """
         Return the object with data rescaled to different units.
 
         Parameters
         ----------
-        other : |Quantity| or str
+        other : `Quantity` or str
             Destination units.
         inplace : bool, optional, default=`False`
             Flag to say that the method return a new object (default)
             or not (inplace=True).
         force : bool, optional, default=False
             If True the change of units is forced, even for incompatible units.
 
@@ -1977,15 +2022,16 @@
         We want to change the units to seconds for instance
         but there is no relation with meters,
         so an error is generated during the change
 
         >>> ndd.to('second')
         Traceback (most recent call last):
         ...
-        pint.errors.DimensionalityError: Cannot convert from 'meter' ([length]) to 'second' ([time])
+        pint.errors.DimensionalityError: Cannot convert from 'meter' ([length]) to
+        'second' ([time])
 
         However, we can force the change
 
         >>> ndd.to('second', force=True)
         NDArray: [float64] s (shape: (y:3, x:3))
 
         By default the conversion is not done inplace, so the original is not
@@ -2120,15 +2166,15 @@
         ----------
         inplace : bool
             If True the rescaling is done in place.
 
         Returns
         -------
         rescaled
-            A rescaled array
+            A rescaled array.
         """
         q = Quantity(1.0, self.units)
         q.ito_base_units()
 
         if not inplace:
             new = self.copy()
         else:
@@ -2217,15 +2263,15 @@
     @property
     def transposed(self):
         return self._transposed
 
     @property
     def umasked_data(self):
         """
-        The actual array with mask and unit (|Quantity|).
+        The actual array with mask and unit (`Quantity`).
 
         (Readonly property).
         """
         if self.data is None:
             return None
         return self._uarray(self.masked_data, self.units)
 
@@ -2235,15 +2281,15 @@
         `bool` - True if the `data` does not have `units` (Readonly property).
         """
         return not self.has_units
 
     @property
     def units(self):
         """
-        |Unit| - The units of the data.
+        `Unit` - The units of the data.
         """
         return self._units
 
     @units.setter
     def units(self, units):
         if units is None:
             return
@@ -2263,15 +2309,15 @@
                     f" use the to() method, with force flag set to True"
                 )
         self._units = units
 
     @property
     def values(self):
         """
-        |Quantity| - The actual values (data, units) contained in this object (Readonly property).
+        `Quantity` - The actual values (data, units) contained in this object (Readonly property).
         """
 
         if self.data is not None:
             if self.is_masked:
                 data = self._umasked(self.masked_data, self.mask)
                 if self.units:
                     return Quantity(data, self.units)
@@ -2283,10 +2329,10 @@
                 return data.squeeze()[()]
         elif self.is_labeled:
             return self._labels[()]
 
     @property
     def value(self):
         """
-        Alias of `values`.
+        Alias of `values` .
         """
         return self.values
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/dataset/baseobjects/ndcomplex.py` & `spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/ndcomplex.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
-This module implements a subclass of |NDArray| with complex/quaternion related attributes.
+This module implements a subclass of  `NDArray` with complex/quaternion related attributes.
 """
 
 __all__ = []
 
 import itertools
 import textwrap
 
@@ -34,75 +34,92 @@
 # NDComplexArray
 # ======================================================================================
 class NDComplexArray(NDArray):
     _interleaved = Bool(False)
 
     def __init__(self, data=None, **kwargs):
         """
-        This class provides the complex/quaternion related functionalities to |NDArray| .
+        This class provides the complex/quaternion related functionalities to  `NDArray` .
 
         It is a subclass bringing complex and quaternion related attributes.
 
         Parameters
         ----------
         data : array of complex number or quaternion.
-            Data array contained in the object. The data can be a list, a tuple, a |ndarray| , a ndarray-like,
-            a |NDArray| or any subclass of |NDArray| . Any size or shape of data is accepted. If not given, an empty
-            |NDArray| will be inited.
-            At the initialisation the provided data will be eventually casted to a numpy-ndarray.
-            If a subclass of |NDArray| is passed which already contains some mask, labels, or units, these elements will
-            be used to accordingly set those of the created object. If possible, the provided data will not be copied
-            for `data` input, but will be passed by reference, so you should make a copy of the `data` before passing
+            Data array contained in the object. The data can be a list, a tuple, a
+            `~numpy.ndarray` , a ndarray-like,
+            a  `NDArray` or any subclass of  `NDArray` . Any size or shape of data is
+            accepted. If not given, an empty `NDArray` will be inited.
+            At the initialisation the provided data will be eventually casted to a
+            `numpy.ndarray`\ .
+            If a subclass of  `NDArray` is passed which already contains some mask,
+            labels, or units, these elements will
+            be used to accordingly set those of the created object. If possible, the
+            provided data will not be copied
+            for `data` input, but will be passed by reference, so you should make a
+            copy of the `data` before passing
             them if that's the desired behavior or set the `copy` argument to True.
 
         Other Parameters
         ----------------
         dims : list of chars, optional.
-            if specified the list must have a length equal to the number od data dimensions (ndim) and the chars must be
-            taken among among x,y,z,u,v,w or t. If not specified, the dimension names are automatically attributed in
+            if specified the list must have a length equal to the number od data
+            dimensions (ndim) and the chars must be
+            taken among among x,y,z,u,v,w or t. If not specified, the dimension names
+            are automatically attributed in
             this order.
         name : str, optional
-            A user friendly name for this object. If not given, the automatic `id` given at the object creation will be
+            A user friendly name for this object. If not given, the automatic `id`
+            given at the object creation will be
             used as a name.
         labels : array of objects, optional
-            Labels for the `data`. labels can be used only for 1D-datasets.
-            The labels array may have an additional dimension, meaning several series of labels for the same data.
-            The given array can be a list, a tuple, a |ndarray| , a ndarray-like, a |NDArray| or any subclass of
-            |NDArray| .
-        mask : array of bool or `NOMASK`, optional
-            Mask for the data. The mask array must have the same shape as the data. The given array can be a list,
-            a tuple, or a |ndarray| . Each values in the array must be `False` where the data are *valid* and True when
-            they are not (like in numpy masked arrays). If `data` is already a :class:`~numpy.ma.MaskedArray`, or any
-            array object (such as a |NDArray| or subclass of it), providing a `mask` here will causes the mask from the
+            Labels for the `data` . labels can be used only for 1D-datasets.
+            The labels array may have an additional dimension, meaning several series
+            of labels for the same data.
+            The given array can be a list, a tuple, a `~numpy.ndarray` , a ndarray-like,
+            a  `NDArray` or any subclass of `NDArray` .
+        mask : array of bool or `NOMASK` , optional
+            Mask for the data. The mask array must have the same shape as the data.
+            The given array can be a list,
+            a tuple, or a `~numpy.ndarray` . Each values in the array must be `False`
+            where the data are *valid* and True when
+            they are not (like in numpy masked arrays). If `data` is already a
+            :class:`~numpy.ma.MaskedArray` , or any
+            array object (such as a  `NDArray` or subclass of it), providing a `mask`
+            here will causes the mask from the
             masked array to be ignored.
-        units : |Unit| instance or str, optional
-            Units of the data. If data is a |Quantity| then `units` is set to the unit of the `data`; if a unit is also
-            explicitly provided an error is raised. Handling of units use the `pint <https://pint.readthedocs.org/>`_
+        units : `Unit` instance or str, optional
+            Units of the data. If data is a `Quantity` then `units` is set to the unit
+            of the `data`; if a unit is also
+            explicitly provided an error is raised. Handling of units use the
+            `pint <https://pint.readthedocs.org/>`_
             package.
         title : str, optional
-            The title of the dimension. It will later be used for instance for labelling plots of the data.
+            The title of the dimension. It will later be used for instance for
+            labelling plots of the data.
             It is optional but recommended to give a title to each ndarray.
         dlabel :  str, optional.
-            Alias of `title`.
+            Alias of `title` .
         meta : dict-like object, optional.
             Additional metadata for this object. Must be dict-like but no
             further restriction is placed on meta.
         author : str, optional.
-            name(s) of the author(s) of this dataset. BNy default, name of the computer note where this dataset is
+            name(s) of the author(s) of this dataset. BNy default, name of the computer
+            note where this dataset is
             created.
         description : str, optional.
-            A optional description of the nd-dataset. A shorter alias is `desc`.
+            A optional description of the nd-dataset. A shorter alias is `desc` .
         history : str, optional.
             A string to add to the object history.
         copy : bool, optional
             Perform a copy of the passed object. Default is False.
 
         See Also
         --------
-        NDDataset : Object which subclass |NDArray| with the addition of coordinates.
+        NDDataset : Object which subclass  `NDArray` with the addition of coordinates.
 
         Examples
         --------
         >>> from spectrochempy import NDComplexArray
         >>> myarray = NDComplexArray([1. + 0j, 2., 3.])
         >>> myarray
         NDComplexArray: [complex128] unitless (size: 3)
@@ -208,15 +225,15 @@
                 return np.any(self._mask["I"])
             else:
                 raise e
 
     @property
     def real(self):
         """
-        The array with real component of the `data`.
+        The array with real component of the `data` .
 
         (Readonly property).
         """
         new = self.copy()
         if not new.has_complex_dims:
             return new
         ma = new.masked_data
@@ -235,15 +252,15 @@
         if isinstance(ma, np.ma.masked_array):
             new._mask = ma.mask
         return new
 
     @property
     def imag(self):
         """
-        The array with imaginary component of the `data`.
+        The array with imaginary component of the `data` .
 
         (Readonly property).
         """
         new = self.copy()
         if not new.has_complex_dims:
             return None
 
@@ -264,37 +281,37 @@
         if isinstance(ma, np.ma.masked_array):
             new._mask = ma.mask
         return new
 
     @property
     def RR(self):
         """
-        The array with real component in both dimension of hypercomplex 2D `data`.
+        The array with real component in both dimension of hypercomplex 2D `data` .
 
         This readonly property is equivalent to the `real` property.
         """
         if not self.is_quaternion:
             raise TypeError("Not an hypercomplex array")
         return self.real
 
     @property
     def RI(self):
         """
-        The array with real-imaginary component of hypercomplex 2D `data`.
+        The array with real-imaginary component of hypercomplex 2D `data` .
 
         (Readonly property).
         """
         if not self.is_quaternion:
             raise TypeError("Not an hypercomplex array")
         return self.component("RI")
 
     @property
     def IR(self):
         """
-        The array with imaginary-real component of hypercomplex 2D `data`.
+        The array with imaginary-real component of hypercomplex 2D `data` .
 
         (Readonly property).
         """
         if not self.is_quaternion:
             raise TypeError("Not an hypercomplex array")
         return self.component("IR")
 
@@ -370,29 +387,32 @@
 
         return new
 
     def set_complex(self, inplace=False):
         """
         Set the object data as complex.
 
-        When nD-dimensional array are set to complex, we assume that it is along the first dimension.
-        Two succesives rows are merged to form a complex rows. This means that the number of row must be even
-        If the complexity is to be applied in other dimension, either transpose/swapdims your data before applying this
+        When nD-dimensional array are set to complex, we assume that it is along the
+        first dimension.
+        Two succesives rows are merged to form a complex rows. This means that the
+        number of row must be even
+        If the complexity is to be applied in other dimension, either transpose/swapdims
+        your data before applying this
         function in order that the complex dimension is the first in the array.
 
         Parameters
         ----------
         inplace : bool, optional, default=False
             Flag to say that the method return a new object (default)
             or not (inplace=True).
 
         Returns
         -------
         out
-            Same object or a copy depending on the ``inplace`` flag.
+            Same object or a copy depending on the `inplace` flag.
 
         See Also
         --------
         set_quaternion, has_complex_dims, is_complex, is_quaternion
         """
         if not inplace:  # default is to return a new array
             new = self.copy()
@@ -416,15 +436,15 @@
         inplace : bool, optional, default=False
             Flag to say that the method return a new object (default)
             or not (inplace=True).
 
         Returns
         -------
         out
-            Same object or a copy depending on the ``inplace`` flag.
+            Same object or a copy depending on the `inplace` flag.
         """
         if not inplace:  # default is to return a new array
             new = self.copy()
         else:
             new = self  # work inplace
 
         if new.dtype != typequaternion:  # not already a quaternion
@@ -446,15 +466,15 @@
         inplace : bool, optional, default=False
             Flag to say that the method return a new object (default)
             or not (inplace=True)
 
         Returns
         -------
         transposed
-            Same object or a copy depending on the ``inplace`` flag.
+            Same object or a copy depending on the `inplace` flag.
         """
 
         new = super().transpose(*dims, inplace=inplace)
 
         if new.is_quaternion:
             # here if it is hypercomplex quaternion
             # we should interchange the imaginary component
@@ -479,15 +499,15 @@
         inplace : bool, optional, default=False
             Flag to say that the method return a new object (default)
             or not (inplace=True)
 
         Returns
         -------
         transposed
-            Same object or a copy depending on the ``inplace`` flag.
+            Same object or a copy depending on the `inplace` flag.
         """
 
         new = super().swapdims(dim1, dim2, inplace=inplace)
 
         # we need also to swap the quaternion
         # WARNING: this work only for 2D - when swapdims is equivalent to a 2D transpose
         # TODO: implement something for any n-D array (n>2)
@@ -594,15 +614,16 @@
     def _make_complex(self, data):
 
         if data.dtype in TYPE_COMPLEX:
             return data.astype(np.complex128)
 
         if data.shape[-1] % 2 != 0:
             raise ValueError(
-                "An array of real data to be transformed to complex must have an even number of columns!."
+                "An array of real data to be transformed to complex must have an even "
+                "number of columns!."
             )
 
         data = data.astype(np.float64)
 
         # to work the data must be in C order
         fortran = np.isfortran(data)
         if fortran:
@@ -625,27 +646,30 @@
             raise ValueError(
                 "An array of data to be transformed to quaternion must be 2D."
             )
 
         if data.dtype not in TYPE_COMPLEX:
             if data.shape[1] % 2 != 0:
                 raise ValueError(
-                    "An array of real data to be transformed to quaternion must have even number of columns!."
+                    "An array of real data to be transformed to quaternion must have "
+                    "even number of columns!."
                 )
             # convert to double precision complex
             data = self._make_complex(data)
 
         if data.shape[0] % 2 != 0:
             raise ValueError(
-                "An array data to be transformed to quaternion must have even number of rows!."
+                "An array data to be transformed to quaternion must have even number "
+                "of rows!."
             )
 
         r = data[::2]
         i = data[1::2]
-        #  _data = as_quat_array(list(zip(r.real.flatten(), r.imag.flatten(), i.real.flatten(), i.imag.flatten())))
+        #  _data = as_quat_array(list(zip(r.real.flatten(), r.imag.flatten(),
+        #  i.real.flatten(), i.imag.flatten())))
         #  _data = _data.reshape(r.shape)
 
         self._dtype = None  # reset dtyep
         return as_quaternion(r, i)
 
     # ----------------------------------------------------------------------------------
     # special methods
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/dataset/coord.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/baseline.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,1083 +1,854 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
-This module implements the class |Coord| .
+This module implements the `BaselineCorrection` class for baseline corrections.
 """
+__all__ = ["BaselineCorrection", "ab", "abc", "dc", "basc"]
 
-__all__ = ["Coord", "LinearCoord"]
-
-import copy as cpy
-import textwrap
+__dataset_methods__ = ["ab", "abc", "dc", "basc"]
 
+import matplotlib.pyplot as plt
 import numpy as np
-from traitlets import All, Bool, CFloat, CInt, Instance, Integer, Unicode, Union
-from traitlets import default as traitdefault
-from traitlets import observe
-
-from spectrochempy.core import error_
-from spectrochempy.core.dataset.arraymixins.ndmath import NDMath, _set_operators
-from spectrochempy.core.dataset.baseobjects.ndarray import NDArray
-from spectrochempy.core.units import Quantity, ur
-from spectrochempy.utils.constants import INPLACE, NOMASK
-from spectrochempy.utils.misc import spacing_
-from spectrochempy.utils.print import colored_output
+import scipy.interpolate
+from matplotlib.widgets import SpanSelector
+from traitlets import Enum, Float, HasTraits, Int, List, Tuple, Unicode
+
+from spectrochempy.core import debug_, warning_
+from spectrochempy.core.plotters.multiplot import multiplot
+from spectrochempy.core.processors.smooth import smooth
+from spectrochempy.core.processors.utils import _units_agnostic_method
+from spectrochempy.utils.coordrange import trim_ranges
+from spectrochempy.utils.decorators import signature_has_configurable_traits
+from spectrochempy.utils.misc import TYPE_FLOAT, TYPE_INTEGER
+from spectrochempy.utils.traits import NDDatasetType
+
+
+@signature_has_configurable_traits
+# Note: with this decorator
+# Configurable traits are added to the signature as keywords if they are not yet present.
+class BaselineCorrection(HasTraits):
+    """
+    Baseline Correction processor.
 
+    Two methods are proposed :
 
-# ======================================================================================
-# Coord
-# ======================================================================================
-class Coord(NDMath, NDArray):
-    """
-    Explicit coordinates for a dataset along a given axis.
+    - ``'sequential'`` (default) = classical polynom fit or spline
+      interpolation with separate fitting of each row (spectrum)
+    - ``'multivariate'`` = SVD modeling of baseline, polynomial fit of PC's
+      and calculation of the modeled baseline spectra.
 
-    The coordinates of a |NDDataset| can be created using the |Coord|
-    object.
-    This is a single dimension array with either numerical (float)
-    values or labels (str, `Datetime` objects, or any other kind of objects) to
-    represent the coordinates. Only a one numerical axis can be defined,
-    but labels can be multiple.
+    Interactive mode is proposed using the interactive method `run` .
 
     Parameters
     ----------
-    data : ndarray, tuple or list
-        The actual data array contained in the |Coord| object.
-        The given array (with a single dimension) can be a list,
-        a tuple, a |ndarray| , or a |ndarray|-like object.
-        If an object is passed that contains labels, or units,
-        these elements will be used to accordingly set those of the
-        created object.
-        If possible, the provided data will not be copied for `data` input,
-        but will be passed by reference, so you should make a copy the
-        `data` before passing it in the object constructor if that's the
-        desired behavior or set the `copy` argument to True.
-    **kwargs
-        Optional keywords parameters. See other parameters.
-
-    Other Parameters
-    ----------------
-    dtype : str or dtype, optional, default=np.float64
-        If specified, the data will be casted to this dtype, else the
-        type of the data will be used.
-    dims : list of chars, optional.
-        if specified the list must have a length equal to the number od
-        data dimensions (ndim) and the chars must be
-        taken among among x,y,z,u,v,w or t. If not specified,
-        the dimension names are automatically attributed in
-        this order.
-    name : str, optional
-        A user friendly name for this object. If not given,
-        the automatic `id` given at the object creation will be
-        used as a name..
-    labels : array of objects, optional
-        Labels for the `data`. labels can be used only for 1D-datasets.
-        The labels array may have an additional dimension, meaning
-        several series of labels for the same data.
-        The given array can be a list, a tuple, a |ndarray| ,
-        a ndarray-like, a |NDArray| or any subclass of
-        |NDArray| .
-    units : |Unit| instance or str, optional
-        Units of the data. If data is a |Quantity| then `units` is set
-        to the unit of the `data`; if a unit is also
-        explicitly provided an error is raised. Handling of units use
-        the `pint <https://pint.readthedocs.org/>`_
-        package.
-    title : str, optional
-        The title of the dimension. It will later be used for instance
-        for labelling plots of the data.
-        It is optional but recommended to give a title to each ndarray.
-    dlabel :  str, optional
-        Alias of `title`.
-    copy : bool, optional
-        Perform a copy of the passed object. Default is False.
-    linear : bool, optional
-        If set to True, the coordinate is considered as a
-        ``LinearCoord`` object.
-    offset : float, optional
-        Only used is linear is True.
-        If omitted a value of 0.0 is taken for the coordinate offset.
-    increment : float, optional
-        Only used if linear is true.
-        If omitted a value of 1.0 is taken for the coordinate increment.
+    dataset : `NDDataset`
+        The dataset to be transformed.
 
     See Also
     --------
-    NDDataset : Main SpectroChemPy object: an array with masks, units and
-                coordinates.
-    LinearCoord : linear coordinates.
+    abc : Automatic baseline correction.
+    BaselineCorrector : A helper widget to use in Jupyter notebooks
 
     Examples
     --------
+    .. plot::
+        :include-source:
 
-    We first import the object from the api :
-
-    >>> from spectrochempy import Coord
-
-    We then create a numpy |ndarray| and use it as the numerical `data`
-    axis of our new |Coord| object :
-
-    >>> c0 = Coord.arange(1., 12., 2., title='frequency', units='Hz')
-    >>> c0
-    Coord: [float64] Hz (size: 6)
-
-    We can take a series of str to create a non numerical but labelled
-    axis :
-
-    >>> tarr = list('abcdef')
-    >>> tarr
-    ['a', 'b', 'c', 'd', 'e', 'f']
-
-    >>> c1 = Coord(labels=tarr, title='mylabels')
-    >>> c1
-    Coord: [labels] [  a   b   c   d   e   f] (size: 6)
+        from spectrochempy import *
+        nd = NDDataset.read_omnic('irdata/nh4y-activation.spg')
+        ndp = nd[:, 1291.0:5999.0]
+        bc = BaselineCorrection(ndp)
+        ranges=[[5996., 5998.], [1290., 1300.],
+                [2205., 2301.], [5380., 5979.],
+                [3736., 5125.]]
+        span = bc.compute(*ranges,method='multivariate',
+                          interpolation='pchip', npc=8)
+        _ = bc.corrected.plot_stack()
+        show()
     """
 
-    _copy = Bool()
-
-    _html_output = False
-    _parent_dim = Unicode(allow_none=True)
-
-    # For linear data generation
-    _offset = Union((CFloat(), CInt(), Instance(Quantity)))
-    _increment = Union((CFloat(), CInt(), Instance(Quantity)))
-    _size = Integer(0)
-    _linear = Bool(False)
-
-    # ----------------------------------------------------------------------------------
-    # initialization
-    # ----------------------------------------------------------------------------------
-    def __init__(self, data=None, **kwargs):
-
-        super().__init__(data=data, **kwargs)
-
-        if len(self.shape) > 1:
-            raise ValueError("Only one 1D arrays can be used to define coordinates")
-
-        self._linear = kwargs.pop("linear", False)
-        self._increment = kwargs.pop("increment", 1.0)
-        self._offset = kwargs.pop("offset", 0.0)
-        self._size = kwargs.pop("size", 0)
-        # self._accuracy = kwargs.pop('accuracy', None)
-
-    # ----------------------------------------------------------------------------------
-    # readonly property
-    # ----------------------------------------------------------------------------------
-    @property
-    def reversed(self):
-        """bool - Whether the axis is reversed (readonly
-        property).
-        """
-        if self.units == "ppm":
-            return True
-        elif self.units == "1 / centimeter" and "raman" not in self.title.lower():
-            return True
-        return False
-
-        # Return a correct result only if the data are sorted  # return  # bool(self.data[0] > self.data[-1])
-
-    @property
-    def data(self):
-        """
-        The `data` array (|ndarray|).
-
-        If there is no data but labels, then the labels are returned instead of data.
-        """
-        if self.linear:
-            data = np.arange(self.size) * self._increment + self._offset
-            # if hasattr(data, "units"):
-            #    data = data.m
-        else:
-            data = self._data
-
-        return data
-
-    @data.setter
-    def data(self, data):
-
-        self._set_data(data)
-
-    @property
-    def default(self):
-        # this is in case default is called on a coord, while it is a coordset property
-        return self
-
-    # ----------------------------------------------------------------------------------
-    # hidden properties (for the documentation, only - we remove the docstring)
-    # some of the property of NDArray has to be hidden because they
-    # are not useful for this Coord class
-    # ----------------------------------------------------------------------------------
-    # NDarray methods
-
-    @property
-    def is_complex(self):
-        return False  # always real
-
-    @property
-    def is_empty(self):
-        """
-        True if the `data` array is empty or size=0, and if no label are present
-        - Readonly property (bool).
-        """
-        if not self.linear:
-            return super().is_empty
-
-        return False
-
-    @property
-    def ndim(self):
-        if self.linear:
-            return 1
-        ndim = super().ndim
-        if ndim > 1:
-            raise ValueError("Coordinate's array should be 1-dimensional!")
-        return ndim
-
-    @property
-    def T(self):  # no transpose
-        return self
-
-    # @property
-    # def values(self):
-    #    return super().values
-
-    def to(self, other, inplace=False, force=False):
-
-        new = super().to(other, force=force)
-
-        if inplace:
-            self._units = new._units
-            self._title = new._title
-            self._roi = new._roi
-            if not self.linear:
-                self._data = new._data
-            else:
-                self._offset = new._offset
-                self._increment = new._increment
-                self._linear = new._linear
-
-        else:
-            return new
-
-    to.__doc__ = NDArray.to.__doc__
-
-    @property
-    def masked_data(self):
-        return super().masked_data
+    dataset = NDDatasetType()
 
-    @property
-    def is_masked(self):
-        return False
+    # hidden parameters (not passed in the constructor)
+    corrected = NDDatasetType()
+    method = Enum(
+        ["sequential", "multivariate"],
+        default_value="sequential",
+        help="Method used for baseline resolution.",
+    ).tag(config=True)
+    interpolation = Unicode(
+        "polynomial",
+    )
+    axis = Int(-1)
+    dim = Unicode("")
+    ranges = List(List(minlen=2, maxlen=2))
+    order = Int(1, min=1, allow_none=True)
+    npc = Int(5, min=1, allow_none=True)
+    zoompreview = Float(1.0)
+    figsize = Tuple((7, 5))
+    sps = List()
+
+    def __init__(self, dataset, **kwargs):
+
+        super().__init__(**kwargs)
+
+        self.dataset = dataset
+
+        self.corrected = self.dataset.copy()
+        if kwargs:
+            warning_(
+                "DEPRECATION WARNING: Pass all arguments such range, and method definition in the "
+                "`compute` method, not during the initialisation of the BaselineCorrection instance.\n"
+                "Here they are ignored."
+            )
 
-    @property
-    def linear(self):
-        """
-        Flag to specify if the data can be constructed using a linear variation (bool).
-        """
-        return self._linear
+    def _extendranges(self, *ranges, **kwargs):
+        if not ranges:
+            # look in the kwargs
+            ranges = kwargs.pop("ranges", ())
+        if isinstance(ranges, tuple) and len(ranges) == 1:
+            ranges = ranges[0]  # probably passed with no start to the compute function
+        if not isinstance(ranges, (list, tuple)):
+            ranges = list(ranges)
+        if not ranges:
+            return
 
-    @linear.setter
-    def linear(self, val):
+        if len(ranges) == 2:
+            if isinstance(ranges[0], TYPE_INTEGER + TYPE_FLOAT) and isinstance(
+                ranges[1], TYPE_INTEGER + TYPE_FLOAT
+            ):
+                # a pair a values, we interpret this as a single range
+                ranges = [[ranges[0], ranges[1]]]
+        # find the single values
+        for item in ranges:
+            if isinstance(item, TYPE_INTEGER + TYPE_FLOAT):
+                # a single numerical value: interpret this as a single range
+                item = [item, item]
+            self.ranges.append(item)
+
+    def _setup(self, **kwargs):
+
+        self.method = kwargs.get("method", self.method)
+        self.interpolation = kwargs.get("interpolation", self.interpolation)
+        if self.interpolation == "polynomial":
+            self.order = int(kwargs.get("order", self.order))
+        if self.method == "multivariate":
+            self.npc = int(kwargs.get("npc", self.npc))
+        self.zoompreview = kwargs.get("zoompreview", self.zoompreview)
+        self.figsize = kwargs.get("figsize", self.figsize)
 
-        self._linear = (
-            val  # it val is true this provoque the linearization (  # see observe)
-        )
+    def __call__(self, *ranges, **kwargs):
 
-        # if val and self._data is not None:  #     # linearisation of the data, if possible  #     self._linearize()
+        return self.compute(*ranges, **kwargs)
 
-    @property
-    def offset(self):
+    def compute(self, *ranges, **kwargs):
         """
-        Starting value for linear array
-        """
-        return self._offset
+        Base function for dataset baseline correction.
 
-    @offset.setter
-    def offset(self, val):
-        if isinstance(val, Quantity):
-            if self.has_units:
-                val.ito(self.units)
-                val = val.m
-            else:
-                self.units = val.units
-                val = val.m
-        self._offset = val
-
-    @property
-    def offset_value(self):
-        offset = self.offset
-        if self.units:
-            return Quantity(offset, self._units)
-        else:
-            return offset
-
-    @property
-    def mask(self):
-        return NOMASK
-
-    @mask.setter
-    def mask(self, val):
-        # Coordinates cannot be masked. Set mask always to NOMASK
-        self._mask = NOMASK
-
-    # NDmath methods
-
-    def cumsum(self, **kwargs):
-        raise NotImplementedError
-
-    def mean(self, **kwargs):
-        raise NotImplementedError
-
-    def pipe(self, func=None, *args, **kwargs):
-        raise NotImplementedError
-
-    def remove_masks(self, **kwargs):
-        raise NotImplementedError
+        Parameters
+        ----------
+        *ranges : a variable number of pair-tuples
+            The regions taken into account for the manual baseline correction.
+        **kwargs
+            Optional keyword parameters (see Other Parameters).
 
-    @property
-    def size(self):
-        """
-        Size of the underlying `data` array - Readonly property (int).
+        Other Parameters
+        ----------------
+        dim : str or int, keyword parameter, optional, default='x'.
+            Specify on which dimension to apply the apodization method.
+            If `dim` is specified as an integer
+            it is equivalent  to the usual `axis` numpy parameter.
+        method : str, keyword parameter, optional, default='sequential'
+            Correction method among ['multivariate','sequential']
+        interpolation : string, keyword parameter, optional, default='polynomial'
+            Interpolation method for the computation of the baseline,
+            among ['polynomial','pchip']
+        order : int, keyword parameter, optional, default=1
+            If the correction method polynomial,
+            this give the polynomial order to use.
+        npc : int, keyword parameter, optional, default=5
+            Number of components to keep for the `multivariate` method
+        zoompreview : float, keyword parameter, optional, default=1.0
+            The zoom factor for the preview in interactive mode
+        figsize : tuple, keyword parameter, optional, default=(8, 6)
+            Size of the figure to display in inch
         """
 
-        if self.linear:
-            # the provided size is returned i or its default
-            return self._size
-        else:
-            return super().size
+        self._setup(**kwargs)
 
-    @property
-    def shape(self):
-        if self.linear:
-            return (self._size,)
-        return super().shape
+        # output dataset
+        new = self.corrected
 
-    def std(self, *args, **kwargs):
-        raise NotImplementedError
+        # we assume that the last dimension
+        # if always the dimension to which we want to subtract the baseline.
+        # Swap the axes to be sure to be in this situation
+        axis, dim = new.get_axis(**kwargs, negative_axis=True)
 
-    def sum(self, *args, **kwargs):
-        raise NotImplementedError
+        swapped = False
+        if axis != -1:
+            new.swapdims(axis, -1, inplace=True)
+            swapped = True
 
-    def swapdims(self, *args, **kwargs):
-        raise NotImplementedError
+        lastcoord = new.coordset[dim]
 
-    def swapaxes(self, *args, **kwargs):
-        raise NotImplementedError
+        # most of the time we need sorted axis, so let's do it now
+        is_descendant = False
+        if lastcoord.descendant:
+            new.sort(dim=dim, inplace=True, descend=False)
+            is_descendant = True
+            lastcoord = new.coordset[dim]
 
-    @property
-    def spacing(self):
-        """
-        Return coordinates spacing.
+        x = lastcoord.data
+        self.ranges = [[x[0], x[2]], [x[-3], x[-1]]]
+        self._extendranges(*ranges, **kwargs)
+        self.ranges = ranges = trim_ranges(*self.ranges)
 
-        It will be a scalar if the coordinates are uniformly spaced,
-        else an array of the different spacings
-        """
-        if self.linear:
-            return self.increment * self.units
-        return spacing_(self.data) * self.units
+        baseline = np.zeros_like(new)
 
-    def squeeze(self, *args, **kwargs):
-        raise NotImplementedError
+        # Extract: Sbase: the matrix of data corresponding to ranges
+        #          xbase: the xaxis values corresponding to ranges
 
-    def random(self, *args, **kwargs):
-        raise NotImplementedError
+        s = []
+        for pair in ranges:
+            # determine the slices
 
-    def empty(self, *args, **kwargs):
-        raise NotImplementedError
+            sl = slice(*pair)
+            sect = new[..., sl]
+            if sect is None:
+                continue
 
-    def empty_like(self, *args, **kwargs):
-        raise NotImplementedError
+            s.append(sect)
 
-    def var(self, *args, **kwargs):
-        raise NotImplementedError
+        from spectrochempy.core.dataset.nddataset import NDDataset
 
-    def ones(self, *args, **kwargs):
-        raise NotImplementedError
+        sbase = NDDataset.concatenate(s, axis=-1)
+        # TODO: probably we could use masked data instead of concatenating - could be faster
+        xbase = sbase.coordset(dim)
 
-    def ones_like(self, *args, **kwargs):
-        raise NotImplementedError
+        if self.method == "sequential":
 
-    def full(self, *args, **kwargs):
-        raise NotImplementedError
+            if self.interpolation == "polynomial":
+                # # bad fit when NaN values => are replaced by 0      # NO reason we have Nan -> suppressed
+                # if np.any(np.isnan(sbase)):
+                #     sbase[np.isnan(sbase)] = 0
 
-    def diag(self, *args, **kwargs):
-        raise NotImplementedError
+                polycoef = np.polynomial.polynomial.polyfit(
+                    xbase.data, sbase.data.T, deg=self.order, rcond=None, full=False
+                )
+                baseline = np.polynomial.polynomial.polyval(x, polycoef)
 
-    def diagonal(self, *args, **kwargs):
-        raise NotImplementedError
+            elif self.interpolation == "pchip":
+                for i in range(new.shape[0]):
+                    interp = scipy.interpolate.PchipInterpolator(
+                        xbase.data, sbase.data[i]
+                    )
+                    baseline[i] = interp(x)
 
-    def full_like(self, *args, **kwargs):
-        raise NotImplementedError
+        elif self.method == "multivariate":
 
-    def identity(self, *args, **kwargs):
-        raise NotImplementedError
+            # SVD of Sbase
+            U, s, Vt = np.linalg.svd(sbase.data, full_matrices=False, compute_uv=True)
 
-    def eye(self, *args, **kwargs):
-        raise NotImplementedError
+            # npc cannot be higher than the size of s
+            npc = min(self.npc, s.shape[0])
 
-    def zeros(self, *args, **kwargs):
-        raise NotImplementedError
+            # select npc loadings & compute scores
+            Pt = Vt[0:npc]
+            T = np.dot(U[:, 0:npc], np.diag(s)[0:npc, 0:npc])
 
-    def zeros_like(self, *args, **kwargs):
-        raise NotImplementedError
+            baseline_loadings = np.zeros((npc, new.shape[-1]))
 
-    def coordmin(self, *args, **kwargs):
-        raise NotImplementedError
+            if self.interpolation == "pchip":
+                for i in range(npc):
+                    interp = scipy.interpolate.PchipInterpolator(xbase.data, Pt[i])
+                    baseline_loadings[i] = interp(x)
 
-    def coordmax(self, *args, **kwargs):
-        raise NotImplementedError
+            elif self.interpolation == "polynomial":
+                polycoef = np.polynomial.polynomial.polyfit(
+                    xbase.data, Pt.T, deg=self.order, rcond=None, full=False
+                )
 
-    def conjugate(self, *args, **kwargs):
-        raise NotImplementedError
+                baseline_loadings = np.polynomial.polynomial.polyval(x, polycoef)
 
-    def conj(self, *args, **kwargs):
-        raise NotImplementedError
+            baseline = np.dot(T, baseline_loadings)
 
-    def abs(self, *args, **kwargs):
-        raise NotImplementedError
+        new.data = new.data - baseline
 
-    def absolute(self, *args, **kwargs):
-        raise NotImplementedError
+        # eventually sort back to the original order
+        if is_descendant:
+            new.sort(axis=-1, inplace=True, descend=True)
 
-    def all(self, *args, **kwargs):
-        raise NotImplementedError
-
-    def any(self, *args, **kwargs):
-        raise NotImplementedError
+        new.history = "Baseline correction." + " Method: "
+        if self.method == "Multivariate":
+            new.history = "Multivariate (" + str(self.npc) + " PCs)."
+        else:
+            new.history = "Sequential."
 
-    def argmax(self, *args, **kwargs):
-        raise NotImplementedError
+        if self.interpolation == "polynomial":
+            new.history = "Interpolation: Polynomial, order=" + str(self.order) + ".\n"
+        else:
+            new.history = "Interpolation: Pchip. \n"
 
-    def argmin(self, *args, **kwargs):
-        raise NotImplementedError
+        if swapped:
+            new = new.swapdims(axis, -1)
 
-    def asfortranarray(self, *args, **kwargs):
-        raise NotImplementedError
+        self.corrected = new
+        return new
 
-    def astype(self, dtype=None, **kwargs):
-        """
-        Cast the data to a specified type.
+    def show_regions(self, ax):
+        if self.sps:
+            for sp in self.sps:
+                sp.remove()
+        self.sps = []
+        self.ranges = list(trim_ranges(*self.ranges))
+        for x in self.ranges:
+            x.sort()
+            sp = ax.axvspan(x[0], x[1], facecolor="#2ca02c", alpha=0.5)
+            self.sps.append(sp)
 
-        Parameters
-        ----------
-        dtype : str or dtype
-            Typecode or data-type to which the array is cast.
-        """
-        if not self.linear:
-            self._data = self._data.astype(dtype, **kwargs)
-        else:
-            self._increment = np.array(self._increment).astype(dtype, **kwargs)[()]
-            self._offset = np.array(self._offset).astype(dtype, **kwargs)[()]
-        return self
-
-    def average(self, *args, **kwargs):
-        raise NotImplementedError
-
-    def clip(self, *args, **kwargs):
-        raise NotImplementedError
-
-    def get_axis(self, *args, **kwargs):
-        return super().get_axis(*args, **kwargs)
-
-    @property
-    def origin(self, *args, **kwargs):
-        raise NotImplementedError
-
-    @property
-    def author(self):
-        return None
-
-    @property
-    def descendant(self):
-        return (self.data[-1] - self.data[0]) < 0
-
-    @property
-    def dims(self):
-        return ["x"]
-
-    @property
-    def is_1d(self):
-        return True
-
-    def transpose(self, **kwargs):
-        return self
-
-    # ----------------------------------------------------------------------------------
-    # public methods
-    # ----------------------------------------------------------------------------------
-    def loc2index(self, loc):
+    def run(self, *ranges, **kwargs):
         """
-        Return the index corresponding to a given location.
+        Interactive version of the baseline correction.
 
         Parameters
         ----------
-        loc : float.
-            Value corresponding to a given location on the coordinates axis.
-
-        Returns
-        -------
-        index : int.
-            The corresponding index.
-
-        Examples
-        --------
-
-        >>> dataset = scp.NDDataset.read("irdata/nh4y-activation.spg")
-        >>> dataset.x.loc2index(1644.0)
-        4517
-        """
-        return self._loc2index(loc)
-
-    # ----------------------------------------------------------------------------------
-    # special methods
-    # ----------------------------------------------------------------------------------
-    def __copy__(self):
-        res = self.copy(deep=False)  # we keep name of the coordinate by default
-        res.name = self.name
-        return res
-
-    def __deepcopy__(self, memo=None):
-        res = self.copy(deep=True, memo=memo)
-        res.name = self.name
-        return res
-
-    def __dir__(self):
-        # remove some methods with respect to the full NDArray
-        # as they are not useful for Coord.
-        return [
-            "data",
-            "labels",
-            "units",
-            "title",
-            "name",
-            "offset",
-            "increment",
-            "linear",
-            "roi",
+        *ranges : a variable number of pair-tuples
+            The regions taken into account for the manual baseline correction.
+        **kwargs
+            See other parameter of method compute.
+        """
+        self._setup(**kwargs)
+        self.sps = []
+
+        # output dataset
+        new = self.corrected
+        origin = self.dataset.copy()
+
+        # we assume that the last dimension if always the dimension to which we want to subtract the baseline.
+        # Swap the axes to be sure to be in this situation
+        axis, dim = new.get_axis(**kwargs, negative_axis=True)
+
+        # swapped = False
+        if axis != -1:
+            new.swapdims(axis, -1, inplace=True)
+            origin.swapdims(axis, -1, inplace=True)
+            # swapped = True
+
+        lastcoord = new.coordset[dim]
+
+        # most of the time we need sorted axis, so let's do it now
+
+        if lastcoord.reversed:
+            new.sort(dim=dim, inplace=True, descend=False)
+            lastcoord = new.coordset[dim]
+
+        x = lastcoord.data
+        self.ranges = [[x[0], x[2]], [x[-3], x[-1]]]
+        self._extendranges(*ranges, **kwargs)
+        self.ranges = ranges = trim_ranges(*self.ranges)
+
+        new = self.compute(*ranges, **kwargs)
+
+        # display
+        datasets = [origin, new]
+        labels = [
+            "Click on left button & Span to set regions. Click on right button on a region to remove it.",
+            "Baseline corrected dataset preview",
         ]
+        axes = multiplot(
+            datasets,
+            labels,
+            method="stack",
+            sharex=True,
+            nrow=2,
+            ncol=1,
+            figsize=self.figsize,
+            suptitle="INTERACTIVE BASELINE CORRECTION",
+        )
 
-    def __getitem__(self, items, **kwargs):
-
-        if isinstance(items, list):
-            # Special case of fancy indexing
-            items = (items,)
-
-        # choose, if we keep the same or create new object
-        inplace = False
-        if isinstance(items, tuple) and items[-1] == INPLACE:
-            items = items[:-1]
-            inplace = True
-
-        # Eventually get a better representation of the indexes
-        keys = self._make_index(items)
-
-        # init returned object
-        if inplace:
-            new = self
-        else:
-            new = self.copy()
-
-        # slicing by index of all internal array
-        if new.data is not None:
-            udata = new.data[keys]
-
-            if new.linear:
-                # if self.increment > 0:
-                #     new._offset = udata.min()
-                # else:
-                #     new._offset = udata.max()
-                new._size = udata.size
-                if new._size > 1:
-                    inc = np.diff(udata)
-                    variation = (inc.max() - inc.min()) / udata.ptp()
-                    if variation < 1.0e-5:
-                        new._increment = np.mean(inc)  # np.round(np.mean(
-                        # inc), 5)
-                        new._offset = udata[0]
-                        new._data = None
-                        new._linear = True
-                    else:
-                        new._linear = False
-                else:
-                    new._linear = False
-
-            if not new.linear:
-                new._data = np.asarray(udata)
-
-        if self.is_labeled:
-            # case only of 1D dataset such as Coord
-            new._labels = np.array(self._labels[keys])
-
-        if new.is_empty:
-            error_(
-                IndexError,
-                f"Empty array of shape {new._data.shape} resulted from slicing.\n"
-                f"Check the indexes and make sure to use floats for location slicing",
-            )
-            new = None
-
-        new._mask = NOMASK
-
-        # we need to keep the names when copying coordinates to avoid later
-        # problems
-        new.name = self.name
-        return new
-
-    def __setitem__(self, items, value):
+        fig = plt.gcf()
+        fig.canvas.draw()
 
-        if self.linear:
-            error_(Exception, "Linearly defined array are readonly")
-            return
+        ax1 = axes["axe11"]
+        ax2 = axes["axe21"]
 
-        super().__setitem__(items, value)
+        self.show_regions(ax1)
 
-    def __str__(self):
-        return repr(self)
+        def show_basecor(ax2):
 
-    def _cstr(self, header="  coordinates: ... \n", print_size=True, **kwargs):
+            corrected = self.compute(*ranges, **kwargs)
 
-        indent = kwargs.get("indent", 0)
-
-        out = ""
-        if not self.is_empty and print_size:
-            out += f"{self._str_shape().rstrip()}\n"
-        out += f"        title: {self.title}\n" if self.title else ""
-        if self.has_data:
-            out += "{}\n".format(self._str_value(header=header))
-        elif self.is_empty and not self.is_labeled:
-            out += header.replace("...", "\0Undefined\0")
-
-        if self.is_labeled:
-            header = "       labels: ... \n"
-            text = str(self.labels.T).strip()
-            if "\n" not in text:  # single line!
-                out += header.replace("...", "\0\0{}\0\0".format(text))
+            ax2.clear()
+            ax2.set_title(
+                "Baseline corrected dataset preview", fontweight="bold", fontsize=8
+            )
+            if self.zoompreview > 1:
+                zb = 1.0  # self.zoompreview
+                zlim = [corrected.data.min() / zb, corrected.data.max() / zb]
+                _ = corrected.plot_stack(ax=ax2, colorbar=False, zlim=zlim, clear=False)
             else:
-                out += header
-                out += "\0\0{}\0\0".format(textwrap.indent(text.strip(), " " * 9))
-
-        if out[-1] == "\n":
-            out = out[:-1]
+                _ = corrected.plot_stack(ax=ax2, colorbar=False, clear=False)
 
-        if indent:
-            out = "{}".format(textwrap.indent(out, " " * indent))
+        show_basecor(ax2)
 
-        first_indent = kwargs.get("first_indent", 0)
-        if first_indent < indent:
-            out = out[indent - first_indent :]
-
-        if not self._html_output:
-            return colored_output(out)
-        else:
-            return out
-
-    def __repr__(self):
-        out = self._repr_value().rstrip()
-        return out
-
-    # ----------------------------------------------------------------------------------
-    # Private properties and methods
-    # ----------------------------------------------------------------------------------
-    @traitdefault("_increment")
-    def _increment_default(self):
-        return 1.0
-
-    def _linearize(self):
-
-        if not self.linear or self._data is None:
-            return
-
-        self._linear = False  # to avoid action of the observer
-
-        if self._squeeze_ndim > 1:
-            error_(NotImplementedError, "Linearization is only implemented for 1D data")
-            return
-
-        data = self._data.squeeze()
+        def onselect(xmin, xmax):
+            self.ranges.append([xmin, xmax])
+            self.show_regions(ax1)
+            show_basecor(ax2)
+            fig.canvas.draw()
+
+        def onclick(event):
+            if event.button == 3:
+                for i, r in enumerate(self.ranges):
+                    if r[0] > event.xdata or r[1] < event.xdata:
+                        continue
+                    else:
+                        self.ranges.remove(r)
+                        self.show_regions(ax1)
+                        show_basecor(ax2)
+                        fig.canvas.draw()  # _idle
+
+        _ = fig.canvas.mpl_connect("button_press_event", onclick)
+
+        _ = SpanSelector(
+            ax1,
+            onselect,
+            "horizontal",
+            minspan=5,
+            button=[1],
+            useblit=True,
+            props=dict(alpha=0.5, facecolor="blue"),
+        )
 
-        # try to find an increment
-        if data.size > 1:
-            inc = np.diff(data)
-            variation = (inc.max() - inc.min()) / data.ptp()
-            if variation < 1.0e-5:
-                self._increment = (
-                    data.ptp() / (data.size - 1) * np.sign(inc[0])
-                )  # np.mean(inc)  # np.round(np.mean(inc), 5)
-                self._offset = data[0]
-                self._size = data.size
-                self._data = None
-                self._linear = True
-            else:
-                self._linear = False
-        else:
-            self._linear = False
+        fig.canvas.draw()
 
-    @traitdefault("_offset")
-    def _offset_default(self):
-        return 0
+        return
 
-    def _set_data(self, data):
 
-        if data is None:
-            return
+def basc(dataset, *ranges, **kwargs):
+    """
+    Compute a baseline correction using the BaselineCorrection processor.
 
-        elif isinstance(data, Coord) and data.linear:
-            # Case of LinearCoord
-            for attr in self.__dir__():
-                try:
-                    if attr in ["linear", "offset", "increment"]:
-                        continue
-                    if attr == "data":
-                        val = data.data
-                    else:
-                        val = getattr(data, f"_{attr}")
-                    if self._copy:
-                        val = cpy.deepcopy(val)
-                    setattr(self, f"_{attr}", val)
-                except AttributeError:
-                    # some attribute of NDDataset are missing in NDArray
-                    pass
-
-        elif isinstance(data, NDArray):
-            # init data with data from another NDArray or NDArray's subclass
-            # No need to check the validity of the data
-            # because the data must have been already
-            # successfully initialized for the passed NDArray.data
-            for attr in self.__dir__():
-                try:
-                    val = getattr(data, f"_{attr}")
-                    if self._copy:
-                        val = cpy.deepcopy(val)
-                    setattr(self, f"_{attr}", val)
-                except AttributeError:
-                    # some attribute of NDDataset are missing in NDArray
-                    pass
-
-        elif isinstance(data, Quantity):
-            self._data = np.array(data.magnitude, subok=True, copy=self._copy)
-            self._units = data.units
-
-        elif hasattr(data, "mask"):
-            # an object with data and mask attributes
-            self._data = np.array(data.data, subok=True, copy=self._copy)
-            if isinstance(data.mask, np.ndarray) and data.mask.shape == data.data.shape:
-                self.mask = np.array(data.mask, dtype=np.bool_, copy=False)
-
-        elif (
-            not hasattr(data, "shape")
-            or not hasattr(data, "__getitem__")
-            or not hasattr(data, "__array_struct__")
-        ):
-            # Data doesn't look like a numpy array, try converting it to
-            # one. Non-numerical input are converted to an array of objects.
-            self._data = np.array(data, subok=True, copy=False)
+    2 methods are proposed :
 
-        else:
-            data = np.array(data, subok=True, copy=self._copy)
-            if data.dtype == np.object_:  # likely None value
-                data = data.astype(float)
-            self._data = data
-
-        if self.linear:
-            # we try to replace data by only an offset and an increment
-            self._linearize()
-
-    @staticmethod
-    def _unittransform(new, units):
-        oldunits = new.units
-        if not new.linear:
-            udata = (new.data * oldunits).to(units)
-            new._data = udata.m
-            new._units = udata.units
-        else:
-            offset = (new.offset * oldunits).to(units)
-            increment = (new.increment * oldunits).to(units)
-            new._offset = offset.m
-            new._increment = increment.m
-            new._units = increment.units
-
-        if new._roi is not None:
-            roi = (np.array(new._roi) * oldunits).to(units)
-            new._roi = list(roi)
-
-        # if new._linear:
-        #     # try to make it linear as well
-        #     new._linearize()
-        #     if not new._linear and new._implements("LinearCoord"):
-        #         # can't be linearized -> Coord
-        #         if inplace:
-        #             raise Exception(
-        #                     "A LinearCoord object cannot be transformed to a non linear coordinate "
-        #                     "`inplace`. "
-        #                     "Use to() instead of ito() and leave the `inplace` attribute to False"
-        #             )
-        #         else:
-        #             from spectrochempy import Coord
-        #
-        #             new = Coord(new)
-        return new
+    * `sequential` (default) = classical polynom fit or spline
+      interpolation with separate fitting of each row (spectrum)
+    * `multivariate` = SVD modeling of baseline, polynomial fit of PC's
+      and calculation of the modelled baseline spectra.
 
-    # ----------------------------------------------------------------------------------
-    # Events
-    # ----------------------------------------------------------------------------------
-    @observe(All)
-    def _anytrait_changed(self, change):
-        # ex: change {
-        #   'owner': object, # The HasTraits instance
-        #   'new': 6, # The new value
-        #   'old': 5, # The old value
-        #   'name': "foo", # The name of the changed trait
-        #   'type': 'change', # The event type of the notification, usually
-        #   'change'
-        # }
-
-        if change.name in ["_linear", "_increment", "_offset", "_size"]:
-            if self._linear:
-                self._linearize()
-            return
+    Parameters
+    ----------
+    dataset : a [NDDataset| instance
+        The dataset where to calculate the baseline.
+    \*ranges : a variable number of pair-tuples
+        The regions taken into account for the manual baseline correction.
+    **kwargs
+        Optional keyword parameters (see Other Parameters).
 
-    @property
-    def increment(self):
-        return self._increment
-
-    @increment.setter
-    def increment(self, val):
-        if isinstance(val, Quantity):
-            if self.has_units:
-                val.ito(self.units)
-                val = val.m
-            else:
-                self.units = val.units
-                val = val.m
-        self._increment = val
-
-    @property
-    def increment_value(self):
-        increment = self.increment
-        if self.units:
-            return Quantity(increment, self._units)
-        else:
-            return increment
+    Other Parameters
+    ----------------
+    dim : str or int, keyword parameter, optional, default: 'x'.
+        Specify on which dimension to apply the apodization method.
+        If `dim` is specified as an integer
+        it is equivalent  to the usual `axis` numpy parameter.
+    method : str, keyword parameter, optional, default: 'sequential'
+        Correction method among ['multivariate','sequential']
+    interpolation : string, keyword parameter, optional, default='polynomial'
+        Interpolation method for the computation of the baseline,
+        among ['polynomial','pchip']
+    order : int, keyword parameter, optional, default: 6
+        If the correction method polynomial, this give the polynomial order to use.
+    npc : int, keyword parameter, optional, default: 5
+        Number of components to keep for the `multivariate` method
 
+    See Also
+    --------
+    BaselineCorrection : Manual baseline corrections.
+    abc : Automatic baseline correction.
 
-class LinearCoord(Coord):
+    Notes
+    -----
+    For more flexibility and functionality, it is advised to use the BaselineCorrection
+    processor instead.
     """
-    Linear coordinates.
+    blc = BaselineCorrection(dataset)
+    if not ranges and dataset.meta.regions is not None:
+        # use the range stored in metadata
+        ranges = dataset.meta.regions["baseline"]
+    return blc.compute(*ranges, **kwargs)
 
-    Such coordinates correspond to a ascending or descending linear
-    sequence of values, fully determined by two parameters, i.e., an offset (off) and an increment (inc) :
 
-    .. math::
+# ======================================================================================
+# abc # TODO: some work to perform on this
+# ======================================================================================
+def abc(dataset, dim=-1, **kwargs):
+    """
+    Automatic baseline correction.
 
-        \\mathrm{data} = i*\\mathrm{inc} + \\mathrm{off}.
+    Various algorithms are provided to calculate the baseline automatically.
 
     Parameters
     ----------
-    data : a 1D array-like object, optional
-        WWen provided, the `size` parameters is adjusted to the size of
-        the array, and a linearization of the
-        array is performed (only if it is possible: regular spacing in
-        the 1.e5 relative accuracy).
-    offset : float, optional
-        If omitted a value of 0.0 is taken for the coordinate offset.
-    increment : float, optional
-        If omitted a value of 1.0 is taken for the coordinate increment.
+    dataset : a [NDDataset| instance
+        The dataset where to calculate the baseline.
+    dim : str or int, optional
+        The dataset dimentsion where to calculate the baseline. Default is -1.
     **kwargs
-        Optional keywords parameters. See other parameters.
+        Optional keyword parameters (see Other Parameters).
+
+    Returns
+    -------
+    baseline_corrected
+        A baseline corrected dataset.
+    baseline_only
+        Only the baseline (apply must be set to False).
+    baseline_points
+        Points where the baseline is calculated (return_points must be set to True).
 
     Other Parameters
     ----------------
-    dtype : str or dtype, optional, default=np.float64
-        If specified, the data will be casted to this dtype, else the
-        type of the data will be used
-    dims : list of chars, optional.
-        if specified the list must have a length equal to the number od
-        data dimensions (ndim) and the chars must be
-        taken among x,y,z,u,v,w or t. If not specified,
-        the dimension names are automatically attributed in
-        this order.
-    name : str, optional
-        A user-friendly name for this object. If not given,
-        the automatic `id` given at the object creation will be
-        used as a name.
-    labels : array of objects, optional
-        Labels for the `data`. labels can be used only for 1D-datasets.
-        The labels array may have an additional dimension, meaning
-        several series of labels for the same data.
-        The given array can be a list, a tuple, a |ndarray| ,
-        a ndarray-like, a |NDArray| or any subclass of
-        |NDArray| .
-    units : |Unit| instance or str, optional
-        Units of the data. If data is a |Quantity| then `units` is set
-        to the unit of the `data`; if a unit is also
-        explicitly provided an error is raised. Handling of units use
-        the `pint <https://pint.readthedocs.org/>`_
-        package.
-    title : str, optional
-        The title of the dimension. It will later be used for instance
-        for labelling plots of the data.
-        It is optional but recommended to give a title to each ndarray.
-    dlabel : str, optional.
-        Alias of `title`.
-    meta : dict-like object, optional.
-        Additional metadata for this object. Must be dict-like but no
-        further restriction is placed on meta.
-    copy : bool, optional
-        Perform a copy of the passed object. Default is False.
-    fill_missing : bool
-        Create a linear coordinate array where missing data are masked.
+    basetype : string, optional, default: 'linear'
+        See notes - available = linear, basf, ...
+    window : float/int, optional, default is 0.05
+        If float <1 then the corresponding percentage of the axis size is taken as window.
+    nbzone : int, optional, default is 32
+        Number of zones. We will divide the size of the last axis by this number
+        to determine the number of points in each zone (nw).
+    mult : int
+        A multiplicator. determine the number of point for the database calculation (nw*mult<n base points).
+    nstd : int, optional, default is 2 times the standard error
+        Another multiplicator. Multiply the standard error to determine the region in which points are from the
+        baseline.
+    polynom : bool, optional, default is True
+        If True a polynom is computed for the base line, else an interpolation is achieved betwwen points.
+    porder : int, default is 6
+        Order of the polynom to fit on the baseline points
+    return_points : bool, optional, default is False
+        If True, the points abscissa used to determine the baseline are returned.
+    apply : bool, optional, default is True
+        If apply is False, the data are not modified only the baseline is returned.
+    return_pts : bool, optional, default is False
+        If True, the baseline reference points are returned.
 
     See Also
     --------
-    NDDataset : Main SpectroChemPy object: an array with masks, units and
-    coordinates.
-    Coord : Explicit coordinates.
+    BaselineCorrection : Manual baseline corrections.
+    basc : Manual baseline correction.
+
+    Notes
+    -----
+    #TODO: description of these algorithms
+    * linear -
+    * basf -
 
     Examples
     --------
-    >>> from spectrochempy import LinearCoord, Coord
-
-    To create a linear coordinate, we need to specify an offset,
-    an increment and
-    the size of the data
+    To be done
+    """
+    # # options evaluation
+    # parser = argparse.ArgumentParser(description='BC processing.', usage="""
+    # ab [-h] [--mode {linear,poly, svd}] [--dryrun]
+    #                        [--window WINDOW] [--step STEP] [--nbzone NBZONE]
+    #                        [--mult MULT] [--order ORDER] [--verbose]
+    # """)
+    # # positional arguments
+    # parser.add_argument('--mode', '-mo', default='linear',
+    #                      choices=['linear', 'poly', 'svd'], help="mode of correction")
+    # parser.add_argument('--dryrun', action='store_true', help='dry flag')
+    #
+    # parser.add_argument('--window', '-wi', default=0.05, type=float, help='selected window for linear and svd bc')
+    # parser.add_argument('--step', '-st', default=5, type=int, help='step for svd bc')
+    # parser.add_argument('--nbzone', '-nz', default=32, type=int, help='number of zone for poly')
+    # parser.add_argument('--mult', '-mt', default=4, type=int, help='multiplicator of zone for poly')
+    # parser.add_argument('--order', '-or', default=5, type=int, help='polynom order for poly')
+    #
+    # parser.add_argument('--verbose', action='store_true', help='verbose flag')
+    # args = parser.parse_args(options.split())
+    #
+    # source.history.append('baseline correction mode:%s' % args.mode)
+
+    inplace = kwargs.pop("inplace", False)
+    dryrun = kwargs.pop("dryrun", False)
+
+    # output dataset inplace or not
+    if not inplace or dryrun:  # default
+        new = dataset.copy()
+    else:
+        new = dataset
+
+    axis, dim = new.get_axis(dim, negative_axis=True)
+    swapped = False
+    if axis != -1:
+        new.swapdims(axis, -1, inplace=True)  # must be done in  place
+        swapped = True
+
+    base = _basecor(new.data.real, **kwargs)
+
+    if not dryrun:
+        new.data -= base  # return the corrected spectra
+    else:
+        new.data = base  # return the baseline
+
+    # restore original data order if it was swapped
+    if swapped:
+        new.swapdims(axis, -1, inplace=True)  # must be done inplace
 
-    >>> c1 = LinearCoord(offset=2.0, increment=2.0, size=10)
+    new.history = "`abc` Baseline correction applied."
+    return new
 
-    Alternatively, linear coordinates can be created using the
-    ``linear`` keyword
 
-    >>> c2 = Coord(linear=True, offset=2.0, increment=2.0, size=10)
+def ab(dataset, dim=-1, **kwargs):
     """
+    Alias of `abc` .
+    """
+    return abs(dataset, dim, **kwargs)
 
-    _use_time = Bool(False)
-    _show_datapoints = Bool(True)
-    _zpd = Integer()
-
-    def __init__(self, data=None, offset=0.0, increment=1.0, **kwargs):
-
-        if data is not None and isinstance(data, Coord) and not data.linear:
-            raise ValueError(
-                "Only linear Coord (with attribute linear set to True, can be transformed into "
-                "LinearCoord class"
-            )
-
-        super().__init__(data, **kwargs)
 
-        # when data is present, we don't need offset and increment, nor size,
-        # we just do linear=True and these parameters are ignored
+@_units_agnostic_method
+def dc(dataset, **kwargs):
+    """
+    Time domain baseline correction.
 
-        if self._data is not None:
-            self._linear = True
+    Parameters
+    ----------
+    dataset : nddataset
+        The time domain daatset to be corrected.
+    kwargs : dict, optional
+        Additional parameters.
+
+    Returns
+    -------
+    dc
+        DC corrected array.
 
-        elif not self.linear:
-            # in case it was not already a linear array
-            self.offset = offset
-            self.increment = increment
-            self._linear = True
-
-    @property  # read only
-    def linear(self):
-        return self._linear
-
-    def __dir__(self):
-        # remove some methods with respect to the full NDArray
-        # as they are not useful for Coord.
-
-        return [
-            "data",
-            "labels",
-            "units",
-            "meta",
-            "title",
-            "name",
-            "offset",
-            "increment",
-            "linear",
-            "size",
-            "roi",
-            "show_datapoints",
-        ]
+    Other Parameters
+    ----------------
+    len : float, optional
+        Proportion in percent of the data at the end of the dataset to take into account. By default, 25%.
+    """
 
-    def set_laser_frequency(self, frequency=15798.26 * ur("cm^-1")):
+    len = int(kwargs.pop("len", 0.25) * dataset.shape[-1])
+    dc = np.mean(np.atleast_2d(dataset)[..., -len:])
+    dataset -= dc
 
-        if not isinstance(frequency, Quantity):
-            frequency = frequency * ur("cm^-1")
+    return dataset
 
-        frequency.ito("Hz")
-        self.meta.laser_frequency = frequency
 
-        if self._use_time:
-            spacing = 1.0 / frequency
-            spacing.ito("picoseconds")
-
-            self.increment = spacing.m
-            self.offset = 0
-            self._units = ur.picoseconds
-            self.title = "time"
+# ======================================================================================
+# private functions
+# ======================================================================================
+def _basecor(data, **kwargs):
+    mode = kwargs.pop("mode", "linear")
 
-        else:
-            frequency.ito("cm^-1")
-            spacing = 1.0 / frequency
-            spacing.ito("mm")
-
-            self.increment = spacing.m
-            self.offset = -self.increment * self._zpd
-            self._units = ur.mm
-            self.title = "optical path difference"
-
-    @property
-    def _use_time_axis(self):
-        # private property
-        # True if time scale must be used for interferogram axis. Else it
-        # will be set to optical path difference.
-        return self._use_time
-
-    @_use_time_axis.setter
-    def _use_time_axis(self, val):
-
-        self._use_time = val
-        if "laser_frequency" in self.meta:
-            self.set_laser_frequency(self.meta.laser_frequency)
+    if mode == "linear":
+        return _linearbase(data, **kwargs)
 
-    @property
-    def show_datapoints(self):
-        """
-        Bool : True if axis must discard values and show only datapoints.
+    if mode == "svd":
+        return _svdbase(data, **kwargs)
 
-        """
-        if "laser_frequency" not in self.meta or self.units.dimensionality not in [
-            "[time]",
-            "[length]",
-        ]:
-            return False
+    if mode == "poly":
+        return _polybase(data, **kwargs)
+    else:
+        raise ValueError(f"`ab` mode = `{mode}`  not known")
+
+
+#
+# _linear mode
+#
+def _linearbase(data, **kwargs):
+    # Apply a linear baseline correction
+    # Very simple and naive procedure that compute a straight baseline from side to the other
+    # (averging on a window given by the window parameters : 5% of the total width on each side by default)
+
+    window = kwargs.pop("window", 0.05)
+
+    if window <= 1.0:
+        # percent
+        window = int(data.shape[-1] * window)
+
+    if len(data.shape) == 1:
+        npts = float(data.shape[-1])
+        a = (data[-window:].mean() - data[:window].mean()) / (npts - 1.0)
+        b = data[:window].mean()
+        baseline = a * np.arange(npts) + b
+
+    else:
+        npts = float(data.shape[-1])
+        a = (data[:, -window:].mean(axis=-1) - data[:, :window].mean(axis=-1)) / (
+            npts - 1.0
+        )
+        b = data[:, :window].mean(axis=-1)
+        baseline = (((np.ones_like(data).T * a).T * np.arange(float(npts))).T + b).T
 
-        return self._show_datapoints
+    return baseline
 
-    @show_datapoints.setter
-    def show_datapoints(self, val):
 
-        self._show_datapoints = val
+def _planeFit(points):
+    # p, n = planeFit(points)  # copied from https://stackoverflow.com/a/18968498
+    #
+    # Fit an multi-dimensional plane to the points.
+    # Return a point on the plane and the normal.
+    #
+    # Parameters
+    # ----------
+    # points :
+    #
+    # Notes
+    # -----
+    #     Replace the nonlinear optimization with an SVD.
+    #     The following creates the moment of inertia tensor, M, and then
+    #     SVD's it to get the normal to the plane.
+    #     This should be a close approximation to the least-squares fit
+    #     and be much faster and more predictable.
+    #     It returns the point-cloud center and the normal.
+
+    from numpy.linalg import svd
+
+    npts = points.shape[0]
+    points = np.reshape(points, (npts, -1))
+    assert points.shape[0] < points.shape[1]
+    ctr = points.mean(axis=1)
+    x = points - ctr[:, None]
+    M = np.dot(x, x.T)
+    return ctr, svd(M)[0][:, -1]
+
+
+def _svdbase(data, args=None, retw=False):
+    # Apply a planar baseline correction to 2D data
+    import pandas as pd  # TODO: suppress this need
+
+    if not args:
+        window = 0.05
+        step = 5
+    else:
+        window = args.window
+        step = args.step
+
+    if window <= 1.0:
+        # percent
+        window = int(data.shape[-1] * window)
+
+    data = pd.DataFrame(
+        data
+    )  # TODO: facilitate the manipulation (but to think about further)
+    a = pd.concat([data.iloc[:window], data.iloc[-window:]])
+    b = pd.concat(
+        [data.iloc[window:-window, :window], data.iloc[window:-window, -window:]],
+        axis=1,
+    )
+    bs = pd.concat([a, b])
+    bs = bs.stack()
+    bs.sort()
+    x = []
+    y = []
+    z = []
+    for item in bs.index[::step]:
+        x.append(item[0])
+        y.append(item[1])
+        z.append(bs[item].real)
+
+    norm = np.max(np.abs(z))
+    z = np.array(z)
+    z = z / norm
+    XYZ = np.array((x, y, z))
+    p, n = _planeFit(XYZ)
+    d = np.dot(p, n)
+
+    col = data.columns
+    row = data.index
+    X, Y = np.meshgrid(col, row)
+    Z = -norm * (n[0] * X + n[1] * Y - d) / n[2]
+
+    if retw:
+        return Z, None  # TODO: return something
+    return Z
+
+
+def _polybase(data, **kwargs):
+    # Automatic baseline correction
+
+    if data.ndim == 1:
+        dat = np.array(
+            [
+                data,
+            ]
+        )
 
-    @property
-    def laser_frequency(self):
-        """
-        Laser frequency if needed (Quantity).
-        """
-        return self.meta.laser_frequency
+    nbzone = kwargs.pop("nbzone", 64)
+    mult = kwargs.pop("mult", 4)
+    order = kwargs.pop("order", 6)
+
+    npts = data.shape[-1]
+    w = np.arange(npts)
+
+    baseline = np.ma.masked_array(dat, mask=True)
+    sigma = 1.0e6
+    nw = int(npts / nbzone)
+
+    # print (nw)
+    # unmask extremities of the baseline
+    baseline[:, :nw].mask = False
+    baseline[:, -nw:].mask = False
+
+    for j in range(nbzone):
+        s = dat[:, nw * j : min(nw * (j + 1), npts + 1)]
+        sigma = min(s.std(), sigma)
+
+    nw = nw * 2  # bigger window
+    nw2 = int(nw / 2)
+
+    found = False
+    nb = 0
+    nstd = 2.0
+    while (not found) or (nb < nw * mult):
+        nb = 0
+        for i in range(nw2, npts - nw2 + 1, 1):
+            s1 = dat[:, max(i - 1 - nw2, 0) : min(i - 1 + nw2, npts + 1)]
+            s2 = dat[:, max(i - nw2, 0) : min(i + nw2, npts + 1)]
+            s3 = dat[:, max(i + 1 - nw2, 0) : min(i + 1 + nw2, npts + 1)]
+            mi1, mi2, mi3 = s1.min(), s2.min(), s3.min()
+            ma1, ma2, ma3 = s1.max(), s2.max(), s3.max()
+
+            if (
+                abs(ma1 - mi1) < float(nstd) * sigma
+                and abs(ma2 - mi2) < float(nstd) * sigma
+                and abs(ma3 - mi3) < float(nstd) * sigma
+            ):
+                found = True
+                nb += 1
+                baseline[:1, i].mask = False  # baseline points
+
+        # increase nstd
+        nstd = nstd * 1.1
+    debug_("basf optimized nstd: %.2F mult: %.2f" % (nstd, mult))
+
+    wm = np.array(list(zip(*np.argwhere(~baseline[:1].mask)))[1])
+    bm = baseline[:, wm]
+    if data.ndim > 1:
+        bm = smooth(bm.T, max(int(dat.shape[0] / 10), 3)).T
+    bm = smooth(bm, max(int(dat.shape[-1] / 10), 3))
+
+    # if not polynom:
+    #    sr = pchip(wm, bm.real)
+    #    si = pchip(wm, bm.imag)
+    #    baseline = sr(w) + si(w) * 1.0j
+    #    baseline = smooth(baseline, window_len=int(nw / 4))
+    # else:
+    # fit a polynom
+    pf = np.polyfit(wm, bm.T, order).T
+    for i, row in enumerate(pf[:]):
+        poly = np.poly1d(row)
+        baseline[i] = poly(w)
 
-    @laser_frequency.setter
-    def laser_frequency(self, val):
-        self.meta.aser_frequency = val
+    if data.ndim == 1:
+        baseline = baseline[0]
 
+    return baseline
 
-# ======================================================================================
-# Set the operators
-# ======================================================================================
-_set_operators(Coord, priority=50)
-_set_operators(LinearCoord, priority=50)
 
-# ======================================================================================
 if __name__ == "__main__":
     pass
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/dataset/coordset.py` & `spectrochempy-0.6.1/spectrochempy/core/dataset/coordset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
-This module implements class |CoordSet| .
+This module implements class `CoordSet` .
 """
 
 __all__ = ["CoordSet"]
 
 import copy as cpy
 import uuid
 import warnings
@@ -21,52 +21,54 @@
     Dict,
     HasTraits,
     Int,
     List,
     Unicode,
     default,
     observe,
+    signature_has_traits,
     validate,
 )
 
 from spectrochempy.core.dataset.baseobjects.ndarray import DEFAULT_DIM_NAME, NDArray
 from spectrochempy.core.dataset.coord import Coord, LinearCoord
 from spectrochempy.utils.misc import is_sequence
 from spectrochempy.utils.print import colored_output, convert_to_html
 
 
 # ======================================================================================
 # CoordSet
 # ======================================================================================
+@signature_has_traits
 class CoordSet(HasTraits):
     """
     A collection of Coord objects for a NDArray object with validation.
 
     This object is an iterable containing a collection of Coord objects.
 
     Parameters
     ----------
-    *coords : |NDarray| , |NDArray| subclass or |CoordSet| sequence of objects.
+    \*coords : `NDArray` ,  `NDArray` subclass or `CoordSet` sequence of objects.
         If an instance of CoordSet is found, instead of an array, this means
         that all coordinates in this coords describe the same axis.
         It is assumed that the coordinates are passed in the order of the
         dimensions of a nD numpy array (
         `row-major <https://docs.scipy.org/doc/numpy-1.14.1/glossary.html#term-row-major>`_
         order), i.e., for a 3d object : 'z', 'y', 'x'.
     **kwargs
         Additional keyword parameters (see Other Parameters).
 
     Other Parameters
     ----------------
-    x : |NDarray| , |NDArray| subclass or |CoordSet|
+    x : `NDArray` ,  `NDArray` subclass or `CoordSet`
         A single coordinate associated to the 'x'-dimension.
         If a coord was already passed in the argument, this will overwrite
         the previous. It is thus not recommended to simultaneously use
         both way to initialize the coordinates to avoid such conflicts.
-    y, z, u, ... : |NDarray| , |NDArray| subclass or |CoordSet|
+    y, z, u, ... : `NDArray` ,  `NDArray` subclass or `CoordSet`
         Same as `x` for the others dimensions.
     dims : list of string, optional
         Names of the dims to use corresponding to the coordinates. If not
         given, standard names are used: x, y, ...
     copy : bool, optional
         Perform a copy of the passed object. Default is True.
 
@@ -238,15 +240,15 @@
                     # replace it
                     idx = self.names.index(key)
                     coord.name = key
                     self._coords[idx] = coord
 
                 else:
                     raise KeyError(
-                        f"Probably an invalid key (`{key}`) for coordinates has been passed. "
+                        f"Probably an invalid key (`{key}` ) for coordinates has been passed. "
                         f"Valid keys are among:{DEFAULT_DIM_NAME}"
                     )
 
             else:
                 raise ValueError(
                     f"Probably an invalid type of coordinates has been passed: {key}:{coord} "
                 )
@@ -264,15 +266,15 @@
 
         # initialize the base class with the eventual remaining arguments
         super().__init__(**kwargs)
 
     @staticmethod
     def _implements(name=None):
         """
-        Utility to check if the current object implement `CoordSet`.
+        Utility to check if the current object implement `CoordSet` .
 
         Rather than isinstance(obj, CoordSet) use object._implements('CoordSet').
 
         This is useful to check type without importing the module.
         """
         if name is None:
             return "CoordSet"
@@ -599,15 +601,15 @@
             coordinate's name list. This
             is the recommended way to set titles as this will be less prone to errors.
 
         Notes
         -----
         If the args are not named, then the attributions are made in coordinate's  name
         alphabetical order :
-        e.g, the first title will be for the `x` coordinates, the second for the `y`,
+        e.g, the first title will be for the `x` coordinates, the second for the `y` ,
         etc.
         """
         if len(args) == 1 and (is_sequence(args[0]) or isinstance(args[0], CoordSet)):
             args = args[0]
 
         for i, item in enumerate(args):
             if not isinstance(self[i], CoordSet):
@@ -632,21 +634,21 @@
             alphabetical order.
         **kwargs
             Keyword attribution of the units. The keys must be valid names among the
             coordinate's name list. This
             is the recommended way to set units as this will be less prone to errors.
         force : bool, optional, default=False
             Whether or not the new units must be compatible with the current units. See
-            the `Coord`.`to` method.
+            the `Coord` .`to` method.
 
         Notes
         -----
         If the args are not named, then the attributions are made in coordinate's name
         alphabetical order :
-        e.g, the first units will be for the `x` coordinates, the second for the `y`, etc.
+        e.g, the first units will be for the `x` coordinates, the second for the `y` , etc.
         """
         force = kwargs.pop("force", False)
 
         if len(args) == 1 and is_sequence(args[0]):
             args = args[0]
 
         for i, item in enumerate(args):
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/dataset/nddataset.py` & `spectrochempy-0.6.1/spectrochempy/core/dataset/nddataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,26 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
-This module implements the |NDDataset| class.
+This module implements the `NDDataset` class.
 """
 
 __all__ = ["NDDataset"]
 
 import sys
 import textwrap
 from datetime import datetime, tzinfo
 
 import numpy as np
 import pytz  # TODO: for py>=3.9, we could use builtin zoneinfo library instead of pyt
-from traitlets import (
-    All,
-    Bool,
-    Float,
-    HasTraits,
-    Instance,
-    List,
-    Tuple,
-    Unicode,
-    default,
-    observe,
-    validate,
-)
+import traitlets as tr
 
 from spectrochempy.core import error_, warning_
 from spectrochempy.core.dataset.arraymixins.ndio import NDIO
 from spectrochempy.core.dataset.arraymixins.ndmath import NDMath  # _set_ufuncs,
 from spectrochempy.core.dataset.arraymixins.ndmath import _set_operators
 from spectrochempy.core.dataset.arraymixins.ndplot import NDPlot
 from spectrochempy.core.dataset.baseobjects.ndarray import DEFAULT_DIM_NAME, NDArray
@@ -47,170 +35,158 @@
 
 #       but we need compatibility with 3.7 (Colab).
 
 
 # ======================================================================================
 # NDDataset class definition
 # ======================================================================================
+@tr.signature_has_traits
 class NDDataset(NDMath, NDIO, NDPlot, NDComplexArray):
     """
-    The main N-dimensional dataset class used by |scpy| .
+    The main N-dimensional dataset class used by  `SpectroChemPy`\ .
 
-    The NDDataset is the main object use by SpectroChemPy. Like numpy
-    ndarrays, NDDataset have the capability to be
-    sliced, sorted and subject to mathematical operations. But, in addition,
-    NDDataset may have units,
-    can be masked
-    and each dimensions can have coordinates also with units. This make
-    NDDataset aware of unit compatibility,
-    e.g.,
-    for binary operation such as additions or subtraction or during the
+    The `NDDataset` is the main object use by SpectroChemPy. Like numpy
+    `~numpy.ndarray`\ s, `NDDataset` have the capability to be sliced, sorted and subject to
+    mathematical operations. But, in addition, `NDDataset` may have units,
+    can be masked and each dimensions can have coordinates also with units. This make
+    `NDDataset` aware of unit compatibility,
+    *e.g.,* for binary operation such as additions or subtraction or during the
     application of mathematical operations.
     In addition or in replacement of numerical data for coordinates,
-    NDDataset can also have labeled coordinates
-    where labels can be different kind of objects (strings, datetime,
-    numpy nd.ndarray or other NDDatasets, etc…).
+    `NDDataset` can also have labeled coordinates where labels can be different kind of
+    objects (`str`\ , `datetime`\ , `~numpy.ndarray` or other `NDDataset`\ 's, etc...).
 
     Parameters
     ----------
-    data : array of floats
+    data : :term:`array-like`
         Data array contained in the object. The data can be a list, a tuple,
-        a |ndarray| , a ndarray-like,
-        a |NDArray| or any subclass of |NDArray| . Any size or shape of data
-        is accepted. If not given, an empty
-        |NDArray| will be inited.
-        At the initialisation the provided data will be eventually casted to
-        a numpy-ndarray.
-        If a subclass of |NDArray| is passed which already contains some
-        mask, labels, or units, these elements
-        will
-        be used to accordingly set those of the created object. If possible,
-        the provided data will not be copied
+        a `~numpy.ndarray`, a subclass of `~numpy.ndarray`, another `NDDataset` or a  `Coord` object.
+        Any size or shape of data is accepted. If not given, an empty
+        `NDDataset` will be inited.
+        At the initialisation the provided data will be eventually cast to
+        a `~numpy.ndarray`\ .
+        If the provided objects is passed which already contains some
+        mask, or units, these elements will be used if possible to accordingly set
+        those of the created object. If possible, the provided data will not be copied
         for `data` input, but will be passed by reference, so you should
-        make a copy of the `data` before passing
-        them if that's the desired behavior or set the `copy` argument to True.
-    coordset : An instance of |CoordSet| , optional
-        `coords` contains the coordinates for the different dimensions of
-        the `data`. if `coords` is provided,
-        it must specified the `coord` and `labels` for all dimensions of the
-        `data`.
-        Multiple `coord`'s can be specified in an |CoordSet| instance for
-        each dimension.
-    coordunits : list, optional
+        make a copy of the `data` before passing them if that's the desired behavior
+        or set the `copy` argument to `True`\ .
+    coordset : `CoordSet` instance, optional
+        It contains the coordinates for the different dimensions of the `data`\ .
+        if `CoordSet` is provided, it must specify the `coord` and `labels` for all
+        dimensions of the `data`\ . Multiple `coord`\ 's can be specified in a
+        `CoordSet` instance for each dimension.
+    coordunits : `list`\ , optional, default: `None`
         A list of units corresponding to the dimensions in the order of the
         coordset.
-    coordtitles : list, optional
+    coordtitles : `list`\ , optional, default: `None`
         A list of titles corresponding of the dimensions in the order of the
         coordset.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Other Parameters
     ----------------
-    dtype : str or dtype, optional, default=np.float64
+    dtype : `str` or `~numpy.dtype`\ , optional, default: `np.float64`
         If specified, the data will be cast to this dtype, else the data
         will be cast to float64 or complex128.
-    dims : list of chars, optional
+    dims : `list` of `str`\ , optional
         If specified the list must have a length equal to the number od data
-        dimensions (ndim) and the chars
-        must be
-        taken among x,y,z,u,v,w or t. If not specified, the dimension
-        names are automatically attributed in
-        this order.
-    name : str, optional
+        dimensions (`ndim`) and the elements must be
+        taken among ``x,y,z,u,v,w or t``\ . If not specified, the dimension
+        names are automatically attributed in this order.
+    name : `str`\ , optional
         A user-friendly name for this object. If not given, the automatic
         `id` given at the object creation will be used as a name.
-    labels : array of objects, optional
-        Labels for the `data`. labels can be used only for 1D-datasets.
+    labels : :term:`array-like` of objects, optional
+        Labels for the `data`\ . labels can be used only for 1D-datasets.
         The labels array may have an additional dimension, meaning several
         series of labels for the same data.
-        The given array can be a list, a tuple, a |ndarray| , a ndarray-like,
-        a |NDArray| or any subclass of
-        |NDArray| .
-    mask : array of bool or `NOMASK`, optional
+        The given array can be a list, a tuple, a `~numpy.ndarray` , a ndarray-like,
+        a  `NDArray` or any subclass of `NDArray` .
+    mask : :term:`array-like` of `bool` or `NOMASK` , optional
         Mask for the data. The mask array must have the same shape as the
         data. The given array can be a list,
-        a tuple, or a |ndarray| . Each values in the array must be `False`
+        a tuple, or a `~numpy.ndarray` . Each values in the array must be `False`
         where the data are *valid* and True when
         they are not (like in numpy masked arrays). If `data` is already a
-        :class:`~numpy.ma.MaskedArray`, or any
-        array object (such as a |NDArray| or subclass of it), providing a
-        `mask` here, will causes the mask from the
+        :class:`~numpy.ma.MaskedArray` , or any
+        array object (such as a  `NDArray` or subclass of it), providing a
+        `mask` here, will cause the mask from the
         masked array to be ignored.
-    units : |Unit| instance or str, optional
-        Units of the data. If data is a |Quantity| then `units` is set to
-        the unit of the `data`; if a unit is also
+    units : `Unit` instance or `str`, optional
+        Units of the data. If data is a `Quantity` then `units` is set to
+        the unit of the `data`\ ; if a unit is also
         explicitly provided an error is raised. Handling of units use the
-        `pint <https://pint.readthedocs.org/>`_
+        `pint <https://pint.readthedocs.org/>`__
         package.
-    timezone : datetime.tzinfo, optional
+    timezone : `datetime.tzinfo`\ , optional
         The timezone where the data were created. If not specified, the local timezone
         is assumed.
-    title : str, optional
+    title : `str`\ , optional
         The title of the data dimension. The `title` attribute should not be confused
         with the `name` .
         The `title` attribute is used for instance for labelling plots of the data.
         It is optional but recommended to give a title to each ndarray data.
-    dlabel :  str, optional
-        Alias of `title`.
-    meta : dict-like object, optional
+    dlabel :  `str`\ , optional
+        Alias of `title` .
+    meta : `dict`\ -like object, optional
         Additional metadata for this object. Must be dict-like but no
         further restriction is placed on meta.
-    author : str, optional
-        Name(s) of the author(s) of this dataset. BNy default, name of the
+    author : `str`\ , optional
+        Name(s) of the author(s) of this dataset. By default, name of the
         computer note where this dataset is
         created.
-    description : str, optional
-        An optional description of the nd-dataset. A shorter alias is `desc`.
-    origin : str, optional
+    description : `str`\ , optional
+        An optional description of the nd-dataset. A shorter alias is `desc` .
+    origin : `str`\ , optional
         Origin of the data: Name of organization, address, telephone number,
         name of individual contributor, etc., as appropriate.
-    roi : list
+    roi : `list`
         Region of interest (ROI) limits.
-    history : str, optional
+    history : `str`\ , optional
         A string to add to the object history.
-    copy : bool, optional
+    copy : `bool`\ , optional
         Perform a copy of the passed object. Default is False.
 
     See Also
     --------
     Coord : Explicit coordinates object.
     LinearCoord : Implicit coordinates object.
     CoordSet : Set of coordinates.
 
     Notes
     -----
-    The underlying array in a |NDDataset| object can be accessed through the
-    `data` attribute, which will return a conventional |ndarray| .
+    The underlying array in a `NDDataset` object can be accessed through the
+    `data` attribute, which will return a conventional `~numpy.ndarray`\ .
     """
 
     # Examples
     # --------
     # Usage by an end-user
     #
     # >>> x = scp.NDDataset([1, 2, 3])
     # >>> print(x.data)  # doctest: +NORMALIZE_WHITESPACE
     # [       1        2        3.]
     # """
 
     # coordinates
-    _coordset = Instance(CoordSet, allow_none=True)
+    _coordset = tr.Instance(CoordSet, allow_none=True)
 
     # model data (e.g., for fit)
-    _modeldata = Array(Float(), allow_none=True)
+    _modeldata = Array(tr.Float(), allow_none=True)
 
     # some setting for NDDataset
-    _copy = Bool(False)
-    _labels_allowed = Bool(False)  # no labels for NDDataset
+    _copy = tr.Bool(False)
+    _labels_allowed = tr.Bool(False)  # no labels for NDDataset
 
     # dataset can be members of a project.
-    # we use the abstract class to avoid circular imports.
-    from spectrochempy.core.project.abstractproject import AbstractProject
-
-    _parent = Instance(AbstractProject, allow_none=True)
+    _parent = tr.Instance(
+        "spectrochempy.core.project.abstractproject.AbstractProject", allow_none=True
+    )
 
     # For the GUI interface
 
     # parameters state
     # _state = Dict()
 
     # processed data (for GUI)
@@ -225,26 +201,26 @@
     # reference data (for GUI)
     # _referencedata = Array(Float(), allow_none=True)
 
     # region ranges
     # _ranges = Instance(Meta)
 
     # history
-    _history = List(Tuple(), allow_none=True)
+    _history = tr.List(tr.Tuple(), allow_none=True)
 
     # Dates
     # _acquisition_date = Instance(datetime, allow_none=True)
-    _created = Instance(datetime)
-    _modified = Instance(datetime)
-    _timezone = Instance(tzinfo, allow_none=True)
+    _created = tr.Instance(datetime)
+    _modified = tr.Instance(datetime)
+    _timezone = tr.Instance(tzinfo, allow_none=True)
 
     # Metadata
-    _author = Unicode()
-    _description = Unicode()
-    _origin = Unicode()
+    _author = tr.Unicode()
+    _description = tr.Unicode()
+    _origin = tr.Unicode()
 
     # ----------------------------------------------------------------------------------
     # Initialisation
     # ----------------------------------------------------------------------------------
     def __init__(
         self, data=None, coordset=None, coordunits=None, coordtitles=None, **kwargs
     ):
@@ -286,20 +262,22 @@
                     if u is not None:
                         coord.units = u
                     if t is not None:
                         coord.title = t
                 else:
                     if u:  # pragma: no cover
                         warning_(
-                            "units have been set for a CoordSet, but this will be ignored "
+                            "units have been set for a CoordSet, "
+                            "but this will be ignored "
                             "(units are only defined at the coordinate level"
                         )
                     if t:  # pragma: no cover
                         warning_(
-                            "title will be ignored as they are only defined at the coordinates level"
+                            "title will be ignored as they are only defined at "
+                            "the coordinates level"
                         )
                     coord = c
 
                 _coordset.append(coord)
 
             if _coordset and set(_coordset) != {
                 Coord()
@@ -309,15 +287,16 @@
         self._modified = self._created
 
     # ----------------------------------------------------------------------------------
     # Special methods
     # ----------------------------------------------------------------------------------
     def __dir__(self):
         # Only these attributes are used for saving dataset
-        # WARNING: be careful to keep the present order of the three first elements! Needed for save/load operations
+        # WARNING: be careful to keep the present order of the three first elements!
+        # Needed for save/load operations
         return [
             # Keep the following order
             "dims",
             "coordset",
             "data",
             # From here it is free
             "name",
@@ -414,14 +393,16 @@
                 "_ax_lines",
                 "_axcb",
                 "clevels",
                 "__wrapped__",
                 "coords",
                 "__await__",
                 "__aiter__",
+                "__name__",
+                "__qualname__",
             ]
             or "_validate" in item
             or "_changed" in item
         ):
             # raise an error so that traits, ipython operation and more ... will be handled correctly
             raise AttributeError
 
@@ -469,15 +450,14 @@
                     )
 
             return None
 
         raise AttributeError
 
     def __setattr__(self, key, value):
-
         if key in DEFAULT_DIM_NAME:  # syntax such as ds.x, ds.y, etc...
             # Note the above test is important to avoid errors with traitlets
             # even if it looks redundant with the following
             if key in self.dims:
                 if self._coordset is None:
                     # we need to create a coordset first
                     self.set_coordset(
@@ -542,71 +522,71 @@
     def __hash__(self):
         # all instance of this class has same hash, so they can be compared
         return super().__hash__ + hash(self._coordset)
 
     # ----------------------------------------------------------------------------------
     # Private methods and properties
     # ----------------------------------------------------------------------------------
-    @default("_coordset")
+    @tr.default("_coordset")
     def _coordset_default(self):
         return None
 
-    @default("_modeldata")
+    @tr.default("_modeldata")
     def _modeldata_default(self):
         return None
 
-    # @default("_processeddata")
+    # @tr.default("_processeddata")
     # def _processeddata_default(self):
     #     return None
     #
-    # @default("_baselinedata")
+    # @tr.default("_baselinedata")
     # def _baselinedata_default(self):
     #     return None
     #
-    # @default("_referencedata")
+    # @tr.default("_referencedata")
     # def _referencedata_default(self):
     #     return None
     #
-    # @default("_ranges")
+    # @tr.default("_ranges")
     # def _ranges_default(self):
     #     ranges = Meta()
     #     for dim in self.dims:
     #         ranges[dim] = dict(masks={}, baselines={}, integrals={}, others={})
     #     return ranges
 
-    @default("_timezone")
+    @tr.default("_timezone")
     def _timezone_default(self):
         # Return the default timezone (UTC)
         return datetime.utcnow().astimezone().tzinfo
 
-    @validate("_created")
+    @tr.validate("_created")
     def _created_validate(self, proposal):
         date = proposal["value"]
         if date.tzinfo is not None:
             # make the date utc naive
             date = date.replace(tzinfo=None)
         return date
 
-    @validate("_history")
+    @tr.validate("_history")
     def _history_validate(self, proposal):
         history = proposal["value"]
         if isinstance(history, list) or history is None:
             # reset
             self._history = None
         return history
 
-    @validate("_modified")
+    @tr.validate("_modified")
     def _modified_validate(self, proposal):
         date = proposal["value"]
         if date.tzinfo is not None:
             # make the date utc naive
             date = date.replace(tzinfo=None)
         return date
 
-    @observe(All)
+    @tr.observe(tr.All)
     def _anytrait_changed(self, change):
 
         # ex: change {
         #   'owner': object, # The HasTraits instance
         #   'new': 6, # The new value
         #   'old': 5, # The old value
         #   'name': "foo", # The name of the changed trait
@@ -710,15 +690,15 @@
 
     _repr_dims = _str_dims
 
     def _dims_update(self, change=None):
         # when notified that a coords names have been updated
         _ = self.dims  # fire an update
 
-    @validate("_coordset")
+    @tr.validate("_coordset")
     def _coordset_validate(self, proposal):
         coords = proposal["value"]
         return self._valid_coordset(coords)
 
     def _valid_coordset(self, coords):
         # uses in coords_validate and setattr
         if coords is None:
@@ -829,15 +809,15 @@
             self._coordset = CoordSet(*coords, dims=dims, **kwargs)
         else:
             # add one coordinate
             self._coordset._append(*coords, **kwargs)
 
         if self._coordset:
             # set a notifier to the updated traits of the CoordSet instance
-            HasTraits.observe(self._coordset, self._dims_update, "_updated")
+            tr.HasTraits.observe(self._coordset, self._dims_update, "_updated")
             # force it one time after this initialization
             self._coordset._updated = True
 
     @property
     def author(self):
         """
         Creator of the dataset (str).
@@ -878,20 +858,20 @@
     def coord(self, dim="x"):
         """
         Return the coordinates along the given dimension.
 
         Parameters
         ----------
         dim : int or str
-            A dimension index or name, default index = `x`.
+            A dimension index or name, default index = `x` .
             If an integer is provided, it is equivalent to the `axis` parameter for numpy array.
 
         Returns
         -------
-        |Coord|
+         `Coord`
             Coordinates along the given axis.
         """
         idx = self._get_dims_index(dim)[0]  # should generate an error if the
         # dimension name is not recognized
         if idx is None:
             return None
 
@@ -907,15 +887,15 @@
         else:
             error_(f"could not find this dimenson name: `{name}`")
             return None
 
     @property
     def coordset(self):
         """
-        |CoordSet| instance.
+        `CoordSet` instance.
 
         Contains the coordinates of the various dimensions of the dataset.
         It's a readonly property. Use set_coords to change one or more coordinates at once.
         """
         if self._coordset and all(c.is_empty for c in self._coordset):
             # all coordinates are empty, this is equivalent to None for the coordset
             return None
@@ -927,35 +907,35 @@
             self.set_coordset(**coords)
         else:
             self.set_coordset(coords)
 
     @property
     def coordnames(self):
         """
-        List of the |Coord| names.
+        List of the  `Coord` names.
 
         Read only property.
         """
         if self._coordset is not None:
             return self._coordset.names
 
     @property
     def coordtitles(self):
         """
-        List of the |Coord| titles.
+        List of the  `Coord` titles.
 
         Read only property. Use set_coordtitle to eventually set titles.
         """
         if self._coordset is not None:
             return self._coordset.titles
 
     @property
     def coordunits(self):
         """
-        List of the |Coord| units.
+        List of the  `Coord` units.
 
         Read only property. Use set_coordunits to eventually set units.
         """
         if self._coordset is not None:
             return self._coordset.units
 
     @property
@@ -965,15 +945,15 @@
         """
         created = pytz.utc.localize(self._created)
         return created.astimezone(self.timezone).isoformat(sep=" ", timespec="seconds")
 
     @property
     def data(self):
         """
-        The ``data`` array.
+        The `data` array.
 
         If there is no data but labels, then the labels are returned instead of data.
         """
         return super().data
 
     @data.setter
     def data(self, data):
@@ -1009,15 +989,15 @@
         Return the local timezone.
         """
         return str(datetime.utcnow().astimezone().tzinfo)
 
     @property
     def modeldata(self):
         """
-        |ndarray| - models data.
+        `~numpy.ndarray` - models data.
 
         Data eventually generated by modelling of the data.
         """
         return self._modeldata
 
     @modeldata.setter
     def modeldata(self, data):
@@ -1043,15 +1023,15 @@
     @origin.setter
     def origin(self, value):
         self._origin = value
 
     @property
     def parent(self):
         """
-        |Project| instance.
+        `Project` instance.
 
         The parent project of the dataset.
         """
         return self._parent
 
     @parent.setter
     def parent(self, value):
@@ -1102,27 +1082,27 @@
         Parameters
         ----------
         dim : str or int, optional, default=-1
             Dimension index or name along which to sort.
         pos : int , optional
             If labels are multidimensional  - allow to sort on a define
             row of labels : labels[pos]. Experimental : Not yet checked.
-        by : str among ['value', 'label'], optional, default=``value``
+        by : str among ['value', 'label'], optional, default=`value`
             Indicate if the sorting is following the order of labels or
             numeric coord values.
-        descend : `bool`, optional, default=`False`
+        descend : `bool` , optional, default=`False`
             If true the dataset is sorted in a descending direction. Default is False  except if coordinates
             are reversed.
         inplace : bool, optional, default=`False`
             Flag to say that the method return a new object (default)
             or not (inplace=True).
 
         Returns
         -------
-        |NDDataset|
+        `NDDataset`
             Sorted dataset.
         """
 
         inplace = kwargs.get("inplace", False)
         if not inplace:
             new = self.copy()
         else:
@@ -1189,22 +1169,22 @@
             one, an error is raised.
         inplace : bool, optional, default=`False`
             Flag to say that the method return a new object (default)
             or not (inplace=True).
 
         Returns
         -------
-        |NDDataset|
+        `NDDataset`
             The input array, but with all or a subset of the
             dimensions of length 1 removed.
 
         Raises
         ------
         ValueError
-            If `dim` is not `None`, and the dimension being squeezed is not
+            If `dim` is not `None` , and the dimension being squeezed is not
             of length 1.
         """
         # make a copy of the original dims
         old = self.dims[:]
 
         # squeeze the data and determine which axis must be squeezed
         new, axis = super().squeeze(*dims, inplace=inplace, return_axis=True)
@@ -1228,15 +1208,15 @@
         Parameters
         ----------
         dim : int or str
             Position in the expanded axes where the new axis (or axes) is placed.
 
         Returns
         -------
-        |NDDataset|
+        `NDDataset`
             View of `a` with the number of dimensions increased.
 
         See Also
         --------
         squeeze : The inverse operation, removing singleton dimensions.
         """
         # TODO
@@ -1253,42 +1233,42 @@
             Second axis.
         inplace : bool, optional, default=`False`
             Flag to say that the method return a new object (default)
             or not (inplace=True).
 
         Returns
         -------
-        |NDDataset|
+        `NDDataset`
             Swaped dataset.
 
         See Also
         --------
         transpose : Transpose a dataset.
         """
 
         new = super().swapdims(dim1, dim2, inplace=inplace)
         new.history = f"Data swapped between dims {dim1} and {dim2}"
         return new
 
     @property
     def T(self):
         """
-        Transposed |NDDataset| .
+        Transposed `NDDataset` .
 
         The same object is returned if `ndim` is less than 2.
         """
         return self.transpose()
 
     def take(self, indices, **kwargs):
         """
         Take elements from an array.
 
         Returns
         -------
-        |NDDataset|
+        `NDDataset`
             A sub dataset defined by the input indices.
         """
 
         # handle the various syntax to pass the axis
         dims = self._get_dims_from_args(**kwargs)
         axis = self._get_dims_index(dims)
         axis = axis[0] if axis else None
@@ -1341,15 +1321,15 @@
         """
         Return a numpy masked array.
 
         Other NDDataset attributes are lost.
 
         Returns
         -------
-        |ndarray|
+        `~numpy.ndarray`
             The numpy masked array from the NDDataset data.
 
         Examples
         ========
 
         >>> dataset = scp.read('wodger.spg')
         >>> a = scp.to_array(dataset)
@@ -1390,28 +1370,28 @@
         # attrs: OrderedDict
         #     Dictionary for holding arbitrary metadata.
         # Init docstring
         #
         # Parameters
         # ----------
         # data: array_like
-        #     Values for this array. Must be an ``numpy.ndarray``, ndarray like,
-        #     or castable to an ``ndarray``.
+        #     Values for this array. Must be an `numpy.ndarray` , ndarray like,
+        #     or castable to an `~numpy.ndarray` .
         # coords: sequence or dict of array_like objects, optional
         #     Coordinates (tick labels) to use for indexing along each dimension.
         #     If dict-like, should be a mapping from dimension names to the
         #     corresponding coordinates. If sequence-like, should be a sequence
         #     of tuples where the first element is the dimension name and the
         #     second element is the corresponding coordinate array_like object.
         # dims: str or sequence of str, optional
         #     Name(s) of the data dimension(s). Must be either a string (only
         #     for 1D data) or a sequence of strings with length equal to the
         #     number of dimensions. If this argument is omitted, dimension names
-        #     are taken from ``coords`` (if possible) and otherwise default to
-        #     ``['dim_0', ... 'dim_n']``.
+        #     are taken from `coords` (if possible) and otherwise default to
+        #     `['dim_0', ... 'dim_n']` .
         # name: str or None, optional
         #     Name of this array.
         # attrs: dict_like or None, optional
         #     Attributes to assign to the new instance. By default, an empty
         #     attribute dictionary is initialized.
         # encoding: dict_like or None, optional
         #     Dictionary specifying how to encode this array's data into a
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/plotters/api.py` & `spectrochempy-0.6.1/spectrochempy/core/plotters/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/core/plotters/multiplot.py` & `spectrochempy-0.6.1/spectrochempy/core/plotters/multiplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,69 +37,69 @@
 # from spectrochempy.core import preferences, project_preferences
 
 
 def multiplot_scatter(datasets, **kwargs):
     """
     Plot a multiplot with 1D scatter type plots.
 
-    Alias of multiplot (with `method` argument set to ``scatter``.
+    Alias of multiplot (with `method` argument set to `scatter` .
     """
     kwargs["method"] = "scatter"
     return multiplot(datasets, **kwargs)
 
 
 def multiplot_lines(datasets, **kwargs):
     """
     Plot a multiplot with 1D linetype plots.
 
-    Alias of multiplot (with `method` argument set to ``lines``.
+    Alias of multiplot (with `method` argument set to `lines` .
     """
     kwargs["method"] = "lines"
     return multiplot(datasets, **kwargs)
 
 
 def multiplot_stack(datasets, **kwargs):
     """
     Plot a multiplot with 2D stack type plots.
 
-    Alias of multiplot (with `method` argument set to ``stack``.
+    Alias of multiplot (with `method` argument set to `stack` .
     """
     kwargs["method"] = "stack"
     return multiplot(datasets, **kwargs)
 
 
 def multiplot_map(datasets, **kwargs):
     """
     Plot a multiplot with 2D map type plots.
 
-    Alias of multiplot (with `method` argument set to ``map``.
+    Alias of multiplot (with `method` argument set to `map` .
     """
     kwargs["method"] = "map"
     return multiplot(datasets, **kwargs)
 
 
 def multiplot_image(datasets, **kwargs):
     """
     Plot a multiplot with 2D image type plots.
 
-    Alias of multiplot (with `method` argument set to ``image``.
+    Alias of multiplot (with `method` argument set to `image` .
     """
     kwargs["method"] = "image"
     return multiplot(datasets, **kwargs)
 
 
 # with transpose plot  -----------------------------------------------------------------
 
 
 def plot_with_transposed(dataset, **kwargs):
     """
     Plot a 2D dataset as a stacked plot with its transposition in a second
     axe.
 
-    Alias of plot_2D (with `method` argument set to ``with_transposed``).
+    Alias of plot_2D (with `method` argument set to `with_transposed` ).
     """
     kwargs["method"] = "with_transposed"
     axes = multiplot(dataset, **kwargs)
     return axes
 
 
 multiplot_with_transposed = plot_with_transposed
@@ -127,20 +127,20 @@
     ----------
     datasets : nddataset or list of nddataset
         Datasets to plot.
     labels : list of str
         The labels that will be used as title of each axes.
     method : str, default to `map` for 2D and `lines` for 1D data
         Type of plot to draw in all axes (`lines` , `scatter` , `stack` , `map`
-        ,`image` or `with_transposed`).
+        ,`image` or `with_transposed` ).
     nrows, ncols : int, default=1
         Number of rows/cols of the subplot grid. ncol*nrow must be equal
         to the number of datasets to plot.
     sharex, sharey : bool or {'none', 'all', 'row', 'col'}, default=False
-        Controls sharing of properties among x (`sharex`) or y (`sharey`)
+        Controls sharing of properties among x (`sharex` ) or y (`sharey` )
         axes::
 
         - True or 'all' : x- or y-axis will be shared among all subplots.
         - False or 'none' : each subplot x- or y-axis will be independent.
         - 'row' : each subplot row will share an x- or y-axis.
         - 'col' : each subplot column will share an x- or y-axis.
 
@@ -149,21 +149,21 @@
         subplots have a shared y-axis along a row, only the y tick labels
         of the first column subplot are visible.
     sharez : bool or {'none', 'all', 'row', 'col'}, default=False
         Equivalent to sharey for 1D plot.
         for 2D plot, z is the intensity axis (i.e., contour levels for maps or
         the vertical axis for stack plot), y is the third axis.
     figsize : 2-tuple of floats
-        ``(width, height)`` tuple in inches.
+        `(width, height)` tuple in inches.
     dpi : float
         Dots per inch
     facecolor : color
-        The figure patch facecolor; defaults to rc ``figure.facecolor``.
+        The figure patch facecolor; defaults to rc `figure.facecolor` .
     edgecolor : color
-        The figure patch edge color; defaults to rc ``figure.edgecolor``.
+        The figure patch edge color; defaults to rc `figure.edgecolor` .
     linewidth : float
         The figure patch edge linewidth; the default linewidth of the frame.
     frameon : bool
         If `False` , suppress drawing the figure frame.
     left : float in the [0-1] interval
         The left side of the subplots of the figure.
     right : float in the [0-1] interval
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/plotters/plot1d.py` & `spectrochempy-0.6.1/spectrochempy/core/plotters/plot1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 ax : Axe, optional
     Axe where to plot. If not specified, create a new one.
 style : str, optional, default: `dataset.preferences.style` (scpy)
     Matplotlib stylesheet (use `available_style` to get a list of available
     styles for plotting.
 use_plotly : bool, optional, default: `preferences.use_plotly` (False)
     Should we use plotly instead of matplotlib for plotting.
-twinx : :class:`~matplotlib.Axes` instance, optional, default: None
+twinx : :class:`~matplotlib.axes.Axes` instance, optional, default: None
     If this is not None, then a twin axes will be created with a
     common x dimension.
 clear : bool, optional, default: True
     If false, hold the current figure and ax until a new plot is performed.
 reverse : bool or None [optional, default=None/False
     In principle, coordinates run from left to right,
     except for wavenumbers
@@ -107,42 +107,42 @@
 
 
 @plot_method("1D", _PLOT1D_DOC)
 def plot_scatter(dataset, **kwargs):
     """
     Plot a 1D dataset as a scatter plot (points can be added on lines).
 
-    Alias of plot (with `method` argument set to ``scatter``.
+    Alias of plot (with `method` argument set to `scatter` .
     """
 
 
 @plot_method("1D", _PLOT1D_DOC)
 def plot_pen(dataset, **kwargs):
     """
     Plot a 1D dataset with solid pen by default.
 
-    Alias of plot (with `method` argument set to ``pen``.
+    Alias of plot (with `method` argument set to `pen` .
     """
 
 
 @plot_method("1D", _PLOT1D_DOC)
 def plot_scatter_pen(dataset, **kwargs):
     """
     Plot a 1D dataset with solid pen by default.
 
-    Alias of plot (with `method` argument set to ``scatter_pen``.
+    Alias of plot (with `method` argument set to `scatter_pen` .
     """
 
 
 @plot_method("1D", _PLOT1D_DOC)
 def plot_bar(dataset, **kwargs):
     """
     Plot a 1D dataset with bars.
 
-    Alias of plot (with `method` argument set to ``bar``.
+    Alias of plot (with `method` argument set to `bar` .
     """
 
 
 def plot_multiple(datasets, method="scatter", pen=True, labels=None, **kwargs):
     """
     Plot a series of 1D datasets as a scatter plot with optional lines between markers.
 
@@ -245,20 +245,20 @@
     Plot of one-dimensional data.
 
     Parameters
     ----------
     dataset : :class:`~spectrochempy.ddataset.nddataset.NDDataset`
         Source of data to plot.
     method : str, optional, default: dataset.preference.method_1D
-        The method can be one among ``pen``, ``bar``, ``scatter`` or ``scatter+pen``.
-        Default values is ``pen``, i.e., solid lines are drawn. This default can be changed
-        using ``dataset.preference.method_1D``.
-        To draw a Bar graph, use method ``bar``.
-        For a Scatter plot, use method ``scatter``.
-        For pen and scatter simultaneously, use method ``scatter+pen``.
+        The method can be one among `pen` , `bar` , `scatter` or `scatter+pen` .
+        Default values is `pen` , i.e., solid lines are drawn. This default can be changed
+        using `dataset.preference.method_1D` .
+        To draw a Bar graph, use method `bar` .
+        For a Scatter plot, use method `scatter` .
+        For pen and scatter simultaneously, use method `scatter+pen` .
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Other Parameters
     ----------------
     {0}
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/plotters/plot2d.py` & `spectrochempy-0.6.1/spectrochempy/core/plotters/plot2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 clear : bool, optional, default=`True`
     Should we plot on the ax previously used or create a new figure?.
 figsize : tuple, optional
     The figure size expressed as a tuple (w,h) in inch.
 fontsize : int, optional
     The font size in pixels, default is 10 (or read from preferences).
 style : str
-autolayout : `bool`, optional, default=True
+autolayout : `bool` , optional, default=True
     if True, layout will be set automatically.
 output : str
     A string containing a path to a filename. The output format is deduced
     from the extension of the filename. If the filename has no extension,
     the value of the rc parameter savefig.format is used.
 dpi : [ None | scalar > 0]
     The resolution in dots per inch. If None it will default to the
@@ -52,15 +52,15 @@
 ax :
 twinx :
 use_plotly : bool, optional
     Should we use plotly instead of mpl for plotting. Default to `preferences.use_plotly`  (default=False)
 data_only : `bool` [optional, default=`False`]
     Only the plot is done. No addition of axes or label specifications
     (current if any or automatic settings are kept.
-method : str [optional among ``map``, ``stack``, ``image`` or ``3D``]
+method : str [optional among `map` , `stack` , `image` or `3D`]
     The type of plot,
 projections : `bool` [optional, default=False]
 style : str, optional, default='notebook'
     Matplotlib stylesheet (use `available_style` to get a list of available
     styles for plotting
 reverse : `bool` or None [optional, default=None
     In principle, coordinates run from left to right, except for wavenumbers
@@ -75,49 +75,49 @@
 # nddataset plot2D functions
 # ======================================================================================
 @plot_method("2D", _PLOT2D_DOC)
 def plot_stack(dataset, **kwargs):
     """
     Plot a 2D dataset as a stack plot.
 
-    Alias of plot_2D (with `method` argument set to ``stack``).
+    Alias of plot_2D (with `method` argument set to `stack` ).
     """
 
 
 @plot_method("2D", _PLOT2D_DOC)
 def plot_map(dataset, **kwargs):
     """
     Plot a 2D dataset as a contoured map.
 
-    Alias of plot_2D (with `method` argument set to ``map``.
+    Alias of plot_2D (with `method` argument set to `map` .
     """
 
 
 @plot_method("2D", _PLOT2D_DOC)
 def plot_image(dataset, **kwargs):
     """
     Plot a 2D dataset as an image plot.
 
-    Alias of plot_2D (with `method` argument set to ``image``).
+    Alias of plot_2D (with `method` argument set to `image` ).
     """
 
 
 @add_docstring(_PLOT2D_DOC)
 def plot_2D(dataset, method=None, **kwargs):
     """
     Plot of 2D array.
 
     Parameters
     ----------
-    dataset : |NDDataset|
+    dataset : `NDDataset`
         The dataset to plot.
     method : ['stack', 'map', 'image'] , optional
         The method of plot of the dataset, which will determine the plotter to use.
         Default method is given 'stack' but this can be changed using
-        ``dataset.preference.method_2D``.
+        `dataset.preference.method_2D` .
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Other Parameters
     ----------------
     {0}
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/plotters/plot3d.py` & `spectrochempy-0.6.1/spectrochempy/core/plotters/plot3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 _PLOT3D_DOC = """
 ax : |Axes| instance. Optional
     The axe where to plot. The default is the current axe or to create a new one if is None.
 figsize : tuple, optional
     The figure size expressed as a tuple (w,h) in inch.
 fontsize : int, optional
     The font size in pixels, default is 10 (or read from preferences).
-autolayout : `bool`, optional, default=True
+autolayout : `bool` , optional, default=True
     if True, layout will be set automatically.
 dpi : [ None | scalar > 0]
     The resolution in dots per inch. If None it will default to the
     value savefig.dpi in the matplotlibrc file.
 colorbar :
-method : str [optional among ``surface``, ``waterfall``, ...]
+method : str [optional among `surface` , `waterfall` , ...]
     The type of plot,
 style : str, optional, default='notebook'
     Matplotlib stylesheet (use `available_style` to get a list of available
     styles for plotting
 reverse : `bool` or None [optional, default=None
     In principle, coordinates run from left to right, except for wavenumbers
     (e.g., FTIR spectra) or ppm (e.g., NMR), that spectrochempy
@@ -47,37 +47,37 @@
 # nddataset plot3D functions
 # ======================================================================================
 @plot_method("2D", _PLOT3D_DOC)
 def plot_surface(dataset, **kwargs):
     """
     Plot a 2D dataset as a a 3D-surface.
 
-    Alias of plot_3D (with `method` argument set to ``surface``).
+    Alias of plot_3D (with `method` argument set to `surface` ).
     """
     return
 
 
 @plot_method("2D", _PLOT3D_DOC)
 def plot_waterfall(dataset, **kwargs):
     """
     Plot a 2D dataset as a a 3D-waterfall plot.
 
-    Alias of plot_2D (with `method` argument set to ``waterfall``).
+    Alias of plot_2D (with `method` argument set to `waterfall` ).
     """
     return
 
 
 @add_docstring(_PLOT3D_DOC)
 def plot_3D(dataset, method="surface", **kwargs):
     """
     Plot of 2D array as 3D plot
 
     Parameters
     ----------
-    dataset : |NDDataset|
+    dataset : `NDDataset`
         The dataset to plot.
     method : ['surface', 'waterfall'] , optional
         The method of plot of the dataset, which will determine the plotter to use. Default is stack.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Other Parameters
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/plotters/plotly.py` & `spectrochempy-0.6.1/spectrochempy/core/plotters/plotly.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,65 +24,65 @@
 #
 # # contour map (default) -------------------------------------------------------
 #
 # def plotly_map(dataset, **kwargs):
 #     """
 #     Plot a 2D dataset as a contoured map.
 #
-#     Alias of plot_2D (with `method` argument set to ``map``.
+#     Alias of plot_2D (with `method` argument set to `map` .
 #     """
 #     kwargs['method'] = 'map'
 #     return plotly(dataset, **kwargs)
 #
 #
 # # stack plot  -----------------------------------------------------------------
 #
 # def plotly_stack(dataset, **kwargs):
 #     """
 #     Plot a 2D dataset as a stacked plot.
 #
-#     Alias of plot_2D (with `method` argument set to ``stack``).
+#     Alias of plot_2D (with `method` argument set to `stack` ).
 #     """
 #     kwargs['method'] = 'stack'
 #     return plotly(dataset, **kwargs)
 #
 #
 # # image plot --------------------------------------------------------
 #
 # def plotly_image(dataset, **kwargs):
 #     """
 #     Plot a 2D dataset as an image plot.
 #
-#     Alias of plot_2D (with `method` argument set to ``image``).
+#     Alias of plot_2D (with `method` argument set to `image` ).
 #     """
 #     kwargs['method'] = 'image'
 #     return plotly(dataset, **kwargs)
 #
 #
 # # surface plot -----------------------------------------------------------------
 #
 # def plotly_surface(dataset, **kwargs):
 #     """
 #     Plot a 2D dataset as a a 3D-surface.
 #
-#     Alias of plot_2D (with `method` argument set to ``surface``.
+#     Alias of plot_2D (with `method` argument set to `surface` .
 #     """
 #     kwargs['method'] = 'surface'
 #     return plotly(dataset, **kwargs)
 #
 #
 # # generic plot (default stack plot) -------------------------------------------
 #
 # def plotly(dataset, **kwargs):
 #     """
 #     Generate a Plotly plot
 #
 #     Parameters
 #     ----------
-#     dataset; |NDDataset|
+#     dataset; `NDDataset`
 #         The dataset to plot
 #     kwargs: any
 #         Additional keyword arguments
 #
 #     Returns
 #     -------
 #     figure
@@ -482,15 +482,15 @@
 #             (x2 - x1) * (x2 - x1) + (y2 - y1) * (y2 - y1))
 #
 #
 # def calc_distances(p, start=None, end=None):
 #     """
 #     Parameters
 #     ----------
-#     p : |NDDataset|
+#     p : `NDDataset`
 #     """
 #     dimx = p.dims[-1]
 #     x = getattr(p, dimx).data
 #     z = p.data
 #     # ny = z.shape[0]
 #     if start is None:
 #         start = 0
@@ -532,15 +532,15 @@
 #
 #
 # def _compress(ds, optimisation=None):
 #     """
 #     reduce the number of spectra to display
 #     Parameters
 #     ----------
-#     ds: |NDDataset|
+#     ds: `NDDataset`
 #         The dataset to simplify
 #
 #     Returns
 #     -------
 #     a list a (x,y) traces
 #     """
 #     sizey, sizex = ds.shape
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/processors/align.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/align.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 def can_merge_or_align(coord1, coord2):
     """
     Check if two coordinates can be merged or aligned.
 
     Parameters
     ----------
-    coord1, coord2 : |Coord|
+    coord1, coord2 :  `Coord`
         Coordinates to merge or align.
 
     Returns
     -------
     can_merge, can_align : tuple of bools
         Two flags about merge and alignment possibility.
     """
@@ -56,60 +56,63 @@
                 can_align &= coord2.is_units_compatible(coord1)
 
     return can_merge, can_align
 
 
 def align(dataset, *others, **kwargs):
     """
-    Align individual |NDDataset| along given dimensions using various methods.
+    Align individual `NDDataset` along given dimensions using various methods.
 
     Parameters
     -----------
-    dataset : |NDDataset|
-        Dataset on which we want to salign other objects.
-    *others : |NDDataset|
+    dataset : `NDDataset`
+        Dataset on which we want to align other objects.
+    \*others : `NDDataset`
         Objects to align.
     dim : str. Optional, default='x'
         Along which axis to perform the alignment.
     dims : list of str, optional, default=None
         Align along all dims defined in dims (if dim is also
         defined, then dims have higher priority).
     method : enum ['outer', 'inner', 'first', 'last', 'interpolate'], optional, default='outer'
         Which method to use for the alignment.
 
         If align is defined :
 
         * 'outer' means that a union of the different coordinates is
-        achieved (missing values are masked).
+          achieved (missing values are masked).
         * 'inner' means that the intersection of the coordinates is used.
         * 'first' means that the first dataset is used as reference.
         * 'last' means that the last dataset is used as reference.
         * 'interpolate' means that interpolation is performed relative to
-        the first dataset.
+          the first dataset.
+
     interpolate_method : enum ['linear','pchip']. Optional, default='linear'
         Method of interpolation to performs for the alignment.
     interpolate_sampling : 'auto', int or float. Optional, default='auto'
+        Values:
 
         * 'auto' : sampling is determined automatically from the existing data.
         * int :  if an integer values is specified, then the
           sampling interval for the interpolated data will be split in
           this number of points.
         * float : If a float value is provided, it determines the interval
-        between the interpolated data.
-    coord : |Coord| , optional, default=None
+          between the interpolated data.
+
+    coord :  `Coord` , optional, default=None
         Coordinates to use for alignment. Ignore those corresponding to the
         dimensions to align.
     copy : bool, optional, default=True
         If False then the returned objects will share memory with the
         original objects, whenever it is possible :
         in principle only if reindexing is not necessary.
 
     Returns
     --------
-    aligned_datasets : tuple of |NDDataset|
+    tuple of `NDDataset`
         Same objects as datasets with dimensions aligned.
 
     Raises
     ------
     ValueError
         Issued when the dimensions given in `dim` or `dims` argument are not
         compatibles (units, titles, etc.).
@@ -242,15 +245,15 @@
 
             new_coord_data = set(np.around(new_coord.data, ndec))
             coord_data = set(np.around(coord.data, ndec))
 
             if method in ["outer", "interpolate"]:
                 # in this case we do a union of the coords (masking the
                 # missing values)
-                # For method=`interpolate`, the interpolation will be
+                # For method=`interpolate` , the interpolation will be
                 # performed in a second step
                 new_coord._data = sorted(coord_data | new_coord_data)
 
             elif method == "inner":
                 # take only intersection of the coordinates
                 # and generate a warning if it result something null or
                 new_coord._data = sorted(coord_data & new_coord_data)
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/processors/api.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/core/processors/apodization.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/apodization.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,18 +176,18 @@
         e = \pi * lb
 
 
     Parameters
     ----------
     dataset : Dataset
         Input dataset.
-    lb : float or |Quantity| , optional, default=1 Hz
+    lb : float or `Quantity` , optional, default=1 Hz
         Exponential line broadening,
         If it is not a quantity with units, it is assumed to be a broadening expressed in Hz.
-    shifted : float or `quantity`, optional, default=0 us
+    shifted : float or `quantity` , optional, default=0 us
         Shift the data time origin by this amount. If it is not a quantity
         it is assumed to be expressed in the data units of the last
         dimension.
 
     Returns
     -------
     apodized
@@ -252,23 +252,23 @@
     .. math::
         g = 0.6 * \pi * gb * (t - t0)
 
     Parameters
     ----------
     dataset : ndarray
         Dataset we want to apodize using an Lorentz Multiplication.
-    lb : float or `quantity`, optional, default=0 Hz
+    lb : float or `quantity` , optional, default=0 Hz
         Inverse exponential width.
         If it is not a quantity with units,
         it is assumed to be a broadening expressed in Hz.
-    gb : float or `quantity`, optional, default=1 Hz
+    gb : float or `quantity` , optional, default=1 Hz
         Gaussian broadening width.
         If it is not a quantity with units,
         it is assumed to be a broadening expressed in Hz.
-    shifted : float or `quantity`, optional, default=0 us
+    shifted : float or `quantity` , optional, default=0 us
         Shift the data time origin by this amount. If it is not a quantity
         it is assumed to be expressed in the data units of the last
         dimension.
 
     Returns
     -------
     apodized
@@ -344,15 +344,15 @@
     ----------
     dataset : Dataset
         Dataset we want to apodize using Sine Bell or Squared Sine Bell window multiplication.
     sbb : int or float, optional, default=1
         This processing parameter mimics the behaviour of the SSB parameter on bruker TOPSPIN software:
         Typical values are 1 for a pure sine function and 2 for a pure cosine function.
         Values greater than 2 give a mixed sine/cosine function. Note that all values smaller than 2, for example 0,
-        have the same effect as :math:`\text{ssb}=1`, namely a pure sine function.
+        have the same effect as :math:`\text{ssb}=1` , namely a pure sine function.
     pow : enum [1,2], optional, default=1
         Exponent value - If pow=2 a Squared Sine Bell window multiplication is performed.
 
     Returns
     -------
     apodized
         Dataset.
@@ -394,37 +394,52 @@
     else:
         phi = np.pi / ssb
     return np.sin((np.pi - phi) * t + phi) ** pow
 
 
 def sine(dataset, *args, **kwargs):
     """
-    Strictly equivalent to :meth:`sp`.
+    Strictly equivalent to :meth:`sp` .
+
+    Returns
+    -------
+    `NDDataset`
+        Modified dataset.
 
     See Also
     --------
     em, gm, sp, sinm, qsin, hamming, triang, bartlett, blackmanharris
     """
     return sp(dataset, *args, **kwargs)
 
 
 def sinm(dataset, ssb=1, **kwargs):
     """
-    Equivalent to :meth:`sp`, with pow = 1 (sine bell apodization window).
+    Equivalent to :meth:`sp` , with pow = 1 (sine bell apodization window).
+
+    Returns
+    -------
+    `NDDataset`
+        Modified dataset.
+
+    Returns
+    -------
+    `NDDataset`
+        Modified dataset.
 
     See Also
     --------
     em, gm, sp, sine, qsin, hamming, triang, bartlett, blackmanharris
     """
     return sp(dataset, ssb=ssb, pow=1, **kwargs)
 
 
 def qsin(dataset, ssb=1, **kwargs):
     """
-    Equivalent to :meth:`sp`, with pow = 2 (squared sine bell apodization window).
+    Equivalent to :meth:`sp` , with pow = 2 (squared sine bell apodization window).
 
     See Also
     --------
     em, gm, sp, sine, sinm, hamming, triang, bartlett, blackmanharris
     """
     return sp(dataset, ssb=ssb, pow=2, **kwargs)
 
@@ -559,15 +574,16 @@
     .. math::
        w(n) = \alpha - (1 - \alpha) \cos(\frac{2\pi{n}}{M-1}) \qquad 0 \leq n \leq M-1
 
     where M is the number of point of the input dataset and :math:`\alpha` = 0.5
 
     Parameters
     ----------
-    dataset : array.
+    dataset : `NDDataset`
+        Input dataset.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     -------
     apodized
         Dataset.
@@ -612,15 +628,15 @@
         Input dataset.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     -------
     apodized
-        Dataset
+        Dataset.
     apod_arr
         The apodization array only if 'retapod' is True.
 
     Other Parameters
     ----------------
     dim : str or int, keyword parameter, optional, default='x'.
         Specify on which dimension to apply the apodization method. If `dim` is specified as an integer it is equivalent
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/processors/autosub.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/autosub.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,41 +26,41 @@
     The subtraction coefficient are adjusted to either
     minimise the variance of the subtraction (method = 'vardiff') which will
     minimize peaks due to ref or minimize the sum of squares of the subtraction
     (method = 'ssdiff').
 
     Parameters
     ----------
-    dataset : |NDDataset|
+    dataset : `NDDataset`
         Dataset to which we want to subtract the reference data.
-    ref : |NDDataset|
+    ref : `NDDataset`
          1D reference data, with a size matching the axis to subtract.
          (axis parameter).  # TODO : optionally use title of axis.
-    *ranges : pair(s) of values
+    \*ranges : pair(s) of values
         Any number of pairs is allowed.
         Coord range(s) in which the variance is minimized.
-    dim : `str` or `int`, optional, default='x'
+    dim : `str` or `int` , optional, default='x'
         Tells on which dimension to perform the subtraction.
         If dim is an integer it refers to the axis index.
     method : str, optional, default='vardiff'
         'vardiff': minimize the difference of the variance.
         'ssdiff': minimize the sum of squares difference of sum of squares.
-    return_coefs : `bool`, optional, default=`False`
+    return_coefs : `bool` , optional, default=`False`
          Returns the table of coefficients.
-    inplace : `bool`, optional, default=`False`
+    inplace : `bool` , optional, default=`False`
         True if the subtraction is done in place.
         In this case we do not need to catch the function output.
 
     Returns
     --------
-    out : |NDDataset|
+    out : `NDDataset`
         The subtracted dataset.
-    coefs : `ndarray`.
+    coefs : `~numpy.ndarray` .
         The table of subtraction coefficients
-        (only if `return_coefs` is set to `True`).
+        (only if `return_coefs` is set to `True` ).
 
     See Also
     --------
     BaselineCorrection : Manual baseline corrections.
     abc : Automatic baseline corrections.
 
     Examples
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/processors/baseline.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/importer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,853 +1,769 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
-This module implements the `BaselineCorrection` class for baseline corrections.
+This module define a generic class to import directories, files and contents.
 """
-__all__ = ["BaselineCorrection", "ab", "abc", "dc", "basc"]
+__all__ = ["read", "read_dir", "read_remote"]
+__dataset_methods__ = __all__
 
-__dataset_methods__ = ["ab", "abc", "dc", "basc"]
+from io import BytesIO
+from warnings import warn
+from zipfile import ZipFile
+
+import requests
+import yaml
+from traitlets import Dict, HasTraits, List, Type, Unicode
+
+from spectrochempy.core import info_, warning_
+from spectrochempy.utils.exceptions import DimensionsCompatibilityError, ProtocolError
+from spectrochempy.utils.file import (
+    check_filename_to_open,
+    get_directory_name,
+    get_filenames,
+    pathclean,
+)
+
+FILETYPES = [
+    ("scp", "SpectroChemPy files (*.scp)"),
+    ("omnic", "Nicolet OMNIC files and series (*.spa *.spg *.srs)"),
+    ("soc", "Surface Optics Corp. (*.ddr *.hdr *.sdr)"),
+    ("labspec", "LABSPEC exported files (*.txt)"),
+    ("opus", "Bruker OPUS files (*.[0-9]*)"),
+    (
+        "topspin",
+        "Bruker TOPSPIN fid or series or processed data files (fid ser 1[r|i] 2[r|i]* 3[r|i]*)",
+    ),
+    ("matlab", "MATLAB files (*.mat)"),
+    ("dso", "Data Set Object files (*.dso)"),
+    ("jcamp", "JCAMP-DX files (*.jdx *.dx)"),
+    ("csv", "CSV files (*.csv)"),
+    ("excel", "Microsoft Excel files (*.xls)"),
+    ("zip", "Compressed folder of data files (*.zip)"),
+    ("quadera", "Quadera ascii files (*.asc)"),
+    ("carroucell", "Carroucell files (*spa)"),
+    ("galactic", "GRAMS/Thermo Galactic files (*.spc)")
+    #  ('all', 'All files (*.*)')
+]
+ALIAS = [
+    ("spg", "omnic"),
+    ("spa", "omnic"),
+    ("ddr", "soc"),
+    ("hdr", "soc"),
+    ("sdr", "soc"),
+    ("spc", "galactic"),
+    ("srs", "omnic"),
+    ("mat", "matlab"),
+    ("txt", "labspec"),
+    ("jdx", "jcamp"),
+    ("dx", "jcamp"),
+    ("xls", "excel"),
+    ("asc", "quadera"),
+]
+
+
+# --------------------------------------------------------------------------------------
+class Importer(HasTraits):
+    # Private _Importer class
+
+    objtype = Type()
+    datasets = List()
+    files = Dict()
+    default_key = Unicode()
+    protocol = Unicode()
+
+    protocols = Dict()
+    filetypes = Dict()
+
+    def __init__(self):
+
+        super().__init__()
+
+        self.filetypes = dict(FILETYPES)
+        temp = list(zip(*FILETYPES))
+        temp.reverse()
+        self.protocols = dict(zip(*temp))
+
+        #  add alias
+
+        self.alias = dict(ALIAS)
+
+    def __call__(self, *args, **kwargs):
+
+        self.datasets = []
+        self.default_key = kwargs.pop("default_key", ".scp")
+
+        if "merge" not in kwargs.keys():
+            # if merge is not specified, but the args are provided as a single list, then will are supposed to merge
+            # the datasets. If merge is specified then it has priority.
+            # This is not useful for the 1D datasets, as if they are compatible they are merged automatically
+            if args and len(args) == 1 and isinstance(args[0], (list, tuple)):
+                kwargs["merge"] = True
+
+        args, kwargs = self._setup_objtype(*args, **kwargs)
+        res = check_filename_to_open(*args, **kwargs)
+        if res:
+            # Normal return
+            self.files = res
+        else:
+            # Cancel in dialog!
+            return None
 
-import matplotlib.pyplot as plt
-import numpy as np
-import scipy.interpolate
-from matplotlib.widgets import SpanSelector
-from traitlets import Float, HasTraits, Int, List, Tuple, Unicode
-
-from spectrochempy.core import debug_, warning_
-from spectrochempy.core.plotters.multiplot import multiplot
-from spectrochempy.core.processors.smooth import smooth
-from spectrochempy.core.processors.utils import _units_agnostic_method
-from spectrochempy.utils.coordrange import trim_ranges
-from spectrochempy.utils.misc import TYPE_FLOAT, TYPE_INTEGER
-from spectrochempy.utils.traits import NDDatasetType
+        for key in self.files.keys():
 
+            if key == "" and kwargs.get("protocol") == ["carroucell"]:
+                key = ".carroucell"
+                self.files = {".carroucell": self.files[""]}
+
+            if key == "frombytes":
+                # here we need to read contents
+                for filename, content in self.files[key].items():
+                    files_ = check_filename_to_open(filename)
+                    kwargs["content"] = content
+                    key_ = list(files_.keys())[0]
+                    self._switch_protocol(key_, files_, **kwargs)
+                if len(self.datasets) > 1:
+                    self.datasets = self._do_merge(self.datasets, **kwargs)
 
-class BaselineCorrection(HasTraits):
-    """
-    Baseline Correction processor.
+            elif key and key[1:] not in list(zip(*FILETYPES))[0] + list(zip(*ALIAS))[0]:
+                raise TypeError(f"Filetype `{key}` is unknown in spectrochempy")
+            else:
+                # here files are read / or remotely from the disk using filenames
+                self._switch_protocol(key, self.files, **kwargs)
 
-    2 methods are proposed :
+        # now we will reset preference for this newly loaded datasets
+        if len(self.datasets) > 0:
 
-    * ``sequential`` (default) = classical polynom fit or spline
-      interpolation with separate fitting of each row (spectrum)
-    * ``multivariate`` = SVD modeling of baseline, polynomial fit of PC's
-      and calculation of the modelled baseline spectra.
+            if all(self.datasets) is None:
+                return None
 
-    Interactive mode is proposed using the interactive function : :meth:`run`.
+            prefs = self.datasets[0].preferences
+            try:
+                prefs.reset()
+            except (FileNotFoundError, AttributeError):
+                pass
+        else:
+            return None
 
-    Parameters
-    ----------
-    dataset : |NDDataset|
-        The dataset to be transformed.
+        if len(self.datasets) == 1:
+            nd = self.datasets[0]  # a single dataset is returned
+            name = kwargs.pop("name", None)
+            if name:
+                nd.name = name
+            return nd
 
-    See Also
-    --------
-    abc : Automatic baseline correction.
+        else:
+            nds = self.datasets
+            names = kwargs.pop("names", None)
+            if names and len(names) == len(nds):
+                for nd, name in zip(nds, names):
+                    nd.name = name
+            elif names and len(names) != len(nds):
+                warn(
+                    "length of the `names` list and of the list of datasets mismatch - names not applied"
+                )
+            return sorted(
+                nds, key=str
+            )  # return a sorted list (sorted according to their string representation)
+
+    def _setup_objtype(self, *args, **kwargs):
+        # check if the first argument is an instance of NDDataset or Project
+
+        args = list(args)
+        if (
+            args
+            and hasattr(args[0], "_implements")
+            and args[0]._implements() in ["NDDataset"]
+        ):
+            # the first arg is an instance of NDDataset
+            object = args.pop(0)
+            self.objtype = type(object)
 
-    Examples
-    --------
-    .. plot::
-        :include-source:
+        else:
+            # by default returned objtype is NDDataset (import here to avoid circular import)
+            from spectrochempy.core.dataset.nddataset import NDDataset
 
-        from spectrochempy import *
-        nd = NDDataset.read_omnic('irdata/nh4y-activation.spg')
-        ndp = nd[:, 1291.0:5999.0]
-        bc = BaselineCorrection(ndp)
-        ranges=[[5996., 5998.], [1290., 1300.],
-                [2205., 2301.], [5380., 5979.],
-                [3736., 5125.]]
-        span = bc.compute(*ranges,method='multivariate',
-                          interpolation='pchip', npc=8)
-        _ = bc.corrected.plot_stack()
-        show()
-    """
+            self.objtype = kwargs.pop("objtype", NDDataset)
 
-    dataset = NDDatasetType()
-    corrected = NDDatasetType()
-    method = Unicode("sequential")
-    interpolation = Unicode("polynomial")
-    axis = Int(-1)
-    dim = Unicode("")
-    ranges = List(List(minlen=2, maxlen=2))
-    order = Int(1, min=1, allow_none=True)
-    npc = Int(5, min=1, allow_none=True)
-    zoompreview = Float(1.0)
-    figsize = Tuple((7, 5))
-    sps = List()
-
-    def __init__(self, dataset, *args, **kwargs):
-        self.dataset = dataset
-        self.corrected = self.dataset.copy()
-        if args or kwargs:
-            warning_(
-                "DEPRECATION WARNING: Pass all arguments such range, and method definition in the "
-                "``compute`` method, not during the initialisation of the BaselineCorrection instance.\n"
-                "Here they are ignored."
-            )
-
-    def _extendranges(self, *ranges, **kwargs):
-        if not ranges:
-            # look in the kwargs
-            ranges = kwargs.pop("ranges", ())
-        if isinstance(ranges, tuple) and len(ranges) == 1:
-            ranges = ranges[0]  # probably passed with no start to the compute function
-        if not isinstance(ranges, (list, tuple)):
-            ranges = list(ranges)
-        if not ranges:
-            return
-
-        if len(ranges) == 2:
-            if isinstance(ranges[0], TYPE_INTEGER + TYPE_FLOAT) and isinstance(
-                ranges[1], TYPE_INTEGER + TYPE_FLOAT
-            ):
-                # a pair a values, we interpret this as a single range
-                ranges = [[ranges[0], ranges[1]]]
-        # find the single values
-        for item in ranges:
-            if isinstance(item, TYPE_INTEGER + TYPE_FLOAT):
-                # a single numerical value: interpret this as a single range
-                item = [item, item]
-            self.ranges.append(item)
-
-    def _setup(self, **kwargs):
-
-        self.method = kwargs.get("method", self.method)
-        self.interpolation = kwargs.get("interpolation", self.interpolation)
-        if self.interpolation == "polynomial":
-            self.order = int(kwargs.get("order", self.order))
-        if self.method == "multivariate":
-            self.npc = int(kwargs.get("npc", self.npc))
-        self.zoompreview = kwargs.get("zoompreview", self.zoompreview)
-        self.figsize = kwargs.get("figsize", self.figsize)
-
-    def __call__(self, *ranges, **kwargs):
-
-        return self.compute(*ranges, **kwargs)
-
-    def compute(self, *ranges, **kwargs):
-        """
-        Base function for dataset baseline correction.
-
-        Parameters
-        ----------
-        *ranges : a variable number of pair-tuples
-            The regions taken into account for the manual baseline correction.
-        **kwargs
-            Optional keyword parameters (see Other Parameters).
-
-
-        Other Parameters
-        ----------------
-        dim : str or int, keyword parameter, optional, default='x'.
-            Specify on which dimension to apply the apodization method.
-            If `dim` is specified as an integer
-            it is equivalent  to the usual `axis` numpy parameter.
-        method : str, keyword parameter, optional, default='sequential'
-            Correction method among ['multivariate','sequential']
-        interpolation : string, keyword parameter, optional, default='polynomial'
-            Interpolation method for the computation of the baseline,
-            among ['polynomial','pchip']
-        order : int, keyword parameter, optional, default=1
-            If the correction method polynomial,
-            this give the polynomial order to use.
-        npc : int, keyword parameter, optional, default=5
-            Number of components to keep for the ``multivariate`` method
-        zoompreview : float, keyword parameter, optional, default=1.0
-            The zoom factor for the preview in interactive mode
-        figsize : tuple, keyword parameter, optional, default=(8, 6)
-            Size of the figure to display in inch
-        """
-
-        self._setup(**kwargs)
-
-        # output dataset
-        new = self.corrected
-
-        # we assume that the last dimension
-        # if always the dimension to which we want to subtract the baseline.
-        # Swap the axes to be sure to be in this situation
-        axis, dim = new.get_axis(**kwargs, negative_axis=True)
-
-        swapped = False
-        if axis != -1:
-            new.swapdims(axis, -1, inplace=True)
-            swapped = True
-
-        lastcoord = new.coordset[dim]
-
-        # most of the time we need sorted axis, so let's do it now
-        is_descendant = False
-        if lastcoord.descendant:
-            new.sort(dim=dim, inplace=True, descend=False)
-            is_descendant = True
-            lastcoord = new.coordset[dim]
-
-        x = lastcoord.data
-        self.ranges = [[x[0], x[2]], [x[-3], x[-1]]]
-        self._extendranges(*ranges, **kwargs)
-        self.ranges = ranges = trim_ranges(*self.ranges)
-
-        baseline = np.zeros_like(new)
-
-        # Extract: Sbase: the matrix of data corresponding to ranges
-        #          xbase: the xaxis values corresponding to ranges
-
-        s = []
-        for pair in ranges:
-            # determine the slices
-
-            sl = slice(*pair)
-            sect = new[..., sl]
-            if sect is None:
-                continue
-
-            s.append(sect)
-
-        from spectrochempy.core.dataset.nddataset import NDDataset
-
-        sbase = NDDataset.concatenate(s, axis=-1)
-        # TODO: probably we could use masked data instead of concatenating - could be faster
-        xbase = sbase.coordset(dim)
-
-        if self.method == "sequential":
-
-            if self.interpolation == "polynomial":
-                # # bad fit when NaN values => are replaced by 0      # NO reason we have Nan -> suppressed
-                # if np.any(np.isnan(sbase)):
-                #     sbase[np.isnan(sbase)] = 0
+        return args, kwargs
 
-                polycoef = np.polynomial.polynomial.polyfit(
-                    xbase.data, sbase.data.T, deg=self.order, rcond=None, full=False
-                )
-                baseline = np.polynomial.polynomial.polyval(x, polycoef)
+    def _switch_protocol(self, key, files, **kwargs):
 
-            elif self.interpolation == "pchip":
-                for i in range(new.shape[0]):
-                    interp = scipy.interpolate.PchipInterpolator(
-                        xbase.data, sbase.data[i]
-                    )
-                    baseline[i] = interp(x)
+        protocol = kwargs.get("protocol", None)
+        if protocol is not None and protocol != "ALL":
+            if not isinstance(protocol, list):
+                protocol = [protocol]
+            if key and key[1:] not in protocol and self.alias[key[1:]] not in protocol:
+                return
+        datasets = []
+        for filename in files[key]:
+            if (
+                isinstance(filename, str)
+                and not filename.startswith("http://")
+                and not filename.startswith("https://")
+            ):
+                filename = pathclean(filename)
+            read_ = getattr(self, f"_read_{key[1:]}")
+            try:
+                res = read_(self.objtype(), filename, **kwargs)
+                # sometimes read_ can return None (e.g. non labspec text file)
+            except FileNotFoundError:
+                # try to get the file from github
+                kwargs["read_method"] = read_
+                try:
+                    res = _read_remote(self.objtype(), filename, **kwargs)
+
+                except OSError as e:
+                    if kwargs.get("remote"):
+                        raise e
+                    else:
+                        raise FileNotFoundError(f"{filename} not found")
 
-        elif self.method == "multivariate":
+                except IOError as e:
+                    warning_(str(e))
+                    res = None
+
+                except NotImplementedError as e:
+                    warning_(str(e))
+                    res = None
+
+                except Exception as e:
+                    raise e
+
+            except IOError as e:
+                warning_(str(e))
+                res = None
+
+            except NotImplementedError as e:
+                warning_(str(e))
+                res = None
+
+            if res is not None:
+                if not isinstance(res, list):
+                    datasets.append(res)
+                else:
+                    datasets.extend(res)
+
+        if len(datasets) > 1:
+            datasets = self._do_merge(datasets, **kwargs)
+            if kwargs.get("merge", False):
+                datasets[0].name = pathclean(filename).stem
+                datasets[0].filename = pathclean(filename)
+
+        self.datasets.extend(datasets)
+
+    def _do_merge(self, datasets, **kwargs):
+
+        # several datasets returned (only if several files have been passed) and the `merge` keyword argument is False
+        merged = kwargs.get("merge", False)
+        shapes = {nd.shape for nd in datasets}
+        if len(shapes) == 1:
+            # homogeneous set of files
+            dim0 = shapes.pop()[0]
+            if dim0 == 1:
+                merged = kwargs.get("merge", True)  # priority to the keyword setting
+        else:
+            # not homogeneous
+            merged = kwargs.get("merge", False)
 
-            # SVD of Sbase
-            U, s, Vt = np.linalg.svd(sbase.data, full_matrices=False, compute_uv=True)
+        if merged:
+            # Try to stack the dataset into a single one
+            try:
+                dataset = self.objtype.concatenate(datasets, axis=0)
+                if dataset.coordset is not None and kwargs.pop("sortbydate", True):
+                    dataset.sort(dim="y", inplace=True)
+                    dataset.history = "Sorted by date"
+                datasets = [dataset]
+
+            except DimensionsCompatibilityError as e:
+                warn(str(e))  # return only the list
+
+        return datasets
+
+
+def _importer_method(func):
+    # Decorator to define a given read function as belonging to Importer
+    setattr(Importer, func.__name__, staticmethod(func))
+    return func
+
+
+# --------------------------------------------------------------------------------------
+# Generic Read function
+# --------------------------------------------------------------------------------------
+def read(*paths, **kwargs):
+    """
+    Generic read method.
 
-            # npc cannot be higher than the size of s
-            npc = min(self.npc, s.shape[0])
+    This method is generally able to load experimental files based on extensions.
 
-            # select npc loadings & compute scores
-            Pt = Vt[0:npc]
-            T = np.dot(U[:, 0:npc], np.diag(s)[0:npc, 0:npc])
+    Parameters
+    ----------
+    *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
+        The data source(s) can be specified by the name or a list of name for the
+        file(s) to be loaded:
 
-            baseline_loadings = np.zeros((npc, new.shape[-1]))
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
-            if self.interpolation == "pchip":
-                for i in range(npc):
-                    interp = scipy.interpolate.PchipInterpolator(xbase.data, Pt[i])
-                    baseline_loadings[i] = interp(x)
+        If the list of filenames are enclosed into brackets:
 
-            elif self.interpolation == "polynomial":
-                polycoef = np.polynomial.polynomial.polyfit(
-                    xbase.data, Pt.T, deg=self.order, rcond=None, full=False
-                )
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
-                baseline_loadings = np.polynomial.polynomial.polyval(x, polycoef)
+        The returned datasets are merged to form a single dataset,
+        except if `merge` is set to False. If a source is not provided (i.e. no
+        `filename` , nor `content` ),
+        a dialog box will be opened to select files.
+    **kwargs
+        Optional keyword parameters (see Other Parameters).
 
-            baseline = np.dot(T, baseline_loadings)
+    Returns
+    --------
+    read
+        `NDDataset` or list of `NDDataset` .
 
-        new.data = new.data - baseline
+    Other Parameters
+    ----------------
+    protocol : {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel'}, optional
+        Protocol used for reading. If not provided, the correct protocol
+        is inferred (whenever it is possible) from the file name extension.
+    directory : str, optional
+        From where to read the specified `filename` . If not specified, read in the
+        default `datadir` specified in
+        SpectroChemPy Preferences.
+    merge : bool, optional
+        Default value is False. If True, and several filenames have been provided as
+        arguments,
+        then a single dataset with merged (stacked along the first
+        dimension) is returned (default=False).
+    sortbydate : bool, optional
+        Sort multiple spectra by acquisition date (default=True).
+    description : str, optional
+        A Custom description.
+    origin : {'omnic', 'tga'}, optional
+        In order to properly interpret CSV file it can be necessary to set the origin
+        of the spectra.
+        Up to now only 'omnic' and 'tga' have been implemented.
+    csv_delimiter : str, optional
+        Set the column delimiter in CSV file.
+        By default it is the one set in SpectroChemPy `Preferences` .
+    content : bytes object, optional
+        Instead of passing a filename for further reading, a bytes content can be directly provided as bytes objects.
+        The most convenient way is to use a dictionary. This feature is particularly useful for a GUI Dash application
+        to handle drag and drop of files into a Browser.
+        For examples on how to use this feature, one can look in the `tests/tests_readers` directory.
+    listdir : bool, optional
+        If True and filename is None, all files present in the provided `directory` are returned (and merged if `merge`
+        is True. It is assumed that all the files correspond to current reading protocol (default=True)
+    recursive : bool, optional
+        Read also in subfolders. (default=False)
 
-        # eventually sort back to the original order
-        if is_descendant:
-            new.sort(axis=-1, inplace=True, descend=True)
+    See Also
+    --------
+    read_topspin : Read TopSpin Bruker NMR spectra.
+    read_omnic : Read Omnic spectra.
+    read_opus : Read OPUS spectra.
+    read_labspec : Read Raman LABSPEC spectra.
+    read_spg : Read Omnic .spg grouped spectra.
+    read_spa : Read Omnic .spa single spectra.
+    read_spc : Read Galactic .spc files.
+    read_srs : Read Omnic series.
+    read_csv : Read CSV files.
+    read_zip : Read Zip files.
+    read_matlab : Read Matlab files.
 
-        new.history = "Baseline correction." + " Method: "
-        if self.method == "Multivariate":
-            new.history = "Multivariate (" + str(self.npc) + " PCs)."
-        else:
-            new.history = "Sequential."
+    Examples
+    ---------
+    Reading a single OPUS file  (providing a windows type filename relative to the default `Datadir` )
 
-        if self.interpolation == "polynomial":
-            new.history = "Interpolation: Polynomial, order=" + str(self.order) + ".\n"
-        else:
-            new.history = "Interpolation: Pchip. \n"
+    >>> scp.read('irdata\\\\OPUS\\\\test.0000')
+    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
-        if swapped:
-            new = new.swapdims(axis, -1)
+    Reading a single OPUS file  (providing a unix/python type filename relative to the default `Datadir` )
+    Note that here read_opus is called as a classmethod of the NDDataset class
 
-        self.corrected = new
-        return new
+    >>> scp.NDDataset.read('irdata/OPUS/test.0000')
+    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
-    def show_regions(self, ax):
-        if self.sps:
-            for sp in self.sps:
-                sp.remove()
-        self.sps = []
-        self.ranges = list(trim_ranges(*self.ranges))
-        for x in self.ranges:
-            x.sort()
-            sp = ax.axvspan(x[0], x[1], facecolor="#2ca02c", alpha=0.5)
-            self.sps.append(sp)
-
-    def run(self, *ranges, **kwargs):
-        """
-        Interactive version of the baseline correction.
-
-        Parameters
-        ----------
-        *ranges : a variable number of pair-tuples
-            The regions taken into account for the manual baseline correction.
-        **kwargs
-            See other parameter of method compute.
-        """
-        self._setup(**kwargs)
-        self.sps = []
-
-        # output dataset
-        new = self.corrected
-        origin = self.dataset.copy()
-
-        # we assume that the last dimension if always the dimension to which we want to subtract the baseline.
-        # Swap the axes to be sure to be in this situation
-        axis, dim = new.get_axis(**kwargs, negative_axis=True)
-
-        # swapped = False
-        if axis != -1:
-            new.swapdims(axis, -1, inplace=True)
-            origin.swapdims(axis, -1, inplace=True)
-            # swapped = True
-
-        lastcoord = new.coordset[dim]
-
-        # most of the time we need sorted axis, so let's do it now
-
-        if lastcoord.reversed:
-            new.sort(dim=dim, inplace=True, descend=False)
-            lastcoord = new.coordset[dim]
-
-        x = lastcoord.data
-        self.ranges = [[x[0], x[2]], [x[-3], x[-1]]]
-        self._extendranges(*ranges, **kwargs)
-        self.ranges = ranges = trim_ranges(*self.ranges)
-
-        new = self.compute(*ranges, **kwargs)
-
-        # display
-        datasets = [origin, new]
-        labels = [
-            "Click on left button & Span to set regions. Click on right button on a region to remove it.",
-            "Baseline corrected dataset preview",
-        ]
-        axes = multiplot(
-            datasets,
-            labels,
-            method="stack",
-            sharex=True,
-            nrow=2,
-            ncol=1,
-            figsize=self.figsize,
-            suptitle="INTERACTIVE BASELINE CORRECTION",
-        )
+    Single file specified with pathlib.Path object
 
-        fig = plt.gcf()
-        fig.canvas.draw()
+    >>> from pathlib import Path
+    >>> folder = Path('irdata/OPUS')
+    >>> p = folder / 'test.0000'
+    >>> scp.read(p)
+    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
-        ax1 = axes["axe11"]
-        ax2 = axes["axe21"]
+    Multiple files not merged (return a list of datasets). Note that a directory is specified
 
-        self.show_regions(ax1)
+    >>> le = scp.read('test.0000', 'test.0001', 'test.0002', directory='irdata/OPUS')
+    >>> len(le)
+    3
+    >>> le[0]
+    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
-        def show_basecor(ax2):
-
-            corrected = self.compute(*ranges, **kwargs)
-
-            ax2.clear()
-            ax2.set_title(
-                "Baseline corrected dataset preview", fontweight="bold", fontsize=8
-            )
-            if self.zoompreview > 1:
-                zb = 1.0  # self.zoompreview
-                zlim = [corrected.data.min() / zb, corrected.data.max() / zb]
-                _ = corrected.plot_stack(ax=ax2, colorbar=False, zlim=zlim, clear=False)
-            else:
-                _ = corrected.plot_stack(ax=ax2, colorbar=False, clear=False)
+    Multiple files merged as the `merge` keyword is set to true
 
-        show_basecor(ax2)
+    >>> scp.read('test.0000', 'test.0001', 'test.0002', directory='irdata/OPUS', merge=True)
+    NDDataset: [float64] a.u. (shape: (y:3, x:2567))
 
-        def onselect(xmin, xmax):
-            self.ranges.append([xmin, xmax])
-            self.show_regions(ax1)
-            show_basecor(ax2)
-            fig.canvas.draw()
-
-        def onclick(event):
-            if event.button == 3:
-                for i, r in enumerate(self.ranges):
-                    if r[0] > event.xdata or r[1] < event.xdata:
-                        continue
-                    else:
-                        self.ranges.remove(r)
-                        self.show_regions(ax1)
-                        show_basecor(ax2)
-                        fig.canvas.draw()  # _idle
-
-        _ = fig.canvas.mpl_connect("button_press_event", onclick)
-
-        _ = SpanSelector(
-            ax1,
-            onselect,
-            "horizontal",
-            minspan=5,
-            button=[1],
-            useblit=True,
-            props=dict(alpha=0.5, facecolor="blue"),
-        )
+    Multiple files to merge : they are passed as a list instead of using the keyword `merge`
 
-        fig.canvas.draw()
+    >>> scp.read(['test.0000', 'test.0001', 'test.0002'], directory='irdata/OPUS')
+    NDDataset: [float64] a.u. (shape: (y:3, x:2567))
 
-        return
+    Multiple files not merged : they are passed as a list but `merge` is set to false
 
+    >>> le = scp.read(['test.0000', 'test.0001', 'test.0002'], directory='irdata/OPUS', merge=False)
+    >>> len(le)
+    3
 
-def basc(dataset, *ranges, **kwargs):
-    """
-    Compute a baseline correction using the BaselineCorrection processor.
+    Read without a filename. This has the effect of opening a dialog for file(s) selection
 
-    2 methods are proposed :
+    >>> nd = scp.read()
 
-    * ``sequential`` (default) = classical polynom fit or spline
-      interpolation with separate fitting of each row (spectrum)
-    * ``multivariate`` = SVD modeling of baseline, polynomial fit of PC's
-      and calculation of the modelled baseline spectra.
+    Read in a directory (assume that only OPUS files are present in the directory
+    (else we must use the generic `read` function instead)
 
-    Parameters
-    ----------
-    dataset : a [NDDataset| instance
-        The dataset where to calculate the baseline.
-    *ranges : a variable number of pair-tuples
-        The regions taken into account for the manual baseline correction.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
+    >>> le = scp.read(directory='irdata/OPUS')
+    >>> len(le)
+    2
 
-    Other Parameters
-    ----------------
-    dim : str or int, keyword parameter, optional, default='x'.
-        Specify on which dimension to apply the apodization method. If `dim` is specified as an integer
-        it is equivalent  to the usual `axis` numpy parameter.
-    method : str, keyword parameter, optional, default='sequential'
-        Correction method among ['multivariate','sequential']
-    interpolation : string, keyword parameter, optional, default='polynomial'
-        Interpolation method for the computation of the baseline, among ['polynomial','pchip']
-    order : int, keyword parameter, optional, default=6
-        If the correction method polynomial, this give the polynomial order to use.
-    npc : int, keyword parameter, optional, default=5
-        Number of components to keep for the ``multivariate`` method
+    Again we can use merge to stack all 4 spectra if thet have compatible dimensions.
 
-    See Also
-    --------
-    BaselineCorrection : Manual baseline corrections.
-    abc : Automatic baseline correction.
+    >>> scp.read(directory='irdata/OPUS', merge=True)
+    [NDDataset: [float64] a.u. (shape: (y:1, x:5549)), NDDataset: [float64] a.u. (shape: (y:4, x:2567))]
+    """
 
-    Notes
-    -----
-    For more flexibility and functionality, it is advised to use the BaselineCorrection processor instead.
+    importer = Importer()
 
-    Examples
-    --------
-    .. plot::
-        :include-source:
+    protocol = kwargs.get("protocol", None)
+    available_protocols = list(importer.protocols.values())
+    available_protocols.extend(
+        list(importer.alias.keys())
+    )  # to handle variants of protocols
+    if protocol is None:
+        kwargs["filetypes"] = list(importer.filetypes.values())
+        kwargs["protocol"] = "ALL"
+        default_filter = kwargs.get("default_filter", None)
+        if default_filter is not None:
+            kwargs["default_filter"] = importer.filetypes[default_filter]
+    else:
+        try:
+            kwargs["filetypes"] = [importer.filetypes[protocol]]
+        except KeyError:
+            raise ProtocolError(protocol, list(importer.protocols.values()))
 
-        import spectrochempy as scp
-        nd = scp.read('irdata/nh4y-activation.spg')
-        ndp = nd[:, 1291.0:5999.0]
-
-        ranges=[[5996., 5998.], [1290., 1300.],
-                [2205., 2301.], [5380., 5979.],
-                [3736., 5125.]]
-
-        ndcorr = scp.basc(ndp, *ranges,method='multivariate', interpolation='pchip', npc=8)
-        ndcorr.plot()
-        scp.show()
-    """
-    blc = BaselineCorrection(dataset)
-    if not ranges and dataset.meta.regions is not None:
-        # use the range stored in metadata
-        ranges = dataset.meta.regions["baseline"]
-    return blc.compute(*ranges, **kwargs)
+    return importer(*paths, **kwargs)
 
 
-# ======================================================================================
-# abc # TODO: some work to perform on this
-# ======================================================================================
-def abc(dataset, dim=-1, **kwargs):
+def read_dir(directory=None, **kwargs):
     """
-    Automatic baseline correction.
+    Read an entire directory.
 
-    Various algorithms are provided to calculate the baseline automatically.
+    Open a list of readable files in a and store data/metadata in a dataset or a list of datasets according to the
+    following rules :
+
+    * 2D spectroscopic data (e.g. valid .spg files or matlab arrays, etc...) from
+      distinct files are stored in distinct NDdatasets.
+    * 1D spectroscopic data (e.g., .spa files) in a given directory are grouped
+      into single NDDataset, providing their unique dimension are compatible. If not,
+      an error is generated.
+    * non-readable files are ignored
 
     Parameters
     ----------
-    dataset : a [NDDataset| instance
-        The dataset where to calculate the baseline.
-    dim : str or int, optional
-        The dataset dimentsion where to calculate the baseline. Default is -1.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
-
+    directory : str or pathlib
+        Folder where are located the files to read.
 
     Returns
-    -------
-    baseline_corrected
-        A baseline corrected dataset.
-    baseline_only
-        Only the baseline (apply must be set to False).
-    baseline_points
-        Points where the baseline is calculated (return_points must be set to True).
+    --------
+    read_dir
+        `NDDataset` or list of `NDDataset` .
 
-    Other Parameters
-    ----------------
-    basetype : string, optional, default: 'linear'
-        See notes - available = linear, basf, ...
-    window : float/int, optional, default is 0.05
-        If float <1 then the corresponding percentage of the axis size is taken as window.
-    nbzone : int, optional, default is 32
-        Number of zones. We will divide the size of the last axis by this number
-        to determine the number of points in each zone (nw).
-    mult : int
-        A multiplicator. determine the number of point for the database calculation (nw*mult<n base points).
-    nstd : int, optional, default is 2 times the standard error
-        Another multiplicator. Multiply the standard error to determine the region in which points are from the
-        baseline.
-    polynom : bool, optional, default is True
-        If True a polynom is computed for the base line, else an interpolation is achieved betwwen points.
-    porder : int, default is 6
-        Order of the polynom to fit on the baseline points
-    return_points : bool, optional, default is False
-        If True, the points abscissa used to determine the baseline are returned.
-    apply : bool, optional, default is True
-        If apply is False, the data are not modified only the baseline is returned.
-    return_pts : bool, optional, default is False
-        If True, the baseline reference points are returned.
+    Depending on the python version, the order of the datasets in the list may change.
 
     See Also
     --------
-    BaselineCorrection : Manual baseline corrections.
-    basc : Manual baseline correction.
-
-    Notes
-    -----
-    #TODO: description of these algorithms
-    * linear -
-    * basf -
+    read_topspin : Read TopSpin Bruker NMR spectra.
+    read_omnic : Read Omnic spectra.
+    read_opus : Read OPUS spectra.
+    read_spg : Read Omnic .spg grouped spectra.
+    read_spa : Read Omnic .Spa single spectra.
+    read_srs : Read Omnic series.
+    read_csv : Read CSV files.
+    read_zip : Read Zip files.
+    read_matlab : Read Matlab files.
 
     Examples
     --------
-    To be done
-    """
-    # # options evaluation
-    # parser = argparse.ArgumentParser(description='BC processing.', usage="""
-    # ab [-h] [--mode {linear,poly, svd}] [--dryrun]
-    #                        [--window WINDOW] [--step STEP] [--nbzone NBZONE]
-    #                        [--mult MULT] [--order ORDER] [--verbose]
-    # """)
-    # # positional arguments
-    # parser.add_argument('--mode', '-mo', default='linear',
-    #                      choices=['linear', 'poly', 'svd'], help="mode of correction")
-    # parser.add_argument('--dryrun', action='store_true', help='dry flag')
-    #
-    # parser.add_argument('--window', '-wi', default=0.05, type=float, help='selected window for linear and svd bc')
-    # parser.add_argument('--step', '-st', default=5, type=int, help='step for svd bc')
-    # parser.add_argument('--nbzone', '-nz', default=32, type=int, help='number of zone for poly')
-    # parser.add_argument('--mult', '-mt', default=4, type=int, help='multiplicator of zone for poly')
-    # parser.add_argument('--order', '-or', default=5, type=int, help='polynom order for poly')
-    #
-    # parser.add_argument('--verbose', action='store_true', help='verbose flag')
-    # args = parser.parse_args(options.split())
-    #
-    # source.history.append('baseline correction mode:%s' % args.mode)
-
-    inplace = kwargs.pop("inplace", False)
-    dryrun = kwargs.pop("dryrun", False)
-
-    # output dataset inplace or not
-    if not inplace or dryrun:  # default
-        new = dataset.copy()
-    else:
-        new = dataset
-
-    axis, dim = new.get_axis(dim, negative_axis=True)
-    swapped = False
-    if axis != -1:
-        new.swapdims(axis, -1, inplace=True)  # must be done in  place
-        swapped = True
-
-    base = _basecor(new.data.real, **kwargs)
-
-    if not dryrun:
-        new.data -= base  # return the corrected spectra
-    else:
-        new.data = base  # return the baseline
-
-    # restore original data order if it was swapped
-    if swapped:
-        new.swapdims(axis, -1, inplace=True)  # must be done inplace
-
-    new.history = "`abc` Baseline correction applied."
-    return new
 
+    >>> scp.preferences.csv_delimiter = ','
+    >>> A = scp.read_dir('irdata')
+    >>> len(A)
+    4
 
-def ab(dataset, dim=-1, **kwargs):
+    >>> B = scp.NDDataset.read_dir()
     """
-    Alias of `abc`.
-    """
-    return abs(dataset, dim, **kwargs)
+    kwargs["listdir"] = True
+    importer = Importer()
+    return importer(directory, **kwargs)
 
 
-@_units_agnostic_method
-def dc(dataset, **kwargs):
+def read_remote(file_or_dir, **kwargs):
     """
-    Time domain baseline correction.
+    Download and read files or an entire directory on github spectrochempy_data
+    repository.
+
+    This is done only if the data are not yet downloaded and present in the DATADIR
+    directory.
 
     Parameters
     ----------
-    dataset : nddataset
-        The time domain daatset to be corrected.
-    kwargs : dict, optional
-        Additional parameters.
-
-    Returns
-    -------
-    dc
-        DC corrected array.
+    file_or_dir : str or pathlib
+        Folder where are located the files to read
+        (it should be written as if it was locally downloaded already).
+    **kwargs : optional keywords parameters
+        See Other Parameters.
 
     Other Parameters
     ----------------
-    len : float, optional
-        Proportion in percent of the data at the end of the dataset to take into account. By default, 25%.
-    """
-
-    len = int(kwargs.pop("len", 0.25) * dataset.shape[-1])
-    dc = np.mean(np.atleast_2d(dataset)[..., -len:])
-    dataset -= dc
+    merge : bool, optional, default: False
+        By default files read are noot merged
+    replace_existing: bool, optional, default: False
+        By default, existing files are not replaced so not downloaded.
+    download_only: bool, optional, default: False
+        If True, only downloading and saving of the files is performed, with no
+        attempt to read their content.
 
-    return dataset
+    Returns
+    --------
+    dataset(s)
+        `NDDataset` or list of `NDDataset` .
 
+    See Also
+    --------
+    read_topspin : Read TopSpin Bruker NMR spectra.
+    read_omnic : Read Omnic spectra.
+    read_opus : Read OPUS spectra.
+    read_spg : Read Omnic \*.spg grouped spectra.
+    read_spa : Read Omnic \*.spa single spectra.
+    read_srs : Read Omnic series.
+    read_csv : Read CSV files.
+    read_zip : Read Zip files.
+    read_matlab : Read Matlab files.
 
-# ======================================================================================
-# private functions
-# ======================================================================================
-def _basecor(data, **kwargs):
-    mode = kwargs.pop("mode", "linear")
+    Examples
+    --------
 
-    if mode == "linear":
-        return _linearbase(data, **kwargs)
+    >>> A = scp.read_remote('irdata/subdir')
+    """
+    kwargs["remote"] = True
+    if "merge" not in kwargs:
+        kwargs["merge"] = False  # by default, no attempt to merge
+    if "replace_existing" not in kwargs:
+        kwargs["replace_existing"] = False  # by default we download only if needed.
+    importer = Importer()
+    return importer(file_or_dir, **kwargs)
+
+
+def _write_downloaded_file(content, dst):
+    if not dst.parent.exists():
+        # create the eventually missing subdirectory
+        dst.parent.mkdir(parents=True, exist_ok=True)
+    dst.write_bytes(content)
+    info_(f"{dst.name} has been downloaded and written in {dst.parent}")
 
-    if mode == "svd":
-        return _svdbase(data, **kwargs)
 
-    if mode == "poly":
-        return _polybase(data, **kwargs)
-    else:
-        raise ValueError(f"`ab` mode = `{mode}`  not known")
+def _get_url_content_and_save(url, dst, replace):
 
+    if not replace and dst.exists():
+        return
 
-#
-# _linear mode
-#
-def _linearbase(data, **kwargs):
-    # Apply a linear baseline correction
-    # Very simple and naive procedure that compute a straight baseline from side to the other
-    # (averging on a window given by the window parameters : 5% of the total width on each side by default)
-
-    window = kwargs.pop("window", 0.05)
-
-    if window <= 1.0:
-        # percent
-        window = int(data.shape[-1] * window)
-
-    if len(data.shape) == 1:
-        npts = float(data.shape[-1])
-        a = (data[-window:].mean() - data[:window].mean()) / (npts - 1.0)
-        b = data[:window].mean()
-        baseline = a * np.arange(npts) + b
+    try:
+        r = requests.get(url, allow_redirects=True)
 
-    else:
-        npts = float(data.shape[-1])
-        a = (data[:, -window:].mean(axis=-1) - data[:, :window].mean(axis=-1)) / (
-            npts - 1.0
+        # write downloaded file
+        r.raise_for_status()
+        _write_downloaded_file(r.content, dst)
+
+    except OSError:
+        raise FileNotFoundError(f"Not found locally or at url:{url}")
+
+
+def _download_full_testdata_directory():
+    from spectrochempy.core import preferences as prefs
+
+    datadir = prefs.datadir
+
+    url = "https://github.com/spectrochempy/spectrochempy_data/archive/refs/heads/master.zip"
+
+    resp = requests.get(url)
+    zipfile = ZipFile(BytesIO(resp.content))
+    files = [zipfile.open(file_name) for file_name in zipfile.namelist()]
+
+    for file in files:
+        name = file.name
+        if name.endswith("/") or "testdata/" not in name:  # dir
+            continue
+        uncompressed = zipfile.read(name)
+        p = list(pathclean(name).parts)[2:]
+        dst = datadir.joinpath("/".join(p))
+        _write_downloaded_file(uncompressed, dst)
+
+
+def _download_from_url(url, dst, replace=False):
+    # ##
+    # ##    Do not forget to change the fork in the following url
+    # ##
+    if not str(url).startswith("https://") and not str(url).startswith("http://"):
+        # download on github
+        url = (
+            f"https://github.com/spectrochempy/spectrochempy_data/raw/master/"
+            f"testdata/{url}"
         )
-        b = data[:, :window].mean(axis=-1)
-        baseline = (((np.ones_like(data).T * a).T * np.arange(float(npts))).T + b).T
 
-    return baseline
+        # first determine if it is a directory
+        r = requests.get(url + "/__index__", allow_redirects=True)
+        index = None
+        if r.status_code == 200:
+            index = yaml.load(r.content, Loader=yaml.CLoader)
 
+        if index is None:
+            _get_url_content_and_save(url, dst, replace)
 
-def _planeFit(points):
-    # p, n = planeFit(points)  # copied from https://stackoverflow.com/a/18968498
-    #
-    # Fit an multi-dimensional plane to the points.
-    # Return a point on the plane and the normal.
-    #
-    # Parameters
-    # ----------
-    # points :
-    #
-    # Notes
-    # -----
-    #     Replace the nonlinear optimization with an SVD.
-    #     The following creates the moment of inertia tensor, M, and then
-    #     SVD's it to get the normal to the plane.
-    #     This should be a close approximation to the least-squares fit
-    #     and be much faster and more predictable.
-    #     It returns the point-cloud center and the normal.
-
-    from numpy.linalg import svd
-
-    npts = points.shape[0]
-    points = np.reshape(points, (npts, -1))
-    assert points.shape[0] < points.shape[1]
-    ctr = points.mean(axis=1)
-    x = points - ctr[:, None]
-    M = np.dot(x, x.T)
-    return ctr, svd(M)[0][:, -1]
-
-
-def _svdbase(data, args=None, retw=False):
-    # Apply a planar baseline correction to 2D data
-    import pandas as pd  # TODO: suppress this need
-
-    if not args:
-        window = 0.05
-        step = 5
+        else:
+            for filename in index["files"]:
+                _get_url_content_and_save(f"{url}/{filename}", dst / filename, replace)
+            for folder in index["folders"]:
+                _download_from_url(f"{url}/{folder}", dst / folder)
     else:
-        window = args.window
-        step = args.step
+        # download url
+        _get_url_content_and_save(url, dst, replace)
+
 
-    if window <= 1.0:
-        # percent
-        window = int(data.shape[-1] * window)
-
-    data = pd.DataFrame(
-        data
-    )  # TODO: facilitate the manipulation (but to think about further)
-    a = pd.concat([data.iloc[:window], data.iloc[-window:]])
-    b = pd.concat(
-        [data.iloc[window:-window, :window], data.iloc[window:-window, -window:]],
-        axis=1,
+def _is_relative_to(path, base):
+    # try to emulate the pathlib is_relative_to method which does not work on python
+    # 3.7 (needed for Colab!)
+    # TODO: replace as Colab is updated to 3.9
+    pparts = path.parts
+    bparts = base.parts
+    if bparts[-1] in pparts:
+        idx = pparts.index(bparts[-1])
+        pparts_base = pparts[: idx + 1]
+        return pparts_base == bparts
+    return False
+
+
+def _relative_to(path, base):
+    pparts = path.parts
+    bparts = base.parts
+    if bparts[-1] in pparts:
+        idx = pparts.index(bparts[-1])
+        return pathclean("/".join(pparts[idx + 1 :]))
+    raise ValueError(
+        f"'{path}' is not in the subpath of '{base}' OR one path is "
+        f"relative and the other absolute."
     )
-    bs = pd.concat([a, b])
-    bs = bs.stack()
-    bs.sort()
-    x = []
-    y = []
-    z = []
-    for item in bs.index[::step]:
-        x.append(item[0])
-        y.append(item[1])
-        z.append(bs[item].real)
-
-    norm = np.max(np.abs(z))
-    z = np.array(z)
-    z = z / norm
-    XYZ = np.array((x, y, z))
-    p, n = _planeFit(XYZ)
-    d = np.dot(p, n)
-
-    col = data.columns
-    row = data.index
-    X, Y = np.meshgrid(col, row)
-    Z = -norm * (n[0] * X + n[1] * Y - d) / n[2]
-
-    if retw:
-        return Z, None  # TODO: return something
-    return Z
-
-
-def _polybase(data, **kwargs):
-    # Automatic baseline correction
-
-    if data.ndim == 1:
-        dat = np.array(
-            [
-                data,
-            ]
-        )
 
-    nbzone = kwargs.pop("nbzone", 64)
-    mult = kwargs.pop("mult", 4)
-    order = kwargs.pop("order", 6)
-
-    npts = data.shape[-1]
-    w = np.arange(npts)
-
-    baseline = np.ma.masked_array(dat, mask=True)
-    sigma = 1.0e6
-    nw = int(npts / nbzone)
-
-    # print (nw)
-    # unmask extremities of the baseline
-    baseline[:, :nw].mask = False
-    baseline[:, -nw:].mask = False
-
-    for j in range(nbzone):
-        s = dat[:, nw * j : min(nw * (j + 1), npts + 1)]
-        sigma = min(s.std(), sigma)
-
-    nw = nw * 2  # bigger window
-    nw2 = int(nw / 2)
-
-    found = False
-    nb = 0
-    nstd = 2.0
-    while (not found) or (nb < nw * mult):
-        nb = 0
-        for i in range(nw2, npts - nw2 + 1, 1):
-            s1 = dat[:, max(i - 1 - nw2, 0) : min(i - 1 + nw2, npts + 1)]
-            s2 = dat[:, max(i - nw2, 0) : min(i + nw2, npts + 1)]
-            s3 = dat[:, max(i + 1 - nw2, 0) : min(i + 1 + nw2, npts + 1)]
-            mi1, mi2, mi3 = s1.min(), s2.min(), s3.min()
-            ma1, ma2, ma3 = s1.max(), s2.max(), s3.max()
 
-            if (
-                abs(ma1 - mi1) < float(nstd) * sigma
-                and abs(ma2 - mi2) < float(nstd) * sigma
-                and abs(ma3 - mi3) < float(nstd) * sigma
-            ):
-                found = True
-                nb += 1
-                baseline[:1, i].mask = False  # baseline points
-
-        # increase nstd
-        nstd = nstd * 1.1
-    debug_("basf optimized nstd: %.2F mult: %.2f" % (nstd, mult))
-
-    wm = np.array(list(zip(*np.argwhere(~baseline[:1].mask)))[1])
-    bm = baseline[:, wm]
-    if data.ndim > 1:
-        bm = smooth(bm.T, max(int(dat.shape[0] / 10), 3)).T
-    bm = smooth(bm, max(int(dat.shape[-1] / 10), 3))
-
-    # if not polynom:
-    #    sr = pchip(wm, bm.real)
-    #    si = pchip(wm, bm.imag)
-    #    baseline = sr(w) + si(w) * 1.0j
-    #    baseline = smooth(baseline, window_len=int(nw / 4))
-    # else:
-    # fit a polynom
-    pf = np.polyfit(wm, bm.T, order).T
-    for i, row in enumerate(pf[:]):
-        poly = np.poly1d(row)
-        baseline[i] = poly(w)
+@_importer_method
+def _read_remote(*args, **kwargs):
+    from spectrochempy.core import preferences as prefs
+
+    datadir = prefs.datadir
+
+    dataset, path = args
+    is_url = str(path).startswith("http://") or str(path).startswith("https://")
+
+    replace = kwargs.pop("replace_existing", False)
+    if not is_url:
+        path = pathclean(path)
+
+        if _is_relative_to(path, datadir):
+            # try to make it relative for remote downloading on github
+            relative_path = _relative_to(path, datadir)
+        else:
+            # assume it is already relative
+            relative_path = path
 
-    if data.ndim == 1:
-        baseline = baseline[0]
+        # in principle the data came from github. Try to download it
+        dst = datadir / relative_path
+        if dst.name != "testdata":
+            _download_from_url(relative_path, dst, replace)
+        else:
+            # we are going to download the whole testdata directory -> use a faster method
+            _download_full_testdata_directory()
 
-    return baseline
+    else:
+        # download localy
+        dst = pathclean(path.split("/")[-1])
+        _download_from_url(path, dst, replace)
+
+    if not kwargs.pop("download_only", False):
+        read_method = kwargs.pop("read_method", read)
+        return read_method(dataset, dst, **kwargs)
+
+
+# ======================================================================================
+# Private functions
+# ======================================================================================
+@_importer_method
+def _read_dir(*args, **kwargs):
+    _, directory = args
+    directory = get_directory_name(directory)
+    files = get_filenames(directory, **kwargs)
+    datasets = []
+    valid_extensions = list(zip(*FILETYPES))[0] + list(zip(*ALIAS))[0]
+    for key in [key for key in files.keys() if key[1:] in valid_extensions]:
+        if key:
+            importer = Importer()
+            nd = importer(files[key], **kwargs)
+            if nd is not None:
+                if not isinstance(nd, list):
+                    nd = [nd]
+                datasets.extend(nd)
+    return datasets
+
+
+@_importer_method
+def _read_scp(*args, **kwargs):
+    dataset, filename = args
+    return dataset.load(filename, **kwargs)
+
+
+@_importer_method
+def _read_(*args, **kwargs):
+    dataset, filename = args
+
+    if kwargs.pop("remote", False):
+        return Importer._read_remote(*args, **kwargs)
+    elif not filename or filename.is_dir():
+        return Importer._read_dir(*args, **kwargs)
+
+    # protocol = kwargs.get("protocol", None)
+    # if protocol and ".scp" in protocol:
+    #     return dataset.load(filename, **kwargs)
+    #
+    # elif filename and filename.name in ("fid", "ser", "1r", "2rr", "3rrr"):
+    #     # probably an Topspin NMR file
+    #     return dataset.read_topspin(filename, **kwargs)
+    # elif filename:
+    #     # try scp format
+    #     try:
+    #         return dataset.load(filename, **kwargs)
+    #     except Exception:
+    #         # lets try some common format
+    #         for key in ["omnic", "opus", "topspin", "labspec", "matlab", "jdx"]:
+    #             try:
+    #                 _read = getattr(dataset, f"read_{key}")
+    #                 f = f"{filename}.{key}"
+    #                 return _read(f, **kwargs)
+    #             except Exception:
+    #                 pass
+    #         raise NotImplementedError
 
 
+# --------------------------------------------------------------------------------------
 if __name__ == "__main__":
     pass
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/processors/concatenate.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/concatenate.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,55 +12,56 @@
 from warnings import warn
 
 import numpy as np
 
 from spectrochempy.core.dataset.baseobjects.ndarray import DEFAULT_DIM_NAME
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.utils import exceptions
+from spectrochempy.utils.decorators import deprecated
 from spectrochempy.utils.orderedset import OrderedSet
 
 
 def concatenate(*datasets, **kwargs):
     """
-    Concatenation of |NDDataset| objects along a given axis.
+    Concatenation of `NDDataset` objects along a given axis.
 
-    Any number of |NDDataset| objects can be concatenated (by default
+    Any number of `NDDataset` objects can be concatenated (by default
     the last on the last dimension). For this operation
     to be defined the following must be true :
 
-        #. all inputs must be valid |NDDataset| objects;
+        #. all inputs must be valid `NDDataset` objects;
         #. units of data must be compatible
         #. concatenation is along the axis specified or the last one;
         #. along the non-concatenated dimensions, shapes must match.
 
     Parameters
     ----------
-    *datasets : positional |NDDataset| arguments
+    \*datasets : positional `NDDataset` arguments
         The dataset(s) to be concatenated to the current dataset. The datasets
         must have the same shape, except in the dimension corresponding to axis
         (the last, by default).
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     out
-        A |NDDataset| created from the contenations of the |NDDataset| input objects.
+        A `NDDataset` created from the contenations of the `NDDataset` input objects.
 
     Other Parameters
     ----------------
     dims : str, optional, default='x'
         The dimension along which the operation is applied.
 
     axis : int, optional
         The axis along which the operation is applied.
 
     See Also
     ---------
-    stack : Stack of |NDDataset| objects along a new dimension.
+    stack : Stack of `NDDataset` objects along a new dimension.
 
     Examples
     --------
     >>> A = scp.read('irdata/nh4y-activation.spg', protocol='omnic')
     >>> B = scp.read('irdata/nh4y-activation.scp')
     >>> C = scp.concatenate(A[10:], B[3:5], A[:10], axis=0)
     >>> A[10:].shape, B[3:5].shape, A[:10].shape, C.shape
@@ -75,15 +76,15 @@
     >>> E = A.concatenate(B, axis=1)
     >>> A.shape, B.shape, E.shape
     ((55, 5549), (55, 5549), (55, 11098))
     """
 
     # check uise
     if "force_stack" in kwargs:
-        exceptions.deprecated("force_stack", replace="method stack()")
+        deprecated("force_stack", replace="method stack()")
         return stack(datasets)
 
     # get a copy of input datasets in order that input data are not modified
     datasets = _get_copy(datasets)
 
     # get axis from arguments
     axis, dim = datasets[0].get_axis(**kwargs)
@@ -185,36 +186,36 @@
     out.history = ["Created by concatenate"]
 
     return out
 
 
 def stack(*datasets):
     """
-    Stack of |NDDataset| objects along a new dimension.
+    Stack of `NDDataset` objects along a new dimension.
 
-    Any number of |NDDataset| objects can be stacked. For this operation
+    Any number of `NDDataset` objects can be stacked. For this operation
     to be defined the following must be true :
 
     #. all inputs must be valid dataset objects,
     #. units of data and axis must be compatible (rescaling is applied
        automatically if necessary).
 
     Parameters
     ----------
-    *datasets : a series of |NDDataset|
+    *datasets : a series of `NDDataset`
         The dataset to be stacked to the current dataset.
 
     Returns
     --------
     out
-        A |NDDataset| created from the stack of the `datasets` datasets.
+        A `NDDataset` created from the stack of the `datasets` datasets.
 
     See Also
     --------
-    concatenate : Concatenate |NDDataset| objects along a given dimension.
+    concatenate : Concatenate `NDDataset` objects along a given dimension.
 
     Examples
     --------
 
     >>> A = scp.read('irdata/nh4y-activation.spg', protocol='omnic')
     >>> B = scp.read('irdata/nh4y-activation.scp')
     >>> C = scp.stack(A, B)
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/processors/fft.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/fft.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,26 +223,26 @@
     The data in the last dimension MUST be in frequency (or without dimension)
     or an error is raised.
 
     To make direct Fourier transform, i.e., from frequency to time domain, use the `fft` transform.
 
     Parameters
     ----------
-    dataset : |NDDataset|
+    dataset : `NDDataset`
         The dataset on which to apply the fft transformation.
     size : int, optional
-        Size of the transformed dataset dimension - a shorter parameter is `si`. by default, the size is the closest
+        Size of the transformed dataset dimension - a shorter parameter is `si` . by default, the size is the closest
         power of two greater than the data size.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     -------
     out
-        Transformed |NDDataset| .
+        Transformed `NDDataset` .
 
     Other Parameters
     ----------------
     dim : str or int, optional, default='x'.
         Specify on which dimension to apply this method. If `dim` is specified as an integer it is equivalent
         to the usual `axis` numpy parameter.
     inplace : bool, optional, default=False.
@@ -266,33 +266,33 @@
     or an error is raised.
 
     To make reverse Fourier transform, i.e., from frequency to time domain, use the `ifft` transform
     (or equivalently, the `inv=True` parameters.
 
     Parameters
     ----------
-    dataset : |NDDataset|
+    dataset : `NDDataset`
         The dataset on which to apply the fft transformation.
     size : int, optional
-        Size of the transformed dataset dimension - a shorter parameter is `si`. by default, the size is the closest
+        Size of the transformed dataset dimension - a shorter parameter is `si` . by default, the size is the closest
         power of two greater than the data size.
     sizeff : int, optional
         The number of effective data point to take into account for the transformation. By default it is equal to the
         data size, but may be smaller.
     inv : bool, optional, default=False
         If True, an inverse Fourier transform is performed - size parameter is not taken into account.
     ppm : bool, optional, default=True
         If True, and data are from NMR, then a ppm scale is calculated instead of frequency.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     -------
     out
-        Transformed |NDDataset| .
+        Transformed `NDDataset` .
 
     Other Parameters
     ----------------
     dim : str or int, optional, default='x'.
         Specify on which dimension to apply this method. If `dim` is specified as an integer it is equivalent
         to the usual `axis` numpy parameter.
     inplace : bool, optional, default=False.
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/processors/integrate.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/integrate.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 __dataset_methods__ = ["simps", "trapz", "simpson", "trapezoid"]
 
 import functools
 
 import scipy.integrate
 
-from spectrochempy.utils import exceptions
+from spectrochempy.utils.decorators import deprecated
 
 
 def _integrate_method(method):
     @functools.wraps(method)
     def wrapper(dataset, *args, **kwargs):
 
         # handle the various syntax to pass the axis
@@ -75,118 +75,119 @@
 
 
 @_integrate_method
 def trapezoid(dataset, **kwargs):
     """
     Integrate using the composite trapezoidal rule.
 
-    Wrapper of scpy.integrate.trapezoid.
+    Wrapper of `scpy.integrate.trapezoid`\ .
 
     Performs the integration along the last or given dimension.
 
     Parameters
     ----------
-    dataset : |NDDataset|
+    dataset : `NDDataset`
         Dataset to be integrated.
     **kwargs
-        Additional keywords parameters.
-        See Other Parameters.
+        Additional keywords parameters. See Other Parameters.
 
     Returns
     -------
-    integral
+    `~spectrochempy.core.dataset.ndataset.NDDataset`
         Definite integral as approximated by trapezoidal rule.
 
     Other Parameters
     ----------------
-    dim : int or str, optional, default: "x"
-        Dimension along which to integrate.       If an integer is provided, it is equivalent to the `axis` parameter for numpy arrays.
+    dim : `int` or `str`, optional, default: ``"x"``
+        Dimension along which to integrate.
+        If an integer is provided, it is equivalent to the numpy axis
+        parameter for `~numpy.ndarray`\ s.
 
     See Also
     --------
-    trapz : An alias of trapezoid.
-
-    simps : Integrate using the composite simpson rule.
+    trapz : An alias of `trapezoid`.
+    simpson : Integrate using the composite simpson rule.
 
     Example
-    --------
+    -------
     >>> dataset = scp.read('irdata/nh4y-activation.spg')
     >>> dataset[:,1250.:1800.].trapz()
     NDDataset: [float64] a.u..cm^-1 (size: 55)
     """
 
     return scipy.integrate.trapz(dataset, **kwargs)
 
 
-@exceptions.deprecated(replace="Trapezoid")
+@deprecated(replace="Trapezoid")
 def trapz(dataset, **kwargs):
     return trapezoid(dataset, **kwargs)
 
 
 trapz.__doc__ = f"""
-An alias of `trapezoid` kept for backwards compatibility.
+    An alias of `trapezoid` kept for backwards compatibility.
 {trapezoid.__doc__}"""
 
 
 @_integrate_method
 def simpson(dataset, *args, **kwargs):
     """
     Integrate using the composite Simpson's rule.
 
-    Wrapper of scpy.integrate.trapezoid.
+    Wrapper of `scpy.integrate.simpson`.
 
     Performs the integration along the last or given dimension.
 
-    If there are an even number of samples, N, then there are an odd
-    number of intervals (N-1), but Simpson's rule requires an even number
+    If there are an even number of samples, ``N``, then there are an odd
+    number of intervals (``N-1``), but Simpson's rule requires an even number
     of intervals. The parameter 'even' controls how this is handled.
 
     Parameters
     ----------
-    dataset : |NDDataset|
+    dataset : `NDDataset`
         Dataset to be integrated.
     **kwargs
-        Additional keywords parameters.
-        See Other Parameters.
+        Additional keywords parameters. See Other Parameters.
 
     Returns
     -------
-    integral
+    `~spectrochempy.core.dataset.ndataset.NDDataset`
         Definite integral as approximated using the composite Simpson's rule.
 
     Other Parameters
     ----------------
-    dim : int or str, optional, default: "x"
+    dim : `int` or `str`, optional, default: ``"x"``
         Dimension along which to integrate.
-        If an integer is provided, it is equivalent to the `axis` parameter for numpy arrays.
-    even : str {'avg', 'first', 'last'}, optional, default is 'avg'
-        'avg' : Average two results: 1) use the first N-2 intervals with
-                  a trapezoidal rule on the last interval and 2) use the last
-                  N-2 intervals with a trapezoidal rule on the first interval.
-        'first' : Use Simpson's rule for the first N-2 intervals with
-                a trapezoidal rule on the last interval.
-        'last' : Use Simpson's rule for the last N-2 intervals with a
-               trapezoidal rule on the first interval.
+        If an integer is provided, it is equivalent to the `numpy.axis` parameter
+        for `~numpy.ndarray`\ s.
+    even : any of [``'avg'``\ , ``'first'``\ , ``'last'``\ }, optional, default: ``'avg'``
+
+        * ``'avg'`` : Average two results: 1) use the first N-2 intervals with
+          a trapezoidal rule on the last interval and 2) use the last
+          ``N-2`` intervals with a trapezoidal rule on the first interval.
+        * ``'first'`` : Use Simpson's rule for the first ``N-2`` intervals with
+          a trapezoidal rule on the last interval.
+        * ``'last'`` : Use Simpson's rule for the last ``N-2`` intervals with a
+          trapezoidal rule on the first interval.
 
     See Also
     --------
-    simps : An alias of simpson.
+    simps : An alias of simpson (Deprecated).
     trapezoid : Integrate using the composite simpson rule.
 
     Example
     --------
 
     >>> dataset = scp.read('irdata/nh4y-activation.spg')
     >>> dataset[:,1250.:1800.].simps()
     NDDataset: [float64] a.u..cm^-1 (size: 55)
     """
     return scipy.integrate.simps(dataset.data, **kwargs)
 
 
-@exceptions.deprecated(replace="simpson")
+@deprecated(replace="simpson")
 def simps(dataset, **kwargs):
     return simpson(dataset, **kwargs)
 
 
-simps__doc__ = f"""
-An alias of `Simpson` kept for backwards compatibility.
+simps.__doc__ = f"""
+    An alias of `simpson` kept for backwards compatibility.
 {trapezoid.__doc__}"""
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/processors/interpolate.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/interpolate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/core/processors/phasing.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/phasing.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,21 +137,21 @@
     For multidimensional NDDataset,
     the phase is by default applied on the last dimension.
 
     Parameters
     ----------
     dataset : nddataset
         Input dataset.
-    phc0 : float or |Quantity| , optional, default=0 degree
+    phc0 : float or `Quantity` , optional, default=0 degree
         Zero order phase in degrees.
-    phc1 : float or |Quantity| , optional, default=0 degree
+    phc1 : float or `Quantity` , optional, default=0 degree
         First order phase in degrees.
-    exptc : float or |Quantity| , optional, default=0 us
+    exptc : float or `Quantity` , optional, default=0 us
         Exponential decay constant. If not 0, phc1 is ignored.
-    pivot: float or |Quantity| , optional, default=0 in units of the x coordinate
+    pivot: float or `Quantity` , optional, default=0 in units of the x coordinate
         Units if any must be compatible with last dimension units.
 
     Returns
     -------
     phased
         Dataset.
 
@@ -190,17 +190,17 @@
     For multidimensional NDDataset,
     the phase is by default applied on the last dimension.
 
     Parameters
     ----------
     dataset : nddataset
         Input dataset.
-    phc0 : float or |Quantity| , optional, default=0 degree
+    phc0 : float or `Quantity` , optional, default=0 degree
         Zero order phase in degrees.
-    exptc : float or |Quantity| , optional, default=0 us
+    exptc : float or `Quantity` , optional, default=0 us
         Exponential decay constant.
 
     Returns
     -------
     phased
         Dataset.
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/processors/shift.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/shift.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,16 @@
     dataset : nddataset
         NDDataset to be left-shifted.
     pts : int
         Number of points to right shift.
 
     Returns
     -------
-    dataset
-        dataset left shifted and zero filled.
+    `NDDataset`
+        Modified dataset.
 
     Other Parameters
     ----------------
     dim : str or int, keyword parameter, optional, default='x'
         Specify on which dimension to apply the shift method. If `dim` is specified as an integer it is equivalent
         to the usual `axis` numpy parameter.
     inplace : bool, keyword parameter, optional, default=False
@@ -194,15 +194,15 @@
     pts : float
         Number of points to frequency shift the data.  Positive value will
         shift the spectrum to the right, negative values to the left.
 
     Returns
     -------
     dataset
-        dataset shifted
+        dataset shifted.
 
     Other Parameters
     ----------------
     dim : str or int, keyword parameter, optional, default='x'
         Specify on which dimension to apply the shift method. If `dim` is specified as an integer it is equivalent
         to the usual `axis` numpy parameter.
     inplace : bool, keyword parameter, optional, default=False
@@ -238,15 +238,15 @@
     pts : float
         Number of points to frequency shift the data.  Positive value will
         shift the spectrum to the right, negative values to the left.
 
     Returns
     -------
     dataset
-        dataset shifted
+        dataset shifted.
 
     Other Parameters
     ----------------
     dim : str or int, keyword parameter, optional, default='x'
         Specify on which dimension to apply the shift method. If `dim` is specified as an integer it is equivalent
         to the usual `axis` numpy parameter.
     inplace : bool, keyword parameter, optional, default=False
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/processors/smooth.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/smooth.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     This method is based on the convolution of a scaled window with the signal.
     The signal is prepared by introducing reflected copies of the signal (with the window size) in both ends so that
     transient parts are minimized in the beginning and end part of the output data.
 
     Parameters
     ----------
-    dataset :  |NDDataset| or a ndarray-like object
+    dataset :  `NDDataset` or a ndarray-like object
         Input object.
     window_length :  int, optional, default=5
         The dimension of the smoothing window; must be an odd integer.
     window : str, optional, default='flat'
         The type of window from 'flat', 'hanning', 'hamming', 'bartlett', 'blackman'.
         flat window will produce a moving average smoothing.
     **kwargs
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/processors/utils.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/utils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/core/processors/zero_filling.py` & `spectrochempy-0.6.1/spectrochempy/core/processors/zero_filling.py`

 * *Files 8% similar despite different names*

```diff
@@ -140,25 +140,25 @@
 @_zf_method
 def zf_size(dataset, size=None, mid=False, **kwargs):
     """
     Zero fill to given size.
 
     Parameters
     ----------
-    dataset : ndarray
-        Array of NMR data.
+    dataset : `NDDataset`
+        Input dataset.
     size : int
         Size of data after zero filling.
     mid : bool
         True to zero fill in the middle of data.
 
     Returns
     -------
-    ndata : ndarray
-        Zero filled array of NMR data.
+    `NDDataset`
+        Modified dataset.
     """
     if size is None:
         size = dataset.shape[-1]
     return _zf_pad(dataset, pad=int(size - dataset.shape[-1]), mid=mid)
 
 
 def zf_auto(dataset, mid=False):
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/project/abstractproject.py` & `spectrochempy-0.6.1/spectrochempy/core/project/abstractproject.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/core/project/project.py` & `spectrochempy-0.6.1/spectrochempy/core/project/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,36 +25,37 @@
 # cfg = config_manager
 # preferences = preferences
 
 
 # ======================================================================================
 # Project class
 # ======================================================================================
+@tr.signature_has_traits
 class Project(AbstractProject, NDIO):
     """
     A manager for projects, datasets and scripts.
 
     It can handle multiple datasets, subprojects, and scripts in a main
     project.
 
     Parameters
     ----------
     *args : Series of objects, optional
         Argument type will be interpreted correctly if they are of type
-        |NDDataset| , |Project| , or other objects such as |Script| .
+        `NDDataset` ,  `Project` , or other objects such as `Script` .
         This is optional, as they can be added later.
     argnames : list, optional
         If not None, this list gives the names associated to each
         object passed as args. It MUST be the same length that the
         number of args, or an error will be raised.
         If None, the internal name of each object will be used instead.
     name : str, optional
         The name of the project.  If the name is not provided, it will be
         generated automatically.
-    **meta : dict
+    \**meta : dict
         Any other attributes to describe the project.
 
     See Also
     --------
     NDDataset : The main object containing arrays.
     Script : Executables scripts container.
 
@@ -408,15 +409,15 @@
 
     # ----------------------------------------------------------------------------------
     # Public methods
     # ----------------------------------------------------------------------------------
     @staticmethod
     def _implements(name=None):
         """
-        Utility to check if the current object implement `Project`.
+        Utility to check if the current object implement `Project` .
 
         Rather than isinstance(obj, Project) use object._implements('Project').
         This is useful to check type without importing the module.
         """
         if name is None:
             return "Project"
         else:
@@ -433,15 +434,15 @@
     # ----------------------------------------------------------------------------------
     def add_datasets(self, *datasets):
         """
         Add several datasets to the current project.
 
         Parameters
         ----------
-        *datasets : series of |NDDataset|
+        *datasets : series of `NDDataset`
             Datasets to add to the current project.
             The name of the entries in the project will be identical to the
             names of the datasets.
 
         See Also
         --------
         add_dataset : Add a single dataset to the current project.
@@ -460,15 +461,15 @@
 
     def add_dataset(self, dataset, name=None):
         """
         Add a single dataset to the current project.
 
         Parameters
         ----------
-        dataset : |NDDataset|
+        dataset : `NDDataset`
             Datasets to add.
             The name of the entry will be the name of the dataset, except
             if parameter `name` is defined.
         name : str, optional
             If provided the name will be used to name the entry in the project.
 
         See Also
@@ -572,26 +573,26 @@
     # ----------------------------------------------------------------------------------
     def add_scripts(self, *scripts):
         """
         Add one or a series of scripts to the current project.
 
         Parameters
         ----------
-        scripts : |Script| instances
+        scripts : `Script` instances
         """
         for sc in scripts:
             self.add_script(sc)
 
     def add_script(self, script, name=None):
         """
         Add one script to the current project.
 
         Parameters
         ----------
-        script : a |Script| instance
+        script : a `Script` instance
         name : str
         """
         script.parent = self
         if name is None:
             name = script.name
         else:
             script.name = name
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/readers/api.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/core/readers/download.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/download.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 In this module, methods are provided to download external datasets
 from public database.
 """
-__all__ = ["download_iris", "download_nist_ir"]
+__all__ = ["download_iris", "download_nist_ir", "download"]
 __dataset_methods__ = __all__
 
+import shutil
 from io import StringIO
 from pathlib import Path
 
 import numpy as np
 import requests
 
 from spectrochempy.core import error_, info_
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.dataset.nddataset import NDDataset
+from spectrochempy.core.readers.importer import read
 from spectrochempy.core.readers.read_jcamp import read_jcamp
 from spectrochempy.utils.misc import is_iterable
 from spectrochempy.utils.optional import import_optional_dependency
 
 
 def download_iris():
     """
@@ -120,16 +122,16 @@
 
     Parameters
     ----------
     CAS : int or str
         the CAS number, can be given as "XXXX-XX-X" (str), "XXXXXXX" (str), XXXXXXX (int)
 
     index : str or int or tuple of ints
-        If set to 'all' (default, import all available spectra for the compound corresponding to the index, or a single spectrum,
-        or selected spectra.
+        If set to 'all' (default, import all available spectra for the compound
+        corresponding to the index, or a single spectrum, or selected spectra.
 
     Returns
     -------
     list of NDDataset or NDDataset
         The dataset(s).
 
     See Also
@@ -214,10 +216,55 @@
 
     if len(out) == 1:
         return out[0]
     else:
         return out
 
 
+def download(url):
+    """
+    Download data from an url
+
+    Parameters
+    ----------
+    url : str
+        url to a readable file
+
+    Returns
+    -------
+    list of NDDataset or NDDataset
+        The dataset(s).
+
+    See Also
+    --------
+    read : Read data from experimental data.
+    """
+
+    # https://stackoverflow.com/questions/16694907/download-large-file-in-python-with-requests
+
+    local_filename = url.split("/")[-1]
+
+    try:
+        response = requests.get(url, stream=True, timeout=10)
+    except OSError:
+        error_("OSError: could not connect")
+        return None
+
+    with response as r:
+        r.raise_for_status()
+        with open(local_filename, "wb") as f:
+            shutil.copyfileobj(r.raw, f)
+            ds = read(local_filename)
+
+            if isinstance(ds, NDDataset):
+                ds.history = f"Downloaded from {url}"
+            elif isinstance(ds, list):
+                for ds_ in ds:
+                    ds_.history = f"Downloaded from {url}"
+
+    Path(local_filename).unlink()
+    return ds
+
+
 # ======================================================================================
 if __name__ == "__main__":
     pass
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/readers/read_carroucell.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/read_carroucell.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,23 +52,23 @@
     delta_clocks : int, optional, default=0
         Difference in seconds between the clocks used for spectra and temperature acquisition.
         Defined as t(thermocouple clock) - t(spectrometer clock).
 
     Returns
     --------
     nddataset
-        |NDDataset| or list of |NDDataset| .
+        `NDDataset` or list of `NDDataset` .
 
     See Also
     --------
     read_topspin : Read TopSpin Bruker NMR spectra.
     read_omnic : Read Omnic spectra.
     read_opus : Read OPUS spectra.
-    read_spg : Read Omnic *.spg grouped spectra.
-    read_spa : Read Omnic *.Spa single spectra.
+    read_spg : Read Omnic .spg grouped spectra.
+    read_spa : Read Omnic .spa single spectra.
     read_srs : Read Omnic series.
     read_csv : Read CSV files.
     read_zip : Read Zip files.
     read_matlab : Read Matlab files.
 
     Notes
     ------
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/readers/read_csv.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/read_matlab.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,291 +1,290 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
-__all__ = ["read_csv"]
+"""
+Plugin module to extend NDDataset with the import methods method.
+"""
+
+__all__ = ["read_matlab", "read_mat"]
 __dataset_methods__ = __all__
 
-# --------------------------------------------------------------------------------------
-# standard and other imports
-# --------------------------------------------------------------------------------------
 import io
-import locale
-import warnings
 from datetime import datetime
+from warnings import warn
 
 import numpy as np
+import scipy.io as sio
 
-from spectrochempy.core import preferences as prefs
-from spectrochempy.core.dataset.coord import Coord
+from spectrochempy.core.dataset.nddataset import Coord, NDDataset
 from spectrochempy.core.readers.importer import Importer, _importer_method
 
-try:
-    locale.setlocale(locale.LC_ALL, "en_US")  # to avoid problems with date format
-except Exception:  # pragma: no cover
-    try:
-        locale.setlocale(
-            locale.LC_ALL, "en_US.utf8"
-        )  # to avoid problems with date format
-    except Exception:
-        warnings.warn("Could not set locale: en_US or en_US.utf8")
-
 
 # ======================================================================================
 # Public functions
 # ======================================================================================
-def read_csv(*paths, **kwargs):
+def read_matlab(*paths, **kwargs):
     """
-    Open a *.csv file or a list of *.csv files.
+    Read a matlab file with extension ` .mat` and return its content as a list.
 
-    This is limited to 1D array - csv file must have two columns [index, data]
-    without header.
+    The array of numbers (i.e. matlab matrices) and Eigenvector's DataSet Object (DSO, see
+    `DSO <https://www.eigenvector.com/software/dataset.htm>`_ ) are returned as NDDatasets.  The
+    content not recognized by SpectroChemPy is returned as a tuple (name, object).
 
     Parameters
-    ----------
+    -----------
     *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
         The data source(s) can be specified by the name or a list of name for the file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e. no `filename`, nor `content`),
+        except if `merge` is set to False. If a source is not provided (i.e. no `filename` , nor `content` ),
         a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
-    read_csv
-        |NDDataset| or list of |NDDataset| .
+    read_matlab
+        `NDDataset` or list of `NDDataset` .
 
     Other Parameters
     ----------------
+    protocol : {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel'}, optional
+        Protocol used for reading. If not provided, the correct protocol
+        is inferred (whnever it is possible) from the file name extension.
     directory : str, optional
-        From where to read the specified `filename`. If not specified, read in the default ``datadir`` specified in
+        From where to read the specified `filename` . If not specified, read in the default `datadir` specified in
         SpectroChemPy Preferences.
     merge : bool, optional
         Default value is False. If True, and several filenames have been provided as arguments,
         then a single dataset with merged (stacked along the first
-        dimension) is returned (default=False).
-    sortbydate : bool, optional
-        Sort multiple spectra by acquisition date (default=True).
+        dimension) is returned (default=False)
     description: str, optional
         A Custom description.
-    origin : {'omnic', 'tga'}, optional
-        in order to properly interpret CSV file it can be necessary to set the origin of the spectra.
-        Up to now only 'omnic' and 'tga' have been implemented.
-    csv_delimiter : str, optional
-        Set the column delimiter in CSV file.
-        By default it is the one set in SpectroChemPy ``Preferences``.
     content : bytes object, optional
         Instead of passing a filename for further reading, a bytes content can be directly provided as bytes objects.
         The most convenient way is to use a dictionary. This feature is particularly useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the ``tests/tests_readers`` directory.
+        For examples on how to use this feature, one can look in the `tests/tests_readers` directory
     listdir : bool, optional
         If True and filename is None, all files present in the provided `directory` are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current reading protocol (default=True).
+        is True. It is assumed that all the files correspond to current reading protocol (default=True)
     recursive : bool, optional
-        Read also in subfolders. (default=False).
+        Read also in subfolders. (default=False)
+
+    Examples
+    ---------
+
+    >>> scp.read_matlab('matlabdata/dso.mat')
+    NDDataset: [float64] unitless (shape: (y:20, x:426))
 
+    See `read_omnic` for more examples of use
     See Also
     --------
+    read : Read generic files.
     read_topspin : Read TopSpin Bruker NMR spectra.
     read_omnic : Read Omnic spectra.
     read_opus : Read OPUS spectra.
-    read_spg : Read Omnic *.spg grouped spectra.
-    read_spa : Read Omnic *.Spa single spectra.
+    read_labspec : Read Raman LABSPEC spectra.
+    read_spg : Read Omnic .spg grouped spectra.
+    read_spa : Read Omnic .spa single spectra.
     read_srs : Read Omnic series.
+    read_csv : Read CSV files.
     read_zip : Read Zip files.
-    read_matlab : Read Matlab files.
-    read : Generic file reading.
-
-    Examples
-    ---------
-
-    >>> scp.read_csv('agirdata/P350/TGA/tg.csv')
-    NDDataset: [float64] unitless (shape: (y:1, x:3247))
-
-    Additional information can be stored in the dataset if the origin is given
-    (known origin for now : tga or omnic)
-    # TODO: define some template to allow adding new origins
-
-    >>> scp.read_csv('agirdata/P350/TGA/tg.csv', origin='tga')
-    NDDataset: [float64] wt.% (shape: (y:1, x:3247))
-
-    Sometimes the delimiteur needs to be adjusted
-
-    >>> prefs = scp.preferences
-    >>> scp.read_csv('irdata/IR.CSV', directory=prefs.datadir, origin='omnic', csv_delimiter=',')
-    NDDataset: [float64] a.u. (shape: (y:1, x:3736))
     """
-    kwargs["filetypes"] = ["CSV files (*.csv)"]
-    kwargs["protocol"] = ["csv"]
+    kwargs["filetypes"] = ["MATLAB files (*.mat *.dso)"]
+    kwargs["protocol"] = ["matlab", "mat", "dso"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
-# ======================================================================================
-# Private functions
-# ======================================================================================
-@_importer_method
-def _read_csv(*args, **kwargs):
-    # read csv file
-    dataset, filename = args
-    content = kwargs.get("content", None)
-    delimiter = kwargs.get("csv_delimiter", prefs.csv_delimiter)
-
-    def _open():
-        if content is not None:
-            f = io.StringIO(content.decode("utf-8"))
-        else:
-            f = open(filename, "r")
-        return f
+read_mat = read_matlab
 
-    try:
-        fid = _open()
-        d = np.loadtxt(fid, unpack=True, delimiter=delimiter)
-        fid.close()
-    except ValueError:
-        # it might be that the delimiter is not correct (default is ','), but
-        # french excel export with the french locale for instance, use ";".
-        _delimiter = ";"
-        try:
-            fid = _open()
-            if fid:
-                fid.close()
-            fid = _open()
-            d = np.loadtxt(fid, unpack=True, delimiter=_delimiter)
-            fid.close()
-
-        except Exception:  # pragma: no cover
-            # in french, very often the decimal '.' is replaced by a
-            # comma:  Let's try to correct this
-            if fid:
-                fid.close()
-            if not isinstance(fid, io.StringIO):
-                with open(fid, "r") as fid_:
-                    txt = fid_.read()
-            else:
-                txt = fid.read()
-            txt = txt.replace(",", ".")
-            fil = io.StringIO(txt)
-            try:
-                d = np.loadtxt(fil, unpack=True, delimiter=delimiter)
-            except Exception:
-                raise IOError(
-                    "{} is not a .csv file or its structure cannot be recognized"
-                )
-
-    # First column is the x coordinates
-    coordx = Coord(d[0])
-
-    # create a second coordinate for dimension y of size 1
-    coordy = Coord([0])
-
-    # and data is the second column -  we make it a vector
-    data = d[1].reshape((1, coordx.size))
-
-    # update the dataset
-    dataset.data = data
-    dataset.set_coordset(y=coordy, x=coordx)
-
-    # set the additional attributes
-    name = filename.stem
-    dataset.filename = filename
-    dataset.name = kwargs.get("name", name)
-    dataset.title = kwargs.get("title", None)
-    dataset.units = kwargs.get("units", None)
-    dataset.description = kwargs.get("description", '"name" ' + "read from .csv file")
-    dataset.history = "Read from .csv file"
-
-    # here we can check some particular format
-    origin = kwargs.get("origin", "")
-    if "omnic" in origin:
-        # this will be treated as csv export from omnic (IR data)
-        dataset = _add_omnic_info(dataset, **kwargs)
-    elif "tga" in origin:
-        # this will be treated as csv export from tga analysis
-        dataset = _add_tga_info(dataset, **kwargs)
-    elif origin:
-        raise NotImplementedError(
-            f"Sorry, but reading a csv file with '{origin}' origin is not implemented. "
-            "Please, remove or set the keyword 'origin'\n "
-            "(Up to now implemented csv files are: `omnic`, `tga`)"
-        )
 
-    # reset modification date to cretion date
-    dataset._modified = dataset._created
+# --------------------------------------------------------------------------------------
+# Private methods
+# --------------------------------------------------------------------------------------
+@_importer_method
+def _read_mat(*args, **kwargs):
+    _, filename = args
+    content = kwargs.get("content", False)
+
+    if content:
+        fid = io.BytesIO(content)
+    else:
+        fid = open(filename, "rb")
+
+    dic = sio.loadmat(fid)
+
+    datasets = []
+    for name, data in dic.items():
+
+        dataset = NDDataset()
+        if name == "__header__":
+            dataset.description = str(data, "utf-8", "ignore")
+            continue
+        if name.startswith("__"):
+            continue
+
+        if data.dtype in [
+            np.dtype("float64"),
+            np.dtype("float32"),
+            np.dtype("int8"),
+            np.dtype("int16"),
+            np.dtype("int32"),
+            np.dtype("int64"),
+            np.dtype("uint8"),
+            np.dtype("uint16"),
+            np.dtype("uint32"),
+            np.dtype("uint64"),
+        ]:
+
+            # this is an array of numbers
+            dataset.data = data
+            dataset.name = name
+            dataset.history = "Imported from .mat file"
+            # TODO: reshape from fortran/Matlab order to C opder
+            # for 3D or higher datasets ?
+            datasets.append(dataset)
+
+        elif data.dtype.char == "U":
+            # this is an array of string
+            warn(
+                f"The mat file contains an array of strings named '{name}' which will not be converted to NDDataset"
+            )
+            continue
+
+        elif all(
+            name_ in data.dtype.names for name_ in ["moddate", "axisscale", "imagesize"]
+        ):
+            # this is probably a DSO object
+            dataset = _read_dso(dataset, name, data)
+            datasets.append(dataset)
 
-    return dataset
+        else:
+            warn(f"unsupported data type : {data.dtype}")
+            # TODO: implement DSO reader
+            datasets.append([name, data])
 
+    return datasets
 
-def _add_omnic_info(dataset, **kwargs):
-    # get the time and name
-    name = desc = dataset.name
-
-    # modify the dataset metadata
-    dataset.units = "absorbance"
-    dataset.title = "absorbance"
-    dataset.name = name
-    dataset.description = "Dataset from .csv file: {}\n".format(desc)
-    dataset.history = "Read from omnic exported csv file."
-    dataset.origin = "omnic"
-
-    # x axis
-    dataset.x.units = "cm^-1"
-
-    # y axis ?
-    if "_" in name:
-        name, dat = name.split("_")
-        # if needed convert weekday name to English
-        dat = dat.replace("Lun", "Mon")
-        dat = dat[:3].replace("Mar", "Tue") + dat[3:]
-        dat = dat.replace("Mer", "Wed")
-        dat = dat.replace("Jeu", "Thu")
-        dat = dat.replace("Ven", "Fri")
-        dat = dat.replace("Sam", "Sat")
-        dat = dat.replace("Dim", "Sun")
-        # convert month name to English
-        dat = dat.replace("Aout", "Aug")
-
-        # get the dates
-        acqdate = datetime.strptime(dat, "%a %b %d %H-%M-%S %Y")
-
-        # Transform back to timestamp for storage in the Coord object
-        # use datetime.fromtimestamp(d, timezone.utc))
-        # to transform back to datetime obkct
-        timestamp = acqdate.timestamp()
-
-        dataset.y = Coord(np.array([timestamp]), name="y")
-        dataset.set_coordtitles(y="acquisition timestamp (GMT)", x="wavenumbers")
-        dataset.y.labels = np.array([[acqdate], [name]])
-        dataset.y.units = "s"
 
-    # reset modification date to cretion date
-    dataset._modified = dataset._created
+@_importer_method
+def _read_dso(dataset, name, data):
+    name_mat = data["name"][0][0]
+    if len(name_mat) == 0:
+        name = ""
+    else:
+        name = name_mat[0]
+
+    typedata_mat = data["type"][0][0]
+    if len(typedata_mat) == 0:
+        typedata = ""
+    else:
+        typedata = typedata_mat[0]
+
+    if typedata != "data":
+        return (name, data)
+
+    else:
+        author_mat = data["author"][0][0]
+        if len(author_mat) == 0:
+            author = "*unknown*"
+        else:
+            author = author_mat[0]
 
-    return dataset
+        date_mat = data["date"][0][0]
+        if len(date_mat) == 0:
+            date = datetime(1, 1, 1, 0, 0)
+        else:
+            date = datetime(
+                int(date_mat[0][0]),
+                int(date_mat[0][1]),
+                int(date_mat[0][2]),
+                int(date_mat[0][3]),
+                int(date_mat[0][4]),
+                int(date_mat[0][5]),
+            )
+
+        dat = data["data"][0][0]
+
+        # look at coords and labels
+        # only the first label and axisscale are taken into account
+        # the axisscale title is used as the coordinate title
+
+        coords = []
+        for i in range(len(dat.shape)):
+            coord = datac = None  # labels = title = None
+            labelsarray = data["label"][0][0][i][0]
+            if len(labelsarray):  # some labels might be present
+                if isinstance(labelsarray[0], np.ndarray):
+                    labels = data["label"][0][0][i][0][0]
+                else:
+                    labels = data["label"][0][0][i][0]
+                if len(labels):
+                    coord = Coord(labels=[str(label) for label in labels])
+                if len(data["label"][0][0][i][1]):
+                    if isinstance(data["label"][0][0][i][1][0], np.ndarray):
+                        if len(data["label"][0][0][i][1][0]):
+                            coord.name = data["label"][0][0][i][1][0][0]
+                    elif isinstance(data["label"][0][0][i][1][0], str):
+                        coord.name = data["label"][0][0][i][1][0]
+
+            axisdataarray = data["axisscale"][0][0][i][0]
+            if len(axisdataarray):  # some axiscale might be present
+                if isinstance(axisdataarray[0], np.ndarray):
+                    if len(axisdataarray[0]) == dat.shape[i]:
+                        datac = axisdataarray[0]  # take the first axiscale data
+                    elif axisdataarray[0].size == dat.shape[i]:
+                        datac = axisdataarray[0][0]
+
+                if datac is not None:
+                    if isinstance(coord, Coord):
+                        coord.data = datac
+                    else:
+                        coord = Coord(data=datac)
+
+                if len(data["axisscale"][0][0][i][1]):  # some titles might be present
+                    try:
+                        coord.title = data["axisscale"][0][0][i][1][0]
+                    except Exception:
+                        try:
+                            coord.title = data["axisscale"][0][0][i][1][0][0]
+                        except Exception:
+                            pass
+
+            if not isinstance(coord, Coord):
+                coord = Coord(data=[j for j in range(dat.shape[i])], title="index")
+
+            coords.append(coord)
+
+        dataset.data = dat
+        dataset.set_coordset(*[coord for coord in coords])
+        dataset.author = author
+        dataset.name = name
+        dataset.date = date
+
+        # TODO: reshape from fortran/Matlab order to C order
+        #  for 3D or higher datasets ?
 
+        for i in data["description"][0][0]:
+            dataset.description += i
 
-def _add_tga_info(dataset, **kwargs):
-    # for TGA, some information are needed.
-    # we add them here
-    dataset.x.units = "hour"
-    dataset.units = "weight_percent"
-    dataset.x.title = "time-on-stream"
-    dataset.title = "mass change"
-    dataset.origin = "tga"
+        for i in data["history"][0][0][0][0]:
+            dataset.history = i
 
+        dataset.history = "Imported by spectrochempy."
     return dataset
 
 
 # --------------------------------------------------------------------------------------
 if __name__ == "__main__":
     pass
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/readers/read_jcamp.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/read_jcamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,102 +15,102 @@
 import re
 from datetime import datetime, timezone
 
 import numpy as np
 
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.readers.importer import Importer, _importer_method
-from spectrochempy.utils import exceptions
+from spectrochempy.utils.decorators import deprecated
 
 
 # ======================================================================================
 # Public functions
 # ======================================================================================
 def read_jcamp(*paths, **kwargs):
     """
-    Open Infrared JCAMP-DX files with extension ``.jdx`` or ``.dx``.
+    Open Infrared JCAMP-DX files with extension ` .jdx` or ` .dx` .
 
     Limited to AFFN encoding (see R. S. McDonald and Paul A. Wilks,
     JCAMP-DX: A Standard Form for Exchange of Infrared Spectra in Computer Readable Form,
     Appl. Spec., 1988, 1, 151–162. doi:10.1366/0003702884428734.)
 
     Parameters
     ----------
     *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
         The data source(s) can be specified by the name or a list of name for the file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e. no `filename`, nor `content`),
+        except if `merge` is set to False. If a source is not provided (i.e. no `filename` , nor `content` ),
         a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     read_jcamp
-        |NDDataset| or list of |NDDataset| .
+        `NDDataset` or list of `NDDataset` .
 
     Other Parameters
     ----------------
     protocol : {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel'}, optional
         Protocol used for reading. If not provided, the correct protocol
         is inferred (whnever it is possible) from the file name extension.
     directory : str, optional
-        From where to read the specified `filename`. If not specified, read in the default ``datadir`` specified in
+        From where to read the specified `filename` . If not specified, read in the default `datadir` specified in
         SpectroChemPy Preferences.
     merge : bool, optional
         Default value is False. If True, and several filenames have been provided as arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False).
     sortbydate : bool, optional
         Sort multiple spectra by acquisition date (default=True).
     description: str, optional
         A Custom description.
     content : bytes object, optional
         Instead of passing a filename for further reading, a bytes content can be directly provided as bytes objects.
         The most convenient way is to use a dictionary. This feature is particularly useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the ``tests/tests_readers`` directory.
+        For examples on how to use this feature, one can look in the `tests/tests_readers` directory.
     listdir : bool, optional
         If True and filename is None, all files present in the provided `directory` are returned (and merged if `merge`
         is True. It is assumed that all the files correspond to current reading protocol (default=True).
     recursive : bool, optional
         Read also in subfolders. (default=False).
 
     See Also
     ---------
     read : Generic read method.
     read_topspin : Read TopSpin Bruker NMR spectra.
     read_omnic : Read Omnic spectra.
     read_opus : Read OPUS spectra.
-    read_spg : Read Omnic *.spg grouped spectra.
-    read_spa : Read Omnic *.Spa single spectra.
+    read_spg : Read Omnic .spg grouped spectra.
+    read_spa : Read Omnic .spa single spectra.
     read_srs : Read Omnic series.
     read_csv : Read CSV files.
     read_zip : Read Zip files.
     read_matlab : Read Matlab files.
     """
     kwargs["filetypes"] = ["JCAMP-DX files (*.jdx *.dx)"]
     kwargs["protocol"] = ["jcamp"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
-@exceptions.deprecated(replace="read__jcamp")
+@deprecated(replace="read__jcamp")
 def read_jdx(*args, **kwargs):
     return read_jcamp(*args, **kwargs)
 
 
-@exceptions.deprecated(replace="read_jcamp")
+@deprecated(replace="read_jcamp")
 def read_dx(*args, **kwargs):  # pragma: no cover
     return read_jcamp(*args, **kwargs)
 
 
 # ======================================================================================
 # private functions
 # ======================================================================================
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/readers/read_labspec.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/read_labspec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
-This module extend NDDataset with the import method for Labspec *.txt generated data files.
+This module extend NDDataset with the import method for Labspec \*.txt generated data files.
 """
 
 __all__ = ["read_labspec"]
 __dataset_methods__ = __all__
 
 import datetime
 
@@ -23,73 +23,81 @@
 # ======================================================================================
 # Public functions
 # ======================================================================================
 def read_labspec(*paths, **kwargs):
     """
     Read a single Raman spectrum or a series of Raman spectra.
 
-    Files to open are *.txt file created by Labspec software. Non-labspec .txt files are ignored (return None)
+    Files to open are .txt file created by Labspec software. Non-labspec .txt files
+    are ignored (return None)
 
     Parameters
     ----------
     *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
-        The data source(s) can be specified by the name or a list of name for the file(s) to be loaded:
+        The data source(s) can be specified by the name or a list of name for the
+        file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e. no `filename`, nor `content`),
-        a dialog box will be opened to select files.
+        except if `merge` is set to False. If a source is not provided (i.e. no
+        `filename` , nor `content` ), a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     read
-        |NDDataset| or list of |NDDataset| or None.
+        `NDDataset` or list of `NDDataset` or None.
 
     Other Parameters
     ----------------
     protocol : {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel'}, optional
         Protocol used for reading. If not provided, the correct protocol
         is inferred (whnever it is possible) from the file name extension.
     directory : str, optional
-        From where to read the specified `filename`. If not specified, read in the default ``datadir`` specified in
-        SpectroChemPy Preferences.
+        From where to read the specified `filename` . If not specified, read in the
+        default `datadir` specified in SpectroChemPy Preferences.
     merge : bool, optional
-        Default value is False. If True, and several filenames have been provided as arguments,
+        Default value is False. If True, and several filenames have been provided as
+        arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False)
     sortbydate : bool, optional
         Sort multiple spectra by acquisition date (default=True)
     description: str, optional
         A Custom description.
     content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content can be directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is particularly useful for a GUI Dash application
+        Instead of passing a filename for further reading, a bytes content can be
+        directly provided as bytes objects.
+        The most convenient way is to use a dictionary. This feature is particularly
+        useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the ``tests/tests_readers`` directory
+        For examples on how to use this feature, one can look in the
+        `tests/tests_readers` directory
     listdir : bool, optional
-        If True and filename is None, all files present in the provided `directory` are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current reading protocol (default=True)
+        If True and filename is None, all files present in the provided `directory`
+        are returned (and merged if `merge`
+        is True. It is assumed that all the files correspond to current reading protocol
+        (default=True)
     recursive : bool, optional
         Read also in subfolders. (default=False).
 
     See Also
     --------
     read : Generic read method.
     read_topspin : Read TopSpin Bruker NMR spectra.
     read_omnic : Read Omnic spectra.
     read_opus : Read OPUS spectra.
-    read_spg : Read Omnic *.spg grouped spectra.
-    read_spa : Read Omnic *.Spa single spectra.
+    read_spg : Read Omnic .spg grouped spectra.
+    read_spa : Read Omnic .spa single spectra.
     read_srs : Read Omnic series.
     read_csv : Read CSV files.
     read_zip : Read Zip files.
     read_matlab : Read Matlab files.
 
     Examples
     --------
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/readers/read_omnic.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/read_omnic.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 # ======================================================================================
 # Public functions
 # ======================================================================================
 def read_omnic(*paths, **kwargs):
     """
     Open a Thermo Nicolet OMNIC file.
 
-    Open Omnic file or a list of files with extension ``.spg`` , ``.spa`` or
-    ``.srs`` and set data/metadata in the current dataset.
+    Open Omnic file or a list of files with extension ` .spg` , ` .spa` or
+    ` .srs` and set data/metadata in the current dataset.
 
     The collected metadata are:
     - names of spectra
     - acquisition dates (UTC)
     - units of spectra (absorbance, transmittance, reflectance, Log(1/R),
     Kubelka-Munk, Raman intensity, photoacoustics, volts)
     - units of xaxis (wavenumbers in cm^-1, wavelengths in nm or micrometer,
@@ -51,38 +51,38 @@
 
     Parameters
     -----------
     *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
         The data source(s) can be specified by the name or a list of name
         for the file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
         except if `merge` is set to False. If a source is not provided (i.e.
-        no `filename`, nor `content`),
+        no `filename` , nor `content` ),
         a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     out
         The dataset or a list of dataset corresponding to a (set of) .spg,
         .spa or .srs file(s).
 
     Other Parameters
     -----------------
     directory : str, optional
-        From where to read the specified `filename`. If not specified,
-        read in the default ``datadir`` specified in
+        From where to read the specified `filename` . If not specified,
+        read in the default `datadir` specified in
         SpectroChemPy Preferences.
     merge : bool, optional
         Default value is False. If True, and several filenames have been
         provided as arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False).
     sortbydate : bool, optional
@@ -92,15 +92,15 @@
     content : bytes object, optional
         Instead of passing a filename for further reading, a bytes content
         can be directly provided as bytes objects.
         The most convenient way is to use a dictionary. This feature is
         particularly useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
         For examples on how to use this feature, one can look in the
-        ``tests/tests_readers`` directory.
+        `tests/tests_readers` directory.
     listdir : bool, optional
         If True and filename is None, all files present in the provided
         `directory` are returned (and merged if `merge`
         is True. It is assumed that all the files correspond to current
         reading protocol (default=True).
     recursive : bool, optional
         Read also in subfolders. (default=False).
@@ -117,21 +117,21 @@
     read_csv : Read .csv.
     read_matlab : Read MATLAB files .mat.
     read_zip : Read zipped group of files.
 
     Examples
     ---------
     Reading a single OMNIC file  (providing a windows type filename relative
-    to the default ``datadir``)
+    to the default `datadir` )
 
     >>> scp.read_omnic('irdata\\\\nh4y-activation.spg')
     NDDataset: [float64] a.u. (shape: (y:55, x:5549))
 
     Reading a single OMNIC file  (providing a unix/python type filename
-    relative to the default ``datadir``)
+    relative to the default `datadir` )
     Note that here read_omnic is called as a classmethod of the NDDataset class
 
     >>> scp.NDDataset.read_omnic('irdata/nh4y-activation.spg')
     NDDataset: [float64] a.u. (shape: (y:55, x:5549))
 
     Single file specified with pathlib.Path object
 
@@ -211,49 +211,49 @@
     kwargs["protocol"] = ["omnic", "spa", "spg", "srs"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
 def read_spg(*paths, **kwargs):
     """
-    Open a Thermo Nicolet file or a list of files with extension ``.spg``.
+    Open a Thermo Nicolet file or a list of files with extension ` .spg` .
 
-    Open Omnic file or a list of files with extension ``.spg`` and set
+    Open Omnic file or a list of files with extension ` .spg` and set
     data/metadata in the current dataset.
 
     Parameters
     -----------
     *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
         The data source(s) can be specified by the name or a list of name
         for the file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
         except if `merge` is set to False. If a source is not provided (i.e.
-        no `filename`, nor `content`),
+        no `filename` , nor `content` ),
         a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     read_spg
         The dataset or a list of dataset corresponding to a (set of) .spg
         file(s).
 
     Other Parameters
     -----------------
     directory : str, optional
-        From where to read the specified `filename`. If not specified,
-        read in the default ``datadir`` specified in
+        From where to read the specified `filename` . If not specified,
+        read in the default `datadir` specified in
         SpectroChemPy Preferences.
     merge : bool, optional
         Default value is False. If True, and several filenames have been
         provided as arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False).
     sortbydate : bool, optional
@@ -263,39 +263,39 @@
     content : bytes object, optional
         Instead of passing a filename for further reading, a bytes content
         can be directly provided as bytes objects.
         The most convenient way is to use a dictionary. This feature is
         particularly useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
         For examples on how to use this feature, one can look in the
-        ``tests/tests_readers`` directory.
+        `tests/tests_readers` directory.
     listdir : bool, optional
         If True and filename is None, all files present in the provided
         `directory` are returned (and merged if `merge`
         is True. It is assumed that all the files correspond to current
         reading protocol (default=True).
     recursive : bool, optional
         Read also in subfolders. (default=False).
 
     See Also
     --------
     read : Generic read method.
     read_dir : Read a set of data from a directory.
     read_omnnic : Read Omnic files.
-    read_spa : Read Omnic files *.spa.
-    read_srs : Read Omnic files *.srs.
+    read_spa : Read Omnic files .spa.
+    read_srs : Read Omnic files .srs.
     read_opus : Read Bruker OPUS files.
     read_topspin : Read TopSpin NMR files.
-    read_csv : Read *.csv.
-    read_matlab : Read MATLAB files *.mat.
+    read_csv : Read .csv.
+    read_matlab : Read MATLAB files .mat.
     read_zip : Read zipped group of files.
 
     Notes
     -----
-    This method is an alias of ``read_omnic``, except that the type of file
+    This method is an alias of `read_omnic`\ , except that the type of file
     is contrain to *.spg.
 
     Examples
     ---------
 
     >>> scp.read_spg('irdata/nh4y-activation.spg')
     NDDataset: [float64] a.u. (shape: (y:55, x:5549))
@@ -305,34 +305,34 @@
     kwargs["protocol"] = ["spg", "spa"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
 def read_spa(*paths, **kwargs):
     """
-    Open a Thermo Nicolet file or a list of files with extension ``.spa``.
+    Open a Thermo Nicolet file or a list of files with extension ` .spa` .
 
-    Open Omnic file or a list of files with extension ``.spa`` and set
+    Open Omnic file or a list of files with extension ` .spa` and set
     data/metadata in the current dataset.
 
     Parameters
     -----------
     *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
         The data source(s) can be specified by the name or a list of name
         for the file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
         except if `merge` is set to False. If a source is not provided (i.e.
-        no `filename`, nor `content`),
+        no `filename` , nor `content` ),
         a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     read_spa
@@ -342,16 +342,16 @@
     Other Parameters
     -----------------
     return_ifg : str or None, optional
         Default value is None. When set to 'sample' returns the sample interferogram
         of the spa file if present or None if absent. When set to 'backgroung' returns
         the backgroung interferogram of the spa file if present or None if absent.
     directory : str, optional
-        From where to read the specified `filename`. If not specified,
-        read in the default ``datadir`` specified in
+        From where to read the specified `filename` . If not specified,
+        read in the default `datadir` specified in
         SpectroChemPy Preferences.
     merge : bool, optional
         Default value is False. If True, and several filenames have been
         provided as arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False).
     sortbydate : bool, optional
@@ -361,15 +361,15 @@
     content : bytes object, optional
         Instead of passing a filename for further reading, a bytes content
         can be directly provided as bytes objects.
         The most convenient way is to use a dictionary. This feature is
         particularly useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
         For examples on how to use this feature, one can look in the
-        ``tests/tests_readers`` directory.
+        `tests/tests_readers` directory.
     listdir : bool, optional
         If True and filename is None, all files present in the provided
         `directory` are returned (and merged if `merge`
         is True. It is assumed that all the files correspond to current
         reading protocol (default=True).
     recursive : bool, optional
         Read also in subfolders. (default=False).
@@ -377,23 +377,23 @@
     See Also
     --------
     read : Generic read method.
     read_topspin : Read TopSpin Bruker NMR spectra.
     read_omnic : Read Omnic spectra.
     read_opus : Read OPUS spectra.
     read_labspec : Read Raman LABSPEC spectra.
-    read_spg : Read Omnic *.spg grouped spectra.
+    read_spg : Read Omnic \*.spg grouped spectra.
     read_srs : Read Omnic series.
     read_csv : Read CSV files.
     read_zip : Read Zip files.
     read_matlab : Read Matlab files.
 
     Notes
     -----
-    This method is an alias of ``read_omnic``, except that the type of file
+    This method is an alias of `read_omnic`\ , except that the type of file
     is contrain to *.spa.
 
     Examples
     ---------
 
     >>> scp.read_spa('irdata/subdir/20-50/7_CZ0-100 Pd_21.SPA')
     NDDataset: [float64] a.u. (shape: (y:1, x:5549))
@@ -405,34 +405,34 @@
     kwargs["protocol"] = ["spa"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
 def read_srs(*paths, **kwargs):
     """
-    Open a Thermo Nicolet file or a list of files with extension ``.srs``.
+    Open a Thermo Nicolet file or a list of files with extension `.srs` .
 
-    Open Omnic file or a list of files with extension ``.srs`` and set
+    Open Omnic file or a list of files with extension `.srs` and set
     data/metadata in the current dataset.
 
     Parameters
     -----------
     *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
         The data source(s) can be specified by the name or a list of name
         for the file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
         except if `merge` is set to False. If a source is not provided (i.e.
-        no `filename`, nor `content`),
+        no `filename` , nor `content` ),
         a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     NDDataset
@@ -440,16 +440,16 @@
         or backgroun files.
 
     Other Parameters
     -----------------
     return_bg : bool, optional
         Default value is False. When set to 'True' returns the series background
     directory : str, optional
-        From where to read the specified `filename`. If not specified,
-        read in the default ``datadir`` specified in
+        From where to read the specified `filename` . If not specified,
+        read in the default `datadir` specified in
         SpectroChemPy Preferences.
     merge : bool, optional
         Default value is False. If True, and several filenames have been
         provided as arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False).
     sortbydate : bool, optional
@@ -459,15 +459,15 @@
     content : bytes object, optional
         Instead of passing a filename for further reading, a bytes content
         can be directly provided as bytes objects.
         The most convenient way is to use a dictionary. This feature is
         particularly useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
         For examples on how to use this feature, one can look in the
-        ``tests/tests_readers`` directory.
+        `tests/tests_readers` directory.
     listdir : bool, optional
         If True and filename is None, all files present in the provided
         `directory` are returned (and merged if `merge`
         is True. It is assumed that all the files correspond to current
         reading protocol (default=True)
     recursive : bool, optional
         Read also in subfolders. (default=False).
@@ -475,23 +475,23 @@
     See Also
     --------
     read : Generic read method.
     read_topspin : Read TopSpin Bruker NMR spectra.
     read_omnic : Read Omnic spectra.
     read_opus : Read OPUS spectra.
     read_labspec : Read Raman LABSPEC spectra.
-    read_spg : Read Omnic *.spg grouped spectra.
-    read_spa : Read Omnic *.Spa single spectra.
+    read_spg : Read Omnic \*.spg grouped spectra.
+    read_spa : Read Omnic \*.Spa single spectra.
     read_csv : Read CSV files.
     read_zip : Read Zip files.
     read_matlab : Read Matlab files.
 
     Notes
     -----
-    This method is an alias of ``read_omnic``, except that the type of file
+    This method is an alias of `read_omnic`\ , except that the type of file
     is constrained to *.srs.
 
     Examples
     ---------
     >>> scp.read_srs('irdata/omnic_series/rapid_scan_reprocessed.srs')
     NDDataset: [float64] a.u. (shape: (y:643, x:3734))
     """
@@ -702,14 +702,21 @@
     _x = LinearCoord(
         offset=firstx[0],
         increment=spacing,
         size=int(nx[0]),
         title=xtitles[0],
         units=xunits[0],
     )
+    # _x = Coord.linspace(
+    #     firstx[0],
+    #     lastx[0],
+    #     int(nx[0]),
+    #     title=xtitles[0],
+    #     units=xunits[0],
+    # )
 
     _y = Coord(
         timestamps,
         title="acquisition timestamp (GMT)",
         units="s",
         labels=(acquisitiondates, spectitles),
     )
@@ -879,14 +886,21 @@
         firstx = info["firstx"]
         lastx = info["lastx"]
         xunit = info["xunits"]
         xtitle = info["xtitle"]
 
         spacing = (lastx - firstx) / (nx - 1)
 
+        # _x = Coord.linspace(
+        #     firstx,
+        #     lastx,
+        #     int(nx),
+        #     title=xtitle,
+        #     units=xunit,
+        # )
         _x = LinearCoord(
             offset=firstx, increment=spacing, size=nx, title=xtitle, units=xunit
         )
 
     else:  # interferogram
         if return_ifg == "sample":
             default_description = (
@@ -900,14 +914,20 @@
         _x = LinearCoord(
             offset=0,
             increment=1,
             size=len(intensities),
             title="data points",
             units=None,
         )
+        #
+        # _x = Coord.arange(
+        #     len(intensities),
+        #     title="data points",
+        #     units=None,
+        # )
 
     dataset.set_coordset(y=_y, x=_x)
     dataset.name = spa_name  # to be consistent with omnic behaviour
     dataset.filename = str(filename)
 
     # Set origin, description, history, date
     # Omnic spg file don't have specific "origin" field stating the oirigin of the data
@@ -1060,14 +1080,21 @@
 
     dataset.units = info["units"]
     dataset.title = info["title"]
     dataset.origin = "omnic"
 
     # now add coordinates
     spacing = (info["lastx"] - info["firstx"]) / (info["nx"] - 1)
+    # _x = Coord.linspace(
+    #     info["firstx"],
+    #     info["lastx"],
+    #     int(info["nx"]),
+    #     title=info["xtitle"],
+    #     units=info["xunits"],
+    # )
     _x = LinearCoord(
         offset=info["firstx"],
         increment=spacing,
         size=info["nx"],
         title=info["xtitle"],
         units=info["xunits"],
     )
@@ -1218,30 +1245,36 @@
     -------
         dict, int
         Dictionary and current position in file
 
     Notes
     -----
         So far, the header structure is as follows:
+
         - starts with b'\x01' , b'\x02', b'\x03' ... maybe indicating the header "type"
         - nx (UInt32): 4 bytes behind
         - xunits (UInt8): 8 bytes behind. So far, we have the following correspondence:
-            `x\01`: wavenumbers, cm-1
-            `x\02`: datapoints (interferogram)
-            `x\03`: wavelength, nm
-            `x\04': wavelength, um
-            `x\20': Raman shift, cm-1
-        - data units (UInt8): 12 bytes behind. So far, we have the following correspondence:
-            `x\11`: absorbance
-            `x\10`: transmittance (%)
-            `x\0B`: reflectance (%)
-            `x\0C`: Kubelka_Munk
-            `x\16`:  Volts (interferogram)
-            `x\1A`:  photoacoustic
-            `x\1F`: Raman intensity
+
+            * `x\01` : wavenumbers, cm-1
+            * `x\02` : datapoints (interferogram)
+            * `x\03` : wavelength, nm
+            * `x\04' : wavelength, um
+            * `x\20' : Raman shift, cm-1
+
+        - data units (UInt8): 12 bytes behind. So far, we have the following
+          correspondence:
+
+            * `x\11` : absorbance
+            * `x\10` : transmittance (%)
+            * `x\0B` : reflectance (%)
+            * `x\0C` : Kubelka_Munk
+            * `x\16` :  Volts (interferogram)
+            * `x\1A` :  photoacoustic
+            * `x\1F` : Raman intensity
+
         - first x value (float32), 16 bytes behind
         - last x value (float32), 20 bytes behind
         - ... unknown
         - scan points (UInt32), 28 bytes behind
         - zpd (UInt32),  32 bytes behind
         - number of scans (UInt32), 36 bytes behind
         - ... unknown
@@ -1252,20 +1285,21 @@
         - reference frequency (float32), 80 bytes behind
         - ...
         - optical velocity (float32), 188 bytes behind
         - ...
         - spectrum history (text), 208 bytes behind
 
         For "rapid-scan" srs files:
+
         - series name (text), 938 bytes behind
         - collection length (float32), 1002 bytes behind
         - last y (float 32), 1006 bytes behind
         - first y (float 32), 1010 bytes behind
         - ny (UInt32), 1026
-        ... y unit could be at pos+1030 with 01 = minutes ?
+        - ... y unit could be at pos+1030 with 01 = minutes ?
         - history (text), 1200 bytes behind (only initila hgistopry.
            When reprocessed, updated history is at the end of the file after the
            b`\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF` sequence
     """
 
     out = {}
     # determine the type of file
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/readers/read_opus.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/read_opus.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,22 +32,22 @@
     extracted ("AB" field). Returns an error if dimensions are incompatibles.
 
     Parameters
     -----------
     *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
         The data source(s) can be specified by the name or a list of name for the file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e. no `filename`, nor `content`),
+        except if `merge` is set to False. If a source is not provided (i.e. no `filename` , nor `content` ),
         a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     read_opus
@@ -55,56 +55,56 @@
 
     Other Parameters
     -----------------
     protocol : {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel'}, optional
         Protocol used for reading. If not provided, the correct protocol
         is inferred (whnever it is possible) from the file name extension.
     directory : str, optional
-        From where to read the specified `filename`. If not specified, read in the default ``datadir`` specified in
+        From where to read the specified `filename` . If not specified, read in the default `datadir` specified in
         SpectroChemPy Preferences.
     merge : bool, optional
         Default value is False. If True, and several filenames have been provided as arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False).
     sortbydate : bool, optional
         Sort multiple spectra by acquisition date (default=True).
     description: str, optional
         A Custom description.
     content : bytes object, optional
         Instead of passing a filename for further reading, a bytes content can be directly provided as bytes objects.
         The most convenient way is to use a dictionary. This feature is particularly useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the ``tests/tests_readers`` directory.
+        For examples on how to use this feature, one can look in the `tests/tests_readers` directory.
     listdir : bool, optional
         If True and filename is None, all files present in the provided `directory` are returned (and merged if `merge`
         is True. It is assumed that all the files correspond to current reading protocol (default=True).
     recursive : bool, optional
         Read also in subfolders. (default=False).
 
     See Also
     --------
     read : Generic read method.
     read_topspin : Read TopSpin Bruker NMR spectra.
     read_omnic : Read Omnic spectra.
     read_labspec : Read Raman LABSPEC spectra.
-    read_spg : Read Omnic *.spg grouped spectra.
-    read_spa : Read Omnic *.Spa single spectra.
+    read_spg : Read Omnic \*.spg grouped spectra.
+    read_spa : Read Omnic \*.Spa single spectra.
     read_srs : Read Omnic series.
     read_csv : Read CSV files.
     read_zip : Read Zip files.
     read_matlab : Read Matlab files.
 
     Examples
     ---------
-    Reading a single OPUS file  (providing a windows type filename relative to the default ``Datadir``)
+    Reading a single OPUS file  (providing a windows type filename relative to the default `Datadir` )
 
     >>> scp.read_opus('irdata\\\\OPUS\\\\test.0000')
     NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
-    Reading a single OPUS file  (providing a unix/python type filename relative to the default ``Datadir``)
+    Reading a single OPUS file  (providing a unix/python type filename relative to the default `Datadir` )
     Note that here read_opus is called as a classmethod of the NDDataset class
 
     >>> scp.NDDataset.read_opus('irdata/OPUS/test.0000')
     NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
     Single file specified with pathlib.Path object
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/readers/read_quadera.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/read_quadera.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,81 +23,88 @@
 
 
 # ======================================================================================
 # Public functions
 # ======================================================================================
 def read_quadera(*paths, **kwargs):
     """
-    Read a Pfeiffer Vacuum's QUADERA® mass spectrometer software file with extension ``.asc``.
+    Read a Pfeiffer Vacuum's QUADERA mass spectrometer software file with extension `.asc` .
 
     Parameters
     -----------
-    *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
+    paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
         The data source(s) can be specified by the name or a list of name for the file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        - e.g.,( file1, file2, ...,  **kwargs )
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        - e.g., ( [file1, file2, ... ], **kwargs )
 
         The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e. no `filename`, nor `content`),
+        except if `merge` is set to False. If a source is not provided (i.e. no `filename` , nor `content` ),
         a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
-    read_quadera
-        |NDDataset| or list of |NDDataset| .
+    `NDDataset` or list of `NDDataset` .
 
     Other Parameters
     ----------------
     timestamp: bool, optional
         returns the acquisition timestamp as Coord (Default=True).
         If set to false, returns the time relative to the acquisition time of the data
     protocol : {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel', 'asc'}, optional
         Protocol used for reading. If not provided, the correct protocol
         is inferred (whnever it is possible) from the file name extension.
     directory : str, optional
-        From where to read the specified `filename`. If not specified, read in the default ``datadir`` specified in
+        From where to read the specified `filename` . If not specified, read in the
+        default `datadir` specified in
         SpectroChemPy Preferences.
     merge : bool, optional
-        Default value is False. If True, and several filenames have been provided as arguments,
+        Default value is False. If True, and several filenames have been provided as
+        arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False)
     description: str, optional
         A Custom description.
     content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content can be directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is particularly useful for a GUI Dash application
+        Instead of passing a filename for further reading, a bytes content can be
+        directly provided as bytes objects.
+        The most convenient way is to use a dictionary. This feature is particularly
+        useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the ``tests/tests_readers`` directory
+        For examples on how to use this feature, one can look in the
+        `tests/tests_readers` directory
     listdir : bool, optional
-        If True and filename is None, all files present in the provided `directory` are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current reading protocol (default=True)
+        If True and filename is None, all files present in the provided `directory` are
+        returned (and merged if `merge`
+        is True. It is assumed that all the files correspond to current reading protocol
+        (default=True)
     recursive : bool, optional
         Read also in subfolders. (default=False)
 
     Notes
     ------
-    Currently the acquisition time is that of the first channel as the timeshift of other channels are typically
+    Currently the acquisition time is that of the first channel as the timeshift of
+    other channels are typically
     within few seconds, and the data of other channels are NOT interpolated
     Todo: check with users whether data interpolation should be made
 
     See Also
     --------
     read : Read generic files.
     read_topspin : Read TopSpin Bruker NMR spectra.
     read_omnic : Read Omnic spectra.
     read_opus : Read OPUS spectra.
     read_labspec : Read Raman LABSPEC spectra.
-    read_spg : Read Omnic *.spg grouped spectra.
-    read_spa : Read Omnic *.Spa single spectra.
+    read_spg : Read Omnic \*.spg grouped spectra.
+    read_spa : Read Omnic \*.spa single spectra.
     read_srs : Read Omnic series.
     read_csv : Read CSV files.
     read_zip : Read Zip files.
 
     Examples
     ---------
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/readers/read_soc.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/read_soc.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,45 +16,45 @@
 
 
 # ======================================================================================
 # Public function
 # ======================================================================================
 def read_soc(*paths, **kwargs):
     """
-    Open a Surface Optics Corps. file or a list of files with extension ``.ddr``, ``.hdr`` or ``.sdr``.
+    Open a Surface Optics Corps. file or a list of files with extension `.ddr` , `.hdr` or `.sdr`\ .
 
     Parameters
     -----------
     *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
         The data source(s) can be specified by the name or a list of name
         for the file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
         except if `merge` is set to False. If a source is not provided (i.e.
-        no `filename`, nor `content`),
+        no `filename` , nor `content` ),
         a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     read_soc
         The dataset or a list of dataset corresponding to a (set of) file(s).
 
     Other Parameters
     -----------------
     directory : str, optional
-        From where to read the specified `filename`. If not specified,
-        read in the default ``datadir`` specified in
+        From where to read the specified `filename` . If not specified,
+        read in the default `datadir` specified in
         SpectroChemPy Preferences.
     merge : bool, optional
         Default value is False. If True, and several filenames have been
         provided as arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False).
     sortbydate : bool, optional
@@ -64,15 +64,15 @@
     content : bytes object, optional
         Instead of passing a filename for further reading, a bytes content
         can be directly provided as bytes objects.
         The most convenient way is to use a dictionary. This feature is
         particularly useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
         For examples on how to use this feature, one can look in the
-        ``tests/tests_readers`` directory.
+        `tests/tests_readers` directory.
     listdir : bool, optional
         If True and filename is None, all files present in the provided
         `directory` are returned (and merged if `merge`
         is True. It is assumed that all the files correspond to current
         reading protocol (default=True).
     recursive : bool, optional
         Read also in subfolders. (default=False).
@@ -80,16 +80,16 @@
     See Also
     --------
     read : Generic read method.
     read_topspin : Read TopSpin Bruker NMR spectra.
     read_omnic : Read Omnic spectra.
     read_opus : Read OPUS spectra.
     read_labspec : Read Raman LABSPEC spectra.
-    read_spa : Read Omnic *.spa spectra.
-    read_spg : Read Omnic *.spg grouped spectra.
+    read_spa : Read Omnic \*.spa spectra.
+    read_spg : Read Omnic \*.spg grouped spectra.
     read_srs : Read Omnic series.
     read_csv : Read CSV files.
     read_zip : Read Zip files.
     read_matlab : Read Matlab files.
 
     Examples
     ---------
@@ -100,34 +100,34 @@
     kwargs["protocol"] = ["soc", "ddr", "hdr", "sdr"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
 def read_ddr(*paths, **kwargs):
     """
-    Open a Surface Optics Corps. file or a list of files with extension ``.ddr``.
+    Open a Surface Optics Corps. file or a list of files with extension ` .ddr` .
 
-    Open Surface Optics Corps. file or a list of files with extension ``.ddr`` and set
+    Open Surface Optics Corps. file or a list of files with extension ` .ddr` and set
     data/metadata in the current dataset.
 
     Parameters
     -----------
     *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
         The data source(s) can be specified by the name or a list of name
         for the file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
         except if `merge` is set to False. If a source is not provided (i.e.
-        no `filename`, nor `content`),
+        no `filename` , nor `content` ),
         a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     read_ddr
@@ -137,16 +137,16 @@
     Other Parameters
     -----------------
     return_ifg : str or None, optional
         Default value is None. When set to 'sample' returns the sample interferogram
         of the spa file if present or None if absent. When set to 'background' returns
         the backgroung interferogram of the spa file if present or None if absent.
     directory : str, optional
-        From where to read the specified `filename`. If not specified,
-        read in the default ``datadir`` specified in
+        From where to read the specified `filename` . If not specified,
+        read in the default `datadir` specified in
         SpectroChemPy Preferences.
     merge : bool, optional
         Default value is False. If True, and several filenames have been
         provided as arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False).
     sortbydate : bool, optional
@@ -156,15 +156,15 @@
     content : bytes object, optional
         Instead of passing a filename for further reading, a bytes content
         can be directly provided as bytes objects.
         The most convenient way is to use a dictionary. This feature is
         particularly useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
         For examples on how to use this feature, one can look in the
-        ``tests/tests_readers`` directory.
+        `tests/tests_readers` directory.
     listdir : bool, optional
         If True and filename is None, all files present in the provided
         `directory` are returned (and merged if `merge`
         is True. It is assumed that all the files correspond to current
         reading protocol (default=True).
     recursive : bool, optional
         Read also in subfolders. (default=False).
@@ -182,34 +182,34 @@
     kwargs["protocol"] = ["ddr"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
 def read_hdr(*paths, **kwargs):
     """
-    Open a Surface Optics Corps. file or a list of files with extension ``.hdr``.
+    Open a Surface Optics Corps. file or a list of files with extension ` .hdr` .
 
-    Open Surface Optics Corps. file or a list of files with extension ``.hdr`` and set
+    Open Surface Optics Corps. file or a list of files with extension ` .hdr` and set
     data/metadata in the current dataset.
 
     Parameters
     -----------
     *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
         The data source(s) can be specified by the name or a list of name
         for the file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
         except if `merge` is set to False. If a source is not provided (i.e.
-        no `filename`, nor `content`),
+        no `filename` , nor `content` ),
         a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     read_ddr
@@ -219,16 +219,16 @@
     Other Parameters
     -----------------
     return_ifg : str or None, optional
         Default value is None. When set to 'sample' returns the sample interferogram
         of the spa file if present or None if absent. When set to 'background' returns
         the backgroung interferogram of the spa file if present or None if absent.
     directory : str, optional
-        From where to read the specified `filename`. If not specified,
-        read in the default ``datadir`` specified in
+        From where to read the specified `filename` . If not specified,
+        read in the default `datadir` specified in
         SpectroChemPy Preferences.
     merge : bool, optional
         Default value is False. If True, and several filenames have been
         provided as arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False).
     sortbydate : bool, optional
@@ -238,15 +238,15 @@
     content : bytes object, optional
         Instead of passing a filename for further reading, a bytes content
         can be directly provided as bytes objects.
         The most convenient way is to use a dictionary. This feature is
         particularly useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
         For examples on how to use this feature, one can look in the
-        ``tests/tests_readers`` directory.
+        `tests/tests_readers` directory.
     listdir : bool, optional
         If True and filename is None, all files present in the provided
         `directory` are returned (and merged if `merge`
         is True. It is assumed that all the files correspond to current
         reading protocol (default=True).
     recursive : bool, optional
         Read also in subfolders. (default=False).
@@ -264,34 +264,34 @@
     kwargs["protocol"] = ["hdr"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
 def read_sdr(*paths, **kwargs):
     """
-    Open a Surface Optics Corps. file or a list of files with extension ``.sdr``.
+    Open a Surface Optics Corps. file or a list of files with extension ` .sdr` .
 
-    Open Surface Optics Corps. file or a list of files with extension ``.sdr`` and set
+    Open Surface Optics Corps. file or a list of files with extension ` .sdr` and set
     data/metadata in the current dataset.
 
     Parameters
     -----------
     *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
         The data source(s) can be specified by the name or a list of name
         for the file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
         except if `merge` is set to False. If a source is not provided (i.e.
-        no `filename`, nor `content`),
+        no `filename` , nor `content` ),
         a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     read_ddr
@@ -301,16 +301,16 @@
     Other Parameters
     -----------------
     return_ifg : str or None, optional
         Default value is None. When set to 'sample' returns the sample interferogram
         of the spa file if present or None if absent. When set to 'background' returns
         the backgroung interferogram of the spa file if present or None if absent.
     directory : str, optional
-        From where to read the specified `filename`. If not specified,
-        read in the default ``datadir`` specified in
+        From where to read the specified `filename` . If not specified,
+        read in the default `datadir` specified in
         SpectroChemPy Preferences.
     merge : bool, optional
         Default value is False. If True, and several filenames have been
         provided as arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False).
     sortbydate : bool, optional
@@ -320,15 +320,15 @@
     content : bytes object, optional
         Instead of passing a filename for further reading, a bytes content
         can be directly provided as bytes objects.
         The most convenient way is to use a dictionary. This feature is
         particularly useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
         For examples on how to use this feature, one can look in the
-        ``tests/tests_readers`` directory.
+        `tests/tests_readers` directory.
     listdir : bool, optional
         If True and filename is None, all files present in the provided
         `directory` are returned (and merged if `merge`
         is True. It is assumed that all the files correspond to current
         reading protocol (default=True).
     recursive : bool, optional
         Read also in subfolders. (default=False).
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/readers/read_spc.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/read_spc.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,46 +24,46 @@
 
 
 # ======================================================================================
 # Public function
 # ======================================================================================
 def read_spc(*paths, **kwargs):
     """
-    Open a Thermo Nicolet file or a list of files with extension ``.spg``.
+    Open a Thermo Nicolet file or a list of files with extension ` .spg` .
 
     Parameters
     -----------
     *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
         The data source(s) can be specified by the name or a list of name
         for the file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
         except if `merge` is set to False. If a source is not provided (i.e.
-        no `filename`, nor `content`),
+        no `filename` , nor `content` ),
         a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     read_spc
         The dataset or a list of dataset corresponding to a (set of) .spa
         file(s).
 
     Other Parameters
     -----------------
     directory : str, optional
-        From where to read the specified `filename`. If not specified,
-        read in the default ``datadir`` specified in
+        From where to read the specified `filename` . If not specified,
+        read in the default `datadir` specified in
         SpectroChemPy Preferences.
     merge : bool, optional
         Default value is False. If True, and several filenames have been
         provided as arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False).
     sortbydate : bool, optional
@@ -73,15 +73,15 @@
     content : bytes object, optional
         Instead of passing a filename for further reading, a bytes content
         can be directly provided as bytes objects.
         The most convenient way is to use a dictionary. This feature is
         particularly useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
         For examples on how to use this feature, one can look in the
-        ``tests/tests_readers`` directory.
+        `tests/tests_readers` directory.
     listdir : bool, optional
         If True and filename is None, all files present in the provided
         `directory` are returned (and merged if `merge`
         is True. It is assumed that all the files correspond to current
         reading protocol (default=True).
     recursive : bool, optional
         Read also in subfolders. (default=False).
@@ -89,16 +89,16 @@
     See Also
     --------
     read : Generic read method.
     read_topspin : Read TopSpin Bruker NMR spectra.
     read_omnic : Read Omnic spectra.
     read_opus : Read OPUS spectra.
     read_labspec : Read Raman LABSPEC spectra.
-    read_spa : Read Omnic *.spa spectra.
-    read_spg : Read Omnic *.spg grouped spectra.
+    read_spa : Read Omnic \*.spa spectra.
+    read_spg : Read Omnic \*.spg grouped spectra.
     read_srs : Read Omnic series.
     read_csv : Read CSV files.
     read_zip : Read Zip files.
     read_matlab : Read Matlab files.
 
     Examples
     ---------
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/readers/read_topspin.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/read_topspin.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from spectrochempy.core import debug_
 from spectrochempy.core.dataset.baseobjects.meta import Meta
 from spectrochempy.core.dataset.coord import LinearCoord
 from spectrochempy.core.readers.importer import Importer, _importer_method
 from spectrochempy.core.units import ur
 from spectrochempy.extern.nmrglue import read_fid, read_pdata
-from spectrochempy.utils import exceptions
+from spectrochempy.utils.decorators import deprecated
 
 # ======================================================================================
 # Constants
 # ======================================================================================
 FnMODE = ["undefined", "QF", "QSEQ", "TPPI", "STATES", "STATES-TPPI", "ECHO-ANTIECHO"]
 AQ_mod = ["QF", "QSIM", "QSEQ", "DQD"]
 
@@ -707,61 +707,69 @@
         Paths of the Bruker directories to read.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     read_topspin
-        |NDDataset| or list of |NDDataset| .
+        `NDDataset` or list of `NDDataset` .
 
     Other Parameters
     ----------------
     expno : int, optional
         experiment number.
     procno : int
         processing number.
     protocol : {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel'}, optional
         Protocol used for reading. If not provided, the correct protocol
         is inferred (whnever it is possible) from the file name extension.
     directory : str, optional
-        From where to read the specified `filename`. If not specified, read in the default ``datadir`` specified in
+        From where to read the specified `filename` . If not specified, read in the
+        default `datadir` specified in
         SpectroChemPy Preferences.
     merge : bool, optional
-        Default value is False. If True, and several filenames have been provided as arguments,
+        Default value is False. If True, and several filenames have been provided as
+        arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False).
     sortbydate : bool, optional
         Sort multiple spectra by acquisition date (default=True).
     description : str, optional
         A Custom description.
     origin : {'omnic', 'tga'}, optional
-        In order to properly interpret CSV file it can be necessary to set the origin of the spectra.
+        In order to properly interpret CSV file it can be necessary to set the origin
+        of the spectra.
         Up to now only 'omnic' and 'tga' have been implemented.
     csv_delimiter : str, optional
         Set the column delimiter in CSV file.
-        By default it is the one set in SpectroChemPy ``Preferences``.
+        By default it is the one set in SpectroChemPy `Preferences` .
     content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content can be directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is particularly useful for a GUI Dash application
+        Instead of passing a filename for further reading, a bytes content can be
+        directly provided as bytes objects.
+        The most convenient way is to use a dictionary. This feature is particularly
+        useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the ``tests/tests_readers`` directory.
+        For examples on how to use this feature, one can look in the
+        `tests/tests_readers` directory.
     listdir : bool, optional
-        If True and filename is None, all files present in the provided `directory` are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current reading protocol (default=True)
+        If True and filename is None, all files present in the provided `directory` are
+        returned (and merged if `merge`
+        is True. It is assumed that all the files correspond to current reading protocol
+        (default=True)
     recursive : bool, optional
         Read also in subfolders. (default=False)
 
     See Also
     --------
     read_topspin : Read TopSpin Bruker NMR spectra.
     read_omnic : Read Omnic spectra.
     read_opus : Read OPUS spectra.
     read_labspec : Read Raman LABSPEC spectra.
-    read_spg : Read Omnic *.spg grouped spectra.
-    read_spa : Read Omnic *.Spa single spectra.
+    read_spg : Read Omnic \*.spg grouped spectra.
+    read_spa : Read Omnic \*.Spa single spectra.
     read_srs : Read Omnic series.
     read_csv : Read CSV files.
     read_zip : Read Zip files.
     read_matlab : Read Matlab files.
     """
 
     kwargs["filetypes"] = [
@@ -769,15 +777,15 @@
         "Compressed TOPSPIN data directories (*.zip)",
     ]
     kwargs["protocol"] = ["topspin"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
-@exceptions.deprecated(replace="read_topspin")
+@deprecated(replace="read_topspin")
 def read_bruker_nmr(*args, **kwargs):
     return read_topspin(*args, **kwargs)
 
 
 def _get_files(path, typ="acqu"):
     files = []
     for i in ["", 2, 3]:
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/readers/read_zip.py` & `spectrochempy-0.6.1/spectrochempy/core/readers/read_zip.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,74 +18,84 @@
 def read_zip(*paths, **kwargs):
     """
     Open a zipped list of data files.
 
     Parameters
     ----------
     *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
-        The data source(s) can be specified by the name or a list of name for the file(s) to be loaded:
+        The data source(s) can be specified by the name or a list of name for the
+        file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  **kwargs )*
+        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, **kwargs *)*
+        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e. no `filename`, nor `content`),
+        except if `merge` is set to False. If a source is not provided (i.e. no `filename` , nor `content` ),
         a dialog box will be opened to select files.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
     --------
     read_zip
-        |NDDataset| or list of |NDDataset| .
+        `NDDataset` or list of `NDDataset` .
 
     Other Parameters
     ----------------
-    protocol : {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel'}, optional
+    protocol : 'str'\ , optional
+        One of {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel'}
         Protocol used for reading. If not provided, the correct protocol
-        is inferred (whnever it is possible) from the file name extension.
-    directory : str, optional
-        From where to read the specified `filename`. If not specified, read in the default ``datadir`` specified in
+        is inferred (whenever it is possible) from the file name extension.
+    directory : `str`\ , optional
+        From where to read the specified `filename`\ . If not specified, read in the
+        default ``datadir`` specified in
         SpectroChemPy Preferences.
-    merge : bool, optional
-        Default value is False. If True, and several filenames have been provided as arguments,
+    merge : `bool`, optional
+        Default value is False. If True, and several filenames have been provided as
+        arguments,
         then a single dataset with merged (stacked along the first
         dimension) is returned (default=False).
-    sortbydate : bool, optional
+    sortbydate : `bool`, optional
         Sort multiple spectra by acquisition date (default=True).
-    description: str, optional
+    description: `str`\ , optional
         A Custom description.
     origin : {'omnic', 'tga'}, optional
-        in order to properly interpret CSV file it can be necessary to set the origin of the spectra.
+        in order to properly interpret CSV file it can be necessary to set the origin
+        of the spectra.
         Up to now only 'omnic' and 'tga' have been implemented.
     csv_delimiter : str, optional
         Set the column delimiter in CSV file.
-        By default it is the one set in SpectroChemPy ``Preferences``.
+        By default it is the one set in SpectroChemPy `Preferences` .
     content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content can be directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is particularly useful for a GUI Dash application
+        Instead of passing a filename for further reading, a bytes content can be
+        directly provided as bytes objects.
+        The most convenient way is to use a dictionary. This feature is particularly
+        useful for a GUI Dash application
         to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the ``tests/tests_readers`` directory.
-    listdir : bool, optional
-        If True and filename is None, all files present in the provided `directory` are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current reading protocol (default=True).
-    recursive : bool, optional
-        Read also in subfolders. (default=False).
+        For examples on how to use this feature, one can look in the
+        ``tests/tests_readers`` directory.
+    listdir : `bool`, optional, default: `True`
+        If `True` and filename is None, all files present in the provided `directory`
+        are returned (and merged if `merge`
+        is True. It is assumed that all the files correspond to current
+        reading protocol.
+    recursive : bool, optional, default=False
+        Read also in subfolders.
 
     See Also
     --------
     read_topspin : Read TopSpin Bruker NMR spectra.
     read_omnic : Read Omnic spectra.
     read_opus : Read OPUS spectra.
     read_labspec : Read Raman LABSPEC spectra.
-    read_spg : Read Omnic *.spg grouped spectra.
-    read_spa : Read Omnic *.Spa single spectra.
+    read_spg : Read Omnic \*.spg grouped spectra.
+    read_spa : Read Omnic \*.Spa single spectra.
     read_srs : Read Omnic series.
     read_csv : Read CSV files.
     read_zip : Read Zip files.
     read_matlab : Read Matlab files.
 
     Examples
     --------
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/script/__init__.py` & `spectrochempy-0.6.1/spectrochempy/core/script/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,42 +3,51 @@
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 import ast
 import re
 
-from traitlets import Float, HasTraits, Instance, TraitError, Unicode, validate
+from traitlets import (
+    Float,
+    HasTraits,
+    Instance,
+    TraitError,
+    Unicode,
+    signature_has_traits,
+    validate,
+)
 
 from spectrochempy.core import error_
 from spectrochempy.core.project.abstractproject import AbstractProject
 
 __all__ = ["Script", "run_script", "run_all_scripts"]
 
 
+@signature_has_traits
 class Script(HasTraits):
     """
     Executable scripts.
 
     The scripts are used in a project.
 
     Parameters
     ----------
-    name : str
+    name : `str`
         Name of the script. The name should be unique.
-    content : str
+    content : `str`
         Content of sthe script.
-    parent : instance of |Project|
+    parent : instance of `Project`
         Parent project.
-    priority: int
-        Default=50.
+    priority: `int`, optional, default: 50
+        priority.
 
     See Also
     --------
-    Project: Object containing |NDDataset|s, sub-|Project|s and |Scripts| .
+    Project: Object containing `NDDataset`\'s, sub-\ `Project`\ 's and `Script`\ .
 
     Examples
     --------
     Make a script
 
     >>> s = "set_loglevel(INFO)"
     >>> s = "info_('Hello')"
@@ -50,15 +59,17 @@
     """
 
     _name = Unicode()
     _content = Unicode(allow_none=True)
     _priority = Float(min=0.0, max=100.0)
     _parent = Instance(AbstractProject, allow_none=True)
 
-    def __init__(self, name="unamed_script", content=None, parent=None, priority=50.0):
+    def __init__(
+        self, name="unamed_script", content=None, parent=None, priority=50.0, **kwargs
+    ):
 
         self.name = name
         self.content = content
         self.parent = parent
         self.priority = priority
 
     # ----------------------------------------------------------------------------------
@@ -137,15 +148,15 @@
 
     # ----------------------------------------------------------------------------------
     # Public methods
     # ----------------------------------------------------------------------------------
     @staticmethod
     def _implements(name=None):
         """
-        Utility to check if the current object implement `Project`.
+        Utility to check if the current object implement `Project` .
 
         Rather than isinstance(obj, Project) use object._implements('Project').
         This is useful to check type without importing the module
 
         Parameters
         ----------
         name : Object type name, optional
@@ -202,20 +213,20 @@
 
     Parameters
     ----------
     script : script instance
         The script to execute.
     localvars : dict, optional
         If provided it will be used for evaluating the script. In general,
-        it can be `localvrs`=``locals()``.
+        it can be `localvrs`=`locals()` .
 
     Returns
     -------
     out
-        Output of the script if any
+        Output of the script if any.
     """
 
     return script.execute(localvars)
 
 
 def run_all_scripts(project):
     """
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/units/__init__.py` & `spectrochempy-0.6.1/spectrochempy/core/units/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 )
 
 # check pint version
 pint_version = int(__version__.split(".")[1])
 if pint_version < 18:
     raise ImportError(
         "Current pint version is {__version__} but must be 0.18 or higher. Please consider upgrading it "
-        "(e.g. `> pip install pint --upgrade` or `> conda update pint`)\n"
+        "(e.g. `> pip install pint --upgrade` or `> conda update pint` )\n"
     )
 if pint_version < 20:
     print(
         f"Warning: current pint version is {__version__}. It might not be supported by SpectroChemPy in the future.\n"
-        f"Please consider upgrading it to 0.20 or higher (e.g. `> pip install pint --upgrade` or `> conda update pint`)\n"
+        f"Please consider upgrading it to 0.20 or higher (e.g. `> pip install pint --upgrade` or `> conda update pint` )\n"
     )
 
     from pint.converters import ScaleConverter
     from pint.quantity import Quantity
     from pint.unit import Unit, UnitDefinition, UnitsContainer
 else:
     from pint import Quantity, Unit
@@ -328,21 +328,20 @@
 # --------------------------------------------------------------------------------------
 def set_nmr_context(larmor):
     """
     Set a NMR context relative to the given Larmor frequency.
 
     Parameters
     ----------
-    larmor : |Quantity| or float
+    larmor : `Quantity` or `float`
         The Larmor frequency of the current nucleus.
         If it is not a quantity it is assumed to be given in MHz.
 
     Examples
     --------
-
     First we set the NMR context,
 
     >>> from spectrochempy.core.units import ur, set_nmr_context
     >>>
     >>> set_nmr_context(104.3 * ur.MHz)
 
     then, we can use the context as follow
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/writers/api.py` & `spectrochempy-0.6.1/spectrochempy/core/writers/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/core/writers/exporter.py` & `spectrochempy-0.6.1/spectrochempy/core/writers/exporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 # --------------------------------------------------------------------------------------
 def write(dataset, filename=None, **kwargs):
     """
     Write  the current dataset.
 
     Parameters
     ----------
-    dataset : |NDDataset|
+    dataset : `NDDataset`
         Dataset to write.
     filename : str or pathlib object, optional
         If not provided, a dialog is opened to select a file for writing.
     **kwargs
         Optional keyword parameters (see Other Parameters).
 
     Returns
@@ -112,28 +112,28 @@
 
     Other Parameters
     ----------------
     protocol : {'scp', 'matlab', 'jcamp', 'csv', 'excel'}, optional
         Protocol used for writing. If not provided, the correct protocol
         is inferred (whnever it is possible) from the file name extension.
     directory : str, optional
-        Where to write the specified `filename`. If not specified, write in the current directory.
+        Where to write the specified `filename` . If not specified, write in the current directory.
     description: str, optional
         A Custom description.
     csv_delimiter : str, optional
         Set the column delimiter in CSV file.
-        By default it is the one set in SpectroChemPy `Preferences`.
+        By default it is the one set in SpectroChemPy `Preferences` .
 
     See Also
     --------
     save : Generic function for saving a NDDataset in SpectroChemPy format.
 
     Examples
     ---------
-    write a dataset (providing a windows type filename relative to the default ``Datadir``)
+    write a dataset (providing a windows type filename relative to the default `Datadir` )
 
     >>> nd = scp.read_opus('irdata/OPUS')
     >>> f = nd.write('opus.scp') # doctest: +SKIP
     >>> f.name                   # doctest: +SKIP
     'opus.scp'                   # doctest: +SKIP
 
     """
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/writers/write_csv.py` & `spectrochempy-0.6.1/spectrochempy/core/writers/write_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,20 +28,20 @@
     ----------
     filename: str or pathlib object, optional
         If not provided, a dialog is opened to select a file for writing.
     protocol : {'scp', 'matlab', 'jcamp', 'csv', 'excel'}, optional
         Protocol used for writing. If not provided, the correct protocol
         is inferred (whnever it is possible) from the file name extension.
     directory : str, optional
-        Where to write the specified `filename`. If not specified, write in the current directory.
+        Where to write the specified `filename` . If not specified, write in the current directory.
     description: str, optional
         A Custom description.
     delimiter : str, optional
         Set the column delimiter in CSV file.
-        By default it is ',' or the one set in SpectroChemPy `Preferences`.
+        By default it is ',' or the one set in SpectroChemPy `Preferences` .
 
     Returns
     -------
     out : `pathlib` object
         Path of the saved file.
 
     Examples
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/writers/write_excel.py` & `spectrochempy-0.6.1/spectrochempy/core/writers/write_excel.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ----------
     filename: str or pathlib object, optional
         If not provided, a dialog is opened to select a file for writing
     protocol : {'scp', 'matlab', 'jcamp', 'csv', 'excel'}, optional
         Protocol used for writing. If not provided, the correct protocol
         is inferred (whnever it is possible) from the file name extension.
     directory : str, optional
-        Where to write the specified `filename`. If not specified, write in the current directory.
+        Where to write the specified `filename` . If not specified, write in the current directory.
     description: str, optional
         A Custom description.
 
     Returns
     -------
     out : `pathlib` object
         path of the saved file.
@@ -45,13 +45,13 @@
     exporter = Exporter()
     kwargs["filetypes"] = ["Microsoft Excel files (*.xls)"]
     kwargs["suffix"] = ".xls"
     return exporter(*args, **kwargs)
 
 
 write_xls = write_excel
-write_xls.__doc__ = "This method is an alias of `write_excel`."
+write_xls.__doc__ = "This method is an alias of `write_excel` ."
 
 
 @exportermethod
 def _write_excel(*args, **kwargs):
     raise NotImplementedError
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/writers/write_jcamp.py` & `spectrochempy-0.6.1/spectrochempy/core/writers/write_jcamp.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     ----------
     filename: str or pathlib object, optional
         If not provided, a dialog is opened to select a file for writing.
     protocol : {'scp', 'matlab', 'jcamp', 'csv', 'excel'}, optional
         Protocol used for writing. If not provided, the correct protocol
         is inferred (whnever it is possible) from the file name extension.
     directory : str, optional
-        Where to write the specified `filename`. If not specified, write in the current directory.
+        Where to write the specified `filename` . If not specified, write in the current directory.
     description: str, optional
         A Custom description.
 
     Returns
     -------
     out : `pathlib` object
         path of the saved file.
@@ -49,15 +49,15 @@
     exporter = Exporter()
     kwargs["filetypes"] = ["JCAMP-DX files (*.jdx)"]
     kwargs["suffix"] = ".jdx"
     return exporter(*args, **kwargs)
 
 
 write_jdx = write_jcamp
-write_jdx.__doc__ = "This method is an alias of `write_jcamp`."
+write_jdx.__doc__ = "This method is an alias of `write_jcamp` ."
 
 
 @exportermethod
 def _write_jcamp(*args, **kwargs):
     # Writes a dataset in JCAMP-DX format
 
     dataset, filename = args
```

### Comparing `spectrochempy-0.5.5/spectrochempy/core/writers/write_matlab.py` & `spectrochempy-0.6.1/spectrochempy/core/writers/write_matlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 def write_matlab(*args, **kwargs):
     """
     Write a dataset in CSV format.
 
     Parameters
     ----------
-    *args
+    \*args
     **kwargs
 
     Returns
     -------
     out : `pathlib` object
         Path of the saved file.
 
@@ -37,13 +37,13 @@
     exporter = Exporter()
     kwargs["filetypes"] = ["MATLAB files (*.mat)"]
     kwargs["suffix"] = ".mat"
     return exporter(*args, **kwargs)
 
 
 write_mat = write_matlab
-write_mat.__doc__ = "This method is an alias of `write_matlab`."
+write_mat.__doc__ = "This method is an alias of `write_matlab` ."
 
 
 @exportermethod
 def _write_matlab(*args, **kwargs):
     raise NotImplementedError
```

### Comparing `spectrochempy-0.5.5/spectrochempy/extern/nmrglue.py` & `spectrochempy-0.6.1/spectrochempy/extern/nmrglue.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,14 @@
 import os
 import string
 from functools import reduce
 from warnings import warn
 
 import numpy as np
 
-__all__ = []
-
 
 def create_blank_udic(ndim):
     """
     Create a blank universal dictionary for a spectrum of dimension ndim.
     """
     udic = dict()
     udic["ndim"] = ndim
@@ -576,15 +574,15 @@
 
 def fft_positive(data):
     """
     Fourier transform with positive exponential, NMR ordering of results
 
     This is similar to the transform performed by NMRPipe's FFT function.
 
-    See :py:func:`fft` for documentation of the transformation applied by this
+    See :func:`fft` for documentation of the transformation applied by this
     function.
 
     Parameters
     ----------
     data : ndarray
         Array of NMR data.
 
@@ -684,15 +682,15 @@
     Parameters
     ----------
     dic : dict
         Dictionary of Bruker parameters.
     data : ndarray
         Array of NMR data.
     strip_fake: bool
-        If data is proceed (i.e. read using `bruker.read_pdata`) and the Bruker
+        If data is proceed (i.e. read using `bruker.read_pdata` ) and the Bruker
         processing parameters STSI and/or STSR are set, the returned sweep
         width and carrier frequencies is changed to values that are incorrect
         but instead can are intended to trick the normal unit_conversion object
         into producing the correct result.
 
     Returns
     -------
```

### Comparing `spectrochempy-0.5.5/spectrochempy/extern/traittypes.py` & `spectrochempy-0.6.1/spectrochempy/extern/traittypes.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/extern/traittypes_utils.py` & `spectrochempy-0.6.1/spectrochempy/extern/traittypes_utils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/ipython/magics.py` & `spectrochempy-0.6.1/spectrochempy/ipython/magics.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,27 @@
 from IPython.core.error import UsageError
 from IPython.core.magic import Magics, line_cell_magic, magics_class
 from IPython.core.magics.code import extract_symbols
 from IPython.utils.text import get_text_list
 
 from spectrochempy import error_, warning_
 
+__all__ = ["SpectroChemPyMagics"]
+
 
 # ======================================================================================
 # Magic ipython Classes
 # ======================================================================================
 @magics_class
 class SpectroChemPyMagics(Magics):
     """
     This class implements the addscript ipython magic function.
+
+    The ipython extensions`can be loaded via `%load_ext spectrochempy.ipython`
+    or be configured to be autoloaded by IPython at startup time.
     """
 
     @line_cell_magic
     def addscript(self, pars="", cell=None):
         """
         This works both as **%addscript** and as **%%addscript**.
 
@@ -143,11 +148,11 @@
         # args = self.parse_options(pars, '')  #  #     if  # not args:
         #         raise UsageError('Missing script
         # name')  #  #  # return args
 
 
 def load_ipython_extension(ipython):
     """
-    The ipython extensions`can be loaded via `%load_ext spectrochempy.ipython` or be configured to be
-    autoloaded by IPython at startup time.
+    The ipython extensions`can be loaded via `%load_ext spectrochempy.ipython`
+    or be configured to be autoloaded by IPython at startup time.
     """
     ipython.register_magics(SpectroChemPyMagics)
```

### Comparing `spectrochempy-0.5.5/spectrochempy/plot_preferences.py` & `spectrochempy-0.6.1/spectrochempy/application/plot_preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,26 +19,26 @@
     Tuple,
     Unicode,
     Union,
     default,
     observe,
 )
 
-from spectrochempy.utils.traits import MetaConfigurable
+from spectrochempy.application.metaconfigurable import MetaConfigurable
 
 # from spectrochempy.core import warning_
 
 
 # --------------------------------------------------------------------------------------
 # available matplotlib styles (equivalent of plt.style.available)
 # --------------------------------------------------------------------------------------
 def available_styles():
     """
     All matplotlib `styles <https://matplotlib.org/users/style_sheets.html>`_
-    which are available in |scpy|
+    which are available in  `SpectroChemPy`
 
     Returns
     -------
     A list of matplotlib styles
     """
     from spectrochempy.utils.file import pathclean
 
@@ -329,15 +329,15 @@
     mathtext_cal = Unicode("cursive", help=r"""""").tag(config=True, kind="")
     mathtext_rm = Unicode("dejavusans", help=r"""""").tag(config=True, kind="")
     mathtext_tt = Unicode("monospace", help=r"""""").tag(config=True, kind="")
     mathtext_it = Unicode("dejavusans:italic", help=r"""italic""").tag(
         config=True, kind=""
     )
     mathtext_bf = Unicode("dejavusans:bold", help=r"""bold""").tag(config=True, kind="")
-    mathtext_sf = Unicode("sans\-serif", help=r"""""").tag(
+    mathtext_sf = Unicode(r"sans\-serif", help=r"""""").tag(
         config=True, kind=""
     )  # noqa: W605
     mathtext_fontset = Unicode(
         "dejavusans",
         help=r'''Should be "dejavusans" (default),
                                "dejavuserif", "cm" (Computer Modern), "stix", "stixsans" or "custom"''',
     ).tag(config=True, kind="")
@@ -878,15 +878,15 @@
         config=True
     )
     ccount = Integer(50, help="ccount (steps in the column mode) for surface plot").tag(
         config=True
     )
 
     def __init__(self, **kwargs):
-        super().__init__(section="PlotPreferences", **kwargs)
+        super().__init__(**kwargs)
         for key in plt.rcParams:
             lis = key.split(".")
             if len(lis) > 1:
                 self._groups.add(lis.pop(0))
             if len(lis) > 1:
                 self.subgroups.add(lis.pop(0))
             if len(lis) > 1:
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/__init__.py` & `spectrochempy-0.6.1/spectrochempy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/citation.py` & `spectrochempy-0.6.1/spectrochempy/utils/citation.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 import pathlib
 import sys
 from datetime import date
 
 import yaml
 from cffconvert.cli.create_citation import create_citation
 
-__all__ = ["Citation", "Zenodo"]
-
 sys.tracebacklimit = 2
 
 HOME = pathlib.Path(__file__).parent.parent.parent
 
 
 class Zenodo:
     def __init__(self, infile=HOME / ".zenodo.json"):
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/constants.py` & `spectrochempy-0.6.1/spectrochempy/utils/constants.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/coordrange.py` & `spectrochempy-0.6.1/spectrochempy/utils/coordrange.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 This module implements the class _CoordRange.
 """
 
-__all__ = ["trim_ranges"]
-
 import traitlets as tr
 
 
 # ======================================================================================
 # _CoordRange
 # ======================================================================================
 class _CoordRange(tr.HasTraits):
@@ -81,15 +79,15 @@
     Set of ordered, non intersecting intervals.
 
     An ordered set of ranges is constructed from the inputs and returned.
     *e.g.,* [[a, b], [c, d]] with a < b < c < d or a > b > c > d.
 
     Parameters
     -----------
-    *ranges :  iterable
+    \*ranges :  iterable
         An interval or a set of intervals.
         set of  intervals. If none is given, the range will be a set of an empty
         interval [[]]. The interval
         limits do not need to be ordered, and the intervals do not need to be distincts.
     reversed : bool, optional
         The intervals are ranked by decreasing order if True or increasing order if
         False.
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/docstrings.py` & `spectrochempy-0.6.1/spectrochempy/utils/docstrings.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,43 +46,46 @@
     "EX02": "Examples do not pass tests:\n{doctest_log}",
     "EX03": "flake8 error: {error_code} {error_message}{times_happening}",
     "EX04": "Do not import {imported_library}, as it is imported "
     "automatically for the examples (numpy as np, spectrochempy as scp)",
 }
 
 
-common_doc = """
-copy : bool, optional, Default: True
+_common_doc = """
+copy : `bool`, optional, default: `True`
     Perform a copy of the passed object.
-inplace : bool, optional, default: False
+inplace : `bool`, optional, default: `False`
     By default, the method returns a newly allocated object.
-    If `inplace` is set to True, the input object is returned.
+    If `inplace` is set to `True`, the input object is returned.
 **kwargs : keyword parameters, optional
     See Other Parameters.
 """
 
 
 class DocstringProcessor(docrep.DocstringProcessor):
+
+    param_like_sections = ["See Also"] + docrep.DocstringProcessor.param_like_sections
+
     def __init__(self, **kwargs):
 
         super().__init__(**kwargs)
 
         regex = re.compile(r"(?=^[*]{0,2}\b\w+\b\s?:?\s?)", re.MULTILINE | re.DOTALL)
-        plist = regex.split(common_doc.strip())[1:]
+        plist = regex.split(_common_doc.strip())[1:]
         params = {
             k.strip("*"): f"{k.strip()} : {v.strip()}"
             for k, v in (re.split(r"\s?:\s?", p, maxsplit=1) for p in plist)
         }
         self.params.update(params)
         self.params.update(
             {
-                "out": "object\n"
+                "out": "`object`\n"
                 "    Input object or a newly allocated object\n"
                 "    depending on the `inplace` flag.",
-                "new": "object\n" "    Newly allocated object.",
+                "new": "`object`\n" "    Newly allocated object.",
             }
         )
 
     def dedent(self, s, stacklevel=3):
         s_ = s
         start = ""
         end = ""
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/fake.py` & `spectrochempy-0.6.1/spectrochempy/utils/fake.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 import numpy as np
 
-__all__ = ["generate_fake"]
-
 
 # --------------------------------------------------------------------------------------
 # Create fake data to be used by analysis routine for testing
 # --------------------------------------------------------------------------------------
 def _make_spectra_matrix(modelname, ampl, pos, width, ratio=None, asym=None):
-    from spectrochempy.analysis import models
+    from spectrochempy.analysis.optimize import _models
     from spectrochempy.core.dataset.coord import Coord
     from spectrochempy.core.dataset.nddataset import NDDataset
 
     x = Coord(np.linspace(6000.0, 1000.0, 4000), units="cm^-1", title="wavenumbers")
     s = []
     for arg in zip(modelname, ampl, pos, width, ratio, asym):
-        model = getattr(models, arg[0] + "model")()
+        model = getattr(_models, arg[0] + "model")()
         kwargs = {argname: arg[index + 1] for index, argname in enumerate(model.args)}
         s.append(model.f(x.data, **kwargs))
 
     st = np.vstack(s)
     st = NDDataset(
         data=st, units="absorbance", title="absorbance", coordset=[range(len(st)), x]
     )
@@ -57,33 +55,33 @@
     -------
     datasets:
         2D spectra, individual spectra and concentrations
     """
 
     # define properties of the spectra and concentration profiles
     # ----------------------------------------------------------------------------------
-    from spectrochempy.analysis import models
+    from spectrochempy.analysis.optimize import _models
     from spectrochempy.core.dataset.arraymixins.npy import dot
 
     # data for four peaks (one very broad)
     POS = (6000.0, 4000.0, 2000.0, 2500.0)
     WIDTH = (6000.0, 1000.0, 250.0, 800.0)
     AMPL = (100.0, 70.0, 10.0, 50.0)
     RATIO = (0.1, 0.5, 0.2, 1.0)
     ASYM = (0.0, 0.0, 0, 4)
     MODEL = ("gaussian", "voigt", "voigt", "asymmetricvoigt")
 
     def C1(t):
         return t * 0.05 + 0.01  # linear evolution of the baseline
 
     def C2(t):
-        return models.sigmoidmodel().f(t, 1.0, max(t) / 2.0, 1, 2)
+        return _models.sigmoidmodel().f(t, 1.0, max(t) / 2.0, 1, 2)
 
     def C3(t):
-        return models.sigmoidmodel().f(t, 1.0, max(t) / 5.0, 1, -2)
+        return _models.sigmoidmodel().f(t, 1.0, max(t) / 5.0, 1, -2)
 
     def C4(t):
         return 1.0 - C2(t) - C3(t)
 
     specs = _make_spectra_matrix(MODEL, AMPL, POS, WIDTH, RATIO, ASYM)
 
     concs = _make_concentrations_matrix(C1, C2, C3, C4)
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/file.py` & `spectrochempy-0.6.1/spectrochempy/utils/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,14 @@
 File utilities.
 """
 import re
 import warnings
 from os import environ
 from pathlib import Path, PosixPath, WindowsPath
 
-__all__ = [
-    "get_filenames",
-    "get_directory_name",
-    "pathclean",
-    "patterns",
-    "check_filenames",
-    "check_filename_to_open",
-    "check_filename_to_save",
-    "download_testdata",
-]
-
 
 # ======================================================================================
 # Utility functions
 # ======================================================================================
 def download_testdata():
     from spectrochempy.core import preferences
     from spectrochempy.core.readers.importer import read_remote
@@ -59,25 +48,27 @@
         return patterns
     else:
         return [_insensitive_case_glob(p) for p in patterns]
 
 
 def pathclean(paths):
     """
-    Clean a path or a series of path in order to be compatible with windows and unix-based system.
+    Clean a path or a series of path.
+
+    The aim is to be compatible with windows and unix-based system.
 
     Parameters
     ----------
     paths :  str or a list of str
         Path to clean. It may contain windows or conventional python separators.
 
     Returns
     -------
-    out : a pathlib object or a list of pathlib objects
-        Cleaned path(s)
+    pathlib or list of pathlib
+        Cleaned path(s).
 
     Examples
     --------
     >>> from spectrochempy.utils import pathclean
 
     Using unix/mac way to write paths
     >>> filename = pathclean('irdata/nh4y-activation.spg')
@@ -152,15 +143,15 @@
 
 def check_filenames(*args, **kwargs):
     """
     Return a list or a dictionary of filenames.
 
     Parameters
     ----------
-    *args
+    \*args
         If passed it is a str, a list of str or a dictionary containing filenames or a byte's contents.
     **kwargs
         Optional keywords parameters. See Other parameters
 
     Other Parameters
     ----------------
     filename :
@@ -184,15 +175,22 @@
     from spectrochempy.core import preferences as prefs
 
     datadir = pathclean(prefs.datadir)
 
     filenames = None
 
     if args:
-        if isinstance(args[0], (str, Path, PosixPath, WindowsPath)):
+        if (
+            isinstance(args[0], str)
+            and (args[0].startswith("http://") or args[0].startswith("https://"))
+            and kwargs.get("remote")
+        ):
+            # return url
+            return args
+        elif isinstance(args[0], (str, Path, PosixPath, WindowsPath)):
             # one or several filenames are passed - make Path objects
             filenames = pathclean(args)
         elif isinstance(args[0], bytes):
             # in this case, one or several byte contents has been passed instead of filenames
             # as filename where not given we passed the 'unnamed' string
             # return a dictionary
             return {pathclean(f"no_name_{i}"): arg for i, arg in enumerate(args)}
@@ -340,20 +338,20 @@
         List of filenames.
 
     Other Parameters
     ----------------
     directory : `str` or pathlib object, optional.
         The directory where to look at. If not specified, read in
         current directory, or in the datadir if unsuccessful.
-    filetypes : `list`, optional, default=['all files, '.*)'].
+    filetypes : `list` , optional, default=['all files, '.*)'].
         File type filter.
-    dictionary : `bool`, optional, default=True
+    dictionary : `bool` , optional, default=True
         Whether a dictionary or a list should be returned.
     listdir : bool, default=False
-        Read all file (possibly limited by `filetypes` in a given `directory`.
+        Read all file (possibly limited by `filetypes` in a given `directory` .
     recursive : bool, optional,  default=False.
         Read also subfolders.
 
     Warnings
     --------
     if several filenames are provided in the arguments, they must all reside in the same directory!
 
@@ -663,15 +661,20 @@
 
     if not isinstance(filenames, dict):
 
         if len(filenames) == 1 and filenames[0] is None:
             raise (FileNotFoundError)
 
         # deal with some specific cases
-        key = filenames[0].suffix.lower()
+        if isinstance(filenames[0], Path):
+            # all filename should be Path, except case of urls
+            key = filenames[0].suffix.lower()
+        elif filenames[0].startswith("http://") or filenames[0].startswith("https://"):
+            key = pathclean(filenames[0]).suffix.lower()
+
         if not key:
             if re.match(r"^fid$|^ser$|^[1-3][ri]*$", filenames[0].name) is not None:
                 key = ".topspin"
         if key[1:].isdigit():
             # probably an opus file
             key = ".opus"
         return {key: filenames}
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/jsonutils.py` & `spectrochempy-0.6.1/spectrochempy/utils/jsonutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 import base64
 import datetime
 import pathlib
 import pickle
 
 import numpy as np
 
-__all__ = ["json_serialiser", "json_decoder"]
-
 
 def fromisoformat(s):
     try:
         date = datetime.datetime.strptime(s, "%Y-%m-%dT%H:%M:%S.%f%Z")
     except Exception:
         date = datetime.datetime.strptime(s, "%Y-%m-%dT%H:%M:%S.%f")
     return date
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/misc.py` & `spectrochempy-0.6.1/spectrochempy/utils/misc.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,40 +13,14 @@
 import uuid
 import warnings
 from datetime import datetime, timezone
 
 import numpy as np
 from quaternion import as_float_array, as_quat_array
 
-__all__ = [
-    "TYPE_INTEGER",
-    "TYPE_COMPLEX",
-    "TYPE_FLOAT",
-    "TYPE_BOOL",
-    "EPSILON",
-    "INPLACE",
-    "typequaternion",
-    "make_new_object",
-    "getdocfrom",
-    "dict_compare",
-    "htmldoc",
-    "is_iterable",
-    "is_sequence",
-    "is_number",
-    "spacing_",
-    "largest_power_of_2",
-    "get_component",
-    "interleaved2quaternion",
-    "interleaved2complex",
-    "as_quaternion",
-    "quat_as_complex_array",
-    "get_n_decimals",
-    "gt_eps",
-]
-
 #
 # constants
 #
 TYPE_INTEGER = (int, np.int_, np.int32, np.int64, np.uint32, np.uint64)
 TYPE_FLOAT = (float, np.float_, np.float32, np.float64)
 TYPE_COMPLEX = (complex, np.complex_, np.complex64, np.complex128)
 TYPE_BOOL = (bool, np.bool_)
@@ -97,35 +71,28 @@
         names.insert(1, "co_kwonlyargcount")
     if hasattr(code, "co_posonlyargcount"):
         names.insert(1, "co_posonlyargcount")
     values = [changes.get(name, getattr(code_obj, name)) for name in names]
     return code(*values)
 
 
-class _DummyFile(object):
-    """
-    A writeable object.
-    """
-
-    def write(self, s):
-        pass
-
-
 # ======================================================================================
 # Public methods
 # ======================================================================================
 def as_quaternion(*args):
     """
     Recombine the arguments to produce a numpy array with quaternion dtype.
 
     Parameters
     ----------
-    *args : ndarray with dtype:float or complex
-        The quaternion array components: If there is 4 components, then we assume it is the four components of the
-        quaternion array: w, x, y, z. If there is only two, they are casted to complex and correspond respectively
+    *args : `ndarray` with dtype: `float` or `complex`
+        The quaternion array components: If there is 4 components, then we assume it is
+        the four components of the
+        quaternion array: w, x, y, z. If there is only two, they are casted to complex
+        and correspond respectively
         to w + i.x and y + j.z.
     """
     if len(args) == 4:
         # we assume here that the for components have been provided w, x, y, z
         w, x, y, z = args
 
     if len(args) == 2:
@@ -140,14 +107,15 @@
     """
     Recombine the component of a quaternion array into a tuple of two complex array.
 
     Parameters
     ----------
     arr : quaternion ndarray
         The arr will be separated into (w + i.x) and (y + i.z).
+
     Returns
     -------
     tuple
         Tuple of two complex array.
     """
     if not arr.dtype == np.quaternion:
         # no change
@@ -225,32 +193,35 @@
 
 def get_component(data, select="REAL"):
     """
     Take selected components of an hypercomplex array (RRR, RIR, ...).
 
     Parameters
     ----------
-    data : ndarray
-    select : str, optional, default='REAL'
+    data : `ndarray`
+        Input data array.
+    select : `str`, optional, default: 'REAL'
         If 'REAL', only real component in all dimensions will be selected.
         Else a string must specify which real (R) or imaginary (I) component
         has to be selected along a specific dimension. For instance,
         a string such as 'RRI' for a 2D hypercomplex array indicated
         that we take the real component in each dimension except the last
         one, for which imaginary component is preferred.
 
     Returns
     -------
     component
         A component of the complex or hypercomplex array.
 
     .. warning::
-        The definition is somewhat different from Bruker, as we order the component in the order of the dimensions in
+        The definition is somewhat different from Bruker, as we order the component in
+        the order of the dimensions in
         dataset:
-        e.g., for dims = ['y','x'], 'IR' means that the `y` component is imaginary while the `x` is real.
+        e.g., for dims = ['y','x'], 'IR' means that the `y` component is imaginary
+        while the `x` is real.
     """
     if not select:
         return data
 
     new = data.copy()
 
     if select == "REAL":
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/optional.py` & `spectrochempy-0.6.1/spectrochempy/utils/optional.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import importlib
 import sys
 import types
 import warnings
 
 from pkg_resources import DistributionNotFound, get_distribution
 
-__all__ = ["import_optional_dependency", "get_module_version"]
 VERSIONS = {
     "xarray": "*",
     "cantera": "2.5.1",
     "PyQt5": "*",
 }
 
 # A mapping from import name to package name (on PyPI) for packages where
@@ -51,38 +50,40 @@
 
     By default, if a dependency is missing an ImportError with a nice
     message will be raised. If a dependency is present, but too old,
     we raise.
 
     Parameters
     ----------
-    name : str
+    name : `str`
         The module name.
-    extra : str
+    extra : `str`
         Additional text to include in the ImportError message.
-    errors : str {'raise', 'warn', 'ignore'}
+    errors : `str` {'raise', 'warn', 'ignore'}
         What to do when a dependency is not found or its version is too old.
 
         * raise : Raise an ImportError
         * warn : Only applicable when a module's version is to old.
           Warns that the version is too old and returns None
-        * ignore: If the module is not installed, return None, otherwise,
+        * ignore : If the module is not installed, return None, otherwise,
           return the module, even if the version is too old.
           It's expected that users validate the version locally when
-          using ``errors="ignore"`` (see. ``io/html.py``)
-    min_version : str, default None
-        Specify a minimum version that is different from the global pandas
+          using ``errors="ignore"`` (see. `io/html.py`\ )
+
+    min_version : `str`, default: `None`
+        Specify a minimum version that is different from the global
         minimum version required.
+
     Returns
     -------
     maybe_module : Optional[ModuleType]
         The imported module, when found and the version is correct.
         None is returned when the package is not found and `errors`
         is False, or when the package's version is too old and `errors`
-        is ``'warn'``.
+        is ``'warn'``\ .
     """
     from spectrochempy.utils.version import Version
 
     assert errors in {"warn", "raise", "ignore"}
 
     package_name = INSTALL_MAPPING.get(name)
     install_name = package_name if package_name is not None else name
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/orderedset.py` & `spectrochempy-0.6.1/spectrochempy/utils/orderedset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # https://code.activestate.com/recipes/576694/
 # by Raymond Hettinger
 # license: MIT
 
 import collections
 
-__all__ = ["OrderedSet"]
-
 
 class OrderedSet(collections.abc.MutableSet):
     def __init__(self, iterable=None):
         self.end = end = []
         end += [None, end, end]  # sentinel node for doubly linked list
         self.map = {}  # key --> [key, prev, next]
         if iterable is not None:
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/packages.py` & `spectrochempy-0.6.1/spectrochempy/utils/packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 # ======================================================================================
 import os
 import sys
 from pkgutil import walk_packages
 
 from traitlets import import_item
 
-__all__ = ["list_packages", "generate_api", "get_pkg_path"]
-
 
 # ======================================================================================
 # PACKAGE and API UTILITIES
 # ======================================================================================
 def list_packages(package):
     """
     Return a list of the names of a package and its subpackages.
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/plots.py` & `spectrochempy-0.6.1/spectrochempy/utils/plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,30 +8,14 @@
 
 import matplotlib as mpl
 import matplotlib.axes as maxes
 import mpl_toolkits.mplot3d.axes3d as maxes3D
 import numpy as np
 from matplotlib import pyplot as plt
 
-__all__ = [
-    "cmyk2rgb",
-    "NBlack",
-    "NRed",
-    "NBlue",
-    "NGreen",
-    "figure",
-    "show",
-    "get_figure",  # Plotly specific
-    "get_plotly_figure",
-    "colorscale",
-    "make_attr",
-    "make_label",
-    "plot_method",
-]
-
 
 @maxes.subplot_class_factory
 class _Axes(maxes.Axes):
     """
     Subclass of matplotlib Axes class
     """
 
@@ -323,15 +307,15 @@
                 return getattr(dataset, f"plot_{type}")(*args, method=method, **kwargs)
 
         wrapper.__doc__ = f"""
 {textwrap.dedent(func.__doc__).strip()}
 
 Parameters
 ----------
-dataset : |NDDataset|
+dataset : `NDDataset`
     The dataset to plot.
 **kwargs
     Optional keyword parameters (see Other Parameters).
 
 
 Other Parameters
 ----------------
@@ -391,14 +375,15 @@
 #   Red CMYK= 0, 77, 100, 0 %
 #   Blue CMYK= 100, 30, 0, 0 %
 #   Green CMYK= 85, 0, 60, 10 %
 NBlack = (0, 0, 0)
 NRed = cmyk2rgb(0, 77, 100, 0)
 NBlue = cmyk2rgb(100, 30, 0, 0)
 NGreen = cmyk2rgb(85, 0, 60, 10)
+# TODO : make a color cycle based on these colors
 
 
 def figure(preferences=None, **kwargs):
     """
     Method to open a new figure.
 
     Parameters
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/print.py` & `spectrochempy-0.6.1/spectrochempy/utils/print.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,31 +5,14 @@
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 import re
 
 import numpy as np
 from colorama import Fore, Style
 
-__all__ = [
-    "numpyprintoptions",
-    "insert_masked_print",
-    "TBlack",
-    "TBold",
-    "TRed",
-    "TGreen",
-    "TBlue",
-    "TCyan",
-    "TMagenta",
-    "TYellow",
-    "colored",
-    "colored_output",
-    "pstr",
-    "convert_to_html",
-]
-
 
 def pstr(object, **kwargs):
     if hasattr(object, "_implements") and object._implements() in [
         "NDArray",
         "NDComplexArrray",
         "NDDataset",
         "LinearCoord",
@@ -233,15 +216,15 @@
         # Is the use of the display value enabled?
         #
         # """
         return self._enabled
 
     def enable(self, shrink=1):
         # """
-        # Set the enabling shrink to `shrink`.
+        # Set the enabling shrink to `shrink` .
         #
         # """
         self._enabled = shrink
 
     def __str__(self):
         return str(self._display)
 
@@ -283,15 +266,15 @@
 
 
 def _replace_dtype_fields(dtype, primitive_dtype):
     # """
     # Construct a dtype description list from a given dtype.
     #
     # Returns a new dtype object, with all fields and subtypes in the given type
-    # recursively replaced with `primitive_dtype`.
+    # recursively replaced with `primitive_dtype` .
     #
     # Arguments are coerced to dtypes first.
     #
     # -- copied from numpy.ma.core
     # """
     dtype = np.dtype(dtype)
     primitive_dtype = np.dtype(primitive_dtype)
@@ -321,15 +304,15 @@
     """
     Replace masked values with mask_string.
 
     -- copied from numpy.ma.core and modified
 
     Parameters
     ----------
-    ds : |NDDataset| instance
+    ds : `NDDataset` instance
     mask_string : str
     """
     from spectrochempy.utils.constants import NOMASK
 
     mask = ds._mask
     if mask is NOMASK:
         res = ds._data
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/print_versions.py` & `spectrochempy-0.6.1/spectrochempy/utils/print_versions.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/system.py` & `spectrochempy-0.6.1/spectrochempy/utils/system.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
-__all__ = [
-    "get_user_and_node",
-    "get_user",
-    "get_node",
-    "is_kernel",
-    "sh",
-]
-
 import getpass
 import platform
 import sys
 from subprocess import PIPE, STDOUT, run
 
 
 def get_user():
@@ -42,19 +34,20 @@
     from IPython import get_ipython  # pragma: no cover
 
     # check for `kernel` attribute on the IPython instance
     return getattr(get_ipython(), "kernel", None) is not None  # pragma: no cover
 
 
 class _ExecCommand:
-    """
-    Parameters
-    ----------
-    command : shell command to execute
-    """
+    # """
+    # Parameters
+    # ----------
+    # command : `str`
+    #     shell command to execute
+    # """
 
     def __init__(self, command):
 
         self.commands = [command]
 
     def __call__(self, *args, **kwargs):
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/testing.py` & `spectrochempy-0.6.1/spectrochempy/utils/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,25 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
-__all__ = [
-    "set_env",
-    "assert_equal",
-    "assert_array_equal",
-    "assert_array_almost_equal",
-    "assert_ndarray_equal",
-    "assert_ndarray_almost_equal",
-    "assert_coord_equal",
-    "assert_coord_almost_equal",
-    "assert_dataset_equal",
-    "assert_dataset_almost_equal",
-    "assert_equal_units",
-    "assert_project_equal",
-    "assert_script_equal",
-    "assert_project_almost_equal",
-    "assert_approx_equal",
-    "assert_raises",
-    "raises",
-    "catch_warnings",
-    "RandomSeedContext",
-]
 
 import contextlib
 import functools
 import operator
 import os
 import warnings
 
 import numpy as np
 
 # import matplotlib.pyplot as plt
 # from matplotlib.testing.compare import calculate_rms, ImageAssertionError
-from numpy.testing import (
+from numpy.testing import (  # noqa
     assert_approx_equal,
     assert_array_almost_equal,
     assert_array_compare,
     assert_array_equal,
     assert_equal,
     assert_raises,
 )
@@ -567,15 +546,15 @@
 
 
 # ======================================================================================
 # RandomSeedContext
 # ======================================================================================
 class RandomSeedContext(object):
     """
-    A context manager (for use with the ``with`` statement) that will seed the
+    A context manager (for use with the `with` statement) that will seed the
     numpy random number generator (RNG) to a specific value, and then restore
     the RNG state back to whatever it was before.
 
     (Copied from Astropy, licence BSD-3).
 
     Parameters
     ----------
@@ -618,15 +597,15 @@
     Parameters
     ----------
     unit1 : units
         Units to be compared.
     unit2 : units
         Other units to be compared
     strict :  bool, optional, default: False
-        If True, units should be exactly the same: `km` != `mm`.
+        If True, units should be exactly the same: `km` != `mm` .
     """
     from pint import DimensionalityError
 
     try:
         x = (1.0 * unit1).to_base_units() / (1.0 * unit2).to_base_units()
     except DimensionalityError:
         raise AssertionError
@@ -653,15 +632,15 @@
     Use as follows::
 
         @raises(ZeroDivisionError)
         def test_foo():
             x = 1/0
 
     This can also be used a context manager, in which case it is just
-    an alias for the ``pytest.raises`` context manager (because the
+    an alias for the `pytest.raises` context manager (because the
     two have the same name this help avoid confusion by being
     flexible).
 
     (Copied from Astropy, licence BSD-3)
     """
 
     # pep-8 naming exception -- this is a decorator class
@@ -693,15 +672,15 @@
     A high-powered version of warnings.catch_warnings to use for testing
     and to make sure that there is no dependence on the order in which
     the tests are run.
 
     This completely blitzes any memory of any warnings that have
     appeared before so that all warnings will be caught and displayed.
 
-    ``*args`` is a set of warning classes to collect.  If no arguments are
+    `*args` is a set of warning classes to collect.  If no arguments are
     provided, all warnings are collected.
 
     Use as follows::
 
         with catch_warnings(MyCustomWarning) as w :
             do.something.bad()
         assert len(w) > 0
@@ -836,43 +815,43 @@
 #     automatic similarity check is done :
 #
 #     Parameters
 #     ----------
 #     reference : list of image filename for the references
 #
 #         List the image filenames of the reference figures
-#         (located in ``.spectrochempy/figures``) which correspond in
+#         (located in ` .spectrochempy/figures` ) which correspond in
 #         the same order to
 #         the various figures created in the decorated function. if
 #         these files doesn't exist an error is generated, except if the
 #         force_creation argument is True. This should allow the creation
 #         of a reference figures, the first time the corresponding figures are
 #         created.
 #
-#     extension : str, optional, default=``png``
+#     extension : str, optional, default=`png`
 #
 #         Extension to be used to save figure, among
 #         (eps, jpeg, jpg, pdf, pgf, png, ps, raw, rgba, svg, svgz, tif, tiff)
 #
-#     force_creation : `bool`, optional, default=`False`.
+#     force_creation : `bool` , optional, default=`False` .
 #
 #         if this flag is True, the figures created in the decorated
 #         function are
 #         saved in the reference figures directory (
-#         ``.spectrocchempy/figures``)
+#         ` .spectrocchempy/figures` )
 #
 #     min_similarity : float (percent).
 #
 #         If set, then it will be used to decide if an image is the same (
 #         similar)
 #         or not. In this case max_rms is not used.
 #
 #     max_rms : float
 #
-#         rms stands for `Root Mean Square`. If set, then it will
+#         rms stands for `Root Mean Square` . If set, then it will
 #         be used to decide if an image is the same
 #         (less than the acceptable rms). Not used if min_similarity also set.
 #
 #     savedpi : int, optional, default=150
 #
 #         dot per inch of the generated figures
 #
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/traits.py` & `spectrochempy-0.6.1/spectrochempy/application/metaconfigurable.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,183 +1,153 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
-import inspect
 from pathlib import Path
 
 import numpy as np
 import traitlets as tr
 from matplotlib import cycler
+from traitlets.config import Config
 from traitlets.config.configurable import Configurable
 from traitlets.config.loader import LazyConfigValue
 
-from spectrochempy.extern.traittypes import Empty, SciType
-
-__all__ = []
+from spectrochempy.utils.objects import Adict
 
 
 class MetaConfigurable(Configurable):
     """
     A subclass of Configurable that stores configuration changes in a json file.
 
     Saving the configuration changes allows to retrieve them between different
     executions of the main application.
     """
 
-    def __init__(self, section, **kwargs):  # lgtm[py/missing-call-to-init]
-
-        super().__init__(**kwargs)
+    name = tr.Unicode(allow_none=True)
 
+    def __init__(self, **kwargs):
+        # keep only the current config section
+        reset = kwargs.pop("reset", False)
+        parent = kwargs.get("parent")
+        parent_config = parent.config
+        config = Config()
+        if self.name in parent_config and not reset:
+            config = Config({self.name: parent_config[self.name]})
+        # call the superclass __init__ is required
+        super().__init__(parent=parent, config=config)
+        # get the config manager
         self.cfg = self.parent.config_manager
-        self.section = section
+
+    @tr.default("name")
+    def _name_default(self):
+        # this ensures a name has been defined for the subclassed model estimators
+        return self.__class__.__name__
 
     def to_dict(self):
         """
         Return config value in a dict form.
 
         Returns
         -------
-        dict
+        `dict`
             A regular dictionary.
         """
         d = {}
         for k, v in self.traits(config=True).items():
             d[k] = v.default_value
         return d
 
     def trait_defaults(self, *names, **metadata):
         # override traitlets trait default to take into accound changes in the config file
         defaults = super().trait_defaults(*names, **metadata)
         # modify with the loaded external config
         if not names:  # full dictionary
-            config = self.config[self.section]
+            config = self.config[self.name]
             if "shape" in config and isinstance(config["shape"], LazyConfigValue):
                 del config["shape"]  # remove the lazy configurable object
             defaults.update(config)
         return defaults
 
+    def parameters(self, default=False):
+        """
+        Current or default configuration values.
+
+        Parameters
+        ----------
+        default : `bool`, optional, default: `False`
+            If `default` is `True`, the default parameters are returned,
+            else the current values.
+
+        Returns
+        -------
+        `dict`
+            Current or default configuration values.
+        """
+        d = Adict()
+        if not default:
+            d.update(self.trait_values(config=True))
+        else:
+            d.update(self.trait_defaults(config=True))
+        return d
+
+    def reset(self):
+        """
+        Reset configuration parameters to their default values
+        """
+        # for this we need to remove the section corresponding
+        # to the current configurable (i.e., self.name)
+        if self.name in self.config:
+            # remove this entry in config
+            del self.config[self.name]
+            # also delete the current JSON config file
+            f = (Path(self.cfg.config_dir) / self.name).with_suffix(".json")
+            f.unlink(missing_ok=True)
+
+        # then set the default parameters
+        for k, v in self.parameters(default=True).items():
+            if getattr(self, k) != v:
+                setattr(self, k, v)
+
     @tr.observe(tr.All)
     def _anytrait_changed(self, change):
         # update configuration after any change
 
         if not hasattr(self, "cfg"):
             # not yet initialized
             return
 
-        if change.name in self.traits(config=True):
+        if change.name in self.trait_names(config=True):
 
             value = change.new
-            # replace non serializable value by an equivalent
-            if isinstance(value, (type(cycler), Path)):
+
+            # Serialization of callable functions
+            # (avoid recursive functions, though!)
+            # for this we use the dill library
+            # (see
+            # https://medium.com/@greyboi/serialising-all-the-functions-in-python-cd880a63b591)
+            if callable(value):
+                import dill
+
+                value = dill.dumps(value)
+                # bytes are however not JSON serialisable: make an encoded string
+                import base64
+
+                value = base64.b64encode(value).decode()
+
+            # replace other serializable value by an equivalent
+            elif isinstance(value, (type(cycler), Path)):
                 value = str(value)
             if isinstance(value, np.ndarray):
                 # we need to transform it to a list of elements, bUT with python built-in
                 # types, which is not the case e.g., for int64
                 value = value.tolist()
 
             self.cfg.update(
-                self.section,
+                self.name,
                 {
                     self.__class__.__name__: {
                         change.name: value,
                     }
                 },
             )
-
-            self.updated = True
-
-
-class SpectroChemPyType(SciType):
-    """
-    A SpectroChemPy trait type.
-    """
-
-    info_text = "a Spectrochempy object"
-
-    klass = None
-
-    def validate(self, obj, value):
-        if value is None and not self.allow_none:
-            self.error(obj, value)
-        if value is None or value is tr.Undefined:
-            return super().validate(obj, value)
-        try:
-            value = self.klass(value)
-        except (ValueError, TypeError) as e:
-            raise tr.TraitError(e)
-        return super().validate(obj, value)
-
-    def set(self, obj, value):
-        new_value = self._validate(obj, value)
-        old_value = obj._trait_values.get(self.name, self.default_value)
-        obj._trait_values[self.name] = new_value
-        if (
-            (old_value is None and new_value is not None)
-            or (old_value is tr.Undefined and new_value is not tr.Undefined)
-            or not (old_value == new_value)
-        ):
-            obj._notify_trait(self.name, old_value, new_value)
-
-    def __init__(self, default_value=Empty, allow_none=False, klass=None, **kwargs):
-        if klass is None:
-            klass = self.klass
-        if (klass is not None) and inspect.isclass(klass):
-            self.klass = klass
-        else:
-            raise tr.TraitError(
-                "The klass attribute must be a class" " not: %r" % klass
-            )
-        if default_value is Empty:
-            default_value = klass()
-        elif default_value is not None and default_value is not tr.Undefined:
-            default_value = klass(default_value)
-        super().__init__(default_value=default_value, allow_none=allow_none, **kwargs)
-
-    def make_dynamic_default(self):
-        if self.default_value is None or self.default_value is tr.Undefined:
-            return self.default_value
-        else:
-            return self.default_value.copy()
-
-
-class NDDatasetType(SpectroChemPyType):
-    """
-    A NDDataset trait type.
-    """
-
-    info_text = "a SpectroChemPy NDDataset"
-
-    def __init__(self, default_value=Empty, allow_none=False, dtype=None, **kwargs):
-        if "klass" not in kwargs and self.klass is None:
-            from spectrochempy.core.dataset.nddataset import NDDataset
-
-            kwargs["klass"] = NDDataset
-        super().__init__(
-            default_value=default_value,
-            allow_none=allow_none,
-            **kwargs,
-        )
-        self.metadata.update({"dtype": dtype})
-
-
-class CoordType(SpectroChemPyType):
-    """
-    A NDDataset trait type.
-    """
-
-    info_text = "a SpectroChemPy coordinates object"
-
-    def __init__(self, default_value=Empty, allow_none=False, dtype=None, **kwargs):
-        if "klass" not in kwargs and self.klass is None:
-            from spectrochempy.core.dataset.coord import Coord
-
-            kwargs["klass"] = Coord
-        super().__init__(default_value=default_value, allow_none=allow_none, **kwargs)
-        self.metadata.update({"dtype": dtype})
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/version.py` & `spectrochempy-0.6.1/spectrochempy/utils/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 
 import collections
 import itertools
 import re
 import warnings
 from typing import Callable, Iterator, SupportsInt, Tuple, Union
 
-__all__ = ["parse", "Version", "LegacyVersion", "InvalidVersion"]
-
 
 class InfinityType:
     def __repr__(self) -> str:
         return "Infinity"
 
     def __hash__(self) -> int:
         return hash(repr(self))
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/warnings.py` & `spectrochempy-0.6.1/spectrochempy/utils/warnings.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,37 +5,35 @@
 from __future__ import annotations
 
 import re
 import warnings
 from contextlib import contextmanager
 from typing import Sequence, Type, cast
 
-__all__ = ["assert_produces_warning"]
-
 
 @contextmanager
 def assert_produces_warning(
     expected_warning: type[Warning] | bool | None = Warning,
     filter_level="always",
     check_stacklevel: bool = True,
     raise_on_extra_warnings: bool = True,
     match: str | None = None,
 ):
     """
     Context manager for running code expected to either raise a specific
     warning, or not raise any warnings. Verifies that the code raises the
     expected warning, and that it does not raise any other unexpected
-    warnings. It is basically a wrapper around ``warnings.catch_warnings``.
+    warnings. It is basically a wrapper around `warnings.catch_warnings` .
 
     Parameters
     ----------
     expected_warning : {Warning, False, None}, default Warning
-        The type of Exception raised. ``exception.Warning`` is the base
+        The type of Exception raised. `exception.Warning` is the base
         class for all warnings. To check that no warning is returned,
-        specify ``False`` or ``None``.
+        specify `False` or `None` .
     filter_level : str or None, default "always"
         Specifies whether warnings are ignored, displayed, or turned
         into errors.
         Valid values are:
 
         * "error" - turns matching warnings into exceptions
         * "ignore" - discard the warning
```

### Comparing `spectrochempy-0.5.5/spectrochempy/utils/zip.py` & `spectrochempy-0.6.1/spectrochempy/utils/zip.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,30 +6,28 @@
 # ======================================================================================
 import json
 import os
 from collections.abc import Mapping
 
 from numpy.lib.format import read_array
 
-__all__ = ["make_zipfile", "ScpFile"]
-
 
 # ======================================================================================
 # ZIP UTILITIES
 # ======================================================================================
 def make_zipfile(file, **kwargs):
     """
     Create a ZipFile.
 
     Allows for Zip64 (useful if files are larger than 4 GiB)
     (adapted from numpy)
 
     Parameters
     ----------
-    file :  file or str
+    file :  `file` or `str`
         The file to be zipped.
     **kwargs
         Additional keyword parameters.
         They are passed to the zipfile.ZipFile constructor.
 
     Returns
     -------
@@ -41,35 +39,35 @@
     return zipfile.ZipFile(file, **kwargs)
 
 
 class ScpFile(Mapping):  # lgtm[py/missing-equals]
     """
     ScpFile(fid).
 
-    (largely inspired by ``NpzFile`` object in numpy).
+    (largely inspired by `NpzFile` object in numpy).
 
-    `ScpFile` is used to load files stored in ``.scp`` or ``.pscp``
+    `ScpFile` is used to load files stored in ` .scp` or ` .pscp`
     format.
 
-    It assumes that files in the archive have a ``.npy`` extension in
-    the case of the dataset's ``.scp`` file format) ,  ``.scp``  extension
-    in the case of project's ``.pscp`` file format and finally ``pars.json``
+    It assumes that files in the archive have a ` .npy` extension in
+    the case of the dataset's ` .scp` file format) ,  ` .scp`  extension
+    in the case of project's ` .pscp` file format and finally `pars.json`
     files which contains other information on the structure and  attributes of
     the saved objects. Other files are ignored.
 
     Parameters
     ----------
     fid : file or str
         The zipped archive to open. This is either a file-like object
         or a string containing the path to the archive.
 
     Attributes
     ----------
     files : list of str
-        List of all files in the archive with a ``.npy`` extension.
+        List of all files in the archive with a ` .npy` extension.
     zip : ZipFile instance
         The ZipFile object initialized with the zipped archive.
     """
 
     def __init__(self, fid):
 
         _zip = make_zipfile(fid)
```

### Comparing `spectrochempy-0.5.5/spectrochempy/widgets/api.py` & `spectrochempy-0.6.1/spectrochempy/widgets/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.5.5/spectrochempy/widgets/baselinecorrector.py` & `spectrochempy-0.6.1/spectrochempy/widgets/baselinecorrector.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,31 +24,31 @@
 class BaselineCorrector:
     """
     Launch a GUI for baseline corrections.
 
     Wrapper of BaselineCorrection(X), with widgets for dataset slicing,
     input parameters and graphical output.
     Should be run in jupyter notebook (does not always run properly in jupyter lab)
-    with the widget backend (magic `%matplotlib widget`).
+    with the widget backend (magic `%matplotlib widget` ).
 
     Parameters
     ----------
-    X : |NDDataset|, default: None
+    X : `NDDataset`\, default: None
         The NDDataset to process. If None, an upload button can be used to load data.
     initial_ranges : list, optional, default: None
         The initial regions where to compute the baseline. If not given, 5% on each
         side of the spectra will be taken as a starting range's list.
 
     Attributes
     ----------
-    original : |NDDataset|
+    original : `NDDataset`
         The (sliced) NDDataset, without baseline correction.
-    corrected : |NDDataset|
+    corrected : `NDDataset`
         The baseline corrected NDDataset.
-    baseline : |NDDataset|
+    baseline : `NDDataset`
         The baselines.
 
     See Also
     --------
     BaselineCorrection : Baseline correction method.
 
     Notes
@@ -365,24 +365,28 @@
         else:
             for j, sub_item in enumerate(item):
                 ranges[i][j] = round(sub_item, decimals)
     return tuple(ranges)
 
 
 def _update_ranges(ranges, coord, decimals=2):
-    """return valid ranges
-
-    Ranges outside the coord limits (if any), are replaced
-    by the min or max the coords. Ranges with the limits or including
-    the limits are unchanged.
-    returns:
-    --------
-     list of ranges
-     Bool True if changed
-    """
+    # """
+    # Return valid ranges
+    #
+    # Ranges outside the coord limits (if any), are replaced
+    # by the min or max the coords. Ranges with the limits or including
+    # the limits are unchanged.
+    #
+    # Returns
+    # -------
+    # `list`
+    #     list of ranges
+    # `bool`
+    #     True if changed
+    # """
     ranges = list(ranges)
     changed = False
     # sort coord id needed
     if coord[-1] < coord[0]:
         coord = coord[::-1]
     for i, item in enumerate(ranges):
         # if out of range, makes it within coord limits"
```

### Comparing `spectrochempy-0.5.5/spectrochempy/widgets/fileselector.py` & `spectrochempy-0.6.1/spectrochempy/widgets/fileselector.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,16 +86,16 @@
                 self.widget._handle_displayed(**kwargs)
 
 
 class FileSelector(Base):
     """
     IPyWidgets interface for picking files.
 
-    The current path is stored in ``.path`` and the current selection is
-    stored in ``.value``.
+    The current path is stored in ` .path` and the current selection is
+    stored in ` .value` .
 
     Parameters
     ----------
     done_callback : function
         Called when the tick or cross buttons are clicked. Expects signature
         func(path, ok=True|False).
     filters : list of str or None
```

### Comparing `spectrochempy-0.5.5/spectrochempy.egg-info/PKG-INFO` & `spectrochempy-0.6.1/spectrochempy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrochempy
-Version: 0.5.5
+Version: 0.6.1
 Summary: Processing, analysis and modelling Spectroscopic data for Chemistry with Python
 Home-page: https://www.spectrochempy.fr
 Author: Arnaud Travert & Christian Fernandez
 Author-email: contact@spectrochempy.fr
 Maintainer: C. Fernandez
 Maintainer-email: christian.fernandez@ensicaen.fr
 License: CECILL-B
@@ -14,18 +14,18 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align ="center">
 <img src='https://github.com/spectrochempy/spectrochempy/raw/master/docs/_static/scpy.png' width="150">
 <br>
 SpectroChemPy
```

### Comparing `spectrochempy-0.5.5/spectrochempy.egg-info/SOURCES.txt` & `spectrochempy-0.6.1/spectrochempy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -58,36 +58,43 @@
 scp_data/stylesheets/scpy.mplstyle
 scp_data/stylesheets/serif.mplstyle
 scp_data/stylesheets/talk.mplstyle
 scripts/checkindex.py
 scripts/validate_docstrings.py
 spectrochempy/__init__.py
 spectrochempy/api.py
-spectrochempy/application.py
-spectrochempy/plot_preferences.py
 spectrochempy.egg-info/PKG-INFO
 spectrochempy.egg-info/SOURCES.txt
 spectrochempy.egg-info/dependency_links.txt
 spectrochempy.egg-info/not-zip-safe
 spectrochempy.egg-info/requires.txt
 spectrochempy.egg-info/top_level.txt
 spectrochempy/analysis/__init__.py
+spectrochempy/analysis/_base.py
 spectrochempy/analysis/api.py
-spectrochempy/analysis/cantera_utilities.py
 spectrochempy/analysis/efa.py
-spectrochempy/analysis/fitting.py
 spectrochempy/analysis/iris.py
-spectrochempy/analysis/lstsq.py
+spectrochempy/analysis/kinetic_utilities.py
+spectrochempy/analysis/linearregression.py
 spectrochempy/analysis/mcrals.py
-spectrochempy/analysis/models.py
 spectrochempy/analysis/nnmf.py
 spectrochempy/analysis/pca.py
 spectrochempy/analysis/peakfinding.py
+spectrochempy/analysis/readme.rst
 spectrochempy/analysis/simplisma.py
 spectrochempy/analysis/svd.py
+spectrochempy/analysis/optimize/__init__.py
+spectrochempy/analysis/optimize/_models.py
+spectrochempy/analysis/optimize/_parameters.py
+spectrochempy/analysis/optimize/optimize.py
+spectrochempy/application/__init__.py
+spectrochempy/application/application.py
+spectrochempy/application/general_preferences.py
+spectrochempy/application/metaconfigurable.py
+spectrochempy/application/plot_preferences.py
 spectrochempy/core/__init__.py
 spectrochempy/core/common/__init__.py
 spectrochempy/core/common/dialogs.py
 spectrochempy/core/dataset/__init__.py
 spectrochempy/core/dataset/api.py
 spectrochempy/core/dataset/coord.py
 spectrochempy/core/dataset/coordset.py
@@ -158,20 +165,22 @@
 spectrochempy/extern/traittypes_utils.py
 spectrochempy/ipython/__init__.py
 spectrochempy/ipython/magics.py
 spectrochempy/utils/__init__.py
 spectrochempy/utils/citation.py
 spectrochempy/utils/constants.py
 spectrochempy/utils/coordrange.py
+spectrochempy/utils/decorators.py
 spectrochempy/utils/docstrings.py
 spectrochempy/utils/exceptions.py
 spectrochempy/utils/fake.py
 spectrochempy/utils/file.py
 spectrochempy/utils/jsonutils.py
 spectrochempy/utils/misc.py
+spectrochempy/utils/objects.py
 spectrochempy/utils/optional.py
 spectrochempy/utils/orderedset.py
 spectrochempy/utils/packages.py
 spectrochempy/utils/plots.py
 spectrochempy/utils/print.py
 spectrochempy/utils/print_versions.py
 spectrochempy/utils/system.py
```

