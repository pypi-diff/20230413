# Comparing `tmp/rqalpha-4.9.1.tar.gz` & `tmp/rqalpha-4.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rqalpha/rqalpha/dist/tmpo_ymnfng/rqalpha-4.9.1.tar", last modified: Thu Jul 21 04:01:06 2022, max compression
+gzip compressed data, was "/home/runner/work/rqalpha/rqalpha/dist/tmpvihuja4t/rqalpha-4.9.2.tar", last modified: Thu Jul 21 04:01:35 2022, max compression
```

## Comparing `rqalpha-4.9.1.tar` & `rqalpha-4.9.2.tar`

### file list

```diff
@@ -1,235 +1,235 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)    56630 2022-07-21 04:00:57.000000 rqalpha-4.9.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-07-21 04:00:57.000000 rqalpha-4.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-07-21 04:00:57.000000 rqalpha-4.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-07-21 04:01:06.000000 rqalpha-4.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11339 2022-07-21 04:00:57.000000 rqalpha-4.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/
--rw-r--r--   0 runner    (1001) docker     (121)     7790 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3290 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/apis/
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19532 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/apis/api_abstract.py
--rw-r--r--   0 runner    (1001) docker     (121)    32995 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/apis/api_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    48850 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/apis/api_rqdatac.py
--rw-r--r--   0 runner    (1001) docker     (121)     3775 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/apis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/cmds/
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7599 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/cmds/bundle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/cmds/entry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/cmds/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4209 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/cmds/mod.py
--rw-r--r--   0 runner    (1001) docker     (121)     5043 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/cmds/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6471 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/const.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/core/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6597 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/core/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     4359 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/core/execution_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     5531 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/core/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/core/global_var.py
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/core/strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6883 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/core/strategy_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/core/strategy_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     2863 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/core/strategy_universe.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/data/
--rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/data/bar_dict_price_board.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/data/base_data_source/
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/data/base_data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3209 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/data/base_data_source/adjust.py
--rw-r--r--   0 runner    (1001) docker     (121)    16225 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/data/base_data_source/data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     3259 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/data/base_data_source/storage_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)    10044 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/data/base_data_source/storages.py
--rw-r--r--   0 runner    (1001) docker     (121)    18663 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/data/bundle.py
--rw-r--r--   0 runner    (1001) docker     (121)    13947 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/data/data_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5837 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/data/trading_dates_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     8025 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/examples/
--rw-r--r--   0 runner    (1001) docker     (121)    22343 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/IF1706_20161108.csv
--rw-r--r--   0 runner    (1001) docker     (121)     2000 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/IF_macd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/buy_and_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/examples/data_source/
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/data_source/get_csv_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     2180 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/data_source/import_get_csv_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/data_source/read_csv_as_df.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/examples/extend_api/
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/extend_api/test_extend_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/golden_cross.py
--rw-r--r--   0 runner    (1001) docker     (121)     2110 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/macd.py
--rw-r--r--   0 runner    (1001) docker     (121)     5532 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/pair_trading.py
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/rsi.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/run_code_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/run_file_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/run_func_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/subscribe_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/test_pt.py
--rw-r--r--   0 runner    (1001) docker     (121)     4619 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/examples/turtle.py
--rw-r--r--   0 runner    (1001) docker     (121)    20838 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)    12204 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/mod/
--rw-r--r--   0 runner    (1001) docker     (121)     4489 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/
--rw-r--r--   0 runner    (1001) docker     (121)     3200 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10930 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
--rw-r--r--   0 runner    (1001) docker     (121)    32509 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
--rw-r--r--   0 runner    (1001) docker     (121)     2973 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
--rw-r--r--   0 runner    (1001) docker     (121)    19262 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/
--rw-r--r--   0 runner    (1001) docker     (121)     5712 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20668 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5479 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py
--rw-r--r--   0 runner    (1001) docker     (121)     9256 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3740 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3000 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py
--rw-r--r--   0 runner    (1001) docker     (121)     5526 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/
--rw-r--r--   0 runner    (1001) docker     (121)    13833 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_progress/
--rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_progress/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2801 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2902 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_scheduler/
--rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2448 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py
--rw-r--r--   0 runner    (1001) docker     (121)    13505 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (121)     5339 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16525 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     5480 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
--rw-r--r--   0 runner    (1001) docker     (121)     6053 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
--rw-r--r--   0 runner    (1001) docker     (121)     9498 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
--rw-r--r--   0 runner    (1001) docker     (121)     9732 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     5156 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/
--rw-r--r--   0 runner    (1001) docker     (121)     3067 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7348 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
--rw-r--r--   0 runner    (1001) docker     (121)     2785 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
--rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/mod_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/model/
--rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12793 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/model/bar.py
--rw-r--r--   0 runner    (1001) docker     (121)    23525 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/model/instrument.py
--rw-r--r--   0 runner    (1001) docker     (121)    12026 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/model/order.py
--rw-r--r--   0 runner    (1001) docker     (121)     6448 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/model/tick.py
--rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/model/trade.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/portfolio/
--rw-r--r--   0 runner    (1001) docker     (121)    11108 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17895 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/portfolio/account.py
--rw-r--r--   0 runner    (1001) docker     (121)    14993 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/portfolio/position.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/resource/
--rw-r--r--   0 runner    (1001) docker     (121)    32799 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/resource/ricequant-logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/user_module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     7589 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17569 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/arg_checker.py
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/class_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/click_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3670 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (121)    10415 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3729 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/datetime_func.py
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/dict_func.py
--rw-r--r--   0 runner    (1001) docker     (121)     4853 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     4445 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/functools.py
--rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/i18n.py
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/log_capture.py
--rw-r--r--   0 runner    (1001) docker     (121)     3141 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/package_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3863 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/persisit_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     4038 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2205 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/risk_free_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/rq_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/strategy_loader_help.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5056 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/testing/mocking.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/utils/translations/
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/utils/translations/zh_Hans_CN/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17796 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)    48759 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/translations/zh_Hans_CN/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-07-21 04:00:57.000000 rqalpha-4.9.1/rqalpha/utils/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6993 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 04:01:05.000000 rqalpha-4.9.1/rqalpha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-21 04:01:06.000000 rqalpha-4.9.1/rqalpha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-07-21 04:01:06.000000 rqalpha-4.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3430 2022-07-21 04:00:57.000000 rqalpha-4.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/tests/api_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     3205 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/tests/api_tests/mod/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/tests/api_tests/mod/sys_accounts/
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/mod/sys_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5407 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/mod/sys_accounts/test_account_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2318 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/mod/sys_accounts/test_position_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/tests/api_tests/mod/sys_scheduler/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/mod/sys_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/mod/sys_scheduler/test_physical_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     2215 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/mod/sys_scheduler/test_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/tests/api_tests/mod/sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/mod/sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/mod/sys_simulation/test_management_fee.py
--rw-r--r--   0 runner    (1001) docker     (121)     2456 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/mod/sys_simulation/test_signal_broker.py
--rw-r--r--   0 runner    (1001) docker     (121)     3624 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/mod/sys_simulation/test_simulation_broker.py
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    16648 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/test_api_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4390 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/test_api_future.py
--rw-r--r--   0 runner    (1001) docker     (121)     9118 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/test_api_stock.py
--rw-r--r--   0 runner    (1001) docker     (121)     4086 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/api_tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/test_f_buy_and_hold.py
--rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/test_f_macd.py
--rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/test_f_macd_signal.py
--rw-r--r--   0 runner    (1001) docker     (121)     5741 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/test_f_mean_reverting.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/test_s_buy_and_hold.py
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/test_s_dual_thrust.py
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/test_s_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/test_s_tick_size.py
--rw-r--r--   0 runner    (1001) docker     (121)     5043 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/test_s_turtle.py
--rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/test_s_turtle_signal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/test_sf_buy_and_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/tests/unittest/
--rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/unittest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/tests/unittest/test_data/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/unittest/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2876 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/unittest/test_data/test_instrument_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/unittest/test_data/test_trading_dates_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/tests/unittest/test_mod/
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/unittest/test_mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:06.000000 rqalpha-4.9.1/tests/unittest/test_mod/test_sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/unittest/test_mod/test_sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4219 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-07-21 04:00:57.000000 rqalpha-4.9.1/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    79815 2022-07-21 04:00:57.000000 rqalpha-4.9.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)    56630 2022-07-21 04:01:26.000000 rqalpha-4.9.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-07-21 04:01:26.000000 rqalpha-4.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-07-21 04:01:26.000000 rqalpha-4.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2022-07-21 04:01:35.000000 rqalpha-4.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11339 2022-07-21 04:01:26.000000 rqalpha-4.9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/
+-rw-r--r--   0 runner    (1001) docker     (121)     7790 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3290 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/api.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/apis/
+-rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19532 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/apis/api_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32995 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/apis/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50314 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/apis/api_rqdatac.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3775 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/apis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/cmds/
+-rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7599 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/cmds/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1586 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/cmds/entry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/cmds/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4209 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/cmds/mod.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5043 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/cmds/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/config.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6471 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/const.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/core/
+-rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6597 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4359 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5531 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/global_var.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6883 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/strategy_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/strategy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2863 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/core/strategy_universe.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/bar_dict_price_board.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/data/base_data_source/
+-rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/base_data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3209 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/base_data_source/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16225 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/base_data_source/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3259 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/base_data_source/storage_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10044 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/base_data_source/storages.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18663 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13947 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/data_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5837 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/data/trading_dates_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8025 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)    22343 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/IF1706_20161108.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2000 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/IF_macd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/buy_and_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/examples/data_source/
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/data_source/get_csv_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2180 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/data_source/import_get_csv_module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/data_source/read_csv_as_df.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/examples/extend_api/
+-rw-r--r--   0 runner    (1001) docker     (121)     2706 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/extend_api/test_extend_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2151 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/golden_cross.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2110 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/macd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5532 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/pair_trading.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/rsi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      822 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/run_code_demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/run_file_demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/run_func_demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/subscribe_event.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/test_pt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4619 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/examples/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20838 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12204 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/
+-rw-r--r--   0 runner    (1001) docker     (121)     4489 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/
+-rw-r--r--   0 runner    (1001) docker     (121)     3200 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/
+-rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10930 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32509 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2973 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19262 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/
+-rw-r--r--   0 runner    (1001) docker     (121)     5712 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20668 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/
+-rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5479 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9256 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3740 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3000 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5526 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)    13833 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_progress/
+-rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_progress/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/
+-rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/
+-rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2801 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2902 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2448 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13505 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (121)     5339 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16525 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5480 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6053 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9498 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9732 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5156 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/
+-rw-r--r--   0 runner    (1001) docker     (121)     3067 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7348 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2785 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/mod_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/model/
+-rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12793 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/model/bar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23525 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/model/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12026 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/model/order.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6448 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/model/tick.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/model/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (121)    11108 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17895 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/portfolio/account.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14993 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/portfolio/position.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/resource/
+-rw-r--r--   0 runner    (1001) docker     (121)    32799 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/resource/ricequant-logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/user_module.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     7589 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17569 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/arg_checker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/class_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/click_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3670 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10415 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3729 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/datetime_func.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/dict_func.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4853 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4445 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/functools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3141 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/package_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3863 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/persisit_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4038 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2205 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/risk_free_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2651 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/rq_json.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/strategy_loader_help.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5056 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/testing/mocking.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/utils/translations/
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17796 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    48759 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-07-21 04:01:26.000000 rqalpha-4.9.2/rqalpha/utils/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6993 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-21 04:01:35.000000 rqalpha-4.9.2/rqalpha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-07-21 04:01:35.000000 rqalpha-4.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3430 2022-07-21 04:01:26.000000 rqalpha-4.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/api_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     3205 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/api_tests/mod/
+-rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_accounts/
+-rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5407 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_accounts/test_account_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2318 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_accounts/test_position_models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_scheduler/test_physical_time.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2215 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_scheduler/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3342 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_management_fee.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2456 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_signal_broker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3624 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_simulation_broker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16648 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/test_api_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4390 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/test_api_future.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9118 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/test_api_stock.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4086 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/api_tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_f_buy_and_hold.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_f_macd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2534 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_f_macd_signal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5741 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_f_mean_reverting.py
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_s_buy_and_hold.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_s_dual_thrust.py
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_s_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_s_tick_size.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5043 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_s_turtle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_s_turtle_signal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/test_sf_buy_and_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/unittest/
+-rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/unittest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/unittest/test_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/unittest/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2876 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/unittest/test_data/test_instrument_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/unittest/test_data/test_trading_dates_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/unittest/test_mod/
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/unittest/test_mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:01:35.000000 rqalpha-4.9.2/tests/unittest/test_mod/test_sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/unittest/test_mod/test_sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4219 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-07-21 04:01:26.000000 rqalpha-4.9.2/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    79815 2022-07-21 04:01:26.000000 rqalpha-4.9.2/versioneer.py
```

### Comparing `rqalpha-4.9.1/CHANGELOG.rst` & `rqalpha-4.9.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/LICENSE` & `rqalpha-4.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/PKG-INFO` & `rqalpha-4.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqalpha
-Version: 4.9.1
+Version: 4.9.2
 Summary: Ricequant Algorithm Trading System
 Home-page: https://github.com/ricequant/rqalpha
 Author: ricequant
 Author-email: public@ricequant.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
