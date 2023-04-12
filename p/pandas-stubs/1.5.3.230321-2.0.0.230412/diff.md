# Comparing `tmp/pandas_stubs-1.5.3.230321.tar.gz` & `tmp/pandas_stubs-2.0.0.230412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_stubs-1.5.3.230321.tar", max compression
+gzip compressed data, was "pandas_stubs-2.0.0.230412.tar", max compression
```

## Comparing `pandas_stubs-1.5.3.230321.tar` & `pandas_stubs-2.0.0.230412.tar`

### file list

```diff
@@ -1,206 +1,205 @@
--rw-r--r--   0        0        0     1514 2022-08-08 01:00:32.131878 pandas_stubs-1.5.3.230321/LICENSE
--rw-r--r--   0        0        0     3816 2022-12-28 15:28:49.654657 pandas_stubs-1.5.3.230321/pandas-stubs/__init__.pyi
--rw-r--r--   0        0        0      220 2022-08-08 01:00:32.243006 pandas_stubs-1.5.3.230321/pandas-stubs/_config/__init__.pyi
--rw-r--r--   0        0        0     4145 2023-02-26 16:00:15.410944 pandas_stubs-1.5.3.230321/pandas-stubs/_config/config.pyi
--rw-r--r--   0        0        0      251 2022-08-08 01:00:32.265011 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/__init__.pyi
--rw-r--r--   0        0        0      132 2022-08-08 01:00:32.278047 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/indexing.pyi
--rw-r--r--   0        0        0     8318 2023-02-23 17:31:11.760589 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/interval.pyi
--rw-r--r--   0        0        0      130 2022-08-08 01:00:32.293998 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/json.pyi
--rw-r--r--   0        0        0      866 2023-02-27 22:18:36.850339 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/lib.pyi
--rw-r--r--   0        0        0     1893 2023-02-23 17:31:11.761589 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/missing.pyi
--rw-r--r--   0        0        0      126 2022-08-08 01:00:32.310002 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/ops_dispatch.pyi
--rw-r--r--   0        0        0      421 2023-02-04 17:09:12.289425 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/properties.pyi
--rw-r--r--   0        0        0       91 2022-08-08 01:00:32.320997 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/sparse.pyi
--rw-r--r--   0        0        0      573 2022-12-28 15:28:49.657656 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/__init__.pyi
--rw-r--r--   0        0        0       65 2022-08-08 01:00:32.332997 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/base.pyi
--rw-r--r--   0        0        0      143 2022-08-08 01:00:32.346996 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/conversion.pyi
--rw-r--r--   0        0        0     1195 2022-08-10 19:03:04.643581 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/dtypes.pyi
--rw-r--r--   0        0        0     3543 2023-02-23 17:31:11.762588 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/nattype.pyi
--rw-r--r--   0        0        0       89 2022-12-28 15:28:49.658657 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/np_datetime.pyi
--rw-r--r--   0        0        0     8230 2023-02-23 17:31:11.763588 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/offsets.pyi
--rw-r--r--   0        0        0      163 2022-08-08 01:00:32.387997 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/parsing.pyi
--rw-r--r--   0        0        0     6525 2023-02-23 17:31:11.764590 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/period.pyi
--rw-r--r--   0        0        0       72 2022-08-08 01:00:32.405128 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/strptime.pyi
--rw-r--r--   0        0        0    13987 2023-02-23 17:31:11.765598 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/timedeltas.pyi
--rw-r--r--   0        0        0    10731 2023-02-23 17:31:11.766587 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/timestamps.pyi
--rw-r--r--   0        0        0       62 2022-08-08 01:00:32.438009 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/tzconversion.pyi
--rw-r--r--   0        0        0      613 2023-02-04 17:09:12.293389 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/vectorized.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.574585 pandas_stubs-1.5.3.230321/pandas-stubs/_libs/window/__init__.pyi
--rw-r--r--   0        0        0     4126 2023-02-04 17:09:12.293389 pandas_stubs-1.5.3.230321/pandas-stubs/_testing/__init__.pyi
--rw-r--r--   0        0        0    15120 2023-03-13 15:04:46.616677 pandas_stubs-1.5.3.230321/pandas-stubs/_typing.pyi
--rw-r--r--   0        0        0      124 2023-03-21 14:28:40.804192 pandas_stubs-1.5.3.230321/pandas-stubs/_version.pyi
--rw-r--r--   0        0        0       94 2022-08-08 01:00:32.471998 pandas_stubs-1.5.3.230321/pandas-stubs/api/__init__.pyi
--rw-r--r--   0        0        0      603 2023-02-27 22:18:36.851320 pandas_stubs-1.5.3.230321/pandas-stubs/api/extensions/__init__.pyi
--rw-r--r--   0        0        0      241 2022-08-08 01:00:32.486031 pandas_stubs-1.5.3.230321/pandas-stubs/api/indexers/__init__.pyi
--rw-r--r--   0        0        0      164 2022-12-28 15:28:49.664655 pandas_stubs-1.5.3.230321/pandas-stubs/api/interchange/__init__.pyi
--rw-r--r--   0        0        0     1959 2022-12-28 15:28:49.665655 pandas_stubs-1.5.3.230321/pandas-stubs/api/types/__init__.pyi
--rw-r--r--   0        0        0      373 2022-08-08 01:00:32.499997 pandas_stubs-1.5.3.230321/pandas-stubs/arrays/__init__.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.550503 pandas_stubs-1.5.3.230321/pandas-stubs/core/__init__.pyi
--rw-r--r--   0        0        0      471 2022-08-08 01:00:32.505997 pandas_stubs-1.5.3.230321/pandas-stubs/core/accessor.pyi
--rw-r--r--   0        0        0     2295 2023-03-04 20:30:27.571571 pandas_stubs-1.5.3.230321/pandas-stubs/core/algorithms.pyi
--rw-r--r--   0        0        0     2779 2022-12-28 15:28:49.666655 pandas_stubs-1.5.3.230321/pandas-stubs/core/api.pyi
--rw-r--r--   0        0        0     1846 2023-02-27 22:18:36.852304 pandas_stubs-1.5.3.230321/pandas-stubs/core/arraylike.pyi
--rw-r--r--   0        0        0      726 2022-08-10 19:03:04.648579 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/__init__.pyi
--rw-r--r--   0        0        0      321 2023-02-27 03:32:24.825818 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/arrow/dtype.pyi
--rw-r--r--   0        0        0     2133 2023-02-27 22:18:36.853367 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/base.pyi
--rw-r--r--   0        0        0      954 2023-02-27 22:18:36.854305 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/boolean.pyi
--rw-r--r--   0        0        0     7407 2023-02-27 22:18:36.855305 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/categorical.pyi
--rw-r--r--   0        0        0     2841 2023-02-27 22:18:36.855305 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/datetimelike.pyi
--rw-r--r--   0        0        0     2216 2022-12-28 15:28:49.669665 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/datetimes.pyi
--rw-r--r--   0        0        0      133 2022-12-28 15:28:49.670655 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/floating.pyi
--rw-r--r--   0        0        0     1010 2023-02-27 03:32:24.827813 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/integer.pyi
--rw-r--r--   0        0        0     2428 2023-02-27 22:18:36.856321 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/interval.pyi
--rw-r--r--   0        0        0      964 2023-02-27 22:18:36.857336 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/masked.pyi
--rw-r--r--   0        0        0       99 2023-02-27 03:32:24.828808 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/numeric.pyi
--rw-r--r--   0        0        0      513 2023-02-27 03:32:24.828808 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/numpy_.pyi
--rw-r--r--   0        0        0     1661 2023-02-04 17:09:12.300387 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/period.pyi
--rw-r--r--   0        0        0      210 2022-12-28 15:28:49.674654 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/sparse/__init__.pyi
--rw-r--r--   0        0        0      613 2022-12-28 15:28:49.674654 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/sparse/accessor.pyi
--rw-r--r--   0        0        0     2309 2023-02-27 22:18:36.857336 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/sparse/array.pyi
--rw-r--r--   0        0        0      448 2023-02-27 03:32:24.829807 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/sparse/dtype.pyi
--rw-r--r--   0        0        0      715 2023-02-27 03:32:24.830807 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/string_.pyi
--rw-r--r--   0        0        0     1963 2023-02-04 17:09:12.301416 pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/timedeltas.pyi
--rw-r--r--   0        0        0     2685 2023-03-04 20:30:27.571571 pandas_stubs-1.5.3.230321/pandas-stubs/core/base.pyi
--rw-r--r--   0        0        0      955 2023-02-04 17:09:12.302429 pandas_stubs-1.5.3.230321/pandas-stubs/core/common.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.561504 pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/__init__.pyi
--rw-r--r--   0        0        0       79 2022-08-08 01:00:32.662463 pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/align.pyi
--rw-r--r--   0        0        0       54 2022-08-08 01:00:32.670999 pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/api.pyi
--rw-r--r--   0        0        0       47 2022-08-10 19:03:04.655579 pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/common.pyi
--rw-r--r--   0        0        0      438 2022-12-28 15:28:49.678655 pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/engines.pyi
--rw-r--r--   0        0        0      668 2023-02-04 17:09:12.302429 pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/eval.pyi
--rw-r--r--   0        0        0     2265 2022-08-08 01:00:32.699007 pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/expr.pyi
--rw-r--r--   0        0        0      270 2022-08-08 01:00:32.711086 pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/expressions.pyi
--rw-r--r--   0        0        0     2324 2022-08-08 01:00:32.722048 pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/ops.pyi
--rw-r--r--   0        0        0      487 2023-02-04 17:09:12.303395 pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/parsing.pyi
--rw-r--r--   0        0        0     3061 2022-08-08 01:00:32.745044 pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/pytables.pyi
--rw-r--r--   0        0        0      645 2022-08-08 01:00:32.755711 pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/scope.pyi
--rw-r--r--   0        0        0     1621 2022-08-08 01:00:32.764271 pandas_stubs-1.5.3.230321/pandas-stubs/core/config_init.pyi
--rw-r--r--   0        0        0      935 2023-02-04 17:09:12.303395 pandas_stubs-1.5.3.230321/pandas-stubs/core/construction.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.565503 pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/__init__.pyi
--rw-r--r--   0        0        0     1625 2022-12-28 15:28:49.680655 pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/api.pyi
--rw-r--r--   0        0        0      834 2023-02-27 22:18:36.858307 pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/base.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.681655 pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/cast.pyi
--rw-r--r--   0        0        0     2377 2023-02-23 17:31:11.770587 pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/common.pyi
--rw-r--r--   0        0        0      308 2023-02-23 17:31:11.771588 pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/concat.pyi
--rw-r--r--   0        0        0     1687 2023-02-27 22:18:36.858307 pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/dtypes.pyi
--rw-r--r--   0        0        0      207 2022-12-28 15:28:49.683657 pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/generic.pyi
--rw-r--r--   0        0        0      610 2022-12-28 15:28:49.684666 pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/inference.pyi
--rw-r--r--   0        0        0     1027 2022-12-28 15:28:49.684666 pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/missing.pyi
--rw-r--r--   0        0        0    64211 2023-03-20 22:45:34.798554 pandas_stubs-1.5.3.230321/pandas-stubs/core/frame.pyi
--rw-r--r--   0        0        0    15001 2023-03-13 15:04:46.619676 pandas_stubs-1.5.3.230321/pandas-stubs/core/generic.pyi
--rw-r--r--   0        0        0      120 2022-08-08 01:00:32.927699 pandas_stubs-1.5.3.230321/pandas-stubs/core/groupby/__init__.pyi
--rw-r--r--   0        0        0      261 2023-02-04 17:09:12.306444 pandas_stubs-1.5.3.230321/pandas-stubs/core/groupby/base.pyi
--rw-r--r--   0        0        0      246 2022-08-10 19:03:04.661580 pandas_stubs-1.5.3.230321/pandas-stubs/core/groupby/categorical.pyi
--rw-r--r--   0        0        0    12835 2023-03-04 20:30:27.574572 pandas_stubs-1.5.3.230321/pandas-stubs/core/groupby/generic.pyi
--rw-r--r--   0        0        0     4139 2023-03-04 20:30:27.574572 pandas_stubs-1.5.3.230321/pandas-stubs/core/groupby/groupby.pyi
--rw-r--r--   0        0        0     1647 2023-02-04 17:09:12.308388 pandas_stubs-1.5.3.230321/pandas-stubs/core/groupby/grouper.pyi
--rw-r--r--   0        0        0     2721 2023-02-04 17:09:12.308388 pandas_stubs-1.5.3.230321/pandas-stubs/core/groupby/ops.pyi
--rw-r--r--   0        0        0     1673 2022-08-10 19:03:04.663578 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexers.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.575505 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/__init__.pyi
--rw-r--r--   0        0        0    12910 2023-02-23 17:31:11.775601 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/accessors.pyi
--rw-r--r--   0        0        0      928 2022-08-10 19:03:04.664580 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/api.pyi
--rw-r--r--   0        0        0     8965 2023-02-23 17:31:11.776589 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/base.pyi
--rw-r--r--   0        0        0     1741 2023-02-23 17:31:11.776589 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/category.pyi
--rw-r--r--   0        0        0      812 2023-02-23 17:31:11.777589 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/datetimelike.pyi
--rw-r--r--   0        0        0     4407 2023-02-23 17:31:11.778625 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/datetimes.pyi
--rw-r--r--   0        0        0       80 2023-02-23 17:31:11.778625 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/extension.pyi
--rw-r--r--   0        0        0      429 2022-08-08 01:00:33.113434 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/frozen.pyi
--rw-r--r--   0        0        0    12977 2023-02-23 17:31:11.779587 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/interval.pyi
--rw-r--r--   0        0        0     5354 2023-02-23 17:31:11.780587 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/multi.pyi
--rw-r--r--   0        0        0     1759 2023-02-04 17:09:12.312423 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/numeric.pyi
--rw-r--r--   0        0        0     2933 2023-02-23 17:31:11.781588 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/period.pyi
--rw-r--r--   0        0        0     2868 2023-02-23 17:31:11.782590 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/range.pyi
--rw-r--r--   0        0        0     2713 2023-02-23 17:31:11.783587 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/timedeltas.pyi
--rw-r--r--   0        0        0     1849 2023-02-23 17:31:11.783587 pandas_stubs-1.5.3.230321/pandas-stubs/core/indexing.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.696655 pandas_stubs-1.5.3.230321/pandas-stubs/core/interchange/__init__.pyi
--rw-r--r--   0        0        0     3166 2023-02-04 17:09:12.315386 pandas_stubs-1.5.3.230321/pandas-stubs/core/interchange/dataframe_protocol.pyi
--rw-r--r--   0        0        0       92 2022-12-28 15:28:49.697655 pandas_stubs-1.5.3.230321/pandas-stubs/core/interchange/from_dataframe.pyi
--rw-r--r--   0        0        0      346 2022-12-28 15:28:49.698655 pandas_stubs-1.5.3.230321/pandas-stubs/core/missing.pyi
--rw-r--r--   0        0        0      211 2022-08-10 19:03:04.669578 pandas_stubs-1.5.3.230321/pandas-stubs/core/ops/__init__.pyi
--rw-r--r--   0        0        0      517 2022-08-10 19:03:04.669578 pandas_stubs-1.5.3.230321/pandas-stubs/core/ops/array_ops.pyi
--rw-r--r--   0        0        0       45 2022-08-08 01:00:33.245986 pandas_stubs-1.5.3.230321/pandas-stubs/core/ops/common.pyi
--rw-r--r--   0        0        0      120 2022-12-28 15:28:49.698655 pandas_stubs-1.5.3.230321/pandas-stubs/core/ops/dispatch.pyi
--rw-r--r--   0        0        0       17 2022-08-08 01:00:33.268029 pandas_stubs-1.5.3.230321/pandas-stubs/core/ops/docstrings.pyi
--rw-r--r--   0        0        0       81 2022-08-08 01:00:33.278086 pandas_stubs-1.5.3.230321/pandas-stubs/core/ops/invalid.pyi
--rw-r--r--   0        0        0      606 2022-08-08 01:00:33.289023 pandas_stubs-1.5.3.230321/pandas-stubs/core/ops/mask_ops.pyi
--rw-r--r--   0        0        0     6266 2023-03-04 20:30:27.575571 pandas_stubs-1.5.3.230321/pandas-stubs/core/resample.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.589504 pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/__init__.pyi
--rw-r--r--   0        0        0      633 2022-12-28 15:28:49.699654 pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/api.pyi
--rw-r--r--   0        0        0     2860 2023-03-04 20:30:27.576572 pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/concat.pyi
--rw-r--r--   0        0        0      716 2023-02-04 17:09:12.318387 pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/encoding.pyi
--rw-r--r--   0        0        0      741 2023-02-04 17:09:12.318387 pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/melt.pyi
--rw-r--r--   0        0        0     3089 2022-12-28 15:28:49.701655 pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/merge.pyi
--rw-r--r--   0        0        0     4113 2023-02-23 17:31:11.784589 pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/pivot.pyi
--rw-r--r--   0        0        0     7722 2023-02-23 17:31:11.785588 pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/tile.pyi
--rw-r--r--   0        0        0       30 2022-08-08 01:00:33.431568 pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/util.pyi
--rw-r--r--   0        0        0    61683 2023-03-14 13:29:20.772095 pandas_stubs-1.5.3.230321/pandas-stubs/core/series.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.591599 pandas_stubs-1.5.3.230321/pandas-stubs/core/sparse/__init__.pyi
--rw-r--r--   0        0        0     6667 2023-02-04 17:09:12.321425 pandas_stubs-1.5.3.230321/pandas-stubs/core/strings.pyi
--rw-r--r--   0        0        0        0 2022-08-10 19:03:04.672581 pandas_stubs-1.5.3.230321/pandas-stubs/core/tools/__init__.pyi
--rw-r--r--   0        0        0     2781 2023-02-23 17:31:11.787588 pandas_stubs-1.5.3.230321/pandas-stubs/core/tools/datetimes.pyi
--rw-r--r--   0        0        0      873 2023-02-23 17:31:11.787588 pandas_stubs-1.5.3.230321/pandas-stubs/core/tools/numeric.pyi
--rw-r--r--   0        0        0     1074 2023-02-04 17:09:12.322446 pandas_stubs-1.5.3.230321/pandas-stubs/core/tools/timedeltas.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.592587 pandas_stubs-1.5.3.230321/pandas-stubs/core/util/__init__.pyi
--rw-r--r--   0        0        0      480 2022-12-28 15:28:49.706655 pandas_stubs-1.5.3.230321/pandas-stubs/core/util/hashing.pyi
--rw-r--r--   0        0        0      274 2022-08-08 01:00:33.545825 pandas_stubs-1.5.3.230321/pandas-stubs/core/window/__init__.pyi
--rw-r--r--   0        0        0     2484 2022-12-28 15:28:49.706655 pandas_stubs-1.5.3.230321/pandas-stubs/core/window/ewm.pyi
--rw-r--r--   0        0        0     3838 2023-02-04 17:09:12.323425 pandas_stubs-1.5.3.230321/pandas-stubs/core/window/expanding.pyi
--rw-r--r--   0        0        0     5796 2023-02-04 17:09:12.324423 pandas_stubs-1.5.3.230321/pandas-stubs/core/window/rolling.pyi
--rw-r--r--   0        0        0     1808 2022-12-28 15:28:49.709656 pandas_stubs-1.5.3.230321/pandas-stubs/errors/__init__.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.599505 pandas_stubs-1.5.3.230321/pandas-stubs/io/__init__.pyi
--rw-r--r--   0        0        0     1132 2022-08-08 01:00:33.649500 pandas_stubs-1.5.3.230321/pandas-stubs/io/api.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.710655 pandas_stubs-1.5.3.230321/pandas-stubs/io/clipboard/__init__.pyi
--rw-r--r--   0        0        0     7254 2023-02-04 17:09:12.324423 pandas_stubs-1.5.3.230321/pandas-stubs/io/clipboards.pyi
--rw-r--r--   0        0        0      487 2022-12-28 15:28:49.711655 pandas_stubs-1.5.3.230321/pandas-stubs/io/common.pyi
--rw-r--r--   0        0        0      128 2022-08-08 01:00:33.708448 pandas_stubs-1.5.3.230321/pandas-stubs/io/excel/__init__.pyi
--rw-r--r--   0        0        0     7825 2023-02-23 17:31:11.788590 pandas_stubs-1.5.3.230321/pandas-stubs/io/excel/_base.pyi
--rw-r--r--   0        0        0       73 2022-08-08 01:00:33.734493 pandas_stubs-1.5.3.230321/pandas-stubs/io/excel/_util.pyi
--rw-r--r--   0        0        0      335 2022-08-29 12:14:24.788360 pandas_stubs-1.5.3.230321/pandas-stubs/io/feather_format.pyi
--rw-r--r--   0        0        0        0 2022-07-03 21:17:38.596585 pandas_stubs-1.5.3.230321/pandas-stubs/io/formats/__init__.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.712655 pandas_stubs-1.5.3.230321/pandas-stubs/io/formats/css.pyi
--rw-r--r--   0        0        0      338 2022-12-28 15:28:49.713678 pandas_stubs-1.5.3.230321/pandas-stubs/io/formats/format.pyi
--rw-r--r--   0        0        0    11408 2023-03-04 20:30:27.577572 pandas_stubs-1.5.3.230321/pandas-stubs/io/formats/style.pyi
--rw-r--r--   0        0        0     2436 2023-03-04 20:30:27.578572 pandas_stubs-1.5.3.230321/pandas-stubs/io/formats/style_render.pyi
--rw-r--r--   0        0        0      685 2022-08-20 01:19:02.005181 pandas_stubs-1.5.3.230321/pandas-stubs/io/gbq.pyi
--rw-r--r--   0        0        0     1382 2023-02-04 17:09:12.326429 pandas_stubs-1.5.3.230321/pandas-stubs/io/html.pyi
--rw-r--r--   0        0        0      170 2022-08-29 12:14:24.789359 pandas_stubs-1.5.3.230321/pandas-stubs/io/json/__init__.pyi
--rw-r--r--   0        0        0     4110 2023-02-04 17:09:12.327388 pandas_stubs-1.5.3.230321/pandas-stubs/io/json/_json.pyi
--rw-r--r--   0        0        0      403 2022-08-29 12:14:24.790358 pandas_stubs-1.5.3.230321/pandas-stubs/io/json/_normalize.pyi
--rw-r--r--   0        0        0      285 2022-08-29 12:14:24.790358 pandas_stubs-1.5.3.230321/pandas-stubs/io/json/_table_schema.pyi
--rw-r--r--   0        0        0      282 2022-08-29 12:14:24.791359 pandas_stubs-1.5.3.230321/pandas-stubs/io/orc.pyi
--rw-r--r--   0        0        0      421 2022-08-29 12:14:24.791359 pandas_stubs-1.5.3.230321/pandas-stubs/io/parquet.pyi
--rw-r--r--   0        0        0      168 2022-12-28 15:28:49.716655 pandas_stubs-1.5.3.230321/pandas-stubs/io/parsers/__init__.pyi
--rw-r--r--   0        0        0    16344 2023-02-23 17:31:11.790587 pandas_stubs-1.5.3.230321/pandas-stubs/io/parsers/readers.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.716655 pandas_stubs-1.5.3.230321/pandas-stubs/io/parsers.pyi
--rw-r--r--   0        0        0      558 2022-12-28 15:28:49.717656 pandas_stubs-1.5.3.230321/pandas-stubs/io/pickle.pyi
--rw-r--r--   0        0        0     6725 2023-02-23 17:31:11.791589 pandas_stubs-1.5.3.230321/pandas-stubs/io/pytables.pyi
--rw-r--r--   0        0        0       58 2022-08-29 12:14:24.793360 pandas_stubs-1.5.3.230321/pandas-stubs/io/sas/__init__.pyi
--rw-r--r--   0        0        0      256 2022-12-28 15:28:49.718670 pandas_stubs-1.5.3.230321/pandas-stubs/io/sas/sas7bdat.pyi
--rw-r--r--   0        0        0      250 2022-08-29 12:14:24.794359 pandas_stubs-1.5.3.230321/pandas-stubs/io/sas/sas_xport.pyi
--rw-r--r--   0        0        0     2976 2023-02-23 17:31:11.792588 pandas_stubs-1.5.3.230321/pandas-stubs/io/sas/sasreader.pyi
--rw-r--r--   0        0        0      250 2022-08-29 12:14:24.795362 pandas_stubs-1.5.3.230321/pandas-stubs/io/spss.pyi
--rw-r--r--   0        0        0     4871 2023-02-23 17:31:11.794588 pandas_stubs-1.5.3.230321/pandas-stubs/io/sql.pyi
--rw-r--r--   0        0        0     4334 2023-02-23 17:31:11.795592 pandas_stubs-1.5.3.230321/pandas-stubs/io/stata.pyi
--rw-r--r--   0        0        0     1015 2023-02-04 17:09:12.330386 pandas_stubs-1.5.3.230321/pandas-stubs/io/xml.pyi
--rw-r--r--   0        0        0      587 2022-12-28 15:28:49.720654 pandas_stubs-1.5.3.230321/pandas-stubs/plotting/__init__.pyi
--rw-r--r--   0        0        0    12852 2023-02-23 17:31:11.796591 pandas_stubs-1.5.3.230321/pandas-stubs/plotting/_core.pyi
--rw-r--r--   0        0        0     2360 2023-02-23 17:31:11.797589 pandas_stubs-1.5.3.230321/pandas-stubs/plotting/_misc.pyi
--rw-r--r--   0        0        0        0 2022-12-28 15:28:49.722656 pandas_stubs-1.5.3.230321/pandas-stubs/py.typed
--rw-r--r--   0        0        0      368 2022-08-08 01:00:34.094401 pandas_stubs-1.5.3.230321/pandas-stubs/testing.pyi
--rw-r--r--   0        0        0        0 2022-07-02 19:36:57.614504 pandas_stubs-1.5.3.230321/pandas-stubs/tseries/__init__.pyi
--rw-r--r--   0        0        0       64 2022-08-08 01:00:34.100409 pandas_stubs-1.5.3.230321/pandas-stubs/tseries/api.pyi
--rw-r--r--   0        0        0      378 2022-12-28 15:28:49.722656 pandas_stubs-1.5.3.230321/pandas-stubs/tseries/frequencies.pyi
--rw-r--r--   0        0        0      118 2022-08-29 12:14:32.889752 pandas_stubs-1.5.3.230321/pandas-stubs/tseries/holiday.pyi
--rw-r--r--   0        0        0     1312 2022-08-08 01:00:34.111525 pandas_stubs-1.5.3.230321/pandas-stubs/tseries/offsets.pyi
--rw-r--r--   0        0        0      255 2022-12-28 15:28:49.723655 pandas_stubs-1.5.3.230321/pandas-stubs/util/__init__.pyi
--rw-r--r--   0        0        0     1230 2023-02-04 17:09:12.332423 pandas_stubs-1.5.3.230321/pandas-stubs/util/_decorators.pyi
--rw-r--r--   0        0        0      279 2022-08-08 01:00:34.130416 pandas_stubs-1.5.3.230321/pandas-stubs/util/_doctools.pyi
--rw-r--r--   0        0        0       57 2022-08-08 01:00:34.135732 pandas_stubs-1.5.3.230321/pandas-stubs/util/_exceptions.pyi
--rw-r--r--   0        0        0       53 2022-12-28 15:28:49.723655 pandas_stubs-1.5.3.230321/pandas-stubs/util/_print_versions.pyi
--rw-r--r--   0        0        0       38 2022-08-08 01:00:34.153394 pandas_stubs-1.5.3.230321/pandas-stubs/util/_tester.pyi
--rw-r--r--   0        0        0      594 2023-02-04 17:09:12.332423 pandas_stubs-1.5.3.230321/pandas-stubs/util/_validators.pyi
--rw-r--r--   0        0        0     1899 2022-12-28 15:28:49.725656 pandas_stubs-1.5.3.230321/pandas-stubs/util/version/__init__.pyi
--rw-r--r--   0        0        0     6871 2023-03-21 14:27:51.956889 pandas_stubs-1.5.3.230321/pyproject.toml
--rw-r--r--   0        0        0     8173 2023-02-04 17:09:12.285386 pandas_stubs-1.5.3.230321/README.md
--rw-r--r--   0        0        0    10179 1970-01-01 00:00:00.000000 pandas_stubs-1.5.3.230321/setup.py
--rw-r--r--   0        0        0     9448 1970-01-01 00:00:00.000000 pandas_stubs-1.5.3.230321/PKG-INFO
+-rw-r--r--   0        0        0     1514 2022-08-08 01:00:32.131878 pandas_stubs-2.0.0.230412/LICENSE
+-rw-r--r--   0        0        0     3717 2023-04-05 02:20:38.238520 pandas_stubs-2.0.0.230412/pandas-stubs/__init__.pyi
+-rw-r--r--   0        0        0      220 2022-08-08 01:00:32.243006 pandas_stubs-2.0.0.230412/pandas-stubs/_config/__init__.pyi
+-rw-r--r--   0        0        0     4145 2023-02-26 16:00:15.410944 pandas_stubs-2.0.0.230412/pandas-stubs/_config/config.pyi
+-rw-r--r--   0        0        0      251 2022-08-08 01:00:32.265011 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/__init__.pyi
+-rw-r--r--   0        0        0      132 2022-08-08 01:00:32.278047 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/indexing.pyi
+-rw-r--r--   0        0        0     8318 2023-02-23 17:31:11.760589 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/interval.pyi
+-rw-r--r--   0        0        0      130 2022-08-08 01:00:32.293998 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/json.pyi
+-rw-r--r--   0        0        0      866 2023-02-27 22:18:36.850339 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/lib.pyi
+-rw-r--r--   0        0        0     1893 2023-02-23 17:31:11.761589 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/missing.pyi
+-rw-r--r--   0        0        0      126 2022-08-08 01:00:32.310002 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/ops_dispatch.pyi
+-rw-r--r--   0        0        0      421 2023-02-04 17:09:12.289425 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/properties.pyi
+-rw-r--r--   0        0        0       91 2022-08-08 01:00:32.320997 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/sparse.pyi
+-rw-r--r--   0        0        0      573 2022-12-28 15:28:49.657656 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/__init__.pyi
+-rw-r--r--   0        0        0       65 2022-08-08 01:00:32.332997 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/base.pyi
+-rw-r--r--   0        0        0      143 2022-08-08 01:00:32.346996 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/conversion.pyi
+-rw-r--r--   0        0        0     1195 2022-08-10 19:03:04.643581 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/dtypes.pyi
+-rw-r--r--   0        0        0     3543 2023-02-23 17:31:11.762588 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/nattype.pyi
+-rw-r--r--   0        0        0       89 2022-12-28 15:28:49.658657 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/np_datetime.pyi
+-rw-r--r--   0        0        0     8230 2023-02-23 17:31:11.763588 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/offsets.pyi
+-rw-r--r--   0        0        0      163 2022-08-08 01:00:32.387997 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/parsing.pyi
+-rw-r--r--   0        0        0     6525 2023-02-23 17:31:11.764590 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/period.pyi
+-rw-r--r--   0        0        0       72 2022-08-08 01:00:32.405128 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/strptime.pyi
+-rw-r--r--   0        0        0    14082 2023-04-05 02:20:38.239523 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/timedeltas.pyi
+-rw-r--r--   0        0        0    10731 2023-02-23 17:31:11.766587 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/timestamps.pyi
+-rw-r--r--   0        0        0       62 2022-08-08 01:00:32.438009 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/tzconversion.pyi
+-rw-r--r--   0        0        0      613 2023-02-04 17:09:12.293389 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/vectorized.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.574585 pandas_stubs-2.0.0.230412/pandas-stubs/_libs/window/__init__.pyi
+-rw-r--r--   0        0        0     4126 2023-02-04 17:09:12.293389 pandas_stubs-2.0.0.230412/pandas-stubs/_testing/__init__.pyi
+-rw-r--r--   0        0        0    15476 2023-04-12 19:14:53.205397 pandas_stubs-2.0.0.230412/pandas-stubs/_typing.pyi
+-rw-r--r--   0        0        0      124 2023-04-12 21:59:05.354817 pandas_stubs-2.0.0.230412/pandas-stubs/_version.pyi
+-rw-r--r--   0        0        0       94 2022-08-08 01:00:32.471998 pandas_stubs-2.0.0.230412/pandas-stubs/api/__init__.pyi
+-rw-r--r--   0        0        0      603 2023-02-27 22:18:36.851320 pandas_stubs-2.0.0.230412/pandas-stubs/api/extensions/__init__.pyi
+-rw-r--r--   0        0        0      241 2022-08-08 01:00:32.486031 pandas_stubs-2.0.0.230412/pandas-stubs/api/indexers/__init__.pyi
+-rw-r--r--   0        0        0      164 2022-12-28 15:28:49.664655 pandas_stubs-2.0.0.230412/pandas-stubs/api/interchange/__init__.pyi
+-rw-r--r--   0        0        0     1959 2022-12-28 15:28:49.665655 pandas_stubs-2.0.0.230412/pandas-stubs/api/types/__init__.pyi
+-rw-r--r--   0        0        0      373 2022-08-08 01:00:32.499997 pandas_stubs-2.0.0.230412/pandas-stubs/arrays/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.550503 pandas_stubs-2.0.0.230412/pandas-stubs/core/__init__.pyi
+-rw-r--r--   0        0        0      471 2022-08-08 01:00:32.505997 pandas_stubs-2.0.0.230412/pandas-stubs/core/accessor.pyi
+-rw-r--r--   0        0        0     2295 2023-03-04 20:30:27.571571 pandas_stubs-2.0.0.230412/pandas-stubs/core/algorithms.pyi
+-rw-r--r--   0        0        0     2680 2023-04-05 02:20:38.240522 pandas_stubs-2.0.0.230412/pandas-stubs/core/api.pyi
+-rw-r--r--   0        0        0     1846 2023-02-27 22:18:36.852304 pandas_stubs-2.0.0.230412/pandas-stubs/core/arraylike.pyi
+-rw-r--r--   0        0        0      726 2022-08-10 19:03:04.648579 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/__init__.pyi
+-rw-r--r--   0        0        0      321 2023-02-27 03:32:24.825818 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/arrow/dtype.pyi
+-rw-r--r--   0        0        0     2168 2023-04-01 02:35:39.716027 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/base.pyi
+-rw-r--r--   0        0        0      954 2023-02-27 22:18:36.854305 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/boolean.pyi
+-rw-r--r--   0        0        0     7407 2023-02-27 22:18:36.855305 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/categorical.pyi
+-rw-r--r--   0        0        0     2841 2023-02-27 22:18:36.855305 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/datetimelike.pyi
+-rw-r--r--   0        0        0     2216 2022-12-28 15:28:49.669665 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/datetimes.pyi
+-rw-r--r--   0        0        0      133 2022-12-28 15:28:49.670655 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/floating.pyi
+-rw-r--r--   0        0        0     1010 2023-02-27 03:32:24.827813 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/integer.pyi
+-rw-r--r--   0        0        0     2428 2023-02-27 22:18:36.856321 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/interval.pyi
+-rw-r--r--   0        0        0      964 2023-02-27 22:18:36.857336 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/masked.pyi
+-rw-r--r--   0        0        0       99 2023-02-27 03:32:24.828808 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/numeric.pyi
+-rw-r--r--   0        0        0      513 2023-02-27 03:32:24.828808 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/numpy_.pyi
+-rw-r--r--   0        0        0     1661 2023-02-04 17:09:12.300387 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/period.pyi
+-rw-r--r--   0        0        0      210 2022-12-28 15:28:49.674654 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/sparse/__init__.pyi
+-rw-r--r--   0        0        0      650 2023-04-12 19:14:53.206395 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/sparse/accessor.pyi
+-rw-r--r--   0        0        0     2309 2023-02-27 22:18:36.857336 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/sparse/array.pyi
+-rw-r--r--   0        0        0      448 2023-02-27 03:32:24.829807 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/sparse/dtype.pyi
+-rw-r--r--   0        0        0      715 2023-02-27 03:32:24.830807 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/string_.pyi
+-rw-r--r--   0        0        0     1963 2023-02-04 17:09:12.301416 pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/timedeltas.pyi
+-rw-r--r--   0        0        0     2681 2023-04-01 02:35:39.717031 pandas_stubs-2.0.0.230412/pandas-stubs/core/base.pyi
+-rw-r--r--   0        0        0      955 2023-02-04 17:09:12.302429 pandas_stubs-2.0.0.230412/pandas-stubs/core/common.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.561504 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/__init__.pyi
+-rw-r--r--   0        0        0       79 2022-08-08 01:00:32.662463 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/align.pyi
+-rw-r--r--   0        0        0       54 2022-08-08 01:00:32.670999 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/api.pyi
+-rw-r--r--   0        0        0       47 2022-08-10 19:03:04.655579 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/common.pyi
+-rw-r--r--   0        0        0      438 2022-12-28 15:28:49.678655 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/engines.pyi
+-rw-r--r--   0        0        0      668 2023-02-04 17:09:12.302429 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/eval.pyi
+-rw-r--r--   0        0        0     2265 2022-08-08 01:00:32.699007 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/expr.pyi
+-rw-r--r--   0        0        0      270 2022-08-08 01:00:32.711086 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/expressions.pyi
+-rw-r--r--   0        0        0     2324 2022-08-08 01:00:32.722048 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/ops.pyi
+-rw-r--r--   0        0        0      487 2023-02-04 17:09:12.303395 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/parsing.pyi
+-rw-r--r--   0        0        0     3061 2022-08-08 01:00:32.745044 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/pytables.pyi
+-rw-r--r--   0        0        0      645 2022-08-08 01:00:32.755711 pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/scope.pyi
+-rw-r--r--   0        0        0     1621 2022-08-08 01:00:32.764271 pandas_stubs-2.0.0.230412/pandas-stubs/core/config_init.pyi
+-rw-r--r--   0        0        0      926 2023-04-01 02:35:39.718026 pandas_stubs-2.0.0.230412/pandas-stubs/core/construction.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.565503 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/__init__.pyi
+-rw-r--r--   0        0        0     1625 2022-12-28 15:28:49.680655 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/api.pyi
+-rw-r--r--   0        0        0      834 2023-02-27 22:18:36.858307 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/base.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.681655 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/cast.pyi
+-rw-r--r--   0        0        0     2377 2023-02-23 17:31:11.770587 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/common.pyi
+-rw-r--r--   0        0        0      308 2023-02-23 17:31:11.771588 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/concat.pyi
+-rw-r--r--   0        0        0     1687 2023-02-27 22:18:36.858307 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/dtypes.pyi
+-rw-r--r--   0        0        0      207 2022-12-28 15:28:49.683657 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/generic.pyi
+-rw-r--r--   0        0        0      610 2022-12-28 15:28:49.684666 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/inference.pyi
+-rw-r--r--   0        0        0     1027 2022-12-28 15:28:49.684666 pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/missing.pyi
+-rw-r--r--   0        0        0    65003 2023-04-12 19:14:53.207397 pandas_stubs-2.0.0.230412/pandas-stubs/core/frame.pyi
+-rw-r--r--   0        0        0    14954 2023-04-12 19:14:53.208396 pandas_stubs-2.0.0.230412/pandas-stubs/core/generic.pyi
+-rw-r--r--   0        0        0      120 2022-08-08 01:00:32.927699 pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/__init__.pyi
+-rw-r--r--   0        0        0      261 2023-02-04 17:09:12.306444 pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/base.pyi
+-rw-r--r--   0        0        0      246 2022-08-10 19:03:04.661580 pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/categorical.pyi
+-rw-r--r--   0        0        0    12835 2023-03-04 20:30:27.574572 pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/generic.pyi
+-rw-r--r--   0        0        0     4139 2023-03-04 20:30:27.574572 pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/groupby.pyi
+-rw-r--r--   0        0        0     1647 2023-02-04 17:09:12.308388 pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/grouper.pyi
+-rw-r--r--   0        0        0     2721 2023-02-04 17:09:12.308388 pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/ops.pyi
+-rw-r--r--   0        0        0     1673 2022-08-10 19:03:04.663578 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexers.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.575505 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/__init__.pyi
+-rw-r--r--   0        0        0    12913 2023-04-05 02:20:38.241521 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/accessors.pyi
+-rw-r--r--   0        0        0      748 2023-04-05 02:20:38.241521 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/api.pyi
+-rw-r--r--   0        0        0    10393 2023-04-12 19:14:53.209396 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/base.pyi
+-rw-r--r--   0        0        0     1741 2023-02-23 17:31:11.776589 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/category.pyi
+-rw-r--r--   0        0        0      812 2023-02-23 17:31:11.777589 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/datetimelike.pyi
+-rw-r--r--   0        0        0     4393 2023-04-05 02:20:38.243522 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/datetimes.pyi
+-rw-r--r--   0        0        0       80 2023-02-23 17:31:11.778625 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/extension.pyi
+-rw-r--r--   0        0        0      429 2022-08-08 01:00:33.113434 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/frozen.pyi
+-rw-r--r--   0        0        0    13062 2023-04-05 02:20:38.243522 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/interval.pyi
+-rw-r--r--   0        0        0     5428 2023-04-01 02:35:39.720026 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/multi.pyi
+-rw-r--r--   0        0        0     2933 2023-02-23 17:31:11.781588 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/period.pyi
+-rw-r--r--   0        0        0     2853 2023-04-05 02:20:38.244521 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/range.pyi
+-rw-r--r--   0        0        0     2713 2023-02-23 17:31:11.783587 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/timedeltas.pyi
+-rw-r--r--   0        0        0     1849 2023-02-23 17:31:11.783587 pandas_stubs-2.0.0.230412/pandas-stubs/core/indexing.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.696655 pandas_stubs-2.0.0.230412/pandas-stubs/core/interchange/__init__.pyi
+-rw-r--r--   0        0        0     3166 2023-02-04 17:09:12.315386 pandas_stubs-2.0.0.230412/pandas-stubs/core/interchange/dataframe_protocol.pyi
+-rw-r--r--   0        0        0       92 2022-12-28 15:28:49.697655 pandas_stubs-2.0.0.230412/pandas-stubs/core/interchange/from_dataframe.pyi
+-rw-r--r--   0        0        0      346 2022-12-28 15:28:49.698655 pandas_stubs-2.0.0.230412/pandas-stubs/core/missing.pyi
+-rw-r--r--   0        0        0      211 2022-08-10 19:03:04.669578 pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/__init__.pyi
+-rw-r--r--   0        0        0      517 2022-08-10 19:03:04.669578 pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/array_ops.pyi
+-rw-r--r--   0        0        0       45 2022-08-08 01:00:33.245986 pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/common.pyi
+-rw-r--r--   0        0        0      120 2022-12-28 15:28:49.698655 pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/dispatch.pyi
+-rw-r--r--   0        0        0       17 2022-08-08 01:00:33.268029 pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/docstrings.pyi
+-rw-r--r--   0        0        0       81 2022-08-08 01:00:33.278086 pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/invalid.pyi
+-rw-r--r--   0        0        0      606 2022-08-08 01:00:33.289023 pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/mask_ops.pyi
+-rw-r--r--   0        0        0     6266 2023-03-04 20:30:27.575571 pandas_stubs-2.0.0.230412/pandas-stubs/core/resample.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.589504 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/__init__.pyi
+-rw-r--r--   0        0        0      633 2022-12-28 15:28:49.699654 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/api.pyi
+-rw-r--r--   0        0        0     2872 2023-04-12 19:14:53.210397 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/concat.pyi
+-rw-r--r--   0        0        0      716 2023-02-04 17:09:12.318387 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/encoding.pyi
+-rw-r--r--   0        0        0      741 2023-02-04 17:09:12.318387 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/melt.pyi
+-rw-r--r--   0        0        0     3089 2022-12-28 15:28:49.701655 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/merge.pyi
+-rw-r--r--   0        0        0     4113 2023-02-23 17:31:11.784589 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/pivot.pyi
+-rw-r--r--   0        0        0     7900 2023-04-05 02:20:38.246521 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/tile.pyi
+-rw-r--r--   0        0        0       30 2022-08-08 01:00:33.431568 pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/util.pyi
+-rw-r--r--   0        0        0    62534 2023-04-12 19:14:53.212397 pandas_stubs-2.0.0.230412/pandas-stubs/core/series.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.591599 pandas_stubs-2.0.0.230412/pandas-stubs/core/sparse/__init__.pyi
+-rw-r--r--   0        0        0     6667 2023-02-04 17:09:12.321425 pandas_stubs-2.0.0.230412/pandas-stubs/core/strings.pyi
+-rw-r--r--   0        0        0        0 2022-08-10 19:03:04.672581 pandas_stubs-2.0.0.230412/pandas-stubs/core/tools/__init__.pyi
+-rw-r--r--   0        0        0     2781 2023-02-23 17:31:11.787588 pandas_stubs-2.0.0.230412/pandas-stubs/core/tools/datetimes.pyi
+-rw-r--r--   0        0        0      873 2023-02-23 17:31:11.787588 pandas_stubs-2.0.0.230412/pandas-stubs/core/tools/numeric.pyi
+-rw-r--r--   0        0        0     1074 2023-02-04 17:09:12.322446 pandas_stubs-2.0.0.230412/pandas-stubs/core/tools/timedeltas.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.592587 pandas_stubs-2.0.0.230412/pandas-stubs/core/util/__init__.pyi
+-rw-r--r--   0        0        0      480 2022-12-28 15:28:49.706655 pandas_stubs-2.0.0.230412/pandas-stubs/core/util/hashing.pyi
+-rw-r--r--   0        0        0      274 2022-08-08 01:00:33.545825 pandas_stubs-2.0.0.230412/pandas-stubs/core/window/__init__.pyi
+-rw-r--r--   0        0        0     2484 2022-12-28 15:28:49.706655 pandas_stubs-2.0.0.230412/pandas-stubs/core/window/ewm.pyi
+-rw-r--r--   0        0        0     3838 2023-02-04 17:09:12.323425 pandas_stubs-2.0.0.230412/pandas-stubs/core/window/expanding.pyi
+-rw-r--r--   0        0        0     5796 2023-02-04 17:09:12.324423 pandas_stubs-2.0.0.230412/pandas-stubs/core/window/rolling.pyi
+-rw-r--r--   0        0        0     1808 2022-12-28 15:28:49.709656 pandas_stubs-2.0.0.230412/pandas-stubs/errors/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.599505 pandas_stubs-2.0.0.230412/pandas-stubs/io/__init__.pyi
+-rw-r--r--   0        0        0     1132 2022-08-08 01:00:33.649500 pandas_stubs-2.0.0.230412/pandas-stubs/io/api.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.710655 pandas_stubs-2.0.0.230412/pandas-stubs/io/clipboard/__init__.pyi
+-rw-r--r--   0        0        0     6938 2023-04-12 19:14:53.213395 pandas_stubs-2.0.0.230412/pandas-stubs/io/clipboards.pyi
+-rw-r--r--   0        0        0      487 2022-12-28 15:28:49.711655 pandas_stubs-2.0.0.230412/pandas-stubs/io/common.pyi
+-rw-r--r--   0        0        0      128 2022-08-08 01:00:33.708448 pandas_stubs-2.0.0.230412/pandas-stubs/io/excel/__init__.pyi
+-rw-r--r--   0        0        0     7653 2023-04-12 19:14:53.214395 pandas_stubs-2.0.0.230412/pandas-stubs/io/excel/_base.pyi
+-rw-r--r--   0        0        0       73 2022-08-08 01:00:33.734493 pandas_stubs-2.0.0.230412/pandas-stubs/io/excel/_util.pyi
+-rw-r--r--   0        0        0      335 2022-08-29 12:14:24.788360 pandas_stubs-2.0.0.230412/pandas-stubs/io/feather_format.pyi
+-rw-r--r--   0        0        0        0 2022-07-03 21:17:38.596585 pandas_stubs-2.0.0.230412/pandas-stubs/io/formats/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.712655 pandas_stubs-2.0.0.230412/pandas-stubs/io/formats/css.pyi
+-rw-r--r--   0        0        0      338 2022-12-28 15:28:49.713678 pandas_stubs-2.0.0.230412/pandas-stubs/io/formats/format.pyi
+-rw-r--r--   0        0        0    11408 2023-03-04 20:30:27.577572 pandas_stubs-2.0.0.230412/pandas-stubs/io/formats/style.pyi
+-rw-r--r--   0        0        0     2436 2023-03-04 20:30:27.578572 pandas_stubs-2.0.0.230412/pandas-stubs/io/formats/style_render.pyi
+-rw-r--r--   0        0        0      685 2022-08-20 01:19:02.005181 pandas_stubs-2.0.0.230412/pandas-stubs/io/gbq.pyi
+-rw-r--r--   0        0        0     1382 2023-02-04 17:09:12.326429 pandas_stubs-2.0.0.230412/pandas-stubs/io/html.pyi
+-rw-r--r--   0        0        0      170 2022-08-29 12:14:24.789359 pandas_stubs-2.0.0.230412/pandas-stubs/io/json/__init__.pyi
+-rw-r--r--   0        0        0     4110 2023-02-04 17:09:12.327388 pandas_stubs-2.0.0.230412/pandas-stubs/io/json/_json.pyi
+-rw-r--r--   0        0        0      403 2022-08-29 12:14:24.790358 pandas_stubs-2.0.0.230412/pandas-stubs/io/json/_normalize.pyi
+-rw-r--r--   0        0        0      285 2022-08-29 12:14:24.790358 pandas_stubs-2.0.0.230412/pandas-stubs/io/json/_table_schema.pyi
+-rw-r--r--   0        0        0      282 2022-08-29 12:14:24.791359 pandas_stubs-2.0.0.230412/pandas-stubs/io/orc.pyi
+-rw-r--r--   0        0        0      421 2022-08-29 12:14:24.791359 pandas_stubs-2.0.0.230412/pandas-stubs/io/parquet.pyi
+-rw-r--r--   0        0        0      168 2022-12-28 15:28:49.716655 pandas_stubs-2.0.0.230412/pandas-stubs/io/parsers/__init__.pyi
+-rw-r--r--   0        0        0    15581 2023-04-12 19:14:53.215395 pandas_stubs-2.0.0.230412/pandas-stubs/io/parsers/readers.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.716655 pandas_stubs-2.0.0.230412/pandas-stubs/io/parsers.pyi
+-rw-r--r--   0        0        0      558 2022-12-28 15:28:49.717656 pandas_stubs-2.0.0.230412/pandas-stubs/io/pickle.pyi
+-rw-r--r--   0        0        0     6725 2023-02-23 17:31:11.791589 pandas_stubs-2.0.0.230412/pandas-stubs/io/pytables.pyi
+-rw-r--r--   0        0        0       58 2022-08-29 12:14:24.793360 pandas_stubs-2.0.0.230412/pandas-stubs/io/sas/__init__.pyi
+-rw-r--r--   0        0        0      256 2022-12-28 15:28:49.718670 pandas_stubs-2.0.0.230412/pandas-stubs/io/sas/sas7bdat.pyi
+-rw-r--r--   0        0        0      250 2022-08-29 12:14:24.794359 pandas_stubs-2.0.0.230412/pandas-stubs/io/sas/sas_xport.pyi
+-rw-r--r--   0        0        0     2976 2023-02-23 17:31:11.792588 pandas_stubs-2.0.0.230412/pandas-stubs/io/sas/sasreader.pyi
+-rw-r--r--   0        0        0      250 2022-08-29 12:14:24.795362 pandas_stubs-2.0.0.230412/pandas-stubs/io/spss.pyi
+-rw-r--r--   0        0        0     4871 2023-02-23 17:31:11.794588 pandas_stubs-2.0.0.230412/pandas-stubs/io/sql.pyi
+-rw-r--r--   0        0        0     4334 2023-02-23 17:31:11.795592 pandas_stubs-2.0.0.230412/pandas-stubs/io/stata.pyi
+-rw-r--r--   0        0        0     1015 2023-02-04 17:09:12.330386 pandas_stubs-2.0.0.230412/pandas-stubs/io/xml.pyi
+-rw-r--r--   0        0        0      587 2022-12-28 15:28:49.720654 pandas_stubs-2.0.0.230412/pandas-stubs/plotting/__init__.pyi
+-rw-r--r--   0        0        0    12852 2023-02-23 17:31:11.796591 pandas_stubs-2.0.0.230412/pandas-stubs/plotting/_core.pyi
+-rw-r--r--   0        0        0     2360 2023-02-23 17:31:11.797589 pandas_stubs-2.0.0.230412/pandas-stubs/plotting/_misc.pyi
+-rw-r--r--   0        0        0        0 2022-12-28 15:28:49.722656 pandas_stubs-2.0.0.230412/pandas-stubs/py.typed
+-rw-r--r--   0        0        0      368 2022-08-08 01:00:34.094401 pandas_stubs-2.0.0.230412/pandas-stubs/testing.pyi
+-rw-r--r--   0        0        0        0 2022-07-02 19:36:57.614504 pandas_stubs-2.0.0.230412/pandas-stubs/tseries/__init__.pyi
+-rw-r--r--   0        0        0       64 2022-08-08 01:00:34.100409 pandas_stubs-2.0.0.230412/pandas-stubs/tseries/api.pyi
+-rw-r--r--   0        0        0      378 2022-12-28 15:28:49.722656 pandas_stubs-2.0.0.230412/pandas-stubs/tseries/frequencies.pyi
+-rw-r--r--   0        0        0      118 2022-08-29 12:14:32.889752 pandas_stubs-2.0.0.230412/pandas-stubs/tseries/holiday.pyi
+-rw-r--r--   0        0        0     1312 2022-08-08 01:00:34.111525 pandas_stubs-2.0.0.230412/pandas-stubs/tseries/offsets.pyi
+-rw-r--r--   0        0        0      255 2022-12-28 15:28:49.723655 pandas_stubs-2.0.0.230412/pandas-stubs/util/__init__.pyi
+-rw-r--r--   0        0        0     1230 2023-02-04 17:09:12.332423 pandas_stubs-2.0.0.230412/pandas-stubs/util/_decorators.pyi
+-rw-r--r--   0        0        0      279 2022-08-08 01:00:34.130416 pandas_stubs-2.0.0.230412/pandas-stubs/util/_doctools.pyi
+-rw-r--r--   0        0        0       57 2022-08-08 01:00:34.135732 pandas_stubs-2.0.0.230412/pandas-stubs/util/_exceptions.pyi
+-rw-r--r--   0        0        0       53 2022-12-28 15:28:49.723655 pandas_stubs-2.0.0.230412/pandas-stubs/util/_print_versions.pyi
+-rw-r--r--   0        0        0       38 2022-08-08 01:00:34.153394 pandas_stubs-2.0.0.230412/pandas-stubs/util/_tester.pyi
+-rw-r--r--   0        0        0      594 2023-02-04 17:09:12.332423 pandas_stubs-2.0.0.230412/pandas-stubs/util/_validators.pyi
+-rw-r--r--   0        0        0     1899 2022-12-28 15:28:49.725656 pandas_stubs-2.0.0.230412/pandas-stubs/util/version/__init__.pyi
+-rw-r--r--   0        0        0     6935 2023-04-12 21:58:43.256511 pandas_stubs-2.0.0.230412/pyproject.toml
+-rw-r--r--   0        0        0     8415 2023-04-12 21:57:46.990004 pandas_stubs-2.0.0.230412/README.md
+-rw-r--r--   0        0        0    10415 1970-01-01 00:00:00.000000 pandas_stubs-2.0.0.230412/setup.py
+-rw-r--r--   0        0        0     9685 1970-01-01 00:00:00.000000 pandas_stubs-2.0.0.230412/PKG-INFO
```

### Comparing `pandas_stubs-1.5.3.230321/LICENSE` & `pandas_stubs-2.0.0.230412/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/__init__.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/__init__.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -25,23 +25,21 @@
     CategoricalIndex as CategoricalIndex,
     DataFrame as DataFrame,
     DateOffset as DateOffset,
     DatetimeIndex as DatetimeIndex,
     DatetimeTZDtype as DatetimeTZDtype,
     Float32Dtype as Float32Dtype,
     Float64Dtype as Float64Dtype,
