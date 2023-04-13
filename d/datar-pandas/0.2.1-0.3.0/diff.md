# Comparing `tmp/datar_pandas-0.2.1.tar.gz` & `tmp/datar_pandas-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datar_pandas-0.2.1.tar", max compression
+gzip compressed data, was "datar_pandas-0.3.0.tar", max compression
```

## Comparing `datar_pandas-0.2.1.tar` & `datar_pandas-0.3.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0      465 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/README.md
--rw-r--r--   0        0        0       75 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/__init__.py
--rw-r--r--   0        0        0       72 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/__init__.py
--rw-r--r--   0        0        0    10768 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/arithm.py
--rw-r--r--   0        0        0     7544 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/asis.py
--rw-r--r--   0        0        0      614 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/bessel.py
--rw-r--r--   0        0        0      494 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/complex.py
--rw-r--r--   0        0        0      451 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/cum.py
--rw-r--r--   0        0        0     2560 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/factor.py
--rw-r--r--   0        0        0     1759 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/funs.py
--rw-r--r--   0        0        0      315 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/null.py
--rw-r--r--   0        0        0      772 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/random.py
--rw-r--r--   0        0        0     7526 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/seq.py
--rw-r--r--   0        0        0     1066 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/special.py
--rw-r--r--   0        0        0     4183 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/string.py
--rw-r--r--   0        0        0     6260 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/table.py
--rw-r--r--   0        0        0     2073 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/trig.py
--rw-r--r--   0        0        0     4687 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/verbs.py
--rw-r--r--   0        0        0      336 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/base/which.py
--rw-r--r--   0        0        0        0 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/dplyr/__init__.py
--rw-r--r--   0        0        0     4617 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/dplyr/_rank.py
--rw-r--r--   0        0        0     2768 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/dplyr/across.py
--rw-r--r--   0        0        0     1377 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/dplyr/arrange.py
--rw-r--r--   0        0        0     4276 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/dplyr/bind.py
--rw-r--r--   0        0        0     4239 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/dplyr/context.py
--rw-r--r--   0        0        0     4486 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/dplyr/count_tally.py
--rw-r--r--   0        0        0     1094 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/dplyr/desc.py
--rw-r--r--   0        0        0     2591 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/dplyr/distinct.py
--rw-r--r--   0        0        0     1588 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/dplyr/filter_.py
--rw-r--r--   0        0        0     5462 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/dplyr/funs.py
--rw-r--r--   0        0        0      425 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/dplyr/glimpse.py
--rw-r--r--   0        0        0     5150 2023-03-06 21:33:36.042751 datar_pandas-0.2.1/datar_pandas/api/dplyr/group_by.py
--rw-r--r--   0        0        0     4077 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/group_data.py
--rw-r--r--   0        0        0     8005 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/group_iter.py
--rw-r--r--   0        0        0     2832 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/if_else.py
--rw-r--r--   0        0        0     7418 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/join.py
--rw-r--r--   0        0        0     1969 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/lead_lag.py
--rw-r--r--   0        0        0     4468 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/mutate.py
--rw-r--r--   0        0        0     2084 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/order_by.py
--rw-r--r--   0        0        0     2901 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/pull.py
--rw-r--r--   0        0        0     1107 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/rank.py
--rw-r--r--   0        0        0     9682 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/recode.py
--rw-r--r--   0        0        0     2331 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/relocate.py
--rw-r--r--   0        0        0     1754 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/rename.py
--rw-r--r--   0        0        0     4545 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/rows.py
--rw-r--r--   0        0        0     2287 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/select.py
--rw-r--r--   0        0        0     5851 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/sets.py
--rw-r--r--   0        0        0     8380 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/slice_.py
--rw-r--r--   0        0        0     4875 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/summarise.py
--rw-r--r--   0        0        0     5251 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/dplyr/tidyselect.py
--rw-r--r--   0        0        0        0 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/forcats/__init__.py
--rw-r--r--   0        0        0     2344 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/forcats/fct_multi.py
--rw-r--r--   0        0        0     3773 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/forcats/lvl_addrm.py
--rw-r--r--   0        0        0    11555 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/forcats/lvl_order.py
--rw-r--r--   0        0        0    17268 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/forcats/lvl_value.py
--rw-r--r--   0        0        0     5503 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/forcats/lvls.py
--rw-r--r--   0        0        0     3399 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/forcats/misc.py
--rw-r--r--   0        0        0      479 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/forcats/utils.py
--rw-r--r--   0        0        0     5784 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/misc.py
--rw-r--r--   0        0        0        0 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tibble/__init__.py
--rw-r--r--   0        0        0     6261 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tibble/tibble.py
--rw-r--r--   0        0        0     9985 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tibble/verbs.py
--rw-r--r--   0        0        0        0 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/__init__.py
--rw-r--r--   0        0        0     8095 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/chop.py
--rw-r--r--   0        0        0     1938 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/complete.py
--rw-r--r--   0        0        0     1450 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/drop_na.py
--rw-r--r--   0        0        0    13699 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/expand.py
--rw-r--r--   0        0        0     2984 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/extract.py
--rw-r--r--   0        0        0     2126 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/fill.py
--rw-r--r--   0        0        0     1127 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/funs.py
--rw-r--r--   0        0        0     9502 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/nest.py
--rw-r--r--   0        0        0     5067 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/pack.py
--rw-r--r--   0        0        0    10118 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/pivot_long.py
--rw-r--r--   0        0        0     7384 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/pivot_wide.py
--rw-r--r--   0        0        0     2372 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/replace_na.py
--rw-r--r--   0        0        0     7110 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/separate.py
--rw-r--r--   0        0        0     2099 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/uncount.py
--rw-r--r--   0        0        0     2029 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/api/tidyr/unite.py
--rw-r--r--   0        0        0    24230 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/broadcast.py
--rw-r--r--   0        0        0    11011 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/collections.py
--rw-r--r--   0        0        0     1207 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/common.py
--rw-r--r--   0        0        0     1484 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/contexts.py
--rw-r--r--   0        0        0    15407 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/factory.py
--rw-r--r--   0        0        0     9340 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/middlewares.py
--rw-r--r--   0        0        0     3762 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/operators.py
--rw-r--r--   0        0        0     1951 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/pandas.py
--rw-r--r--   0        0        0     3205 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/plugin.py
--rw-r--r--   0        0        0    15233 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/tibble.py
--rw-r--r--   0        0        0      469 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/typing.py
--rw-r--r--   0        0        0     4530 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/utils.py
--rw-r--r--   0        0        0       22 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/datar_pandas/version.py
--rw-r--r--   0        0        0     1041 2023-03-06 21:33:36.046751 datar_pandas-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 datar_pandas-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      465 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/README.md
+-rw-r--r--   0        0        0       75 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/__init__.py
+-rw-r--r--   0        0        0       72 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/__init__.py
+-rw-r--r--   0        0        0    10768 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/arithm.py
+-rw-r--r--   0        0        0     7544 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/asis.py
+-rw-r--r--   0        0        0      614 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/bessel.py
+-rw-r--r--   0        0        0      494 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/complex.py
+-rw-r--r--   0        0        0      451 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/cum.py
+-rw-r--r--   0        0        0     2560 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/factor.py
+-rw-r--r--   0        0        0     1759 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/funs.py
+-rw-r--r--   0        0        0      315 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/null.py
+-rw-r--r--   0        0        0      772 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/random.py
+-rw-r--r--   0        0        0     7526 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/seq.py
+-rw-r--r--   0        0        0     1066 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/special.py
+-rw-r--r--   0        0        0     4183 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/string.py
+-rw-r--r--   0        0        0     6260 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/table.py
+-rw-r--r--   0        0        0     2073 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/trig.py
+-rw-r--r--   0        0        0     4687 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/verbs.py
+-rw-r--r--   0        0        0      336 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/base/which.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/dplyr/__init__.py
+-rw-r--r--   0        0        0     4617 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/dplyr/_rank.py
+-rw-r--r--   0        0        0     2768 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/dplyr/across.py
+-rw-r--r--   0        0        0     1377 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/dplyr/arrange.py
+-rw-r--r--   0        0        0     4276 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/dplyr/bind.py
+-rw-r--r--   0        0        0     4239 2023-04-13 07:52:47.690445 datar_pandas-0.3.0/datar_pandas/api/dplyr/context.py
+-rw-r--r--   0        0        0     4486 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/count_tally.py
+-rw-r--r--   0        0        0     1094 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/desc.py
+-rw-r--r--   0        0        0     2591 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/distinct.py
+-rw-r--r--   0        0        0     1588 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/filter_.py
+-rw-r--r--   0        0        0     5462 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/funs.py
+-rw-r--r--   0        0        0      425 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/glimpse.py
+-rw-r--r--   0        0        0     5150 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/group_by.py
+-rw-r--r--   0        0        0     4077 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/group_data.py
+-rw-r--r--   0        0        0     8005 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/group_iter.py
+-rw-r--r--   0        0        0     2832 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/if_else.py
+-rw-r--r--   0        0        0     7418 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/join.py
+-rw-r--r--   0        0        0     1969 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/lead_lag.py
+-rw-r--r--   0        0        0     4611 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/mutate.py
+-rw-r--r--   0        0        0     2084 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/order_by.py
+-rw-r--r--   0        0        0     2901 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/pull.py
+-rw-r--r--   0        0        0     1107 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/rank.py
+-rw-r--r--   0        0        0     9682 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/recode.py
+-rw-r--r--   0        0        0     2331 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/relocate.py
+-rw-r--r--   0        0        0     1754 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/rename.py
+-rw-r--r--   0        0        0     4545 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/rows.py
+-rw-r--r--   0        0        0     2287 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/select.py
+-rw-r--r--   0        0        0     5851 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/sets.py
+-rw-r--r--   0        0        0     8669 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/slice_.py
+-rw-r--r--   0        0        0     4633 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/summarise.py
+-rw-r--r--   0        0        0     5251 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/dplyr/tidyselect.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/forcats/__init__.py
+-rw-r--r--   0        0        0     2344 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/forcats/fct_multi.py
+-rw-r--r--   0        0        0     3773 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/forcats/lvl_addrm.py
+-rw-r--r--   0        0        0    11555 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/forcats/lvl_order.py
+-rw-r--r--   0        0        0    17268 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/forcats/lvl_value.py
+-rw-r--r--   0        0        0     5503 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/forcats/lvls.py
+-rw-r--r--   0        0        0     3399 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/forcats/misc.py
+-rw-r--r--   0        0        0      479 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/forcats/utils.py
+-rw-r--r--   0        0        0     5784 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/misc.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tibble/__init__.py
+-rw-r--r--   0        0        0     6261 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tibble/tibble.py
+-rw-r--r--   0        0        0     9985 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tibble/verbs.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/__init__.py
+-rw-r--r--   0        0        0     8095 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/chop.py
+-rw-r--r--   0        0        0     1938 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/complete.py
+-rw-r--r--   0        0        0     1450 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/drop_na.py
+-rw-r--r--   0        0        0    13699 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/expand.py
+-rw-r--r--   0        0        0     2984 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/extract.py
+-rw-r--r--   0        0        0     2126 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/fill.py
+-rw-r--r--   0        0        0     1127 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/funs.py
+-rw-r--r--   0        0        0     9502 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/nest.py
+-rw-r--r--   0        0        0     5067 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/pack.py
+-rw-r--r--   0        0        0    10118 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/pivot_long.py
+-rw-r--r--   0        0        0     7384 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/pivot_wide.py
+-rw-r--r--   0        0        0     2372 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/replace_na.py
+-rw-r--r--   0        0        0     7110 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/separate.py
+-rw-r--r--   0        0        0     2099 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/uncount.py
+-rw-r--r--   0        0        0     2029 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/api/tidyr/unite.py
+-rw-r--r--   0        0        0    24230 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/broadcast.py
+-rw-r--r--   0        0        0    11011 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/collections.py
+-rw-r--r--   0        0        0     1207 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/common.py
+-rw-r--r--   0        0        0     1484 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/contexts.py
+-rw-r--r--   0        0        0    15407 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/factory.py
+-rw-r--r--   0        0        0     9340 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/middlewares.py
+-rw-r--r--   0        0        0     3762 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/operators.py
+-rw-r--r--   0        0        0     1951 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/pandas.py
+-rw-r--r--   0        0        0     3205 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/plugin.py
+-rw-r--r--   0        0        0    15233 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/tibble.py
+-rw-r--r--   0        0        0      469 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/typing.py
+-rw-r--r--   0        0        0     4530 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/utils.py
+-rw-r--r--   0        0        0       22 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/datar_pandas/version.py
+-rw-r--r--   0        0        0     1039 2023-04-13 07:52:47.694445 datar_pandas-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 datar_pandas-0.3.0/PKG-INFO
```

### Comparing `datar_pandas-0.2.1/datar_pandas/api/base/arithm.py` & `datar_pandas-0.3.0/datar_pandas/api/base/arithm.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/base/asis.py` & `datar_pandas-0.3.0/datar_pandas/api/base/asis.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/base/bessel.py` & `datar_pandas-0.3.0/datar_pandas/api/base/bessel.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/base/factor.py` & `datar_pandas-0.3.0/datar_pandas/api/base/factor.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/base/funs.py` & `datar_pandas-0.3.0/datar_pandas/api/base/funs.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/base/random.py` & `datar_pandas-0.3.0/datar_pandas/api/base/random.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/base/seq.py` & `datar_pandas-0.3.0/datar_pandas/api/base/seq.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/base/special.py` & `datar_pandas-0.3.0/datar_pandas/api/base/special.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/base/string.py` & `datar_pandas-0.3.0/datar_pandas/api/base/string.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/base/table.py` & `datar_pandas-0.3.0/datar_pandas/api/base/table.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/base/trig.py` & `datar_pandas-0.3.0/datar_pandas/api/base/trig.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/base/verbs.py` & `datar_pandas-0.3.0/datar_pandas/api/base/verbs.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/_rank.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/_rank.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/across.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/across.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/arrange.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/arrange.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/bind.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/bind.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/context.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/context.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/count_tally.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/count_tally.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/desc.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/desc.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/distinct.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/distinct.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/filter_.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/filter_.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/funs.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/funs.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/group_by.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/group_by.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/group_data.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/group_data.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/group_iter.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/group_iter.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/if_else.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/if_else.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/join.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/join.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/lead_lag.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/lead_lag.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/mutate.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/mutate.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     _data,
     *args,
     _keep="all",
     _before=None,
     _after=None,
     **kwargs,
 ):