```

### Comparing `rqalpha-4.9.1/README.rst` & `rqalpha-4.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/__init__.py` & `rqalpha-4.9.2/rqalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/__main__.py` & `rqalpha-4.9.2/rqalpha/__main__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/api.py` & `rqalpha-4.9.2/rqalpha/api.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/apis/__init__.py` & `rqalpha-4.9.2/rqalpha/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/apis/api_abstract.py` & `rqalpha-4.9.2/rqalpha/apis/api_abstract.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/apis/api_base.py` & `rqalpha-4.9.2/rqalpha/apis/api_base.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/apis/api_rqdatac.py` & `rqalpha-4.9.2/rqalpha/apis/api_rqdatac.py`

 * *Files 2% similar despite different names*

```diff
@@ -1093,32 +1093,78 @@
 
 @export_as_api
 @apply_rules(verify_that('statements').is_in(['all', 'latest'], ignore_none=True))
 def get_pit_financials_ex(order_book_ids, fields, count, statements='latest'):
     if isinstance(order_book_ids, str):
         order_book_ids = [order_book_ids]
     env = Environment.get_instance()
-    dt = env.calendar_dt.date()
-    year = dt.year
-    mon = dt.month
-    q = (mon - 4) // 3 + 1
-    y = year
-    if q <= 0:
-        y -= 1
-        q = 4
-    end_quarter = str(y) + 'q' + str(q)
-
-    q_num = y * 4 + q - count
-    start_y = q_num // 4
-    start_q = q_num % 4 + 1
 