-    Float64Index as Float64Index,
     Grouper as Grouper,
     Index as Index,
     IndexSlice as IndexSlice,
     Int8Dtype as Int8Dtype,
     Int16Dtype as Int16Dtype,
     Int32Dtype as Int32Dtype,
     Int64Dtype as Int64Dtype,
-    Int64Index as Int64Index,
     Interval as Interval,
     IntervalDtype as IntervalDtype,
     IntervalIndex as IntervalIndex,
     MultiIndex as MultiIndex,
     NamedAgg as NamedAgg,
     NaT as NaT,
     Period as Period,
@@ -53,15 +51,14 @@
     Timedelta as Timedelta,
     TimedeltaIndex as TimedeltaIndex,
     Timestamp as Timestamp,
     UInt8Dtype as UInt8Dtype,
     UInt16Dtype as UInt16Dtype,
     UInt32Dtype as UInt32Dtype,
     UInt64Dtype as UInt64Dtype,
-    UInt64Index as UInt64Index,
     array as array,
     bdate_range as bdate_range,
     date_range as date_range,
     factorize as factorize,
     interval_range as interval_range,
     isna as isna,
     isnull as isnull,
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/_config/config.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/_config/config.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/_libs/interval.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/interval.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/_libs/lib.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/lib.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/_libs/missing.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/missing.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/__init__.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/dtypes.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/nattype.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/nattype.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/offsets.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/offsets.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/period.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/period.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/timedeltas.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/timedeltas.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,22 @@
     overload,
 )
 
 import numpy as np
 import pandas as pd
 from pandas import (
     DatetimeIndex,
-    Float64Index,
-    Int64Index,
     PeriodIndex,
     Series,
     TimedeltaIndex,
 )
