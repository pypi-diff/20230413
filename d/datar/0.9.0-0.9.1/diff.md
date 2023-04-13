# Comparing `tmp/datar-0.9.0.tar.gz` & `tmp/datar-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datar-0.9.0.tar", max compression
+gzip compressed data, was "datar-0.9.1.tar", max compression
```

## Comparing `datar-0.9.0.tar` & `datar-0.9.1.tar`

### file list

```diff
@@ -1,166 +1,166 @@
--rw-r--r--   0        0        0     1063 2022-09-14 05:32:24.091177 datar-0.9.0/LICENSE
--rw-r--r--   0        0        0     3865 2022-09-14 05:32:24.091177 datar-0.9.0/README.md
--rw-r--r--   0        0        0     1447 2022-09-14 05:32:24.091177 datar-0.9.0/datar/__init__.py
--rw-r--r--   0        0        0      887 2022-09-14 05:32:24.091177 datar-0.9.0/datar/all.py
--rw-r--r--   0        0        0     3320 2022-09-14 05:32:24.091177 datar-0.9.0/datar/base/__init__.py
--rw-r--r--   0        0        0    21342 2022-09-14 05:32:24.091177 datar-0.9.0/datar/base/arithmetic.py
--rw-r--r--   0        0        0     3837 2022-09-14 05:32:24.091177 datar-0.9.0/datar/base/bessel.py
--rw-r--r--   0        0        0     3402 2022-09-14 05:32:24.091177 datar-0.9.0/datar/base/casting.py
--rw-r--r--   0        0        0     2657 2022-09-14 05:32:24.091177 datar-0.9.0/datar/base/complex.py
--rw-r--r--   0        0        0      565 2022-09-14 05:32:24.091177 datar-0.9.0/datar/base/constants.py
--rw-r--r--   0        0        0     1514 2022-09-14 05:32:24.091177 datar-0.9.0/datar/base/cum.py
--rw-r--r--   0        0        0     4579 2022-09-14 05:32:24.091177 datar-0.9.0/datar/base/date.py
--rw-r--r--   0        0        0     4104 2022-09-14 05:32:24.091177 datar-0.9.0/datar/base/factor.py
--rw-r--r--   0        0        0     7822 2022-09-14 05:32:24.091177 datar-0.9.0/datar/base/funs.py
--rw-r--r--   0        0        0     1887 2022-09-14 05:32:24.095177 datar-0.9.0/datar/base/logical.py
--rw-r--r--   0        0        0     2365 2022-09-14 05:32:24.095177 datar-0.9.0/datar/base/na.py
--rw-r--r--   0        0        0      640 2022-09-14 05:32:24.095177 datar-0.9.0/datar/base/null.py
--rw-r--r--   0        0        0      203 2022-09-14 05:32:24.095177 datar-0.9.0/datar/base/random.py
--rw-r--r--   0        0        0     5073 2022-09-14 05:32:24.095177 datar-0.9.0/datar/base/rep.py
--rw-r--r--   0        0        0    10154 2022-09-14 05:32:24.095177 datar-0.9.0/datar/base/seq.py
--rw-r--r--   0        0        0     5133 2022-09-14 05:32:24.095177 datar-0.9.0/datar/base/special.py
--rw-r--r--   0        0        0     3682 2022-09-14 05:32:24.095177 datar-0.9.0/datar/base/stats.py
--rw-r--r--   0        0        0    15226 2022-09-14 05:32:24.095177 datar-0.9.0/datar/base/string.py
--rw-r--r--   0        0        0     6482 2022-09-14 05:32:24.095177 datar-0.9.0/datar/base/table.py
--rw-r--r--   0        0        0     4469 2022-09-14 05:32:24.095177 datar-0.9.0/datar/base/testing.py
--rw-r--r--   0        0        0     4562 2022-09-14 05:32:24.095177 datar-0.9.0/datar/base/trig_hb.py
--rw-r--r--   0        0        0    12664 2022-09-14 05:32:24.095177 datar-0.9.0/datar/base/verbs.py
--rw-r--r--   0        0        0     1237 2022-09-14 05:32:24.095177 datar-0.9.0/datar/base/which.py
--rw-r--r--   0        0        0      149 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/__init__.py
--rw-r--r--   0        0        0       66 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/backends/__init__.py
--rw-r--r--   0        0        0      888 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/backends/pandas/__init__.py
--rw-r--r--   0        0        0        0 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/backends/pandas/api/__init__.py
--rw-r--r--   0        0        0      306 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/backends/pandas/api/types.py
--rw-r--r--   0        0        0        0 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/backends/pandas/core/__init__.py
--rw-r--r--   0        0        0       42 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/backends/pandas/core/base.py
--rw-r--r--   0        0        0       40 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/backends/pandas/core/generic.py
--rw-r--r--   0        0        0      316 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/backends/pandas/core/groupby.py
--rw-r--r--   0        0        0      105 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/backends/pandas/testing.py
--rw-r--r--   0        0        0    23702 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/broadcast.py
--rw-r--r--   0        0        0    12639 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/collections.py
--rw-r--r--   0        0        0     1456 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/contexts.py
--rw-r--r--   0        0        0      133 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/defaults.py
--rw-r--r--   0        0        0      100 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/exceptions.py
--rw-r--r--   0        0        0    28275 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/factory.py
--rw-r--r--   0        0        0     2328 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/import_names_conflict.py
--rw-r--r--   0        0        0      657 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/middlewares.py
--rw-r--r--   0        0        0     5370 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/names.py
--rw-r--r--   0        0        0     4842 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/operator.py
--rw-r--r--   0        0        0     4223 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/options.py
--rw-r--r--   0        0        0    15187 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/tibble.py
--rw-r--r--   0        0        0     4209 2022-09-14 05:32:24.095177 datar-0.9.0/datar/core/utils.py
--rw-r--r--   0        0        0      143 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datar/__init__.py
--rw-r--r--   0        0        0     4323 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datar/funcs.py
--rw-r--r--   0        0        0     2053 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datar/verbs.py
--rw-r--r--   0        0        0     1102 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datasets/__init__.py
--rw-r--r--   0        0        0      242 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datasets/airlines.csv.gz
--rw-r--r--   0        0        0    37924 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datasets/airports.csv.gz
--rw-r--r--   0        0        0     1300 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datasets/airquality.csv.gz
--rw-r--r--   0        0        0      211 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datasets/anscombe.csv.gz
--rw-r--r--   0        0        0       88 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datasets/band_instruments.csv.gz
--rw-r--r--   0        0        0       91 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datasets/band_instruments2.csv.gz
--rw-r--r--   0        0        0       84 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datasets/band_members.csv.gz
--rw-r--r--   0        0        0    13706 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datasets/billboard.csv.gz
--rw-r--r--   0        0        0     1995 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datasets/chickweight.csv.gz
--rw-r--r--   0        0        0      305 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datasets/construction.csv.gz
--rw-r--r--   0        0        0   445681 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datasets/diamonds.csv.gz
--rw-r--r--   0        0        0     8780 2022-09-14 05:32:24.095177 datar-0.9.0/datar/datasets/economics.csv.gz
--rw-r--r--   0        0        0    33152 2022-09-14 05:32:24.099177 datar-0.9.0/datar/datasets/economics_long.csv.gz
--rw-r--r--   0        0        0      883 2022-09-14 05:32:24.099177 datar-0.9.0/datar/datasets/faithful.csv.gz
--rw-r--r--   0        0        0    71260 2022-09-14 05:32:24.099177 datar-0.9.0/datar/datasets/faithfuld.csv.gz
--rw-r--r--   0        0        0      410 2022-09-14 05:32:24.099177 datar-0.9.0/datar/datasets/fish_encounters.csv.gz
--rw-r--r--   0        0        0  8242566 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/flights.csv.gz
--rw-r--r--   0        0        0   152654 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/gss_cat.csv.gz
--rw-r--r--   0        0        0      865 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/iris.csv.gz
--rw-r--r--   0        0        0    15922 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/luv_colours.csv.gz
--rw-r--r--   0        0        0     8816 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/metadata.toml
--rw-r--r--   0        0        0    46964 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/midwest.csv.gz
--rw-r--r--   0        0        0     1904 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/mpg.csv.gz
--rw-r--r--   0        0        0     2505 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/msleep.csv.gz
--rw-r--r--   0        0        0      891 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/mtcars.csv.gz
--rw-r--r--   0        0        0    15627 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/planes.csv.gz
--rw-r--r--   0        0        0    31014 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/population.csv.gz
--rw-r--r--   0        0        0      221 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/presidential.csv.gz
--rw-r--r--   0        0        0      606 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/relig_income.csv.gz
--rw-r--r--   0        0        0    23931 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/seals.csv.gz
--rw-r--r--   0        0        0      103 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/smiths.csv.gz
--rw-r--r--   0        0        0     2423 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/starwars.csv.gz
--rw-r--r--   0        0        0      142 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/state_abb.csv.gz
--rw-r--r--   0        0        0      200 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/state_division.csv.gz
--rw-r--r--   0        0        0      125 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/state_region.csv.gz
--rw-r--r--   0        0        0   105912 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/storms.csv.gz
--rw-r--r--   0        0        0      177 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/table1.csv.gz
--rw-r--r--   0        0        0      202 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/table2.csv.gz
--rw-r--r--   0        0        0      170 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/table3.csv.gz
--rw-r--r--   0        0        0      114 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/table4a.csv.gz
--rw-r--r--   0        0        0      128 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/table4b.csv.gz
--rw-r--r--   0        0        0      178 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/table5.csv.gz
--rw-r--r--   0        0        0      236 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/toothgrowth.csv.gz
--rw-r--r--   0        0        0   145001 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/txhousing.csv.gz
--rw-r--r--   0        0        0     1226 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/us_rent_income.csv.gz
--rw-r--r--   0        0        0      186 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/warpbreaks.csv.gz
--rw-r--r--   0        0        0   403158 2022-09-14 05:32:24.115177 datar-0.9.0/datar/datasets/weather.csv.gz
--rw-r--r--   0        0        0   142951 2022-09-14 05:32:24.119177 datar-0.9.0/datar/datasets/who.csv.gz
--rw-r--r--   0        0        0   121581 2022-09-14 05:32:24.119177 datar-0.9.0/datar/datasets/world_bank_pop.csv.gz
--rw-r--r--   0        0        0     2303 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/__init__.py
--rw-r--r--   0        0        0     4444 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/_rank.py
--rw-r--r--   0        0        0     9377 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/across.py
--rw-r--r--   0        0        0     2109 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/arrange.py
--rw-r--r--   0        0        0     5786 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/bind.py
--rw-r--r--   0        0        0     4016 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/context.py
--rw-r--r--   0        0        0     4917 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/count_tally.py
--rw-r--r--   0        0        0      920 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/desc.py
--rw-r--r--   0        0        0     1890 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/dfilter.py
--rw-r--r--   0        0        0     3052 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/distinct.py
--rw-r--r--   0        0        0    10764 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/dslice.py
--rw-r--r--   0        0        0     5612 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/funs.py
--rw-r--r--   0        0        0     5012 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/glimpse.py
--rw-r--r--   0        0        0     6322 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/group_by.py
--rw-r--r--   0        0        0     3987 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/group_data.py
--rw-r--r--   0        0        0     6641 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/group_iter.py
--rw-r--r--   0        0        0     3731 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/if_else.py
--rw-r--r--   0        0        0     8510 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/join.py
--rw-r--r--   0        0        0     1608 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/lead_lag.py
--rw-r--r--   0        0        0     6655 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/mutate.py
--rw-r--r--   0        0        0     3099 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/order_by.py
--rw-r--r--   0        0        0     4328 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/pull.py
--rw-r--r--   0        0        0     2596 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/rank.py
--rw-r--r--   0        0        0     9683 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/recode.py
--rw-r--r--   0        0        0     3167 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/relocate.py
--rw-r--r--   0        0        0     2264 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/rename.py
--rw-r--r--   0        0        0     8789 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/rows.py
--rw-r--r--   0        0        0     2947 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/select.py
--rw-r--r--   0        0        0     5386 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/sets.py
--rw-r--r--   0        0        0     6222 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/summarise.py
--rw-r--r--   0        0        0     8855 2022-09-14 05:32:24.119177 datar-0.9.0/datar/dplyr/tidyselect.py
--rw-r--r--   0        0        0      720 2022-09-14 05:32:24.119177 datar-0.9.0/datar/forcats/__init__.py
--rw-r--r--   0        0        0     1581 2022-09-14 05:32:24.119177 datar-0.9.0/datar/forcats/fct_multi.py
--rw-r--r--   0        0        0     3494 2022-09-14 05:32:24.119177 datar-0.9.0/datar/forcats/lvl_addrm.py
--rw-r--r--   0        0        0     9905 2022-09-14 05:32:24.119177 datar-0.9.0/datar/forcats/lvl_order.py
--rw-r--r--   0        0        0    14210 2022-09-14 05:32:24.119177 datar-0.9.0/datar/forcats/lvl_value.py
--rw-r--r--   0        0        0     4043 2022-09-14 05:32:24.119177 datar-0.9.0/datar/forcats/lvls.py
--rw-r--r--   0        0        0     2612 2022-09-14 05:32:24.119177 datar-0.9.0/datar/forcats/misc.py
--rw-r--r--   0        0        0      583 2022-09-14 05:32:24.119177 datar-0.9.0/datar/forcats/utils.py
--rw-r--r--   0        0        0      702 2022-09-14 05:32:24.119177 datar-0.9.0/datar/testing.py
--rw-r--r--   0        0        0      382 2022-09-14 05:32:24.119177 datar-0.9.0/datar/tibble/__init__.py
--rw-r--r--   0        0        0     5501 2022-09-14 05:32:24.119177 datar-0.9.0/datar/tibble/tibble.py
--rw-r--r--   0        0        0     9580 2022-09-14 05:32:24.119177 datar-0.9.0/datar/tibble/verbs.py
--rw-r--r--   0        0        0      532 2022-09-14 05:32:24.119177 datar-0.9.0/datar/tidyr/__init__.py
--rw-r--r--   0        0        0     8083 2022-09-14 05:32:24.119177 datar-0.9.0/datar/tidyr/chop.py
--rw-r--r--   0        0        0     1844 2022-09-14 05:32:24.119177 datar-0.9.0/datar/tidyr/complete.py
--rw-r--r--   0        0        0     1320 2022-09-14 05:32:24.119177 datar-0.9.0/datar/tidyr/drop_na.py
--rw-r--r--   0        0        0    12949 2022-09-14 05:32:24.119177 datar-0.9.0/datar/tidyr/expand.py
--rw-r--r--   0        0        0     2990 2022-09-14 05:32:24.119177 datar-0.9.0/datar/tidyr/extract.py
--rw-r--r--   0        0        0     2035 2022-09-14 05:32:24.119177 datar-0.9.0/datar/tidyr/fill.py
--rw-r--r--   0        0        0      825 2022-09-14 05:32:24.119177 datar-0.9.0/datar/tidyr/funcs.py
--rw-r--r--   0        0        0     9195 2022-09-14 05:32:24.119177 datar-0.9.0/datar/tidyr/nest.py
--rw-r--r--   0        0        0     5041 2022-09-14 05:32:24.123177 datar-0.9.0/datar/tidyr/pack.py
--rw-r--r--   0        0        0    10116 2022-09-14 05:32:24.123177 datar-0.9.0/datar/tidyr/pivot_long.py
--rw-r--r--   0        0        0     7374 2022-09-14 05:32:24.123177 datar-0.9.0/datar/tidyr/pivot_wide.py
--rw-r--r--   0        0        0     2304 2022-09-14 05:32:24.123177 datar-0.9.0/datar/tidyr/replace_na.py
--rw-r--r--   0        0        0     6855 2022-09-14 05:32:24.123177 datar-0.9.0/datar/tidyr/separate.py
--rw-r--r--   0        0        0     2093 2022-09-14 05:32:24.123177 datar-0.9.0/datar/tidyr/uncount.py
--rw-r--r--   0        0        0     2061 2022-09-14 05:32:24.123177 datar-0.9.0/datar/tidyr/unite.py
--rw-r--r--   0        0        0     1706 2022-09-14 05:32:24.135177 datar-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5215 1970-01-01 00:00:00.000000 datar-0.9.0/setup.py
--rw-r--r--   0        0        0     4948 1970-01-01 00:00:00.000000 datar-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-10-13 19:29:34.090123 datar-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3865 2022-10-13 19:29:34.090123 datar-0.9.1/README.md
+-rw-r--r--   0        0        0     1447 2022-10-13 19:29:34.090123 datar-0.9.1/datar/__init__.py
+-rw-r--r--   0        0        0      887 2022-10-13 19:29:34.090123 datar-0.9.1/datar/all.py
+-rw-r--r--   0        0        0     3320 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/__init__.py
+-rw-r--r--   0        0        0    21342 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/arithmetic.py
+-rw-r--r--   0        0        0     3837 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/bessel.py
+-rw-r--r--   0        0        0     3402 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/casting.py
+-rw-r--r--   0        0        0     2657 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/complex.py
+-rw-r--r--   0        0        0      565 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/constants.py
+-rw-r--r--   0        0        0     1514 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/cum.py
+-rw-r--r--   0        0        0     4579 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/date.py
+-rw-r--r--   0        0        0     4104 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/factor.py
+-rw-r--r--   0        0        0     7822 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/funs.py
+-rw-r--r--   0        0        0     1887 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/logical.py
+-rw-r--r--   0        0        0     2365 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/na.py
+-rw-r--r--   0        0        0      640 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/null.py
+-rw-r--r--   0        0        0      203 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/random.py
+-rw-r--r--   0        0        0     5073 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/rep.py
+-rw-r--r--   0        0        0    10154 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/seq.py
+-rw-r--r--   0        0        0     5133 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/special.py
+-rw-r--r--   0        0        0     3682 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/stats.py
+-rw-r--r--   0        0        0    15226 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/string.py
+-rw-r--r--   0        0        0     6482 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/table.py
+-rw-r--r--   0        0        0     4469 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/testing.py
+-rw-r--r--   0        0        0     4562 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/trig_hb.py
+-rw-r--r--   0        0        0    12664 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/verbs.py
+-rw-r--r--   0        0        0     1237 2022-10-13 19:29:34.090123 datar-0.9.1/datar/base/which.py
+-rw-r--r--   0        0        0      149 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/__init__.py
+-rw-r--r--   0        0        0       66 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/backends/__init__.py
+-rw-r--r--   0        0        0      888 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/backends/pandas/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/backends/pandas/api/__init__.py
+-rw-r--r--   0        0        0      306 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/backends/pandas/api/types.py
+-rw-r--r--   0        0        0        0 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/backends/pandas/core/__init__.py
+-rw-r--r--   0        0        0       42 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/backends/pandas/core/base.py
+-rw-r--r--   0        0        0       40 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/backends/pandas/core/generic.py
+-rw-r--r--   0        0        0      316 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/backends/pandas/core/groupby.py
+-rw-r--r--   0        0        0      105 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/backends/pandas/testing.py
+-rw-r--r--   0        0        0    23702 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/broadcast.py
+-rw-r--r--   0        0        0    12639 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/collections.py
+-rw-r--r--   0        0        0     1456 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/contexts.py
+-rw-r--r--   0        0        0      133 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/defaults.py
+-rw-r--r--   0        0        0      100 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/exceptions.py
+-rw-r--r--   0        0        0    28275 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/factory.py
+-rw-r--r--   0        0        0     2328 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/import_names_conflict.py
+-rw-r--r--   0        0        0      657 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/middlewares.py
+-rw-r--r--   0        0        0     5370 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/names.py
+-rw-r--r--   0        0        0     4842 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/operator.py
+-rw-r--r--   0        0        0     4223 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/options.py
+-rw-r--r--   0        0        0    15187 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/tibble.py
+-rw-r--r--   0        0        0     4209 2022-10-13 19:29:34.090123 datar-0.9.1/datar/core/utils.py
+-rw-r--r--   0        0        0      143 2022-10-13 19:29:34.090123 datar-0.9.1/datar/datar/__init__.py
+-rw-r--r--   0        0        0     4323 2022-10-13 19:29:34.090123 datar-0.9.1/datar/datar/funcs.py
+-rw-r--r--   0        0        0     2053 2022-10-13 19:29:34.090123 datar-0.9.1/datar/datar/verbs.py
+-rw-r--r--   0        0        0     1102 2022-10-13 19:29:34.090123 datar-0.9.1/datar/datasets/__init__.py
+-rw-r--r--   0        0        0      242 2022-10-13 19:29:34.090123 datar-0.9.1/datar/datasets/airlines.csv.gz
+-rw-r--r--   0        0        0    37924 2022-10-13 19:29:34.090123 datar-0.9.1/datar/datasets/airports.csv.gz
+-rw-r--r--   0        0        0     1300 2022-10-13 19:29:34.090123 datar-0.9.1/datar/datasets/airquality.csv.gz
+-rw-r--r--   0        0        0      211 2022-10-13 19:29:34.090123 datar-0.9.1/datar/datasets/anscombe.csv.gz
+-rw-r--r--   0        0        0       88 2022-10-13 19:29:34.090123 datar-0.9.1/datar/datasets/band_instruments.csv.gz
+-rw-r--r--   0        0        0       91 2022-10-13 19:29:34.090123 datar-0.9.1/datar/datasets/band_instruments2.csv.gz
+-rw-r--r--   0        0        0       84 2022-10-13 19:29:34.090123 datar-0.9.1/datar/datasets/band_members.csv.gz
+-rw-r--r--   0        0        0    13706 2022-10-13 19:29:34.090123 datar-0.9.1/datar/datasets/billboard.csv.gz
+-rw-r--r--   0        0        0     1995 2022-10-13 19:29:34.090123 datar-0.9.1/datar/datasets/chickweight.csv.gz
+-rw-r--r--   0        0        0      305 2022-10-13 19:29:34.090123 datar-0.9.1/datar/datasets/construction.csv.gz
+-rw-r--r--   0        0        0   445681 2022-10-13 19:29:34.094123 datar-0.9.1/datar/datasets/diamonds.csv.gz
+-rw-r--r--   0        0        0     8780 2022-10-13 19:29:34.094123 datar-0.9.1/datar/datasets/economics.csv.gz
+-rw-r--r--   0        0        0    33152 2022-10-13 19:29:34.094123 datar-0.9.1/datar/datasets/economics_long.csv.gz
+-rw-r--r--   0        0        0      883 2022-10-13 19:29:34.094123 datar-0.9.1/datar/datasets/faithful.csv.gz
+-rw-r--r--   0        0        0    71260 2022-10-13 19:29:34.094123 datar-0.9.1/datar/datasets/faithfuld.csv.gz
+-rw-r--r--   0        0        0      410 2022-10-13 19:29:34.094123 datar-0.9.1/datar/datasets/fish_encounters.csv.gz
+-rw-r--r--   0        0        0  8242566 2022-10-13 19:29:34.106123 datar-0.9.1/datar/datasets/flights.csv.gz
+-rw-r--r--   0        0        0   152654 2022-10-13 19:29:34.106123 datar-0.9.1/datar/datasets/gss_cat.csv.gz
+-rw-r--r--   0        0        0      865 2022-10-13 19:29:34.106123 datar-0.9.1/datar/datasets/iris.csv.gz
+-rw-r--r--   0        0        0    15922 2022-10-13 19:29:34.106123 datar-0.9.1/datar/datasets/luv_colours.csv.gz
+-rw-r--r--   0        0        0     8816 2022-10-13 19:29:34.106123 datar-0.9.1/datar/datasets/metadata.toml
+-rw-r--r--   0        0        0    46964 2022-10-13 19:29:34.106123 datar-0.9.1/datar/datasets/midwest.csv.gz
+-rw-r--r--   0        0        0     1904 2022-10-13 19:29:34.106123 datar-0.9.1/datar/datasets/mpg.csv.gz
+-rw-r--r--   0        0        0     2505 2022-10-13 19:29:34.106123 datar-0.9.1/datar/datasets/msleep.csv.gz
+-rw-r--r--   0        0        0      891 2022-10-13 19:29:34.106123 datar-0.9.1/datar/datasets/mtcars.csv.gz
+-rw-r--r--   0        0        0    15627 2022-10-13 19:29:34.106123 datar-0.9.1/datar/datasets/planes.csv.gz
+-rw-r--r--   0        0        0    31014 2022-10-13 19:29:34.106123 datar-0.9.1/datar/datasets/population.csv.gz
+-rw-r--r--   0        0        0      221 2022-10-13 19:29:34.106123 datar-0.9.1/datar/datasets/presidential.csv.gz
+-rw-r--r--   0        0        0      606 2022-10-13 19:29:34.106123 datar-0.9.1/datar/datasets/relig_income.csv.gz
+-rw-r--r--   0        0        0    23931 2022-10-13 19:29:34.106123 datar-0.9.1/datar/datasets/seals.csv.gz
+-rw-r--r--   0        0        0      103 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/smiths.csv.gz
+-rw-r--r--   0        0        0     2423 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/starwars.csv.gz
+-rw-r--r--   0        0        0      142 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/state_abb.csv.gz
+-rw-r--r--   0        0        0      200 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/state_division.csv.gz
+-rw-r--r--   0        0        0      125 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/state_region.csv.gz
+-rw-r--r--   0        0        0   105912 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/storms.csv.gz
+-rw-r--r--   0        0        0      177 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/table1.csv.gz
+-rw-r--r--   0        0        0      202 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/table2.csv.gz
+-rw-r--r--   0        0        0      170 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/table3.csv.gz
+-rw-r--r--   0        0        0      114 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/table4a.csv.gz
+-rw-r--r--   0        0        0      128 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/table4b.csv.gz
+-rw-r--r--   0        0        0      178 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/table5.csv.gz
+-rw-r--r--   0        0        0      236 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/toothgrowth.csv.gz
+-rw-r--r--   0        0        0   145001 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/txhousing.csv.gz
+-rw-r--r--   0        0        0     1226 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/us_rent_income.csv.gz
+-rw-r--r--   0        0        0      186 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/warpbreaks.csv.gz
+-rw-r--r--   0        0        0   403158 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/weather.csv.gz
+-rw-r--r--   0        0        0   142951 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/who.csv.gz
+-rw-r--r--   0        0        0   121581 2022-10-13 19:29:34.110123 datar-0.9.1/datar/datasets/world_bank_pop.csv.gz
+-rw-r--r--   0        0        0     2303 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/__init__.py
+-rw-r--r--   0        0        0     4444 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/_rank.py
+-rw-r--r--   0        0        0     9377 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/across.py
+-rw-r--r--   0        0        0     2109 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/arrange.py
+-rw-r--r--   0        0        0     5786 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/bind.py
+-rw-r--r--   0        0        0     4016 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/context.py
+-rw-r--r--   0        0        0     4917 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/count_tally.py
+-rw-r--r--   0        0        0      920 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/desc.py
+-rw-r--r--   0        0        0     1890 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/dfilter.py
+-rw-r--r--   0        0        0     3052 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/distinct.py
+-rw-r--r--   0        0        0    10764 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/dslice.py
+-rw-r--r--   0        0        0     5612 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/funs.py
+-rw-r--r--   0        0        0     5012 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/glimpse.py
+-rw-r--r--   0        0        0     6322 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/group_by.py
+-rw-r--r--   0        0        0     4178 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/group_data.py
+-rw-r--r--   0        0        0     6641 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/group_iter.py
+-rw-r--r--   0        0        0     3731 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/if_else.py
+-rw-r--r--   0        0        0     8510 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/join.py
+-rw-r--r--   0        0        0     1608 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/lead_lag.py
+-rw-r--r--   0        0        0     6655 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/mutate.py
+-rw-r--r--   0        0        0     3099 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/order_by.py
+-rw-r--r--   0        0        0     4328 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/pull.py
+-rw-r--r--   0        0        0     2596 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/rank.py
+-rw-r--r--   0        0        0     9683 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/recode.py
+-rw-r--r--   0        0        0     3167 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/relocate.py
+-rw-r--r--   0        0        0     2264 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/rename.py
+-rw-r--r--   0        0        0     8789 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/rows.py
+-rw-r--r--   0        0        0     2947 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/select.py
+-rw-r--r--   0        0        0     5386 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/sets.py
+-rw-r--r--   0        0        0     6222 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/summarise.py
+-rw-r--r--   0        0        0     8855 2022-10-13 19:29:34.110123 datar-0.9.1/datar/dplyr/tidyselect.py
+-rw-r--r--   0        0        0      720 2022-10-13 19:29:34.110123 datar-0.9.1/datar/forcats/__init__.py
+-rw-r--r--   0        0        0     1581 2022-10-13 19:29:34.110123 datar-0.9.1/datar/forcats/fct_multi.py
+-rw-r--r--   0        0        0     3494 2022-10-13 19:29:34.110123 datar-0.9.1/datar/forcats/lvl_addrm.py
+-rw-r--r--   0        0        0     9905 2022-10-13 19:29:34.110123 datar-0.9.1/datar/forcats/lvl_order.py
+-rw-r--r--   0        0        0    14210 2022-10-13 19:29:34.114123 datar-0.9.1/datar/forcats/lvl_value.py
+-rw-r--r--   0        0        0     4043 2022-10-13 19:29:34.114123 datar-0.9.1/datar/forcats/lvls.py
+-rw-r--r--   0        0        0     2612 2022-10-13 19:29:34.114123 datar-0.9.1/datar/forcats/misc.py
+-rw-r--r--   0        0        0      583 2022-10-13 19:29:34.114123 datar-0.9.1/datar/forcats/utils.py
+-rw-r--r--   0        0        0      702 2022-10-13 19:29:34.114123 datar-0.9.1/datar/testing.py
+-rw-r--r--   0        0        0      382 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tibble/__init__.py
+-rw-r--r--   0        0        0     5501 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tibble/tibble.py
+-rw-r--r--   0        0        0     9580 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tibble/verbs.py
+-rw-r--r--   0        0        0      532 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/__init__.py
+-rw-r--r--   0        0        0     8083 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/chop.py
+-rw-r--r--   0        0        0     1844 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/complete.py
+-rw-r--r--   0        0        0     1320 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/drop_na.py
+-rw-r--r--   0        0        0    12949 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/expand.py
+-rw-r--r--   0        0        0     2990 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/extract.py
+-rw-r--r--   0        0        0     2035 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/fill.py
+-rw-r--r--   0        0        0      825 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/funcs.py
+-rw-r--r--   0        0        0     9195 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/nest.py
+-rw-r--r--   0        0        0     5041 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/pack.py
+-rw-r--r--   0        0        0    10116 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/pivot_long.py
+-rw-r--r--   0        0        0     7374 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/pivot_wide.py
+-rw-r--r--   0        0        0     2304 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/replace_na.py
+-rw-r--r--   0        0        0     6855 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/separate.py
+-rw-r--r--   0        0        0     2093 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/uncount.py
+-rw-r--r--   0        0        0     2061 2022-10-13 19:29:34.114123 datar-0.9.1/datar/tidyr/unite.py
+-rw-r--r--   0        0        0     1704 2022-10-13 19:29:34.126123 datar-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5211 1970-01-01 00:00:00.000000 datar-0.9.1/setup.py
+-rw-r--r--   0        0        0     4995 1970-01-01 00:00:00.000000 datar-0.9.1/PKG-INFO
```

### Comparing `datar-0.9.0/LICENSE` & `datar-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/README.md` & `datar-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/__init__.py` & `datar-0.9.1/datar/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "options_context",
     "add_option",
     "get_option",
     "logger",
 )
 
 __all__ = ("f", "get_versions")
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 apply_init_callbacks()
 
 
 def get_versions(prnt: bool = True):
     """Print or return related versions which help for bug reporting.
```

### Comparing `datar-0.9.0/datar/all.py` & `datar-0.9.1/datar/all.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/__init__.py` & `datar-0.9.1/datar/base/__init__.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/arithmetic.py` & `datar-0.9.1/datar/base/arithmetic.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/bessel.py` & `datar-0.9.1/datar/base/bessel.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/casting.py` & `datar-0.9.1/datar/base/casting.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/complex.py` & `datar-0.9.1/datar/base/complex.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/constants.py` & `datar-0.9.1/datar/base/constants.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/cum.py` & `datar-0.9.1/datar/base/cum.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/date.py` & `datar-0.9.1/datar/base/date.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/factor.py` & `datar-0.9.1/datar/base/factor.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/funs.py` & `datar-0.9.1/datar/base/funs.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/logical.py` & `datar-0.9.1/datar/base/logical.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/na.py` & `datar-0.9.1/datar/base/na.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/null.py` & `datar-0.9.1/datar/base/null.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/rep.py` & `datar-0.9.1/datar/base/rep.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/seq.py` & `datar-0.9.1/datar/base/seq.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/special.py` & `datar-0.9.1/datar/base/special.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/stats.py` & `datar-0.9.1/datar/base/stats.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/string.py` & `datar-0.9.1/datar/base/string.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/table.py` & `datar-0.9.1/datar/base/table.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/testing.py` & `datar-0.9.1/datar/base/testing.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/trig_hb.py` & `datar-0.9.1/datar/base/trig_hb.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/verbs.py` & `datar-0.9.1/datar/base/verbs.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/base/which.py` & `datar-0.9.1/datar/base/which.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/core/backends/pandas/__init__.py` & `datar-0.9.1/datar/core/backends/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/core/broadcast.py` & `datar-0.9.1/datar/core/broadcast.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/core/collections.py` & `datar-0.9.1/datar/core/collections.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/core/contexts.py` & `datar-0.9.1/datar/core/contexts.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/core/factory.py` & `datar-0.9.1/datar/core/factory.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/core/import_names_conflict.py` & `datar-0.9.1/datar/core/import_names_conflict.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/core/middlewares.py` & `datar-0.9.1/datar/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/core/names.py` & `datar-0.9.1/datar/core/names.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/core/operator.py` & `datar-0.9.1/datar/core/operator.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/core/options.py` & `datar-0.9.1/datar/core/options.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/core/tibble.py` & `datar-0.9.1/datar/core/tibble.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/core/utils.py` & `datar-0.9.1/datar/core/utils.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datar/funcs.py` & `datar-0.9.1/datar/datar/funcs.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datar/verbs.py` & `datar-0.9.1/datar/datar/verbs.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/__init__.py` & `datar-0.9.1/datar/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/airports.csv.gz` & `datar-0.9.1/datar/datasets/airports.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/airquality.csv.gz` & `datar-0.9.1/datar/datasets/airquality.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/billboard.csv.gz` & `datar-0.9.1/datar/datasets/billboard.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/chickweight.csv.gz` & `datar-0.9.1/datar/datasets/chickweight.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/diamonds.csv.gz` & `datar-0.9.1/datar/datasets/diamonds.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/economics.csv.gz` & `datar-0.9.1/datar/datasets/economics.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/economics_long.csv.gz` & `datar-0.9.1/datar/datasets/economics_long.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/faithful.csv.gz` & `datar-0.9.1/datar/datasets/faithful.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/faithfuld.csv.gz` & `datar-0.9.1/datar/datasets/faithfuld.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/flights.csv.gz` & `datar-0.9.1/datar/datasets/flights.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/gss_cat.csv.gz` & `datar-0.9.1/datar/datasets/gss_cat.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/iris.csv.gz` & `datar-0.9.1/datar/datasets/iris.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/luv_colours.csv.gz` & `datar-0.9.1/datar/datasets/luv_colours.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/metadata.toml` & `datar-0.9.1/datar/datasets/metadata.toml`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/midwest.csv.gz` & `datar-0.9.1/datar/datasets/midwest.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/mpg.csv.gz` & `datar-0.9.1/datar/datasets/mpg.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/msleep.csv.gz` & `datar-0.9.1/datar/datasets/msleep.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/mtcars.csv.gz` & `datar-0.9.1/datar/datasets/mtcars.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/planes.csv.gz` & `datar-0.9.1/datar/datasets/planes.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/population.csv.gz` & `datar-0.9.1/datar/datasets/population.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/relig_income.csv.gz` & `datar-0.9.1/datar/datasets/relig_income.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/seals.csv.gz` & `datar-0.9.1/datar/datasets/seals.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/starwars.csv.gz` & `datar-0.9.1/datar/datasets/starwars.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/storms.csv.gz` & `datar-0.9.1/datar/datasets/storms.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/txhousing.csv.gz` & `datar-0.9.1/datar/datasets/txhousing.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/us_rent_income.csv.gz` & `datar-0.9.1/datar/datasets/us_rent_income.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/weather.csv.gz` & `datar-0.9.1/datar/datasets/weather.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/who.csv.gz` & `datar-0.9.1/datar/datasets/who.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/datasets/world_bank_pop.csv.gz` & `datar-0.9.1/datar/datasets/world_bank_pop.csv.gz`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/__init__.py` & `datar-0.9.1/datar/dplyr/__init__.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/_rank.py` & `datar-0.9.1/datar/dplyr/_rank.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/across.py` & `datar-0.9.1/datar/dplyr/across.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/arrange.py` & `datar-0.9.1/datar/dplyr/arrange.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/bind.py` & `datar-0.9.1/datar/dplyr/bind.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/context.py` & `datar-0.9.1/datar/dplyr/context.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/count_tally.py` & `datar-0.9.1/datar/dplyr/count_tally.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/desc.py` & `datar-0.9.1/datar/dplyr/desc.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/dfilter.py` & `datar-0.9.1/datar/dplyr/dfilter.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/distinct.py` & `datar-0.9.1/datar/dplyr/distinct.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/dslice.py` & `datar-0.9.1/datar/dplyr/dslice.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/funs.py` & `datar-0.9.1/datar/dplyr/funs.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/glimpse.py` & `datar-0.9.1/datar/dplyr/glimpse.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/group_by.py` & `datar-0.9.1/datar/dplyr/group_by.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/group_data.py` & `datar-0.9.1/datar/dplyr/group_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 from typing import List, Sequence, Union
 
 from pipda import register_verb
 
 from ..core.backends.pandas import DataFrame
 from ..core.backends.pandas.core.groupby import GroupBy
 
+from ..core.contexts import Context
+
 from ..core.tibble import Tibble, TibbleGrouped, TibbleRowwise
 from ..core.utils import dict_get
 
 
-@register_verb(DataFrame)
+@register_verb(DataFrame, context=Context.EVAL)
 def group_data(_data: DataFrame) -> Tibble:
     """Returns a data frame that defines the grouping structure.
 
     Args:
         _data: The data frame
 
     Returns:
