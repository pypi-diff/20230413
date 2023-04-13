# Comparing `tmp/awkward-2.1.2.tar.gz` & `tmp/awkward-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Apr  8 19:13:43 2023, max compression
+gzip compressed data, last modified: Thu Apr 13 15:38:23 2023, max compression
```

## Comparing `awkward-2.1.2.tar` & `awkward-2.1.3.tar`

### file list

```diff
@@ -1,829 +1,838 @@
--rw-r--r--   0        0        0     1893 2023-04-08 19:13:43.000000 awkward-2.1.2/CITATION.cff
--rw-r--r--   0        0        0    13386 2023-04-08 19:13:43.000000 awkward-2.1.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    22687 2023-04-08 19:13:43.000000 awkward-2.1.2/README.md
--rw-r--r--   0        0        0      241 2023-04-08 19:13:43.000000 awkward-2.1.2/requirements-test.txt
--rw-r--r--   0        0        0     7833 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/_toc.yml
--rw-r--r--   0        0        0     7624 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/conf.py
--rw-r--r--   0        0        0      346 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/environment.yml.cog
--rw-r--r--   0        0        0     2603 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/index.md
--rw-r--r--   0        0        0    11642 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/prepare_docstrings.py
--rw-r--r--   0        0        0     4448 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/redirects-user-guide.json
--rw-r--r--   0        0        0    11436 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/redirects.json
--rw-r--r--   0        0        0      463 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/requirements.txt
--rw-r--r--   0        0        0      369 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/switcher.json
--rw-r--r--   0        0        0      930 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/_static/css/awkward.css
--rw-r--r--   0        0        0      354 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/_static/css/try-awkward-array.css
-lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
-lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0      469 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/_templates/funding.html
--rw-r--r--   0        0        0      474 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/_templates/redirect.html
--rw-r--r--   0        0        0     2968 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/getting-started/community-tutorials.md
--rw-r--r--   0        0        0     4654 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/getting-started/index.md
--rw-r--r--   0        0        0     3346 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/getting-started/papers-and-talks.md
--rw-r--r--   0        0        0       82 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/getting-started/try-awkward-array.md
-lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    12847 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/getting-started/demo/what-is-an-awkward-array.ipynb
-lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
-lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
-lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
-lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    17067 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/example-hierarchy.svg
-lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
-lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
-lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
-lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
-lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
-lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    25309 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/reference/ak.behavior.rst
--rw-r--r--   0        0        0     1430 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/reference/ak.builder.ArrayBuilder.rst
--rw-r--r--   0        0        0    64727 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/reference/awkwardforth.rst
--rw-r--r--   0        0        0      270 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/reference/index.md
--rw-r--r--   0        0        0     7252 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/reference/toctree.txt
--rw-r--r--   0        0        0     8320 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/10-minutes-to-awkward-array.md
--rw-r--r--   0        0        0      926 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-combinatorics-best-match.md
--rw-r--r--   0        0        0      930 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
--rw-r--r--   0        0        0      263 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-combinatorics.md
--rw-r--r--   0        0        0     8335 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert-arrow.md
--rw-r--r--   0        0        0     6392 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert-buffers.md
--rw-r--r--   0        0        0     2455 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert-json.md
--rw-r--r--   0        0        0    13475 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert-numpy.md
--rw-r--r--   0        0        0     7182 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert-pandas.md
--rw-r--r--   0        0        0    18830 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert-python.md
--rw-r--r--   0        0        0     3554 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert-rdataframe.md
--rw-r--r--   0        0        0      271 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert.md
--rw-r--r--   0        0        0    11973 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create-arraybuilder.md
--rw-r--r--   0        0        0    36520 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create-constructors.md
--rw-r--r--   0        0        0     7383 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create-lists.md
--rw-r--r--   0        0        0     7456 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create-missing.md
--rw-r--r--   0        0        0    11542 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create-records.md
--rw-r--r--   0        0        0     4066 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create-strings.md
--rw-r--r--   0        0        0      866 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create-unflatten-group.md
--rw-r--r--   0        0        0      267 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create.md
--rw-r--r--   0        0        0      834 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-examine-checking-validity.md
--rw-r--r--   0        0        0     2919 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-examine-list-fields.md
--rw-r--r--   0        0        0      848 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-examine-simple-slicing.md
--rw-r--r--   0        0        0      838 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-examine-single-item.md
--rw-r--r--   0        0        0     6778 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-examine-type.md
--rw-r--r--   0        0        0      269 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-examine.md
--rw-r--r--   0        0        0      844 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-filter-cut-mask.md
--rw-r--r--   0        0        0     3889 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-filter-masked.md
--rw-r--r--   0        0        0      840 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-filter-num.md
--rw-r--r--   0        0        0     7955 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-filter-ragged.md
--rw-r--r--   0        0        0      265 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-filter.md
--rw-r--r--   0        0        0      818 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-math-argminmax.md
--rw-r--r--   0        0        0      822 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-math-broadcasting.md
--rw-r--r--   0        0        0      828 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-math-gpu.md
--rw-r--r--   0        0        0      838 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-math-numpy.md
--rw-r--r--   0        0        0      846 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-math-reducing.md
--rw-r--r--   0        0        0      870 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-math-statistics.md
--rw-r--r--   0        0        0      265 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-math.md
--rw-r--r--   0        0        0     3411 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure-add-fields.md
--rw-r--r--   0        0        0      842 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure-concatenate.md
--rw-r--r--   0        0        0    19083 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure-flatten.md
--rw-r--r--   0        0        0     7568 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure-pad.md
--rw-r--r--   0        0        0      852 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure-rename-records.md
--rw-r--r--   0        0        0      832 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure-sort.md
--rw-r--r--   0        0        0     9624 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure-zip-project.md
--rw-r--r--   0        0        0      273 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure.md
--rw-r--r--   0        0        0     2599 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-specialize-differentiate-jax.md
--rw-r--r--   0        0        0      870 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-specialize-in-numba.md
--rw-r--r--   0        0        0      838 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-specialize-lorentz.md
--rw-r--r--   0        0        0      874 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-specialize-override-numpy.md
--rw-r--r--   0        0        0      870 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-specialize-subclass.md
--rw-r--r--   0        0        0      277 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-specialize.md
--rw-r--r--   0        0        0    11724 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-use-header-only-layoutbuilder.md
--rw-r--r--   0        0        0      900 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-use-in-numba-arraybuilder.md
--rw-r--r--   0        0        0     9973 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-use-in-numba-cuda.ipynb
--rw-r--r--   0        0        0      900 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-use-in-numba-features.md
--rw-r--r--   0        0        0      279 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-use-in-numba.md
--rw-r--r--   0        0        0      344 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/index.md
--rw-r--r--   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/requirements.txt
--rw-r--r--   0        0        0   367587 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-data-analysts.png
--rw-r--r--   0        0        0   794465 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-data-analysts.svg
--rw-r--r--   0        0        0   140700 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-developers.png
--rw-r--r--   0        0        0   328307 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-developers.svg
--rw-r--r--   0        0        0    73584 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-doxygen.png
--rw-r--r--   0        0        0    58179 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-sphinx.png
--rw-r--r--   0        0        0   127063 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-tutorials-alternate.png
--rw-r--r--   0        0        0   173327 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-tutorials.png
--rw-r--r--   0        0        0    12541 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-1-0-layers.pdf
--rw-r--r--   0        0        0    65246 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-1-0-layers.png
--rw-r--r--   0        0        0    41004 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-1-0-layers.svg
--rw-r--r--   0        0        0    14946 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-timeline.pdf
--rw-r--r--   0        0        0   125180 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-timeline.png
--rw-r--r--   0        0        0    70209 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-timeline.svg
--rw-r--r--   0        0        0   436595 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
--rw-r--r--   0        0        0   426911 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
--rw-r--r--   0        0        0   335955 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip.png
--rw-r--r--   0        0        0   325268 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip.svg
--rw-r--r--   0        0        0   129696 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline.png
--rw-r--r--   0        0        0   120554 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline.svg
--rw-r--r--   0        0        0     5208 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-broadcasting.png
--rw-r--r--   0        0        0    25065 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-broadcasting.svg
--rw-r--r--   0        0        0     5754 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-cartesian.png
--rw-r--r--   0        0        0    32616 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-cartesian.svg
--rw-r--r--   0        0        0     9584 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-combinations.png
--rw-r--r--   0        0        0    39524 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-combinations.svg
--rw-r--r--   0        0        0    10808 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-schematic.png
--rw-r--r--   0        0        0    25779 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-schematic.svg
--rw-r--r--   0        0        0    18178 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    36024 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/example-hierarchy.png
--rw-r--r--   0        0        0    17092 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/example-hierarchy.svg
--rw-r--r--   0        0        0    21120 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/example-reduction-sum-only.svg
--rw-r--r--   0        0        0    29325 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    55553 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/example-reduction.png
--rw-r--r--   0        0        0    21631 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/example-reduction.svg
--rw-r--r--   0        0        0    10978 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/git-strategy.pdf
--rw-r--r--   0        0        0    58904 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/git-strategy.png
--rw-r--r--   0        0        0    28990 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/git-strategy.svg
--rw-r--r--   0        0        0   113587 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/how-it-works-muons.png
--rw-r--r--   0        0        0    57471 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/how-it-works-muons.svg
--rw-r--r--   0        0        0    58475 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/how-it-works.svg
--rw-r--r--   0        0        0    63989 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/sorting-axis.svg
--rw-r--r--   0        0        0   124038 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/all.svg
--rw-r--r--   0        0        0   128558 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/any.svg
--rw-r--r--   0        0        0   134490 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/argmax.svg
--rw-r--r--   0        0        0   133192 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/argmin.svg
--rw-r--r--   0        0        0   106277 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/count.svg
--rw-r--r--   0        0        0   116417 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/count_nonzero.svg
--rw-r--r--   0        0        0   111789 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/max.svg
--rw-r--r--   0        0        0   109239 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/min.svg
--rw-r--r--   0        0        0   124702 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/product.svg
--rw-r--r--   0        0        0   108897 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/sum.svg
--rw-r--r--   0        0        0     8347 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/logo/favicon.ico
--rw-r--r--   0        0        0     8984 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/logo/logo-300px-white.png
--rw-r--r--   0        0        0    11964 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    24707 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/logo/logo-600px.png
--rw-r--r--   0        0        0    18767 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/logo/logo.svg
--rw-r--r--   0        0        0    90413 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/photos/desire-path.jpg
--rw-r--r--   0        0        0    52113 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/plots/awkward-0-popularity.pdf
--rw-r--r--   0        0        0   146109 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/plots/awkward-0-popularity.png
--rw-r--r--   0        0        0   147576 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/plots/awkward-0-popularity.svg
--rw-r--r--   0        0        0    26938 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/plots/bikeroutes-scaling.svg
--rw-r--r--   0        0        0     8891 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/screenshots/github-issues-documentation.png
--rw-r--r--   0        0        0     1301 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/__init__.py
--rw-r--r--   0        0        0     7950 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_backends.py
--rw-r--r--   0        0        0     5418 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_behavior.py
--rw-r--r--   0        0        0    38002 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_broadcasting.py
--rw-r--r--   0        0        0    13390 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_do.py
--rw-r--r--   0        0        0    11875 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_errors.py
--rw-r--r--   0        0        0     5130 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_kernels.py
--rw-r--r--   0        0        0     5781 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_layout.py
--rw-r--r--   0        0        0     9983 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_lookup.py
--rw-r--r--   0        0        0     5454 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_parameters.py
--rw-r--r--   0        0        0     9965 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_prettyprint.py
--rw-r--r--   0        0        0    24569 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_reducers.py
--rw-r--r--   0        0        0     2041 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_regularize.py
--rw-r--r--   0        0        0      420 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_singleton.py
--rw-r--r--   0        0        0    23977 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_slicing.py
--rw-r--r--   0        0        0      647 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_typetracer.py
--rw-r--r--   0        0        0     1163 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_typing.py
--rw-r--r--   0        0        0     2439 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_util.py
--rw-r--r--   0        0        0      758 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_v2.py
--rw-r--r--   0        0        0      233 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/builder.py
--rw-r--r--   0        0        0      866 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/cppyy.py
--rw-r--r--   0        0        0      271 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forth.py
--rw-r--r--   0        0        0   102580 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/highlevel.py
--rw-r--r--   0        0        0     7899 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/index.py
--rw-r--r--   0        0        0     3982 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/jax.py
--rw-r--r--   0        0        0     2764 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/numba.py
--rw-r--r--   0        0        0     7982 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/record.py
--rw-r--r--   0        0        0      165 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/typetracer.py
--rw-r--r--   0        0        0       88 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/__init__.py
--rw-r--r--   0        0        0    32504 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/avro.py
--rw-r--r--   0        0        0    53533 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cling.py
--rw-r--r--   0        0        0      992 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/hist.py
--rw-r--r--   0        0        0     4485 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numexpr.py
--rw-r--r--   0        0        0    10031 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numpy.py
--rw-r--r--   0        0        0    37991 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/pyarrow.py
--rw-r--r--   0        0        0     7038 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/__init__.py
--rw-r--r--   0        0        0     2555 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
--rw-r--r--   0        0        0     4326 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
--rw-r--r--   0        0        0      987 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
--rw-r--r--   0        0        0     2542 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3034 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0      630 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
--rw-r--r--   0        0        0      830 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3196 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
--rw-r--r--   0        0        0     2668 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0      749 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
--rw-r--r--   0        0        0     2749 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
--rw-r--r--   0        0        0      552 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
--rw-r--r--   0        0        0      637 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
--rw-r--r--   0        0        0     2886 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
--rw-r--r--   0        0        0     2904 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3416 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0     3531 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
--rw-r--r--   0        0        0      556 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
--rw-r--r--   0        0        0      695 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3036 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
--rw-r--r--   0        0        0      795 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
--rw-r--r--   0        0        0     2523 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0     2729 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
--rw-r--r--   0        0        0     1035 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
--rw-r--r--   0        0        0      961 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
--rw-r--r--   0        0        0     2593 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
--rw-r--r--   0        0        0     1536 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
--rw-r--r--   0        0        0     1710 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     2012 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1184 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
--rw-r--r--   0        0        0      755 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu
--rw-r--r--   0        0        0      806 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
--rw-r--r--   0        0        0      744 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
--rw-r--r--   0        0        0     1169 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0     1059 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
--rw-r--r--   0        0        0     3208 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
--rw-r--r--   0        0        0      575 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
--rw-r--r--   0        0        0      830 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
--rw-r--r--   0        0        0      650 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
--rw-r--r--   0        0        0     2610 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
--rw-r--r--   0        0        0     1126 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
--rw-r--r--   0        0        0      951 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      721 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
--rw-r--r--   0        0        0     1003 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
--rw-r--r--   0        0        0     1339 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
--rw-r--r--   0        0        0      835 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
--rw-r--r--   0        0        0      975 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
--rw-r--r--   0        0        0      802 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
--rw-r--r--   0        0        0     1123 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu
--rw-r--r--   0        0        0      623 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu
--rw-r--r--   0        0        0      789 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
--rw-r--r--   0        0        0     1040 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     1020 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1045 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      974 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
--rw-r--r--   0        0        0      946 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
--rw-r--r--   0        0        0      980 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
--rw-r--r--   0        0        0      663 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
--rw-r--r--   0        0        0      586 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
--rw-r--r--   0        0        0     2580 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
--rw-r--r--   0        0        0     1360 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
--rw-r--r--   0        0        0      461 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
--rw-r--r--   0        0        0      534 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
--rw-r--r--   0        0        0      529 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
--rw-r--r--   0        0        0      830 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
--rw-r--r--   0        0        0      636 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
--rw-r--r--   0        0        0      689 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0      457 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
--rw-r--r--   0        0        0      830 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
--rw-r--r--   0        0        0     2043 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
--rw-r--r--   0        0        0     2198 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
--rw-r--r--   0        0        0     2043 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
--rw-r--r--   0        0        0     2198 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
--rw-r--r--   0        0        0     3054 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
--rw-r--r--   0        0        0     3289 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
--rw-r--r--   0        0        0     2022 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
--rw-r--r--   0        0        0     2022 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
--rw-r--r--   0        0        0     3202 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
--rw-r--r--   0        0        0     3012 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
--rw-r--r--   0        0        0     3171 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
--rw-r--r--   0        0        0     3439 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
--rw-r--r--   0        0        0     3439 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
--rw-r--r--   0        0        0      865 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
--rw-r--r--   0        0        0      443 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
--rw-r--r--   0        0        0     3195 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
--rw-r--r--   0        0        0     1859 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/header-only/awkward/BuilderOptions.h
--rw-r--r--   0        0        0    19867 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
--rw-r--r--   0        0        0    89307 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
--rw-r--r--   0        0        0      298 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/header-only/awkward/demo_impl.h
--rw-r--r--   0        0        0     8025 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/header-only/awkward/utils.h
--rw-r--r--   0        0        0      239 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/jax/__init__.py
--rw-r--r--   0        0        0     6627 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/jax/reducers.py
--rw-r--r--   0        0        0     5930 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/jax/trees.py
--rw-r--r--   0        0        0       88 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numba/__init__.py
--rw-r--r--   0        0        0    35824 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numba/arrayview.py
--rw-r--r--   0        0        0     1148 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numba/arrayview_cuda.py
--rw-r--r--   0        0        0    31514 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numba/builder.py
--rw-r--r--   0        0        0    12431 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numba/growablebuffer.py
--rw-r--r--   0        0        0    49132 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numba/layout.py
--rw-r--r--   0        0        0       88 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/rdataframe/__init__.py
--rw-r--r--   0        0        0     9341 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/rdataframe/from_rdataframe.py
--rw-r--r--   0        0        0     9922 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/rdataframe/to_rdataframe.py
--rw-r--r--   0        0        0     1487 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
--rw-r--r--   0        0        0     3526 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/__init__.py
--rw-r--r--   0        0        0    12077 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/array_module.py
--rw-r--r--   0        0        0     4754 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/cupy.py
--rw-r--r--   0        0        0     2036 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/jax.py
--rw-r--r--   0        0        0     2737 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/numpy.py
--rw-r--r--   0        0        0    13660 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/numpylike.py
--rw-r--r--   0        0        0     2330 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/shape.py
--rw-r--r--   0        0        0    42156 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/typetracer.py
--rw-r--r--   0        0        0     2527 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/ufuncs.py
--rw-r--r--   0        0        0       88 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/behaviors/__init__.py
--rw-r--r--   0        0        0     3479 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/behaviors/categorical.py
--rw-r--r--   0        0        0     3898 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/behaviors/mixins.py
--rw-r--r--   0        0        0     8509 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/behaviors/string.py
--rw-r--r--   0        0        0      986 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/__init__.py
--rw-r--r--   0        0        0    27770 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/bitmaskedarray.py
--rw-r--r--   0        0        0    40807 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/bytemaskedarray.py
--rw-r--r--   0        0        0    45218 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/content.py
--rw-r--r--   0        0        0    13230 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/emptyarray.py
--rw-r--r--   0        0        0    40314 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/indexedarray.py
--rw-r--r--   0        0        0    63394 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/indexedoptionarray.py
--rw-r--r--   0        0        0    59892 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/listarray.py
--rw-r--r--   0        0        0    85099 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/listoffsetarray.py
--rw-r--r--   0        0        0    49464 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/numpyarray.py
--rw-r--r--   0        0        0    40376 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/recordarray.py
--rw-r--r--   0        0        0    54508 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/regulararray.py
--rw-r--r--   0        0        0    56977 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/unionarray.py
--rw-r--r--   0        0        0    18810 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/unmaskedarray.py
--rw-r--r--   0        0        0      951 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/__init__.py
--rw-r--r--   0        0        0     6081 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/bitmaskedform.py
--rw-r--r--   0        0        0     5368 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/bytemaskedform.py
--rw-r--r--   0        0        0     3369 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/emptyform.py
--rw-r--r--   0        0        0    12414 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/form.py
--rw-r--r--   0        0        0     5638 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/indexedform.py
--rw-r--r--   0        0        0     5133 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/indexedoptionform.py
--rw-r--r--   0        0        0     5621 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/listform.py
--rw-r--r--   0        0        0     4715 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/listoffsetform.py
--rw-r--r--   0        0        0     6004 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/numpyform.py
--rw-r--r--   0        0        0     8208 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/recordform.py
--rw-r--r--   0        0        0     5084 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/regularform.py
--rw-r--r--   0        0        0     7760 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/unionform.py
--rw-r--r--   0        0        0     4229 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/unmaskedform.py
--rw-r--r--   0        0        0     4779 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/__init__.py
--rw-r--r--   0        0        0     3998 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_all.py
--rw-r--r--   0        0        0     5132 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_almost_equal.py
--rw-r--r--   0        0        0     4001 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_any.py
--rw-r--r--   0        0        0     5049 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_argcartesian.py
--rw-r--r--   0        0        0     3819 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_argcombinations.py
--rw-r--r--   0        0        0     6888 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_argmax.py
--rw-r--r--   0        0        0     6845 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_argmin.py
--rw-r--r--   0        0        0     3158 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_argsort.py
--rw-r--r--   0        0        0      915 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_backend.py
--rw-r--r--   0        0        0     9442 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_broadcast_arrays.py
--rw-r--r--   0        0        0     6522 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_broadcast_fields.py
--rw-r--r--   0        0        0    16000 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_cartesian.py
--rw-r--r--   0        0        0     1420 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_categories.py
--rw-r--r--   0        0        0     8118 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_combinations.py
--rw-r--r--   0        0        0    12195 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_concatenate.py
--rw-r--r--   0        0        0     2715 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_copy.py
--rw-r--r--   0        0        0     5817 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_corr.py
--rw-r--r--   0        0        0     5228 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_count.py
--rw-r--r--   0        0        0     4035 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_count_nonzero.py
--rw-r--r--   0        0        0     5170 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_covar.py
--rw-r--r--   0        0        0     4579 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_drop_none.py
--rw-r--r--   0        0        0     1106 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_fields.py
--rw-r--r--   0        0        0     5215 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_fill_none.py
--rw-r--r--   0        0        0     3432 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_firsts.py
--rw-r--r--   0        0        0     7802 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_flatten.py
--rw-r--r--   0        0        0     3154 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_arrow.py
--rw-r--r--   0        0        0      813 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_arrow_schema.py
--rw-r--r--   0        0        0     2727 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_avro_file.py
--rw-r--r--   0        0        0    14408 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_buffers.py
--rw-r--r--   0        0        0     1839 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_categorical.py
--rw-r--r--   0        0        0     1651 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_cupy.py
--rw-r--r--   0        0        0     4111 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_iter.py
--rw-r--r--   0        0        0     1716 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_jax.py
--rw-r--r--   0        0        0    30067 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_json.py
--rw-r--r--   0        0        0     2282 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_numpy.py
--rw-r--r--   0        0        0    11860 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_parquet.py
--rw-r--r--   0        0        0     3324 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_rdataframe.py
--rw-r--r--   0        0        0     2965 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_regular.py
--rw-r--r--   0        0        0     8859 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_full_like.py
--rw-r--r--   0        0        0      873 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_is_categorical.py
--rw-r--r--   0        0        0     2478 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_is_none.py
--rw-r--r--   0        0        0      705 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_is_tuple.py
--rw-r--r--   0        0        0      930 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_is_valid.py
--rw-r--r--   0        0        0     2568 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_isclose.py
--rw-r--r--   0        0        0     9122 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_linear_fit.py
--rw-r--r--   0        0        0     3258 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_local_index.py
--rw-r--r--   0        0        0     4757 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_mask.py
--rw-r--r--   0        0        0     7430 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_max.py
--rw-r--r--   0        0        0     9067 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_mean.py
--rw-r--r--   0        0        0     3532 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_merge_option_of_records.py
--rw-r--r--   0        0        0    12342 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_merge_union_of_records.py
--rw-r--r--   0        0        0     3217 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_metadata_from_parquet.py
--rw-r--r--   0        0        0     7382 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_min.py
--rw-r--r--   0        0        0     4908 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_moment.py
--rw-r--r--   0        0        0     2081 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_nan_to_none.py
--rw-r--r--   0        0        0     5103 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_nan_to_num.py
--rw-r--r--   0        0        0     3874 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_num.py
--rw-r--r--   0        0        0     1951 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_ones_like.py
--rw-r--r--   0        0        0     4362 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_pad_none.py
--rw-r--r--   0        0        0     1786 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_parameters.py
--rw-r--r--   0        0        0     6360 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_prod.py
--rw-r--r--   0        0        0     4710 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_ptp.py
--rw-r--r--   0        0        0     2275 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_ravel.py
--rw-r--r--   0        0        0     9531 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_run_lengths.py
--rw-r--r--   0        0        0     3028 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_singletons.py
--rw-r--r--   0        0        0     3339 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_softmax.py
--rw-r--r--   0        0        0     2670 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_sort.py
--rw-r--r--   0        0        0     8124 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_std.py
--rw-r--r--   0        0        0     3058 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_strings_astype.py
--rw-r--r--   0        0        0    11718 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_sum.py
--rw-r--r--   0        0        0     4931 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_arrow.py
--rw-r--r--   0        0        0     6725 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_arrow_table.py
--rw-r--r--   0        0        0     2325 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_backend.py
--rw-r--r--   0        0        0     6333 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_buffers.py
--rw-r--r--   0        0        0     6050 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_categorical.py
--rw-r--r--   0        0        0     1073 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_cupy.py
--rw-r--r--   0        0        0    13370 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_dataframe.py
--rw-r--r--   0        0        0     1074 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_jax.py
--rw-r--r--   0        0        0    11652 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_json.py
--rw-r--r--   0        0        0     4461 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_layout.py
--rw-r--r--   0        0        0     2612 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_list.py
--rw-r--r--   0        0        0     2088 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_numpy.py
--rw-r--r--   0        0        0     3354 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_packed.py
--rw-r--r--   0        0        0    16968 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_parquet.py
--rw-r--r--   0        0        0     2750 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_rdataframe.py
--rw-r--r--   0        0        0     3347 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_regular.py
--rw-r--r--   0        0        0    23906 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_transform.py
--rw-r--r--   0        0        0     4304 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_type.py
--rw-r--r--   0        0        0     9461 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_unflatten.py
--rw-r--r--   0        0        0     2484 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_unzip.py
--rw-r--r--   0        0        0     1138 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_validity_error.py
--rw-r--r--   0        0        0     2659 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_values_astype.py
--rw-r--r--   0        0        0     9352 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_var.py
--rw-r--r--   0        0        0     5502 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_where.py
--rw-r--r--   0        0        0     5065 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_with_field.py
--rw-r--r--   0        0        0     2610 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_with_name.py
--rw-r--r--   0        0        0     1848 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_with_parameter.py
--rw-r--r--   0        0        0     3756 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_without_field.py
--rw-r--r--   0        0        0     1509 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_without_parameters.py
--rw-r--r--   0        0        0     2134 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_zeros_like.py
--rw-r--r--   0        0        0     8819 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_zip.py
--rw-r--r--   0        0        0      707 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/__init__.py
--rw-r--r--   0        0        0   163323 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/_awkward_datashape_parser.py
--rw-r--r--   0        0        0     1914 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/arraytype.py
--rw-r--r--   0        0        0     2451 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/listtype.py
--rw-r--r--   0        0        0     5652 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/numpytype.py
--rw-r--r--   0        0        0     4180 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/optiontype.py
--rw-r--r--   0        0        0     8067 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/recordtype.py
--rw-r--r--   0        0        0     3133 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/regulartype.py
--rw-r--r--   0        0        0     1105 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/scalartype.py
--rw-r--r--   0        0        0     9622 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/type.py
--rw-r--r--   0        0        0     3725 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/uniontype.py
--rw-r--r--   0        0        0     1937 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/unknowntype.py
--rw-r--r--   0        0        0       88 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/__init__.py
--rw-r--r--   0        0        0     3358 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0002_minimal_listarray.py
--rw-r--r--   0        0        0      487 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0006_deep_iteration.py
--rw-r--r--   0        0        0     5565 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0008_slices_and_getitem.py
--rw-r--r--   0        0        0    13378 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0011_listarray.py
--rw-r--r--   0        0        0     4462 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0013_error_handling_struct.py
--rw-r--r--   0        0        0    17019 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0014_finish_up_getitem.py
--rw-r--r--   0        0        0     5169 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0018_fromiter_fillable.py
--rw-r--r--   0        0        0     8833 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0019_use_json_library.py
--rw-r--r--   0        0        0    13687 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0020_support_unsigned_indexes.py
--rw-r--r--   0        0        0     6391 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0021_emptyarray.py
--rw-r--r--   0        0        0    10743 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0023_regular_array.py
--rw-r--r--   0        0        0     4890 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0024_use_regular_array.py
--rw-r--r--   0        0        0    25581 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0025_record_array.py
--rw-r--r--   0        0        0     3436 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0028_add_dressed_types.py
--rw-r--r--   0        0        0     6361 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0032_replace_dressedtype.py
--rw-r--r--   0        0        0    12027 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0046_start_indexedarray.py
--rw-r--r--   0        0        0      898 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
--rw-r--r--   0        0        0    12231 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0057_introducing_forms.py
--rw-r--r--   0        0        0     5430 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0070_argmin_and_argmax.py
--rw-r--r--   0        0        0     5384 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0072_fillna_operation.py
--rw-r--r--   0        0        0    15655 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0074_argsort_and_sort.py
--rw-r--r--   0        0        0     2836 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0077_zip_operation.py
--rw-r--r--   0        0        0    11934 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0078_argcross_and_cross.py
--rw-r--r--   0        0        0    12124 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0079_argchoose_and_choose.py
--rw-r--r--   0        0        0     7071 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
--rw-r--r--   0        0        0     6579 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0084_start_unionarray.py
--rw-r--r--   0        0        0     6551 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0086_nep13_ufunc.py
--rw-r--r--   0        0        0    12540 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0089_numpy_functions.py
--rw-r--r--   0        0        0    46684 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0093_simplify_uniontypes_and_optiontypes.py
--rw-r--r--   0        0        0     6959 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0107_assign_fields_to_records.py
--rw-r--r--   0        0        0    46658 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0111_jagged_and_masked_getitem.py
--rw-r--r--   0        0        0    77224 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0115_generic_reducer_operation.py
--rw-r--r--   0        0        0    35084 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0118_numba_cpointers.py
--rw-r--r--   0        0        0     1091 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0119_numexpr_and_broadcast_arrays.py
--rw-r--r--   0        0        0     1106 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0124_strings_in_numba.py
--rw-r--r--   0        0        0    32114 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0127_tomask_operation.py
--rw-r--r--   0        0        0     3683 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0127b_tomask_operation_numba.py
--rw-r--r--   0        0        0      838 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0138_emptyarray_type.py
--rw-r--r--   0        0        0    17923 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0150_flatten.py
--rw-r--r--   0        0        0     3602 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0163_negative_axis_wrap.py
--rw-r--r--   0        0        0     9779 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0166_0167_0170_random_issues.py
--rw-r--r--   0        0        0     4552 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0173_astype_operation.py
--rw-r--r--   0        0        0    24034 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0184_concatenate_operation.py
--rw-r--r--   0        0        0     2063 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0193_is_none_axis_parameter.py
--rw-r--r--   0        0        0     3352 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0198_tutorial_documentation_1.py
--rw-r--r--   0        0        0     8998 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0222_count_with_axis0.py
--rw-r--r--   0        0        0    75605 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0224_arrow_to_awkward.py
--rw-r--r--   0        0        0      581 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0264_reduce_last_empty.py
--rw-r--r--   0        0        0     3251 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0273_path_for_with_field.py
--rw-r--r--   0        0        0      743 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0286_broadcast_single_value_with_field.py
--rw-r--r--   0        0        0     2205 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0290_bug_fixes_for_hats.py
--rw-r--r--   0        0        0     4806 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0315_integerindex.py
--rw-r--r--   0        0        0     5745 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0331_pandas_indexedarray.py
--rw-r--r--   0        0        0     1257 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0334_fully_broadcastable_where.py
--rw-r--r--   0        0        0      566 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0339_highlevel_sorting_function.py
--rw-r--r--   0        0        0     6757 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0348_form_keys.py
--rw-r--r--   0        0        0     4523 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0355_mixins.py
--rw-r--r--   0        0        0    10396 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0395_complex_type_arrays.py
--rw-r--r--   0        0        0     4934 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0395_fix_numba_indexedarray.py
--rw-r--r--   0        0        0     3077 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0397_arrays_as_constants_in_numba.py
--rw-r--r--   0        0        0    14529 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
--rw-r--r--   0        0        0    22467 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0404_array_validity_check.py
--rw-r--r--   0        0        0    14282 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0410_fix_argminmax_positions_for_missing_values.py
--rw-r--r--   0        0        0    17455 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0437_stream_of_many_json_files.py
--rw-r--r--   0        0        0    32921 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0447_preserve_regularness_in_reduce.py
--rw-r--r--   0        0        0    24075 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0449_merge_many_arrays_in_one_pass.py
--rw-r--r--   0        0        0     4059 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0493_zeros_ones_full_like.py
--rw-r--r--   0        0        0     1606 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0496_provide_local_index.py
--rw-r--r--   0        0        0     2059 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0499_getitem_indexedarray_bug.py
--rw-r--r--   0        0        0     1286 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0504_block_ufuncs_for_strings.py
--rw-r--r--   0        0        0     2926 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0511_copy_and_deepcopy.py
--rw-r--r--   0        0        0     9119 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
--rw-r--r--   0        0        0      365 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0546_fill_none_replacement_value_type.py
--rw-r--r--   0        0        0     1102 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0549_numba_array_asarray.py
--rw-r--r--   0        0        0     4268 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0557_min_max_initial_argument.py
--rw-r--r--   0        0        0      537 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0559_fix_booleans_in_numba.py
--rw-r--r--   0        0        0      636 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0572_numba_array_ndim.py
--rw-r--r--   0        0        0     4901 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0582_propagate_context_in_broadcast_and_apply.py
--rw-r--r--   0        0        0     1099 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0583_implement_unflatten_function.py
--rw-r--r--   0        0        0     3084 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0590_allow_regulararray_size_zero.py
--rw-r--r--   0        0        0     5957 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
--rw-r--r--   0        0        0      478 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0627_behavior_from_dict_of_arrays.py
--rw-r--r--   0        0        0     8205 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0652_tests_of_complex_numbers.py
--rw-r--r--   0        0        0     2338 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0674_categorical_validation.py
--rw-r--r--   0        0        0      750 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0713_getitem_field_should_simplify_optiontype.py
--rw-r--r--   0        0        0     1242 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
--rw-r--r--   0        0        0     1055 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0730_unflatten_axis_parameter.py
--rw-r--r--   0        0        0     2569 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0733_run_lengths.py
--rw-r--r--   0        0        0     2127 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0736_implement_argsort_for_strings.py
--rw-r--r--   0        0        0      330 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0758_ak_zip_scallars.py
--rw-r--r--   0        0        0     1122 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0766_prevent_combinations_of_characters.py
--rw-r--r--   0        0        0    26349 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0773_typeparser.py
--rw-r--r--   0        0        0      779 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
--rw-r--r--   0        0        0      871 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0794_ak_cartesian_on_empty_array.py
--rw-r--r--   0        0        0     1148 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0803_argsort_fix_type.py
--rw-r--r--   0        0        0     1364 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0806_empty_lists_cartesian_fix.py
--rw-r--r--   0        0        0     6311 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0813_full_like_dtype_arg.py
--rw-r--r--   0        0        0     1661 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0815_broadcast_union_types_to_all_possibilities.py
--rw-r--r--   0        0        0      488 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0819_issue.py
--rw-r--r--   0        0        0      682 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0828_arrow_datatype_null.py
--rw-r--r--   0        0        0    23609 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0835_datetime_type.py
--rw-r--r--   0        0        0      676 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0835_datetime_type_pandas.py
--rw-r--r--   0        0        0     4662 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0835_datetime_type_pyarrow.py
--rw-r--r--   0        0        0      680 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0850_argsort_mask_array.py
--rw-r--r--   0        0        0      449 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0863_is_none_numpy_array.py
--rw-r--r--   0        0        0     1029 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0866_getitem_field_and_flatten_unions.py
--rw-r--r--   0        0        0      929 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0875_arrow_null_type.py
--rw-r--r--   0        0        0      901 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0879_non_primitive_with_field.py
--rw-r--r--   0        0        0      563 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0884_index_and_identifier_refactoring.py
--rw-r--r--   0        0        0     1086 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0889_ptp.py
--rw-r--r--   0        0        0    53355 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0896_content_classes_refactoring.py
--rw-r--r--   0        0        0     1751 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0898_unzip_heterogeneous_records.py
--rw-r--r--   0        0        0      421 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
--rw-r--r--   0        0        0      530 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0905_leading_zeros_in_unflatten.py
--rw-r--r--   0        0        0     1048 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0906_arrow_fixed_size_list_type.py
--rw-r--r--   0        0        0      666 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0910_unflatten_counts_relation.py
--rw-r--r--   0        0        0     5261 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0912_packed.py
--rw-r--r--   0        0        0   115760 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0914_types_and_forms.py
--rw-r--r--   0        0        0     1877 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0916_datetime_values_astype.py
--rw-r--r--   0        0        0     5522 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0927_numpy_array_nbytes.py
--rw-r--r--   0        0        0      709 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0930_bug_in_unionarray_purelist_parameter.py
--rw-r--r--   0        0        0     1627 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0945_argsort_sort_nan_array.py
--rw-r--r--   0        0        0    28028 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0958_new_forms_must_accept_old_form_json.py
--rw-r--r--   0        0        0    28284 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0959__getitem_array_implementation.py
--rw-r--r--   0        0        0      651 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0975_mask_multidimensional_numpy_array.py
--rw-r--r--   0        0        0      644 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0979_where_multidimentional_numpy_array.py
--rw-r--r--   0        0        0     5803 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0982_missing_case_in_nonlocal_reducers.py
--rw-r--r--   0        0        0     1976 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0984_ravel.py
--rw-r--r--   0        0        0     1806 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0992_correct_ptp_unmasking.py
--rw-r--r--   0        0        0     2100 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
--rw-r--r--   0        0        0      429 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1006_packed_regular_array_zero_size.py
--rw-r--r--   0        0        0      416 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1007_from_buffers_empty_ndarray.py
--rw-r--r--   0        0        0      551 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1017_numpyarray_broadcast.py
--rw-r--r--   0        0        0      785 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1030_mixin_class_name.py
--rw-r--r--   0        0        0    52114 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1031_start_getitem_next.py
--rw-r--r--   0        0        0    18007 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1031b_start_getitem_next_specialized.py
--rw-r--r--   0        0        0     1146 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1049_concatenate_single_array.py
--rw-r--r--   0        0        0     1559 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1055_fill_none_numpy_dimension.py
--rw-r--r--   0        0        0    42250 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1059_localindex.py
--rw-r--r--   0        0        0      551 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1066_to_numpy_masked_structured_array.py
--rw-r--r--   0        0        0      685 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1071_mask_identity_false_should_not_return_option_type.py
--rw-r--r--   0        0        0    27714 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1072_sort.py
--rw-r--r--   0        0        0    44140 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1074_combinations.py
--rw-r--r--   0        0        0     5181 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1075_validityerror.py
--rw-r--r--   0        0        0      273 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1106_argminmax_axis_None_missing_values.py
--rw-r--r--   0        0        0    25531 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1110_type_tracer_1.py
--rw-r--r--   0        0        0     1870 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1116_project_maskedarrays.py
--rw-r--r--   0        0        0    28234 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1125_to_arrow_from_arrow.py
--rw-r--r--   0        0        0     6276 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1132_utility_methods_for_highlevel_functions.py
--rw-r--r--   0        0        0    21098 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1134_from_buffers_to_buffers.py
--rw-r--r--   0        0        0    57322 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1135_rpad_operation.py
--rw-r--r--   0        0        0     4639 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1136_regulararray_zeros_in_shape.py
--rw-r--r--   0        0        0    10487 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1137_num.py
--rw-r--r--   0        0        0    10222 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1142_numbers_to_type.py
--rw-r--r--   0        0        0     2559 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1149_datetime_sort.py
--rw-r--r--   0        0        0      630 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1154_arrow_tables_should_preserve_parameters.py
--rw-r--r--   0        0        0    27983 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1162_ak_from_json_schema.py
--rw-r--r--   0        0        0      766 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1183_bugs_found_by_dask_project_2.py
--rw-r--r--   0        0        0     1286 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1189_fix_singletons_for_non_optional_data.py
--rw-r--r--   0        0        0      551 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1192_iterables_in___array_function__.py
--rw-r--r--   0        0        0      608 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1193_is_none_nested_option.py
--rw-r--r--   0        0        0     2601 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1233_ak_with_name.py
--rw-r--r--   0        0        0    26467 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1240_v2_implementation_of_numba_1.py
--rw-r--r--   0        0        0     1146 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1259_simplify_optiontype.py
--rw-r--r--   0        0        0     1560 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1260_simplify_masked_option_types.py
--rw-r--r--   0        0        0      681 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1271_fix_4D_reducers.py
--rw-r--r--   0        0        0    33003 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1294_to_and_from_parquet.py
--rw-r--r--   0        0        0     1945 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
--rw-r--r--   0        0        0    62340 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1300_awkward_to_cpp_converter_with_cling.py
--rw-r--r--   0        0        0    39474 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1300b_same_for_numba.py
--rw-r--r--   0        0        0      367 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1305_mixed_awkward_numpy_slicing.py
--rw-r--r--   0        0        0     1702 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1308_zip_after_option.py
--rw-r--r--   0        0        0     1703 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1318_array_function_types.py
--rw-r--r--   0        0        0     1730 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1320_mask_identity_defaults.py
--rw-r--r--   0        0        0      647 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1344_broadcast_arrays_depth_limit.py
--rw-r--r--   0        0        0     6621 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1345_avro_reader.py
--rw-r--r--   0        0        0     4562 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1351_is_tuple.py
--rw-r--r--   0        0        0     8362 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1374_to_rdataframe.py
--rw-r--r--   0        0        0     1755 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1377_ravel_string.py
--rw-r--r--   0        0        0     1468 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1379_reducers_with_axis_None_and_typetracers.py
--rw-r--r--   0        0        0     1384 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1399_from_jax.py
--rw-r--r--   0        0        0     1227 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1399_to_jax.py
--rw-r--r--   0        0        0      297 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1400_with_name_record.py
--rw-r--r--   0        0        0      449 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1403_from_numpy_strings.py
--rw-r--r--   0        0        0     3470 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1405_slicing_untested_cases.py
--rw-r--r--   0        0        0     6909 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1415_behaviour_forwarding.py
--rw-r--r--   0        0        0    18809 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1440_start_v2_to_parquet.py
--rw-r--r--   0        0        0    14402 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1447_jax_autodiff_slices_ufuncs.py
--rw-r--r--   0        0        0     8591 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1449_v2_to_json_from_json_functions.py
--rw-r--r--   0        0        0      692 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1453_write_single_records_to_parquet.py
--rw-r--r--   0        0        0     9828 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1473_from_rdataframe.py
--rw-r--r--   0        0        0    24648 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1477_generator_entry_type_as_rvec.py
--rw-r--r--   0        0        0     3579 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1490_jax_reducers_combinations.py
--rw-r--r--   0        0        0     3905 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1502_getitem_jagged_issue1406.py
--rw-r--r--   0        0        0     1733 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1504_typetracer_like.py
--rw-r--r--   0        0        0     4913 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1508_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     2186 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1511_set_attribute.py
--rw-r--r--   0        0        0      754 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1539_isnone_axis_check_issue1417.py
--rw-r--r--   0        0        0     1570 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1559_fix_ufuncs_records_1439.py
--rw-r--r--   0        0        0      990 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1565_axis_wrap_if_negative_record.py
--rw-r--r--   0        0        0     1080 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1567_fix_longlong_in_Index.py
--rw-r--r--   0        0        0     3022 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1568_fix_lengths_empty_regular_slices.py
--rw-r--r--   0        0        0      385 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1578_to_arrow_empty_recordarray.py
--rw-r--r--   0        0        0     5911 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1586_concatenate_should_preserve_regulararray.py
--rw-r--r--   0        0        0      216 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1593_empty_slice_list_record.py
--rw-r--r--   0        0        0     7260 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1604_preserve_form_in_concatenate.py
--rw-r--r--   0        0        0     3636 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1607_no_reducers_on_records.py
--rw-r--r--   0        0        0    10035 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1613_generator_tolayout_records.py
--rw-r--r--   0        0        0      727 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1619_from_parquet_empty_field.py
--rw-r--r--   0        0        0     6024 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1620_layout_builders.py
--rw-r--r--   0        0        0     8122 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1625_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0      770 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1642_from_iter_of_tuples.py
--rw-r--r--   0        0        0      389 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1644_concatenate_zeros_length.py
--rw-r--r--   0        0        0     4317 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1650_Record_to_list_should_listify_itself.py
--rw-r--r--   0        0        0      560 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1671_categorical_type.py
--rw-r--r--   0        0        0    11761 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1672_broadcast_parameters.py
--rw-r--r--   0        0        0     4453 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1677_array_builder_in_numba.py
--rw-r--r--   0        0        0      544 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1685_IndexedArray_project_parameters.py
--rw-r--r--   0        0        0      778 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1686_UnionArray_simplified_preserve_parameters.py
--rw-r--r--   0        0        0      936 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1688_pack_categorical.py
--rw-r--r--   0        0        0      525 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1703_fill_none_typetracer.py
--rw-r--r--   0        0        0     1743 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1707_broadcast_parameters_ufunc.py
--rw-r--r--   0        0        0      512 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1709_ak_array_constructor_behavior.py
--rw-r--r--   0        0        0      398 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1735_from_numpy_mask.py
--rw-r--r--   0        0        0      577 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1747_bytemaskedarray_mergemany.py
--rw-r--r--   0        0        0      824 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1753_indexedarray_merge_kernel.py
--rw-r--r--   0        0        0     1480 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1762_jax_behavior_support.py
--rw-r--r--   0        0        0      589 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1764_jax_jacobian.py
--rw-r--r--   0        0        0      962 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1765_add_ioanas_test_of_to_arraylib.py
--rw-r--r--   0        0        0     4790 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1766_record_form_fields.py
--rw-r--r--   0        0        0     2905 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1781_rdataframe_snapshot.py
--rw-r--r--   0        0        0      701 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1784_reduce_leading_sublist.py
--rw-r--r--   0        0        0      567 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1790_reduce_regulararray.py
--rw-r--r--   0        0        0     4191 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1791_reduce_trailing_sublist.py
--rw-r--r--   0        0        0     1027 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1794_run_lengths_empty_sublist.py
--rw-r--r--   0        0        0      407 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1823_fill_none_axis_none.py
--rw-r--r--   0        0        0      481 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1826_ravel_preserve_none.py
--rw-r--r--   0        0        0     1451 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1829_to_from_rdataframe_bool.py
--rw-r--r--   0        0        0      588 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
--rw-r--r--   0        0        0     1097 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1847_numpy_array_contiguous.py
--rw-r--r--   0        0        0      681 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
--rw-r--r--   0        0        0     1640 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1867_pass_behavior_through_combinations.py
--rw-r--r--   0        0        0    17239 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1904_drop_none.py
--rw-r--r--   0        0        0     3553 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1914_improved_axis_to_posaxis.py
--rw-r--r--   0        0        0     3444 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
--rw-r--r--   0        0        0      921 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1930_unflatten_counts_checks.py
--rw-r--r--   0        0        0      769 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1936_with_field_broadcasting.py
--rw-r--r--   0        0        0      551 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1940_ak_backend.py
--rw-r--r--   0        0        0     1457 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1943_regular_indexing.py
--rw-r--r--   0        0        0      188 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1944_to_numpy_empty_record_array.py
--rw-r--r--   0        0        0     1131 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1960_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     3286 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1961_ak_without_field.py
--rw-r--r--   0        0        0      280 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1978_akRecord_constructor_should_retain_type.py
--rw-r--r--   0        0        0      349 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
--rw-r--r--   0        0        0      371 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2008_ak_type_layout.py
--rw-r--r--   0        0        0    10222 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2020_reduce_axis_none.py
--rw-r--r--   0        0        0      803 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2021_check_TypeTracerArray_in_ak_where.py
--rw-r--r--   0        0        0      645 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2023_from_rdataframe.py
--rw-r--r--   0        0        0     2854 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
--rw-r--r--   0        0        0     1219 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2047_ak_transform_regular_to_jagged.py
--rw-r--r--   0        0        0      406 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2051_arraybuilder_behavior_propagation.py
--rw-r--r--   0        0        0     1275 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2055_array_builder_check.py
--rw-r--r--   0        0        0     1659 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2058_merge_numpy_array.py
--rw-r--r--   0        0        0      708 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2064_fill_none_record.py
--rw-r--r--   0        0        0      799 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2067_to_buffers_byteorder.py
--rw-r--r--   0        0        0      741 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2070_to_layout_string.py
--rw-r--r--   0        0        0     1172 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2071_unflatten_non_packed_counts.py
--rw-r--r--   0        0        0      291 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2076_ak_unzip_record.py
--rw-r--r--   0        0        0      545 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2078_array_function_wrap.py
--rw-r--r--   0        0        0      589 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2082_broadcast_zero_size.py
--rw-r--r--   0        0        0     2765 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2096_ak_scalar_type.py
--rw-r--r--   0        0        0      977 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2101_pickle_behavior_class.py
--rw-r--r--   0        0        0      519 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2104_numpy_merge_option.py
--rw-r--r--   0        0        0     2715 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2106_pickle_class.py
--rw-r--r--   0        0        0      722 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2108_fill_none_indexed.py
--rw-r--r--   0        0        0     2100 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2115_fix_up_typetracers.py
--rw-r--r--   0        0        0      487 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2120_missing_field_error.py
--rw-r--r--   0        0        0     1110 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2125_type_of_scalar.py
--rw-r--r--   0        0        0     1893 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2150_typetracer_high_level_ufunc.py
--rw-r--r--   0        0        0     1898 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2179_parameter_merging_rules.py
--rw-r--r--   0        0        0      510 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2181_with_name_len.py
--rw-r--r--   0        0        0     2957 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2185_merge_union_of_records.py
--rw-r--r--   0        0        0      528 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
--rw-r--r--   0        0        0     5548 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2198_almost_equal.py
--rw-r--r--   0        0        0     1252 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2202_filter_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0     1453 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2214_offset_bool_index.py
--rw-r--r--   0        0        0      334 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2219_flatten_empty.py
--rw-r--r--   0        0        0      663 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2226_slice_regulararray_typetracer.py
--rw-r--r--   0        0        0     1728 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2229_getitem_range_slice.py
--rw-r--r--   0        0        0     4003 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2234_from_rdataframe_keep_order.py
--rw-r--r--   0        0        0     3962 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2236_merge_union_of_records_option.py
--rw-r--r--   0        0        0      485 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2240_merge_union_parameters.py
--rw-r--r--   0        0        0     1338 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2240_simplify_merge_as_union.py
--rw-r--r--   0        0        0      512 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2246_slice_not_packed.py
--rw-r--r--   0        0        0      733 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2250_full_like_bool.py
--rw-r--r--   0        0        0     1835 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2258_from_rdataframe_with_arguments.py
--rw-r--r--   0        0        0      492 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2259_run_lengths_typetracer.py
--rw-r--r--   0        0        0      549 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2263_to_packed_list.py
--rw-r--r--   0        0        0      877 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2266_fix_nan_to_num.py
--rw-r--r--   0        0        0      909 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2267_broadcast_fields.py
--rw-r--r--   0        0        0     1336 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2293_unflatten_typetracer.py
--rw-r--r--   0        0        0      406 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2294_view_unknown_scalar.py
--rw-r--r--   0        0        0     2301 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2297_common_backend.py
--rw-r--r--   0        0        0      455 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2304_index_typetracer.py
--rw-r--r--   0        0        0     2929 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2306_cppyy_git.py
--rw-r--r--   0        0        0     4386 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2319_from_buffers_array.py
--rw-r--r--   0        0        0      865 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2327_array_interface.py
--rw-r--r--   0        0        0     1728 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2329_cartesian_broadcasting_fixes.py
--rw-r--r--   0        0        0      489 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2346_broadcast_depth_limit.py
--rw-r--r--   0        0        0    15576 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2349_growablebuffer_in_numba.py
--rw-r--r--   0        0        0      618 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2354_ufunc_same_backend.py
--rw-r--r--   0        0        0      601 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2355_to_backend_record.py
--rw-r--r--   0        0        0     1435 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2361_typetracer_asarray_nd.py
--rw-r--r--   0        0        0     2921 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2368_type_is_equal.py
--rw-r--r--   0        0        0     5259 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2373_unzip_touching.py
--rw-r--r--   0        0        0     5857 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2374_cartesian_touching.py
--rw-r--r--   0        0        0      128 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/__init__.py
--rw-r--r--   0        0        0      218 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/array_enum_test_data.avro
--rw-r--r--   0        0        0      176 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/array_string_test_data.avro
--rw-r--r--   0        0        0      152 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/array_test_data.avro
--rw-r--r--   0        0        0      115 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/bool_test_data.avro
--rw-r--r--   0        0        0      130 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/bytes_test_data.avro
--rw-r--r--   0        0        0      158 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/double_test_data.avro
--rw-r--r--   0        0        0      191 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/enum_null_test_data.avro
--rw-r--r--   0        0        0      180 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/enum_test_data.avro
--rw-r--r--   0        0        0      218 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/fixed_test_data.avro
--rw-r--r--   0        0        0      116 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/float_test_data.avro
--rw-r--r--   0        0        0      106 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/int_null_test_data.avro
--rw-r--r--   0        0        0      128 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/int_string_null_test_data.avro
--rw-r--r--   0        0        0       89 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/int_test_data.avro
--rw-r--r--   0        0        0     3035 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/list-depths-records-list.parquet
--rw-r--r--   0        0        0     2871 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/list-depths-records.parquet
--rw-r--r--   0        0        0      497 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/list-depths-simple.parquet
--rw-r--r--   0        0        0     1136 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/list-depths-strings.parquet
--rw-r--r--   0        0        0     1060 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/list-depths.parquet
--rw-r--r--   0        0        0      465 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/list-lengths.parquet
--rw-r--r--   0        0        0      116 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/long_test_data.avro
--rw-r--r--   0        0        0      681 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nonnullable-depths.parquet
--rw-r--r--   0        0        0       75 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/null_test_data.avro
--rw-r--r--   0        0        0      719 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-depths.parquet
--rw-r--r--   0        0        0      635 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-levels.parquet
--rw-r--r--   0        0        0     3050 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-list-depths-records-list.parquet
--rw-r--r--   0        0        0     2926 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-list-depths-records.parquet
--rw-r--r--   0        0        0     1179 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-list-depths-strings.parquet
--rw-r--r--   0        0        0     1101 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-list-depths.parquet
--rw-r--r--   0        0        0      430 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-record-primitives-simple.parquet
--rw-r--r--   0        0        0     1181 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-record-primitives.parquet
--rw-r--r--   0        0        0     1193 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/record-primitives.parquet
--rw-r--r--   0        0        0      326 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/record_0_test_data.avro
--rw-r--r--   0        0        0      368 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/record_1_test_data.avro
--rw-r--r--   0        0        0      263 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/record_null_test_data.avro
--rw-r--r--   0        0        0      423 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/record_test_data.avro
--rw-r--r--   0        0        0      116 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/string_null_test_data.avro
--rw-r--r--   0        0        0      125 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/string_test_data.avro
--rw-r--r--   0        0        0      544 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/test-nan-inf.json
--rw-r--r--   0        0        0      155 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/test-record-array.json
--rw-r--r--   0        0        0      803 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/test-two-arrays.json
--rw-r--r--   0        0        0      535 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/test.json
--rw-r--r--   0        0        0      180 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/zero-record-batches.parquet
--rw-r--r--   0        0        0       88 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/__init__.py
--rw-r--r--   0        0        0     7072 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/test_1276_cuda_num.py
--rw-r--r--   0        0        0     9911 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/test_1276_cuda_transfers.py
--rw-r--r--   0        0        0     1197 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/test_1276_cupy_interop.py
--rw-r--r--   0        0        0     1782 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/test_1276_from_cupy.py
--rw-r--r--   0        0        0    42786 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/test_1300_same_for_numba_cuda.py
--rw-r--r--   0        0        0      834 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/test_1381_check_errors.py
--rw-r--r--   0        0        0    11252 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/test_1809_array_cuda_jit.py
--rw-r--r--   0        0        0     2212 2023-04-08 19:13:43.000000 awkward-2.1.2/.gitignore
--rw-r--r--   0        0        0     1520 2023-04-08 19:13:43.000000 awkward-2.1.2/LICENSE
--rw-r--r--   0        0        0     8479 2023-04-08 19:13:43.000000 awkward-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     6933 2023-04-08 19:13:43.000000 awkward-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1893 2023-04-13 15:38:23.000000 awkward-2.1.3/CITATION.cff
+-rw-r--r--   0        0        0    13578 2023-04-13 15:38:23.000000 awkward-2.1.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0    22687 2023-04-13 15:38:23.000000 awkward-2.1.3/README.md
+-rw-r--r--   0        0        0      241 2023-04-13 15:38:23.000000 awkward-2.1.3/requirements-test.txt
+-rw-r--r--   0        0        0     7833 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/_toc.yml
+-rw-r--r--   0        0        0     7624 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/conf.py
+-rw-r--r--   0        0        0      346 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/environment.yml.cog
+-rw-r--r--   0        0        0     2603 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/index.md
+-rw-r--r--   0        0        0    11642 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/prepare_docstrings.py
+-rw-r--r--   0        0        0     4448 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/redirects-user-guide.json
+-rw-r--r--   0        0        0    11436 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/redirects.json
+-rw-r--r--   0        0        0      463 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/requirements.txt
+-rw-r--r--   0        0        0      369 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/switcher.json
+-rw-r--r--   0        0        0      930 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/_static/css/awkward.css
+-rw-r--r--   0        0        0      354 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/_static/css/try-awkward-array.css
+lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
+lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0      469 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/_templates/funding.html
+-rw-r--r--   0        0        0      474 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/_templates/redirect.html
+-rw-r--r--   0        0        0     2968 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/getting-started/community-tutorials.md
+-rw-r--r--   0        0        0     4654 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/getting-started/index.md
+-rw-r--r--   0        0        0     3346 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/getting-started/papers-and-talks.md
+-rw-r--r--   0        0        0       82 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/getting-started/try-awkward-array.md
+lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    12847 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/getting-started/demo/what-is-an-awkward-array.ipynb
+lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
+lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
+lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
+lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    17067 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/example-hierarchy.svg
+lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
+lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
+lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
+lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
+lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
+lrwxr-xr-x   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    25309 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/reference/ak.behavior.rst
+-rw-r--r--   0        0        0     1430 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/reference/ak.builder.ArrayBuilder.rst
+-rw-r--r--   0        0        0    64727 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/reference/awkwardforth.rst
+-rw-r--r--   0        0        0      270 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/reference/index.md
+-rw-r--r--   0        0        0     7252 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/reference/toctree.txt
+-rw-r--r--   0        0        0     8320 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/10-minutes-to-awkward-array.md
+-rw-r--r--   0        0        0      926 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-combinatorics-best-match.md
+-rw-r--r--   0        0        0      930 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
+-rw-r--r--   0        0        0      263 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-combinatorics.md
+-rw-r--r--   0        0        0     8335 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert-arrow.md
+-rw-r--r--   0        0        0     6392 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert-buffers.md
+-rw-r--r--   0        0        0     2455 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert-json.md
+-rw-r--r--   0        0        0    13475 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert-numpy.md
+-rw-r--r--   0        0        0     7182 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert-pandas.md
+-rw-r--r--   0        0        0    18830 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert-python.md
+-rw-r--r--   0        0        0     3554 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert-rdataframe.md
+-rw-r--r--   0        0        0      271 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-convert.md
+-rw-r--r--   0        0        0    11973 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create-arraybuilder.md
+-rw-r--r--   0        0        0    36520 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create-constructors.md
+-rw-r--r--   0        0        0     7383 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create-lists.md
+-rw-r--r--   0        0        0     7456 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create-missing.md
+-rw-r--r--   0        0        0    11542 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create-records.md
+-rw-r--r--   0        0        0     4066 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create-strings.md
+-rw-r--r--   0        0        0      866 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create-unflatten-group.md
+-rw-r--r--   0        0        0      267 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-create.md
+-rw-r--r--   0        0        0      834 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-examine-checking-validity.md
+-rw-r--r--   0        0        0     2919 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-examine-list-fields.md
+-rw-r--r--   0        0        0      848 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-examine-simple-slicing.md
+-rw-r--r--   0        0        0      838 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-examine-single-item.md
+-rw-r--r--   0        0        0     6778 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-examine-type.md
+-rw-r--r--   0        0        0      269 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-examine.md
+-rw-r--r--   0        0        0      844 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-filter-cut-mask.md
+-rw-r--r--   0        0        0     3889 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-filter-masked.md
+-rw-r--r--   0        0        0      840 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-filter-num.md
+-rw-r--r--   0        0        0     7955 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-filter-ragged.md
+-rw-r--r--   0        0        0      265 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-filter.md
+-rw-r--r--   0        0        0      818 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-math-argminmax.md
+-rw-r--r--   0        0        0      822 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-math-broadcasting.md
+-rw-r--r--   0        0        0      828 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-math-gpu.md
+-rw-r--r--   0        0        0      838 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-math-numpy.md
+-rw-r--r--   0        0        0      846 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-math-reducing.md
+-rw-r--r--   0        0        0      870 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-math-statistics.md
+-rw-r--r--   0        0        0      265 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-math.md
+-rw-r--r--   0        0        0     3411 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure-add-fields.md
+-rw-r--r--   0        0        0      842 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure-concatenate.md
+-rw-r--r--   0        0        0    19083 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure-flatten.md
+-rw-r--r--   0        0        0     7568 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure-pad.md
+-rw-r--r--   0        0        0      852 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure-rename-records.md
+-rw-r--r--   0        0        0      832 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure-sort.md
+-rw-r--r--   0        0        0     9624 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure-zip-project.md
+-rw-r--r--   0        0        0      273 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-restructure.md
+-rw-r--r--   0        0        0     2599 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-specialize-differentiate-jax.md
+-rw-r--r--   0        0        0      870 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-specialize-in-numba.md
+-rw-r--r--   0        0        0      838 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-specialize-lorentz.md
+-rw-r--r--   0        0        0      874 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-specialize-override-numpy.md
+-rw-r--r--   0        0        0      870 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-specialize-subclass.md
+-rw-r--r--   0        0        0      277 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-specialize.md
+-rw-r--r--   0        0        0    11724 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-use-header-only-layoutbuilder.md
+-rw-r--r--   0        0        0      900 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-use-in-numba-arraybuilder.md
+-rw-r--r--   0        0        0     9973 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-use-in-numba-cuda.ipynb
+-rw-r--r--   0        0        0      900 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-use-in-numba-features.md
+-rw-r--r--   0        0        0      279 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/how-to-use-in-numba.md
+-rw-r--r--   0        0        0      344 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/index.md
+-rw-r--r--   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/docs/user-guide/requirements.txt
+-rw-r--r--   0        0        0   367587 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-data-analysts.png
+-rw-r--r--   0        0        0   794465 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-data-analysts.svg
+-rw-r--r--   0        0        0   140700 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-developers.png
+-rw-r--r--   0        0        0   328307 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-developers.svg
+-rw-r--r--   0        0        0    73584 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-doxygen.png
+-rw-r--r--   0        0        0    58179 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-sphinx.png
+-rw-r--r--   0        0        0   127063 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-tutorials-alternate.png
+-rw-r--r--   0        0        0   173327 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/panel-tutorials.png
+-rw-r--r--   0        0        0    12541 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-1-0-layers.pdf
+-rw-r--r--   0        0        0    65246 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-1-0-layers.png
+-rw-r--r--   0        0        0    41004 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-1-0-layers.svg
+-rw-r--r--   0        0        0    14946 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-timeline.pdf
+-rw-r--r--   0        0        0   125180 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-timeline.png
+-rw-r--r--   0        0        0    70209 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-timeline.svg
+-rw-r--r--   0        0        0   436595 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
+-rw-r--r--   0        0        0   426911 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
+-rw-r--r--   0        0        0   335955 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip.png
+-rw-r--r--   0        0        0   325268 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip.svg
+-rw-r--r--   0        0        0   129696 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline.png
+-rw-r--r--   0        0        0   120554 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline.svg
+-rw-r--r--   0        0        0     5208 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-broadcasting.png
+-rw-r--r--   0        0        0    25065 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-broadcasting.svg
+-rw-r--r--   0        0        0     5754 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-cartesian.png
+-rw-r--r--   0        0        0    32616 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-cartesian.svg
+-rw-r--r--   0        0        0     9584 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-combinations.png
+-rw-r--r--   0        0        0    39524 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-combinations.svg
+-rw-r--r--   0        0        0    10808 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-schematic.png
+-rw-r--r--   0        0        0    25779 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/cartoon-schematic.svg
+-rw-r--r--   0        0        0    18178 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    36024 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/example-hierarchy.png
+-rw-r--r--   0        0        0    17092 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/example-hierarchy.svg
+-rw-r--r--   0        0        0    21120 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/example-reduction-sum-only.svg
+-rw-r--r--   0        0        0    29325 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    55553 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/example-reduction.png
+-rw-r--r--   0        0        0    21631 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/example-reduction.svg
+-rw-r--r--   0        0        0    10978 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/git-strategy.pdf
+-rw-r--r--   0        0        0    58904 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/git-strategy.png
+-rw-r--r--   0        0        0    28990 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/git-strategy.svg
+-rw-r--r--   0        0        0   113587 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/how-it-works-muons.png
+-rw-r--r--   0        0        0    57471 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/how-it-works-muons.svg
+-rw-r--r--   0        0        0    58475 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/how-it-works.svg
+-rw-r--r--   0        0        0    63989 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/sorting-axis.svg
+-rw-r--r--   0        0        0   124038 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/all.svg
+-rw-r--r--   0        0        0   128558 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/any.svg
+-rw-r--r--   0        0        0   134490 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/argmax.svg
+-rw-r--r--   0        0        0   133192 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/argmin.svg
+-rw-r--r--   0        0        0   106277 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/count.svg
+-rw-r--r--   0        0        0   116417 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/count_nonzero.svg
+-rw-r--r--   0        0        0   111789 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/max.svg
+-rw-r--r--   0        0        0   109239 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/min.svg
+-rw-r--r--   0        0        0   124702 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/product.svg
+-rw-r--r--   0        0        0   108897 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/diagrams/reducers/sum.svg
+-rw-r--r--   0        0        0     8347 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/logo/favicon.ico
+-rw-r--r--   0        0        0     8984 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/logo/logo-300px-white.png
+-rw-r--r--   0        0        0    11964 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    24707 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/logo/logo-600px.png
+-rw-r--r--   0        0        0    18767 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/logo/logo.svg
+-rw-r--r--   0        0        0    90413 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/photos/desire-path.jpg
+-rw-r--r--   0        0        0    52113 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/plots/awkward-0-popularity.pdf
+-rw-r--r--   0        0        0   146109 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/plots/awkward-0-popularity.png
+-rw-r--r--   0        0        0   147576 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/plots/awkward-0-popularity.svg
+-rw-r--r--   0        0        0    26938 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/plots/bikeroutes-scaling.svg
+-rw-r--r--   0        0        0     8891 2023-04-13 15:38:23.000000 awkward-2.1.3/docs-img/screenshots/github-issues-documentation.png
+-rw-r--r--   0        0        0     1325 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/__init__.py
+-rw-r--r--   0        0        0     5418 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_behavior.py
+-rw-r--r--   0        0        0    38046 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_broadcasting.py
+-rw-r--r--   0        0        0    13398 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_do.py
+-rw-r--r--   0        0        0    11999 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_errors.py
+-rw-r--r--   0        0        0     5672 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_kernels.py
+-rw-r--r--   0        0        0     5825 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_layout.py
+-rw-r--r--   0        0        0     9983 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_lookup.py
+-rw-r--r--   0        0        0     5454 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_parameters.py
+-rw-r--r--   0        0        0     9965 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_prettyprint.py
+-rw-r--r--   0        0        0    24569 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_reducers.py
+-rw-r--r--   0        0        0     2041 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_regularize.py
+-rw-r--r--   0        0        0      420 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_singleton.py
+-rw-r--r--   0        0        0    23934 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_slicing.py
+-rw-r--r--   0        0        0      647 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_typetracer.py
+-rw-r--r--   0        0        0     1163 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_typing.py
+-rw-r--r--   0        0        0     2439 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_util.py
+-rw-r--r--   0        0        0      758 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_v2.py
+-rw-r--r--   0        0        0      233 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/builder.py
+-rw-r--r--   0        0        0      866 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/cppyy.py
+-rw-r--r--   0        0        0      271 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forth.py
+-rw-r--r--   0        0        0   103301 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/highlevel.py
+-rw-r--r--   0        0        0     8005 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/index.py
+-rw-r--r--   0        0        0     3988 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/jax.py
+-rw-r--r--   0        0        0     2764 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/numba.py
+-rw-r--r--   0        0        0     8272 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/record.py
+-rw-r--r--   0        0        0      165 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/typetracer.py
+-rw-r--r--   0        0        0        0 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_backends/__init__.py
+-rw-r--r--   0        0        0     1336 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_backends/backend.py
+-rw-r--r--   0        0        0     1259 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_backends/cupy.py
+-rw-r--r--   0        0        0     3574 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_backends/dispatch.py
+-rw-r--r--   0        0        0     1781 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_backends/jax.py
+-rw-r--r--   0        0        0      944 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_backends/numpy.py
+-rw-r--r--   0        0        0     1902 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_backends/typetracer.py
+-rw-r--r--   0        0        0       88 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/__init__.py
+-rw-r--r--   0        0        0    32504 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/avro.py
+-rw-r--r--   0        0        0    53533 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cling.py
+-rw-r--r--   0        0        0      985 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/hist.py
+-rw-r--r--   0        0        0     4485 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numexpr.py
+-rw-r--r--   0        0        0    10027 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numpy.py
+-rw-r--r--   0        0        0    37988 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/pyarrow.py
+-rw-r--r--   0        0        0     7038 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/__init__.py
+-rw-r--r--   0        0        0     2555 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
+-rw-r--r--   0        0        0     4326 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
+-rw-r--r--   0        0        0      987 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
+-rw-r--r--   0        0        0     2542 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3034 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0      630 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
+-rw-r--r--   0        0        0      830 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3196 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0     2668 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0      749 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
+-rw-r--r--   0        0        0     2749 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
+-rw-r--r--   0        0        0      552 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
+-rw-r--r--   0        0        0      637 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
+-rw-r--r--   0        0        0     2886 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
+-rw-r--r--   0        0        0     2904 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3416 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0     3531 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
+-rw-r--r--   0        0        0      556 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
+-rw-r--r--   0        0        0      695 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3036 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0      795 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
+-rw-r--r--   0        0        0     2523 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0     2729 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
+-rw-r--r--   0        0        0     1035 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
+-rw-r--r--   0        0        0      961 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
+-rw-r--r--   0        0        0     2593 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
+-rw-r--r--   0        0        0     1536 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
+-rw-r--r--   0        0        0     1710 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     2012 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1184 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
+-rw-r--r--   0        0        0      755 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu
+-rw-r--r--   0        0        0      806 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
+-rw-r--r--   0        0        0      744 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
+-rw-r--r--   0        0        0     1169 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0     1059 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
+-rw-r--r--   0        0        0     3208 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
+-rw-r--r--   0        0        0      575 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
+-rw-r--r--   0        0        0      830 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
+-rw-r--r--   0        0        0      650 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
+-rw-r--r--   0        0        0     2610 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
+-rw-r--r--   0        0        0     1126 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
+-rw-r--r--   0        0        0      951 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      721 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
+-rw-r--r--   0        0        0     1003 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
+-rw-r--r--   0        0        0     1339 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
+-rw-r--r--   0        0        0      835 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
+-rw-r--r--   0        0        0      975 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
+-rw-r--r--   0        0        0      802 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
+-rw-r--r--   0        0        0     1123 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu
+-rw-r--r--   0        0        0      623 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu
+-rw-r--r--   0        0        0      789 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
+-rw-r--r--   0        0        0     1040 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     1020 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1045 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      974 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
+-rw-r--r--   0        0        0      946 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
+-rw-r--r--   0        0        0      980 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
+-rw-r--r--   0        0        0      663 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
+-rw-r--r--   0        0        0      586 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
+-rw-r--r--   0        0        0     2580 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
+-rw-r--r--   0        0        0     1360 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
+-rw-r--r--   0        0        0      461 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
+-rw-r--r--   0        0        0      534 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
+-rw-r--r--   0        0        0      529 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
+-rw-r--r--   0        0        0      830 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
+-rw-r--r--   0        0        0      636 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
+-rw-r--r--   0        0        0      689 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0      457 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
+-rw-r--r--   0        0        0      830 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
+-rw-r--r--   0        0        0     2043 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
+-rw-r--r--   0        0        0     2198 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
+-rw-r--r--   0        0        0     2043 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
+-rw-r--r--   0        0        0     2198 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
+-rw-r--r--   0        0        0     3054 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
+-rw-r--r--   0        0        0     3289 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
+-rw-r--r--   0        0        0     2022 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
+-rw-r--r--   0        0        0     2022 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
+-rw-r--r--   0        0        0     3202 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
+-rw-r--r--   0        0        0     3012 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
+-rw-r--r--   0        0        0     3171 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
+-rw-r--r--   0        0        0     3439 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
+-rw-r--r--   0        0        0     3439 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
+-rw-r--r--   0        0        0      865 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
+-rw-r--r--   0        0        0      443 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
+-rw-r--r--   0        0        0     3195 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
+-rw-r--r--   0        0        0     1859 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/header-only/awkward/BuilderOptions.h
+-rw-r--r--   0        0        0    19822 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
+-rw-r--r--   0        0        0    89307 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
+-rw-r--r--   0        0        0      298 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/header-only/awkward/demo_impl.h
+-rw-r--r--   0        0        0     8025 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/header-only/awkward/utils.h
+-rw-r--r--   0        0        0      239 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/jax/__init__.py
+-rw-r--r--   0        0        0     6627 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/jax/reducers.py
+-rw-r--r--   0        0        0     5982 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/jax/trees.py
+-rw-r--r--   0        0        0       88 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numba/__init__.py
+-rw-r--r--   0        0        0    35824 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numba/arrayview.py
+-rw-r--r--   0        0        0     1182 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numba/arrayview_cuda.py
+-rw-r--r--   0        0        0    31514 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numba/builder.py
+-rw-r--r--   0        0        0    12431 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numba/growablebuffer.py
+-rw-r--r--   0        0        0    49132 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/numba/layout.py
+-rw-r--r--   0        0        0       88 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/rdataframe/__init__.py
+-rw-r--r--   0        0        0     9377 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/rdataframe/from_rdataframe.py
+-rw-r--r--   0        0        0     9922 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/rdataframe/to_rdataframe.py
+-rw-r--r--   0        0        0     1487 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
+-rw-r--r--   0        0        0     1111 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/__init__.py
+-rw-r--r--   0        0        0    12293 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/array_module.py
+-rw-r--r--   0        0        0     4939 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/cupy.py
+-rw-r--r--   0        0        0     1357 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/dispatch.py
+-rw-r--r--   0        0        0     2010 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/jax.py
+-rw-r--r--   0        0        0     2922 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/numpy.py
+-rw-r--r--   0        0        0    13706 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/numpylike.py
+-rw-r--r--   0        0        0     2288 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/shape.py
+-rw-r--r--   0        0        0    42477 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/typetracer.py
+-rw-r--r--   0        0        0     2527 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/_nplikes/ufuncs.py
+-rw-r--r--   0        0        0       88 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/behaviors/__init__.py
+-rw-r--r--   0        0        0     3479 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/behaviors/categorical.py
+-rw-r--r--   0        0        0     3898 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/behaviors/mixins.py
+-rw-r--r--   0        0        0     8509 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/behaviors/string.py
+-rw-r--r--   0        0        0      986 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/__init__.py
+-rw-r--r--   0        0        0    27803 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/bitmaskedarray.py
+-rw-r--r--   0        0        0    40840 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/bytemaskedarray.py
+-rw-r--r--   0        0        0    45437 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/content.py
+-rw-r--r--   0        0        0    13345 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/emptyarray.py
+-rw-r--r--   0        0        0    40347 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/indexedarray.py
+-rw-r--r--   0        0        0    63427 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/indexedoptionarray.py
+-rw-r--r--   0        0        0    59821 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/listarray.py
+-rw-r--r--   0        0        0    85132 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/listoffsetarray.py
+-rw-r--r--   0        0        0    49416 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/numpyarray.py
+-rw-r--r--   0        0        0    40491 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/recordarray.py
+-rw-r--r--   0        0        0    54541 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/regulararray.py
+-rw-r--r--   0        0        0    56952 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/unionarray.py
+-rw-r--r--   0        0        0    18843 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/contents/unmaskedarray.py
+-rw-r--r--   0        0        0      951 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/__init__.py
+-rw-r--r--   0        0        0     6081 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/bitmaskedform.py
+-rw-r--r--   0        0        0     5368 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/bytemaskedform.py
+-rw-r--r--   0        0        0     3369 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/emptyform.py
+-rw-r--r--   0        0        0    12450 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/form.py
+-rw-r--r--   0        0        0     5638 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/indexedform.py
+-rw-r--r--   0        0        0     5133 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/indexedoptionform.py
+-rw-r--r--   0        0        0     5621 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/listform.py
+-rw-r--r--   0        0        0     4715 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/listoffsetform.py
+-rw-r--r--   0        0        0     6004 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/numpyform.py
+-rw-r--r--   0        0        0     8208 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/recordform.py
+-rw-r--r--   0        0        0     5084 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/regularform.py
+-rw-r--r--   0        0        0     7760 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/unionform.py
+-rw-r--r--   0        0        0     4229 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/forms/unmaskedform.py
+-rw-r--r--   0        0        0     4779 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/__init__.py
+-rw-r--r--   0        0        0     3998 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_all.py
+-rw-r--r--   0        0        0     5141 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_almost_equal.py
+-rw-r--r--   0        0        0     4001 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_any.py
+-rw-r--r--   0        0        0     5109 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_argcartesian.py
+-rw-r--r--   0        0        0     3819 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_argcombinations.py
+-rw-r--r--   0        0        0     6888 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_argmax.py
+-rw-r--r--   0        0        0     6845 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_argmin.py
+-rw-r--r--   0        0        0     3158 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_argsort.py
+-rw-r--r--   0        0        0      952 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_backend.py
+-rw-r--r--   0        0        0     9515 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_broadcast_arrays.py
+-rw-r--r--   0        0        0     6595 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_broadcast_fields.py
+-rw-r--r--   0        0        0    16060 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_cartesian.py
+-rw-r--r--   0        0        0     1420 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_categories.py
+-rw-r--r--   0        0        0     8118 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_combinations.py
+-rw-r--r--   0        0        0    12213 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_concatenate.py
+-rw-r--r--   0        0        0     2715 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_copy.py
+-rw-r--r--   0        0        0     5817 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_corr.py
+-rw-r--r--   0        0        0     5228 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_count.py
+-rw-r--r--   0        0        0     4035 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_count_nonzero.py
+-rw-r--r--   0        0        0     5170 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_covar.py
+-rw-r--r--   0        0        0     4579 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_drop_none.py
+-rw-r--r--   0        0        0     1106 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_fields.py
+-rw-r--r--   0        0        0     5288 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_fill_none.py
+-rw-r--r--   0        0        0     3432 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_firsts.py
+-rw-r--r--   0        0        0     7802 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_flatten.py
+-rw-r--r--   0        0        0     3154 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_arrow.py
+-rw-r--r--   0        0        0      813 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_arrow_schema.py
+-rw-r--r--   0        0        0     2727 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_avro_file.py
+-rw-r--r--   0        0        0    14453 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_buffers.py
+-rw-r--r--   0        0        0     1839 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_categorical.py
+-rw-r--r--   0        0        0     1651 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_cupy.py
+-rw-r--r--   0        0        0     4111 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_iter.py
+-rw-r--r--   0        0        0     1716 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_jax.py
+-rw-r--r--   0        0        0    30067 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_json.py
+-rw-r--r--   0        0        0     2282 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_numpy.py
+-rw-r--r--   0        0        0    11860 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_parquet.py
+-rw-r--r--   0        0        0     3324 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_rdataframe.py
+-rw-r--r--   0        0        0     2965 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_from_regular.py
+-rw-r--r--   0        0        0     8859 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_full_like.py
+-rw-r--r--   0        0        0      873 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_is_categorical.py
+-rw-r--r--   0        0        0     2478 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_is_none.py
+-rw-r--r--   0        0        0      705 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_is_tuple.py
+-rw-r--r--   0        0        0      930 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_is_valid.py
+-rw-r--r--   0        0        0     2568 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_isclose.py
+-rw-r--r--   0        0        0     9131 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_linear_fit.py
+-rw-r--r--   0        0        0     3258 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_local_index.py
+-rw-r--r--   0        0        0     4757 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_mask.py
+-rw-r--r--   0        0        0     7430 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_max.py
+-rw-r--r--   0        0        0     9067 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_mean.py
+-rw-r--r--   0        0        0     3568 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_merge_option_of_records.py
+-rw-r--r--   0        0        0    12378 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_merge_union_of_records.py
+-rw-r--r--   0        0        0     3217 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_metadata_from_parquet.py
+-rw-r--r--   0        0        0     7382 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_min.py
+-rw-r--r--   0        0        0     4908 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_moment.py
+-rw-r--r--   0        0        0     2081 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_nan_to_none.py
+-rw-r--r--   0        0        0     5103 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_nan_to_num.py
+-rw-r--r--   0        0        0     3874 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_num.py
+-rw-r--r--   0        0        0     1951 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_ones_like.py
+-rw-r--r--   0        0        0     4362 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_pad_none.py
+-rw-r--r--   0        0        0     1786 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_parameters.py
+-rw-r--r--   0        0        0     6360 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_prod.py
+-rw-r--r--   0        0        0     4710 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_ptp.py
+-rw-r--r--   0        0        0     2275 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_ravel.py
+-rw-r--r--   0        0        0     9604 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_run_lengths.py
+-rw-r--r--   0        0        0     3028 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_singletons.py
+-rw-r--r--   0        0        0     3339 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_softmax.py
+-rw-r--r--   0        0        0     2670 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_sort.py
+-rw-r--r--   0        0        0     8124 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_std.py
+-rw-r--r--   0        0        0     3058 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_strings_astype.py
+-rw-r--r--   0        0        0    11718 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_sum.py
+-rw-r--r--   0        0        0     4931 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_arrow.py
+-rw-r--r--   0        0        0     6725 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_arrow_table.py
+-rw-r--r--   0        0        0     2370 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_backend.py
+-rw-r--r--   0        0        0     6378 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_buffers.py
+-rw-r--r--   0        0        0     6050 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_categorical.py
+-rw-r--r--   0        0        0     1107 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_cupy.py
+-rw-r--r--   0        0        0    13370 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_dataframe.py
+-rw-r--r--   0        0        0     1106 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_jax.py
+-rw-r--r--   0        0        0    11652 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_json.py
+-rw-r--r--   0        0        0     4507 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_layout.py
+-rw-r--r--   0        0        0     2612 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_list.py
+-rw-r--r--   0        0        0     2123 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_numpy.py
+-rw-r--r--   0        0        0     3354 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_packed.py
+-rw-r--r--   0        0        0    16968 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_parquet.py
+-rw-r--r--   0        0        0     2785 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_rdataframe.py
+-rw-r--r--   0        0        0     3347 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_to_regular.py
+-rw-r--r--   0        0        0    23979 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_transform.py
+-rw-r--r--   0        0        0     4304 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_type.py
+-rw-r--r--   0        0        0     9461 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_unflatten.py
+-rw-r--r--   0        0        0     2484 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_unzip.py
+-rw-r--r--   0        0        0     1138 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_validity_error.py
+-rw-r--r--   0        0        0     2659 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_values_astype.py
+-rw-r--r--   0        0        0     9352 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_var.py
+-rw-r--r--   0        0        0     5562 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_where.py
+-rw-r--r--   0        0        0     5641 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_with_field.py
+-rw-r--r--   0        0        0     2610 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_with_name.py
+-rw-r--r--   0        0        0     1848 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_with_parameter.py
+-rw-r--r--   0        0        0     3756 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_without_field.py
+-rw-r--r--   0        0        0     1509 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_without_parameters.py
+-rw-r--r--   0        0        0     2134 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_zeros_like.py
+-rw-r--r--   0        0        0     8819 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/operations/ak_zip.py
+-rw-r--r--   0        0        0      707 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/__init__.py
+-rw-r--r--   0        0        0   163323 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/_awkward_datashape_parser.py
+-rw-r--r--   0        0        0     1914 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/arraytype.py
+-rw-r--r--   0        0        0     2451 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/listtype.py
+-rw-r--r--   0        0        0     5652 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/numpytype.py
+-rw-r--r--   0        0        0     4180 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/optiontype.py
+-rw-r--r--   0        0        0     8067 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/recordtype.py
+-rw-r--r--   0        0        0     3133 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/regulartype.py
+-rw-r--r--   0        0        0     1105 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/scalartype.py
+-rw-r--r--   0        0        0     9622 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/type.py
+-rw-r--r--   0        0        0     3725 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/uniontype.py
+-rw-r--r--   0        0        0     1937 2023-04-13 15:38:23.000000 awkward-2.1.3/src/awkward/types/unknowntype.py
+-rw-r--r--   0        0        0       88 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     3358 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0002_minimal_listarray.py
+-rw-r--r--   0        0        0      487 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0006_deep_iteration.py
+-rw-r--r--   0        0        0     5565 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0008_slices_and_getitem.py
+-rw-r--r--   0        0        0    13378 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0011_listarray.py
+-rw-r--r--   0        0        0     4462 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0013_error_handling_struct.py
+-rw-r--r--   0        0        0    17019 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0014_finish_up_getitem.py
+-rw-r--r--   0        0        0     5169 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0018_fromiter_fillable.py
+-rw-r--r--   0        0        0     8833 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0019_use_json_library.py
+-rw-r--r--   0        0        0    13687 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0020_support_unsigned_indexes.py
+-rw-r--r--   0        0        0     6391 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0021_emptyarray.py
+-rw-r--r--   0        0        0    10743 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0023_regular_array.py
+-rw-r--r--   0        0        0     4890 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0024_use_regular_array.py
+-rw-r--r--   0        0        0    25581 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0025_record_array.py
+-rw-r--r--   0        0        0     3436 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0028_add_dressed_types.py
+-rw-r--r--   0        0        0     6361 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0032_replace_dressedtype.py
+-rw-r--r--   0        0        0    12027 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0046_start_indexedarray.py
+-rw-r--r--   0        0        0      898 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
+-rw-r--r--   0        0        0    12231 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0057_introducing_forms.py
+-rw-r--r--   0        0        0     5430 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0070_argmin_and_argmax.py
+-rw-r--r--   0        0        0     5384 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0072_fillna_operation.py
+-rw-r--r--   0        0        0    15655 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0074_argsort_and_sort.py
+-rw-r--r--   0        0        0     2836 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0077_zip_operation.py
+-rw-r--r--   0        0        0    11934 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0078_argcross_and_cross.py
+-rw-r--r--   0        0        0    12124 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0079_argchoose_and_choose.py
+-rw-r--r--   0        0        0     7071 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
+-rw-r--r--   0        0        0     6615 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0084_start_unionarray.py
+-rw-r--r--   0        0        0     6551 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0086_nep13_ufunc.py
+-rw-r--r--   0        0        0    12540 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0089_numpy_functions.py
+-rw-r--r--   0        0        0    46684 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0093_simplify_uniontypes_and_optiontypes.py
+-rw-r--r--   0        0        0     6959 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0107_assign_fields_to_records.py
+-rw-r--r--   0        0        0    46658 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0111_jagged_and_masked_getitem.py
+-rw-r--r--   0        0        0    77410 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0115_generic_reducer_operation.py
+-rw-r--r--   0        0        0    35162 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0118_numba_cpointers.py
+-rw-r--r--   0        0        0     1091 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0119_numexpr_and_broadcast_arrays.py
+-rw-r--r--   0        0        0     1106 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0124_strings_in_numba.py
+-rw-r--r--   0        0        0    32114 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0127_tomask_operation.py
+-rw-r--r--   0        0        0     3683 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0127b_tomask_operation_numba.py
+-rw-r--r--   0        0        0      838 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0138_emptyarray_type.py
+-rw-r--r--   0        0        0    17923 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0150_flatten.py
+-rw-r--r--   0        0        0     3602 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0163_negative_axis_wrap.py
+-rw-r--r--   0        0        0     9779 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0166_0167_0170_random_issues.py
+-rw-r--r--   0        0        0     4552 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0173_astype_operation.py
+-rw-r--r--   0        0        0    24034 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0184_concatenate_operation.py
+-rw-r--r--   0        0        0     2063 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0193_is_none_axis_parameter.py
+-rw-r--r--   0        0        0     3352 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0198_tutorial_documentation_1.py
+-rw-r--r--   0        0        0     8998 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0222_count_with_axis0.py
+-rw-r--r--   0        0        0    75605 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0224_arrow_to_awkward.py
+-rw-r--r--   0        0        0      581 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0264_reduce_last_empty.py
+-rw-r--r--   0        0        0     3251 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0273_path_for_with_field.py
+-rw-r--r--   0        0        0      743 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0286_broadcast_single_value_with_field.py
+-rw-r--r--   0        0        0     2205 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0290_bug_fixes_for_hats.py
+-rw-r--r--   0        0        0     4806 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0315_integerindex.py
+-rw-r--r--   0        0        0     5745 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0331_pandas_indexedarray.py
+-rw-r--r--   0        0        0     1257 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0334_fully_broadcastable_where.py
+-rw-r--r--   0        0        0      566 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0339_highlevel_sorting_function.py
+-rw-r--r--   0        0        0     6757 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0348_form_keys.py
+-rw-r--r--   0        0        0     4523 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0355_mixins.py
+-rw-r--r--   0        0        0    10396 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0395_complex_type_arrays.py
+-rw-r--r--   0        0        0     4934 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0395_fix_numba_indexedarray.py
+-rw-r--r--   0        0        0     3212 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0397_arrays_as_constants_in_numba.py
+-rw-r--r--   0        0        0    14529 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
+-rw-r--r--   0        0        0    22467 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0404_array_validity_check.py
+-rw-r--r--   0        0        0    14282 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0410_fix_argminmax_positions_for_missing_values.py
+-rw-r--r--   0        0        0    17455 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0437_stream_of_many_json_files.py
+-rw-r--r--   0        0        0    32921 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0447_preserve_regularness_in_reduce.py
+-rw-r--r--   0        0        0    24075 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0449_merge_many_arrays_in_one_pass.py
+-rw-r--r--   0        0        0     4059 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0493_zeros_ones_full_like.py
+-rw-r--r--   0        0        0     1606 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0496_provide_local_index.py
+-rw-r--r--   0        0        0     2059 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0499_getitem_indexedarray_bug.py
+-rw-r--r--   0        0        0     1286 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0504_block_ufuncs_for_strings.py
+-rw-r--r--   0        0        0     2926 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0511_copy_and_deepcopy.py
+-rw-r--r--   0        0        0     9119 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
+-rw-r--r--   0        0        0      365 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0546_fill_none_replacement_value_type.py
+-rw-r--r--   0        0        0     1102 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0549_numba_array_asarray.py
+-rw-r--r--   0        0        0     4268 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0557_min_max_initial_argument.py
+-rw-r--r--   0        0        0      537 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0559_fix_booleans_in_numba.py
+-rw-r--r--   0        0        0      636 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0572_numba_array_ndim.py
+-rw-r--r--   0        0        0     4901 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0582_propagate_context_in_broadcast_and_apply.py
+-rw-r--r--   0        0        0     1099 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0583_implement_unflatten_function.py
+-rw-r--r--   0        0        0     3084 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0590_allow_regulararray_size_zero.py
+-rw-r--r--   0        0        0     5957 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
+-rw-r--r--   0        0        0      478 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0627_behavior_from_dict_of_arrays.py
+-rw-r--r--   0        0        0     8205 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0652_tests_of_complex_numbers.py
+-rw-r--r--   0        0        0     2338 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0674_categorical_validation.py
+-rw-r--r--   0        0        0      750 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0713_getitem_field_should_simplify_optiontype.py
+-rw-r--r--   0        0        0     1242 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
+-rw-r--r--   0        0        0     1055 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0730_unflatten_axis_parameter.py
+-rw-r--r--   0        0        0     2569 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0733_run_lengths.py
+-rw-r--r--   0        0        0     2127 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0736_implement_argsort_for_strings.py
+-rw-r--r--   0        0        0      330 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0758_ak_zip_scallars.py
+-rw-r--r--   0        0        0     1122 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0766_prevent_combinations_of_characters.py
+-rw-r--r--   0        0        0    26349 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0773_typeparser.py
+-rw-r--r--   0        0        0      779 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
+-rw-r--r--   0        0        0      871 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0794_ak_cartesian_on_empty_array.py
+-rw-r--r--   0        0        0     1148 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0803_argsort_fix_type.py
+-rw-r--r--   0        0        0     1364 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0806_empty_lists_cartesian_fix.py
+-rw-r--r--   0        0        0     6311 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0813_full_like_dtype_arg.py
+-rw-r--r--   0        0        0     1661 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0815_broadcast_union_types_to_all_possibilities.py
+-rw-r--r--   0        0        0      488 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0819_issue.py
+-rw-r--r--   0        0        0      682 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0828_arrow_datatype_null.py
+-rw-r--r--   0        0        0    23609 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0835_datetime_type.py
+-rw-r--r--   0        0        0      676 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0835_datetime_type_pandas.py
+-rw-r--r--   0        0        0     4662 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0835_datetime_type_pyarrow.py
+-rw-r--r--   0        0        0      680 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0850_argsort_mask_array.py
+-rw-r--r--   0        0        0      449 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0863_is_none_numpy_array.py
+-rw-r--r--   0        0        0     1029 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0866_getitem_field_and_flatten_unions.py
+-rw-r--r--   0        0        0      929 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0875_arrow_null_type.py
+-rw-r--r--   0        0        0      901 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0879_non_primitive_with_field.py
+-rw-r--r--   0        0        0      563 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0884_index_and_identifier_refactoring.py
+-rw-r--r--   0        0        0     1086 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0889_ptp.py
+-rw-r--r--   0        0        0    53355 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0896_content_classes_refactoring.py
+-rw-r--r--   0        0        0     1751 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0898_unzip_heterogeneous_records.py
+-rw-r--r--   0        0        0      421 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
+-rw-r--r--   0        0        0      530 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0905_leading_zeros_in_unflatten.py
+-rw-r--r--   0        0        0     1048 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0906_arrow_fixed_size_list_type.py
+-rw-r--r--   0        0        0      666 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0910_unflatten_counts_relation.py
+-rw-r--r--   0        0        0     5261 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0912_packed.py
+-rw-r--r--   0        0        0   115760 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0914_types_and_forms.py
+-rw-r--r--   0        0        0     1877 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0916_datetime_values_astype.py
+-rw-r--r--   0        0        0     5522 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0927_numpy_array_nbytes.py
+-rw-r--r--   0        0        0      709 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0930_bug_in_unionarray_purelist_parameter.py
+-rw-r--r--   0        0        0     1627 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0945_argsort_sort_nan_array.py
+-rw-r--r--   0        0        0    28028 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0958_new_forms_must_accept_old_form_json.py
+-rw-r--r--   0        0        0    28284 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0959__getitem_array_implementation.py
+-rw-r--r--   0        0        0      651 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0975_mask_multidimensional_numpy_array.py
+-rw-r--r--   0        0        0      644 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0979_where_multidimentional_numpy_array.py
+-rw-r--r--   0        0        0     5803 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0982_missing_case_in_nonlocal_reducers.py
+-rw-r--r--   0        0        0     1976 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0984_ravel.py
+-rw-r--r--   0        0        0     1806 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_0992_correct_ptp_unmasking.py
+-rw-r--r--   0        0        0     2100 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
+-rw-r--r--   0        0        0      429 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1006_packed_regular_array_zero_size.py
+-rw-r--r--   0        0        0      416 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1007_from_buffers_empty_ndarray.py
+-rw-r--r--   0        0        0      551 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1017_numpyarray_broadcast.py
+-rw-r--r--   0        0        0      785 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1030_mixin_class_name.py
+-rw-r--r--   0        0        0    52114 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1031_start_getitem_next.py
+-rw-r--r--   0        0        0    18007 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1031b_start_getitem_next_specialized.py
+-rw-r--r--   0        0        0     1146 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1049_concatenate_single_array.py
+-rw-r--r--   0        0        0     1559 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1055_fill_none_numpy_dimension.py
+-rw-r--r--   0        0        0    42250 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1059_localindex.py
+-rw-r--r--   0        0        0      551 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1066_to_numpy_masked_structured_array.py
+-rw-r--r--   0        0        0      685 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1071_mask_identity_false_should_not_return_option_type.py
+-rw-r--r--   0        0        0    27714 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1072_sort.py
+-rw-r--r--   0        0        0    44140 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1074_combinations.py
+-rw-r--r--   0        0        0     5181 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1075_validityerror.py
+-rw-r--r--   0        0        0      273 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1106_argminmax_axis_None_missing_values.py
+-rw-r--r--   0        0        0    25531 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1110_type_tracer_1.py
+-rw-r--r--   0        0        0     1870 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1116_project_maskedarrays.py
+-rw-r--r--   0        0        0    28234 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1125_to_arrow_from_arrow.py
+-rw-r--r--   0        0        0     6276 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1132_utility_methods_for_highlevel_functions.py
+-rw-r--r--   0        0        0    21098 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1134_from_buffers_to_buffers.py
+-rw-r--r--   0        0        0    57322 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1135_rpad_operation.py
+-rw-r--r--   0        0        0     4639 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1136_regulararray_zeros_in_shape.py
+-rw-r--r--   0        0        0    10487 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1137_num.py
+-rw-r--r--   0        0        0    10222 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1142_numbers_to_type.py
+-rw-r--r--   0        0        0     2559 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1149_datetime_sort.py
+-rw-r--r--   0        0        0      630 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1154_arrow_tables_should_preserve_parameters.py
+-rw-r--r--   0        0        0    27983 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1162_ak_from_json_schema.py
+-rw-r--r--   0        0        0      766 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1183_bugs_found_by_dask_project_2.py
+-rw-r--r--   0        0        0     1286 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1189_fix_singletons_for_non_optional_data.py
+-rw-r--r--   0        0        0      551 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1192_iterables_in___array_function__.py
+-rw-r--r--   0        0        0      608 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1193_is_none_nested_option.py
+-rw-r--r--   0        0        0     2601 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1233_ak_with_name.py
+-rw-r--r--   0        0        0    26467 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1240_v2_implementation_of_numba_1.py
+-rw-r--r--   0        0        0     1146 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1259_simplify_optiontype.py
+-rw-r--r--   0        0        0     1560 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1260_simplify_masked_option_types.py
+-rw-r--r--   0        0        0      681 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1271_fix_4D_reducers.py
+-rw-r--r--   0        0        0    33003 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1294_to_and_from_parquet.py
+-rw-r--r--   0        0        0     1945 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
+-rw-r--r--   0        0        0    62340 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1300_awkward_to_cpp_converter_with_cling.py
+-rw-r--r--   0        0        0    39474 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1300b_same_for_numba.py
+-rw-r--r--   0        0        0      367 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1305_mixed_awkward_numpy_slicing.py
+-rw-r--r--   0        0        0     1702 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1308_zip_after_option.py
+-rw-r--r--   0        0        0     1703 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1318_array_function_types.py
+-rw-r--r--   0        0        0     1730 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1320_mask_identity_defaults.py
+-rw-r--r--   0        0        0      647 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1344_broadcast_arrays_depth_limit.py
+-rw-r--r--   0        0        0     6621 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1345_avro_reader.py
+-rw-r--r--   0        0        0     4562 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1351_is_tuple.py
+-rw-r--r--   0        0        0     8362 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1374_to_rdataframe.py
+-rw-r--r--   0        0        0     1755 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1377_ravel_string.py
+-rw-r--r--   0        0        0     1468 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1379_reducers_with_axis_None_and_typetracers.py
+-rw-r--r--   0        0        0     1384 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1399_from_jax.py
+-rw-r--r--   0        0        0     1227 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1399_to_jax.py
+-rw-r--r--   0        0        0      297 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1400_with_name_record.py
+-rw-r--r--   0        0        0      449 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1403_from_numpy_strings.py
+-rw-r--r--   0        0        0     3470 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1405_slicing_untested_cases.py
+-rw-r--r--   0        0        0     6909 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1415_behaviour_forwarding.py
+-rw-r--r--   0        0        0    18809 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1440_start_v2_to_parquet.py
+-rw-r--r--   0        0        0    14402 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1447_jax_autodiff_slices_ufuncs.py
+-rw-r--r--   0        0        0     8591 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1449_v2_to_json_from_json_functions.py
+-rw-r--r--   0        0        0      692 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1453_write_single_records_to_parquet.py
+-rw-r--r--   0        0        0     9828 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1473_from_rdataframe.py
+-rw-r--r--   0        0        0    24648 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1477_generator_entry_type_as_rvec.py
+-rw-r--r--   0        0        0     3579 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1490_jax_reducers_combinations.py
+-rw-r--r--   0        0        0     3905 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1502_getitem_jagged_issue1406.py
+-rw-r--r--   0        0        0     1733 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1504_typetracer_like.py
+-rw-r--r--   0        0        0     4913 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1508_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     2186 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1511_set_attribute.py
+-rw-r--r--   0        0        0      754 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1539_isnone_axis_check_issue1417.py
+-rw-r--r--   0        0        0     1570 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1559_fix_ufuncs_records_1439.py
+-rw-r--r--   0        0        0      990 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1565_axis_wrap_if_negative_record.py
+-rw-r--r--   0        0        0     1085 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1567_fix_longlong_in_Index.py
+-rw-r--r--   0        0        0     3022 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1568_fix_lengths_empty_regular_slices.py
+-rw-r--r--   0        0        0      385 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1578_to_arrow_empty_recordarray.py
+-rw-r--r--   0        0        0     5911 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1586_concatenate_should_preserve_regulararray.py
+-rw-r--r--   0        0        0      216 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1593_empty_slice_list_record.py
+-rw-r--r--   0        0        0     7260 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1604_preserve_form_in_concatenate.py
+-rw-r--r--   0        0        0     3636 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1607_no_reducers_on_records.py
+-rw-r--r--   0        0        0    10035 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1613_generator_tolayout_records.py
+-rw-r--r--   0        0        0      727 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1619_from_parquet_empty_field.py
+-rw-r--r--   0        0        0     6024 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1620_layout_builders.py
+-rw-r--r--   0        0        0     8122 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1625_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0      770 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1642_from_iter_of_tuples.py
+-rw-r--r--   0        0        0      389 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1644_concatenate_zeros_length.py
+-rw-r--r--   0        0        0     4317 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1650_Record_to_list_should_listify_itself.py
+-rw-r--r--   0        0        0      560 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1671_categorical_type.py
+-rw-r--r--   0        0        0    11761 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1672_broadcast_parameters.py
+-rw-r--r--   0        0        0     4453 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1677_array_builder_in_numba.py
+-rw-r--r--   0        0        0      544 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1685_IndexedArray_project_parameters.py
+-rw-r--r--   0        0        0      778 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1686_UnionArray_simplified_preserve_parameters.py
+-rw-r--r--   0        0        0      936 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1688_pack_categorical.py
+-rw-r--r--   0        0        0      525 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1703_fill_none_typetracer.py
+-rw-r--r--   0        0        0     1743 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1707_broadcast_parameters_ufunc.py
+-rw-r--r--   0        0        0      512 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1709_ak_array_constructor_behavior.py
+-rw-r--r--   0        0        0      398 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1735_from_numpy_mask.py
+-rw-r--r--   0        0        0      577 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1747_bytemaskedarray_mergemany.py
+-rw-r--r--   0        0        0      824 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1753_indexedarray_merge_kernel.py
+-rw-r--r--   0        0        0     1480 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1762_jax_behavior_support.py
+-rw-r--r--   0        0        0      589 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1764_jax_jacobian.py
+-rw-r--r--   0        0        0      962 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1765_add_ioanas_test_of_to_arraylib.py
+-rw-r--r--   0        0        0     4790 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1766_record_form_fields.py
+-rw-r--r--   0        0        0     2905 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1781_rdataframe_snapshot.py
+-rw-r--r--   0        0        0      701 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1784_reduce_leading_sublist.py
+-rw-r--r--   0        0        0      567 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1790_reduce_regulararray.py
+-rw-r--r--   0        0        0     4191 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1791_reduce_trailing_sublist.py
+-rw-r--r--   0        0        0     1027 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1794_run_lengths_empty_sublist.py
+-rw-r--r--   0        0        0      407 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1823_fill_none_axis_none.py
+-rw-r--r--   0        0        0      481 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1826_ravel_preserve_none.py
+-rw-r--r--   0        0        0     1451 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1829_to_from_rdataframe_bool.py
+-rw-r--r--   0        0        0      588 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
+-rw-r--r--   0        0        0     1097 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1847_numpy_array_contiguous.py
+-rw-r--r--   0        0        0      681 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
+-rw-r--r--   0        0        0     1640 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1867_pass_behavior_through_combinations.py
+-rw-r--r--   0        0        0    17239 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1904_drop_none.py
+-rw-r--r--   0        0        0     3553 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1914_improved_axis_to_posaxis.py
+-rw-r--r--   0        0        0     3444 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
+-rw-r--r--   0        0        0      921 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1930_unflatten_counts_checks.py
+-rw-r--r--   0        0        0      769 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1936_with_field_broadcasting.py
+-rw-r--r--   0        0        0      551 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1940_ak_backend.py
+-rw-r--r--   0        0        0     1457 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1943_regular_indexing.py
+-rw-r--r--   0        0        0      188 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1944_to_numpy_empty_record_array.py
+-rw-r--r--   0        0        0     1131 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1960_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     3286 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1961_ak_without_field.py
+-rw-r--r--   0        0        0      280 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1978_akRecord_constructor_should_retain_type.py
+-rw-r--r--   0        0        0      349 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
+-rw-r--r--   0        0        0      371 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2008_ak_type_layout.py
+-rw-r--r--   0        0        0    10222 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2020_reduce_axis_none.py
+-rw-r--r--   0        0        0      803 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2021_check_TypeTracerArray_in_ak_where.py
+-rw-r--r--   0        0        0      645 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2023_from_rdataframe.py
+-rw-r--r--   0        0        0     2854 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
+-rw-r--r--   0        0        0     1219 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2047_ak_transform_regular_to_jagged.py
+-rw-r--r--   0        0        0      406 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2051_arraybuilder_behavior_propagation.py
+-rw-r--r--   0        0        0     1275 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2055_array_builder_check.py
+-rw-r--r--   0        0        0     1659 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2058_merge_numpy_array.py
+-rw-r--r--   0        0        0      708 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2064_fill_none_record.py
+-rw-r--r--   0        0        0      799 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2067_to_buffers_byteorder.py
+-rw-r--r--   0        0        0      741 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2070_to_layout_string.py
+-rw-r--r--   0        0        0     1172 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2071_unflatten_non_packed_counts.py
+-rw-r--r--   0        0        0      291 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2076_ak_unzip_record.py
+-rw-r--r--   0        0        0      545 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2078_array_function_wrap.py
+-rw-r--r--   0        0        0      589 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2082_broadcast_zero_size.py
+-rw-r--r--   0        0        0     2765 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2096_ak_scalar_type.py
+-rw-r--r--   0        0        0      977 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2101_pickle_behavior_class.py
+-rw-r--r--   0        0        0      519 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2104_numpy_merge_option.py
+-rw-r--r--   0        0        0     2715 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2106_pickle_class.py
+-rw-r--r--   0        0        0      722 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2108_fill_none_indexed.py
+-rw-r--r--   0        0        0     2100 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2115_fix_up_typetracers.py
+-rw-r--r--   0        0        0      487 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2120_missing_field_error.py
+-rw-r--r--   0        0        0     1110 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2125_type_of_scalar.py
+-rw-r--r--   0        0        0     1893 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2150_typetracer_high_level_ufunc.py
+-rw-r--r--   0        0        0     1898 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2179_parameter_merging_rules.py
+-rw-r--r--   0        0        0      510 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2181_with_name_len.py
+-rw-r--r--   0        0        0     2957 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2185_merge_union_of_records.py
+-rw-r--r--   0        0        0      528 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
+-rw-r--r--   0        0        0     5548 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2198_almost_equal.py
+-rw-r--r--   0        0        0     1252 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2202_filter_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0     1453 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2214_offset_bool_index.py
+-rw-r--r--   0        0        0      334 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2219_flatten_empty.py
+-rw-r--r--   0        0        0      663 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2226_slice_regulararray_typetracer.py
+-rw-r--r--   0        0        0     1728 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2229_getitem_range_slice.py
+-rw-r--r--   0        0        0     4003 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2234_from_rdataframe_keep_order.py
+-rw-r--r--   0        0        0     3962 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2236_merge_union_of_records_option.py
+-rw-r--r--   0        0        0      485 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2240_merge_union_parameters.py
+-rw-r--r--   0        0        0     1338 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2240_simplify_merge_as_union.py
+-rw-r--r--   0        0        0      512 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2246_slice_not_packed.py
+-rw-r--r--   0        0        0      733 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2250_full_like_bool.py
+-rw-r--r--   0        0        0     1835 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2258_from_rdataframe_with_arguments.py
+-rw-r--r--   0        0        0      492 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2259_run_lengths_typetracer.py
+-rw-r--r--   0        0        0      560 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2263_to_packed_list.py
+-rw-r--r--   0        0        0      877 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2266_fix_nan_to_num.py
+-rw-r--r--   0        0        0      909 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2267_broadcast_fields.py
+-rw-r--r--   0        0        0     1336 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2293_unflatten_typetracer.py
+-rw-r--r--   0        0        0      406 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2294_view_unknown_scalar.py
+-rw-r--r--   0        0        0     2262 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2297_common_backend.py
+-rw-r--r--   0        0        0      455 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2304_index_typetracer.py
+-rw-r--r--   0        0        0     2929 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2306_cppyy_git.py
+-rw-r--r--   0        0        0     4386 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2319_from_buffers_array.py
+-rw-r--r--   0        0        0      721 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2327_array_interface.py
+-rw-r--r--   0        0        0     1728 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2329_cartesian_broadcasting_fixes.py
+-rw-r--r--   0        0        0      489 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2346_broadcast_depth_limit.py
+-rw-r--r--   0        0        0    15621 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2349_growablebuffer_in_numba.py
+-rw-r--r--   0        0        0      618 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2354_ufunc_same_backend.py
+-rw-r--r--   0        0        0      647 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2355_to_backend_record.py
+-rw-r--r--   0        0        0     1435 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2361_typetracer_asarray_nd.py
+-rw-r--r--   0        0        0     2921 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2368_type_is_equal.py
+-rw-r--r--   0        0        0     5259 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2373_unzip_touching.py
+-rw-r--r--   0        0        0     5857 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2374_cartesian_touching.py
+-rw-r--r--   0        0        0     1037 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2385_with_field_empty_record.py
+-rw-r--r--   0        0        0      926 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/test_2395_copy_asarray_touch.py
+-rw-r--r--   0        0        0      128 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/__init__.py
+-rw-r--r--   0        0        0      218 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/array_enum_test_data.avro
+-rw-r--r--   0        0        0      176 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/array_string_test_data.avro
+-rw-r--r--   0        0        0      152 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/array_test_data.avro
+-rw-r--r--   0        0        0      115 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/bool_test_data.avro
+-rw-r--r--   0        0        0      130 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/bytes_test_data.avro
+-rw-r--r--   0        0        0      158 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/double_test_data.avro
+-rw-r--r--   0        0        0      191 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/enum_null_test_data.avro
+-rw-r--r--   0        0        0      180 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/enum_test_data.avro
+-rw-r--r--   0        0        0      218 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/fixed_test_data.avro
+-rw-r--r--   0        0        0      116 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/float_test_data.avro
+-rw-r--r--   0        0        0      106 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/int_null_test_data.avro
+-rw-r--r--   0        0        0      128 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/int_string_null_test_data.avro
+-rw-r--r--   0        0        0       89 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/int_test_data.avro
+-rw-r--r--   0        0        0     3035 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2871 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/list-depths-records.parquet
+-rw-r--r--   0        0        0      497 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/list-depths-simple.parquet
+-rw-r--r--   0        0        0     1136 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/list-depths-strings.parquet
+-rw-r--r--   0        0        0     1060 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/list-depths.parquet
+-rw-r--r--   0        0        0      465 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/list-lengths.parquet
+-rw-r--r--   0        0        0      116 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/long_test_data.avro
+-rw-r--r--   0        0        0      681 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nonnullable-depths.parquet
+-rw-r--r--   0        0        0       75 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/null_test_data.avro
+-rw-r--r--   0        0        0      719 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-depths.parquet
+-rw-r--r--   0        0        0      635 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-levels.parquet
+-rw-r--r--   0        0        0     3050 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2926 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-list-depths-records.parquet
+-rw-r--r--   0        0        0     1179 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-list-depths-strings.parquet
+-rw-r--r--   0        0        0     1101 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-list-depths.parquet
+-rw-r--r--   0        0        0      430 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-record-primitives-simple.parquet
+-rw-r--r--   0        0        0     1181 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/nullable-record-primitives.parquet
+-rw-r--r--   0        0        0     1193 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/record-primitives.parquet
+-rw-r--r--   0        0        0      326 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/record_0_test_data.avro
+-rw-r--r--   0        0        0      368 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/record_1_test_data.avro
+-rw-r--r--   0        0        0      263 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/record_null_test_data.avro
+-rw-r--r--   0        0        0      423 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/record_test_data.avro
+-rw-r--r--   0        0        0      116 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/string_null_test_data.avro
+-rw-r--r--   0        0        0      125 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/string_test_data.avro
+-rw-r--r--   0        0        0      544 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/test-nan-inf.json
+-rw-r--r--   0        0        0      155 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/test-record-array.json
+-rw-r--r--   0        0        0      803 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/test-two-arrays.json
+-rw-r--r--   0        0        0      535 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/test.json
+-rw-r--r--   0        0        0      180 2023-04-13 15:38:23.000000 awkward-2.1.3/tests/samples/zero-record-batches.parquet
+-rw-r--r--   0        0        0       88 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/__init__.py
+-rw-r--r--   0        0        0     7072 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/test_1276_cuda_num.py
+-rw-r--r--   0        0        0     9911 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/test_1276_cuda_transfers.py
+-rw-r--r--   0        0        0     1197 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/test_1276_cupy_interop.py
+-rw-r--r--   0        0        0     1782 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/test_1276_from_cupy.py
+-rw-r--r--   0        0        0    42786 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/test_1300_same_for_numba_cuda.py
+-rw-r--r--   0        0        0      834 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/test_1381_check_errors.py
+-rw-r--r--   0        0        0    11252 2023-04-13 15:38:23.000000 awkward-2.1.3/tests-cuda/test_1809_array_cuda_jit.py
+-rw-r--r--   0        0        0     2212 2023-04-13 15:38:23.000000 awkward-2.1.3/.gitignore
+-rw-r--r--   0        0        0     1520 2023-04-13 15:38:23.000000 awkward-2.1.3/LICENSE
+-rw-r--r--   0        0        0     8479 2023-04-13 15:38:23.000000 awkward-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6933 2023-04-13 15:38:23.000000 awkward-2.1.3/PKG-INFO
```

### Comparing `awkward-2.1.2/CITATION.cff` & `awkward-2.1.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/CONTRIBUTING.md` & `awkward-2.1.3/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Contributing to Awkward Array
 