+from pandas.core.indexes.base import (
+    _FloatIndexType,
+    _IntIndexType,
+)
 from pandas.core.series import (
     TimedeltaSeries,
     TimestampSeries,
 )
 from typing_extensions import (
     Self,
     TypeAlias,
@@ -239,25 +241,25 @@
         self, other: npt.NDArray[np.integer] | npt.NDArray[np.floating]
     ) -> npt.NDArray[np.timedelta64]: ...
     @overload
     def __mul__(self, other: Series[int]) -> TimedeltaSeries: ...
     @overload
     def __mul__(self, other: Series[float]) -> TimedeltaSeries: ...
     @overload
-    def __mul__(self, other: Int64Index | Float64Index) -> TimedeltaIndex: ...
+    def __mul__(self, other: _IntIndexType | _FloatIndexType) -> TimedeltaIndex: ...
     @overload
     def __rmul__(self, other: float) -> Timedelta: ...
     @overload
     def __rmul__(self, other: np.ndarray) -> np.ndarray: ...
     @overload
     def __rmul__(self, other: Series[int]) -> TimedeltaSeries: ...
     @overload
     def __rmul__(self, other: Series[float]) -> TimedeltaSeries: ...
     @overload
-    def __rmul__(self, other: Int64Index | Float64Index) -> TimedeltaIndex: ...
+    def __rmul__(self, other: _IntIndexType | _FloatIndexType) -> TimedeltaIndex: ...
     # Override due to more types supported than dt.timedelta
     # error: Signature of "__floordiv__" incompatible with supertype "timedelta"
     @overload  # type: ignore[override]
     def __floordiv__(self, other: timedelta | Timedelta | np.timedelta64) -> int: ...
     @overload
     def __floordiv__(self, other: float) -> Timedelta: ...
     @overload