-    start_quarter = "{}q{}".format(start_y, start_q)
+    if count < 0:
+        user_log.warn("function get_pit_financials_ex : count must >= 0")
+        return None
+
+    # 退市和未退市池
+    de_listed_list, active_list = [], []
+
+    # 遍历每个标的划分池子
+    for order_book_id in order_book_ids:
+        instrument = env.get_instrument(order_book_id)
+        if env.calendar_dt > instrument.de_listed_date:
+            de_listed_list.append(instrument)
+        else:
+            active_list.append(order_book_id)
+
+    # 需要的数量，传入的 0 代表 1个
+    count += 1
+
+    def _get_data(symbol_list, start_dt):
+        dt = start_dt.date()
+        year = dt.year
+        mon = dt.month
+        q = (mon - 4) // 3 + 1
+        y = year
+        if q <= 0:
+            y -= 1
+            q = 4
+        end_quarter = str(y) + 'q' + str(q)
+
+        # 多获取4个季度的财报，以防因为财报未发布导致数量不够
+        q_num = y * 4 + q - count - 4
+
+        start_y = q_num // 4
+        start_q = q_num % 4 + 1
+        start_quarter = "{}q{}".format(start_y, start_q)
+
+        if start_quarter > end_quarter:
+            start_quarter = end_quarter
+
+        result = rqdatac.get_pit_financials_ex(
+            fields=fields, start_quarter=start_quarter, end_quarter=end_quarter, order_book_ids=symbol_list,
+            statements=statements, market='cn', date=env.calendar_dt.date()
+        )
+
+        return result
+
+    # 保存结果
+    result_list = []
+
+    # 获取未退市标的的数据
+    result = _get_data(active_list, env.calendar_dt)
+
+    if isinstance(result, pd.DataFrame):
+        result_list = [group_df.iloc[-count:] for _, group_df in result.groupby("order_book_id")]
+
+    # 获取退市的数据
+    for instrument in de_listed_list:
+        result = _get_data([instrument.order_book_id], instrument.de_listed_date)
+        if isinstance(result, pd.DataFrame):
+            result_list.append(result.iloc[-count:])
+
+    result = pd.concat(result_list) if len(result_list) > 0 else None
 