+[![Needs C++ Release](https://github.com/scikit-hep/awkward/actions/workflows/needs-cpp-release.yml/badge.svg)](https://github.com/scikit-hep/awkward/actions/workflows/needs-cpp-release.yml)
+
 Thank you for your interest in contributing! We're eager to see your ideas and look forward to working with you.
 
 This document describes the technical procedures we follow in this project. It should also be stressed that as members of the Scikit-HEP community, we are all obliged to maintaining a welcoming, harassment-free environment. See the [Code of Conduct](https://scikit-hep.org/code-of-conduct) for details.
 
 ### Where to start
 
 The front page for the Awkward Array project is its [GitHub README](https://github.com/scikit-hep/awkward#readme). This leads directly to tutorials and reference documentation that you may have already seen. It also includes instructions for [compiling for development](https://github.com/scikit-hep/awkward#installation-for-developers).
```

### Comparing `awkward-2.1.2/README.md` & `awkward-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/_toc.yml` & `awkward-2.1.3/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/conf.py` & `awkward-2.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/index.md` & `awkward-2.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/prepare_docstrings.py` & `awkward-2.1.3/docs/prepare_docstrings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/redirects-user-guide.json` & `awkward-2.1.3/docs/redirects-user-guide.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/redirects.json` & `awkward-2.1.3/docs/redirects.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/_static/css/awkward.css` & `awkward-2.1.3/docs/_static/css/awkward.css`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/getting-started/community-tutorials.md` & `awkward-2.1.3/docs/getting-started/community-tutorials.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/getting-started/index.md` & `awkward-2.1.3/docs/getting-started/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/getting-started/papers-and-talks.md` & `awkward-2.1.3/docs/getting-started/papers-and-talks.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/getting-started/demo/what-is-an-awkward-array.ipynb` & `awkward-2.1.3/docs/getting-started/demo/what-is-an-awkward-array.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/image/example-hierarchy.svg` & `awkward-2.1.3/docs/image/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/reference/ak.behavior.rst` & `awkward-2.1.3/docs/reference/ak.behavior.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/reference/ak.builder.ArrayBuilder.rst` & `awkward-2.1.3/docs/reference/ak.builder.ArrayBuilder.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/reference/awkwardforth.rst` & `awkward-2.1.3/docs/reference/awkwardforth.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/reference/toctree.txt` & `awkward-2.1.3/docs/reference/toctree.txt`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/10-minutes-to-awkward-array.md` & `awkward-2.1.3/docs/user-guide/10-minutes-to-awkward-array.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-combinatorics-best-match.md` & `awkward-2.1.3/docs/user-guide/how-to-combinatorics-best-match.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-combinatorics-cartesian-combinations.md` & `awkward-2.1.3/docs/user-guide/how-to-combinatorics-cartesian-combinations.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-convert-arrow.md` & `awkward-2.1.3/docs/user-guide/how-to-convert-arrow.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-convert-buffers.md` & `awkward-2.1.3/docs/user-guide/how-to-convert-buffers.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-convert-json.md` & `awkward-2.1.3/docs/user-guide/how-to-convert-json.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-convert-numpy.md` & `awkward-2.1.3/docs/user-guide/how-to-convert-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-convert-pandas.md` & `awkward-2.1.3/docs/user-guide/how-to-convert-pandas.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-convert-python.md` & `awkward-2.1.3/docs/user-guide/how-to-convert-python.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-convert-rdataframe.md` & `awkward-2.1.3/docs/user-guide/how-to-convert-rdataframe.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-create-arraybuilder.md` & `awkward-2.1.3/docs/user-guide/how-to-create-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-create-constructors.md` & `awkward-2.1.3/docs/user-guide/how-to-create-constructors.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-create-lists.md` & `awkward-2.1.3/docs/user-guide/how-to-create-lists.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-create-missing.md` & `awkward-2.1.3/docs/user-guide/how-to-create-missing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-create-records.md` & `awkward-2.1.3/docs/user-guide/how-to-create-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-create-strings.md` & `awkward-2.1.3/docs/user-guide/how-to-create-strings.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-create-unflatten-group.md` & `awkward-2.1.3/docs/user-guide/how-to-create-unflatten-group.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-examine-checking-validity.md` & `awkward-2.1.3/docs/user-guide/how-to-examine-checking-validity.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-examine-list-fields.md` & `awkward-2.1.3/docs/user-guide/how-to-examine-list-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-examine-simple-slicing.md` & `awkward-2.1.3/docs/user-guide/how-to-examine-simple-slicing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-examine-single-item.md` & `awkward-2.1.3/docs/user-guide/how-to-examine-single-item.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-examine-type.md` & `awkward-2.1.3/docs/user-guide/how-to-examine-type.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-filter-cut-mask.md` & `awkward-2.1.3/docs/user-guide/how-to-filter-cut-mask.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-filter-masked.md` & `awkward-2.1.3/docs/user-guide/how-to-filter-masked.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-filter-num.md` & `awkward-2.1.3/docs/user-guide/how-to-filter-num.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-filter-ragged.md` & `awkward-2.1.3/docs/user-guide/how-to-filter-ragged.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-math-argminmax.md` & `awkward-2.1.3/docs/user-guide/how-to-math-argminmax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-math-broadcasting.md` & `awkward-2.1.3/docs/user-guide/how-to-math-broadcasting.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-math-gpu.md` & `awkward-2.1.3/docs/user-guide/how-to-math-gpu.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-math-numpy.md` & `awkward-2.1.3/docs/user-guide/how-to-math-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-math-reducing.md` & `awkward-2.1.3/docs/user-guide/how-to-math-reducing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-math-statistics.md` & `awkward-2.1.3/docs/user-guide/how-to-math-statistics.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-restructure-add-fields.md` & `awkward-2.1.3/docs/user-guide/how-to-restructure-add-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-restructure-concatenate.md` & `awkward-2.1.3/docs/user-guide/how-to-restructure-concatenate.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-restructure-flatten.md` & `awkward-2.1.3/docs/user-guide/how-to-restructure-flatten.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-restructure-pad.md` & `awkward-2.1.3/docs/user-guide/how-to-restructure-pad.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-restructure-rename-records.md` & `awkward-2.1.3/docs/user-guide/how-to-restructure-rename-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-restructure-sort.md` & `awkward-2.1.3/docs/user-guide/how-to-restructure-sort.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-restructure-zip-project.md` & `awkward-2.1.3/docs/user-guide/how-to-restructure-zip-project.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-specialize-differentiate-jax.md` & `awkward-2.1.3/docs/user-guide/how-to-specialize-differentiate-jax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-specialize-in-numba.md` & `awkward-2.1.3/docs/user-guide/how-to-specialize-in-numba.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-specialize-lorentz.md` & `awkward-2.1.3/docs/user-guide/how-to-specialize-lorentz.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-specialize-override-numpy.md` & `awkward-2.1.3/docs/user-guide/how-to-specialize-override-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-specialize-subclass.md` & `awkward-2.1.3/docs/user-guide/how-to-specialize-subclass.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-use-header-only-layoutbuilder.md` & `awkward-2.1.3/docs/user-guide/how-to-use-header-only-layoutbuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-use-in-numba-arraybuilder.md` & `awkward-2.1.3/docs/user-guide/how-to-use-in-numba-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-use-in-numba-cuda.ipynb` & `awkward-2.1.3/docs/user-guide/how-to-use-in-numba-cuda.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs/user-guide/how-to-use-in-numba-features.md` & `awkward-2.1.3/docs/user-guide/how-to-use-in-numba-features.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/panel-data-analysts.png` & `awkward-2.1.3/docs-img/panel-data-analysts.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/panel-data-analysts.svg` & `awkward-2.1.3/docs-img/panel-data-analysts.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/panel-developers.png` & `awkward-2.1.3/docs-img/panel-developers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/panel-developers.svg` & `awkward-2.1.3/docs-img/panel-developers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/panel-doxygen.png` & `awkward-2.1.3/docs-img/panel-doxygen.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/panel-sphinx.png` & `awkward-2.1.3/docs-img/panel-sphinx.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/panel-tutorials-alternate.png` & `awkward-2.1.3/docs-img/panel-tutorials-alternate.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/panel-tutorials.png` & `awkward-2.1.3/docs-img/panel-tutorials.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/awkward-1-0-layers.pdf` & `awkward-2.1.3/docs-img/diagrams/awkward-1-0-layers.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/awkward-1-0-layers.png` & `awkward-2.1.3/docs-img/diagrams/awkward-1-0-layers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/awkward-1-0-layers.svg` & `awkward-2.1.3/docs-img/diagrams/awkward-1-0-layers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/awkward-timeline.pdf` & `awkward-2.1.3/docs-img/diagrams/awkward-timeline.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/awkward-timeline.png` & `awkward-2.1.3/docs-img/diagrams/awkward-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/awkward-timeline.svg` & `awkward-2.1.3/docs-img/diagrams/awkward-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip-github.png` & `awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg` & `awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip.png` & `awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip.svg` & `awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline-pip.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline.png` & `awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline.svg` & `awkward-2.1.3/docs-img/diagrams/awkward-uproot-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/cartoon-broadcasting.png` & `awkward-2.1.3/docs-img/diagrams/cartoon-broadcasting.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/cartoon-broadcasting.svg` & `awkward-2.1.3/docs-img/diagrams/cartoon-broadcasting.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/cartoon-cartesian.png` & `awkward-2.1.3/docs-img/diagrams/cartoon-cartesian.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/cartoon-cartesian.svg` & `awkward-2.1.3/docs-img/diagrams/cartoon-cartesian.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/cartoon-combinations.png` & `awkward-2.1.3/docs-img/diagrams/cartoon-combinations.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/cartoon-combinations.svg` & `awkward-2.1.3/docs-img/diagrams/cartoon-combinations.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/cartoon-schematic.png` & `awkward-2.1.3/docs-img/diagrams/cartoon-schematic.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/cartoon-schematic.svg` & `awkward-2.1.3/docs-img/diagrams/cartoon-schematic.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/example-array.svg` & `awkward-2.1.3/docs-img/diagrams/example-array.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/example-hierarchy.png` & `awkward-2.1.3/docs-img/diagrams/example-hierarchy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/example-hierarchy.svg` & `awkward-2.1.3/docs-img/diagrams/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/example-reduction-sum-only.svg` & `awkward-2.1.3/docs-img/diagrams/example-reduction-sum-only.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/example-reduction-sum.svg` & `awkward-2.1.3/docs-img/diagrams/example-reduction-sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/example-reduction.png` & `awkward-2.1.3/docs-img/diagrams/example-reduction.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/example-reduction.svg` & `awkward-2.1.3/docs-img/diagrams/example-reduction.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/git-strategy.pdf` & `awkward-2.1.3/docs-img/diagrams/git-strategy.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/git-strategy.png` & `awkward-2.1.3/docs-img/diagrams/git-strategy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/git-strategy.svg` & `awkward-2.1.3/docs-img/diagrams/git-strategy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/how-it-works-muons.png` & `awkward-2.1.3/docs-img/diagrams/how-it-works-muons.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/how-it-works-muons.svg` & `awkward-2.1.3/docs-img/diagrams/how-it-works-muons.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/how-it-works.svg` & `awkward-2.1.3/docs-img/diagrams/how-it-works.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/sorting-axis.svg` & `awkward-2.1.3/docs-img/diagrams/sorting-axis.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/reducers/all.svg` & `awkward-2.1.3/docs-img/diagrams/reducers/all.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/reducers/any.svg` & `awkward-2.1.3/docs-img/diagrams/reducers/any.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/reducers/argmax.svg` & `awkward-2.1.3/docs-img/diagrams/reducers/argmax.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/reducers/argmin.svg` & `awkward-2.1.3/docs-img/diagrams/reducers/argmin.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/reducers/count.svg` & `awkward-2.1.3/docs-img/diagrams/reducers/count.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/reducers/count_nonzero.svg` & `awkward-2.1.3/docs-img/diagrams/reducers/count_nonzero.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/reducers/max.svg` & `awkward-2.1.3/docs-img/diagrams/reducers/max.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/reducers/min.svg` & `awkward-2.1.3/docs-img/diagrams/reducers/min.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/reducers/product.svg` & `awkward-2.1.3/docs-img/diagrams/reducers/product.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/diagrams/reducers/sum.svg` & `awkward-2.1.3/docs-img/diagrams/reducers/sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/logo/favicon.ico` & `awkward-2.1.3/docs-img/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/logo/logo-300px-white.png` & `awkward-2.1.3/docs-img/logo/logo-300px-white.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/logo/logo-300px.png` & `awkward-2.1.3/docs-img/logo/logo-300px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/logo/logo-600px.png` & `awkward-2.1.3/docs-img/logo/logo-600px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/logo/logo.svg` & `awkward-2.1.3/docs-img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/photos/desire-path.jpg` & `awkward-2.1.3/docs-img/photos/desire-path.jpg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/plots/awkward-0-popularity.pdf` & `awkward-2.1.3/docs-img/plots/awkward-0-popularity.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/plots/awkward-0-popularity.png` & `awkward-2.1.3/docs-img/plots/awkward-0-popularity.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/plots/awkward-0-popularity.svg` & `awkward-2.1.3/docs-img/plots/awkward-0-popularity.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/plots/bikeroutes-scaling.svg` & `awkward-2.1.3/docs-img/plots/bikeroutes-scaling.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/docs-img/screenshots/github-issues-documentation.png` & `awkward-2.1.3/docs-img/screenshots/github-issues-documentation.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/__init__.py` & `awkward-2.1.3/src/awkward/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 # Versioning
 from awkward._version import __version__
 
 # NumPy-like alternatives
 import awkward._backends
+import awkward._nplikes
 
 # layout classes; functionality that used to be in C++ (in Awkward 1.x)
 import awkward.index
 import awkward.contents
 import awkward.record
 import awkward.types
 import awkward.forms
```

### Comparing `awkward-2.1.2/src/awkward/_behavior.py` & `awkward-2.1.3/src/awkward/_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_broadcasting.py` & `awkward-2.1.3/src/awkward/_broadcasting.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import copy
 import enum
 import functools
 import itertools
 from collections.abc import Sequence
 
 import awkward as ak
+from awkward._backends.backend import Backend
+from awkward._backends.dispatch import backend_of
 from awkward._behavior import find_custom_broadcast
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._parameters import (
     parameters_are_empty,
     parameters_are_equal,
@@ -83,15 +85,15 @@
         else:
             nextinputs.append(x)
             isscalar.append(True)
 
     return nextinputs
 
 
-def broadcast_unpack(x, isscalar: list[bool], backend: ak._backends.Backend):
+def broadcast_unpack(x, isscalar: list[bool], backend: Backend):
     if all(isscalar):
         if not backend.nplike.known_data or x.length == 0:
             return x._getitem_nothing()._getitem_nothing()
         else:
             return x[0][0]
     else:
         if not backend.nplike.known_data or x.length == 0:
@@ -118,15 +120,15 @@
                     type(x).__name__,
                     x.length,
                     in_function(options),
                 )
             )
 
 
-def all_same_offsets(backend: ak._backends.Backend, inputs: list) -> bool:
+def all_same_offsets(backend: Backend, inputs: list) -> bool:
     index_nplike = backend.index_nplike
 
     offsets = None
     for x in inputs:
         if isinstance(x, ListOffsetArray):
             if offsets is None:
                 offsets = x.offsets.raw(index_nplike)
@@ -361,15 +363,15 @@
 def left_broadcast_to(content: Content, depth: int) -> Content:
     for _ in range(content.purelist_depth, depth):
         content = RegularArray(content, 1, content.length)
     return content
 
 
 def apply_step(
-    backend: ak._backends.Backend,
+    backend: Backend,
     inputs: Sequence,
     action,
     depth: int,
     depth_context,
     lateral_context,
     behavior,
     options,
@@ -1054,15 +1056,15 @@
     left_broadcast=True,
     right_broadcast=True,
     numpy_to_regular=False,
     regular_to_jagged=False,
     function_name=None,
     broadcast_parameters_rule=BroadcastParameterRule.INTERSECT,
 ):
-    backend = ak._backends.backend_of(*inputs)
+    backend = backend_of(*inputs)
     isscalar = []
     out = apply_step(
         backend,
         broadcast_pack(inputs, isscalar),
         action,
         0,
         depth_context,
```

### Comparing `awkward-2.1.2/src/awkward/_do.py` & `awkward-2.1.3/src/awkward/_do.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import copy
 from collections.abc import Mapping, MutableMapping
 from numbers import Integral
 
 import awkward as ak
-from awkward._backends import Backend
+from awkward._backends.backend import Backend
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._typing import Any, AxisMaybeNone, Literal
 from awkward.contents.content import ActionType, Content
 from awkward.forms import form
 from awkward.record import Record
 
 np = NumpyMetadata.instance()
```

### Comparing `awkward-2.1.2/src/awkward/_errors.py` & `awkward-2.1.3/src/awkward/_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,24 +46,24 @@
             self._slate.__dict__.clear()
             self._slate.__dict__.update(self._kwargs)
             self._slate.__dict__["__primary_context__"] = self
 
     def __exit__(self, exception_type, exception_value, traceback):
         try:
             # Handle caught exception
-            if exception_type is not None:
+            if exception_type is not None and self.primary() is self:
                 self.handle_exception(exception_type, exception_value)
         finally:
             # Step out of the way so that another ErrorContext can become primary.
             if self.primary() is self:
                 self._slate.__dict__.clear()
 
     def handle_exception(self, cls: type[E], exception: E) -> E:
         if sys.version_info >= (3, 11, 0, "final"):
-            return self.decorate_exception(cls, exception)
+            self.decorate_exception(cls, exception)
         else:
             raise self.decorate_exception(cls, exception)
 
     def decorate_exception(self, cls: type[E], exception: E) -> E:
         if sys.version_info >= (3, 11, 0, "final"):
             if issubclass(cls, (NotImplementedError, AssertionError)):
                 exception.add_note(
@@ -165,15 +165,16 @@
         raise NotImplementedError
 
 
 class OperationErrorContext(ErrorContext):
     _width = 80 - 8
 
     def __init__(self, name, arguments):
-        from awkward._backends import NumpyBackend, backend_of
+        from awkward._backends.dispatch import backend_of
+        from awkward._backends.numpy import NumpyBackend
 
         numpy_backend = NumpyBackend.instance()
         if self.primary() is not None or all(
             backend_of(x, default=numpy_backend).nplike.is_eager for x in arguments
         ):
             # if primary is not None: we won't be setting an ErrorContext
             # if all nplikes are eager: no accumulation of large arrays
@@ -229,15 +230,16 @@
     {self.name}({"".join(arguments)}{extra_line})"""
 
 
 class SlicingErrorContext(ErrorContext):
     _width = 80 - 4
 
     def __init__(self, array, where):
-        from awkward._backends import NumpyBackend, backend_of
+        from awkward._backends.dispatch import backend_of
+        from awkward._backends.numpy import NumpyBackend
 
         numpy_backend = NumpyBackend.instance()
         if self.primary() is not None or all(
             backend_of(x, default=numpy_backend).nplike.is_eager for x in (array, where)
         ):
             # if primary is not None: we won't be setting an ErrorContext
             # if all nplikes are eager: no accumulation of large arrays
```

### Comparing `awkward-2.1.2/src/awkward/_kernels.py` & `awkward-2.1.3/src/awkward/_kernels.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 from __future__ import annotations
 
 import ctypes
 from abc import abstractmethod
 from typing import Any, Callable
 
 import awkward as ak
+from awkward._nplikes.cupy import Cupy
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._typing import Protocol, TypeAlias
 
 KernelKeyType: TypeAlias = tuple  # Tuple[str, Unpack[Tuple[metadata.dtype, ...]]]
 
 
+numpy = Numpy.instance()
 metadata = NumpyMetadata.instance()
 
 
 class KernelError(Protocol):
     filename: str | None  # pylint: disable=E0602
     str: str | None
     pass_through: bool
@@ -64,15 +66,16 @@
 
 
 class NumpyKernel(BaseKernel):
     @classmethod
     def _cast(cls, x, t):
         if issubclass(t, ctypes._Pointer):
             # Do we have a NumPy-owned array?
-            if Numpy.is_own_array(x):
+            if numpy.is_own_array(x):
+                assert numpy.is_c_contiguous(x), "kernel expects contiguous array"
                 if x.ndim > 0:
                     return ctypes.cast(x.ctypes.data, t)
                 else:
                     return x
             # Or, do we have a ctypes type
             elif hasattr(x, "_b_base_"):
                 return ctypes.cast(x, t)
@@ -91,55 +94,68 @@
         )
 
 
 class JaxKernel(NumpyKernel):
     def __call__(self, *args) -> None:
         assert len(args) == len(self._impl.argtypes)
 
-        if not any(Jax.is_tracer(arg) for arg in args):
+        if not any(Jax.is_tracer_type(type(arg)) for arg in args):
             return super().__call__(*args)
 
 
 class CupyKernel(BaseKernel):
-    def max_length(self, args):
-        import awkward._connect.cuda as ak_cuda
+    def __init__(self, impl: Callable[..., Any], key: KernelKeyType):
+        super().__init__(impl, key)
 
-        cupy = ak_cuda.import_cupy("Awkward Arrays with CUDA")
+        self._cupy = Cupy.instance()
+
+    def max_length(self, args):
         max_length = metadata.iinfo(metadata.int64).min
         # TODO should kernels strip nplike wrapper? Probably
         for array in args:
-            if isinstance(array, cupy.ndarray):
+            if self._cupy.is_own_array(array):
                 max_length = max(max_length, len(array))
         return max_length
 
     def calc_grid(self, length):
         if length > 1024:
             return -(length // -1024), 1, 1
         return 1, 1, 1
 
     def calc_blocks(self, length):
         if length > 1024:
             return 1024, 1, 1
         return length, 1, 1
 
+    def _cast(self, x, t):
+        if issubclass(t, ctypes._Pointer):
+            # Do we have a NumPy-owned array?
+            if self._cupy.is_own_array(x):
+                assert self._cupy.is_c_contiguous(x)
+            return x
+        else:
+            return x
+
     def __call__(self, *args) -> None:
         import awkward._connect.cuda as ak_cuda
 
         cupy = ak_cuda.import_cupy("Awkward Arrays with CUDA")
         maxlength = self.max_length(args)
         grid, blocks = self.calc_grid(maxlength), self.calc_blocks(maxlength)
         cupy_stream_ptr = cupy.cuda.get_current_stream().ptr
 
         if cupy_stream_ptr not in ak_cuda.cuda_streamptr_to_contexts:
             ak_cuda.cuda_streamptr_to_contexts[cupy_stream_ptr] = (
                 cupy.array(ak_cuda.NO_ERROR),
                 [],
             )
+        assert len(args) == len(self._impl.argtypes)
+
+        args = [self._cast(x, t) for x, t in zip(args, self._impl.argtypes)]
 
-        assert len(args) == len(self._impl.dir)
         # The first arg is the invocation index which raises itself by 8 in the kernel if there was no error before.
         # The second arg is the error_code.
         args = (
             *args,
             len(ak_cuda.cuda_streamptr_to_contexts[cupy_stream_ptr][1]),
             ak_cuda.cuda_streamptr_to_contexts[cupy_stream_ptr][0],
         )
```

### Comparing `awkward-2.1.2/src/awkward/_layout.py` & `awkward-2.1.3/src/awkward/_layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 from collections.abc import Mapping
 
-from awkward._backends import NumpyBackend
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
-from awkward._nplikes import nplike_of
+from awkward._nplikes.dispatch import nplike_of
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 numpy_backend = NumpyBackend.instance()
@@ -46,15 +46,16 @@
     )
     from awkward.index import Index8, Index64
 
     # overshadows global NumPy import for nplike-safety
     nplike = nplike_of(array)
 
     def recurse(array, mask=None):
-        if Jax.is_tracer(array):
+        cls = type(array)
+        if Jax.is_tracer_type(cls):
             raise TypeError("Jax tracers cannot be used with `ak.from_arraylib`")
 
         if regulararray and len(array.shape) > 1:
             new_shape = (-1,) + array.shape[2:]
             return RegularArray(
                 recurse(nplike.reshape(array, new_shape), mask),
                 array.shape[1],
```

### Comparing `awkward-2.1.2/src/awkward/_lookup.py` & `awkward-2.1.3/src/awkward/_lookup.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_parameters.py` & `awkward-2.1.3/src/awkward/_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_prettyprint.py` & `awkward-2.1.3/src/awkward/_prettyprint.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_reducers.py` & `awkward-2.1.3/src/awkward/_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_regularize.py` & `awkward-2.1.3/src/awkward/_regularize.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_slicing.py` & `awkward-2.1.3/src/awkward/_slicing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import operator
 
 import awkward as ak
-from awkward._backends import Backend
+from awkward._backends.backend import Backend
 from awkward._nplikes import to_nplike
+from awkward._nplikes.dispatch import nplike_of
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._regularize import is_array_like, is_integer_like, is_sized_iterable
 from awkward._typing import TYPE_CHECKING, Sequence, TypeAlias, TypeVar
 
 if TYPE_CHECKING:
@@ -271,15 +272,15 @@
             return out.data
         else:
             return out
 
     # Fallback for sized objects
     elif is_sized_iterable(item):
         # Do we have an array
-        nplike = ak._nplikes.nplike_of(item, default=None)
+        nplike = nplike_of(item, default=None)
         # We can end up with non-array objects associated with an nplike
         if nplike is not None and nplike.is_own_array(item):
             # Is it a scalar, not array?
             if len(item.shape) == 0:
                 raise AssertionError(
                     "scalar arrays should be handled by integer-like indexing"
                 )
@@ -507,23 +508,23 @@
             cumsum = item_backend.index_nplike.empty(
                 flat_mask.data.shape[0] + 1, dtype=np.int64
             )
             cumsum[0] = 0
             cumsum[1:] = item_backend.index_nplike.asarray(
                 item_backend.nplike.cumsum(flat_mask.data)
             )
-            nextoffsets = cumsum[item.offsets]
+            nextoffsets = ak.index.Index(cumsum[item.offsets])
 
         else:
             item._touch_data(recursive=False)
             nextoffsets = item.offsets
             nextcontent = item_backend.nplike.empty(unknown_length, dtype=np.int64)
 
         return ListOffsetArray(
-            ak.index.Index64(nextoffsets),
+            nextoffsets,
             NumpyArray(nextcontent, backend=item_backend),
         ).to_backend(backend)
 
     elif (
         isinstance(item, ListOffsetArray)
         and isinstance(item.content, IndexedOptionArray)
         and isinstance(item.content.content, NumpyArray)
@@ -555,34 +556,34 @@
             nextcontent = localindex.content.data[expanded]
 
             # list offsets do include missing values
             expanded[isnegative] = True
             cumsum = item_backend.nplike.empty(expanded.shape[0] + 1, dtype=np.int64)
             cumsum[0] = 0
             cumsum[1:] = item_backend.nplike.cumsum(expanded)
-            nextoffsets = cumsum[item.offsets]
+            nextoffsets = ak.index.Index(cumsum[item.offsets])
 
             # outindex fits into the lists; non-missing are sequential
-            outindex = item_backend.index_nplike.full(
-                nextoffsets[-1], -1, dtype=np.int64
+            outindex = ak.index.Index64(
+                item_backend.index_nplike.full(nextoffsets.data[-1], -1, dtype=np.int64)
             )
-            outindex[~isnegative[expanded]] = item_backend.index_nplike.arange(
+            outindex.data[~isnegative[expanded]] = item_backend.index_nplike.arange(
                 nextcontent.shape[0], dtype=np.int64
             )
 
         else:
             item._touch_data(recursive=False)
             nextoffsets = item.offsets
             outindex = item.content.index
             nextcontent = item_backend.nplike.empty(unknown_length, dtype=np.int64)
 
         return ListOffsetArray(
-            ak.index.Index64(nextoffsets, nplike=item_backend.index_nplike),
+            nextoffsets,
             IndexedOptionArray(
-                ak.index.Index(outindex, nplike=item_backend.index_nplike),
+                outindex,
                 NumpyArray(nextcontent, backend=item_backend),
             ),
         ).to_backend(backend)
 
     elif isinstance(item, ListOffsetArray):
         return ListOffsetArray(
             item.offsets, _normalise_item_bool_to_int(item.content, backend)
@@ -625,30 +626,30 @@
 
                 # outindex does include missing values
                 expanded[isnegative] = True
                 lenoutindex = item_backend.nplike.count_nonzero(expanded)
 
                 # non-missing are sequential
                 non_negative = item_backend.nplike.logical_not(isnegative[expanded])
-                outindex = item_backend.index_nplike.full(
-                    lenoutindex, -1, dtype=np.int64
+                outindex = ak.index.Index64(
+                    item_backend.index_nplike.full(lenoutindex, -1, dtype=np.int64)
                 )
-                outindex[
+                outindex.data[
                     to_nplike(non_negative, item_backend.index_nplike)
                 ] = item_backend.index_nplike.arange(
                     nextcontent.shape[0], dtype=np.int64
                 )
 
             else:
                 item._touch_data(recursive=False)
                 outindex = item.index
                 nextcontent = item_backend.nplike.empty(unknown_length, dtype=np.int64)
 
             return IndexedOptionArray(
-                ak.index.Index(outindex, nplike=item_backend.index_nplike),
+                outindex,
                 NumpyArray(nextcontent, backend=item_backend),
             ).to_backend(backend)
 
         else:
             return IndexedOptionArray(
                 item.index, _normalise_item_bool_to_int(item.content, backend)
             ).to_backend(backend)
```

### Comparing `awkward-2.1.2/src/awkward/_typetracer.py` & `awkward-2.1.3/src/awkward/_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_typing.py` & `awkward-2.1.3/src/awkward/_typing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_util.py` & `awkward-2.1.3/src/awkward/_util.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_v2.py` & `awkward-2.1.3/src/awkward/_v2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/cppyy.py` & `awkward-2.1.3/src/awkward/cppyy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/highlevel.py` & `awkward-2.1.3/src/awkward/highlevel.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from collections.abc import Iterable, Mapping, Sized
 
 from awkward_cpp.lib import _ext
 from numpy.lib.mixins import NDArrayOperatorsMixin  # noqa: TID251
 
 import awkward as ak
 import awkward._connect.hist
+from awkward._backends.dispatch import register_backend_lookup_factory
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of, get_array_class, get_record_class
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_non_string_like_iterable
 
 np = NumpyMetadata.instance()
@@ -2791,7 +2793,33 @@
         """
         return self.Record(self, name)
 
 
 def ignore_in_to_list(getitem_function):
     getitem_function.ignore_in_to_list = True
     return getitem_function
+
+
+@register_backend_lookup_factory
+def find_highlevel_backend(obj: type):
+    if issubclass(obj, (Array, Record)):
+
+        def finder(obj: Array):
+            return obj.layout.backend
+
+        return finder
+    elif issubclass(obj, ArrayBuilder):
+
+        def numpy_lookup(obj: ArrayBuilder):
+            return NumpyBackend.instance()
+
+        return numpy_lookup
+
+
+@register_backend_lookup_factory
+def find_lowlevel_backend(obj: type):
+    if issubclass(obj, _ext.ArrayBuilder):
+
+        def numpy_lookup(obj: ArrayBuilder):
+            return NumpyBackend.instance()
+
+        return numpy_lookup
```

### Comparing `awkward-2.1.2/src/awkward/index.py` & `awkward-2.1.3/src/awkward/index.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 
-from awkward._nplikes import nplike_of, to_nplike
+from awkward._nplikes import to_nplike
 from awkward._nplikes.cupy import Cupy
+from awkward._nplikes.dispatch import nplike_of
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyLike, NumpyMetadata
 from awkward._nplikes.typetracer import TypeTracer
 from awkward._typing import Self
 
 np = NumpyMetadata.instance()
@@ -39,16 +40,17 @@
         raise AssertionError(f"unrecognized Index form: {form!r}")
 
 
 class Index:
     _expected_dtype = None
 
     def __init__(self, data, *, metadata=None, nplike=None):
+        assert not isinstance(data, Index)
         if nplike is None:
-            nplike = nplike_of(data)
+            nplike = nplike_of(data, default=Numpy.instance())
         self._nplike = nplike
         if metadata is not None and not isinstance(metadata, dict):
             raise TypeError("Index metadata must be None or a dict")
         self._metadata = metadata
         # We don't care about F, C (it's one dimensional), but we do need
         # the array to be contiguous. This should _not_ return a copy if already
         self._data = self._nplike.ascontiguousarray(
```

### Comparing `awkward-2.1.2/src/awkward/jax.py` & `awkward-2.1.3/src/awkward/jax.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 def register_and_check():
     """
     Register Awkward Array node types with JAX's tree mechanism.
     """
     try:
-        import jax  # noqa: TID251
+        import jax  # noqa: TID251, F401
 
     except ModuleNotFoundError:
         raise ModuleNotFoundError(
             """install the 'jax' package with:
 
         python3 -m pip install jax jaxlib
```

### Comparing `awkward-2.1.2/src/awkward/numba.py` & `awkward-2.1.3/src/awkward/numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/record.py` & `awkward-2.1.3/src/awkward/record.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 from collections.abc import Iterable
 
 import awkward as ak
-from awkward._backends import Backend
+from awkward._backends.backend import Backend
+from awkward._backends.dispatch import (
+    register_backend_lookup_factory,
+    regularize_backend,
+)
 from awkward._behavior import get_record_class
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._regularize import is_integer
 from awkward._typing import Self
 from awkward._util import unset
@@ -224,15 +228,15 @@
         else:
             return dict(zip(self._array.fields, contents))
 
     def to_backend(self, backend: Backend | str | None = None) -> Self:
         if backend is None:
             backend = self._array.backend
         else:
-            backend = ak._backends.regularize_backend(backend)
+            backend = regularize_backend(backend)
         if backend is self._array.backend:
             return self
         else:
             return Record(self._array._to_backend(backend), self._at)
 
     def __copy__(self) -> Self:
         return self.copy()
@@ -240,7 +244,17 @@
     def __deepcopy__(self, memo):
         return Record(copy.deepcopy(self._array, memo), self._at)
 
     def copy(self, array=unset, at=unset) -> Self:
         return Record(
             self._array if array is unset else array, self._at if at is unset else at
         )
+
+
+@register_backend_lookup_factory
+def find_record_backend(obj: type):
+    if issubclass(obj, Record):
+
+        def finder(obj: Record):
+            return obj.backend
+
+        return finder
```

### Comparing `awkward-2.1.2/src/awkward/_connect/avro.py` & `awkward-2.1.3/src/awkward/_connect/avro.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cling.py` & `awkward-2.1.3/src/awkward/_connect/cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/hist.py` & `awkward-2.1.3/src/awkward/_connect/hist.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 Provide native support for Awkward Arrays in Hist via `Hist.fill_flattened`.
 """
 from __future__ import annotations
 
 import numpy as np
 
 import awkward as ak
-from awkward._backends import NumpyBackend
+from awkward._backends.numpy import NumpyBackend
 from awkward._typing import Any, Sequence
 
 numpy = NumpyBackend.instance()
 
 
 def unpack(array: ak.Array) -> dict[str, ak.Array] | None:
     if not ak.fields(array):
         return None
     else:
-        return {k: x for k, x in zip(ak.fields(array), ak.unzip(array))}
+        return dict(zip(ak.fields(array), ak.unzip(array)))
 
 
 def broadcast_and_flatten(args: Sequence[Any]) -> tuple[np.ndarray]:
     try:
         arrays = [ak.Array(x, backend=numpy) for x in args]
     except TypeError:
         return NotImplementedError
```

### Comparing `awkward-2.1.2/src/awkward/_connect/numexpr.py` & `awkward-2.1.3/src/awkward/_connect/numexpr.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/numpy.py` & `awkward-2.1.3/src/awkward/_connect/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import functools
 import inspect
 
 import numpy
 
 import awkward as ak
-from awkward._backends import backend_of
+from awkward._backends.dispatch import backend_of
 from awkward._behavior import (
     behavior_of,
     find_custom_cast,
     find_ufunc,
     find_ufunc_generic,
 )
 from awkward._layout import wrap_layout
@@ -41,15 +41,15 @@
         return numpy.array(out, *args, **kwargs)
 
 
 implemented = {}
 
 
 def _to_rectilinear(arg):
-    backend = ak._backends.backend_of(arg, default=None)
+    backend = backend_of(arg, default=None)
     # We have some array-like object that our backend mechanism understands
     if backend is not None:
         return ak.operations.to_numpy(arg)
     elif isinstance(arg, tuple):
         return tuple(_to_rectilinear(x) for x in arg)
     elif isinstance(arg, list):
         return [_to_rectilinear(x) for x in arg]
```

### Comparing `awkward-2.1.2/src/awkward/_connect/pyarrow.py` & `awkward-2.1.3/src/awkward/_connect/pyarrow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import json
 from collections.abc import Iterable, Sized
 
 import awkward as ak
+from awkward._backends.numpy import NumpyBackend
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._parameters import parameters_union
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
@@ -492,15 +493,15 @@
             parameters = {"__array__": "bytestring"}
         sub_parameters = {"__array__": "byte"}
 
         out = ak.contents.RegularArray(
             ak.contents.NumpyArray(
                 numpy.frombuffer(pacontent, dtype=np.uint8),
                 parameters=sub_parameters,
-                backend=ak._backends.NumpyBackend.instance(),
+                backend=NumpyBackend.instance(),
             ),
             storage_type.byte_width,
             parameters=parameters,
         )
         return popbuffers_finalize(
             out, paarray, validbits, awkwardarrow_type, generate_bitmasks
         )
@@ -528,15 +529,15 @@
             sub_parameters = {"__array__": "byte"}
 
         out = ak.contents.ListOffsetArray(
             akoffsets,
             ak.contents.NumpyArray(
                 numpy.frombuffer(pacontent, dtype=np.uint8),
                 parameters=sub_parameters,
-                backend=ak._backends.NumpyBackend.instance(),
+                backend=NumpyBackend.instance(),
             ),
             parameters=parameters,
         )
         return popbuffers_finalize(
             out, paarray, validbits, awkwardarrow_type, generate_bitmasks
         )
 
@@ -630,15 +631,15 @@
         bytedata = numpy.unpackbits(
             numpy.frombuffer(bitdata, dtype=np.uint8), bitorder="little"
         )
 
         out = ak.contents.NumpyArray(
             bytedata.view(np.bool_),
             parameters=node_parameters(awkwardarrow_type),
-            backend=ak._backends.NumpyBackend.instance(),
+            backend=NumpyBackend.instance(),
         )
         return popbuffers_finalize(
             out, paarray, validbits, awkwardarrow_type, generate_bitmasks
         )
 
     elif isinstance(storage_type, pyarrow.lib.DataType):
         assert storage_type.num_buffers == 2
@@ -650,15 +651,15 @@
             data = numpy.astype(numpy.frombuffer(data, dtype=np.int32), dtype=np.int64)
         if dt is None:
             dt = storage_type.to_pandas_dtype()
 
         out = ak.contents.NumpyArray(
             numpy.frombuffer(data, dtype=dt),
             parameters=node_parameters(awkwardarrow_type),
-            backend=ak._backends.NumpyBackend.instance(),
+            backend=NumpyBackend.instance(),
         )
         return popbuffers_finalize(
             out, paarray, validbits, awkwardarrow_type, generate_bitmasks
         )
 
     else:
         raise TypeError(f"unrecognized Arrow array type: {storage_type!r}")
```

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/__init__.py` & `awkward-2.1.3/src/awkward/_connect/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu` & `awkward-2.1.3/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/header-only/awkward/BuilderOptions.h` & `awkward-2.1.3/src/awkward/_connect/header-only/awkward/BuilderOptions.h`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/header-only/awkward/GrowableBuffer.h` & `awkward-2.1.3/src/awkward/_connect/header-only/awkward/GrowableBuffer.h`

 * *Files 2% similar despite different names*

```diff
@@ -445,15 +445,15 @@
     /// allocation of a new panel.
     ///
     /// This increases the #length by 1; if the new #length is larger than
     /// #reserved, a new panel will be allocated.
     void
     append(PRIMITIVE datum) {
       if (ptr_->current_length() == ptr_->reserved()) {
-        add_panel((size_t)ceil((double)ptr_->reserved() * (double)options_.resize()));
+        add_panel((size_t)ceil(options_.initial() * options_.resize()));
       }
       fill_panel(datum);
     }
 
     /// @brief Inserts an entire array into the panel(s), possibly triggering
     /// allocation of a new panel.
     ///
@@ -495,26 +495,24 @@
       }
     }
 
     /// @brief Moves all accumulated data from multiple panels to one
     /// contiguously allocated `external_pointer`. The panels are deleted,
     /// and a new #ptr is allocated.
     void
-    move_to(PRIMITIVE* to_ptr, size_t offset = 0) noexcept {
-      memcpy(to_ptr + offset,
-             reinterpret_cast<void*>(panel_.get()->data().get()),
-             panel_.get()->current_length() * sizeof(PRIMITIVE));
-
-      // move to next panel
-      panel_ = std::move(panel_.get()->next());
-      if (panel_) {
-        move_to(to_ptr, offset + panel_.get()->current_length());
-      } else {
-        clear();
+    move_to(PRIMITIVE* to_ptr) noexcept {
+      size_t next_offset = 0;
+      while(panel_) {
+        memcpy(to_ptr + next_offset,
+               reinterpret_cast<void*>(panel_.get()->data().get()),
+               panel_.get()->current_length() * sizeof(PRIMITIVE));
+        next_offset += panel_.get()->current_length();
+        panel_ = std::move(panel_.get()->next());
       }
+      clear();
     }
 
     /// @brief Copies and concatenates all accumulated data from multiple panels to one
     /// contiguously allocated `external_pointer`.
     void
     concatenate_from(PRIMITIVE* external_pointer, size_t to, size_t from) const noexcept {
       if (external_pointer) {
```

### Comparing `awkward-2.1.2/src/awkward/_connect/header-only/awkward/LayoutBuilder.h` & `awkward-2.1.3/src/awkward/_connect/header-only/awkward/LayoutBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/header-only/awkward/utils.h` & `awkward-2.1.3/src/awkward/_connect/header-only/awkward/utils.h`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/jax/reducers.py` & `awkward-2.1.3/src/awkward/_connect/jax/reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/jax/trees.py` & `awkward-2.1.3/src/awkward/_connect/jax/trees.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import jax
 
 import awkward as ak
 from awkward import contents, highlevel, record
+from awkward._backends.backend import Backend
+from awkward._backends.jax import JaxBackend
 from awkward._behavior import behavior_of
 from awkward._layout import wrap_layout
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._typing import Generic, TypeVar, Union
 from awkward.contents import Content
@@ -33,15 +35,15 @@
 
     return data_ptrs
 
 
 def replace_all_buffers(
     layout: contents.Content | record.Record,
     buffers: list,
-    backend: ak._backends.Backend,
+    backend: Backend,
 ):
     def action(node, **kwargs):
         jaxlike = Jax.instance()
         if isinstance(node, ak.contents.NumpyArray):
             buffer = buffers.pop(0)
             # JAX might give us non-buffers, so ignore them
             if not (numpy.is_own_array(buffer) or jaxlike.is_own_array(buffer)):
@@ -77,15 +79,15 @@
             layout = obj.layout
         elif isinstance(obj, (contents.Content, record.Record)):
             layout = obj
         else:
             raise TypeError
 
         # First, make sure we're all JAX
-        jax_backend = ak._backends.JaxBackend.instance()
+        jax_backend = JaxBackend.instance()
         layout = layout.to_backend(jax_backend)
 
         # Now pull out the Jax tracers / arrays
         buffers = find_all_buffers(layout)
 
         # # Drop the references to the existing buffers by replacing them with empty buffers
         # # FIXME: This works-around the fact that AuxData should probably contain only a form and length,
@@ -135,15 +137,15 @@
                     "JAX uses this dtype for the tangents of integer/boolean outputs; these cannot "
                     "reasonably be differentiated. Make sure that you are not computing the derivative "
                     "of a boolean/integer (array) valued function."
                 )
 
         # Replace the mixed NumPy-JAX layout leaves with the given buffers (and use the JAX nplike)
         layout = replace_all_buffers(
-            self._layout, list(buffers), backend=ak._backends.JaxBackend.instance()
+            self._layout, list(buffers), backend=JaxBackend.instance()
         )
         return wrap_layout(
             layout, behavior=self._behavior, highlevel=self._is_highlevel
         )
 
     def __eq__(self, other: AuxData) -> bool:
         return self.layout.is_equal_to(
```

### Comparing `awkward-2.1.2/src/awkward/_connect/numba/arrayview.py` & `awkward-2.1.3/src/awkward/_connect/numba/arrayview.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/numba/arrayview_cuda.py` & `awkward-2.1.3/src/awkward/_connect/numba/arrayview_cuda.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 
 from numba import types
 
 import awkward as ak
+from awkward._backends.cupy import CupyBackend
 
 ########## ArrayView Arguments Handler for CUDA JIT
 
 
 class ArrayViewArgHandler:
     def prepare_args(self, ty, val, stream, retr):
         if isinstance(val, ak.Array):
-            if isinstance(val.layout.backend, ak._backends.CupyBackend):
+            if isinstance(val.layout.backend, CupyBackend):
                 # Use uint64 for pos, start, stop, the array pointers values, and the pylookup value
                 tys = types.UniTuple(types.uint64, 5)
 
                 start = val._numbaview.start
                 stop = val._numbaview.stop
                 pos = val._numbaview.pos
                 arrayptrs = val._numbaview.lookup.arrayptrs.data.ptr
```

### Comparing `awkward-2.1.2/src/awkward/_connect/numba/builder.py` & `awkward-2.1.3/src/awkward/_connect/numba/builder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/numba/growablebuffer.py` & `awkward-2.1.3/src/awkward/_connect/numba/growablebuffer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/numba/layout.py` & `awkward-2.1.3/src/awkward/_connect/numba/layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/rdataframe/from_rdataframe.py` & `awkward-2.1.3/src/awkward/_connect/rdataframe/from_rdataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import cppyy
 import ROOT
 
 import awkward as ak
 import awkward._connect.cling
 import awkward._lookup
+from awkward._backends.numpy import NumpyBackend
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward.types.numpytype import primitive_to_dtype
 
 cpp_type_of = {
     "bool": "bool",
@@ -230,15 +231,15 @@
                     buffers,
                     byteorder=ak._util.native_byteorder,
                     highlevel=highlevel,
                     behavior=behavior,
                 )
                 index[col] = ak.index.Index64(
                     index[col].layout.to_backend_array(
-                        allow_missing=True, backend=ak._backends.NumpyBackend.instance()
+                        allow_missing=True, backend=NumpyBackend.instance()
                     )
                 )
             else:
                 contents[col] = ak.from_buffers(
                     form,
                     length,
                     buffers,
```

### Comparing `awkward-2.1.2/src/awkward/_connect/rdataframe/to_rdataframe.py` & `awkward-2.1.3/src/awkward/_connect/rdataframe/to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h` & `awkward-2.1.3/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/_nplikes/array_module.py` & `awkward-2.1.3/src/awkward/_nplikes/array_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,19 @@
             if getattr(obj, "dtype", dtype) != dtype:
                 raise ValueError(
                     "asarray was called with copy=False for an array of a different dtype"
                 )
             else:
                 return self._module.asarray(obj, dtype=dtype)
 
-    def ascontiguousarray(
-        self, x: ArrayLike, *, dtype: np.dtype | None = None
-    ) -> ArrayLike:
-        return self._module.ascontiguousarray(x, dtype=dtype)
+    def ascontiguousarray(self, x: ArrayLike) -> ArrayLike:
+        # Allow buffers to _pretend_ to be contiguous already
+        if x.dtype.metadata is not None and x.dtype.metadata.get("pretend_contiguous"):
+            return x
+        return self._module.ascontiguousarray(x)
 
     def frombuffer(
         self, buffer, *, dtype: np.dtype | None = None, count: int = -1
     ) -> ArrayLike:
         return self._module.frombuffer(buffer, dtype=dtype, count=count)
 
     def zeros(
@@ -376,7 +377,11 @@
     def astype(
         self, x: ArrayLike, dtype: numpy.dtype, *, copy: bool | None = True
     ) -> ArrayLike:
         return x.astype(dtype, copy=copy)
 
     def can_cast(self, from_: np.dtype | ArrayLike, to: np.dtype | ArrayLike) -> bool:
         return self._module.can_cast(from_, to, casting="same_kind")
+
+    @classmethod
+    def is_own_array(cls, obj) -> bool:
+        return cls.is_own_array_type(type(obj))
```

### Comparing `awkward-2.1.2/src/awkward/_nplikes/cupy.py` & `awkward-2.1.3/src/awkward/_nplikes/cupy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import numpy
 
 import awkward as ak
 from awkward._nplikes.array_module import ArrayModuleNumpyLike
+from awkward._nplikes.dispatch import register_nplike
 from awkward._nplikes.numpylike import ArrayLike
 from awkward._typing import Final
 
 
+@register_nplike
 class Cupy(ArrayModuleNumpyLike):
     is_eager: Final = False
 
     def __init__(self):
         import awkward._connect.cuda  # noqa: F401
 
         self._module = ak._connect.cuda.import_cupy("Awkward Arrays with CUDA")
@@ -136,20 +138,22 @@
 
     def array_str(
         self, array, max_line_width=None, precision=None, suppress_small=None
     ):
         return self._module.array_str(array, max_line_width, precision, suppress_small)
 
     @classmethod
-    def is_own_array(cls, obj) -> bool:
+    def is_own_array_type(cls, type_: type) -> bool:
         """
         Args:
-            obj: object to test
+            type_: object to test
 
         Return `True` if the given object is a cupy buffer, otherwise `False`.
 
         """
-        module, _, suffix = type(obj).__module__.partition(".")
+        module, _, suffix = type_.__module__.partition(".")
         return module == "cupy"
 
     def is_c_contiguous(self, x: ArrayLike) -> bool:
-        return x.flags["C_CONTIGUOUS"]
+        return x.flags["C_CONTIGUOUS"] or (
+            x.dtype.metadata is not None and x.dtype.metadata.get("pretend_contiguous")
+        )
```

### Comparing `awkward-2.1.2/src/awkward/_nplikes/jax.py` & `awkward-2.1.3/src/awkward/_nplikes/jax.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
-import numpy
-
 import awkward as ak
 from awkward._nplikes.array_module import ArrayModuleNumpyLike
+from awkward._nplikes.dispatch import register_nplike
 from awkward._nplikes.numpylike import ArrayLike
 from awkward._typing import Final
 
 
+@register_nplike
 class Jax(ArrayModuleNumpyLike):
     is_eager: Final = True
 
     def __init__(self):
         jax = ak.jax.import_jax()
         self._module = jax.numpy
 
@@ -31,51 +31,46 @@
         )
 
     @property
     def ndarray(self):
         return self._module.ndarray
 
     @classmethod
-    def is_own_array(cls, obj) -> bool:
+    def is_own_array_type(cls, type_: type) -> bool:
         """
         Args:
-            obj: object to test
+            type_: object to test
 
         Return `True` if the given object is a jax buffer, otherwise `False`.
 
         """
-        return cls.is_array(obj) or cls.is_tracer(obj)
+        return cls.is_array_type(type_) or cls.is_tracer_type(type_)
 
     @classmethod
-    def is_array(cls, obj) -> bool:
+    def is_array_type(cls, type_: type) -> bool:
         """
         Args:
-            obj: object to test
+            type_: object to test
 
         Return `True` if the given object is a jax buffer, otherwise `False`.
 
         """
-        module, _, suffix = type(obj).__module__.partition(".")
+        module, _, suffix = type_.__module__.partition(".")
         return module == "jaxlib"
 
     @classmethod
-    def is_tracer(cls, obj) -> bool:
+    def is_tracer_type(cls, type_: type) -> bool:
         """
         Args:
-            obj: object to test
+            type_: object to test
 
         Return `True` if the given object is a jax tracer, otherwise `False`.
 
         """
-        module, _, suffix = type(obj).__module__.partition(".")
+        module, _, suffix = type_.__module__.partition(".")
         return module == "jax"
 
     def is_c_contiguous(self, x: ArrayLike) -> bool:
         return True
 
-    def ascontiguousarray(
-        self, x: ArrayLike, *, dtype: numpy.dtype | None = None
-    ) -> ArrayLike:
-        if dtype is not None:
-            return x.astype(dtype)
-        else:
-            return x
+    def ascontiguousarray(self, x: ArrayLike) -> ArrayLike:
+        return x
```

### Comparing `awkward-2.1.2/src/awkward/_nplikes/numpy.py` & `awkward-2.1.3/src/awkward/_nplikes/numpy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import numpy
 
 import awkward as ak
 from awkward._nplikes.array_module import ArrayModuleNumpyLike
+from awkward._nplikes.dispatch import register_nplike
 from awkward._nplikes.numpylike import ArrayLike, NumpyMetadata
 from awkward._typing import Final, Literal
 
 np = NumpyMetadata.instance()
 
 
+@register_nplike
 class Numpy(ArrayModuleNumpyLike):
     is_eager: Final = True
 
     def __init__(self):
         self._module = numpy
 
     @property
@@ -26,26 +28,28 @@
         return self._module.char
 
     @property
     def ndarray(self):
         return self._module.ndarray
 
     @classmethod
-    def is_own_array(cls, obj) -> bool:
+    def is_own_array_type(cls, type_) -> bool:
         """
         Args:
-            obj: object to test
+            type_: object to test
 
         Return `True` if the given object is a numpy buffer, otherwise `False`.
 
         """
-        return isinstance(obj, numpy.ndarray)
+        return issubclass(type_, numpy.ndarray)
 
     def is_c_contiguous(self, x: ArrayLike) -> bool:
-        return x.flags["C_CONTIGUOUS"]
+        return x.flags["C_CONTIGUOUS"] or (
+            x.dtype.metadata is not None and x.dtype.metadata.get("pretend_contiguous")
+        )
 
     def packbits(
         self,
         x: ArrayLike,
         *,
         axis: int | None = None,
         bitorder: Literal["big", "little"] = "big",
```

### Comparing `awkward-2.1.2/src/awkward/_nplikes/numpylike.py` & `awkward-2.1.3/src/awkward/_nplikes/numpylike.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,17 +244,15 @@
         *,
         dtype: numpy.dtype | None = None,
         copy: bool | None = None,
     ) -> ArrayLike:
         ...
 
     @abstractmethod
-    def ascontiguousarray(
-        self, x: ArrayLike, *, dtype: numpy.dtype | None = None
-    ) -> ArrayLike:
+    def ascontiguousarray(self, x: ArrayLike) -> ArrayLike:
         ...
 
     @abstractmethod
     def frombuffer(
         self, buffer, *, dtype: numpy.dtype | None = None, count: int = -1
     ) -> ArrayLike:
         ...
@@ -614,7 +612,12 @@
     def is_c_contiguous(self, x: ArrayLike) -> bool:
         ...
 
     @classmethod
     @abstractmethod
     def is_own_array(cls, obj) -> bool:
         ...
+
+    @classmethod
+    @abstractmethod
+    def is_own_array_type(cls, type_) -> bool:
+        ...
```

### Comparing `awkward-2.1.2/src/awkward/_nplikes/shape.py` & `awkward-2.1.3/src/awkward/_nplikes/shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             return True
         else:
             raise TypeError("cannot compare unknown lengths against known values")
 
     def __gt__(self, other):
         raise TypeError("cannot order unknown lengths")
 
-    def __index__(self):  # pylint: disable=invalid-index-returned
+    def __index__(self):
         raise TypeError("cannot interpret unknown lengths as concrete index values")
 
     def __int__(self):
         raise TypeError("cannot interpret unknown lengths as concrete values")
 
     __bool__ = __int__
     __float__ = __int__
```

### Comparing `awkward-2.1.2/src/awkward/_nplikes/typetracer.py` & `awkward-2.1.3/src/awkward/_nplikes/typetracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from numbers import Number
 
 import numpy
 from numpy.lib.mixins import NDArrayOperatorsMixin
 
 import awkward as ak
+from awkward._nplikes.dispatch import register_nplike
 from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyLike, NumpyMetadata
 from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._regularize import is_integer, is_non_string_like_sequence
 from awkward._typing import (
     Any,
     Final,
     Literal,
@@ -553,14 +554,15 @@
 
 
 def try_touch_shape(array):
     if isinstance(array, TypeTracerArray):
         array.touch_shape()
 
 
+@register_nplike
 class TypeTracer(NumpyLike):
     known_data: Final = False
     is_eager: Final = True
 
     def _apply_ufunc(self, ufunc, *inputs):
         for x in inputs:
             try_touch_data(x)
@@ -601,30 +603,33 @@
     def asarray(
         self,
         obj,
         *,
         dtype: numpy.dtype | None = None,
         copy: bool | None = None,
     ) -> TypeTracerArray:
-        try_touch_data(obj)
-
         if isinstance(obj, ak.index.Index):
             obj = obj.data
 
         if isinstance(obj, TypeTracerArray):
             form_key = obj._form_key
             report = obj._report
 
             if dtype is None:
                 return obj
-            elif copy is False and dtype != obj.dtype:
+            elif dtype == obj.dtype:
+                return TypeTracerArray._new(
+                    dtype, obj.shape, form_key=form_key, report=report
+                )
+            elif copy is False:
                 raise ValueError(
                     "asarray was called with copy=False for an array of a different dtype"
                 )
             else:
+                try_touch_data(obj)
                 return TypeTracerArray._new(
                     dtype, obj.shape, form_key=form_key, report=report
                 )
         else:
             # Convert NumPy generics to scalars
             if isinstance(obj, np.generic):
                 obj = numpy.asarray(obj)
@@ -686,19 +691,18 @@
                 populate_shape_and_items(obj, 1)
                 if dtype is None:
                     dtype = numpy.result_type(*flat_items)
                 return TypeTracerArray._new(dtype, shape=tuple(shape))
             else:
                 raise TypeError
 
-    def ascontiguousarray(
-        self, x: ArrayLike, *, dtype: numpy.dtype | None = None
-    ) -> TypeTracerArray:
-        try_touch_data(x)
-        return TypeTracerArray._new(dtype or x.dtype, shape=x.shape)
+    def ascontiguousarray(self, x: ArrayLike) -> TypeTracerArray:
+        return TypeTracerArray._new(
+            x.dtype, shape=x.shape, form_key=x.form_key, report=x.report
+        )
 
     def frombuffer(
         self, buffer, *, dtype: np.dtype | None = None, count: int = -1
     ) -> TypeTracerArray:
         for x in (buffer, count):
             try_touch_data(x)
         raise NotImplementedError
@@ -1303,12 +1307,16 @@
         x.touch_data()
         return TypeTracerArray._new(np.dtype(dtype), x.shape)
 
     def can_cast(self, from_: np.dtype | ArrayLike, to: np.dtype | ArrayLike) -> bool:
         return numpy.can_cast(from_, to, casting="same_kind")
 
     @classmethod
+    def is_own_array_type(cls, type_: type) -> bool:
+        return issubclass(type_, TypeTracerArray)
+
+    @classmethod
     def is_own_array(cls, obj) -> bool:
-        return isinstance(obj, TypeTracerArray)
+        return cls.is_own_array_type(type(obj))
 
     def is_c_contiguous(self, x: ArrayLike) -> bool:
         return True
```

### Comparing `awkward-2.1.2/src/awkward/_nplikes/ufuncs.py` & `awkward-2.1.3/src/awkward/_nplikes/ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/behaviors/categorical.py` & `awkward-2.1.3/src/awkward/behaviors/categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/behaviors/mixins.py` & `awkward-2.1.3/src/awkward/behaviors/mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/behaviors/string.py` & `awkward-2.1.3/src/awkward/behaviors/string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/contents/__init__.py` & `awkward-2.1.3/src/awkward/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/contents/bitmaskedarray.py` & `awkward-2.1.3/src/awkward/contents/bitmaskedarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import copy
 import json
 import math
 
 import awkward as ak
+from awkward._backends.backend import Backend
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import MaybeNone, TypeTracer
 from awkward._parameters import (
     type_parameters_equal,
 )
@@ -787,15 +788,15 @@
 
         for i, isvalid in enumerate(mask):
             if not isvalid:
                 out[i] = None
 
         return out
 
-    def _to_backend(self, backend: ak._backends.Backend) -> Self:
+    def _to_backend(self, backend: Backend) -> Self:
         content = self._content.to_backend(backend)
         mask = self._mask.to_nplike(backend.index_nplike)
         return BitMaskedArray(
             mask,
             content,
             valid_when=self._valid_when,
             length=len(self),
```

### Comparing `awkward-2.1.2/src/awkward/contents/bytemaskedarray.py` & `awkward-2.1.3/src/awkward/contents/bytemaskedarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import copy
 import json
 import math
 
 import awkward as ak
+from awkward._backends.backend import Backend
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import MaybeNone, TypeTracer
 from awkward._parameters import (
     parameters_intersect,
@@ -1131,15 +1132,15 @@
 
         for i, isvalid in enumerate(mask):
             if not isvalid:
                 out[i] = None
 
         return out
 
-    def _to_backend(self, backend: ak._backends.Backend) -> Self:
+    def _to_backend(self, backend: Backend) -> Self:
         content = self._content.to_backend(backend)
         mask = self._mask.to_nplike(backend.index_nplike)
         return ByteMaskedArray(
             mask, content, valid_when=self._valid_when, parameters=self._parameters
         )
 
     def _is_equal_to(self, other, index_dtype, numpyarray):
```

### Comparing `awkward-2.1.2/src/awkward/contents/content.py` & `awkward-2.1.3/src/awkward/contents/content.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,25 @@
 
 import copy
 import math
 from collections.abc import Callable, Iterable, Mapping, MutableMapping, Sized
 from numbers import Complex, Real
 
 import awkward as ak
-from awkward._backends import Backend
+from awkward._backends.backend import Backend
+from awkward._backends.dispatch import (
+    backend_of,
+    register_backend_lookup_factory,
+    regularize_backend,
+)
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import get_array_class, get_record_class
 from awkward._layout import wrap_layout
 from awkward._nplikes import to_nplike
+from awkward._nplikes.dispatch import nplike_of
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._nplikes.typetracer import TypeTracer
 from awkward._parameters import (
     type_parameters_equal,
 )
@@ -373,15 +380,15 @@
         tail,
         advanced: Index | None,
         raw: Content,
         length: int,
     ):
         # if this is in a tuple-slice and really should be 0, it will be trimmed later
         length = 1 if length is not unknown_length and length == 0 else length
-        index = Index64(head.index, nplike=self._backend.index_nplike)
+        index = head.index
         indexlength = index.length
         index = index.to_nplike(self._backend.index_nplike)
         outindex = Index64.empty(
             index.length * length,
             self._backend.index_nplike,
         )
 
@@ -410,16 +417,15 @@
         )
 
     def _getitem_next_missing_jagged(
         self, head: Content, tail, advanced: Index | None, that: Content
     ):
         head = head.to_backend(self._backend)
         jagged = head.content.to_ListOffsetArray64()
-
-        index = Index64(head._index, nplike=self._backend.index_nplike)
+        index = head._index
         content = that._getitem_at(0)
         if self._backend.nplike.known_data and content.length < index.length:
             raise ak._errors.index_error(
                 self,
                 head,
                 "cannot fit masked jagged slice with length {} into {} of size {}".format(
                     index.length, type(that).__name__, content.length
@@ -554,15 +560,15 @@
             return self._getitem((where,))
 
         elif isinstance(where, tuple):
             if len(where) == 0:
                 return self
 
             # Backend may change if index contains typetracers
-            backend = ak._backends.backend_of(self, *where)
+            backend = backend_of(self, *where)
             this = self.to_backend(backend)
 
             # Normalise valid indices onto well-defined basis
             items = ak._slicing.normalise_items(where, backend)
             # Prepare items for advanced indexing (e.g. via broadcasting)
             nextwhere = ak._slicing.prepare_advanced_indexing(items, backend)
 
@@ -584,15 +590,15 @@
             return self._getitem(where.layout)
 
         # Convert between nplikes of different backends
         elif (
             isinstance(where, ak.contents.Content)
             and where.backend is not self._backend
         ):
-            backend = ak._backends.backend_of(self, where)
+            backend = backend_of(self, where)
             return self.to_backend(backend)._getitem(where.to_backend(backend))
 
         elif isinstance(where, ak.contents.NumpyArray):
             data_as_index = to_nplike(
                 where.data,
                 self._backend.index_nplike,
                 from_nplike=self._backend.nplike,
@@ -656,15 +662,15 @@
             return where.to_NumpyArray(np.int64)
 
         elif isinstance(where, Content):
             return self._getitem((where,))
 
         elif is_sized_iterable(where):
             # Do we have an array
-            nplike = ak._nplikes.nplike_of(where, default=None)
+            nplike = nplike_of(where, default=None)
             # We can end up with non-array objects associated with an nplike
             if nplike is not None and nplike.is_own_array(where):
                 # Is it a scalar, not array?
                 if len(where.shape) == 0:
                     raise AssertionError(
                         "scalar arrays should be handled by integer-like indexing"
                     )
@@ -935,15 +941,15 @@
         return self._nbytes_part()
 
     def purelist_parameter(self, key: str):
         """
         Return the value of the outermost parameter matching `key` in a sequence
         of nested lists, stopping at the first record or tuple layer.
 
-        If a layer has #ak.types.UnionType, the value is only returned if all
+         If a layer has #ak.types.UnionType, the value is only returned if all
         possibilities have the same value.
         """
         return self.form_cls.purelist_parameter(self, key)
 
     def _is_unique(
         self,
         negaxis: AxisMaybeNone,
@@ -1075,28 +1081,26 @@
 
     def to_numpy(self, allow_missing: bool = True):
         ak._errors.deprecate(
             "`Content.to_numpy` is deprecated. Please replace calls to "
             "`Content.to_numpy(...)` with `Content.to_backend_array(..., backend='cpu')`.",
             "2.2.0",
         )
-        return self.to_backend(ak._backends.NumpyBackend.instance())._to_backend_array(
-            allow_missing
-        )
+        return self.to_backend(NumpyBackend.instance())._to_backend_array(allow_missing)
 
     def to_backend_array(
         self, allow_missing: bool = True, *, backend: Backend | str | None = None
     ):
         if backend is None:
             backend = self._backend
         else:
-            backend = ak._backends.regularize_backend(backend)
+            backend = regularize_backend(backend)
         return self._to_backend_array(allow_missing, backend)
 
-    def _to_backend_array(self, allow_missing: bool, backend: ak._backends.Backend):
+    def _to_backend_array(self, allow_missing: bool, backend: Backend):
         raise NotImplementedError
 
     def drop_none(self):
         return self._drop_none()
 
     def _drop_none(self) -> Content:
         raise NotImplementedError
@@ -1264,15 +1268,15 @@
     def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
         raise NotImplementedError
 
     def to_backend(self, backend: Backend | str | None = None) -> Self:
         if backend is None:
             backend = self._backend
         else:
-            backend = ak._backends.regularize_backend(backend)
+            backend = regularize_backend(backend)
         if backend is self._backend:
             return self
         else:
             return self._to_backend(backend)
 
     def _to_backend(self, backend: Backend) -> Self:
         raise NotImplementedError
@@ -1315,7 +1319,17 @@
         raise NotImplementedError
 
     def _fill_none(self, value: Content) -> Content:
         raise NotImplementedError
 
     def copy(self, *, parameters: JSONMapping | None = unset) -> Self:
         raise NotImplementedError
+
+
+@register_backend_lookup_factory
+def find_content_backend(obj: type):
+    if issubclass(obj, Content):
+
+        def finder(obj: Content):
+            return obj.backend
+
+        return finder
```

### Comparing `awkward-2.1.2/src/awkward/contents/emptyarray.py` & `awkward-2.1.3/src/awkward/contents/emptyarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 
 import awkward as ak
+from awkward._backends.backend import Backend
+from awkward._backends.numpy import NumpyBackend
+from awkward._backends.typetracer import TypeTracerBackend
 from awkward._errors import deprecate
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
 from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
@@ -64,15 +67,15 @@
 
     def __init__(self, *, parameters=None, backend=None):
         if not (parameters is None or len(parameters) == 0):
             deprecate(
                 f"{type(self).__name__} cannot contain parameters", version="2.2.0"
             )
         if backend is None:
-            backend = ak._backends.NumpyBackend.instance()
+            backend = NumpyBackend.instance()
         self._init(parameters, backend)
 
     form_cls: Final = EmptyForm
 
     def copy(
         self,
         *,
@@ -105,15 +108,15 @@
 
     def _to_buffers(self, form, getkey, container, backend, byteorder):
         assert isinstance(form, self.form_cls)
 
     def _to_typetracer(self, forget_length: bool) -> Self:
         return EmptyArray(
             parameters=self._parameters,
-            backend=ak._backends.TypeTracerBackend.instance(),
+            backend=TypeTracerBackend.instance(),
         )
 
     def _touch_data(self, recursive):
         pass
 
     def _touch_shape(self, recursive):
         pass
@@ -402,12 +405,12 @@
         return self
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
             raise TypeError("cannot convert typetracer arrays to Python lists")
         return []
 
-    def _to_backend(self, backend: ak._backends.Backend) -> Self:
+    def _to_backend(self, backend: Backend) -> Self:
         return EmptyArray(parameters=self._parameters, backend=backend)
 
     def _is_equal_to(self, other, index_dtype, numpyarray):
         return True
```

### Comparing `awkward-2.1.2/src/awkward/contents/indexedarray.py` & `awkward-2.1.3/src/awkward/contents/indexedarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 
 import awkward as ak
+from awkward._backends.backend import Backend
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.typetracer import TypeTracer
 from awkward._parameters import (
     parameters_intersect,
     parameters_union,
@@ -1110,15 +1111,15 @@
         if out is not None:
             return out
 
         index = self._index.raw(numpy)
         nextcontent = self._content._carry(ak.index.Index(index), False)
         return nextcontent._to_list(behavior, json_conversions)
 
-    def _to_backend(self, backend: ak._backends.Backend) -> Self:
+    def _to_backend(self, backend: Backend) -> Self:
         content = self._content.to_backend(backend)
         index = self._index.to_nplike(backend.index_nplike)
         return IndexedArray(index, content, parameters=self._parameters)
 
     def _is_equal_to(self, other, index_dtype, numpyarray):
         return self.index.is_equal_to(
             other.index, index_dtype, numpyarray
```

### Comparing `awkward-2.1.2/src/awkward/contents/indexedoptionarray.py` & `awkward-2.1.3/src/awkward/contents/indexedoptionarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 
 import awkward as ak
+from awkward._backends.backend import Backend
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import MaybeNone, TypeTracer
 from awkward._parameters import (
     parameters_intersect,
@@ -1702,15 +1703,15 @@
 
         for i, isvalid in enumerate(not_missing):
             if not isvalid:
                 out.insert(i, None)
 
         return out
 
-    def _to_backend(self, backend: ak._backends.Backend) -> Self:
+    def _to_backend(self, backend: Backend) -> Self:
         content = self._content.to_backend(backend)
         index = self._index.to_nplike(backend.index_nplike)
         return IndexedOptionArray(index, content, parameters=self._parameters)
 
     def _is_equal_to(self, other, index_dtype, numpyarray):
         return self.index.is_equal_to(
             other.index, index_dtype, numpyarray
```

### Comparing `awkward-2.1.2/src/awkward/contents/listarray.py` & `awkward-2.1.3/src/awkward/contents/listarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 
 import awkward as ak
+from awkward._backends.backend import Backend
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import TypeTracer
 from awkward._parameters import (
     parameters_intersect,
     type_parameters_equal,
@@ -431,15 +432,15 @@
             )
 
             as_list_offset_array = self.to_ListOffsetArray64(False)
             next_content = as_list_offset_array._content[
                 as_list_offset_array.offsets[0] : as_list_offset_array.offsets[-1]
             ]
 
-            sliceoffsets = ak.index.Index64(slicecontent._offsets)
+            sliceoffsets = slicecontent._offsets
 
             outcontent = next_content._getitem_next_jagged(
                 sliceoffsets[:-1], sliceoffsets[1:], slicecontent._content, tail
             )
 
             return ak.contents.ListOffsetArray(
                 outoffsets, outcontent, parameters=self._parameters
@@ -523,15 +524,15 @@
                     self,
                     ak.contents.ListArray(
                         slicestarts, slicestops, slicecontent, parameters=None
                     ),
                     "jagged slice length differs from array length",
                 )
 
-            missing = ak.index.Index64(slicecontent._index)
+            missing = slicecontent._index
             _numvalid = ak.index.Index64.empty(1, self._backend.index_nplike)
             assert (
                 _numvalid.nplike is self._backend.index_nplike
                 and slicestarts.nplike is self._backend.index_nplike
                 and slicestops.nplike is self._backend.index_nplike
                 and missing.nplike is self._backend.index_nplike
             )
@@ -1082,16 +1083,16 @@
             if isinstance(
                 array,
                 (
                     ak.contents.ListArray,
                     ak.contents.ListOffsetArray,
                 ),
             ):
-                array_starts = ak.index.Index(array.starts)
-                array_stops = ak.index.Index(array.stops)
+                array_starts = array.starts
+                array_stops = array.stops
 
                 assert (
                     nextstarts.nplike is self._backend.index_nplike
                     and nextstops.nplike is self._backend.index_nplike
                     and array_starts.nplike is self._backend.index_nplike
                     and array_stops.nplike is self._backend.index_nplike
                 )
@@ -1116,16 +1117,16 @@
                 contentlength_so_far += array.content.length
 
                 length_so_far += array.length
 
             elif isinstance(array, ak.contents.RegularArray):
                 listoffsetarray = array.to_ListOffsetArray64(True)
 
-                array_starts = ak.index.Index64(listoffsetarray.starts)
-                array_stops = ak.index.Index64(listoffsetarray.stops)
+                array_starts = listoffsetarray.starts
+                array_stops = listoffsetarray.stops
 
                 assert (
                     nextstarts.nplike is self._backend.index_nplike
                     and nextstops.nplike is self._backend.index_nplike
                     and array_starts.nplike is self._backend.index_nplike
                     and array_stops.nplike is self._backend.index_nplike
                 )
@@ -1514,15 +1515,15 @@
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
             raise TypeError("cannot convert typetracer arrays to Python lists")
 
         return ListOffsetArray._to_list(self, behavior, json_conversions)
 
-    def _to_backend(self, backend: ak._backends.Backend) -> Self:
+    def _to_backend(self, backend: Backend) -> Self:
         content = self._content.to_backend(backend)
         starts = self._starts.to_nplike(backend.index_nplike)
         stops = self._stops.to_nplike(backend.index_nplike)
         return ListArray(starts, stops, content, parameters=self._parameters)
 
     def _is_equal_to(self, other, index_dtype, numpyarray):
         return (
```

### Comparing `awkward-2.1.2/src/awkward/contents/listoffsetarray.py` & `awkward-2.1.3/src/awkward/contents/listoffsetarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 
 import awkward as ak
+from awkward._backends.backend import Backend
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import TypeTracer, is_unknown_scalar
 from awkward._parameters import (
     type_parameters_equal,
@@ -2196,15 +2197,15 @@
             content = nextcontent._to_list(behavior, json_conversions)
             out = [None] * starts.length
 
             for i in range(starts.length):
                 out[i] = content[starts_data[i] : stops_data[i]]
             return out
 
-    def _to_backend(self, backend: ak._backends.Backend) -> Self:
+    def _to_backend(self, backend: Backend) -> Self:
         content = self._content.to_backend(backend)
         offsets = self._offsets.to_nplike(backend.index_nplike)
         return ListOffsetArray(offsets, content, parameters=self._parameters)
 
     def _awkward_strings_to_nonfinite(self, nonfinit_dict):
         if self.parameter("__array__") == "string":
             strings = self.to_list()
```

### Comparing `awkward-2.1.2/src/awkward/contents/numpyarray.py` & `awkward-2.1.3/src/awkward/contents/numpyarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 
 import awkward as ak
+from awkward._backends.backend import Backend
+from awkward._backends.dispatch import backend_of
+from awkward._backends.numpy import NumpyBackend
+from awkward._backends.typetracer import TypeTracerBackend
 from awkward._layout import maybe_posaxis
 from awkward._nplikes import to_nplike
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
 from awkward._nplikes.typetracer import TypeTracerArray
 from awkward._parameters import (
@@ -87,17 +91,15 @@
     """
 
     is_numpy = True
     is_leaf = True
 
     def __init__(self, data: ArrayLike, *, parameters=None, backend=None):
         if backend is None:
-            backend = ak._backends.backend_of(
-                data, default=ak._backends.NumpyBackend.instance()
-            )
+            backend = backend_of(data, default=NumpyBackend.instance())
 
         self._data = backend.nplike.asarray(data)
 
         if not isinstance(backend.nplike, Jax):
             ak.types.numpytype.dtype_to_primitive(self._data.dtype)
 
         if len(self._data.shape) == 0:
@@ -180,15 +182,15 @@
         assert isinstance(form, self.form_cls)
         key = getkey(self, form, "data")
         container[key] = ak._util.native_to_byteorder(
             self._raw(backend.nplike), byteorder
         )
 
     def _to_typetracer(self, forget_length: bool) -> Self:
-        backend = ak._backends.TypeTracerBackend.instance()
+        backend = TypeTracerBackend.instance()
         data = self._raw(backend.nplike)
         return NumpyArray(
             data.forget_length() if forget_length else data,
             parameters=self._parameters,
             backend=backend,
         )
 
@@ -697,27 +699,23 @@
             return self
 
         if len(self.shape) == 0:
             return self
 
         if negaxis is None:
             contiguous_self = self.to_contiguous()
-            # Python 3.8 could use math.prod
-            flattened_shape = 1
-            for s in contiguous_self.shape:
-                flattened_shape = flattened_shape * s
 
             offsets = ak.index.Index64.zeros(2, self._backend.index_nplike)
-            offsets[1] = flattened_shape
+            offsets[1] = self._data.size
             dtype = (
                 np.dtype(np.int64)
                 if self._data.dtype.kind.upper() == "M"
                 else self._data.dtype
             )
-            out = self._backend.nplike.empty(offsets[1], dtype=dtype)
+            out = self._backend.nplike.empty(self._data.size, dtype=dtype)
             assert offsets.nplike is self._backend.index_nplike
             self._handle_error(
                 self._backend[
                     "awkward_sort",
                     dtype.type,
                     dtype.type,
                     offsets.dtype.type,
@@ -1362,15 +1360,15 @@
                 neginf_string = json_conversions["neginf_string"]
                 if neginf_string is not None:
                     for i in self._backend.nplike.nonzero(self._data == -np.inf)[0]:
                         out[i] = neginf_string
 
             return out
 
-    def _to_backend(self, backend: ak._backends.Backend) -> Self:
+    def _to_backend(self, backend: Backend) -> Self:
         return NumpyArray(
             self._raw(backend.nplike),
             parameters=self._parameters,
             backend=backend,
         )
 
     def _is_equal_to(self, other, index_dtype, numpyarray):
```

### Comparing `awkward-2.1.2/src/awkward/contents/recordarray.py` & `awkward-2.1.3/src/awkward/contents/recordarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from __future__ import annotations
 
 import copy
 import json
 from collections.abc import Iterable
 
 import awkward as ak
+from awkward._backends.backend import Backend
+from awkward._backends.numpy import NumpyBackend
+from awkward._backends.typetracer import TypeTracerBackend
 from awkward._behavior import find_record_reducer
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._parameters import (
     parameters_intersect,
@@ -160,15 +163,15 @@
                         type(backend).__name__,
                         type(content.backend).__name__,
                     )
                 )
 
         # If no content backend was found, then choose our own
         if backend is None:
-            backend = ak._backends.NumpyBackend.instance()
+            backend = NumpyBackend.instance()
 
         if length is None:
             if len(contents) == 0:
                 raise TypeError(
                     "{} if len(contents) == 0, a 'length' must be specified".format(
                         type(self).__name__
                     )
@@ -321,15 +324,15 @@
         else:
             for field, content in zip(self._fields, self._contents):
                 content._to_buffers(
                     form.content(field), getkey, container, backend, byteorder
                 )
 
     def _to_typetracer(self, forget_length: bool) -> Self:
-        backend = ak._backends.TypeTracerBackend.instance()
+        backend = TypeTracerBackend.instance()
         contents = [x._to_typetracer(forget_length) for x in self._contents]
         return RecordArray(
             contents,
             self._fields,
             unknown_length if forget_length else self._length,
             parameters=self._parameters,
             backend=backend,
@@ -1108,15 +1111,15 @@
                 fields = [str(i) for i in range(len(self._contents))]
             contents = [x._to_list(behavior, json_conversions) for x in self._contents]
             out = [None] * self._length
             for i in range(self._length):
                 out[i] = dict(zip(fields, [x[i] for x in contents]))
             return out
 
-    def _to_backend(self, backend: ak._backends.Backend) -> Self:
+    def _to_backend(self, backend: Backend) -> Self:
         contents = [content.to_backend(backend) for content in self._contents]
         return RecordArray(
             contents,
             self._fields,
             length=self._length,
             parameters=self._parameters,
             backend=backend,
```

### Comparing `awkward-2.1.2/src/awkward/contents/regulararray.py` & `awkward-2.1.3/src/awkward/contents/regulararray.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 
 import awkward as ak
+from awkward._backends.backend import Backend
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._parameters import (
     parameters_intersect,
     parameters_union,
@@ -1419,15 +1420,15 @@
             content = self._content._to_list(behavior, json_conversions)
             length, size = self._length, self._size
             out = [None] * length
             for i in range(length):
                 out[i] = content[(i) * size : (i + 1) * size]
             return out
 
-    def _to_backend(self, backend: ak._backends.Backend) -> Self:
+    def _to_backend(self, backend: Backend) -> Self:
         content = self._content.to_backend(backend)
         return RegularArray(
             content, self._size, zeros_length=self._length, parameters=self._parameters
         )
 
     def _is_equal_to(self, other, index_dtype, numpyarray):
         return self._size == other.size and self._content.is_equal_to(
```

### Comparing `awkward-2.1.2/src/awkward/contents/unionarray.py` & `awkward-2.1.3/src/awkward/contents/unionarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 
 import copy
 import ctypes
 from collections.abc import Iterable, Sequence
 
 import awkward as ak
+from awkward._backends.backend import Backend
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import OneOf, TypeTracer
 from awkward._parameters import parameters_intersect, parameters_union
@@ -645,15 +646,15 @@
         )
         return self._contents[index]._carry(nextcarry, False)
 
     @staticmethod
     def regular_index(
         tags: Index,
         *,
-        backend: ak._backends.Backend,
+        backend: Backend,
         index_cls: type[Index] = Index64,
     ):
         tags = tags.to_nplike(backend.index_nplike)
 
         lentags = tags.length
         _size = ak.index.Index64.empty(1, nplike=backend.index_nplike)
         assert (
@@ -700,15 +701,15 @@
         )
 
     @staticmethod
     def nested_tags_index(
         offsets: Index,
         counts: Sequence[Index],
         *,
-        backend: ak._backends.Backend,
+        backend: Backend,
         tags_cls: type[Index] = Index8,
         index_cls: type[Index] = Index64,
     ) -> tuple[Index, Index]:
         index_nplike = backend.index_nplike
 
         offsets = offsets.to_nplike(index_nplike)
         counts = [c.to_nplike(index_nplike) for c in counts]
@@ -1045,16 +1046,16 @@
         parameters = self._parameters
         for array in head:
             if isinstance(array, ak.contents.EmptyArray):
                 continue
 
             parameters = parameters_intersect(parameters, array._parameters)
             if isinstance(array, ak.contents.UnionArray):
-                union_tags = ak.index.Index(array.tags)
-                union_index = ak.index.Index(array.index)
+                union_tags = array.tags
+                union_index = array.index
                 union_contents = array.contents
                 assert (
                     nexttags.nplike is self._backend.index_nplike
                     and union_tags.nplike is self._backend.index_nplike
                 )
                 self._handle_error(
                     self._backend[
@@ -1564,15 +1565,15 @@
         contents = [x._to_list(behavior, json_conversions) for x in self._contents]
 
         out = [None] * tags.shape[0]
         for i, tag in enumerate(tags):
             out[i] = contents[tag][index[i]]
         return out
 
-    def _to_backend(self, backend: ak._backends.Backend) -> Self:
+    def _to_backend(self, backend: Backend) -> Self:
         tags = self._tags.to_nplike(backend.index_nplike)
         index = self._index.to_nplike(backend.index_nplike)
         contents = [content.to_backend(backend) for content in self._contents]
         return UnionArray(
             tags,
             index,
             contents,
```

### Comparing `awkward-2.1.2/src/awkward/contents/unmaskedarray.py` & `awkward-2.1.3/src/awkward/contents/unmaskedarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 import math
 
 import awkward as ak
+from awkward._backends.backend import Backend
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.typetracer import MaybeNone
 from awkward._parameters import (
     parameters_intersect,
     parameters_union,
@@ -539,13 +540,13 @@
 
         out = self._to_list_custom(behavior, json_conversions)
         if out is not None:
             return out
 
         return self._content._to_list(behavior, json_conversions)
 
-    def _to_backend(self, backend: ak._backends.Backend) -> Self:
+    def _to_backend(self, backend: Backend) -> Self:
         content = self._content.to_backend(backend)
         return UnmaskedArray(content, parameters=self._parameters)
 
     def _is_equal_to(self, other, index_dtype, numpyarray):
         return self.content.is_equal_to(other.content, index_dtype, numpyarray)
```

### Comparing `awkward-2.1.2/src/awkward/forms/__init__.py` & `awkward-2.1.3/src/awkward/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/forms/bitmaskedform.py` & `awkward-2.1.3/src/awkward/forms/bitmaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/forms/bytemaskedform.py` & `awkward-2.1.3/src/awkward/forms/bytemaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/forms/emptyform.py` & `awkward-2.1.3/src/awkward/forms/emptyform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/forms/form.py` & `awkward-2.1.3/src/awkward/forms/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 
 import itertools
 import json
 import re
 from collections.abc import Mapping
 
 import awkward as ak
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import find_typestrs
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._typing import Final, JSONMapping, JSONSerializable
 
 np = NumpyMetadata.instance()
-numpy_backend = ak._backends.NumpyBackend.instance()
+numpy_backend = NumpyBackend.instance()
 
 
 reserved_nominal_parameters: Final = frozenset(
     {
         ("__array__", "string"),
         ("__array__", "bytestring"),
         ("__array__", "char"),
```

### Comparing `awkward-2.1.2/src/awkward/forms/indexedform.py` & `awkward-2.1.3/src/awkward/forms/indexedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/forms/indexedoptionform.py` & `awkward-2.1.3/src/awkward/forms/indexedoptionform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/forms/listform.py` & `awkward-2.1.3/src/awkward/forms/listform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/forms/listoffsetform.py` & `awkward-2.1.3/src/awkward/forms/listoffsetform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/forms/numpyform.py` & `awkward-2.1.3/src/awkward/forms/numpyform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/forms/recordform.py` & `awkward-2.1.3/src/awkward/forms/recordform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/forms/regularform.py` & `awkward-2.1.3/src/awkward/forms/regularform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/forms/unionform.py` & `awkward-2.1.3/src/awkward/forms/unionform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/forms/unmaskedform.py` & `awkward-2.1.3/src/awkward/forms/unmaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/__init__.py` & `awkward-2.1.3/src/awkward/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_all.py` & `awkward-2.1.3/src/awkward/operations/ak_all.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_almost_equal.py` & `awkward-2.1.3/src/awkward/operations/ak_almost_equal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 __all__ = ("almost_equal",)
 
 
-from awkward._backends import backend_of
+from awkward._backends.dispatch import backend_of
 from awkward._behavior import behavior_of, get_array_class, get_record_class
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._parameters import parameters_are_equal
 from awkward.operations.ak_to_layout import to_layout
 
 np = NumpyMetadata.instance()
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_any.py` & `awkward-2.1.3/src/awkward/operations/ak_any.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_argcartesian.py` & `awkward-2.1.3/src/awkward/operations/ak_argcartesian.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("argcartesian",)
 import awkward as ak
+from awkward._backends.dispatch import backend_of
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
-cpu = ak._backends.NumpyBackend.instance()
+cpu = NumpyBackend.instance()
 
 
 def argcartesian(
     arrays,
     axis=1,
     *,
     nested=None,
@@ -101,26 +103,26 @@
         return _impl(arrays, axis, nested, parameters, with_name, highlevel, behavior)
 
 
 def _impl(arrays, axis, nested, parameters, with_name, highlevel, behavior):
     axis = regularize_axis(axis)
 
     if isinstance(arrays, dict):
-        backend = ak._backends.backend_of(*arrays.values(), default=cpu)
+        backend = backend_of(*arrays.values(), default=cpu)
         behavior = behavior_of(*arrays.values(), behavior=behavior)
         layouts = {
             n: ak._do.local_index(
                 ak.operations.to_layout(x, allow_record=False, allow_other=False),
                 axis,
             ).to_backend(backend)
             for n, x in arrays.items()
         }
     else:
         arrays = list(arrays)
-        backend = ak._backends.backend_of(*arrays, default=cpu)
+        backend = backend_of(*arrays, default=cpu)
         behavior = behavior_of(*arrays, behavior=behavior)
         layouts = [
             ak._do.local_index(
                 ak.operations.to_layout(x, allow_record=False, allow_other=False),
                 axis,
             ).to_backend(backend)
             for x in arrays
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_argcombinations.py` & `awkward-2.1.3/src/awkward/operations/ak_argcombinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_argmax.py` & `awkward-2.1.3/src/awkward/operations/ak_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_argmin.py` & `awkward-2.1.3/src/awkward/operations/ak_argmin.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_argsort.py` & `awkward-2.1.3/src/awkward/operations/ak_argsort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_backend.py` & `awkward-2.1.3/src/awkward/operations/ak_backend.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("backend",)
 
 import awkward as ak
+from awkward._backends.dispatch import backend_of
 
 
 def backend(*arrays) -> str:
     """
     Args:
         arrays: Array-like data (anything #ak.to_layout recognizes).
 
@@ -24,9 +25,9 @@
         "ak.backend",
         {"*arrays": arrays},
     ):
         return _impl(arrays)
 
 
 def _impl(arrays) -> str:
-    backend_impl = ak._backends.backend_of(*arrays, default=None)
+    backend_impl = backend_of(*arrays, default=None)
     return backend_impl.name
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_broadcast_arrays.py` & `awkward-2.1.3/src/awkward/operations/ak_broadcast_arrays.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("broadcast_arrays",)
 import awkward as ak
+from awkward._backends.dispatch import backend_of
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import unsupported
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
-cpu = ak._backends.NumpyBackend.instance()
+cpu = NumpyBackend.instance()
 
 
 def broadcast_arrays(
     *arrays,
     depth_limit=None,
     broadcast_parameters_rule="one_to_one",
     left_broadcast=True,
@@ -202,15 +204,15 @@
     depth_limit,
     broadcast_parameters_rule,
     left_broadcast,
     right_broadcast,
     highlevel,
     behavior,
 ):
-    backend = ak._backends.backend_of(*arrays, default=cpu)
+    backend = backend_of(*arrays, default=cpu)
 
     inputs = []
     for x in arrays:
         y = ak.operations.to_layout(x, allow_record=True, allow_other=True)
         if not isinstance(y, (ak.contents.Content, ak.Record)):
             y = ak.contents.NumpyArray(backend.nplike.asarray([y]))
         inputs.append(y.to_backend(backend))
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_broadcast_fields.py` & `awkward-2.1.3/src/awkward/operations/ak_broadcast_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("broadcast_fields",)
 import awkward as ak
+from awkward._backends.dispatch import backend_of
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
 from awkward._layout import wrap_layout
 
-cpu = ak._backends.NumpyBackend.instance()
+cpu = NumpyBackend.instance()
 
 
 def broadcast_fields(
     *arrays,
     highlevel=True,
     behavior=None,
 ):
@@ -56,15 +58,15 @@
             "behavior": behavior,
         },
     ):
         return _impl(arrays, highlevel, behavior)
 
 
 def _impl(arrays, highlevel, behavior):
-    backend = ak._backends.backend_of(*arrays, default=cpu)
+    backend = backend_of(*arrays, default=cpu)
     layouts = [ak.to_layout(x).to_backend(backend) for x in arrays]
     behavior = behavior_of(*arrays, behavior=behavior)
 
     def identity(content):
         return content
 
     def descend_to_record_or_identity(layout, pullback=identity):
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_cartesian.py` & `awkward-2.1.3/src/awkward/operations/ak_cartesian.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("cartesian",)
 import awkward as ak
+from awkward._backends.dispatch import backend_of
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
-cpu = ak._backends.NumpyBackend.instance()
+cpu = NumpyBackend.instance()
 
 
 def cartesian(
     arrays,
     axis=1,
     *,
     nested=None,
@@ -203,26 +205,26 @@
     ):
         return _impl(arrays, axis, nested, parameters, with_name, highlevel, behavior)
 
 
 def _impl(arrays, axis, nested, parameters, with_name, highlevel, behavior):
     axis = regularize_axis(axis)
     if isinstance(arrays, dict):
-        backend = ak._backends.backend_of(*arrays.values(), default=cpu)
+        backend = backend_of(*arrays.values(), default=cpu)
         behavior = behavior_of(*arrays.values(), behavior=behavior)
         array_layouts = {
             name: ak.operations.to_layout(
                 layout, allow_record=False, allow_other=False
             ).to_backend(backend)
             for name, layout in arrays.items()
         }
 
     else:
         arrays = list(arrays)
-        backend = ak._backends.backend_of(*arrays, default=cpu)
+        backend = backend_of(*arrays, default=cpu)
         behavior = behavior_of(*arrays, behavior=behavior)
         array_layouts = [
             ak.operations.to_layout(
                 layout, allow_record=False, allow_other=False
             ).to_backend(backend)
             for layout in arrays
         ]
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_categories.py` & `awkward-2.1.3/src/awkward/operations/ak_categories.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_combinations.py` & `awkward-2.1.3/src/awkward/operations/ak_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_concatenate.py` & `awkward-2.1.3/src/awkward/operations/ak_concatenate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("concatenate",)
 import awkward as ak
-from awkward._backends import NumpyBackend, backend_of
+from awkward._backends.dispatch import backend_of
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_integer, regularize_axis
 from awkward._typing import Sequence
 from awkward.contents import Content
 from awkward.operations.ak_fill_none import fill_none
@@ -49,15 +50,15 @@
     ):
         return _impl(arrays, axis, mergebool, highlevel, behavior)
 
 
 def _impl(arrays, axis, mergebool, highlevel, behavior):
     axis = regularize_axis(axis)
     # Simple single-array, axis=0 fast-path
-    backend = ak._backends.backend_of(*arrays, default=cpu)
+    backend = backend_of(*arrays, default=cpu)
     behavior = behavior_of(*arrays, behavior=behavior)
     if (
         # Is an array with a known backend
         backend_of(arrays, default=None)
         is not None
     ):
         # Convert the array to a layout object
@@ -139,15 +140,15 @@
                     if x.is_option and x.content.is_list:
                         nextinputs.append(fill_none(x, [], axis=0, highlevel=False))
                     else:
                         nextinputs.append(x)
                 inputs = nextinputs
 
             if depth == posaxis:
-                backend = ak._backends.backend_of(*inputs, default=cpu)
+                backend = backend_of(*inputs, default=cpu)
 
                 length = None
                 for x in inputs:
                     if isinstance(x, ak.contents.Content):
                         if not is_integer(length):
                             length = x.length
                         elif length != x.length and is_integer(x.length):
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_copy.py` & `awkward-2.1.3/src/awkward/operations/ak_copy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_corr.py` & `awkward-2.1.3/src/awkward/operations/ak_corr.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_count.py` & `awkward-2.1.3/src/awkward/operations/ak_count.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_count_nonzero.py` & `awkward-2.1.3/src/awkward/operations/ak_count_nonzero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_covar.py` & `awkward-2.1.3/src/awkward/operations/ak_covar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_drop_none.py` & `awkward-2.1.3/src/awkward/operations/ak_drop_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_fields.py` & `awkward-2.1.3/src/awkward/operations/ak_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_fill_none.py` & `awkward-2.1.3/src/awkward/operations/ak_fill_none.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("fill_none",)
 import numbers
 
 import awkward as ak
+from awkward._backends.dispatch import backend_of
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_sized_iterable, regularize_axis
 
 np = NumpyMetadata.instance()
-cpu = ak._backends.NumpyBackend.instance()
+cpu = NumpyBackend.instance()
 
 
 def fill_none(array, value, axis=-1, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         value: Data with which to replace None.
@@ -69,15 +71,15 @@
         return _impl(array, value, axis, highlevel, behavior)
 
 
 def _impl(array, value, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     arraylayout = ak.operations.to_layout(array, allow_record=True, allow_other=False)
     behavior = behavior_of(array, value, behavior=behavior)
-    backend = ak._backends.backend_of(arraylayout, default=cpu)
+    backend = backend_of(arraylayout, default=cpu)
 
     # Convert value type to appropriate layout
     if (
         isinstance(value, np.ndarray)
         and issubclass(value.dtype.type, (np.bool_, np.number))
         and len(value.shape) != 0
     ):
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_firsts.py` & `awkward-2.1.3/src/awkward/operations/ak_firsts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_flatten.py` & `awkward-2.1.3/src/awkward/operations/ak_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_from_arrow.py` & `awkward-2.1.3/src/awkward/operations/ak_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_from_arrow_schema.py` & `awkward-2.1.3/src/awkward/operations/ak_from_arrow_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_from_avro_file.py` & `awkward-2.1.3/src/awkward/operations/ak_from_avro_file.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_from_buffers.py` & `awkward-2.1.3/src/awkward/operations/ak_from_buffers.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 __all__ = ("from_buffers",)
 
 import math
 
 import awkward as ak
+from awkward._backends.dispatch import regularize_backend
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_integer
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
@@ -105,15 +106,15 @@
     buffer_key,
     backend,
     byteorder,
     highlevel,
     behavior,
     simplify,
 ):
-    backend = ak._backends.regularize_backend(backend)
+    backend = regularize_backend(backend)
 
     if isinstance(form, str):
         if ak.types.numpytype.is_primitive(form):
             form = ak.forms.NumpyForm(form)
         else:
             form = ak.forms.from_json(form)
     elif isinstance(form, dict):
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_from_categorical.py` & `awkward-2.1.3/src/awkward/operations/ak_from_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_from_cupy.py` & `awkward-2.1.3/src/awkward/operations/ak_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_from_iter.py` & `awkward-2.1.3/src/awkward/operations/ak_from_iter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_from_jax.py` & `awkward-2.1.3/src/awkward/operations/ak_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_from_json.py` & `awkward-2.1.3/src/awkward/operations/ak_from_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_from_numpy.py` & `awkward-2.1.3/src/awkward/operations/ak_from_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_from_parquet.py` & `awkward-2.1.3/src/awkward/operations/ak_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_from_rdataframe.py` & `awkward-2.1.3/src/awkward/operations/ak_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_from_regular.py` & `awkward-2.1.3/src/awkward/operations/ak_from_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_full_like.py` & `awkward-2.1.3/src/awkward/operations/ak_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_is_categorical.py` & `awkward-2.1.3/src/awkward/operations/ak_is_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_is_none.py` & `awkward-2.1.3/src/awkward/operations/ak_is_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_is_tuple.py` & `awkward-2.1.3/src/awkward/operations/ak_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_is_valid.py` & `awkward-2.1.3/src/awkward/operations/ak_is_valid.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_isclose.py` & `awkward-2.1.3/src/awkward/operations/ak_isclose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_linear_fit.py` & `awkward-2.1.3/src/awkward/operations/ak_linear_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("linear_fit",)
 import awkward as ak
-from awkward._backends import backend_of
+from awkward._backends.dispatch import backend_of
 from awkward._behavior import behavior_of
 from awkward._layout import wrap_layout
 from awkward._nplikes import ufuncs
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 from awkward._util import unset
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_local_index.py` & `awkward-2.1.3/src/awkward/operations/ak_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_mask.py` & `awkward-2.1.3/src/awkward/operations/ak_mask.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_max.py` & `awkward-2.1.3/src/awkward/operations/ak_max.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_mean.py` & `awkward-2.1.3/src/awkward/operations/ak_mean.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_merge_option_of_records.py` & `awkward-2.1.3/src/awkward/operations/ak_merge_option_of_records.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("merge_option_of_records",)
 import awkward as ak
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
-cpu = ak._backends.NumpyBackend.instance()
+cpu = NumpyBackend.instance()
 
 
 def merge_option_of_records(array, axis=-1, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (int): The dimension at which this operation is applied.
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_merge_union_of_records.py` & `awkward-2.1.3/src/awkward/operations/ak_merge_union_of_records.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("merge_union_of_records",)
 import awkward as ak
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import ArrayLike, NumpyMetadata
 from awkward._regularize import regularize_axis
 
 np = NumpyMetadata.instance()
-cpu = ak._backends.NumpyBackend.instance()
+cpu = NumpyBackend.instance()
 
 
 def merge_union_of_records(array, axis=-1, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         axis (int): The dimension at which this operation is applied.
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_metadata_from_parquet.py` & `awkward-2.1.3/src/awkward/operations/ak_metadata_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_min.py` & `awkward-2.1.3/src/awkward/operations/ak_min.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_moment.py` & `awkward-2.1.3/src/awkward/operations/ak_moment.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_nan_to_none.py` & `awkward-2.1.3/src/awkward/operations/ak_nan_to_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_nan_to_num.py` & `awkward-2.1.3/src/awkward/operations/ak_nan_to_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_num.py` & `awkward-2.1.3/src/awkward/operations/ak_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_ones_like.py` & `awkward-2.1.3/src/awkward/operations/ak_ones_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_pad_none.py` & `awkward-2.1.3/src/awkward/operations/ak_pad_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_parameters.py` & `awkward-2.1.3/src/awkward/operations/ak_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_prod.py` & `awkward-2.1.3/src/awkward/operations/ak_prod.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_ptp.py` & `awkward-2.1.3/src/awkward/operations/ak_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_ravel.py` & `awkward-2.1.3/src/awkward/operations/ak_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_run_lengths.py` & `awkward-2.1.3/src/awkward/operations/ak_run_lengths.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("run_lengths",)
 import awkward as ak
+from awkward._backends.dispatch import backend_of
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 
 np = NumpyMetadata.instance()
-cpu = ak._backends.NumpyBackend.instance()
+cpu = NumpyBackend.instance()
 
 
 def run_lengths(array, *, highlevel=True, behavior=None):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         highlevel (bool): If True, return an #ak.Array; otherwise, return
@@ -92,15 +94,15 @@
             "behavior": behavior,
         },
     ):
         return _impl(array, highlevel, behavior)
 
 
 def _impl(array, highlevel, behavior):
-    backend = ak._backends.backend_of(array, default=cpu)
+    backend = backend_of(array, default=cpu)
 
     def lengths_of(data, offsets):
         if backend.nplike.is_own_array(data):
             size = data.size
         else:
             layout = ak.to_layout(data)
             size = layout.length
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_singletons.py` & `awkward-2.1.3/src/awkward/operations/ak_singletons.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_softmax.py` & `awkward-2.1.3/src/awkward/operations/ak_softmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_sort.py` & `awkward-2.1.3/src/awkward/operations/ak_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_std.py` & `awkward-2.1.3/src/awkward/operations/ak_std.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_strings_astype.py` & `awkward-2.1.3/src/awkward/operations/ak_strings_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_sum.py` & `awkward-2.1.3/src/awkward/operations/ak_sum.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_arrow.py` & `awkward-2.1.3/src/awkward/operations/ak_to_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_arrow_table.py` & `awkward-2.1.3/src/awkward/operations/ak_to_arrow_table.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_backend.py` & `awkward-2.1.3/src/awkward/operations/ak_to_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_backend",)
 import awkward as ak
+from awkward._backends.dispatch import regularize_backend
 from awkward._behavior import behavior_of
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
@@ -62,9 +63,9 @@
 def _impl(array, backend, highlevel, behavior):
     layout = ak.operations.to_layout(
         array,
         allow_record=True,
         allow_other=True,
     )
     behavior = behavior_of(array, behavior=behavior)
-    backend_layout = layout.to_backend(ak._backends.regularize_backend(backend))
+    backend_layout = layout.to_backend(regularize_backend(backend))
     return wrap_layout(backend_layout, behavior, highlevel)
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_buffers.py` & `awkward-2.1.3/src/awkward/operations/ak_to_buffers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_buffers",)
 
 import awkward as ak
+from awkward._backends.dispatch import regularize_backend
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
 
 def to_buffers(
     array,
@@ -135,15 +136,15 @@
         )
 
 
 def _impl(array, container, buffer_key, form_key, id_start, backend, byteorder):
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
 
     if backend is not None:
-        backend = ak._backends.regularize_backend(backend)
+        backend = regularize_backend(backend)
 
     return ak._do.to_buffers(
         layout,
         container=container,
         buffer_key=buffer_key,
         form_key=form_key,
         id_start=id_start,
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_categorical.py` & `awkward-2.1.3/src/awkward/operations/ak_to_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_cupy.py` & `awkward-2.1.3/src/awkward/operations/ak_to_cupy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_cupy",)
 
 import awkward as ak
+from awkward._backends.cupy import CupyBackend
 
 
 def to_cupy(array):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
 
@@ -27,11 +28,11 @@
     ):
         return _impl(array)
 
 
 def _impl(array):
     layout = ak.to_layout(array, allow_record=False)
 
-    backend = ak._backends.CupyBackend.instance()
+    backend = CupyBackend.instance()
     cupy_layout = layout.to_backend(backend)
 
     return cupy_layout.to_backend_array(allow_missing=False)
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_dataframe.py` & `awkward-2.1.3/src/awkward/operations/ak_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_jax.py` & `awkward-2.1.3/src/awkward/operations/ak_to_jax.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_jax",)
 
 import awkward as ak
+from awkward._backends.jax import JaxBackend
 
 
 def to_jax(array):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
 
@@ -27,11 +28,11 @@
     ):
         return _impl(array)
 
 
 def _impl(array):
     layout = ak.to_layout(array, allow_record=False)
 
-    backend = ak._backends.JaxBackend.instance()
+    backend = JaxBackend.instance()
     numpy_layout = layout.to_backend(backend)
 
     return numpy_layout.to_backend_array(allow_missing=False)
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_json.py` & `awkward-2.1.3/src/awkward/operations/ak_to_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_layout.py` & `awkward-2.1.3/src/awkward/operations/ak_to_layout.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from collections.abc import Iterable
 
 from awkward_cpp.lib import _ext
 
 import awkward as ak
 from awkward import _errors
+from awkward._backends.typetracer import TypeTracerBackend
 from awkward._nplikes.cupy import Cupy
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.typetracer import TypeTracer
 
 np = NumpyMetadata.instance()
@@ -87,15 +88,15 @@
             array, regulararray=regulararray, highlevel=False
         )
 
     elif Jax.is_own_array(array):
         return ak.operations.from_jax(array, regulararray=regulararray, highlevel=False)
 
     elif TypeTracer.is_own_array(array):
-        backend = ak._backends.TypeTracerBackend.instance()
+        backend = TypeTracerBackend.instance()
 
         if len(array.shape) == 0:
             array = backend.nplike.reshape(array, (1,))
 
         if array.dtype.kind in {"S", "U"}:
             raise NotImplementedError(
                 "strings are currently not supported for typetracer arrays"
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_list.py` & `awkward-2.1.3/src/awkward/operations/ak_to_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_numpy.py` & `awkward-2.1.3/src/awkward/operations/ak_to_numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_numpy",)
-
 import awkward as ak
+from awkward._backends.numpy import NumpyBackend
 
 
 def to_numpy(array, *, allow_missing=True):
     """
     Args:
         array: Array-like data (anything #ak.to_layout recognizes).
         allow_missing (bool): allow missing (None) values.
@@ -44,11 +44,11 @@
 
 def _impl(array, allow_missing):
     import numpy  # noqa: TID251
 
     with numpy.errstate(invalid="ignore"):
         layout = ak.to_layout(array, allow_record=False)
 
-        backend = ak._backends.NumpyBackend.instance()
+        backend = NumpyBackend.instance()
         numpy_layout = layout.to_backend(backend)
 
         return numpy_layout.to_backend_array(allow_missing=allow_missing)
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_packed.py` & `awkward-2.1.3/src/awkward/operations/ak_to_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_parquet.py` & `awkward-2.1.3/src/awkward/operations/ak_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_rdataframe.py` & `awkward-2.1.3/src/awkward/operations/ak_to_rdataframe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("to_rdataframe",)
-
 from collections.abc import Mapping
 
 import awkward as ak
+from awkward._backends.numpy import NumpyBackend
 
-cpu = ak._backends.NumpyBackend.instance()
+cpu = NumpyBackend.instance()
 
 
 def to_rdataframe(arrays, *, flatlist_as_rvec=True):
     """
     Args:
         arrays (dict of arrays): Each value in this dict can be any array-like data
             that #ak.to_layout recognizes, but they must all have the same length.
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_to_regular.py` & `awkward-2.1.3/src/awkward/operations/ak_to_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_transform.py` & `awkward-2.1.3/src/awkward/operations/ak_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("transform",)
 import copy
 
 import awkward as ak
+from awkward._backends.dispatch import backend_of
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
 from awkward._layout import wrap_layout
 
-cpu = ak._backends.NumpyBackend.instance()
+cpu = NumpyBackend.instance()
 
 
 def transform(
     transformation,
     array,
     *more_arrays,
     depth_context=None,
@@ -457,15 +459,15 @@
     numpy_to_regular,
     regular_to_jagged,
     return_value,
     behavior,
     highlevel,
 ):
     behavior = behavior_of(array, *more_arrays, behavior=behavior)
-    backend = ak._backends.backend_of(array, *more_arrays, default=cpu)
+    backend = backend_of(array, *more_arrays, default=cpu)
     layout = ak.operations.ak_to_layout._impl(
         array, allow_record=False, allow_other=False, regulararray=True
     ).to_backend(backend)
     more_layouts = [
         ak.operations.ak_to_layout._impl(
             x, allow_record=False, allow_other=False, regulararray=True
         ).to_backend(backend)
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_type.py` & `awkward-2.1.3/src/awkward/operations/ak_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_unflatten.py` & `awkward-2.1.3/src/awkward/operations/ak_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_unzip.py` & `awkward-2.1.3/src/awkward/operations/ak_unzip.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_validity_error.py` & `awkward-2.1.3/src/awkward/operations/ak_validity_error.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_values_astype.py` & `awkward-2.1.3/src/awkward/operations/ak_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_var.py` & `awkward-2.1.3/src/awkward/operations/ak_var.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_where.py` & `awkward-2.1.3/src/awkward/operations/ak_where.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("where",)
 import awkward as ak
+from awkward._backends.dispatch import backend_of
+from awkward._backends.numpy import NumpyBackend
 from awkward._behavior import behavior_of
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
-cpu = ak._backends.NumpyBackend.instance()
+cpu = NumpyBackend.instance()
 
 
 @ak._connect.numpy.implements("where")
 def where(condition, *args, mergebool=True, highlevel=True, behavior=None):
     """
     Args:
         condition: Array-like data (anything #ak.to_layout recognizes) of booleans.
@@ -72,15 +74,15 @@
         )
 
 
 def _impl1(condition, mergebool, highlevel, behavior):
     akcondition = ak.operations.to_layout(
         condition, allow_record=False, allow_other=False
     )
-    backend = ak._backends.backend_of(akcondition, default=cpu)
+    backend = backend_of(akcondition, default=cpu)
 
     akcondition = ak.contents.NumpyArray(ak.operations.to_numpy(akcondition))
     out = backend.nplike.nonzero(ak.operations.to_numpy(akcondition))
     if highlevel:
         return tuple(
             wrap_layout(
                 ak.contents.NumpyArray(x),
@@ -101,15 +103,15 @@
     right = ak.operations.to_layout(y, allow_record=False, allow_other=True)
 
     good_arrays = [akcondition]
     if isinstance(left, ak.contents.Content):
         good_arrays.append(left)
     if isinstance(right, ak.contents.Content):
         good_arrays.append(right)
-    backend = ak._backends.backend_of(*good_arrays, default=cpu)
+    backend = backend_of(*good_arrays, default=cpu)
 
     def action(inputs, **kwargs):
         akcondition, left, right = inputs
         if isinstance(akcondition, ak.contents.NumpyArray):
             npcondition = backend.index_nplike.asarray(akcondition)
             tags = ak.index.Index8((npcondition == 0).view(np.int8))
             index = ak.index.Index64(
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_with_field.py` & `awkward-2.1.3/src/awkward/operations/ak_with_field.py`

 * *Files 13% similar despite different names*

```diff
@@ -78,24 +78,41 @@
     else:
         # If we have an iterable here, pull out the only ti
         if is_non_string_like_sequence(where):
             where = where[0]
 
         behavior = behavior_of(base, what, behavior=behavior)
         base = ak.operations.to_layout(base, allow_record=True, allow_other=False)
-
-        if len(base.fields) == 0:
-            raise ValueError("no tuples or records in array; cannot add a new field")
-
         what = ak.operations.to_layout(what, allow_record=True, allow_other=True)
 
         keys = copy.copy(base.fields)
         if where in base.fields:
             keys.remove(where)
 
+        def purelist_is_record(layout):
+            result = False
+
+            def action_is_record(input, **kwargs):
+                nonlocal result
+
+                if input.is_record:
+                    result = True
+                    return input
+                elif input.is_union:
+                    result = all(purelist_is_record(x) for x in input.contents)
+                    return input
+                else:
+                    return None
+
+            ak._do.recursively_apply(layout, action_is_record, return_array=False)
+            return result
+
+        if not purelist_is_record(base):
+            raise ValueError("no tuples or records in array; cannot add a new field")
+
         def action(inputs, **kwargs):
             base, what = inputs
             backend = base.backend
 
             if isinstance(base, ak.contents.RecordArray):
                 if what is None:
                     what = ak.contents.IndexedOptionArray(
```

### Comparing `awkward-2.1.2/src/awkward/operations/ak_with_name.py` & `awkward-2.1.3/src/awkward/operations/ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_with_parameter.py` & `awkward-2.1.3/src/awkward/operations/ak_with_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_without_field.py` & `awkward-2.1.3/src/awkward/operations/ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_without_parameters.py` & `awkward-2.1.3/src/awkward/operations/ak_without_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_zeros_like.py` & `awkward-2.1.3/src/awkward/operations/ak_zeros_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/operations/ak_zip.py` & `awkward-2.1.3/src/awkward/operations/ak_zip.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/types/__init__.py` & `awkward-2.1.3/src/awkward/types/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/types/_awkward_datashape_parser.py` & `awkward-2.1.3/src/awkward/types/_awkward_datashape_parser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/types/arraytype.py` & `awkward-2.1.3/src/awkward/types/arraytype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/types/listtype.py` & `awkward-2.1.3/src/awkward/types/listtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/types/numpytype.py` & `awkward-2.1.3/src/awkward/types/numpytype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/types/optiontype.py` & `awkward-2.1.3/src/awkward/types/optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/types/recordtype.py` & `awkward-2.1.3/src/awkward/types/recordtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/types/regulartype.py` & `awkward-2.1.3/src/awkward/types/regulartype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/types/scalartype.py` & `awkward-2.1.3/src/awkward/types/scalartype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/types/type.py` & `awkward-2.1.3/src/awkward/types/type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/types/uniontype.py` & `awkward-2.1.3/src/awkward/types/uniontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/src/awkward/types/unknowntype.py` & `awkward-2.1.3/src/awkward/types/unknowntype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0002_minimal_listarray.py` & `awkward-2.1.3/tests/test_0002_minimal_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0008_slices_and_getitem.py` & `awkward-2.1.3/tests/test_0008_slices_and_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0011_listarray.py` & `awkward-2.1.3/tests/test_0011_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0013_error_handling_struct.py` & `awkward-2.1.3/tests/test_0013_error_handling_struct.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0014_finish_up_getitem.py` & `awkward-2.1.3/tests/test_0014_finish_up_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0018_fromiter_fillable.py` & `awkward-2.1.3/tests/test_0018_fromiter_fillable.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0019_use_json_library.py` & `awkward-2.1.3/tests/test_0019_use_json_library.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0020_support_unsigned_indexes.py` & `awkward-2.1.3/tests/test_0020_support_unsigned_indexes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0021_emptyarray.py` & `awkward-2.1.3/tests/test_0021_emptyarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0023_regular_array.py` & `awkward-2.1.3/tests/test_0023_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0024_use_regular_array.py` & `awkward-2.1.3/tests/test_0024_use_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0025_record_array.py` & `awkward-2.1.3/tests/test_0025_record_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0028_add_dressed_types.py` & `awkward-2.1.3/tests/test_0028_add_dressed_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0032_replace_dressedtype.py` & `awkward-2.1.3/tests/test_0032_replace_dressedtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0046_start_indexedarray.py` & `awkward-2.1.3/tests/test_0046_start_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0049_distinguish_record_and_recordarray_behaviors.py` & `awkward-2.1.3/tests/test_0049_distinguish_record_and_recordarray_behaviors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0057_introducing_forms.py` & `awkward-2.1.3/tests/test_0057_introducing_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0070_argmin_and_argmax.py` & `awkward-2.1.3/tests/test_0070_argmin_and_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0072_fillna_operation.py` & `awkward-2.1.3/tests/test_0072_fillna_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0074_argsort_and_sort.py` & `awkward-2.1.3/tests/test_0074_argsort_and_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0077_zip_operation.py` & `awkward-2.1.3/tests/test_0077_zip_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0078_argcross_and_cross.py` & `awkward-2.1.3/tests/test_0078_argcross_and_cross.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0079_argchoose_and_choose.py` & `awkward-2.1.3/tests/test_0079_argchoose_and_choose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0080_flatpandas_multiindex_rows_and_columns.py` & `awkward-2.1.3/tests/test_0080_flatpandas_multiindex_rows_and_columns.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0084_start_unionarray.py` & `awkward-2.1.3/tests/test_0084_start_unionarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import numpy as np
 import pytest
 
 import awkward as ak
+from awkward._backends.numpy import NumpyBackend
 
 to_list = ak.operations.to_list
 
 
 def test_getitem():
     content0 = ak.operations.from_iter(
         [[1.1, 2.2, 3.3], [], [4.4, 5.5]], highlevel=False
     )
     content1 = ak.operations.from_iter(
         ["one", "two", "three", "four", "five"], highlevel=False
     )
     tags = ak.index.Index8(np.array([1, 1, 0, 0, 1, 0, 1, 1], dtype=np.int8))
 
-    backend = ak._backends.NumpyBackend.instance()
+    backend = NumpyBackend.instance()
     array32 = ak.contents.UnionArray.regular_index(
         tags, index_cls=ak.index.Index32, backend=backend
     )
     arrayU32 = ak.contents.UnionArray.regular_index(
         tags, index_cls=ak.index.IndexU32, backend=backend
     )
     array64 = ak.contents.UnionArray.regular_index(
```

### Comparing `awkward-2.1.2/tests/test_0086_nep13_ufunc.py` & `awkward-2.1.3/tests/test_0086_nep13_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0089_numpy_functions.py` & `awkward-2.1.3/tests/test_0089_numpy_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0093_simplify_uniontypes_and_optiontypes.py` & `awkward-2.1.3/tests/test_0093_simplify_uniontypes_and_optiontypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0107_assign_fields_to_records.py` & `awkward-2.1.3/tests/test_0107_assign_fields_to_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0111_jagged_and_masked_getitem.py` & `awkward-2.1.3/tests/test_0111_jagged_and_masked_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0115_generic_reducer_operation.py` & `awkward-2.1.3/tests/test_0115_generic_reducer_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -801,15 +801,18 @@
     ]
     assert complicated.to_typetracer()["y"].form == complicated["y"].form
 
     with pytest.raises(TypeError):
         to_list(ak.prod(complicated, -1, highlevel=False))
 
     with pytest.raises(TypeError):
-        ak.prod(complicated.to_typetracer(), -1, highlevel=False).form
+        assert (
+            ak.prod(complicated.to_typetracer(), -1, highlevel=False).form
+            == ak.prod(complicated, -1, highlevel=False).form
+        )
 
     assert to_list(ak.prod(complicated["x"], -1, highlevel=False)) == [
         [30],
         [],
         [1, 77],
     ]
     assert (
@@ -826,15 +829,18 @@
         == ak.prod(complicated["y"], -1, highlevel=False).form
     )
 
     with pytest.raises(TypeError):
         to_list(ak.prod(complicated, -2, highlevel=False))
 
     with pytest.raises(TypeError):
-        ak.prod(complicated.to_typetracer(), -2, highlevel=False).form
+        assert (
+            ak.prod(complicated.to_typetracer(), -2, highlevel=False).form
+            == ak.prod(complicated, -2, highlevel=False).form
+        )
     assert to_list(ak.prod(complicated["x"], -2, highlevel=False)) == [
         [2, 3, 5],
         [],
         [7, 11],
     ]
     assert (
         ak.prod(complicated.to_typetracer()["x"], -2, highlevel=False).form
```

### Comparing `awkward-2.1.2/tests/test_0118_numba_cpointers.py` & `awkward-2.1.3/tests/test_0118_numba_cpointers.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         [],
         [4.4, 5.5],
     ]
 
 
 def test_refcount():
     array = ak.highlevel.Array([[1.1, 2.2, 3.3], [], [4.4, 5.5]])
-    array.numba_type
+    array.numba_type  # noqa: B018 (needed to set refcount)
     assert [
         sys.getrefcount(x) == 2
         for x in (
             array._numbaview,
             array._numbaview.lookup,
             array._numbaview.lookup.positions,
             array._numbaview.lookup.arrayptrs,
@@ -465,15 +465,15 @@
             {"x": 1.1, "y": [1]},
             {"x": 2.2, "y": [2, 2]},
             {"x": 3.3, "y": [3, 3, 3]},
             {"x": 4.4, "y": [4, 4, 4, 4]},
         ],
         check_valid=True,
     )[3]
-    record.numba_type
+    record.numba_type  # noqa: B018 (needed to set refcount)
     assert [
         sys.getrefcount(x) == 2
         for x in (
             record._numbaview,
             record._numbaview.arrayview,
             record._numbaview.arrayview.lookup,
             record._numbaview.arrayview.lookup.positions,
```

### Comparing `awkward-2.1.2/tests/test_0119_numexpr_and_broadcast_arrays.py` & `awkward-2.1.3/tests/test_0119_numexpr_and_broadcast_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0124_strings_in_numba.py` & `awkward-2.1.3/tests/test_0124_strings_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0127_tomask_operation.py` & `awkward-2.1.3/tests/test_0127_tomask_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0127b_tomask_operation_numba.py` & `awkward-2.1.3/tests/test_0127b_tomask_operation_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0138_emptyarray_type.py` & `awkward-2.1.3/tests/test_0138_emptyarray_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0150_flatten.py` & `awkward-2.1.3/tests/test_0150_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0163_negative_axis_wrap.py` & `awkward-2.1.3/tests/test_0163_negative_axis_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0166_0167_0170_random_issues.py` & `awkward-2.1.3/tests/test_0166_0167_0170_random_issues.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0173_astype_operation.py` & `awkward-2.1.3/tests/test_0173_astype_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0184_concatenate_operation.py` & `awkward-2.1.3/tests/test_0184_concatenate_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0193_is_none_axis_parameter.py` & `awkward-2.1.3/tests/test_0193_is_none_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0198_tutorial_documentation_1.py` & `awkward-2.1.3/tests/test_0198_tutorial_documentation_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0222_count_with_axis0.py` & `awkward-2.1.3/tests/test_0222_count_with_axis0.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0224_arrow_to_awkward.py` & `awkward-2.1.3/tests/test_0224_arrow_to_awkward.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0264_reduce_last_empty.py` & `awkward-2.1.3/tests/test_0264_reduce_last_empty.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0273_path_for_with_field.py` & `awkward-2.1.3/tests/test_0273_path_for_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0286_broadcast_single_value_with_field.py` & `awkward-2.1.3/tests/test_0286_broadcast_single_value_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0290_bug_fixes_for_hats.py` & `awkward-2.1.3/tests/test_0290_bug_fixes_for_hats.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0315_integerindex.py` & `awkward-2.1.3/tests/test_0315_integerindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0331_pandas_indexedarray.py` & `awkward-2.1.3/tests/test_0331_pandas_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0334_fully_broadcastable_where.py` & `awkward-2.1.3/tests/test_0334_fully_broadcastable_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0339_highlevel_sorting_function.py` & `awkward-2.1.3/tests/test_0339_highlevel_sorting_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0348_form_keys.py` & `awkward-2.1.3/tests/test_0348_form_keys.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0355_mixins.py` & `awkward-2.1.3/tests/test_0355_mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0395_complex_type_arrays.py` & `awkward-2.1.3/tests/test_0395_complex_type_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0395_fix_numba_indexedarray.py` & `awkward-2.1.3/tests/test_0395_fix_numba_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0397_arrays_as_constants_in_numba.py` & `awkward-2.1.3/tests/test_0397_arrays_as_constants_in_numba.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 
 
 def test_refcount():
     array = ak.highlevel.Array([1, 2, 3])
 
     @numba.njit
     def f1():
-        array
+        array  # noqa: B018 (we want to test the unboxing)
         return 3.14
 
     @numba.njit
     def f2():
-        array, array
+        array, array  # noqa: B018 (we want to test the unboxing)
         return 3.14
 
     assert sys.getrefcount(array) == 2
     f1()
     assert sys.getrefcount(array) == 3
     f2()
     assert sys.getrefcount(array) == 5
@@ -36,15 +36,15 @@
 
 
 def test_Array():
     array = ak.highlevel.Array([1, 2, 3])
 
     @numba.njit
     def f1():
-        array
+        array  # noqa: B018 (we want to test the unboxing)
         return 3.14
 
     f1()
     assert (
         sys.getrefcount(array._numbaview),
         sys.getrefcount(array._numbaview.lookup),
     ) == (2, 2)
```

### Comparing `awkward-2.1.2/tests/test_0401_add_categorical_type_for_arrow_dictionary.py` & `awkward-2.1.3/tests/test_0401_add_categorical_type_for_arrow_dictionary.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0404_array_validity_check.py` & `awkward-2.1.3/tests/test_0404_array_validity_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0410_fix_argminmax_positions_for_missing_values.py` & `awkward-2.1.3/tests/test_0410_fix_argminmax_positions_for_missing_values.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0437_stream_of_many_json_files.py` & `awkward-2.1.3/tests/test_0437_stream_of_many_json_files.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0447_preserve_regularness_in_reduce.py` & `awkward-2.1.3/tests/test_0447_preserve_regularness_in_reduce.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0449_merge_many_arrays_in_one_pass.py` & `awkward-2.1.3/tests/test_0449_merge_many_arrays_in_one_pass.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0493_zeros_ones_full_like.py` & `awkward-2.1.3/tests/test_0493_zeros_ones_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0496_provide_local_index.py` & `awkward-2.1.3/tests/test_0496_provide_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0499_getitem_indexedarray_bug.py` & `awkward-2.1.3/tests/test_0499_getitem_indexedarray_bug.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0504_block_ufuncs_for_strings.py` & `awkward-2.1.3/tests/test_0504_block_ufuncs_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0511_copy_and_deepcopy.py` & `awkward-2.1.3/tests/test_0511_copy_and_deepcopy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py` & `awkward-2.1.3/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0549_numba_array_asarray.py` & `awkward-2.1.3/tests/test_0549_numba_array_asarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0557_min_max_initial_argument.py` & `awkward-2.1.3/tests/test_0557_min_max_initial_argument.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0559_fix_booleans_in_numba.py` & `awkward-2.1.3/tests/test_0559_fix_booleans_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0572_numba_array_ndim.py` & `awkward-2.1.3/tests/test_0572_numba_array_ndim.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0582_propagate_context_in_broadcast_and_apply.py` & `awkward-2.1.3/tests/test_0582_propagate_context_in_broadcast_and_apply.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0583_implement_unflatten_function.py` & `awkward-2.1.3/tests/test_0583_implement_unflatten_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0590_allow_regulararray_size_zero.py` & `awkward-2.1.3/tests/test_0590_allow_regulararray_size_zero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py` & `awkward-2.1.3/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0652_tests_of_complex_numbers.py` & `awkward-2.1.3/tests/test_0652_tests_of_complex_numbers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0674_categorical_validation.py` & `awkward-2.1.3/tests/test_0674_categorical_validation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0713_getitem_field_should_simplify_optiontype.py` & `awkward-2.1.3/tests/test_0713_getitem_field_should_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py` & `awkward-2.1.3/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0730_unflatten_axis_parameter.py` & `awkward-2.1.3/tests/test_0730_unflatten_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0733_run_lengths.py` & `awkward-2.1.3/tests/test_0733_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0736_implement_argsort_for_strings.py` & `awkward-2.1.3/tests/test_0736_implement_argsort_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0766_prevent_combinations_of_characters.py` & `awkward-2.1.3/tests/test_0766_prevent_combinations_of_characters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0773_typeparser.py` & `awkward-2.1.3/tests/test_0773_typeparser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0788_indexedarray_carrying_recordarray_parameters.py` & `awkward-2.1.3/tests/test_0788_indexedarray_carrying_recordarray_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0794_ak_cartesian_on_empty_array.py` & `awkward-2.1.3/tests/test_0794_ak_cartesian_on_empty_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0803_argsort_fix_type.py` & `awkward-2.1.3/tests/test_0803_argsort_fix_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0806_empty_lists_cartesian_fix.py` & `awkward-2.1.3/tests/test_0806_empty_lists_cartesian_fix.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0813_full_like_dtype_arg.py` & `awkward-2.1.3/tests/test_0813_full_like_dtype_arg.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0815_broadcast_union_types_to_all_possibilities.py` & `awkward-2.1.3/tests/test_0815_broadcast_union_types_to_all_possibilities.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0828_arrow_datatype_null.py` & `awkward-2.1.3/tests/test_0828_arrow_datatype_null.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0835_datetime_type.py` & `awkward-2.1.3/tests/test_0835_datetime_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0835_datetime_type_pandas.py` & `awkward-2.1.3/tests/test_0835_datetime_type_pandas.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0835_datetime_type_pyarrow.py` & `awkward-2.1.3/tests/test_0835_datetime_type_pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0850_argsort_mask_array.py` & `awkward-2.1.3/tests/test_0850_argsort_mask_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0866_getitem_field_and_flatten_unions.py` & `awkward-2.1.3/tests/test_0866_getitem_field_and_flatten_unions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0875_arrow_null_type.py` & `awkward-2.1.3/tests/test_0875_arrow_null_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0879_non_primitive_with_field.py` & `awkward-2.1.3/tests/test_0879_non_primitive_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0884_index_and_identifier_refactoring.py` & `awkward-2.1.3/tests/test_0884_index_and_identifier_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0889_ptp.py` & `awkward-2.1.3/tests/test_0889_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0896_content_classes_refactoring.py` & `awkward-2.1.3/tests/test_0896_content_classes_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0898_unzip_heterogeneous_records.py` & `awkward-2.1.3/tests/test_0898_unzip_heterogeneous_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0905_leading_zeros_in_unflatten.py` & `awkward-2.1.3/tests/test_0905_leading_zeros_in_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0906_arrow_fixed_size_list_type.py` & `awkward-2.1.3/tests/test_0906_arrow_fixed_size_list_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0910_unflatten_counts_relation.py` & `awkward-2.1.3/tests/test_0910_unflatten_counts_relation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0912_packed.py` & `awkward-2.1.3/tests/test_0912_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0914_types_and_forms.py` & `awkward-2.1.3/tests/test_0914_types_and_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0916_datetime_values_astype.py` & `awkward-2.1.3/tests/test_0916_datetime_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0927_numpy_array_nbytes.py` & `awkward-2.1.3/tests/test_0927_numpy_array_nbytes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0930_bug_in_unionarray_purelist_parameter.py` & `awkward-2.1.3/tests/test_0930_bug_in_unionarray_purelist_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0945_argsort_sort_nan_array.py` & `awkward-2.1.3/tests/test_0945_argsort_sort_nan_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0958_new_forms_must_accept_old_form_json.py` & `awkward-2.1.3/tests/test_0958_new_forms_must_accept_old_form_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0959__getitem_array_implementation.py` & `awkward-2.1.3/tests/test_0959__getitem_array_implementation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0975_mask_multidimensional_numpy_array.py` & `awkward-2.1.3/tests/test_0975_mask_multidimensional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0979_where_multidimentional_numpy_array.py` & `awkward-2.1.3/tests/test_0979_where_multidimentional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0982_missing_case_in_nonlocal_reducers.py` & `awkward-2.1.3/tests/test_0982_missing_case_in_nonlocal_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0984_ravel.py` & `awkward-2.1.3/tests/test_0984_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_0992_correct_ptp_unmasking.py` & `awkward-2.1.3/tests/test_0992_correct_ptp_unmasking.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py` & `awkward-2.1.3/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1017_numpyarray_broadcast.py` & `awkward-2.1.3/tests/test_1017_numpyarray_broadcast.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1030_mixin_class_name.py` & `awkward-2.1.3/tests/test_1030_mixin_class_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1031_start_getitem_next.py` & `awkward-2.1.3/tests/test_1031_start_getitem_next.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1031b_start_getitem_next_specialized.py` & `awkward-2.1.3/tests/test_1031b_start_getitem_next_specialized.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1049_concatenate_single_array.py` & `awkward-2.1.3/tests/test_1049_concatenate_single_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1055_fill_none_numpy_dimension.py` & `awkward-2.1.3/tests/test_1055_fill_none_numpy_dimension.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1059_localindex.py` & `awkward-2.1.3/tests/test_1059_localindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1066_to_numpy_masked_structured_array.py` & `awkward-2.1.3/tests/test_1066_to_numpy_masked_structured_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1071_mask_identity_false_should_not_return_option_type.py` & `awkward-2.1.3/tests/test_1071_mask_identity_false_should_not_return_option_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1072_sort.py` & `awkward-2.1.3/tests/test_1072_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1074_combinations.py` & `awkward-2.1.3/tests/test_1074_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1075_validityerror.py` & `awkward-2.1.3/tests/test_1075_validityerror.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1110_type_tracer_1.py` & `awkward-2.1.3/tests/test_1110_type_tracer_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1116_project_maskedarrays.py` & `awkward-2.1.3/tests/test_1116_project_maskedarrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1125_to_arrow_from_arrow.py` & `awkward-2.1.3/tests/test_1125_to_arrow_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1132_utility_methods_for_highlevel_functions.py` & `awkward-2.1.3/tests/test_1132_utility_methods_for_highlevel_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1134_from_buffers_to_buffers.py` & `awkward-2.1.3/tests/test_1134_from_buffers_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1135_rpad_operation.py` & `awkward-2.1.3/tests/test_1135_rpad_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1136_regulararray_zeros_in_shape.py` & `awkward-2.1.3/tests/test_1136_regulararray_zeros_in_shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1137_num.py` & `awkward-2.1.3/tests/test_1137_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1142_numbers_to_type.py` & `awkward-2.1.3/tests/test_1142_numbers_to_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1149_datetime_sort.py` & `awkward-2.1.3/tests/test_1149_datetime_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1154_arrow_tables_should_preserve_parameters.py` & `awkward-2.1.3/tests/test_1154_arrow_tables_should_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1162_ak_from_json_schema.py` & `awkward-2.1.3/tests/test_1162_ak_from_json_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1183_bugs_found_by_dask_project_2.py` & `awkward-2.1.3/tests/test_1183_bugs_found_by_dask_project_2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1189_fix_singletons_for_non_optional_data.py` & `awkward-2.1.3/tests/test_1189_fix_singletons_for_non_optional_data.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1192_iterables_in___array_function__.py` & `awkward-2.1.3/tests/test_1192_iterables_in___array_function__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1193_is_none_nested_option.py` & `awkward-2.1.3/tests/test_1193_is_none_nested_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1233_ak_with_name.py` & `awkward-2.1.3/tests/test_1233_ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1240_v2_implementation_of_numba_1.py` & `awkward-2.1.3/tests/test_1240_v2_implementation_of_numba_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1259_simplify_optiontype.py` & `awkward-2.1.3/tests/test_1259_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1260_simplify_masked_option_types.py` & `awkward-2.1.3/tests/test_1260_simplify_masked_option_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1271_fix_4D_reducers.py` & `awkward-2.1.3/tests/test_1271_fix_4D_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1294_to_and_from_parquet.py` & `awkward-2.1.3/tests/test_1294_to_and_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py` & `awkward-2.1.3/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1300_awkward_to_cpp_converter_with_cling.py` & `awkward-2.1.3/tests/test_1300_awkward_to_cpp_converter_with_cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1300b_same_for_numba.py` & `awkward-2.1.3/tests/test_1300b_same_for_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1308_zip_after_option.py` & `awkward-2.1.3/tests/test_1308_zip_after_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1318_array_function_types.py` & `awkward-2.1.3/tests/test_1318_array_function_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1320_mask_identity_defaults.py` & `awkward-2.1.3/tests/test_1320_mask_identity_defaults.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1344_broadcast_arrays_depth_limit.py` & `awkward-2.1.3/tests/test_1344_broadcast_arrays_depth_limit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1345_avro_reader.py` & `awkward-2.1.3/tests/test_1345_avro_reader.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1351_is_tuple.py` & `awkward-2.1.3/tests/test_1351_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1374_to_rdataframe.py` & `awkward-2.1.3/tests/test_1374_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1377_ravel_string.py` & `awkward-2.1.3/tests/test_1377_ravel_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1379_reducers_with_axis_None_and_typetracers.py` & `awkward-2.1.3/tests/test_1379_reducers_with_axis_None_and_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1399_from_jax.py` & `awkward-2.1.3/tests/test_1399_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1399_to_jax.py` & `awkward-2.1.3/tests/test_1399_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1405_slicing_untested_cases.py` & `awkward-2.1.3/tests/test_1405_slicing_untested_cases.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1415_behaviour_forwarding.py` & `awkward-2.1.3/tests/test_1415_behaviour_forwarding.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1440_start_v2_to_parquet.py` & `awkward-2.1.3/tests/test_1440_start_v2_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1447_jax_autodiff_slices_ufuncs.py` & `awkward-2.1.3/tests/test_1447_jax_autodiff_slices_ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1449_v2_to_json_from_json_functions.py` & `awkward-2.1.3/tests/test_1449_v2_to_json_from_json_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1453_write_single_records_to_parquet.py` & `awkward-2.1.3/tests/test_1453_write_single_records_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1473_from_rdataframe.py` & `awkward-2.1.3/tests/test_1473_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1477_generator_entry_type_as_rvec.py` & `awkward-2.1.3/tests/test_1477_generator_entry_type_as_rvec.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1490_jax_reducers_combinations.py` & `awkward-2.1.3/tests/test_1490_jax_reducers_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1502_getitem_jagged_issue1406.py` & `awkward-2.1.3/tests/test_1502_getitem_jagged_issue1406.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1504_typetracer_like.py` & `awkward-2.1.3/tests/test_1504_typetracer_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1508_awkward_from_rdataframe.py` & `awkward-2.1.3/tests/test_1508_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1511_set_attribute.py` & `awkward-2.1.3/tests/test_1511_set_attribute.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1539_isnone_axis_check_issue1417.py` & `awkward-2.1.3/tests/test_1539_isnone_axis_check_issue1417.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1559_fix_ufuncs_records_1439.py` & `awkward-2.1.3/tests/test_1559_fix_ufuncs_records_1439.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1565_axis_wrap_if_negative_record.py` & `awkward-2.1.3/tests/test_1565_axis_wrap_if_negative_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1567_fix_longlong_in_Index.py` & `awkward-2.1.3/tests/test_1567_fix_longlong_in_Index.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,13 +25,13 @@
     ]
 
 
 def test_typetracer_view_method():
     a = np.asarray([0, 1, 2, 3, 4, 5, 6, 7, 8, 9], dtype=np.longlong)
     b = ak.contents.NumpyArray(a)
     c = np.array([7, 3, 3, 5], dtype=np.longlong)
-    e = ak.index.Index(b.to_typetracer()[c])
+    e = ak.index.Index(b.to_typetracer()[c].data)
     f = ak.index.Index(a)
 
     assert e.form == f.form
     assert ak.to_list(b[c]) == ak.to_list(a[c])
     assert b.to_typetracer()[c].form == b[c].form
```

### Comparing `awkward-2.1.2/tests/test_1568_fix_lengths_empty_regular_slices.py` & `awkward-2.1.3/tests/test_1568_fix_lengths_empty_regular_slices.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1586_concatenate_should_preserve_regulararray.py` & `awkward-2.1.3/tests/test_1586_concatenate_should_preserve_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1604_preserve_form_in_concatenate.py` & `awkward-2.1.3/tests/test_1604_preserve_form_in_concatenate.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1607_no_reducers_on_records.py` & `awkward-2.1.3/tests/test_1607_no_reducers_on_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1613_generator_tolayout_records.py` & `awkward-2.1.3/tests/test_1613_generator_tolayout_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1619_from_parquet_empty_field.py` & `awkward-2.1.3/tests/test_1619_from_parquet_empty_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1620_layout_builders.py` & `awkward-2.1.3/tests/test_1620_layout_builders.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1625_multiple_columns_from_rdataframe.py` & `awkward-2.1.3/tests/test_1625_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1642_from_iter_of_tuples.py` & `awkward-2.1.3/tests/test_1642_from_iter_of_tuples.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1650_Record_to_list_should_listify_itself.py` & `awkward-2.1.3/tests/test_1650_Record_to_list_should_listify_itself.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1671_categorical_type.py` & `awkward-2.1.3/tests/test_1671_categorical_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1672_broadcast_parameters.py` & `awkward-2.1.3/tests/test_1672_broadcast_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1677_array_builder_in_numba.py` & `awkward-2.1.3/tests/test_1677_array_builder_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1685_IndexedArray_project_parameters.py` & `awkward-2.1.3/tests/test_1685_IndexedArray_project_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1686_UnionArray_simplified_preserve_parameters.py` & `awkward-2.1.3/tests/test_1686_UnionArray_simplified_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1688_pack_categorical.py` & `awkward-2.1.3/tests/test_1688_pack_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1703_fill_none_typetracer.py` & `awkward-2.1.3/tests/test_1703_fill_none_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1707_broadcast_parameters_ufunc.py` & `awkward-2.1.3/tests/test_1707_broadcast_parameters_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1709_ak_array_constructor_behavior.py` & `awkward-2.1.3/tests/test_1709_ak_array_constructor_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1747_bytemaskedarray_mergemany.py` & `awkward-2.1.3/tests/test_1747_bytemaskedarray_mergemany.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1753_indexedarray_merge_kernel.py` & `awkward-2.1.3/tests/test_1753_indexedarray_merge_kernel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1762_jax_behavior_support.py` & `awkward-2.1.3/tests/test_1762_jax_behavior_support.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1764_jax_jacobian.py` & `awkward-2.1.3/tests/test_1764_jax_jacobian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1765_add_ioanas_test_of_to_arraylib.py` & `awkward-2.1.3/tests/test_1765_add_ioanas_test_of_to_arraylib.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1766_record_form_fields.py` & `awkward-2.1.3/tests/test_1766_record_form_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1781_rdataframe_snapshot.py` & `awkward-2.1.3/tests/test_1781_rdataframe_snapshot.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1784_reduce_leading_sublist.py` & `awkward-2.1.3/tests/test_1784_reduce_leading_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1790_reduce_regulararray.py` & `awkward-2.1.3/tests/test_1790_reduce_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1791_reduce_trailing_sublist.py` & `awkward-2.1.3/tests/test_1791_reduce_trailing_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1794_run_lengths_empty_sublist.py` & `awkward-2.1.3/tests/test_1794_run_lengths_empty_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1829_to_from_rdataframe_bool.py` & `awkward-2.1.3/tests/test_1829_to_from_rdataframe_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py` & `awkward-2.1.3/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1847_numpy_array_contiguous.py` & `awkward-2.1.3/tests/test_1847_numpy_array_contiguous.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1850_bytemasked_array_to_bytemaskedarray.py` & `awkward-2.1.3/tests/test_1850_bytemasked_array_to_bytemaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1867_pass_behavior_through_combinations.py` & `awkward-2.1.3/tests/test_1867_pass_behavior_through_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1904_drop_none.py` & `awkward-2.1.3/tests/test_1904_drop_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1914_improved_axis_to_posaxis.py` & `awkward-2.1.3/tests/test_1914_improved_axis_to_posaxis.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py` & `awkward-2.1.3/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1930_unflatten_counts_checks.py` & `awkward-2.1.3/tests/test_1930_unflatten_counts_checks.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1936_with_field_broadcasting.py` & `awkward-2.1.3/tests/test_1936_with_field_broadcasting.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1940_ak_backend.py` & `awkward-2.1.3/tests/test_1940_ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1943_regular_indexing.py` & `awkward-2.1.3/tests/test_1943_regular_indexing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1960_awkward_from_rdataframe.py` & `awkward-2.1.3/tests/test_1960_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_1961_ak_without_field.py` & `awkward-2.1.3/tests/test_1961_ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2020_reduce_axis_none.py` & `awkward-2.1.3/tests/test_2020_reduce_axis_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2021_check_TypeTracerArray_in_ak_where.py` & `awkward-2.1.3/tests/test_2021_check_TypeTracerArray_in_ak_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2023_from_rdataframe.py` & `awkward-2.1.3/tests/test_2023_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py` & `awkward-2.1.3/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2047_ak_transform_regular_to_jagged.py` & `awkward-2.1.3/tests/test_2047_ak_transform_regular_to_jagged.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2055_array_builder_check.py` & `awkward-2.1.3/tests/test_2055_array_builder_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2058_merge_numpy_array.py` & `awkward-2.1.3/tests/test_2058_merge_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2064_fill_none_record.py` & `awkward-2.1.3/tests/test_2064_fill_none_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2067_to_buffers_byteorder.py` & `awkward-2.1.3/tests/test_2067_to_buffers_byteorder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2070_to_layout_string.py` & `awkward-2.1.3/tests/test_2070_to_layout_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2071_unflatten_non_packed_counts.py` & `awkward-2.1.3/tests/test_2071_unflatten_non_packed_counts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2078_array_function_wrap.py` & `awkward-2.1.3/tests/test_2078_array_function_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2082_broadcast_zero_size.py` & `awkward-2.1.3/tests/test_2082_broadcast_zero_size.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2096_ak_scalar_type.py` & `awkward-2.1.3/tests/test_2096_ak_scalar_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2101_pickle_behavior_class.py` & `awkward-2.1.3/tests/test_2101_pickle_behavior_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2104_numpy_merge_option.py` & `awkward-2.1.3/tests/test_2104_numpy_merge_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2106_pickle_class.py` & `awkward-2.1.3/tests/test_2106_pickle_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2108_fill_none_indexed.py` & `awkward-2.1.3/tests/test_2108_fill_none_indexed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2115_fix_up_typetracers.py` & `awkward-2.1.3/tests/test_2115_fix_up_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2125_type_of_scalar.py` & `awkward-2.1.3/tests/test_2125_type_of_scalar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2150_typetracer_high_level_ufunc.py` & `awkward-2.1.3/tests/test_2150_typetracer_high_level_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2179_parameter_merging_rules.py` & `awkward-2.1.3/tests/test_2179_parameter_merging_rules.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2185_merge_union_of_records.py` & `awkward-2.1.3/tests/test_2185_merge_union_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py` & `awkward-2.1.3/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2198_almost_equal.py` & `awkward-2.1.3/tests/test_2198_almost_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2202_filter_multiple_columns_from_rdataframe.py` & `awkward-2.1.3/tests/test_2202_filter_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2214_offset_bool_index.py` & `awkward-2.1.3/tests/test_2214_offset_bool_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2226_slice_regulararray_typetracer.py` & `awkward-2.1.3/tests/test_2226_slice_regulararray_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2229_getitem_range_slice.py` & `awkward-2.1.3/tests/test_2229_getitem_range_slice.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2234_from_rdataframe_keep_order.py` & `awkward-2.1.3/tests/test_2234_from_rdataframe_keep_order.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2236_merge_union_of_records_option.py` & `awkward-2.1.3/tests/test_2236_merge_union_of_records_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2240_simplify_merge_as_union.py` & `awkward-2.1.3/tests/test_2240_simplify_merge_as_union.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2246_slice_not_packed.py` & `awkward-2.1.3/tests/test_2246_slice_not_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2250_full_like_bool.py` & `awkward-2.1.3/tests/test_2250_full_like_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2258_from_rdataframe_with_arguments.py` & `awkward-2.1.3/tests/test_2258_from_rdataframe_with_arguments.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2263_to_packed_list.py` & `awkward-2.1.3/tests/test_2263_to_packed_list.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import numpy as np
 import pytest  # noqa: F401
 
 import awkward as ak
-from awkward._backends import TypeTracerBackend
+from awkward._backends.typetracer import TypeTracerBackend
 
 
 def test():
     backend = TypeTracerBackend.instance()
     layout = ak.contents.ListOffsetArray(
         ak.index.Index64(
             backend.index_nplike.asarray([0, 1, 3, 7], dtype=np.dtype("int64"))
```

### Comparing `awkward-2.1.2/tests/test_2266_fix_nan_to_num.py` & `awkward-2.1.3/tests/test_2266_fix_nan_to_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2267_broadcast_fields.py` & `awkward-2.1.3/tests/test_2267_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2293_unflatten_typetracer.py` & `awkward-2.1.3/tests/test_2293_unflatten_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2297_common_backend.py` & `awkward-2.1.3/tests/test_2297_common_backend.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,68 +10,68 @@
 left = ak.Array([1, 2, 3], backend="jax")
 right = ak.Array([100, 200, 300.0], backend="cpu")
 typetracer = ak.Array([44, 55, 66], backend="typetracer")
 
 
 def test_concatenate():
     with pytest.raises(
-        ValueError, match="cannot operate on arrays with incompatible array libraries"
+        ValueError, match="cannot operate on arrays with incompatible backends"
     ):
         ak.concatenate((left, right))
 
     result = ak.concatenate((left, typetracer))
     assert ak.backend(result) == "typetracer"
 
 
 def test_broadcast_arrays():
     with pytest.raises(
-        ValueError, match="cannot operate on arrays with incompatible array libraries"
+        ValueError, match="cannot operate on arrays with incompatible backends"
     ):
         ak.broadcast_arrays(left, right)
 
     result = ak.broadcast_arrays(left, typetracer)
     assert all(ak.backend(x) == "typetracer" for x in result)
 
 
 def test_broadcast_fields():
     with pytest.raises(
-        ValueError, match="cannot operate on arrays with incompatible array libraries"
+        ValueError, match="cannot operate on arrays with incompatible backends"
     ):
         ak.broadcast_fields(left, right)
 
     result = ak.broadcast_fields(left, typetracer)
     assert all(ak.backend(x) == "typetracer" for x in result)
 
 
 def test_cartesian():
     with pytest.raises(
-        ValueError, match="cannot operate on arrays with incompatible array libraries"
+        ValueError, match="cannot operate on arrays with incompatible backends"
     ):
         ak.cartesian((left, right), axis=0)
 
     result = ak.cartesian((left, typetracer), axis=0)
     assert ak.backend(result) == "typetracer"
 
 
 def test_to_rdataframe():
     pytest.importorskip("ROOT")
     array = ak.Array([100, 200, 300.0], backend="typetracer")
     with pytest.raises(
         TypeError,
-        match="Converting a TypeTracer nplike to an nplike with `known_data=True`",
+        match="from an nplike without known data to an nplike with known data",
     ):
         ak.to_rdataframe({"array": array})
 
 
 def test_transform():
     def apply(layouts, backend, **kwargs):
         if not all(x.is_numpy for x in layouts):
             return
         return tuple(x.copy(data=backend.nplike.asarray(x) * 2) for x in layouts)
 
     with pytest.raises(
-        ValueError, match="cannot operate on arrays with incompatible array libraries"
+        ValueError, match="cannot operate on arrays with incompatible backends"
     ):
         ak.transform(apply, left, right)
 
     result = ak.transform(apply, left, typetracer)
     assert all(ak.backend(x) == "typetracer" for x in result)
```

### Comparing `awkward-2.1.2/tests/test_2306_cppyy_git.py` & `awkward-2.1.3/tests/test_2306_cppyy_git.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2319_from_buffers_array.py` & `awkward-2.1.3/tests/test_2319_from_buffers_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2329_cartesian_broadcasting_fixes.py` & `awkward-2.1.3/tests/test_2329_cartesian_broadcasting_fixes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2349_growablebuffer_in_numba.py` & `awkward-2.1.3/tests/test_2349_growablebuffer_in_numba.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     assert growablebuffer.snapshot().tolist() == list(range(1000))
     assert len(growablebuffer._panels) == 51
 
 
 def test_unbox():
     @numba.njit
     def f1(x):
-        x
+        x  # noqa: B018 (we want to test the unboxing)
         return 3.14
 
     growablebuffer = GrowableBuffer(np.int32)
     f1(growablebuffer)
 
 
 def test_box():
```

### Comparing `awkward-2.1.2/tests/test_2354_ufunc_same_backend.py` & `awkward-2.1.3/tests/test_2354_ufunc_same_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2355_to_backend_record.py` & `awkward-2.1.3/tests/test_2355_to_backend_record.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import numpy as np  # noqa: F401
 import pytest
 
 import awkward as ak
-from awkward._backends import NumpyBackend, TypeTracerBackend
+from awkward._backends.numpy import NumpyBackend
+from awkward._backends.typetracer import TypeTracerBackend
 
 
 def test():
     layout = ak.to_layout({"x": 1, "y": 1})
     assert ak.backend(layout) == "cpu"
     assert layout.backend is NumpyBackend.instance()
```

### Comparing `awkward-2.1.2/tests/test_2361_typetracer_asarray_nd.py` & `awkward-2.1.3/tests/test_2361_typetracer_asarray_nd.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2368_type_is_equal.py` & `awkward-2.1.3/tests/test_2368_type_is_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2373_unzip_touching.py` & `awkward-2.1.3/tests/test_2373_unzip_touching.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/test_2374_cartesian_touching.py` & `awkward-2.1.3/tests/test_2374_cartesian_touching.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/list-depths-records-list.parquet` & `awkward-2.1.3/tests/samples/list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/list-depths-records.parquet` & `awkward-2.1.3/tests/samples/list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/list-depths-strings.parquet` & `awkward-2.1.3/tests/samples/list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/list-depths.parquet` & `awkward-2.1.3/tests/samples/list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/nonnullable-depths.parquet` & `awkward-2.1.3/tests/samples/nonnullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/nullable-depths.parquet` & `awkward-2.1.3/tests/samples/nullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/nullable-levels.parquet` & `awkward-2.1.3/tests/samples/nullable-levels.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/nullable-list-depths-records-list.parquet` & `awkward-2.1.3/tests/samples/nullable-list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/nullable-list-depths-records.parquet` & `awkward-2.1.3/tests/samples/nullable-list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/nullable-list-depths-strings.parquet` & `awkward-2.1.3/tests/samples/nullable-list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/nullable-list-depths.parquet` & `awkward-2.1.3/tests/samples/nullable-list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/nullable-record-primitives.parquet` & `awkward-2.1.3/tests/samples/nullable-record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/record-primitives.parquet` & `awkward-2.1.3/tests/samples/record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/test-nan-inf.json` & `awkward-2.1.3/tests/samples/test-nan-inf.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/test-two-arrays.json` & `awkward-2.1.3/tests/samples/test-two-arrays.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests/samples/test.json` & `awkward-2.1.3/tests/samples/test.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests-cuda/test_1276_cuda_num.py` & `awkward-2.1.3/tests-cuda/test_1276_cuda_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests-cuda/test_1276_cuda_transfers.py` & `awkward-2.1.3/tests-cuda/test_1276_cuda_transfers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests-cuda/test_1276_cupy_interop.py` & `awkward-2.1.3/tests-cuda/test_1276_cupy_interop.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests-cuda/test_1276_from_cupy.py` & `awkward-2.1.3/tests-cuda/test_1276_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests-cuda/test_1300_same_for_numba_cuda.py` & `awkward-2.1.3/tests-cuda/test_1300_same_for_numba_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests-cuda/test_1381_check_errors.py` & `awkward-2.1.3/tests-cuda/test_1381_check_errors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/tests-cuda/test_1809_array_cuda_jit.py` & `awkward-2.1.3/tests-cuda/test_1809_array_cuda_jit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/.gitignore` & `awkward-2.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/LICENSE` & `awkward-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `awkward-2.1.2/pyproject.toml` & `awkward-2.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "hatchling>=1.10.0",
     "hatch-fancy-pypi-readme"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "awkward"
-version = "2.1.2"
+version = "2.1.3"
 description = "Manipulate JSON-like data with NumPy-like idioms."
 license = { text = "BSD-3-Clause" }
 requires-python = ">=3.7"
 authors = [
     { name = "Jim Pivarski", email = "pivarski@princeton.edu" },
 ]
 classifiers = [
@@ -36,15 +36,15 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development",
     "Topic :: Utilities",
 ]
 dependencies = [
-    "awkward_cpp==13",
+    "awkward_cpp==14",
     "importlib_resources;python_version < \"3.9\"",
     "numpy>=1.17.0",
     "packaging",
     "typing_extensions>=4.1.0; python_version < \"3.11\""
 ]
 dynamic = [
     "readme"
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 [build-system] requires = [ "hatchling>=1.10.0", "hatch-fancy-pypi-readme" ]
-build-backend = "hatchling.build" [project] name = "awkward" version = "2.1.2"
+build-backend = "hatchling.build" [project] name = "awkward" version = "2.1.3"
 description = "Manipulate JSON-like data with NumPy-like idioms." license =
 { text = "BSD-3-Clause" } requires-python = ">=3.7" authors = [ { name = "Jim
 Pivarski", email = "pivarski@princeton.edu" }, ] classifiers = [ "Development
 Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Intended
 Audience :: Information Technology", "Intended Audience :: Science/Research",
 "License :: OSI Approved :: BSD License", "Operating System :: MacOS :: MacOS
 X", "Operating System :: Microsoft :: Windows", "Operating System :: POSIX ::
@@ -11,15 +11,15 @@
 "Programming Language :: Python :: 3", "Programming Language :: Python :: 3 ::
 Only", "Programming Language :: Python :: 3.7", "Programming Language :: Python
 :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language ::
 Python :: 3.10", "Programming Language :: Python :: 3.11", "Topic ::
 Scientific/Engineering", "Topic :: Scientific/Engineering :: Information
 Analysis", "Topic :: Scientific/Engineering :: Mathematics", "Topic ::
 Scientific/Engineering :: Physics", "Topic :: Software Development", "Topic ::
-Utilities", ] dependencies = [ "awkward_cpp==13",
+Utilities", ] dependencies = [ "awkward_cpp==14",
 "importlib_resources;python_version < \"3.9\"", "numpy>=1.17.0", "packaging",
 "typing_extensions>=4.1.0; python_version < \"3.11\"" ] dynamic = [ "readme" ]
 [project.entry-points.numba_extensions] init = "awkward.numba:_register"
 [project.urls] "Bug Tracker" = "https://github.com/scikit-hep/awkward-1.0/
 issues" "Chat" = "https://gitter.im/Scikit-HEP/awkward-array" "Discussions" =
 "https://github.com/scikit-hep/awkward-1.0/discussions" "Documentation" =
 "https://awkward-array.org" "Homepage" = "https://github.com/scikit-hep/
```

### Comparing `awkward-2.1.2/PKG-INFO` & `awkward-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awkward
-Version: 2.1.2
+Version: 2.1.3
 Summary: Manipulate JSON-like data with NumPy-like idioms.
 Project-URL: Bug Tracker, https://github.com/scikit-hep/awkward-1.0/issues
 Project-URL: Chat, https://gitter.im/Scikit-HEP/awkward-array
 Project-URL: Discussions, https://github.com/scikit-hep/awkward-1.0/discussions
 Project-URL: Documentation, https://awkward-array.org
 Project-URL: Homepage, https://github.com/scikit-hep/awkward-1.0
 Project-URL: Releases, https://github.com/scikit-hep/awkward-1.0/releases
@@ -32,15 +32,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Requires-Dist: awkward-cpp==13
+Requires-Dist: awkward-cpp==14
 Requires-Dist: importlib-resources; python_version < '3.9'
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: packaging
 Requires-Dist: typing-extensions>=4.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/scikit-hep/awkward-1.0">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: awkward Version: 2.1.2 Summary: Manipulate JSON-
+Metadata-Version: 2.1 Name: awkward Version: 2.1.3 Summary: Manipulate JSON-
 like data with NumPy-like idioms. Project-URL: Bug Tracker, https://github.com/
 scikit-hep/awkward-1.0/issues Project-URL: Chat, https://gitter.im/Scikit-HEP/
 awkward-array Project-URL: Discussions, https://github.com/scikit-hep/awkward-
 1.0/discussions Project-URL: Documentation, https://awkward-array.org Project-
 URL: Homepage, https://github.com/scikit-hep/awkward-1.0 Project-URL: Releases,
 https://github.com/scikit-hep/awkward-1.0/releases Project-URL: Source Code,
 https://github.com/scikit-hep/awkward-1.0 Author-email: Jim Pivarski
@@ -18,15 +18,15 @@
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics Classifier: Topic ::
 Software Development Classifier: Topic :: Utilities Requires-Python: >=3.7
-Requires-Dist: awkward-cpp==13 Requires-Dist: importlib-resources;
+Requires-Dist: awkward-cpp==14 Requires-Dist: importlib-resources;
 python_version < '3.9' Requires-Dist: numpy>=1.17.0 Requires-Dist: packaging
 Requires-Dist: typing-extensions>=4.1.0; python_version < '3.11' Description-
 Content-Type: text/markdown [https://github.com/scikit-hep/awkward-1.0/raw/
 main/docs-img/logo/logo-300px.png] [![PyPI version](https://badge.fury.io/py/
 awkward.svg)](https://pypi.org/project/awkward) [![Conda-Forge](https://
 img.shields.io/conda/vn/conda-forge/awkward)](https://github.com/conda-forge/
 awkward-feedstock) [![Python 3.7â3.11](https://img.shields.io/badge/python-
```