@@ -265,15 +267,17 @@
         self, other: npt.NDArray[np.integer] | npt.NDArray[np.floating]
     ) -> npt.NDArray[np.timedelta64]: ...
     @overload
     def __floordiv__(
         self, other: npt.NDArray[np.timedelta64]
     ) -> npt.NDArray[np.int_]: ...
     @overload
-    def __floordiv__(self, other: Int64Index | Float64Index) -> TimedeltaIndex: ...
+    def __floordiv__(
+        self, other: _IntIndexType | _FloatIndexType
+    ) -> TimedeltaIndex: ...
     @overload
     def __floordiv__(self, other: Series[int]) -> TimedeltaSeries: ...
     @overload
     def __floordiv__(self, other: Series[float]) -> TimedeltaSeries: ...
     @overload
     def __floordiv__(self, other: TimedeltaSeries) -> Series[int]: ...
     @overload
@@ -298,15 +302,15 @@
     @overload
     def __truediv__(self, other: TimedeltaSeries) -> Series[float]: ...
     @overload
     def __truediv__(self, other: Series[int]) -> TimedeltaSeries: ...
     @overload
     def __truediv__(self, other: Series[float]) -> TimedeltaSeries: ...
     @overload
-    def __truediv__(self, other: Int64Index | Float64Index) -> TimedeltaIndex: ...
+    def __truediv__(self, other: _IntIndexType | _FloatIndexType) -> TimedeltaIndex: ...
     def __rtruediv__(self, other: timedelta | Timedelta | NaTType) -> float: ...
     # Override due to more types supported than dt.timedelta
     @overload
     def __eq__(self, other: timedelta | Timedelta | np.timedelta64) -> bool: ...  # type: ignore[misc] # pyright: ignore[reportOverlappingOverload]
     @overload
     def __eq__(self, other: TimedeltaSeries | Series[pd.Timedelta]) -> Series[bool]: ...  # type: ignore[misc]
     @overload
@@ -330,15 +334,15 @@
     @overload  # type: ignore[override]
     def __mod__(self, other: timedelta) -> Timedelta: ...
     @overload
     def __mod__(self, other: float) -> Timedelta: ...
     @overload
     def __mod__(self, other: Series[int] | Series[float]) -> TimedeltaSeries: ...
     @overload
-    def __mod__(self, other: Int64Index | Float64Index) -> TimedeltaIndex: ...
+    def __mod__(self, other: _IntIndexType | _FloatIndexType) -> TimedeltaIndex: ...
     @overload
     def __mod__(
         self, other: npt.NDArray[np.integer] | npt.NDArray[np.floating]
     ) -> npt.NDArray[np.timedelta64]: ...
     @overload
     def __mod__(
         self, other: Series[int] | Series[float] | TimedeltaSeries
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/timestamps.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/timestamps.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/_libs/tslibs/vectorized.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/_libs/tslibs/vectorized.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/_testing/__init__.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/_testing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/_typing.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/_typing.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -265,51 +265,67 @@
 DtypeNp = TypeVar("DtypeNp", bound=np.dtype[np.generic])
 KeysArgType: TypeAlias = Any
 ListLike = TypeVar("ListLike", Sequence, np.ndarray, "Series", "Index")
 ListLikeExceptSeriesAndStr = TypeVar(
     "ListLikeExceptSeriesAndStr", MutableSequence, np.ndarray, tuple, "Index"
 )
 ListLikeU: TypeAlias = Sequence | np.ndarray | Series | Index
+ListLikeHashable: TypeAlias = (
+    MutableSequence[HashableT] | np.ndarray | tuple[HashableT, ...] | range
+)
 StrLike: TypeAlias = str | np.str_
 IndexIterScalar: TypeAlias = (
     str
     | bytes
     | datetime.date
     | datetime.datetime
     | datetime.timedelta
     | np.datetime64
     | np.timedelta64
     | bool
     | int
     | float
     | Timestamp
     | Timedelta
+    | np.integer
+    | np.float_
 )
 Scalar: TypeAlias = IndexIterScalar | complex
 ScalarT = TypeVar("ScalarT", bound=Scalar)
 # Refine the definitions below in 3.9 to use the specialized type.
 np_ndarray_int64: TypeAlias = npt.NDArray[np.int64]
 np_ndarray_int: TypeAlias = npt.NDArray[np.signedinteger]
 np_ndarray_anyint: TypeAlias = npt.NDArray[np.integer]
 np_ndarray_bool: TypeAlias = npt.NDArray[np.bool_]
 np_ndarray_str: TypeAlias = npt.NDArray[np.str_]
 
 IndexType: TypeAlias = slice | np_ndarray_anyint | Index | list[int] | Series[int]
 MaskType: TypeAlias = Series[bool] | np_ndarray_bool | list[bool]
+UsecolsArgType: TypeAlias = (
+    MutableSequence[str]
+    | tuple[str, ...]
+    | Sequence[int]
+    | Series
+    | Index
+    | np.ndarray
+    | Callable[[HashableT], bool]
+    | None
+)
 # Scratch types for generics
 S1 = TypeVar(
     "S1",
     str,
     bytes,
     datetime.date,
     datetime.time,
     bool,
     int,
     float,
     complex,
+    Dtype,
     Timestamp,
     Timedelta,
     Period,
     Interval[int],
     Interval[float],
     Interval[Timestamp],
     Interval[Timedelta],
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/api/extensions/__init__.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/api/extensions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/api/types/__init__.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/api/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/algorithms.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/algorithms.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/api.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/api.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -26,23 +26,20 @@
 from pandas.core.groupby import (
     Grouper as Grouper,
     NamedAgg as NamedAgg,
 )
 from pandas.core.indexes.api import (
     CategoricalIndex as CategoricalIndex,
     DatetimeIndex as DatetimeIndex,
-    Float64Index as Float64Index,
     Index as Index,
-    Int64Index as Int64Index,
     IntervalIndex as IntervalIndex,
     MultiIndex as MultiIndex,
     PeriodIndex as PeriodIndex,
     RangeIndex as RangeIndex,
     TimedeltaIndex as TimedeltaIndex,
-    UInt64Index as UInt64Index,
 )
 from pandas.core.indexes.datetimes import (
     bdate_range as bdate_range,
     date_range as date_range,
 )
 from pandas.core.indexes.interval import (
     Interval as Interval,
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arraylike.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arraylike.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/__init__.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/base.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/base.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         *,
         allow_fill: bool = ...,
         fill_value=...,
     ) -> Self: ...
     def copy(self) -> Self: ...
     def view(self, dtype=...) -> Self | np.ndarray: ...
     def ravel(self, order=...) -> Self: ...
+    def tolist(self) -> list: ...
 
 class ExtensionOpsMixin:
     @classmethod
     def _add_arithmetic_ops(cls) -> None: ...
     @classmethod
     def _add_comparison_ops(cls) -> None: ...
     @classmethod
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/boolean.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/boolean.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/categorical.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/categorical.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/datetimelike.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/datetimelike.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/datetimes.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/datetimes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/integer.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/integer.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/interval.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/interval.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/masked.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/masked.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/numpy_.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/numpy_.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/period.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/period.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/sparse/array.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/sparse/array.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/string_.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/string_.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/arrays/timedeltas.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/arrays/timedeltas.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/base.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/base.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -53,18 +53,18 @@
     ) -> np.ndarray: ...
     @property
     def empty(self) -> bool: ...
     def max(self, axis=..., skipna: bool = ..., **kwargs): ...
     def min(self, axis=..., skipna: bool = ..., **kwargs): ...
     def argmax(
         self, axis: AxisIndex | None = ..., skipna: bool = ..., *args, **kwargs
-    ) -> np.ndarray: ...
+    ) -> np.int64: ...
     def argmin(
         self, axis: AxisIndex | None = ..., skipna: bool = ..., *args, **kwargs
-    ) -> np.ndarray: ...
+    ) -> np.int64: ...
     def tolist(self) -> list: ...
     def to_list(self) -> list: ...
     def __iter__(self): ...
     @property
     def hasnans(self) -> bool: ...
     def value_counts(
         self,
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/common.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/common.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/eval.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/eval.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/expr.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/expr.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/ops.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/pytables.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/pytables.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/computation/scope.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/computation/scope.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/config_init.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/config_init.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/construction.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/construction.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from collections.abc import Sequence
 
 import numpy as np
+from pandas.core.arrays.base import ExtensionArray
 from pandas.core.indexes.api import Index
 from pandas.core.series import Series
 
 from pandas._typing import (
     ArrayLike,
     Dtype,
 )
 
 from pandas.core.dtypes.dtypes import ExtensionDtype
-from pandas.core.dtypes.generic import ABCExtensionArray
 
 def array(
     data: Sequence[object],
     dtype: str | np.dtype | ExtensionDtype | None = ...,
     copy: bool = ...,
-) -> ABCExtensionArray: ...
+) -> ExtensionArray: ...
 def extract_array(obj, extract_numpy: bool = ...): ...
 def sanitize_array(
     data, index, dtype=..., copy: bool = ..., raise_cast_failure: bool = ...
 ): ...
 def is_empty_data(data) -> bool: ...
 def create_series_with_explicit_dtype(
     data=...,
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/api.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/base.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/base.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/common.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/common.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/dtypes.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/inference.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/inference.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/dtypes/missing.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/dtypes/missing.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/frame.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/frame.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -264,40 +264,69 @@
         dtype: npt.DTypeLike | None = ...,
         copy: bool = ...,
         na_value: Scalar = ...,
     ) -> np.ndarray: ...
     @overload
     def to_dict(
         self,
-        orient: Literal["dict", "list", "series", "split", "tight", "index"],
+        orient: Literal["records"],
         into: Mapping | type[Mapping],
+        index: Literal[True] = ...,
+    ) -> list[Mapping[Hashable, Any]]: ...
+    @overload
+    def to_dict(
+        self,
+        orient: Literal["records"],
+        into: None = ...,
+        index: Literal[True] = ...,
+    ) -> list[dict[Hashable, Any]]: ...
+    @overload
+    def to_dict(
+        self,
+        orient: Literal["dict", "list", "series", "index"],
+        into: Mapping | type[Mapping],
+        index: Literal[True] = ...,
     ) -> Mapping[Hashable, Any]: ...
     @overload
     def to_dict(
         self,
-        orient: Literal["dict", "list", "series", "split", "tight", "index"] = ...,
-        *,
+        orient: Literal["split", "tight"],
         into: Mapping | type[Mapping],
+        index: bool = ...,
     ) -> Mapping[Hashable, Any]: ...
     @overload
     def to_dict(
         self,
-        orient: Literal["dict", "list", "series", "split", "tight", "index"] = ...,
-        into: None = ...,
-    ) -> dict[Hashable, Any]: ...
+        orient: Literal["dict", "list", "series", "index"] = ...,
+        *,
+        into: Mapping | type[Mapping],
+        index: Literal[True] = ...,
+    ) -> Mapping[Hashable, Any]: ...
     @overload
     def to_dict(
         self,
-        orient: Literal["records"],
+        orient: Literal["split", "tight"] = ...,
+        *,
         into: Mapping | type[Mapping],
-    ) -> list[Mapping[Hashable, Any]]: ...
+        index: bool = ...,
+    ) -> Mapping[Hashable, Any]: ...
     @overload
     def to_dict(
-        self, orient: Literal["records"], into: None = ...
-    ) -> list[dict[Hashable, Any]]: ...
+        self,
+        orient: Literal["dict", "list", "series", "index"] = ...,
+        into: None = ...,
+        index: Literal[True] = ...,
+    ) -> dict[Hashable, Any]: ...
+    @overload
+    def to_dict(
+        self,
+        orient: Literal["split", "tight"] = ...,
+        into: None = ...,
+        index: bool = ...,
+    ) -> dict[Hashable, Any]: ...
     def to_gbq(
         self,
         destination_table: str,
         project_id: str | None = ...,
         chunksize: int | None = ...,
         reauth: bool = ...,
         if_exists: Literal["fail", "replace", "append"] = ...,
@@ -512,15 +541,15 @@
     ) -> None: ...
     def memory_usage(self, index: _bool = ..., deep: _bool = ...) -> Series: ...
     def transpose(self, *args, copy: _bool = ...) -> DataFrame: ...
     @property
     def T(self) -> DataFrame: ...
     def __getattr__(self, name: str) -> Series: ...
     @overload