-    keep = arg_match(_keep, "_keep", ["all", "unused", "used", "none"])
+    keep = arg_match(_keep, "_keep", ["all", "unused", "used", "none", "trans"])
     gvars = group_vars(_data, __ast_fallback="normal", __backend="pandas")
     data = as_tibble(_data.copy(), __ast_fallback="normal", __backend="pandas")
     data._datar["used_refs"] = set()
     all_columns = data.columns
 
     mutated_cols = []
     for val in args:
@@ -111,19 +111,24 @@
             Collection(gvars, unused, mutated_cols),
         )
     elif keep == "used":
         keep = intersect(
             data.columns,
             Collection(gvars, used_refs, mutated_cols),
         )
-    else:  # keep == 'none':
+    elif keep == "trans":
         keep = union(
             setdiff(gvars, mutated_cols),
             intersect(mutated_cols, data.columns),
         )
+    else:  # keep == 'none':
+        keep = intersect(
+            data.columns,
+            Collection(gvars, mutated_cols),
+        )
 
     data = data[keep]
     # redo grouping if original columns changed
     # so we don't have discripency on
     # df.get_obj(x) when df is grouped
     if intersect(_data.columns, mutated_cols).size > 0:
         data = reconstruct_tibble(data, _data)
@@ -140,14 +145,14 @@
     _before=None,
     _after=None,
     **kwargs,
 ):
     return mutate(
         _data,
         *args,
-        _keep="none",
+        _keep="trans",
         _before=_before,
         _after=_after,
         __ast_fallback="normal",
         __backend="pandas",
         **kwargs,
     )