-    result = rqdatac.get_pit_financials_ex(fields=fields, start_quarter=start_quarter, end_quarter=end_quarter,
-        order_book_ids=order_book_ids, statements=statements, market='cn', date=dt)
     return result
 
 
 @export_as_api
 @apply_rules(verify_that('entities').are_valid_query_entities())
 def query(*entities):
     return rqdatac.query(*entities)
```

### Comparing `rqalpha-4.9.1/rqalpha/apis/names.py` & `rqalpha-4.9.2/rqalpha/apis/names.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/cmds/__init__.py` & `rqalpha-4.9.2/rqalpha/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/cmds/bundle.py` & `rqalpha-4.9.2/rqalpha/cmds/bundle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/cmds/entry.py` & `rqalpha-4.9.2/rqalpha/cmds/entry.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/cmds/misc.py` & `rqalpha-4.9.2/rqalpha/cmds/misc.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/cmds/mod.py` & `rqalpha-4.9.2/rqalpha/cmds/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/cmds/run.py` & `rqalpha-4.9.2/rqalpha/cmds/run.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/config.yml` & `rqalpha-4.9.2/rqalpha/config.yml`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/const.py` & `rqalpha-4.9.2/rqalpha/const.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/core/__init__.py` & `rqalpha-4.9.2/rqalpha/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/core/events.py` & `rqalpha-4.9.2/rqalpha/core/events.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/core/execution_context.py` & `rqalpha-4.9.2/rqalpha/core/execution_context.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/core/executor.py` & `rqalpha-4.9.2/rqalpha/core/executor.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/core/global_var.py` & `rqalpha-4.9.2/rqalpha/core/global_var.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/core/strategy.py` & `rqalpha-4.9.2/rqalpha/core/strategy.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/core/strategy_context.py` & `rqalpha-4.9.2/rqalpha/core/strategy_context.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/core/strategy_loader.py` & `rqalpha-4.9.2/rqalpha/core/strategy_loader.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/core/strategy_universe.py` & `rqalpha-4.9.2/rqalpha/core/strategy_universe.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/data/__init__.py` & `rqalpha-4.9.2/rqalpha/data/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/data/bar_dict_price_board.py` & `rqalpha-4.9.2/rqalpha/data/bar_dict_price_board.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/data/base_data_source/__init__.py` & `rqalpha-4.9.2/rqalpha/data/base_data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/data/base_data_source/adjust.py` & `rqalpha-4.9.2/rqalpha/data/base_data_source/adjust.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/data/base_data_source/data_source.py` & `rqalpha-4.9.2/rqalpha/data/base_data_source/data_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/data/base_data_source/storage_interface.py` & `rqalpha-4.9.2/rqalpha/data/base_data_source/storage_interface.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/data/base_data_source/storages.py` & `rqalpha-4.9.2/rqalpha/data/base_data_source/storages.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/data/bundle.py` & `rqalpha-4.9.2/rqalpha/data/bundle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/data/data_proxy.py` & `rqalpha-4.9.2/rqalpha/data/data_proxy.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/data/trading_dates_mixin.py` & `rqalpha-4.9.2/rqalpha/data/trading_dates_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/environment.py` & `rqalpha-4.9.2/rqalpha/environment.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/IF1706_20161108.csv` & `rqalpha-4.9.2/rqalpha/examples/IF1706_20161108.csv`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/IF_macd.py` & `rqalpha-4.9.2/rqalpha/examples/IF_macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/buy_and_hold.py` & `rqalpha-4.9.2/rqalpha/examples/buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/data_source/get_csv_module.py` & `rqalpha-4.9.2/rqalpha/examples/data_source/get_csv_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/data_source/import_get_csv_module.py` & `rqalpha-4.9.2/rqalpha/examples/data_source/import_get_csv_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/data_source/read_csv_as_df.py` & `rqalpha-4.9.2/rqalpha/examples/data_source/read_csv_as_df.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py` & `rqalpha-4.9.2/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/extend_api/test_extend_api.py` & `rqalpha-4.9.2/rqalpha/examples/extend_api/test_extend_api.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/golden_cross.py` & `rqalpha-4.9.2/rqalpha/examples/golden_cross.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/macd.py` & `rqalpha-4.9.2/rqalpha/examples/macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/pair_trading.py` & `rqalpha-4.9.2/rqalpha/examples/pair_trading.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/rsi.py` & `rqalpha-4.9.2/rqalpha/examples/rsi.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/run_code_demo.py` & `rqalpha-4.9.2/rqalpha/examples/run_code_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/run_func_demo.py` & `rqalpha-4.9.2/rqalpha/examples/run_func_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/subscribe_event.py` & `rqalpha-4.9.2/rqalpha/examples/subscribe_event.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/test_pt.py` & `rqalpha-4.9.2/rqalpha/examples/test_pt.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/examples/turtle.py` & `rqalpha-4.9.2/rqalpha/examples/turtle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/interface.py` & `rqalpha-4.9.2/rqalpha/interface.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/main.py` & `rqalpha-4.9.2/rqalpha/main.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/__init__.py` & `rqalpha-4.9.2/rqalpha/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_progress/mod.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_progress/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/mod.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py` & `rqalpha-4.9.2/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/mod/utils.py` & `rqalpha-4.9.2/rqalpha/mod/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/model/__init__.py` & `rqalpha-4.9.2/rqalpha/model/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/model/bar.py` & `rqalpha-4.9.2/rqalpha/model/bar.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/model/instrument.py` & `rqalpha-4.9.2/rqalpha/model/instrument.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/model/order.py` & `rqalpha-4.9.2/rqalpha/model/order.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/model/tick.py` & `rqalpha-4.9.2/rqalpha/model/tick.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/model/trade.py` & `rqalpha-4.9.2/rqalpha/model/trade.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/portfolio/__init__.py` & `rqalpha-4.9.2/rqalpha/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/portfolio/account.py` & `rqalpha-4.9.2/rqalpha/portfolio/account.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/portfolio/position.py` & `rqalpha-4.9.2/rqalpha/portfolio/position.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/resource/ricequant-logo.png` & `rqalpha-4.9.2/rqalpha/resource/ricequant-logo.png`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/user_module.py` & `rqalpha-4.9.2/rqalpha/user_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/__init__.py` & `rqalpha-4.9.2/rqalpha/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/arg_checker.py` & `rqalpha-4.9.2/rqalpha/utils/arg_checker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/class_helper.py` & `rqalpha-4.9.2/rqalpha/utils/class_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/click_helper.py` & `rqalpha-4.9.2/rqalpha/utils/click_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/concurrent.py` & `rqalpha-4.9.2/rqalpha/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/config.py` & `rqalpha-4.9.2/rqalpha/utils/config.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/datetime_func.py` & `rqalpha-4.9.2/rqalpha/utils/datetime_func.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/dict_func.py` & `rqalpha-4.9.2/rqalpha/utils/dict_func.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/exception.py` & `rqalpha-4.9.2/rqalpha/utils/exception.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/functools.py` & `rqalpha-4.9.2/rqalpha/utils/functools.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/i18n.py` & `rqalpha-4.9.2/rqalpha/utils/i18n.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/log_capture.py` & `rqalpha-4.9.2/rqalpha/utils/log_capture.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/logger.py` & `rqalpha-4.9.2/rqalpha/utils/logger.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/package_helper.py` & `rqalpha-4.9.2/rqalpha/utils/package_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/persisit_helper.py` & `rqalpha-4.9.2/rqalpha/utils/persisit_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/repr.py` & `rqalpha-4.9.2/rqalpha/utils/repr.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/risk_free_helper.py` & `rqalpha-4.9.2/rqalpha/utils/risk_free_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/rq_json.py` & `rqalpha-4.9.2/rqalpha/utils/rq_json.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/strategy_loader_help.py` & `rqalpha-4.9.2/rqalpha/utils/strategy_loader_help.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/testing/__init__.py` & `rqalpha-4.9.2/rqalpha/utils/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/testing/fixtures.py` & `rqalpha-4.9.2/rqalpha/utils/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/testing/mocking.py` & `rqalpha-4.9.2/rqalpha/utils/testing/mocking.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/translations/__init__.py` & `rqalpha-4.9.2/rqalpha/utils/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py` & `rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo` & `rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po` & `rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/translations/zh_Hans_CN/__init__.py` & `rqalpha-4.9.2/rqalpha/utils/translations/zh_Hans_CN/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha/utils/typing.py` & `rqalpha-4.9.2/rqalpha/utils/typing.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/rqalpha.egg-info/PKG-INFO` & `rqalpha-4.9.2/rqalpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqalpha
-Version: 4.9.1
+Version: 4.9.2
 Summary: Ricequant Algorithm Trading System
 Home-page: https://github.com/ricequant/rqalpha
 Author: ricequant
 Author-email: public@ricequant.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
```