-    def __getitem__(self, idx: Scalar | tuple[Hashable, ...]) -> Series: ...
+    def __getitem__(self, idx: Scalar | Hashable) -> Series: ...
     @overload
     def __getitem__(self, rows: slice) -> DataFrame: ...
     @overload
     def __getitem__(
         self,
         idx: Series[_bool]
         | DataFrame
@@ -1396,16 +1425,16 @@
     def add(
         self,
         other: num | ListLike | DataFrame,
         axis: Axis | None = ...,
         level: Level | None = ...,
         fill_value: float | None = ...,
     ) -> DataFrame: ...
-    def add_prefix(self, prefix: _str) -> DataFrame: ...
-    def add_suffix(self, suffix: _str) -> DataFrame: ...
+    def add_prefix(self, prefix: _str, axis: Axis | None = None) -> DataFrame: ...
+    def add_suffix(self, suffix: _str, axis: Axis | None = None) -> DataFrame: ...
     @overload
     def all(
         self,
         axis: None,
         bool_only: _bool | None = ...,
         skipna: _bool = ...,
         **kwargs,
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/generic.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/generic.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
     def ndim(self) -> int: ...
     @property
     def size(self) -> int: ...
     def swapaxes(
         self, axis1: AxisIndex, axis2: AxisIndex, copy: _bool = ...
     ) -> NDFrame: ...
     def droplevel(self, level: Level, axis: AxisIndex = ...) -> NDFrame: ...
-    def pop(self, item: _str) -> NDFrame: ...
     def squeeze(self, axis=...): ...
     def equals(self, other: Series[S1]) -> _bool: ...
     def __neg__(self: NDFrameT) -> NDFrameT: ...
     def __pos__(self: NDFrameT) -> NDFrameT: ...
     def __nonzero__(self) -> None: ...
     @final
     def bool(self) -> _bool: ...
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/groupby/generic.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/generic.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/groupby/groupby.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/groupby.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/groupby/grouper.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/grouper.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/groupby/ops.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/groupby/ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/indexers.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexers.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/accessors.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/accessors.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     PeriodArray,
 )
 from pandas.core.base import (
     NoNewAttributesMixin,
     PandasObject,
 )
 from pandas.core.frame import DataFrame
-from pandas.core.indexes.numeric import NumericIndex
+from pandas.core.indexes.base import _IntIndexType
 from pandas.core.series import (
     PeriodSeries,
     Series,
     TimedeltaSeries,
     TimestampSeries,
 )
 
@@ -39,22 +39,22 @@
     TimestampConvention,
     np_ndarray_bool,
 )
 
 class Properties(PandasDelegate, PandasObject, NoNewAttributesMixin):
     def __init__(self, data: Series, orig) -> None: ...
 
-_DTFieldOpsReturnType = TypeVar("_DTFieldOpsReturnType", Series[int], NumericIndex)
+_DTFieldOpsReturnType = TypeVar("_DTFieldOpsReturnType", Series[int], _IntIndexType)
 
 class _DatetimeFieldOps(
     _DayLikeFieldOps[_DTFieldOpsReturnType], _MiniSeconds[_DTFieldOpsReturnType]
 ): ...
 class PeriodIndexFieldOps(
-    _DayLikeFieldOps[NumericIndex],
-    _PeriodProperties[DatetimeIndex, NumericIndex, Index, DatetimeIndex, PeriodIndex],
+    _DayLikeFieldOps[_IntIndexType],
+    _PeriodProperties[DatetimeIndex, _IntIndexType, Index, DatetimeIndex, PeriodIndex],
 ): ...
 
 class _DayLikeFieldOps(Generic[_DTFieldOpsReturnType]):
     @property
     def year(self) -> _DTFieldOpsReturnType: ...
     @property
     def month(self) -> _DTFieldOpsReturnType: ...
@@ -302,15 +302,15 @@
 class TimedeltaProperties(
     Properties,
     _TimedeltaPropertiesNoRounding[Series[int], Series[float]],
     _DatetimeRoundingMethods[TimedeltaSeries],
 ): ...
 
 _PeriodDTReturnTypes = TypeVar("_PeriodDTReturnTypes", TimestampSeries, DatetimeIndex)