```

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/order_by.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/order_by.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/pull.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/pull.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/rank.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/rank.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/recode.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/recode.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/relocate.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/relocate.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/rename.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/rename.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/rows.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/rows.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/select.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/select.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/sets.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/sets.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/slice_.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/slice_.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Subset rows using their positions
 
 https://github.com/tidyverse/dplyr/blob/master/R/slice.R
 """
+from __future__ import annotations
+
 import builtins
+from math import ceil, floor
 from typing import TYPE_CHECKING, Any, Iterable, Mapping, Union
 
 import numpy as np
 from pipda import Expression
 from datar.core.utils import logger
 from datar.apis.dplyr import (
     slice_,
@@ -124,15 +127,18 @@
     _data: DataFrame,
     n: int = 1,
     prop: float = None,
 ) -> Tibble:
     n = _n_from_prop(_data.shape[0], n, prop)
     return slice_(
         _data,
-        builtins.slice(-n, None),
+        builtins.slice(
+            _data.shape[0] if n == 0 else -n,
+            None,
+        ),
         __ast_fallback="normal",
         __backend="pandas",
     )
 
 
 @slice_tail.register(TibbleGrouped, context=Context.EVAL, backend="pandas")
 def _slice_tail_grouped(
@@ -250,29 +256,34 @@
         weights=_ungroup(weight_by),
         random_state=random_state,
     )
 
 
 def _n_from_prop(
     total: int,
-    n: int = None,
+    n: int | float = None,
     prop: float = None,
 ) -> int:
     """Get n from a proportion"""
     if n is None and prop is None:
         return 1
-    if n is not None and not isinstance(n, int):
-        raise TypeError(f"Expect `n` int type, got {type(n)}.")
+    if n is not None and not isinstance(n, (int, float)):
+        raise TypeError(f"Expect `n` a number, got {type(n)}.")
     if prop is not None and not isinstance(prop, (int, float)):
         raise TypeError(f"Expect `prop` a number, got {type(n)}.")
-    if (n is not None and n < 0) or (prop is not None and prop < 0):
-        raise ValueError("`n` and `prop` should not be negative.")
+    # if (n is not None and n < 0) or (prop is not None and prop < 0):
+    #     raise ValueError("`n` and `prop` should not be negative.")
     if prop is not None:
-        return int(float(total) * min(prop, 1.0))
-    return min(n, total)
+        if prop < 0:
+            return max(ceil((1.0 + prop) * total), 0)
+        return floor(float(total) * min(prop, 1.0))
+
+    if n < 0:
+        return max(ceil(total + n), 0)
+    return min(floor(n), total)
 
 
 def _sanitize_rows(
     rows: Iterable,
     indices: Union[int, Mapping] = None,
     result_index: "Index" = None,
 ) -> np.ndarray:
```

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/summarise.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/summarise.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,22 +77,14 @@
             drop=grouped.observed,
             dropna=grouped.dropna,
         )
 
     elif _groups == "rowwise":
         out = out.rowwise(gvars)
 