@@ -30,15 +32,15 @@
 @group_data.register((TibbleGrouped, GroupBy))
 def _(_data: Union[TibbleGrouped, GroupBy]) -> Tibble:
     gpdata = group_keys(_data, __ast_fallback="normal")
     gpdata["_rows"] = group_rows(_data, __ast_fallback="normal")
     return gpdata
 
 
-@register_verb(DataFrame)
+@register_verb(DataFrame, context=Context.EVAL)
 def group_keys(_data: DataFrame) -> Tibble:
     """Just grouping data without the `_rows` columns
 
     Note:
         Additional arguments to select columns in dplyr are deprecated.
         Here we don't support it ahead.
 
@@ -64,15 +66,15 @@
 
 
 @group_keys.register(TibbleRowwise)
 def _(_data: TibbleRowwise) -> Tibble:
     return Tibble(_data.loc[:, _data.group_vars])
 
 
-@register_verb(DataFrame)
+@register_verb(DataFrame, context=Context.EVAL)
 def group_rows(_data: DataFrame) -> List[List[int]]:
     """The locations of grouping structure, always 0-based."""
     rows = list(range(_data.shape[0]))
     return [rows]
 
 
 @group_rows.register(TibbleGrouped)
@@ -87,15 +89,15 @@
     grouper = _data.grouper
     return [
         list(dict_get(grouper.indices, group_key))
         for group_key in grouper.result_index
     ]
 
 
-@register_verb(DataFrame)
+@register_verb(DataFrame, context=Context.EVAL)
 def group_indices(_data: DataFrame) -> List[int]:
     """Returns an integer vector the same length as `_data`.
 
     Always 0-based.
     """
     return [0] * _data.shape[0]
 
@@ -105,37 +107,37 @@
     ret = {}
     for row in group_data(_data, __ast_fallback="normal").itertuples():
         for index in row[-1]:
             ret[index] = row.Index
     return [ret[key] for key in sorted(ret)]
 
 
-@register_verb(DataFrame)
+@register_verb(DataFrame, context=Context.EVAL)
 def group_vars(_data: DataFrame) -> Sequence[str]:
     """Gives names of grouping variables as character vector"""
     return getattr(_data, "group_vars", [])
 
 
 # groups in dplyr returns R list
 groups = group_vars
 group_cols = group_vars
 
 
-@register_verb(DataFrame)
+@register_verb(DataFrame, context=Context.EVAL)
 def group_size(_data: DataFrame) -> Sequence[int]:
     """Gives the size of each group"""
     return [_data.shape[0]]
 
 
 @group_size.register(TibbleGrouped)
 def _(_data: TibbleGrouped) -> Sequence[int]:
     return list(map(len, group_rows(_data, __ast_fallback="normal")))
 
 
-@register_verb(DataFrame)
+@register_verb(DataFrame, context=Context.EVAL)
 def n_groups(_data: DataFrame) -> int:
     """Gives the total number of groups."""
     return 1
 
 
 @n_groups.register(TibbleGrouped)
 def _(_data: TibbleGrouped) -> int:
```

### Comparing `datar-0.9.0/datar/dplyr/group_iter.py` & `datar-0.9.1/datar/dplyr/group_iter.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/if_else.py` & `datar-0.9.1/datar/dplyr/if_else.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/join.py` & `datar-0.9.1/datar/dplyr/join.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/lead_lag.py` & `datar-0.9.1/datar/dplyr/lead_lag.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/mutate.py` & `datar-0.9.1/datar/dplyr/mutate.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/order_by.py` & `datar-0.9.1/datar/dplyr/order_by.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/pull.py` & `datar-0.9.1/datar/dplyr/pull.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/rank.py` & `datar-0.9.1/datar/dplyr/rank.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/recode.py` & `datar-0.9.1/datar/dplyr/recode.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/relocate.py` & `datar-0.9.1/datar/dplyr/relocate.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/rename.py` & `datar-0.9.1/datar/dplyr/rename.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/rows.py` & `datar-0.9.1/datar/dplyr/rows.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/select.py` & `datar-0.9.1/datar/dplyr/select.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/sets.py` & `datar-0.9.1/datar/dplyr/sets.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/summarise.py` & `datar-0.9.1/datar/dplyr/summarise.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/dplyr/tidyselect.py` & `datar-0.9.1/datar/dplyr/tidyselect.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/forcats/__init__.py` & `datar-0.9.1/datar/forcats/__init__.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/forcats/fct_multi.py` & `datar-0.9.1/datar/forcats/fct_multi.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/forcats/lvl_addrm.py` & `datar-0.9.1/datar/forcats/lvl_addrm.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/forcats/lvl_order.py` & `datar-0.9.1/datar/forcats/lvl_order.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/forcats/lvl_value.py` & `datar-0.9.1/datar/forcats/lvl_value.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/forcats/lvls.py` & `datar-0.9.1/datar/forcats/lvls.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/forcats/misc.py` & `datar-0.9.1/datar/forcats/misc.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/forcats/utils.py` & `datar-0.9.1/datar/forcats/utils.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/testing.py` & `datar-0.9.1/datar/testing.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tibble/tibble.py` & `datar-0.9.1/datar/tibble/tibble.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tibble/verbs.py` & `datar-0.9.1/datar/tibble/verbs.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/__init__.py` & `datar-0.9.1/datar/tidyr/__init__.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/chop.py` & `datar-0.9.1/datar/tidyr/chop.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/complete.py` & `datar-0.9.1/datar/tidyr/complete.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/drop_na.py` & `datar-0.9.1/datar/tidyr/drop_na.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/expand.py` & `datar-0.9.1/datar/tidyr/expand.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/extract.py` & `datar-0.9.1/datar/tidyr/extract.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/fill.py` & `datar-0.9.1/datar/tidyr/fill.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/funcs.py` & `datar-0.9.1/datar/tidyr/funcs.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/nest.py` & `datar-0.9.1/datar/tidyr/nest.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/pack.py` & `datar-0.9.1/datar/tidyr/pack.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/pivot_long.py` & `datar-0.9.1/datar/tidyr/pivot_long.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/pivot_wide.py` & `datar-0.9.1/datar/tidyr/pivot_wide.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/replace_na.py` & `datar-0.9.1/datar/tidyr/replace_na.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/separate.py` & `datar-0.9.1/datar/tidyr/separate.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/uncount.py` & `datar-0.9.1/datar/tidyr/uncount.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/datar/tidyr/unite.py` & `datar-0.9.1/datar/tidyr/unite.py`

 * *Files identical despite different names*

### Comparing `datar-0.9.0/pyproject.toml` & `datar-0.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "datar"
-version = "0.9.0"
+version = "0.9.1"
 description = "Port of dplyr and other related R packages in python, using pipda."
 authors = ["pwwang <pwwang@pwwang.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/pwwang/datar"
 repository = "https://github.com/pwwang/datar"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"  # required by modin 0.10.2
-pipda = "^0.7.1"
+pipda = "^0.8"
 ## included in python-simpleconf
 # diot = "^0.1"
 ## included in pipda
 # executing = "*"
 # varname = "*"
 pandas = "^1.3"
 pdtypes = "^0.0"
```

### Comparing `datar-0.9.0/setup.py` & `datar-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,26 +18,26 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.3,<2.0',
  'pdtypes>=0.0,<0.1',
- 'pipda>=0.7.1,<0.8.0',
+ 'pipda>=0.8,<0.9',
  'python-simpleconf[toml]>=0.5,<0.6']
 
 extras_require = \
 {'modin': ['modin>=0.10,<0.11'],
  'scipy': ['scipy>=1.6,<2.0'],
  'slugify': ['python-slugify>=6,<7'],
  'wcwidth': ['wcwidth>=0.2,<0.3']}
 
 setup_kwargs = {
     'name': 'datar',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Port of dplyr and other related R packages in python, using pipda.',
     'long_description': '# datar\n\nA Grammar of Data Manipulation in python\n\n<!-- badges -->\n[![Pypi][6]][7] [![Github][8]][9] ![Building][10] [![Docs and API][11]][5] [![Codacy][12]][13] [![Codacy coverage][14]][13]\n\n[Documentation][5] | [Reference Maps][15] | [Notebook Examples][16] | [API][17] | [Blog][18]\n\n<img width="30%" style="margin: 10px 10px 10px 30px" align="right" src="logo.png">\n\n`datar` is a re-imagining of APIs of data manipulation libraries in python (currently only `pandas` supported) so that you can manipulate your data with it like with `dplyr` in `R`.\n\n`datar` is an in-depth port of `tidyverse` packages, such as `dplyr`, `tidyr`, `forcats` and `tibble`, as well as some functions from base R.\n\n## Installation\n\n```shell\npip install -U datar\n\n# install pdtypes support\npip install -U datar[pdtypes]\n\n# install dependencies for modin as backend\npip install -U datar[modin]\n# you may also need to install dependencies for modin engines\n# pip install -U modin[ray]\n```\n\n## Example usage\n\n```python\nfrom datar import f\nfrom datar.dplyr import mutate, filter, if_else\nfrom datar.tibble import tibble\n# or\n# from datar.all import f, mutate, filter, if_else, tibble\n\ndf = tibble(\n    x=range(4),  # or c[:4]  (from datar.base import c)\n    y=[\'zero\', \'one\', \'two\', \'three\']\n)\ndf >> mutate(z=f.x)\n"""# output\n        x        y       z\n  <int64> <object> <int64>\n0       0     zero       0\n1       1      one       1\n2       2      two       2\n3       3    three       3\n"""\n\ndf >> mutate(z=if_else(f.x>1, 1, 0))\n"""# output:\n        x        y       z\n  <int64> <object> <int64>\n0       0     zero       0\n1       1      one       0\n2       2      two       1\n3       3    three       1\n"""\n\ndf >> filter(f.x>1)\n"""# output:\n        x        y\n  <int64> <object>\n0       2      two\n1       3    three\n"""\n\ndf >> mutate(z=if_else(f.x>1, 1, 0)) >> filter(f.z==1)\n"""# output:\n        x        y       z\n  <int64> <object> <int64>\n0       2      two       1\n1       3    three       1\n"""\n```\n\n```python\n# works with plotnine\n# example grabbed from https://github.com/has2k1/plydata\nimport numpy\nfrom datar.base import sin, pi\nfrom plotnine import ggplot, aes, geom_line, theme_classic\n\ndf = tibble(x=numpy.linspace(0, 2*pi, 500))\n(df >>\n  mutate(y=sin(f.x), sign=if_else(f.y>=0, "positive", "negative")) >>\n  ggplot(aes(x=\'x\', y=\'y\')) +\n  theme_classic() +\n  geom_line(aes(color=\'sign\'), size=1.2))\n```\n\n![example](./example.png)\n\n```python\n# very easy to integrate with other libraries\n# for example: klib\nimport klib\nfrom pandas import Series\nfrom pipda import register_verb\nfrom datar.datasets import iris\nfrom datar.dplyr import pull\n\ndist_plot = register_verb(Series, func=klib.dist_plot)\niris >> pull(f.Sepal_Length) >> dist_plot()\n```\n\n![example](./example2.png)\n\n\n[1]: https://tidyr.tidyverse.org/index.html\n[2]: https://dplyr.tidyverse.org/index.html\n[3]: https://github.com/pwwang/pipda\n[4]: https://tibble.tidyverse.org/index.html\n[5]: https://pwwang.github.io/datar/\n[6]: https://img.shields.io/pypi/v/datar?style=flat-square\n[7]: https://pypi.org/project/datar/\n[8]: https://img.shields.io/github/v/tag/pwwang/datar?style=flat-square\n[9]: https://github.com/pwwang/datar\n[10]: https://img.shields.io/github/workflow/status/pwwang/datar/Build%20and%20Deploy?style=flat-square\n[11]: https://img.shields.io/github/workflow/status/pwwang/datar/Build%20Docs?label=Docs&style=flat-square\n[12]: https://img.shields.io/codacy/grade/3d9bdff4d7a34bdfb9cd9e254184cb35?style=flat-square\n[13]: https://app.codacy.com/gh/pwwang/datar\n[14]: https://img.shields.io/codacy/coverage/3d9bdff4d7a34bdfb9cd9e254184cb35?style=flat-square\n[15]: https://pwwang.github.io/datar/reference-maps/ALL/\n[16]: https://pwwang.github.io/datar/notebooks/across/\n[17]: https://pwwang.github.io/datar/api/datar/\n[18]: https://pwwang.github.io/datar-blog\n[19]: https://github.com/pwwang/datar-cli\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/datar',
```

### Comparing `datar-0.9.0/PKG-INFO` & `datar-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: datar
-Version: 0.9.0
+Version: 0.9.1
 Summary: Port of dplyr and other related R packages in python, using pipda.
 Home-page: https://github.com/pwwang/datar
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: modin
 Provides-Extra: scipy
 Provides-Extra: slugify
 Provides-Extra: wcwidth
 Requires-Dist: modin (>=0.10,<0.11); extra == "modin"
 Requires-Dist: pandas (>=1.3,<2.0)
 Requires-Dist: pdtypes (>=0.0,<0.1)
-Requires-Dist: pipda (>=0.7.1,<0.8.0)
+Requires-Dist: pipda (>=0.8,<0.9)
 Requires-Dist: python-simpleconf[toml] (>=0.5,<0.6)
 Requires-Dist: python-slugify (>=6,<7); extra == "slugify"
 Requires-Dist: scipy (>=1.6,<2.0); extra == "scipy"
 Requires-Dist: wcwidth (>=0.2,<0.3); extra == "wcwidth"
 Project-URL: Repository, https://github.com/pwwang/datar
 Description-Content-Type: text/markdown
```