-_PeriodIntReturnTypes = TypeVar("_PeriodIntReturnTypes", Series[int], NumericIndex)
+_PeriodIntReturnTypes = TypeVar("_PeriodIntReturnTypes", Series[int], _IntIndexType)
 _PeriodStrReturnTypes = TypeVar("_PeriodStrReturnTypes", Series[str], Index)
 _PeriodDTAReturnTypes = TypeVar("_PeriodDTAReturnTypes", DatetimeArray, DatetimeIndex)
 _PeriodPAReturnTypes = TypeVar("_PeriodPAReturnTypes", PeriodArray, PeriodIndex)
 
 class _PeriodProperties(
     Generic[
         _PeriodDTReturnTypes,
@@ -378,15 +378,15 @@
         PeriodSeries,
     ]
 ): ...
 
 class DatetimeIndexProperties(
     Properties,
     _DatetimeNoTZProperties[
-        NumericIndex,
+        _IntIndexType,
         np_ndarray_bool,
         DatetimeIndex,
         np.ndarray,
         np.ndarray,
         BaseOffset,
         DatetimeIndex,
         Index,
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/api.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/api.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 from pandas.core.indexes.base import Index as Index
 from pandas.core.indexes.category import CategoricalIndex as CategoricalIndex
 from pandas.core.indexes.datetimes import DatetimeIndex as DatetimeIndex
 from pandas.core.indexes.interval import IntervalIndex as IntervalIndex
 from pandas.core.indexes.multi import MultiIndex as MultiIndex
-from pandas.core.indexes.numeric import (
-    Float64Index as Float64Index,
-    Int64Index as Int64Index,
-    NumericIndex as NumericIndex,
-    UInt64Index as UInt64Index,
-)
 from pandas.core.indexes.period import PeriodIndex as PeriodIndex
 from pandas.core.indexes.range import RangeIndex as RangeIndex
 from pandas.core.indexes.timedeltas import TimedeltaIndex as TimedeltaIndex
 
 def get_objs_combined_axis(
     objs, intersect: bool = ..., axis=..., sort: bool = ...
 ) -> Index: ...
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/base.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/base.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     Series,
 )
 from pandas.core.arrays import ExtensionArray
 from pandas.core.base import (
     IndexOpsMixin,
     PandasObject,
 )
-from pandas.core.indexes.numeric import NumericIndex
 from pandas.core.strings import StringMethods
 from typing_extensions import (
     Never,
     Self,
 )
 
 from pandas._typing import (
@@ -70,20 +69,43 @@
 
 class Index(IndexOpsMixin, PandasObject):
     __hash__: ClassVar[None]  # type: ignore[assignment]
     @overload
     def __new__(
         cls,
         data: Iterable,
-        dtype: Literal["float", "int", "complex"] | type_t[complex] | type_t[np.number],
+        dtype: Literal["int"] | type_t[int] | type_t[np.integer],
         copy: bool = ...,
         name=...,
         tupleize_cols: bool = ...,
         **kwargs,
-    ) -> NumericIndex: ...
+    ) -> _IntIndexType: ...
+    @overload
+    def __new__(
+        cls,
+        data: Iterable,
+        dtype: Literal["float"]
+        | type_t[float]
+        | type_t[np.float32]
+        | type_t[np.float64],
+        copy: bool = ...,
+        name=...,
+        tupleize_cols: bool = ...,
+        **kwargs,
+    ) -> _FloatIndexType: ...
+    @overload
+    def __new__(
+        cls,
+        data: Iterable,
+        dtype: Literal["complex"] | type_t[complex],
+        copy: bool = ...,
+        name=...,
+        tupleize_cols: bool = ...,
+        **kwargs,
+    ) -> _ComplexIndexType: ...
     @overload
     def __new__(
         cls,
         data: Iterable = ...,
         dtype=...,
         copy: bool = ...,
         name=...,
@@ -256,7 +278,23 @@
     def __gt__(self, other: Index | Scalar) -> np_ndarray_bool: ...  # type: ignore[override]
 
 def ensure_index_from_sequences(
     sequences: Sequence[Sequence[Dtype]], names: list[str] = ...
 ) -> Index: ...
 def ensure_index(index_like: Sequence | Index, copy: bool = ...) -> Index: ...
 def maybe_extract_name(name, obj, cls) -> Label: ...
+
+class _NumericIndexType(Index):
+    def __add__(self, other: _NumericIndexType | complex) -> Self: ...
+    def __radd__(self, other: _NumericIndexType | complex) -> Self: ...
+    def __sub__(self, other: _NumericIndexType | complex) -> Self: ...
+    def __rsub__(self, other: _NumericIndexType | complex) -> Self: ...
+    def __mul__(self, other: _NumericIndexType | complex) -> Self: ...
+    def __rmul__(self, other: _NumericIndexType | complex) -> Self: ...
+    def __truediv__(self, other: _NumericIndexType | complex) -> Self: ...
+    def __rtruediv__(self, other: _NumericIndexType | complex) -> Self: ...
+    def __floordiv__(self, other: _NumericIndexType | complex) -> Self: ...
+    def __rfloordiv__(self, other: _NumericIndexType | complex) -> Self: ...
+
+class _FloatIndexType(_NumericIndexType): ...
+class _IntIndexType(_NumericIndexType): ...
+class _ComplexIndexType(_NumericIndexType): ...
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/category.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/category.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/datetimelike.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/datetimelike.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/datetimes.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/datetimes.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 from pandas import (
     DataFrame,
     Timedelta,
     TimedeltaIndex,
     Timestamp,
 )
 from pandas.core.indexes.accessors import DatetimeIndexProperties
-from pandas.core.indexes.api import Float64Index
-from pandas.core.indexes.base import _IndexGetitemMixin
+from pandas.core.indexes.base import (
+    _FloatIndexType,
+    _IndexGetitemMixin,
+)
 from pandas.core.indexes.datetimelike import DatetimeTimedeltaMixin
 from pandas.core.series import (
     TimedeltaSeries,
     TimestampSeries,
 )
 
 from pandas._typing import (
@@ -82,15 +84,15 @@
     def inferred_type(self) -> str: ...
     def insert(self, loc, item): ...
     def indexer_at_time(self, time, asof: bool = ...): ...
     def indexer_between_time(
         self, start_time, end_time, include_start: bool = ..., include_end: bool = ...
     ): ...
     def to_perioddelta(self, freq) -> TimedeltaIndex: ...
-    def to_julian_date(self) -> Float64Index: ...
+    def to_julian_date(self) -> _FloatIndexType: ...
     def isocalendar(self) -> DataFrame: ...
     @property
     def tzinfo(self) -> tzinfo | None: ...
     @property
     def dtype(self) -> np.dtype | DatetimeTZDtype: ...
 
 def date_range(
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/interval.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/interval.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,18 @@
     Literal,
     overload,
 )
 
 import numpy as np
 import pandas as pd
 from pandas import Index
+from pandas.core.indexes.base import (
+    _FloatIndexType,
+    _IntIndexType,
+)
 from pandas.core.indexes.extension import ExtensionIndex
 from pandas.core.series import (
     Series,
     TimedeltaSeries,
     TimestampSeries,
 )
 from typing_extensions import TypeAlias
@@ -42,18 +46,18 @@
 
 _EdgesInt: TypeAlias = (
     Sequence[int]
     | npt.NDArray[np.int64]
     | npt.NDArray[np.int32]
     | npt.NDArray[np.intp]
     | pd.Series[int]
-    | pd.Int64Index
+    | _IntIndexType
 )
 _EdgesFloat: TypeAlias = (
-    Sequence[float] | npt.NDArray[np.float64] | pd.Series[float] | pd.Float64Index
+    Sequence[float] | npt.NDArray[np.float64] | pd.Series[float] | _FloatIndexType
 )
 _EdgesTimestamp: TypeAlias = (
     Sequence[DatetimeLike]
     | npt.NDArray[np.datetime64]
     | TimestampSeries
     | pd.DatetimeIndex
 )
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/multi.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/multi.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import numpy as np
 import pandas as pd
 from pandas.core.indexes.base import Index
 from typing_extensions import Self
 
 from pandas._typing import (
     T1,
+    Dtype,
     DtypeArg,
     HashableT,
     np_ndarray_anyint,
     np_ndarray_bool,
 )
 
 class MultiIndex(Index):
@@ -64,14 +65,16 @@
     def set_codes(self, codes, *, level=..., verify_integrity: bool = ...): ...
     def copy(self, names=..., deep: bool = ...) -> MultiIndex: ...
     def __array__(self, dtype=...) -> np.ndarray: ...
     def view(self, cls=...): ...
     def __contains__(self, key) -> bool: ...
     @property
     def dtype(self) -> np.dtype: ...
+    @property
+    def dtypes(self) -> pd.Series[Dtype]: ...
     def memory_usage(self, deep: bool = ...) -> int: ...
     @property
     def nbytes(self) -> int: ...
     def format(
         self,
         name: bool | None = ...,
         formatter: Callable | None = ...,
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/period.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/period.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/range.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/range.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from collections.abc import Sequence
 from typing import overload
 
 import numpy as np
 from pandas import Series
-from pandas.core.indexes.base import Index
-from pandas.core.indexes.numeric import Int64Index
+from pandas.core.indexes.base import (
+    Index,
+    _IntIndexType,
+)
 
 from pandas._typing import (
     HashableT,
     np_ndarray_anyint,
     np_ndarray_bool,
     npt,
 )
 
-class RangeIndex(Int64Index):
+class RangeIndex(_IntIndexType):
     def __new__(
         cls,
         start: int | RangeIndex = ...,
         stop: int = ...,
         step: int = ...,
         dtype=...,
         copy: bool = ...,
@@ -77,15 +79,15 @@
     @property
     def size(self) -> int: ...
     def __floordiv__(self, other): ...
     def all(self) -> bool: ...
     def any(self) -> bool: ...
     def union(
         self, other: list[HashableT] | Index, sort=...
-    ) -> Index | Int64Index | RangeIndex: ...
+    ) -> Index | _IntIndexType | RangeIndex: ...
     @overload  # type: ignore[override]
     def __getitem__(
         self,
         idx: slice
         | np_ndarray_anyint
         | Sequence[int]
         | Index
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/indexes/timedeltas.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexes/timedeltas.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/indexing.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/indexing.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/interchange/dataframe_protocol.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/interchange/dataframe_protocol.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/ops/array_ops.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/array_ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/ops/mask_ops.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/ops/mask_ops.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/resample.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/resample.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/api.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/concat.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/concat.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,43 +25,43 @@
 @overload
 def concat(
     objs: Iterable[DataFrame] | Mapping[HashableT1, DataFrame],
     *,
     axis: AxisIndex = ...,
     join: Literal["inner", "outer"] = ...,
     ignore_index: bool = ...,
-    keys: list[HashableT2] = ...,
+    keys: Iterable[HashableT2] = ...,
     levels: Sequence[list[HashableT3] | tuple[HashableT3, ...]] = ...,
     names: list[HashableT4] = ...,
     verify_integrity: bool = ...,
     sort: bool = ...,
     copy: bool = ...,
 ) -> DataFrame: ...
 @overload
 def concat(
     objs: Iterable[Series] | Mapping[HashableT1, Series],
     *,
     axis: AxisIndex = ...,
     join: Literal["inner", "outer"] = ...,
     ignore_index: bool = ...,
-    keys: list[HashableT2] = ...,
+    keys: Iterable[HashableT2] = ...,
     levels: Sequence[list[HashableT3] | tuple[HashableT3, ...]] = ...,
     names: list[HashableT4] = ...,
     verify_integrity: bool = ...,
     sort: bool = ...,
     copy: bool = ...,
 ) -> Series: ...
 @overload
 def concat(
     objs: Iterable[Series | DataFrame] | Mapping[HashableT1, Series | DataFrame],
     *,
     axis: AxisColumn,
     join: Literal["inner", "outer"] = ...,
     ignore_index: bool = ...,
-    keys: list[HashableT2] = ...,
+    keys: Iterable[HashableT2] = ...,
     levels: Sequence[list[HashableT3] | tuple[HashableT3, ...]] = ...,
     names: list[HashableT4] = ...,
     verify_integrity: bool = ...,
     sort: bool = ...,
     copy: bool = ...,
 ) -> DataFrame: ...
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/encoding.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/encoding.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/melt.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/melt.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/merge.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/merge.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/pivot.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/pivot.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/reshape/tile.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/reshape/tile.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -5,33 +5,40 @@
 )
 
 import numpy as np
 from pandas import (
     Categorical,
     CategoricalDtype,
     DatetimeIndex,
-    Float64Index,
     Index,
-    Int64Index,
     Interval,
     IntervalIndex,
     Series,
     Timestamp,
 )
+from pandas.core.indexes.base import (
+    _FloatIndexType,
+    _IntIndexType,
+)
 from pandas.core.series import TimestampSeries
 
 from pandas._typing import (
     Label,
     npt,
 )
 
 @overload
 def cut(
     x: Index | npt.NDArray | Sequence[int] | Sequence[float],
-    bins: int | Series | Int64Index | Float64Index | Sequence[int] | Sequence[float],
+    bins: int
+    | Series
+    | _IntIndexType
+    | _FloatIndexType
+    | Sequence[int]
+    | Sequence[float],
     right: bool = ...,
     *,
     labels: Literal[False],
     retbins: Literal[True],
     precision: int = ...,
     include_lowest: bool = ...,
     duplicates: Literal["raise", "drop"] = ...,
@@ -79,15 +86,20 @@
     include_lowest: bool = ...,
     duplicates: Literal["raise", "drop"] = ...,
     ordered: bool = ...,
 ) -> tuple[Series, DatetimeIndex]: ...
 @overload
 def cut(
     x: Series,
-    bins: int | Series | Int64Index | Float64Index | Sequence[int] | Sequence[float],
+    bins: int
+    | Series
+    | _IntIndexType
+    | _FloatIndexType
+    | Sequence[int]
+    | Sequence[float],
     right: bool = ...,
     labels: Literal[False] | Sequence[Label] | None = ...,
     *,
     retbins: Literal[True],
     precision: int = ...,
     include_lowest: bool = ...,
     duplicates: Literal["raise", "drop"] = ...,
@@ -105,15 +117,20 @@
     include_lowest: bool = ...,
     duplicates: Literal["raise", "drop"] = ...,
     ordered: bool = ...,
 ) -> tuple[Series, IntervalIndex]: ...
 @overload
 def cut(
     x: Index | npt.NDArray | Sequence[int] | Sequence[float],
-    bins: int | Series | Int64Index | Float64Index | Sequence[int] | Sequence[float],
+    bins: int
+    | Series
+    | _IntIndexType
+    | _FloatIndexType
+    | Sequence[int]
+    | Sequence[float],
     right: bool = ...,
     labels: Sequence[Label] | None = ...,
     *,
     retbins: Literal[True],
     precision: int = ...,
     include_lowest: bool = ...,
     duplicates: Literal["raise", "drop"] = ...,
@@ -133,16 +150,16 @@
     ordered: bool = ...,
 ) -> tuple[Categorical, IntervalIndex]: ...
 @overload
 def cut(
     x: Index | npt.NDArray | Sequence[int] | Sequence[float],
     bins: int
     | Series
-    | Int64Index
-    | Float64Index
+    | _IntIndexType
+    | _FloatIndexType
     | Sequence[int]
     | Sequence[float]
     | IntervalIndex,
     right: bool = ...,
     *,
     labels: Literal[False],
     retbins: Literal[False] = ...,
@@ -169,16 +186,16 @@
     ordered: bool = ...,
 ) -> Series[CategoricalDtype]: ...
 @overload
 def cut(
     x: Series,
     bins: int
     | Series
-    | Int64Index
-    | Float64Index
+    | _IntIndexType
+    | _FloatIndexType
     | Sequence[int]
     | Sequence[float]
     | IntervalIndex,
     right: bool = ...,
     labels: Literal[False] | Sequence[Label] | None = ...,
     retbins: Literal[False] = ...,
     precision: int = ...,
@@ -187,78 +204,78 @@
     ordered: bool = ...,
 ) -> Series: ...
 @overload
 def cut(
     x: Index | npt.NDArray | Sequence[int] | Sequence[float],
     bins: int
     | Series
-    | Int64Index
-    | Float64Index
+    | _IntIndexType
+    | _FloatIndexType
     | Sequence[int]
     | Sequence[float]
     | IntervalIndex,
     right: bool = ...,
     labels: Sequence[Label] | None = ...,
     retbins: Literal[False] = ...,
     precision: int = ...,
     include_lowest: bool = ...,
     duplicates: Literal["raise", "drop"] = ...,
     ordered: bool = ...,
 ) -> Categorical: ...
 @overload
 def qcut(
     x: Index | npt.NDArray | Sequence[int] | Sequence[float],
-    q: int | Sequence[float] | Series[float] | Float64Index | npt.NDArray,
+    q: int | Sequence[float] | Series[float] | _FloatIndexType | npt.NDArray,
     *,
     labels: Literal[False],
     retbins: Literal[False] = ...,
     precision: int = ...,
     duplicates: Literal["raise", "drop"] = ...,
 ) -> npt.NDArray[np.intp]: ...
 @overload
 def qcut(
     x: Index | npt.NDArray | Sequence[int] | Sequence[float],
-    q: int | Sequence[float] | Series[float] | Float64Index | npt.NDArray,
+    q: int | Sequence[float] | Series[float] | _FloatIndexType | npt.NDArray,
     labels: Sequence[Label] | None = ...,
     retbins: Literal[False] = ...,
     precision: int = ...,
     duplicates: Literal["raise", "drop"] = ...,
 ) -> Categorical: ...
 @overload
 def qcut(
     x: Series,
-    q: int | Sequence[float] | Series[float] | Float64Index | npt.NDArray,
+    q: int | Sequence[float] | Series[float] | _FloatIndexType | npt.NDArray,
     labels: Literal[False] | Sequence[Label] | None = ...,
     retbins: Literal[False] = ...,
     precision: int = ...,
     duplicates: Literal["raise", "drop"] = ...,
 ) -> Series: ...
 @overload
 def qcut(
     x: Index | npt.NDArray | Sequence[int] | Sequence[float],
-    q: int | Sequence[float] | Series[float] | Float64Index | npt.NDArray,
+    q: int | Sequence[float] | Series[float] | _FloatIndexType | npt.NDArray,
     *,
     labels: Literal[False],
     retbins: Literal[True],
     precision: int = ...,
     duplicates: Literal["raise", "drop"] = ...,
 ) -> tuple[npt.NDArray[np.intp], npt.NDArray[np.float_]]: ...
 @overload
 def qcut(
     x: Series,
-    q: int | Sequence[float] | Series[float] | Float64Index | npt.NDArray,
+    q: int | Sequence[float] | Series[float] | _FloatIndexType | npt.NDArray,
     labels: Literal[False] | Sequence[Label] | None = ...,
     *,
     retbins: Literal[True],
     precision: int = ...,
     duplicates: Literal["raise", "drop"] = ...,
 ) -> tuple[Series, npt.NDArray[np.float_]]: ...
 @overload
 def qcut(
     x: Index | npt.NDArray | Sequence[int] | Sequence[float],
-    q: int | Sequence[float] | Series[float] | Float64Index | npt.NDArray,
+    q: int | Sequence[float] | Series[float] | _FloatIndexType | npt.NDArray,
     labels: Sequence[Label] | None = ...,
     *,
     retbins: Literal[True],
     precision: int = ...,
     duplicates: Literal["raise", "drop"] = ...,
 ) -> tuple[Categorical, npt.NDArray[np.float_]]: ...
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/series.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/series.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,18 @@
     ExponentialMovingWindow,
     Rolling,
 )
 from pandas.core.window.rolling import (
     Rolling,
     Window,
 )
-from typing_extensions import TypeAlias
+from typing_extensions import (
+    Never,
+    TypeAlias,
+)
 import xarray as xr
 
 from pandas._libs.interval import Interval
 from pandas._libs.missing import NAType
 from pandas._libs.tslibs import BaseOffset
 from pandas._typing import (
     S1,
@@ -757,15 +760,15 @@
         axis: AxisIndex = ...,
         *args,
         **kwargs,
     ) -> DataFrame: ...
     @overload
     def apply(
         self,
-        func: Callable[..., Scalar | Sequence | Mapping],
+        func: Callable[..., Scalar | Sequence | set | Mapping],
         convertDType: _bool = ...,
         args: tuple = ...,
         **kwds,
     ) -> Series: ...
     @overload
     def apply(
         self,
@@ -1014,19 +1017,19 @@
     ) -> SubplotBase: ...
     def swapaxes(
         self, axis1: AxisIndex, axis2: AxisIndex, copy: _bool = ...
     ) -> Series[S1]: ...
     def droplevel(
         self, level: Level | list[Level], axis: AxisIndex = ...
     ) -> DataFrame: ...
-    def pop(self, item: _str) -> Series[S1]: ...
+    def pop(self, item: Hashable) -> S1: ...
     def squeeze(self, axis: AxisIndex | None = ...) -> Scalar: ...
     def __abs__(self) -> Series[S1]: ...
-    def add_prefix(self, prefix: _str) -> Series[S1]: ...
-    def add_suffix(self, suffix: _str) -> Series[S1]: ...
+    def add_prefix(self, prefix: _str, axis: AxisIndex | None = ...) -> Series[S1]: ...
+    def add_suffix(self, suffix: _str, axis: AxisIndex | None = ...) -> Series[S1]: ...
     def reindex(
         self,
         index: Axes | None = ...,
         method: FillnaOptions | Literal["nearest"] | None = ...,
         copy: bool = ...,
         level: int | _str = ...,
         fill_value: Scalar | None = ...,
@@ -1439,24 +1442,14 @@
     @overload
     def __rxor__(self, other: int | np_ndarray_anyint | Series[int]) -> Series[int]: ...  # type: ignore[misc]
     @overload
     def __sub__(
         self, other: Timestamp | datetime | TimestampSeries
     ) -> TimedeltaSeries: ...
     @overload
-    def __sub__(
-        self: Series[Timestamp],
-        other: Timedelta | TimedeltaSeries | TimedeltaIndex | np.timedelta64,
-    ) -> TimestampSeries: ...
-    @overload
-    def __sub__(
-        self: Series[Timedelta],
-        other: Timedelta | TimedeltaSeries | TimedeltaIndex | np.timedelta64,
-    ) -> TimedeltaSeries: ...
-    @overload
     def __sub__(self, other: num | _ListLike | Series) -> Series: ...
     def __truediv__(self, other: num | _ListLike | Series[S1]) -> Series: ...
     # ignore needed for mypy as we want different results based on the arguments
     @overload  # type: ignore[override]
     def __xor__(  # type: ignore[misc]
         self, other: bool | list[bool] | list[int] | np_ndarray_bool | Series[bool]
     ) -> Series[bool]: ...
@@ -1612,15 +1605,15 @@
     def mean(
         self,
         axis: AxisIndex | None = ...,
         skipna: _bool = ...,
         level: None = ...,
         numeric_only: _bool = ...,
         **kwargs,
-    ) -> float: ...
+    ) -> np.float64: ...
     def median(
         self,
         axis: AxisIndex | None = ...,
         skipna: _bool = ...,
         level: None = ...,
         numeric_only: _bool = ...,
         **kwargs,
@@ -1807,14 +1800,38 @@
     def subtract(
         self,
         other: num | _ListLike | Series[S1],
         level: Level | None = ...,
         fill_value: float | None = ...,
         axis: AxisIndex | None = ...,
     ) -> Series[S1]: ...
+    # ignore needed because of mypy, for using `Never` as type-var.
+    @overload
+    def sum(
+        self: Series[Never],  # type: ignore[type-var]
+        axis: AxisIndex | None = ...,
+        skipna: _bool | None = ...,
+        level: None = ...,
+        numeric_only: _bool = ...,
+        min_count: int = ...,
+        **kwargs,
+    ) -> Any: ...
+    # ignore needed because of mypy, for overlapping overloads
+    # between `Series[bool]` and `Series[int]`.
+    @overload
+    def sum(  # type: ignore[misc]
+        self: Series[bool],
+        axis: AxisIndex | None = ...,
+        skipna: _bool | None = ...,
+        level: None = ...,
+        numeric_only: _bool = ...,
+        min_count: int = ...,
+        **kwargs,
+    ) -> int: ...
+    @overload
     def sum(
         self: Series[S1],
         axis: AxisIndex | None = ...,
         skipna: _bool | None = ...,
         level: None = ...,
         numeric_only: _bool = ...,
         min_count: int = ...,
@@ -1873,14 +1890,23 @@
 
 class TimestampSeries(Series[Timestamp]):
     # ignore needed because of mypy
     @property
     def dt(self) -> TimestampProperties: ...  # type: ignore[override]
     def __add__(self, other: TimedeltaSeries | np.timedelta64) -> TimestampSeries: ...  # type: ignore[override]
     def __radd__(self, other: TimedeltaSeries | np.timedelta64) -> TimestampSeries: ...  # type: ignore[override]
+    @overload  # type: ignore[override]
+    def __sub__(
+        self, other: Timestamp | datetime | TimestampSeries
+    ) -> TimedeltaSeries: ...
+    @overload
+    def __sub__(
+        self,
+        other: Timedelta | TimedeltaSeries | TimedeltaIndex | np.timedelta64,
+    ) -> TimestampSeries: ...
     def __mul__(self, other: float | Series[int] | Series[float] | Sequence[float]) -> TimestampSeries: ...  # type: ignore[override]
     def __truediv__(self, other: float | Series[int] | Series[float] | Sequence[float]) -> TimestampSeries: ...  # type: ignore[override]
     def mean(  # type: ignore[override]
         self,
         axis: AxisIndex | None = ...,
         skipna: _bool = ...,
         level: None = ...,
@@ -1915,15 +1941,15 @@
     ) -> TimestampSeries: ...
     @overload
     def __add__(self, other: Timedelta | np.timedelta64) -> TimedeltaSeries: ...
     def __radd__(self, other: Timestamp | TimestampSeries) -> TimestampSeries: ...  # type: ignore[override]
     def __mul__(  # type: ignore[override]
         self, other: num | Sequence[num] | Series[int] | Series[float]
     ) -> TimedeltaSeries: ...
-    def __sub__(
+    def __sub__(  # type: ignore[override]
         self, other: Timedelta | TimedeltaSeries | TimedeltaIndex | np.timedelta64
     ) -> TimedeltaSeries: ...
     def __truediv__(self, other: Timedelta | TimedeltaSeries | np.timedelta64 | TimedeltaIndex) -> Series[float]: ...  # type: ignore[override]
     @property
     def dt(self) -> TimedeltaProperties: ...  # type: ignore[override]
     def mean(  # type: ignore[override]
         self,
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/strings.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/strings.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/tools/datetimes.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/tools/datetimes.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/tools/numeric.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/tools/numeric.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/tools/timedeltas.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/tools/timedeltas.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/window/ewm.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/window/ewm.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/window/expanding.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/window/expanding.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/core/window/rolling.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/core/window/rolling.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/errors/__init__.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/errors/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/api.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/api.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/clipboards.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/clipboards.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -7,43 +7,36 @@
 from typing import (
     Any,
     Literal,
     overload,
 )
 
 from pandas.core.frame import DataFrame
-from pandas.core.indexes.base import Index
-from pandas.core.series import Series
 
 from pandas._typing import (
     CompressionOptions,
     CSVEngine,
     CSVQuoting,
     DtypeArg,
+    ListLikeHashable,
     StorageOptions,
-    npt,
+    UsecolsArgType,
 )
 
 from pandas.io.parsers import TextFileReader
 
 @overload
 def read_clipboard(
     sep: str | None = ...,
     *,
     delimiter: str | None = ...,
     header: int | Sequence[int] | Literal["infer"] | None = ...,
-    names: list[str] = ...,
+    names: ListLikeHashable | None = ...,
     index_col: int | str | Sequence[str | int] | Literal[False] | None = ...,
-    usecols: list[str]
-    | Sequence[int]
-    | Series
-    | Index
-    | npt.NDArray
-    | Callable[[str], bool]
-    | None = ...,
+    usecols: UsecolsArgType = ...,
     dtype: DtypeArg | defaultdict | None = ...,
     engine: CSVEngine | None = ...,
     converters: dict[int | str, Callable[[str], Any]] = ...,
     true_values: list[str] = ...,
     false_values: list[str] = ...,
     skipinitialspace: bool = ...,
     skiprows: int | Sequence[int] | Callable[[int], bool] = ...,
@@ -90,23 +83,17 @@
 ) -> TextFileReader: ...
 @overload
 def read_clipboard(
     sep: str | None = ...,
     *,
     delimiter: str | None = ...,
     header: int | Sequence[int] | Literal["infer"] | None = ...,
-    names: list[str] = ...,
+    names: ListLikeHashable | None = ...,
     index_col: int | str | Sequence[str | int] | Literal[False] | None = ...,
-    usecols: list[str]
-    | Sequence[int]
-    | Series
-    | Index
-    | npt.NDArray
-    | Callable[[str], bool]
-    | None = ...,
+    usecols: UsecolsArgType = ...,
     dtype: DtypeArg | defaultdict | None = ...,
     engine: CSVEngine | None = ...,
     converters: dict[int | str, Callable[[str], Any]] = ...,
     true_values: list[str] = ...,
     false_values: list[str] = ...,
     skipinitialspace: bool = ...,
     skiprows: int | Sequence[int] | Callable[[int], bool] = ...,
@@ -153,23 +140,17 @@
 ) -> TextFileReader: ...
 @overload
 def read_clipboard(
     sep: str | None = ...,
     *,
     delimiter: str | None = ...,
     header: int | Sequence[int] | Literal["infer"] | None = ...,
-    names: list[str] = ...,
+    names: ListLikeHashable | None = ...,
     index_col: int | str | Sequence[str | int] | Literal[False] | None = ...,
-    usecols: list[str]
-    | Sequence[int]
-    | Series
-    | Index
-    | npt.NDArray
-    | Callable[[str], bool]
-    | None = ...,
+    usecols: UsecolsArgType = ...,
     dtype: DtypeArg | defaultdict | None = ...,
     engine: CSVEngine | None = ...,
     converters: dict[int | str, Callable[[str], Any]] = ...,
     true_values: list[str] = ...,
     false_values: list[str] = ...,
     skipinitialspace: bool = ...,
     skiprows: int | Sequence[int] | Callable[[int], bool] = ...,
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/excel/_base.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/excel/_base.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 import pyxlsb.workbook
 from typing_extensions import Self
 from xlrd.book import Book
 
 from pandas._typing import (
     Dtype,
     FilePath,
+    ListLikeHashable,
     ReadBuffer,
     StorageOptions,
+    UsecolsArgType,
     WriteExcelBuffer,
 )
 
 @overload
 def read_excel(
     io: FilePath
     | ReadBuffer[bytes]
@@ -36,17 +38,17 @@
     | Workbook
     | Book
     | OpenDocument
     | pyxlsb.workbook.Workbook,
     sheet_name: list[int | str] | None,
     *,
     header: int | Sequence[int] | None = ...,
-    names: list[str] | None = ...,
+    names: ListLikeHashable | None = ...,
     index_col: int | Sequence[int] | None = ...,
-    usecols: Sequence[int] | Sequence[str] | Callable[[str], bool] | None = ...,
+    usecols: str | UsecolsArgType = ...,
     dtype: str | Dtype | Mapping[str, str | Dtype] | None = ...,
     engine: Literal["xlrd", "openpyxl", "odf", "pyxlsb"] | None = ...,
     converters: Mapping[int | str, Callable[[object], object]] | None = ...,
     true_values: Iterable[Hashable] | None = ...,
     false_values: Iterable[Hashable] | None = ...,
     skiprows: int | Sequence[int] | Callable[[object], bool] | None = ...,
     nrows: int | None = ...,
@@ -74,17 +76,17 @@
     | Workbook
     | Book
     | OpenDocument
     | pyxlsb.workbook.Workbook,
     sheet_name: int | str = ...,
     *,
     header: int | Sequence[int] | None = ...,
-    names: list[str] | None = ...,
+    names: ListLikeHashable | None = ...,
     index_col: int | Sequence[int] | None = ...,
-    usecols: Sequence[int] | Sequence[str] | Callable[[str], bool] | None = ...,
+    usecols: str | UsecolsArgType = ...,
     dtype: str | Dtype | Mapping[str, str | Dtype] | None = ...,
     engine: Literal["xlrd", "openpyxl", "odf", "pyxlsb"] | None = ...,
     converters: Mapping[int | str, Callable[[object], object]] | None = ...,
     true_values: Iterable[Hashable] | None = ...,
     false_values: Iterable[Hashable] | None = ...,
     skiprows: int | Sequence[int] | Callable[[object], bool] | None = ...,
     nrows: int | None = ...,
@@ -151,21 +153,17 @@
     ) -> None: ...
     def __fspath__(self): ...
     @overload
     def parse(
         self,
         sheet_name: list[int | str] | None,
         header: int | Sequence[int] | None = ...,
-        names: list[str] | None = ...,
+        names: ListLikeHashable | None = ...,
         index_col: int | Sequence[int] | None = ...,
-        usecols: str
-        | Sequence[int]
-        | Sequence[str]
-        | Callable[[str], bool]
-        | None = ...,
+        usecols: str | UsecolsArgType = ...,
         converters: dict[int | str, Callable[[object], object]] | None = ...,
         true_values: Iterable[Hashable] | None = ...,
         false_values: Iterable[Hashable] | None = ...,
         skiprows: int | Sequence[int] | Callable[[object], bool] | None = ...,
         nrows: int | None = ...,
         na_values: Sequence[str] | dict[str | int, Sequence[str]] = ...,
         parse_dates: bool
@@ -181,21 +179,17 @@
         **kwds: Any,
     ) -> dict[int | str, DataFrame]: ...
     @overload
     def parse(
         self,
         sheet_name: int | str,
         header: int | Sequence[int] | None = ...,
-        names: list[str] | None = ...,
+        names: ListLikeHashable | None = ...,
         index_col: int | Sequence[int] | None = ...,
-        usecols: str
-        | Sequence[int]
-        | Sequence[str]
-        | Callable[[str], bool]
-        | None = ...,
+        usecols: str | UsecolsArgType = ...,
         converters: dict[int | str, Callable[[object], object]] | None = ...,
         true_values: Iterable[Hashable] | None = ...,
         false_values: Iterable[Hashable] | None = ...,
         skiprows: int | Sequence[int] | Callable[[object], bool] | None = ...,
         nrows: int | None = ...,
         na_values: Sequence[str] | dict[str | int, Sequence[str]] = ...,
         parse_dates: bool
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/formats/style.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/formats/style.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/formats/style_render.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/formats/style_render.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/gbq.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/gbq.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/html.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/html.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/json/_json.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/json/_json.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/parsers/readers.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/parsers/readers.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -12,48 +12,40 @@
 from typing import (
     Any,
     Literal,
     overload,
 )
 
 from pandas.core.frame import DataFrame
-from pandas.core.indexes.base import Index
-from pandas.core.series import Series
 from typing_extensions import Self
 
 from pandas._typing import (
     CompressionOptions,
     CSVEngine,
     CSVQuoting,
     DtypeArg,
     FilePath,
+    ListLikeHashable,
     ReadCsvBuffer,
     StorageOptions,
-    npt,
+    UsecolsArgType,
 )
 
 from pandas.io.common import IOHandles
 
 @overload
 def read_csv(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     sep: str | None = ...,
     delimiter: str | None = ...,
     header: int | Sequence[int] | Literal["infer"] | None = ...,
-    names: list[str] | None = ...,
+    names: ListLikeHashable | None = ...,
     index_col: int | str | Sequence[str | int] | Literal[False] | None = ...,
-    usecols: list[str]
-    | tuple[str, ...]
-    | Sequence[int]
-    | Series
-    | Index
-    | npt.NDArray
-    | Callable[[str], bool]
-    | None = ...,
+    usecols: UsecolsArgType = ...,
     dtype: DtypeArg | defaultdict | None = ...,
     engine: CSVEngine | None = ...,
     converters: Mapping[int | str, Callable[[str], Any]]
     | Mapping[int, Callable[[str], Any]]
     | Mapping[str, Callable[[str], Any]]
     | None = ...,
     true_values: list[str] = ...,
@@ -102,24 +94,17 @@
 @overload
 def read_csv(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     sep: str | None = ...,
     delimiter: str | None = ...,
     header: int | Sequence[int] | Literal["infer"] | None = ...,
-    names: list[str] | None = ...,
+    names: ListLikeHashable | None = ...,
     index_col: int | str | Sequence[str | int] | Literal[False] | None = ...,
-    usecols: list[str]
-    | tuple[str, ...]
-    | Sequence[int]
-    | Series
-    | Index
-    | npt.NDArray
-    | Callable[[str], bool]
-    | None = ...,
+    usecols: UsecolsArgType = ...,
     dtype: DtypeArg | defaultdict | None = ...,
     engine: CSVEngine | None = ...,
     converters: Mapping[int | str, Callable[[str], Any]]
     | Mapping[int, Callable[[str], Any]]
     | Mapping[str, Callable[[str], Any]]
     | None = ...,
     true_values: list[str] = ...,
@@ -168,24 +153,17 @@
 @overload
 def read_csv(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     sep: str | None = ...,
     delimiter: str | None = ...,
     header: int | Sequence[int] | Literal["infer"] | None = ...,
-    names: list[str] | None = ...,
+    names: ListLikeHashable | None = ...,
     index_col: int | str | Sequence[str | int] | Literal[False] | None = ...,
-    usecols: list[str]
-    | tuple[str, ...]
-    | Sequence[int]
-    | Series
-    | Index
-    | npt.NDArray
-    | Callable[[str], bool]
-    | None = ...,
+    usecols: UsecolsArgType = ...,
     dtype: DtypeArg | defaultdict | None = ...,
     engine: CSVEngine | None = ...,
     converters: Mapping[int | str, Callable[[str], Any]]
     | Mapping[int, Callable[[str], Any]]
     | Mapping[str, Callable[[str], Any]]
     | None = ...,
     true_values: list[str] = ...,
@@ -234,24 +212,17 @@
 @overload
 def read_table(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     sep: str | None = ...,
     delimiter: str | None = ...,
     header: int | Sequence[int] | Literal["infer"] | None = ...,
-    names: list[str] | None = ...,
+    names: ListLikeHashable | None = ...,
     index_col: int | str | Sequence[str | int] | Literal[False] | None = ...,
-    usecols: list[str]
-    | tuple[str, ...]
-    | Sequence[int]
-    | Series
-    | Index
-    | npt.NDArray
-    | Callable[[str], bool]
-    | None = ...,
+    usecols: UsecolsArgType = ...,
     dtype: DtypeArg | defaultdict | None = ...,
     engine: CSVEngine | None = ...,
     converters: Mapping[int | str, Callable[[str], Any]]
     | Mapping[int, Callable[[str], Any]]
     | Mapping[str, Callable[[str], Any]]
     | None = ...,
     true_values: list[str] = ...,
@@ -300,24 +271,17 @@
 @overload
 def read_table(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     sep: str | None = ...,
     delimiter: str | None = ...,
     header: int | Sequence[int] | Literal["infer"] | None = ...,
-    names: list[str] | None = ...,
+    names: ListLikeHashable | None = ...,
     index_col: int | str | Sequence[str | int] | Literal[False] | None = ...,
-    usecols: list[str]
-    | tuple[str, ...]
-    | Sequence[int]
-    | Series
-    | Index
-    | npt.NDArray
-    | Callable[[str], bool]
-    | None = ...,
+    usecols: UsecolsArgType = ...,
     dtype: DtypeArg | defaultdict | None = ...,
     engine: CSVEngine | None = ...,
     converters: Mapping[int | str, Callable[[str], Any]]
     | Mapping[int, Callable[[str], Any]]
     | Mapping[str, Callable[[str], Any]]
     | None = ...,
     true_values: list[str] = ...,
@@ -366,24 +330,17 @@
 @overload
 def read_table(
     filepath_or_buffer: FilePath | ReadCsvBuffer[bytes] | ReadCsvBuffer[str],
     *,
     sep: str | None = ...,
     delimiter: str | None = ...,
     header: int | Sequence[int] | Literal["infer"] | None = ...,
-    names: list[str] | None = ...,
+    names: ListLikeHashable | None = ...,
     index_col: int | str | Sequence[str | int] | Literal[False] | None = ...,
-    usecols: list[str]
-    | tuple[str, ...]
-    | Sequence[int]
-    | Series
-    | Index
-    | npt.NDArray
-    | Callable[[str], bool]
-    | None = ...,
+    usecols: UsecolsArgType = ...,
     dtype: DtypeArg | defaultdict | None = ...,
     engine: CSVEngine | None = ...,
     converters: Mapping[int | str, Callable[[str], Any]]
     | Mapping[int, Callable[[str], Any]]
     | Mapping[str, Callable[[str], Any]]
     | None = ...,
     true_values: list[str] = ...,
```

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/pickle.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/pickle.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/pytables.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/pytables.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/sas/sasreader.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/sas/sasreader.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/sql.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/sql.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/stata.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/stata.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/io/xml.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/io/xml.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/plotting/__init__.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/plotting/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/plotting/_core.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/plotting/_core.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/plotting/_misc.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/plotting/_misc.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/tseries/offsets.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/tseries/offsets.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/util/_decorators.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/util/_decorators.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/util/_validators.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/util/_validators.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pandas-stubs/util/version/__init__.pyi` & `pandas_stubs-2.0.0.230412/pandas-stubs/util/version/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pandas_stubs-1.5.3.230321/pyproject.toml` & `pandas_stubs-2.0.0.230412/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandas-stubs"
-version = "1.5.3.230321"
+version = "2.0.0.230412"
 description = "Type annotations for pandas"
 authors = ["The Pandas Development Team <pandas-dev@python.org>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://pandas.pydata.org"
 repository = "https://github.com/pandas-dev/pandas-stubs"
 classifiers = [
@@ -27,33 +27,33 @@
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/pandas-dev/pandas-stubs/issues"
 "Documentation" = "https://pandas.pydata.org/pandas-docs/stable"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.8"
 types-pytz = ">= 2022.1.1"
 
 [tool.poetry.dev-dependencies]
-mypy = "1.0"
+mypy = "1.2.0"
 pyarrow = ">=10.0.1"
 pytest = ">=7.1.2"
-pyright = "1.1.298"
+pyright = ">= 1.1.300"
 poethepoet = ">=0.16.5"
 loguru = ">=0.6.0"
-pandas = "1.5.3"
+pandas = "2.0.0"
 numpy = ">=1.24.1"
 typing-extensions = ">=4.4.0"
 matplotlib = ">=3.5.1"
 pre-commit = ">=2.19.0"
-black = ">=22.12.0"
-isort = ">=5.10.1"
+black = ">=23.3.0"
+isort = ">=5.12.0"
 openpyxl = ">=3.0.10"
-tables = { version = ">=3.7.0" }
+tables = { version = ">=3.7.0" , python = "<4"}  # 3.8.0 depends on blosc2 which caps python to <4
 lxml = { version = ">=4.7.1,<4.9.0", python = "<3.11" }
 pyreadstat = ">=1.2.0"
 xlrd = ">=2.0.1"
 xlsxwriter = ">=3.0.3"
 pyxlsb = ">=1.0.10"
 odfpy = ">=1.4.1"
 xarray = ">=22.6.0"
```

### Comparing `pandas_stubs-1.5.3.230321/README.md` & `pandas_stubs-2.0.0.230412/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ## What is it?
 
 These are public type stubs for [**pandas**](http://pandas.pydata.org/), following the
 convention of providing stubs in a separate package, as specified in [PEP 561](https://peps.python.org/pep-0561/#stub-only-packages).  The stubs cover the most typical use cases of
 pandas.  In general, these stubs are narrower than what is possibly allowed by pandas,
 but follow a convention of suggesting best recommended practices for using pandas.
 
-The stubs are likely incomplete in terms of covering the published API of pandas.
+The stubs are likely incomplete in terms of covering the published API of pandas.  NOTE: The current 2.0.x releases of pandas-stubs do not support all of the new features of pandas 2.0.  See this [tracker](https://github.com/pandas-dev/pandas-stubs/issues/624) to understand the current compatibility with version 2.0.
 
 The stubs are tested with [mypy](http://mypy-lang.org/) and [pyright](https://github.com/microsoft/pyright#readme) and are currently shipped with the Visual Studio Code extension
 [pylance](https://github.com/microsoft/pylance-release#readme).
 
 ## Usage
 
 Let’s take this example piece of code in file `round.py`
@@ -133,26 +133,25 @@
 
 ## Documentation
 
 Documentation is a work-in-progress.  
 
 ## Background
 
-These stubs are the result of a strategic effort lead by the core pandas team to integrate [Microsoft type stub repository](https://github.com/microsoft/python-type-stubs)
-together with the [VirtusLabs pandas_stubs repository](https://github.com/VirtusLab/pandas-stubs).
+These stubs are the result of a strategic effort led by the core pandas team to integrate [Microsoft type stub repository](https://github.com/microsoft/python-type-stubs) with the [VirtusLabs pandas_stubs repository](https://github.com/VirtusLab/pandas-stubs).
 
-These stubs were initially forked from the Microsoft project <https://github.com/microsoft/python-type-stubs> as of [this commit](https://github.com/microsoft/python-type-stubs/tree/6b800063bde687cd1846122431e2a729a9de625a).
+These stubs were initially forked from the Microsoft project at <https://github.com/microsoft/python-type-stubs> as of [this commit](https://github.com/microsoft/python-type-stubs/tree/6b800063bde687cd1846122431e2a729a9de625a).
 
-We are indebted to Microsoft and that project for the initial set of public type stubs.  We are also grateful for the original pandas-stubs project at <https://github.com/VirtusLab/pandas-stubs> that created the framework for testing the stubs.
+We are indebted to Microsoft and that project for providing the initial set of public type stubs.  We are also grateful for the original pandas-stubs project at <https://github.com/VirtusLab/pandas-stubs>, which created the framework for testing the stubs.
 
 ## Differences between type declarations in pandas and pandas-stubs
 
 The <https://github.com/pandas-dev/pandas/> project has type declarations for some parts of pandas, both for the internal and public API's.  Those type declarations are used to make sure that the pandas code is _internally_ consistent.
 
-The <https://github.com/pandas-dev/pandas-stubs/> project provides type declarations for the pandas _public_ API.  The philosophy of these stubs can be found at <https://github.com/pandas-dev/pandas-stubs/blob/main/docs/philosophy.md/> While it would be ideal if the `pyi` files in this project would be part of the `pandas` distribution, this would require consistency between the internal type declarations and the public declarations, and the scope of a project to create that consistency is quite large.  That is a long term goal.  Finally, another goal is to do more frequent releases of the pandas-stubs than is done for pandas, in order to make the stubs more useful.
+The <https://github.com/pandas-dev/pandas-stubs/> project provides type declarations for the pandas _public_ API.  The philosophy of these stubs can be found at <https://github.com/pandas-dev/pandas-stubs/blob/main/docs/philosophy.md/>. While it would be ideal if the `pyi` files in this project would be part of the `pandas` distribution, this would require consistency between the internal type declarations and the public declarations, and the scope of a project to create that consistency is quite large.  That is a long term goal.  Finally, another goal is to do more frequent releases of the pandas-stubs than is done for pandas, in order to make the stubs more useful.
 
 If issues are found with the public stubs, pull requests to correct those issues are welcome.  In addition, pull requests on the pandas repository to fix the same issue are welcome there as well.  However, since the goals of typing in the two projects are different (internal consistency vs. public usage), it may be a challenge to create consistent type declarations across both projects.  See <https://pandas.pydata.org/docs/development/contributing_codebase.html#type-hints/> for a discussion of typing standards used within the pandas code.
 
 ## Getting help
 
 Ask questions and report issues on the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/issues).
```

### Comparing `pandas_stubs-1.5.3.230321/setup.py` & `pandas_stubs-2.0.0.230412/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,23 +46,23 @@
                   'util/version/*']}
 
 install_requires = \
 ['types-pytz>=2022.1.1']
 
 setup_kwargs = {
     'name': 'pandas-stubs',
-    'version': '1.5.3.230321',
+    'version': '2.0.0.230412',
     'description': 'Type annotations for pandas',
-    'long_description': '# pandas-stubs: Public type stubs for pandas\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/pandas-stubs.svg)](https://pypi.org/project/pandas-stubs/)\n[![Conda Latest Release](https://anaconda.org/conda-forge/pandas-stubs/badges/version.svg)](https://anaconda.org/conda-forge/pandas-stubs)\n[![Package Status](https://img.shields.io/pypi/status/pandas-stubs.svg)](https://pypi.org/project/pandas-stubs/)\n[![License](https://img.shields.io/pypi/l/pandas-stubs.svg)](https://github.com/pandas-dev/pandas-stubs/blob/main/LICENSE)\n[![Downloads](https://static.pepy.tech/personalized-badge/pandas-stubs?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/pandas-stubs)\n[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/pydata/pandas)\n[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n\n## What is it?\n\nThese are public type stubs for [**pandas**](http://pandas.pydata.org/), following the\nconvention of providing stubs in a separate package, as specified in [PEP 561](https://peps.python.org/pep-0561/#stub-only-packages).  The stubs cover the most typical use cases of\npandas.  In general, these stubs are narrower than what is possibly allowed by pandas,\nbut follow a convention of suggesting best recommended practices for using pandas.\n\nThe stubs are likely incomplete in terms of covering the published API of pandas.\n\nThe stubs are tested with [mypy](http://mypy-lang.org/) and [pyright](https://github.com/microsoft/pyright#readme) and are currently shipped with the Visual Studio Code extension\n[pylance](https://github.com/microsoft/pylance-release#readme).\n\n## Usage\n\nLet’s take this example piece of code in file `round.py`\n\n```python\nimport pandas as pd\n\ndecimals = pd.DataFrame({\'TSLA\': 2, \'AMZN\': 1})\nprices = pd.DataFrame(data={\'date\': [\'2021-08-13\', \'2021-08-07\', \'2021-08-21\'],\n                            \'TSLA\': [720.13, 716.22, 731.22], \'AMZN\': [3316.50, 3200.50, 3100.23]})\nrounded_prices = prices.round(decimals=decimals)\n```\n\nMypy won\'t see any issues with that, but after installing pandas-stubs and running it again:\n\n```sh\nmypy round.py\n```\n\nwe get the following error message:\n\n```text\nround.py:6: error: Argument "decimals" to "round" of "DataFrame" has incompatible type "DataFrame"; expected "Union[int, Dict[Any, Any], Series[Any]]"  [arg-type]\nFound 1 error in 1 file (checked 1 source file)\n```\n\nAnd, if you use pyright:\n\n```sh\npyright round.py\n```\n\nyou get the following error message:\n\n```text\n round.py:6:40 - error: Argument of type "DataFrame" cannot be assigned to parameter "decimals" of type "int | Dict[Unknown, Unknown] | Series[Unknown]" in function "round"\n  \xa0\xa0Type "DataFrame" cannot be assigned to type "int | Dict[Unknown, Unknown] | Series[Unknown]"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "int"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "Dict[Unknown, Unknown]"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "Series[Unknown]" (reportGeneralTypeIssues)\n```\n\nAnd after confirming with the [docs](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.round.html)\nwe can fix the code:\n\n```python\ndecimals = pd.Series({\'TSLA\': 2, \'AMZN\': 1})\n```\n\n## Version Numbering Convention\n\nThe version number x.y.z.yymmdd corresponds to a test done with pandas version x.y.z, with the stubs released on the date mm/yy/dd.\nIt is anticipated that the stubs will be released more frequently than pandas as the stubs are expected to evolve due to more\npublic visibility.\n\n## Where to get it\n\nThe source code is currently hosted on GitHub at: <https://github.com/pandas-dev/pandas-stubs>\n\nBinary installers for the latest released version are available at the [Python\nPackage Index (PyPI)](https://pypi.org/project/pandas-stubs) and on [conda-forge](https://conda-forge.org/).\n\n```sh\n# conda\nconda install pandas-stubs\n```\n\n```sh\n# or PyPI\npip install pandas-stubs\n```\n\n## Dependencies\n\n- [pandas: powerful Python data analysis toolkit](https://pandas.pydata.org/)\n- [typing-extensions >= 4.2.0 - supporting the latest typing extensions](https://github.com/python/typing_extensions#readme)\n\n## Installation from sources\n\n- Make sure you have `python >= 3.8` installed.\n- Install poetry\n\n```sh\n# conda\nconda install poetry\n```\n\n```sh\n# or PyPI\npip install poetry\n```\n\n- Install the project dependencies\n\n```sh\npoetry update -vvv\n```\n\n- Build and install the distribution\n\n```sh\npoetry run poe build_dist\npoetry run poe install_dist\n```\n\n## License\n\n[BSD 3](LICENSE)\n\n## Documentation\n\nDocumentation is a work-in-progress.  \n\n## Background\n\nThese stubs are the result of a strategic effort lead by the core pandas team to integrate [Microsoft type stub repository](https://github.com/microsoft/python-type-stubs)\ntogether with the [VirtusLabs pandas_stubs repository](https://github.com/VirtusLab/pandas-stubs).\n\nThese stubs were initially forked from the Microsoft project <https://github.com/microsoft/python-type-stubs> as of [this commit](https://github.com/microsoft/python-type-stubs/tree/6b800063bde687cd1846122431e2a729a9de625a).\n\nWe are indebted to Microsoft and that project for the initial set of public type stubs.  We are also grateful for the original pandas-stubs project at <https://github.com/VirtusLab/pandas-stubs> that created the framework for testing the stubs.\n\n## Differences between type declarations in pandas and pandas-stubs\n\nThe <https://github.com/pandas-dev/pandas/> project has type declarations for some parts of pandas, both for the internal and public API\'s.  Those type declarations are used to make sure that the pandas code is _internally_ consistent.\n\nThe <https://github.com/pandas-dev/pandas-stubs/> project provides type declarations for the pandas _public_ API.  The philosophy of these stubs can be found at <https://github.com/pandas-dev/pandas-stubs/blob/main/docs/philosophy.md/> While it would be ideal if the `pyi` files in this project would be part of the `pandas` distribution, this would require consistency between the internal type declarations and the public declarations, and the scope of a project to create that consistency is quite large.  That is a long term goal.  Finally, another goal is to do more frequent releases of the pandas-stubs than is done for pandas, in order to make the stubs more useful.\n\nIf issues are found with the public stubs, pull requests to correct those issues are welcome.  In addition, pull requests on the pandas repository to fix the same issue are welcome there as well.  However, since the goals of typing in the two projects are different (internal consistency vs. public usage), it may be a challenge to create consistent type declarations across both projects.  See <https://pandas.pydata.org/docs/development/contributing_codebase.html#type-hints/> for a discussion of typing standards used within the pandas code.\n\n## Getting help\n\nAsk questions and report issues on the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/issues).  \n\n## Discussion and Development\n\nMost development discussions take place on GitHub in the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/). Further, the [pandas-dev mailing list](https://mail.python.org/mailman/listinfo/pandas-dev) can also be used for specialized discussions or design issues, and a [Gitter channel](https://gitter.im/pydata/pandas) is available for quick development related questions.\n\n## Contributing to pandas-stubs\n\nAll contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.  See <https://github.com/pandas-dev/pandas-stubs/tree/main/docs/> for instructions.\n',
+    'long_description': '# pandas-stubs: Public type stubs for pandas\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/pandas-stubs.svg)](https://pypi.org/project/pandas-stubs/)\n[![Conda Latest Release](https://anaconda.org/conda-forge/pandas-stubs/badges/version.svg)](https://anaconda.org/conda-forge/pandas-stubs)\n[![Package Status](https://img.shields.io/pypi/status/pandas-stubs.svg)](https://pypi.org/project/pandas-stubs/)\n[![License](https://img.shields.io/pypi/l/pandas-stubs.svg)](https://github.com/pandas-dev/pandas-stubs/blob/main/LICENSE)\n[![Downloads](https://static.pepy.tech/personalized-badge/pandas-stubs?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/pandas-stubs)\n[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/pydata/pandas)\n[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n\n## What is it?\n\nThese are public type stubs for [**pandas**](http://pandas.pydata.org/), following the\nconvention of providing stubs in a separate package, as specified in [PEP 561](https://peps.python.org/pep-0561/#stub-only-packages).  The stubs cover the most typical use cases of\npandas.  In general, these stubs are narrower than what is possibly allowed by pandas,\nbut follow a convention of suggesting best recommended practices for using pandas.\n\nThe stubs are likely incomplete in terms of covering the published API of pandas.  NOTE: The current 2.0.x releases of pandas-stubs do not support all of the new features of pandas 2.0.  See this [tracker](https://github.com/pandas-dev/pandas-stubs/issues/624) to understand the current compatibility with version 2.0.\n\nThe stubs are tested with [mypy](http://mypy-lang.org/) and [pyright](https://github.com/microsoft/pyright#readme) and are currently shipped with the Visual Studio Code extension\n[pylance](https://github.com/microsoft/pylance-release#readme).\n\n## Usage\n\nLet’s take this example piece of code in file `round.py`\n\n```python\nimport pandas as pd\n\ndecimals = pd.DataFrame({\'TSLA\': 2, \'AMZN\': 1})\nprices = pd.DataFrame(data={\'date\': [\'2021-08-13\', \'2021-08-07\', \'2021-08-21\'],\n                            \'TSLA\': [720.13, 716.22, 731.22], \'AMZN\': [3316.50, 3200.50, 3100.23]})\nrounded_prices = prices.round(decimals=decimals)\n```\n\nMypy won\'t see any issues with that, but after installing pandas-stubs and running it again:\n\n```sh\nmypy round.py\n```\n\nwe get the following error message:\n\n```text\nround.py:6: error: Argument "decimals" to "round" of "DataFrame" has incompatible type "DataFrame"; expected "Union[int, Dict[Any, Any], Series[Any]]"  [arg-type]\nFound 1 error in 1 file (checked 1 source file)\n```\n\nAnd, if you use pyright:\n\n```sh\npyright round.py\n```\n\nyou get the following error message:\n\n```text\n round.py:6:40 - error: Argument of type "DataFrame" cannot be assigned to parameter "decimals" of type "int | Dict[Unknown, Unknown] | Series[Unknown]" in function "round"\n  \xa0\xa0Type "DataFrame" cannot be assigned to type "int | Dict[Unknown, Unknown] | Series[Unknown]"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "int"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "Dict[Unknown, Unknown]"\n  \xa0\xa0\xa0\xa0"DataFrame" is incompatible with "Series[Unknown]" (reportGeneralTypeIssues)\n```\n\nAnd after confirming with the [docs](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.round.html)\nwe can fix the code:\n\n```python\ndecimals = pd.Series({\'TSLA\': 2, \'AMZN\': 1})\n```\n\n## Version Numbering Convention\n\nThe version number x.y.z.yymmdd corresponds to a test done with pandas version x.y.z, with the stubs released on the date mm/yy/dd.\nIt is anticipated that the stubs will be released more frequently than pandas as the stubs are expected to evolve due to more\npublic visibility.\n\n## Where to get it\n\nThe source code is currently hosted on GitHub at: <https://github.com/pandas-dev/pandas-stubs>\n\nBinary installers for the latest released version are available at the [Python\nPackage Index (PyPI)](https://pypi.org/project/pandas-stubs) and on [conda-forge](https://conda-forge.org/).\n\n```sh\n# conda\nconda install pandas-stubs\n```\n\n```sh\n# or PyPI\npip install pandas-stubs\n```\n\n## Dependencies\n\n- [pandas: powerful Python data analysis toolkit](https://pandas.pydata.org/)\n- [typing-extensions >= 4.2.0 - supporting the latest typing extensions](https://github.com/python/typing_extensions#readme)\n\n## Installation from sources\n\n- Make sure you have `python >= 3.8` installed.\n- Install poetry\n\n```sh\n# conda\nconda install poetry\n```\n\n```sh\n# or PyPI\npip install poetry\n```\n\n- Install the project dependencies\n\n```sh\npoetry update -vvv\n```\n\n- Build and install the distribution\n\n```sh\npoetry run poe build_dist\npoetry run poe install_dist\n```\n\n## License\n\n[BSD 3](LICENSE)\n\n## Documentation\n\nDocumentation is a work-in-progress.  \n\n## Background\n\nThese stubs are the result of a strategic effort led by the core pandas team to integrate [Microsoft type stub repository](https://github.com/microsoft/python-type-stubs) with the [VirtusLabs pandas_stubs repository](https://github.com/VirtusLab/pandas-stubs).\n\nThese stubs were initially forked from the Microsoft project at <https://github.com/microsoft/python-type-stubs> as of [this commit](https://github.com/microsoft/python-type-stubs/tree/6b800063bde687cd1846122431e2a729a9de625a).\n\nWe are indebted to Microsoft and that project for providing the initial set of public type stubs.  We are also grateful for the original pandas-stubs project at <https://github.com/VirtusLab/pandas-stubs>, which created the framework for testing the stubs.\n\n## Differences between type declarations in pandas and pandas-stubs\n\nThe <https://github.com/pandas-dev/pandas/> project has type declarations for some parts of pandas, both for the internal and public API\'s.  Those type declarations are used to make sure that the pandas code is _internally_ consistent.\n\nThe <https://github.com/pandas-dev/pandas-stubs/> project provides type declarations for the pandas _public_ API.  The philosophy of these stubs can be found at <https://github.com/pandas-dev/pandas-stubs/blob/main/docs/philosophy.md/>. While it would be ideal if the `pyi` files in this project would be part of the `pandas` distribution, this would require consistency between the internal type declarations and the public declarations, and the scope of a project to create that consistency is quite large.  That is a long term goal.  Finally, another goal is to do more frequent releases of the pandas-stubs than is done for pandas, in order to make the stubs more useful.\n\nIf issues are found with the public stubs, pull requests to correct those issues are welcome.  In addition, pull requests on the pandas repository to fix the same issue are welcome there as well.  However, since the goals of typing in the two projects are different (internal consistency vs. public usage), it may be a challenge to create consistent type declarations across both projects.  See <https://pandas.pydata.org/docs/development/contributing_codebase.html#type-hints/> for a discussion of typing standards used within the pandas code.\n\n## Getting help\n\nAsk questions and report issues on the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/issues).  \n\n## Discussion and Development\n\nMost development discussions take place on GitHub in the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/). Further, the [pandas-dev mailing list](https://mail.python.org/mailman/listinfo/pandas-dev) can also be used for specialized discussions or design issues, and a [Gitter channel](https://gitter.im/pydata/pandas) is available for quick development related questions.\n\n## Contributing to pandas-stubs\n\nAll contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome.  See <https://github.com/pandas-dev/pandas-stubs/tree/main/docs/> for instructions.\n',
     'author': 'The Pandas Development Team',
     'author_email': 'pandas-dev@python.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pandas.pydata.org',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.12',
+    'python_requires': '>=3.8',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pandas_stubs-1.5.3.230321/PKG-INFO` & `pandas_stubs-2.0.0.230412/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pandas-stubs
-Version: 1.5.3.230321
+Version: 2.0.0.230412
 Summary: Type annotations for pandas
 Home-page: https://pandas.pydata.org
 License: BSD-3-Clause
 Author: The Pandas Development Team
 Author-email: pandas-dev@python.org
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -46,15 +46,15 @@
 ## What is it?
 
 These are public type stubs for [**pandas**](http://pandas.pydata.org/), following the
 convention of providing stubs in a separate package, as specified in [PEP 561](https://peps.python.org/pep-0561/#stub-only-packages).  The stubs cover the most typical use cases of
 pandas.  In general, these stubs are narrower than what is possibly allowed by pandas,
 but follow a convention of suggesting best recommended practices for using pandas.
 
-The stubs are likely incomplete in terms of covering the published API of pandas.
+The stubs are likely incomplete in terms of covering the published API of pandas.  NOTE: The current 2.0.x releases of pandas-stubs do not support all of the new features of pandas 2.0.  See this [tracker](https://github.com/pandas-dev/pandas-stubs/issues/624) to understand the current compatibility with version 2.0.
 
 The stubs are tested with [mypy](http://mypy-lang.org/) and [pyright](https://github.com/microsoft/pyright#readme) and are currently shipped with the Visual Studio Code extension
 [pylance](https://github.com/microsoft/pylance-release#readme).
 
 ## Usage
 
 Let’s take this example piece of code in file `round.py`
@@ -166,26 +166,25 @@
 
 ## Documentation
 
 Documentation is a work-in-progress.  
 
 ## Background
 
-These stubs are the result of a strategic effort lead by the core pandas team to integrate [Microsoft type stub repository](https://github.com/microsoft/python-type-stubs)
-together with the [VirtusLabs pandas_stubs repository](https://github.com/VirtusLab/pandas-stubs).
+These stubs are the result of a strategic effort led by the core pandas team to integrate [Microsoft type stub repository](https://github.com/microsoft/python-type-stubs) with the [VirtusLabs pandas_stubs repository](https://github.com/VirtusLab/pandas-stubs).
 
-These stubs were initially forked from the Microsoft project <https://github.com/microsoft/python-type-stubs> as of [this commit](https://github.com/microsoft/python-type-stubs/tree/6b800063bde687cd1846122431e2a729a9de625a).
+These stubs were initially forked from the Microsoft project at <https://github.com/microsoft/python-type-stubs> as of [this commit](https://github.com/microsoft/python-type-stubs/tree/6b800063bde687cd1846122431e2a729a9de625a).
 
-We are indebted to Microsoft and that project for the initial set of public type stubs.  We are also grateful for the original pandas-stubs project at <https://github.com/VirtusLab/pandas-stubs> that created the framework for testing the stubs.
+We are indebted to Microsoft and that project for providing the initial set of public type stubs.  We are also grateful for the original pandas-stubs project at <https://github.com/VirtusLab/pandas-stubs>, which created the framework for testing the stubs.
 
 ## Differences between type declarations in pandas and pandas-stubs
 
 The <https://github.com/pandas-dev/pandas/> project has type declarations for some parts of pandas, both for the internal and public API's.  Those type declarations are used to make sure that the pandas code is _internally_ consistent.
 
-The <https://github.com/pandas-dev/pandas-stubs/> project provides type declarations for the pandas _public_ API.  The philosophy of these stubs can be found at <https://github.com/pandas-dev/pandas-stubs/blob/main/docs/philosophy.md/> While it would be ideal if the `pyi` files in this project would be part of the `pandas` distribution, this would require consistency between the internal type declarations and the public declarations, and the scope of a project to create that consistency is quite large.  That is a long term goal.  Finally, another goal is to do more frequent releases of the pandas-stubs than is done for pandas, in order to make the stubs more useful.
+The <https://github.com/pandas-dev/pandas-stubs/> project provides type declarations for the pandas _public_ API.  The philosophy of these stubs can be found at <https://github.com/pandas-dev/pandas-stubs/blob/main/docs/philosophy.md/>. While it would be ideal if the `pyi` files in this project would be part of the `pandas` distribution, this would require consistency between the internal type declarations and the public declarations, and the scope of a project to create that consistency is quite large.  That is a long term goal.  Finally, another goal is to do more frequent releases of the pandas-stubs than is done for pandas, in order to make the stubs more useful.
 
 If issues are found with the public stubs, pull requests to correct those issues are welcome.  In addition, pull requests on the pandas repository to fix the same issue are welcome there as well.  However, since the goals of typing in the two projects are different (internal consistency vs. public usage), it may be a challenge to create consistent type declarations across both projects.  See <https://pandas.pydata.org/docs/development/contributing_codebase.html#type-hints/> for a discussion of typing standards used within the pandas code.
 
 ## Getting help
 
 Ask questions and report issues on the [pandas-stubs repository](https://github.com/pandas-dev/pandas-stubs/issues).
```