-    elif isinstance(_data, TibbleRowwise) and get_option(
-        "dplyr_summarise_inform"
-    ):
-        logger.info(
-            "`summarise()` has ungrouped output. "
-            "You can override using the `_groups` argument."
-        )
-
     # else: # drop
     return out
 
 
 def _summarise_build(
     _data: DataFrame,
     *args: Any,
```

### Comparing `datar_pandas-0.2.1/datar_pandas/api/dplyr/tidyselect.py` & `datar_pandas-0.3.0/datar_pandas/api/dplyr/tidyselect.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/forcats/fct_multi.py` & `datar_pandas-0.3.0/datar_pandas/api/forcats/fct_multi.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/forcats/lvl_addrm.py` & `datar_pandas-0.3.0/datar_pandas/api/forcats/lvl_addrm.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/forcats/lvl_order.py` & `datar_pandas-0.3.0/datar_pandas/api/forcats/lvl_order.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/forcats/lvl_value.py` & `datar_pandas-0.3.0/datar_pandas/api/forcats/lvl_value.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/forcats/lvls.py` & `datar_pandas-0.3.0/datar_pandas/api/forcats/lvls.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/forcats/misc.py` & `datar_pandas-0.3.0/datar_pandas/api/forcats/misc.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/misc.py` & `datar_pandas-0.3.0/datar_pandas/api/misc.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tibble/tibble.py` & `datar_pandas-0.3.0/datar_pandas/api/tibble/tibble.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tibble/verbs.py` & `datar_pandas-0.3.0/datar_pandas/api/tibble/verbs.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/chop.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/chop.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/complete.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/complete.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/drop_na.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/drop_na.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/expand.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/expand.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/extract.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/extract.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/fill.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/fill.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/funs.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/funs.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/nest.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/nest.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/pack.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/pack.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/pivot_long.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/pivot_long.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/pivot_wide.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/pivot_wide.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/replace_na.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/replace_na.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/separate.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/separate.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/uncount.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/uncount.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/api/tidyr/unite.py` & `datar_pandas-0.3.0/datar_pandas/api/tidyr/unite.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/broadcast.py` & `datar_pandas-0.3.0/datar_pandas/broadcast.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/collections.py` & `datar_pandas-0.3.0/datar_pandas/collections.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/common.py` & `datar_pandas-0.3.0/datar_pandas/common.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/contexts.py` & `datar_pandas-0.3.0/datar_pandas/contexts.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/factory.py` & `datar_pandas-0.3.0/datar_pandas/factory.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/middlewares.py` & `datar_pandas-0.3.0/datar_pandas/middlewares.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/operators.py` & `datar_pandas-0.3.0/datar_pandas/operators.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/pandas.py` & `datar_pandas-0.3.0/datar_pandas/pandas.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/plugin.py` & `datar_pandas-0.3.0/datar_pandas/plugin.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/tibble.py` & `datar_pandas-0.3.0/datar_pandas/tibble.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/datar_pandas/utils.py` & `datar_pandas-0.3.0/datar_pandas/utils.py`

 * *Files identical despite different names*

### Comparing `datar_pandas-0.2.1/pyproject.toml` & `datar_pandas-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "datar-pandas"
-version = "0.2.1"
+version = "0.3.0"
 description = "The pandas backend for datar"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "datar_pandas"}]
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
+python = "^3.8"
 pdtypes = "^0.0.4"
-datar = "^0.11"
-datar-numpy = "^0.1"
+datar = "^0.12"
+datar-numpy = "^0.2"
 # modin = { version = "^0.10", optional = true }
 
 # [tool.poetry.extras]
 # modin = ["modin"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
```

### Comparing `datar_pandas-0.2.1/PKG-INFO` & `datar_pandas-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: datar-pandas
-Version: 0.2.1
+Version: 0.3.0
 Summary: The pandas backend for datar
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: datar (>=0.11,<0.12)
-Requires-Dist: datar-numpy (>=0.1,<0.2)
+Requires-Dist: datar (>=0.12,<0.13)
+Requires-Dist: datar-numpy (>=0.2,<0.3)
 Requires-Dist: pdtypes (>=0.0.4,<0.0.5)
 Description-Content-Type: text/markdown
 
 # datar-pandas
 
 The pandas backend for [datar][1].
```