### Comparing `rqalpha-4.9.1/rqalpha.egg-info/SOURCES.txt` & `rqalpha-4.9.2/rqalpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/setup.py` & `rqalpha-4.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/__init__.py` & `rqalpha-4.9.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/__init__.py` & `rqalpha-4.9.2/tests/api_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/mod/__init__.py` & `rqalpha-4.9.2/tests/api_tests/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/mod/sys_accounts/__init__.py` & `rqalpha-4.9.2/tests/api_tests/mod/sys_accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/mod/sys_accounts/test_account_model.py` & `rqalpha-4.9.2/tests/api_tests/mod/sys_accounts/test_account_model.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/mod/sys_accounts/test_position_models.py` & `rqalpha-4.9.2/tests/api_tests/mod/sys_accounts/test_position_models.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/mod/sys_scheduler/test_physical_time.py` & `rqalpha-4.9.2/tests/api_tests/mod/sys_scheduler/test_physical_time.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/mod/sys_scheduler/test_scheduler.py` & `rqalpha-4.9.2/tests/api_tests/mod/sys_scheduler/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/mod/sys_simulation/__init__.py` & `rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/mod/sys_simulation/test_management_fee.py` & `rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_management_fee.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/mod/sys_simulation/test_signal_broker.py` & `rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_signal_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/mod/sys_simulation/test_simulation_broker.py` & `rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_simulation_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py` & `rqalpha-4.9.2/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/test_api_base.py` & `rqalpha-4.9.2/tests/api_tests/test_api_base.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/test_api_future.py` & `rqalpha-4.9.2/tests/api_tests/test_api_future.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/test_api_stock.py` & `rqalpha-4.9.2/tests/api_tests/test_api_stock.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/api_tests/test_config.py` & `rqalpha-4.9.2/tests/api_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/test_f_buy_and_hold.py` & `rqalpha-4.9.2/tests/test_f_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/test_f_macd.py` & `rqalpha-4.9.2/tests/test_f_macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/test_f_macd_signal.py` & `rqalpha-4.9.2/tests/test_f_macd_signal.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/test_f_mean_reverting.py` & `rqalpha-4.9.2/tests/test_f_mean_reverting.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/test_s_buy_and_hold.py` & `rqalpha-4.9.2/tests/test_s_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/test_s_dual_thrust.py` & `rqalpha-4.9.2/tests/test_s_dual_thrust.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/test_s_scheduler.py` & `rqalpha-4.9.2/tests/test_s_scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/test_s_tick_size.py` & `rqalpha-4.9.2/tests/test_s_tick_size.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/test_s_turtle.py` & `rqalpha-4.9.2/tests/test_s_turtle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/test_s_turtle_signal.py` & `rqalpha-4.9.2/tests/test_s_turtle_signal.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/test_sf_buy_and_hold.py` & `rqalpha-4.9.2/tests/test_sf_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/unittest/__init__.py` & `rqalpha-4.9.2/tests/unittest/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/unittest/test_data/test_instrument_mixin.py` & `rqalpha-4.9.2/tests/unittest/test_data/test_instrument_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/unittest/test_data/test_trading_dates_mixin.py` & `rqalpha-4.9.2/tests/unittest/test_data/test_trading_dates_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/unittest/test_mod/__init__.py` & `rqalpha-4.9.2/tests/unittest/test_mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/unittest/test_mod/test_sys_simulation/__init__.py` & `rqalpha-4.9.2/tests/unittest/test_mod/test_sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py` & `rqalpha-4.9.2/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/tests/utils.py` & `rqalpha-4.9.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-4.9.1/versioneer.py` & `rqalpha-4.9.2/versioneer.py`

 * *Files identical despite different names*

