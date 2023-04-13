# Comparing `tmp/mia-accounting-1.3.2.tar.gz` & `tmp/mia-accounting-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia-accounting-1.3.2.tar", last modified: Wed Apr 12 10:01:53 2023, max compression
+gzip compressed data, was "mia-accounting-1.3.3.tar", last modified: Thu Apr 13 01:57:14 2023, max compression
```

## Comparing `mia-accounting-1.3.2.tar` & `mia-accounting-1.3.3.tar`

### file list

```diff
@@ -1,310 +1,308 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.3.2/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.3.2/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     5871 2023-04-11 13:56:49.000000 mia-accounting-1.3.2/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.207196 mia-accounting-1.3.2/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.3.2/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.3.2/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.207196 mia-accounting-1.3.2/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.207196 mia-accounting-1.3.2/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.3.2/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.207196 mia-accounting-1.3.2/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.3.2/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-10 16:05:21.000000 mia-accounting-1.3.2/docs/source/accounting.account.rst
--rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-10 16:05:21.000000 mia-accounting-1.3.2/docs/source/accounting.base_account.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.currency.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.journal_entry.forms.rst
--rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.journal_entry.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.journal_entry.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.option.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.report.period.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2043 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.report.reports.rst
--rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.report.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1775 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.report.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1332 2023-04-10 16:05:21.000000 mia-accounting-1.3.2/docs/source/accounting.rst
--rw-r--r--   0 imacat    (1000) users      (100)      615 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.unmatched_offset.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2756 2023-04-10 16:05:22.000000 mia-accounting-1.3.2/docs/source/accounting.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-12 09:53:44.000000 mia-accounting-1.3.2/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.3.2/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.3.2/docs/source/history.rst
--rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.3.2/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     3615 2023-04-11 13:56:49.000000 mia-accounting-1.3.2/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.3.2/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-12 09:53:44.000000 mia-accounting-1.3.2/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.203196 mia-accounting-1.3.2/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.211195 mia-accounting-1.3.2/src/accounting/
--rw-r--r--   0 imacat    (1000) users      (100)     3065 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/__init__.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.211195 mia-accounting-1.3.2/src/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.3.2/src/accounting/account/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.3.2/src/accounting/account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.211195 mia-accounting-1.3.2/src/accounting/base_account/
--rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/base_account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/base_account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/base_account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.3.2/src/accounting/base_account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.3.2/src/accounting/base_account/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/commands.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.211195 mia-accounting-1.3.2/src/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/currency/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2212 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/src/accounting/currency/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/currency/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.3.2/src/accounting/currency/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/currency/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.3.2/src/accounting/currency/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.211195 mia-accounting-1.3.2/src/accounting/data/
--rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.3.2/src/accounting/data/base_accounts.csv
--rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.3.2/src/accounting/data/currencies.csv
--rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.3.2/src/accounting/forms.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.211195 mia-accounting-1.3.2/src/accounting/journal_entry/
--rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/journal_entry/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3283 2023-04-11 16:41:29.000000 mia-accounting-1.3.2/src/accounting/journal_entry/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.215195 mia-accounting-1.3.2/src/accounting/journal_entry/forms/
--rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.3.2/src/accounting/journal_entry/forms/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    11055 2023-04-08 10:12:54.000000 mia-accounting-1.3.2/src/accounting/journal_entry/forms/currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.3.2/src/accounting/journal_entry/forms/journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    19508 2023-04-07 16:44:13.000000 mia-accounting-1.3.2/src/accounting/journal_entry/forms/line_item.py
--rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/journal_entry/forms/reorder.py
--rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.3.2/src/accounting/journal_entry/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.215195 mia-accounting-1.3.2/src/accounting/journal_entry/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.3.2/src/accounting/journal_entry/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1729 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/journal_entry/utils/account_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    12821 2023-04-04 09:21:31.000000 mia-accounting-1.3.2/src/accounting/journal_entry/utils/description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/journal_entry/utils/operators.py
--rw-r--r--   0 imacat    (1000) users      (100)     3787 2023-04-08 10:12:55.000000 mia-accounting-1.3.2/src/accounting/journal_entry/utils/original_line_items.py
--rw-r--r--   0 imacat    (1000) users      (100)     9472 2023-04-09 02:08:22.000000 mia-accounting-1.3.2/src/accounting/journal_entry/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.3.2/src/accounting/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    31691 2023-04-08 10:12:57.000000 mia-accounting-1.3.2/src/accounting/models.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.215195 mia-accounting-1.3.2/src/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/option/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.3.2/src/accounting/option/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.3.2/src/accounting/option/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.215195 mia-accounting-1.3.2/src/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.3.2/src/accounting/report/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.3.2/src/accounting/report/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.215195 mia-accounting-1.3.2/src/accounting/report/period/
--rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.3.2/src/accounting/report/period/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/report/period/chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/report/period/description.py
--rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.3.2/src/accounting/report/period/month_end.py
--rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.3.2/src/accounting/report/period/parser.py
--rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.3.2/src/accounting/report/period/period.py
--rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/report/period/shortcuts.py
--rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/report/period/specification.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.219195 mia-accounting-1.3.2/src/accounting/report/reports/
--rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.3.2/src/accounting/report/reports/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.3.2/src/accounting/report/reports/balance_sheet.py
--rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/report/reports/income_expenses.py
--rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.3.2/src/accounting/report/reports/income_statement.py
--rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.3.2/src/accounting/report/reports/journal.py
--rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.3.2/src/accounting/report/reports/ledger.py
--rw-r--r--   0 imacat    (1000) users      (100)     8819 2023-04-09 13:02:35.000000 mia-accounting-1.3.2/src/accounting/report/reports/search.py
--rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.3.2/src/accounting/report/reports/trial_balance.py
--rw-r--r--   0 imacat    (1000) users      (100)     6975 2023-04-08 16:39:45.000000 mia-accounting-1.3.2/src/accounting/report/reports/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4555 2023-04-08 10:12:55.000000 mia-accounting-1.3.2/src/accounting/report/reports/unapplied_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.3.2/src/accounting/report/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.219195 mia-accounting-1.3.2/src/accounting/report/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/report/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/report/utils/base_page_params.py
--rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.3.2/src/accounting/report/utils/base_report.py
--rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-09 04:04:18.000000 mia-accounting-1.3.2/src/accounting/report/utils/csv_export.py
--rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.3.2/src/accounting/report/utils/option_link.py
--rw-r--r--   0 imacat    (1000) users      (100)     6925 2023-04-08 10:12:55.000000 mia-accounting-1.3.2/src/accounting/report/utils/report_chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     1305 2023-04-08 03:26:33.000000 mia-accounting-1.3.2/src/accounting/report/utils/report_type.py
--rw-r--r--   0 imacat    (1000) users      (100)     2740 2023-04-08 10:12:55.000000 mia-accounting-1.3.2/src/accounting/report/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4477 2023-04-09 02:08:22.000000 mia-accounting-1.3.2/src/accounting/report/utils/urls.py
--rw-r--r--   0 imacat    (1000) users      (100)    10434 2023-04-09 02:08:22.000000 mia-accounting-1.3.2/src/accounting/report/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.203196 mia-accounting-1.3.2/src/accounting/static/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.219195 mia-accounting-1.3.2/src/accounting/static/css/
--rw-r--r--   0 imacat    (1000) users      (100)    13001 2023-04-08 16:39:45.000000 mia-accounting-1.3.2/src/accounting/static/css/style.css
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.219195 mia-accounting-1.3.2/src/accounting/static/js/
--rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/account-form.js
--rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/account-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/currency-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    38778 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/description-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/drag-and-drop-reorder.js
--rw-r--r--   0 imacat    (1000) users      (100)     9092 2023-04-07 04:32:27.000000 mia-accounting-1.3.2/src/accounting/static/js/journal-entry-account-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    32504 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/journal-entry-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    19866 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/journal-entry-line-item-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/journal-entry-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/material-fab-speed-dial.js
--rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/option-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    11640 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/original-line-item-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.3.2/src/accounting/static/js/period-chooser.js
--rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.3.2/src/accounting/template_filters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/template_globals.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.203196 mia-accounting-1.3.2/src/accounting/templates/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.219195 mia-accounting-1.3.2/src/accounting/templates/accounting/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/account/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/account/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/account/include/
--rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/account/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/account/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/base-account/
--rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/base-account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/base-account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/base.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/currency/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/currency/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/currency/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/currency/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/currency/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/currency/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3103 2023-04-10 23:49:07.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/include/nav.html
--rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/include/pagination.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/
--rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.223195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.227195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3373 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)    14459 2023-04-05 01:08:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3131 2023-04-07 06:56:44.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
--rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
--rw-r--r--   0 imacat    (1000) users      (100)     6161 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
--rw-r--r--   0 imacat    (1000) users      (100)     3490 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.227195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/
--rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.227195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.227195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/
--rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.227195 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.227195 mia-accounting-1.3.2/src/accounting/templates/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/option/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/option/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.227195 mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
--rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/form-recurring-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.231195 mia-accounting-1.3.2/src/accounting/templates/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     5065 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/balance-sheet.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.231195 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
--rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/balance-sheet-section.html
--rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/period-chooser.html
--rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/search-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     5572 2023-04-04 23:56:52.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/toolbar-buttons.html
--rw-r--r--   0 imacat    (1000) users      (100)     4623 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/income-expenses.html
--rw-r--r--   0 imacat    (1000) users      (100)     4242 2023-04-04 10:04:12.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/income-statement.html
--rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/journal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4745 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/ledger.html
--rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/search.html
--rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-04 10:04:10.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/trial-balance.html
--rw-r--r--   0 imacat    (1000) users      (100)     2201 2023-04-08 10:12:55.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/unapplied-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     4086 2023-04-08 16:39:45.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/report/unapplied.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.231195 mia-accounting-1.3.2/src/accounting/templates/accounting/unmatched-offset/
--rw-r--r--   0 imacat    (1000) users      (100)     1212 2023-04-08 16:38:54.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/unmatched-offset/dashboard.html
--rw-r--r--   0 imacat    (1000) users      (100)     4668 2023-04-08 10:12:57.000000 mia-accounting-1.3.2/src/accounting/templates/accounting/unmatched-offset/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.231195 mia-accounting-1.3.2/src/accounting/translations/
--rw-r--r--   0 imacat    (1000) users      (100)    47460 2023-04-08 17:41:05.000000 mia-accounting-1.3.2/src/accounting/translations/accounting.pot
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.3.2/src/accounting/translations/babel.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.203196 mia-accounting-1.3.2/src/accounting/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.231195 mia-accounting-1.3.2/src/accounting/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.2/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.2/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.203196 mia-accounting-1.3.2/src/accounting/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.231195 mia-accounting-1.3.2/src/accounting/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.2/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.2/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.231195 mia-accounting-1.3.2/src/accounting/unmatched_offset/
--rw-r--r--   0 imacat    (1000) users      (100)     1032 2023-04-08 10:12:57.000000 mia-accounting-1.3.2/src/accounting/unmatched_offset/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-08 10:12:57.000000 mia-accounting-1.3.2/src/accounting/unmatched_offset/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     3178 2023-04-08 16:39:45.000000 mia-accounting-1.3.2/src/accounting/unmatched_offset/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.235195 mia-accounting-1.3.2/src/accounting/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.3.2/src/accounting/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/utils/cast.py
--rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/utils/current_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/utils/flash_errors.py
--rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.3.2/src/accounting/utils/journal_entry_types.py
--rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.3.2/src/accounting/utils/next_uri.py
--rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.3.2/src/accounting/utils/offset_alias.py
--rw-r--r--   0 imacat    (1000) users      (100)     5198 2023-04-08 16:39:45.000000 mia-accounting-1.3.2/src/accounting/utils/offset_matcher.py
--rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.3.2/src/accounting/utils/options.py
--rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.3.2/src/accounting/utils/pagination.py
--rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.3.2/src/accounting/utils/permission.py
--rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/utils/query.py
--rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/utils/random_id.py
--rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.3.2/src/accounting/utils/strip_text.py
--rw-r--r--   0 imacat    (1000) users      (100)     3080 2023-04-08 10:12:56.000000 mia-accounting-1.3.2/src/accounting/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.3.2/src/accounting/utils/user.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.235195 mia-accounting-1.3.2/src/mia_accounting.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-12 10:01:53.000000 mia-accounting-1.3.2/src/mia_accounting.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)    11508 2023-04-12 10:01:53.000000 mia-accounting-1.3.2/src/mia_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-12 10:01:53.000000 mia-accounting-1.3.2/src/mia_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-12 10:01:53.000000 mia-accounting-1.3.2/src/mia_accounting.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-12 10:01:53.000000 mia-accounting-1.3.2/src/mia_accounting.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/
--rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.3.2/tests/babel-utils-test-site.py
--rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.3.2/tests/babel-utils.py
--rwxr-xr-x   0 imacat    (1000) users      (100)    11020 2023-04-12 09:13:03.000000 mia-accounting-1.3.2/tests/make-sample.py
--rw-r--r--   0 imacat    (1000) users      (100)    32736 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/tests/test_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/tests/test_base_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/tests/test_commands.py
--rw-r--r--   0 imacat    (1000) users      (100)    23824 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/tests/test_currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    15999 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/tests/test_description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)   103461 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/tests/test_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    38264 2023-04-12 04:25:38.000000 mia-accounting-1.3.2/tests/test_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    15935 2023-04-10 15:59:48.000000 mia-accounting-1.3.2/tests/test_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    15371 2023-04-12 04:25:38.000000 mia-accounting-1.3.2/tests/test_report.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/test_site/
--rw-r--r--   0 imacat    (1000) users      (100)     4505 2023-04-11 16:31:36.000000 mia-accounting-1.3.2/tests/test_site/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3073 2023-04-11 14:24:08.000000 mia-accounting-1.3.2/tests/test_site/auth.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/test_site/data/
--rw-r--r--   0 imacat    (1000) users      (100)   121813 2023-04-12 09:21:52.000000 mia-accounting-1.3.2/tests/test_site/data/sample.json
--rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.3.2/tests/test_site/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)     4888 2023-04-12 09:59:37.000000 mia-accounting-1.3.2/tests/test_site/reset.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/test_site/static/
--rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.3.2/tests/test_site/static/favicon.svg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/test_site/templates/
--rw-r--r--   0 imacat    (1000) users      (100)     6435 2023-04-12 09:40:17.000000 mia-accounting-1.3.2/tests/test_site/templates/base.html
--rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.3.2/tests/test_site/templates/home.html
--rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.3.2/tests/test_site/templates/login.html
--rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 09:48:47.000000 mia-accounting-1.3.2/tests/test_site/templates/reset.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/test_site/translations/
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.3.2/tests/test_site/translations/babel.cfg
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.3.2/tests/test_site/translations/messages.pot
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.203196 mia-accounting-1.3.2/tests/test_site/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/test_site/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.3.2/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.3.2/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.203196 mia-accounting-1.3.2/tests/test_site/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-12 10:01:53.239195 mia-accounting-1.3.2/tests/test_site/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.3.2/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.3.2/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
--rw-r--r--   0 imacat    (1000) users      (100)    27871 2023-04-12 04:25:38.000000 mia-accounting-1.3.2/tests/test_unmatched_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.3.2/tests/test_utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    18890 2023-04-12 09:21:46.000000 mia-accounting-1.3.2/tests/testlib.py
--rw-r--r--   0 imacat    (1000) users      (100)    16670 2023-04-09 03:46:55.000000 mia-accounting-1.3.2/tests/testlib_journal_entry.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.120142 mia-accounting-1.3.3/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.3.3/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.3.3/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-13 01:57:14.120142 mia-accounting-1.3.3/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     5871 2023-04-11 13:56:49.000000 mia-accounting-1.3.3/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.960145 mia-accounting-1.3.3/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.3.3/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.3.3/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.960145 mia-accounting-1.3.3/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.960145 mia-accounting-1.3.3/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.3.3/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.960145 mia-accounting-1.3.3/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.3.3/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-10 16:05:21.000000 mia-accounting-1.3.3/docs/source/accounting.account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-10 16:05:21.000000 mia-accounting-1.3.3/docs/source/accounting.base_account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.currency.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.journal_entry.forms.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.journal_entry.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.journal_entry.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.option.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.report.period.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2043 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.report.reports.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.report.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1775 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.report.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1332 2023-04-10 16:05:21.000000 mia-accounting-1.3.3/docs/source/accounting.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      615 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.unmatched_offset.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2756 2023-04-10 16:05:22.000000 mia-accounting-1.3.3/docs/source/accounting.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-13 01:56:16.000000 mia-accounting-1.3.3/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.3.3/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.3.3/docs/source/history.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.3.3/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     3615 2023-04-11 13:56:49.000000 mia-accounting-1.3.3/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.3.3/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-13 01:56:16.000000 mia-accounting-1.3.3/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-13 01:57:14.120142 mia-accounting-1.3.3/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.956145 mia-accounting-1.3.3/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.964145 mia-accounting-1.3.3/src/accounting/
+-rw-r--r--   0 imacat    (1000) users      (100)     3065 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/__init__.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.964145 mia-accounting-1.3.3/src/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.3.3/src/accounting/account/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.3.3/src/accounting/account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.964145 mia-accounting-1.3.3/src/accounting/base_account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/base_account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/base_account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/base_account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.3.3/src/accounting/base_account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.3.3/src/accounting/base_account/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/commands.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.964145 mia-accounting-1.3.3/src/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/currency/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2212 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/src/accounting/currency/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/currency/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.3.3/src/accounting/currency/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/currency/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.3.3/src/accounting/currency/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.964145 mia-accounting-1.3.3/src/accounting/data/
+-rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.3.3/src/accounting/data/base_accounts.csv
+-rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.3.3/src/accounting/data/currencies.csv
+-rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.3.3/src/accounting/forms.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.964145 mia-accounting-1.3.3/src/accounting/journal_entry/
+-rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/journal_entry/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3283 2023-04-11 16:41:29.000000 mia-accounting-1.3.3/src/accounting/journal_entry/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.968145 mia-accounting-1.3.3/src/accounting/journal_entry/forms/
+-rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.3.3/src/accounting/journal_entry/forms/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11055 2023-04-08 10:12:54.000000 mia-accounting-1.3.3/src/accounting/journal_entry/forms/currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.3.3/src/accounting/journal_entry/forms/journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    19508 2023-04-07 16:44:13.000000 mia-accounting-1.3.3/src/accounting/journal_entry/forms/line_item.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/journal_entry/forms/reorder.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.3.3/src/accounting/journal_entry/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.968145 mia-accounting-1.3.3/src/accounting/journal_entry/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.3.3/src/accounting/journal_entry/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1729 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/journal_entry/utils/account_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12821 2023-04-04 09:21:31.000000 mia-accounting-1.3.3/src/accounting/journal_entry/utils/description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/journal_entry/utils/operators.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3787 2023-04-08 10:12:55.000000 mia-accounting-1.3.3/src/accounting/journal_entry/utils/original_line_items.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9472 2023-04-09 02:08:22.000000 mia-accounting-1.3.3/src/accounting/journal_entry/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.3.3/src/accounting/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    31691 2023-04-08 10:12:57.000000 mia-accounting-1.3.3/src/accounting/models.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.968145 mia-accounting-1.3.3/src/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/option/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.3.3/src/accounting/option/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.3.3/src/accounting/option/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.968145 mia-accounting-1.3.3/src/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.3.3/src/accounting/report/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.3.3/src/accounting/report/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.968145 mia-accounting-1.3.3/src/accounting/report/period/
+-rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.3.3/src/accounting/report/period/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/report/period/chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/report/period/description.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.3.3/src/accounting/report/period/month_end.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.3.3/src/accounting/report/period/parser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.3.3/src/accounting/report/period/period.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/report/period/shortcuts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/report/period/specification.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.972145 mia-accounting-1.3.3/src/accounting/report/reports/
+-rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.3.3/src/accounting/report/reports/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.3.3/src/accounting/report/reports/balance_sheet.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/report/reports/income_expenses.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.3.3/src/accounting/report/reports/income_statement.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.3.3/src/accounting/report/reports/journal.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.3.3/src/accounting/report/reports/ledger.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8819 2023-04-09 13:02:35.000000 mia-accounting-1.3.3/src/accounting/report/reports/search.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.3.3/src/accounting/report/reports/trial_balance.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6975 2023-04-08 16:39:45.000000 mia-accounting-1.3.3/src/accounting/report/reports/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4555 2023-04-08 10:12:55.000000 mia-accounting-1.3.3/src/accounting/report/reports/unapplied_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.3.3/src/accounting/report/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.972145 mia-accounting-1.3.3/src/accounting/report/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/report/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/report/utils/base_page_params.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.3.3/src/accounting/report/utils/base_report.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-09 04:04:18.000000 mia-accounting-1.3.3/src/accounting/report/utils/csv_export.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.3.3/src/accounting/report/utils/option_link.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6925 2023-04-08 10:12:55.000000 mia-accounting-1.3.3/src/accounting/report/utils/report_chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1305 2023-04-08 03:26:33.000000 mia-accounting-1.3.3/src/accounting/report/utils/report_type.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2740 2023-04-08 10:12:55.000000 mia-accounting-1.3.3/src/accounting/report/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4477 2023-04-09 02:08:22.000000 mia-accounting-1.3.3/src/accounting/report/utils/urls.py
+-rw-r--r--   0 imacat    (1000) users      (100)    10434 2023-04-09 02:08:22.000000 mia-accounting-1.3.3/src/accounting/report/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.956145 mia-accounting-1.3.3/src/accounting/static/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.972145 mia-accounting-1.3.3/src/accounting/static/css/
+-rw-r--r--   0 imacat    (1000) users      (100)    13001 2023-04-08 16:39:45.000000 mia-accounting-1.3.3/src/accounting/static/css/style.css
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.972145 mia-accounting-1.3.3/src/accounting/static/js/
+-rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/account-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/account-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/currency-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    38778 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/description-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/drag-and-drop-reorder.js
+-rw-r--r--   0 imacat    (1000) users      (100)     9092 2023-04-07 04:32:27.000000 mia-accounting-1.3.3/src/accounting/static/js/journal-entry-account-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    32504 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/journal-entry-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    19866 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/journal-entry-line-item-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/journal-entry-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/material-fab-speed-dial.js
+-rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/option-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    11640 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/original-line-item-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.3.3/src/accounting/static/js/period-chooser.js
+-rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.3.3/src/accounting/template_filters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/template_globals.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.956145 mia-accounting-1.3.3/src/accounting/templates/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.972145 mia-accounting-1.3.3/src/accounting/templates/accounting/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/account/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/account/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/account/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/account/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/account/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/base-account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/base-account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/base-account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/base.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/currency/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/currency/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/currency/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/currency/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/currency/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/currency/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3103 2023-04-10 23:49:07.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/include/nav.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/include/pagination.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/
+-rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.976145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3373 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)    14459 2023-04-05 01:08:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3131 2023-04-07 06:56:44.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6161 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3490 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/
+-rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/
+-rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/option/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/option/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/form-recurring-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.980145 mia-accounting-1.3.3/src/accounting/templates/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     5065 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/balance-sheet.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.984145 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/balance-sheet-section.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/period-chooser.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/search-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     5572 2023-04-04 23:56:52.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/toolbar-buttons.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4623 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/income-expenses.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4242 2023-04-04 10:04:12.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/income-statement.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/journal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4745 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/ledger.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/search.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-04 10:04:10.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/trial-balance.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2201 2023-04-08 10:12:55.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/unapplied-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4086 2023-04-08 16:39:45.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/report/unapplied.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.984145 mia-accounting-1.3.3/src/accounting/templates/accounting/unmatched-offset/
+-rw-r--r--   0 imacat    (1000) users      (100)     1212 2023-04-08 16:38:54.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/unmatched-offset/dashboard.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4668 2023-04-08 10:12:57.000000 mia-accounting-1.3.3/src/accounting/templates/accounting/unmatched-offset/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.040144 mia-accounting-1.3.3/src/accounting/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)    47460 2023-04-08 17:41:05.000000 mia-accounting-1.3.3/src/accounting/translations/accounting.pot
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.3.3/src/accounting/translations/babel.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.956145 mia-accounting-1.3.3/src/accounting/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.068143 mia-accounting-1.3.3/src/accounting/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.3/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.3/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.956145 mia-accounting-1.3.3/src/accounting/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.108142 mia-accounting-1.3.3/src/accounting/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.3/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.3/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.108142 mia-accounting-1.3.3/src/accounting/unmatched_offset/
+-rw-r--r--   0 imacat    (1000) users      (100)     1032 2023-04-08 10:12:57.000000 mia-accounting-1.3.3/src/accounting/unmatched_offset/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-08 10:12:57.000000 mia-accounting-1.3.3/src/accounting/unmatched_offset/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3178 2023-04-08 16:39:45.000000 mia-accounting-1.3.3/src/accounting/unmatched_offset/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.112142 mia-accounting-1.3.3/src/accounting/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.3.3/src/accounting/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/utils/cast.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/utils/current_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/utils/flash_errors.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.3.3/src/accounting/utils/journal_entry_types.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.3.3/src/accounting/utils/next_uri.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.3.3/src/accounting/utils/offset_alias.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5198 2023-04-08 16:39:45.000000 mia-accounting-1.3.3/src/accounting/utils/offset_matcher.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.3.3/src/accounting/utils/options.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.3.3/src/accounting/utils/pagination.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.3.3/src/accounting/utils/permission.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/utils/query.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/utils/random_id.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.3.3/src/accounting/utils/strip_text.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3080 2023-04-08 10:12:56.000000 mia-accounting-1.3.3/src/accounting/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.3.3/src/accounting/utils/user.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.112142 mia-accounting-1.3.3/src/mia_accounting.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     6670 2023-04-13 01:57:13.000000 mia-accounting-1.3.3/src/mia_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)    11477 2023-04-13 01:57:13.000000 mia-accounting-1.3.3/src/mia_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-13 01:57:13.000000 mia-accounting-1.3.3/src/mia_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-13 01:57:13.000000 mia-accounting-1.3.3/src/mia_accounting.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-13 01:57:13.000000 mia-accounting-1.3.3/src/mia_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.116142 mia-accounting-1.3.3/tests/
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-12 07:04:32.000000 mia-accounting-1.3.3/tests/babel-utils-test-site.py
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-12 07:04:32.000000 mia-accounting-1.3.3/tests/babel-utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32736 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/tests/test_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/tests/test_base_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/tests/test_commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)    23824 2023-04-10 15:59:48.000000 mia-accounting-1.3.3/tests/test_currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15999 2023-04-13 01:09:51.000000 mia-accounting-1.3.3/tests/test_description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)   103461 2023-04-13 01:09:51.000000 mia-accounting-1.3.3/tests/test_journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    38887 2023-04-13 01:09:51.000000 mia-accounting-1.3.3/tests/test_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15935 2023-04-13 01:09:51.000000 mia-accounting-1.3.3/tests/test_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15396 2023-04-13 01:09:51.000000 mia-accounting-1.3.3/tests/test_report.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.116142 mia-accounting-1.3.3/tests/test_site/
+-rw-r--r--   0 imacat    (1000) users      (100)     4505 2023-04-13 00:49:22.000000 mia-accounting-1.3.3/tests/test_site/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3898 2023-04-13 01:52:58.000000 mia-accounting-1.3.3/tests/test_site/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13223 2023-04-13 01:30:40.000000 mia-accounting-1.3.3/tests/test_site/lib.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.3.3/tests/test_site/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13048 2023-04-13 01:52:58.000000 mia-accounting-1.3.3/tests/test_site/reset.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.116142 mia-accounting-1.3.3/tests/test_site/static/
+-rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.3.3/tests/test_site/static/favicon.svg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.116142 mia-accounting-1.3.3/tests/test_site/templates/
+-rw-r--r--   0 imacat    (1000) users      (100)     6435 2023-04-12 10:05:13.000000 mia-accounting-1.3.3/tests/test_site/templates/base.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1239 2023-04-11 14:27:31.000000 mia-accounting-1.3.3/tests/test_site/templates/home.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1532 2023-04-11 14:03:59.000000 mia-accounting-1.3.3/tests/test_site/templates/login.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1838 2023-04-12 10:05:13.000000 mia-accounting-1.3.3/tests/test_site/templates/reset.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.116142 mia-accounting-1.3.3/tests/test_site/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.3.3/tests/test_site/translations/babel.cfg
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-12 09:59:51.000000 mia-accounting-1.3.3/tests/test_site/translations/messages.pot
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.956145 mia-accounting-1.3.3/tests/test_site/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.116142 mia-accounting-1.3.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.3.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:00:18.000000 mia-accounting-1.3.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:13.956145 mia-accounting-1.3.3/tests/test_site/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-13 01:57:14.116142 mia-accounting-1.3.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)     2275 2023-04-12 10:00:18.000000 mia-accounting-1.3.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     3505 2023-04-12 10:05:13.000000 mia-accounting-1.3.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
+-rw-r--r--   0 imacat    (1000) users      (100)    27896 2023-04-13 01:30:40.000000 mia-accounting-1.3.3/tests/test_unmatched_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.3.3/tests/test_utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5169 2023-04-13 01:09:51.000000 mia-accounting-1.3.3/tests/testlib.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16670 2023-04-13 01:09:51.000000 mia-accounting-1.3.3/tests/testlib_journal_entry.py
```

### Comparing `mia-accounting-1.3.2/LICENSE` & `mia-accounting-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/MANIFEST.in` & `mia-accounting-1.3.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/PKG-INFO` & `mia-accounting-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
 Keywords: mia,accounting,flask
```

### Comparing `mia-accounting-1.3.2/README.rst` & `mia-accounting-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/Makefile` & `mia-accounting-1.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/make.bat` & `mia-accounting-1.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/accounting.account.rst` & `mia-accounting-1.3.3/docs/source/accounting.account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/accounting.base_account.rst` & `mia-accounting-1.3.3/docs/source/accounting.base_account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/accounting.currency.rst` & `mia-accounting-1.3.3/docs/source/accounting.currency.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/accounting.journal_entry.forms.rst` & `mia-accounting-1.3.3/docs/source/accounting.journal_entry.forms.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/accounting.journal_entry.rst` & `mia-accounting-1.3.3/docs/source/accounting.journal_entry.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/accounting.journal_entry.utils.rst` & `mia-accounting-1.3.3/docs/source/accounting.journal_entry.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/accounting.option.rst` & `mia-accounting-1.3.3/docs/source/accounting.option.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/accounting.report.period.rst` & `mia-accounting-1.3.3/docs/source/accounting.report.period.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/accounting.report.reports.rst` & `mia-accounting-1.3.3/docs/source/accounting.report.reports.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/accounting.report.rst` & `mia-accounting-1.3.3/docs/source/accounting.report.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/accounting.report.utils.rst` & `mia-accounting-1.3.3/docs/source/accounting.report.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/accounting.rst` & `mia-accounting-1.3.3/docs/source/accounting.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/accounting.unmatched_offset.rst` & `mia-accounting-1.3.3/docs/source/accounting.unmatched_offset.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/accounting.utils.rst` & `mia-accounting-1.3.3/docs/source/accounting.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/conf.py` & `mia-accounting-1.3.3/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Mia! Accounting'
 copyright = '2023, imacat'
 author = 'imacat'
-release = '1.3.2'
+release = '1.3.3'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc']
 
 templates_path = ['_templates']
```

### Comparing `mia-accounting-1.3.2/docs/source/examples.rst` & `mia-accounting-1.3.3/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/history.rst` & `mia-accounting-1.3.3/docs/source/history.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/docs/source/intro.rst` & `mia-accounting-1.3.3/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/pyproject.toml` & `mia-accounting-1.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 [project]
 name = "mia-accounting"
-version = "1.3.2"
+version = "1.3.3"
 description = "A Flask accounting module."
 readme = "README.rst"
 requires-python = ">=3.11"
 authors = [
     {name = "imacat", email = "imacat@mail.imacat.idv.tw"},
 ]
 keywords = ["mia", "accounting", "flask"]
```

### Comparing `mia-accounting-1.3.2/src/accounting/__init__.py` & `mia-accounting-1.3.3/src/accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/account/__init__.py` & `mia-accounting-1.3.3/src/accounting/account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/account/commands.py` & `mia-accounting-1.3.3/src/accounting/account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/account/converters.py` & `mia-accounting-1.3.3/src/accounting/account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/account/forms.py` & `mia-accounting-1.3.3/src/accounting/account/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/account/queries.py` & `mia-accounting-1.3.3/src/accounting/account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/account/views.py` & `mia-accounting-1.3.3/src/accounting/account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/base_account/__init__.py` & `mia-accounting-1.3.3/src/accounting/base_account/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/base_account/commands.py` & `mia-accounting-1.3.3/src/accounting/base_account/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/base_account/converters.py` & `mia-accounting-1.3.3/src/accounting/base_account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/base_account/queries.py` & `mia-accounting-1.3.3/src/accounting/base_account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/base_account/views.py` & `mia-accounting-1.3.3/src/accounting/base_account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/commands.py` & `mia-accounting-1.3.3/src/accounting/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/currency/__init__.py` & `mia-accounting-1.3.3/src/accounting/currency/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/currency/commands.py` & `mia-accounting-1.3.3/src/accounting/currency/commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/currency/converters.py` & `mia-accounting-1.3.3/src/accounting/currency/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/currency/forms.py` & `mia-accounting-1.3.3/src/accounting/currency/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/currency/queries.py` & `mia-accounting-1.3.3/src/accounting/currency/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/currency/views.py` & `mia-accounting-1.3.3/src/accounting/currency/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/data/base_accounts.csv` & `mia-accounting-1.3.3/src/accounting/data/base_accounts.csv`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/forms.py` & `mia-accounting-1.3.3/src/accounting/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/journal_entry/__init__.py` & `mia-accounting-1.3.3/src/accounting/journal_entry/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/journal_entry/converters.py` & `mia-accounting-1.3.3/src/accounting/journal_entry/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/journal_entry/forms/__init__.py` & `mia-accounting-1.3.3/src/accounting/journal_entry/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/journal_entry/forms/currency.py` & `mia-accounting-1.3.3/src/accounting/journal_entry/forms/currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/journal_entry/forms/journal_entry.py` & `mia-accounting-1.3.3/src/accounting/journal_entry/forms/journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/journal_entry/forms/line_item.py` & `mia-accounting-1.3.3/src/accounting/journal_entry/forms/line_item.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/journal_entry/forms/reorder.py` & `mia-accounting-1.3.3/src/accounting/journal_entry/forms/reorder.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/journal_entry/template_filters.py` & `mia-accounting-1.3.3/src/accounting/journal_entry/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/journal_entry/utils/__init__.py` & `mia-accounting-1.3.3/src/accounting/journal_entry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/journal_entry/utils/account_option.py` & `mia-accounting-1.3.3/src/accounting/journal_entry/utils/account_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/journal_entry/utils/description_editor.py` & `mia-accounting-1.3.3/src/accounting/journal_entry/utils/description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/journal_entry/utils/operators.py` & `mia-accounting-1.3.3/src/accounting/journal_entry/utils/operators.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/journal_entry/utils/original_line_items.py` & `mia-accounting-1.3.3/src/accounting/journal_entry/utils/original_line_items.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/journal_entry/views.py` & `mia-accounting-1.3.3/src/accounting/journal_entry/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/locale.py` & `mia-accounting-1.3.3/src/accounting/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/models.py` & `mia-accounting-1.3.3/src/accounting/models.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/option/__init__.py` & `mia-accounting-1.3.3/src/accounting/option/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/option/forms.py` & `mia-accounting-1.3.3/src/accounting/option/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/option/views.py` & `mia-accounting-1.3.3/src/accounting/option/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/__init__.py` & `mia-accounting-1.3.3/src/accounting/report/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/converters.py` & `mia-accounting-1.3.3/src/accounting/report/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/period/__init__.py` & `mia-accounting-1.3.3/src/accounting/report/period/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/period/chooser.py` & `mia-accounting-1.3.3/src/accounting/report/period/chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/period/description.py` & `mia-accounting-1.3.3/src/accounting/report/period/description.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/period/month_end.py` & `mia-accounting-1.3.3/src/accounting/report/period/month_end.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/period/parser.py` & `mia-accounting-1.3.3/src/accounting/report/period/parser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/period/period.py` & `mia-accounting-1.3.3/src/accounting/report/period/period.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/period/shortcuts.py` & `mia-accounting-1.3.3/src/accounting/report/period/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/period/specification.py` & `mia-accounting-1.3.3/src/accounting/report/period/specification.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/reports/__init__.py` & `mia-accounting-1.3.3/src/accounting/report/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/reports/balance_sheet.py` & `mia-accounting-1.3.3/src/accounting/report/reports/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/reports/income_expenses.py` & `mia-accounting-1.3.3/src/accounting/report/reports/income_expenses.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/reports/income_statement.py` & `mia-accounting-1.3.3/src/accounting/report/reports/income_statement.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/reports/journal.py` & `mia-accounting-1.3.3/src/accounting/report/reports/journal.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/reports/ledger.py` & `mia-accounting-1.3.3/src/accounting/report/reports/ledger.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/reports/search.py` & `mia-accounting-1.3.3/src/accounting/report/reports/search.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/reports/trial_balance.py` & `mia-accounting-1.3.3/src/accounting/report/reports/trial_balance.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/reports/unapplied.py` & `mia-accounting-1.3.3/src/accounting/report/reports/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/reports/unapplied_accounts.py` & `mia-accounting-1.3.3/src/accounting/report/reports/unapplied_accounts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/template_filters.py` & `mia-accounting-1.3.3/src/accounting/report/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/utils/__init__.py` & `mia-accounting-1.3.3/src/accounting/report/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/utils/base_page_params.py` & `mia-accounting-1.3.3/src/accounting/report/utils/base_page_params.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/utils/base_report.py` & `mia-accounting-1.3.3/src/accounting/report/utils/base_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/utils/csv_export.py` & `mia-accounting-1.3.3/src/accounting/report/utils/csv_export.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/utils/option_link.py` & `mia-accounting-1.3.3/src/accounting/report/utils/option_link.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/utils/report_chooser.py` & `mia-accounting-1.3.3/src/accounting/report/utils/report_chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/utils/report_type.py` & `mia-accounting-1.3.3/src/accounting/report/utils/report_type.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/utils/unapplied.py` & `mia-accounting-1.3.3/src/accounting/report/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/utils/urls.py` & `mia-accounting-1.3.3/src/accounting/report/utils/urls.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/report/views.py` & `mia-accounting-1.3.3/src/accounting/report/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/static/css/style.css` & `mia-accounting-1.3.3/src/accounting/static/css/style.css`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/static/js/account-form.js` & `mia-accounting-1.3.3/src/accounting/static/js/account-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/static/js/account-order.js` & `mia-accounting-1.3.3/src/accounting/static/js/account-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/static/js/currency-form.js` & `mia-accounting-1.3.3/src/accounting/static/js/currency-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/static/js/description-editor.js` & `mia-accounting-1.3.3/src/accounting/static/js/description-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/static/js/drag-and-drop-reorder.js` & `mia-accounting-1.3.3/src/accounting/static/js/drag-and-drop-reorder.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/static/js/journal-entry-account-selector.js` & `mia-accounting-1.3.3/src/accounting/static/js/journal-entry-account-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/static/js/journal-entry-form.js` & `mia-accounting-1.3.3/src/accounting/static/js/journal-entry-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/static/js/journal-entry-line-item-editor.js` & `mia-accounting-1.3.3/src/accounting/static/js/journal-entry-line-item-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/static/js/journal-entry-order.js` & `mia-accounting-1.3.3/src/accounting/static/js/journal-entry-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/static/js/material-fab-speed-dial.js` & `mia-accounting-1.3.3/src/accounting/static/js/material-fab-speed-dial.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/static/js/option-form.js` & `mia-accounting-1.3.3/src/accounting/static/js/option-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/static/js/original-line-item-selector.js` & `mia-accounting-1.3.3/src/accounting/static/js/original-line-item-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/static/js/period-chooser.js` & `mia-accounting-1.3.3/src/accounting/static/js/period-chooser.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/template_filters.py` & `mia-accounting-1.3.3/src/accounting/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/template_globals.py` & `mia-accounting-1.3.3/src/accounting/template_globals.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/account/create.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/account/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/account/detail.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/account/edit.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/account/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/account/include/form.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/account/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/account/list.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/account/order.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/account/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/base-account/detail.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/base-account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/base-account/list.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/base-account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/base.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/currency/create.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/currency/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/currency/detail.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/currency/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/currency/edit.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/currency/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/currency/include/form.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/currency/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/currency/list.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/currency/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/include/nav.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/include/nav.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/include/pagination.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/include/pagination.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/create.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/detail.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/edit.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/detail.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form-currency.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form-line-item.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form-line-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/form.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/order.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/create.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/detail.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/edit.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/receipt/include/form.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/receipt/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/create.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/detail.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/edit.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/journal-entry/transfer/include/form.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/journal-entry/transfer/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/option/detail.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/option/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/option/form.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/option/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/form-recurring-item.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/form-recurring-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/balance-sheet.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/balance-sheet.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/balance-sheet-section.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/balance-sheet-section.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/ledger-row-desktop.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/ledger-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/ledger-row-mobile.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/ledger-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/period-chooser.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/period-chooser.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/search-modal.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/search-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/include/toolbar-buttons.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/include/toolbar-buttons.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/income-expenses.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/income-expenses.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/income-statement.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/income-statement.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/journal.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/journal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/ledger.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/ledger.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/search.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/search.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/trial-balance.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/trial-balance.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/unapplied-accounts.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/unapplied-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/report/unapplied.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/report/unapplied.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/unmatched-offset/dashboard.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/unmatched-offset/dashboard.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/templates/accounting/unmatched-offset/list.html` & `mia-accounting-1.3.3/src/accounting/templates/accounting/unmatched-offset/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/translations/accounting.pot` & `mia-accounting-1.3.3/src/accounting/translations/accounting.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo` & `mia-accounting-1.3.3/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po` & `mia-accounting-1.3.3/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo` & `mia-accounting-1.3.3/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po` & `mia-accounting-1.3.3/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/unmatched_offset/__init__.py` & `mia-accounting-1.3.3/src/accounting/unmatched_offset/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/unmatched_offset/queries.py` & `mia-accounting-1.3.3/src/accounting/unmatched_offset/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/unmatched_offset/views.py` & `mia-accounting-1.3.3/src/accounting/unmatched_offset/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/__init__.py` & `mia-accounting-1.3.3/src/accounting/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/cast.py` & `mia-accounting-1.3.3/src/accounting/utils/cast.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/current_account.py` & `mia-accounting-1.3.3/src/accounting/utils/current_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/flash_errors.py` & `mia-accounting-1.3.3/src/accounting/utils/flash_errors.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/journal_entry_types.py` & `mia-accounting-1.3.3/src/accounting/utils/journal_entry_types.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/next_uri.py` & `mia-accounting-1.3.3/src/accounting/utils/next_uri.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/offset_alias.py` & `mia-accounting-1.3.3/src/accounting/utils/offset_alias.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/offset_matcher.py` & `mia-accounting-1.3.3/src/accounting/utils/offset_matcher.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/options.py` & `mia-accounting-1.3.3/src/accounting/utils/options.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/pagination.py` & `mia-accounting-1.3.3/src/accounting/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/permission.py` & `mia-accounting-1.3.3/src/accounting/utils/permission.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/query.py` & `mia-accounting-1.3.3/src/accounting/utils/query.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/random_id.py` & `mia-accounting-1.3.3/src/accounting/utils/random_id.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/strip_text.py` & `mia-accounting-1.3.3/src/accounting/utils/strip_text.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/unapplied.py` & `mia-accounting-1.3.3/src/accounting/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/accounting/utils/user.py` & `mia-accounting-1.3.3/src/accounting/utils/user.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/src/mia_accounting.egg-info/PKG-INFO` & `mia-accounting-1.3.3/src/mia_accounting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
 Keywords: mia,accounting,flask
```

### Comparing `mia-accounting-1.3.2/src/mia_accounting.egg-info/SOURCES.txt` & `mia-accounting-1.3.3/src/mia_accounting.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,14 @@
 src/mia_accounting.egg-info/PKG-INFO
 src/mia_accounting.egg-info/SOURCES.txt
 src/mia_accounting.egg-info/dependency_links.txt
 src/mia_accounting.egg-info/requires.txt
 src/mia_accounting.egg-info/top_level.txt
 tests/babel-utils-test-site.py
 tests/babel-utils.py
-tests/make-sample.py
 tests/test_account.py
 tests/test_base_account.py
 tests/test_commands.py
 tests/test_currency.py
 tests/test_description_editor.py
 tests/test_journal_entry.py
 tests/test_offset.py
@@ -227,17 +226,17 @@
 tests/test_report.py
 tests/test_unmatched_offset.py
 tests/test_utils.py
 tests/testlib.py
 tests/testlib_journal_entry.py
 tests/test_site/__init__.py
 tests/test_site/auth.py
+tests/test_site/lib.py
 tests/test_site/locale.py
 tests/test_site/reset.py
-tests/test_site/data/sample.json
 tests/test_site/static/favicon.svg
 tests/test_site/templates/base.html
 tests/test_site/templates/home.html
 tests/test_site/templates/login.html
 tests/test_site/templates/reset.html
 tests/test_site/translations/babel.cfg
 tests/test_site/translations/messages.pot
```

### Comparing `mia-accounting-1.3.2/tests/babel-utils-test-site.py` & `mia-accounting-1.3.3/tests/babel-utils-test-site.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/babel-utils.py` & `mia-accounting-1.3.3/tests/babel-utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/make-sample.py` & `mia-accounting-1.3.3/tests/test_site/reset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,102 @@
-#! env python3
-# The Mia! Accounting Project.
-# Author: imacat@mail.imacat.idv.tw (imacat), 2023/4/9
+# The Mia! Accounting Demonstration Website.
+# Author: imacat@mail.imacat.idv.tw (imacat), 2023/4/12
 
 #  Copyright (c) 2023 imacat.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-"""The sample data generation.
+"""The data reset for the Mia! Accounting demonstration website.
 
 """
 from datetime import date, timedelta
 
-import click
-
-from testlib import Accounts, create_test_app, JournalEntryLineItemData, \
-    JournalEntryCurrencyData, JournalEntryData, \
-    BaseTestData
-
-
-@click.command()
-@click.argument("file")
-def main(file) -> None:
-    """Creates the sample data and output to a file."""
-    data: SampleData = SampleData(create_test_app(), "editor")
-    with open(file, "wt") as fp:
-        fp.write(data.json())
+from flask import Flask, Blueprint, url_for, flash, redirect, session, \
+    render_template, current_app
+from flask_babel import lazy_gettext
+
+from . import db
+from .auth import admin_required
+from .lib import Accounts, JournalEntryLineItemData, JournalEntryData, \
+    JournalEntryCurrencyData, BaseTestData
+
+bp: Blueprint = Blueprint("reset", __name__, url_prefix="/")
+
+
+@bp.get("reset", endpoint="reset-page")
+@admin_required
+def reset() -> str:
+    """Resets the sample data.
+
+    :return: Redirection to the accounting application.
+    """
+    return render_template("reset.html")
+
+
+@bp.post("sample", endpoint="sample")
+@admin_required
+def reset_sample() -> redirect:
+    """Resets the sample data.
+
+    :return: Redirection to the accounting application.
+    """
+    from accounting.utils.cast import s
+    __reset_database()
+    SampleData(current_app, "editor").populate()
+    flash(s(lazy_gettext(
+        "The sample data are emptied and reset successfully.")), "success")
+    return redirect(url_for("accounting-report.default"))
+
+
+@bp.post("reset", endpoint="clean-up")
+@admin_required
+def clean_up() -> redirect:
+    """Clean-up the database data.
+
+    :return: Redirection to the accounting application.
+    """
+    from accounting.utils.cast import s
+    __reset_database()
+    flash(s(lazy_gettext("The database is emptied successfully.")), "success")
+    return redirect(url_for("accounting-report.default"))
+
+
+def __reset_database() -> None:
+    """Resets the database.
+
+    :return: None.
+    """
+    from accounting.models import Currency, CurrencyL10n, BaseAccount, \
+        BaseAccountL10n, Account, AccountL10n, JournalEntry, \
+        JournalEntryLineItem
+    from accounting.base_account import init_base_accounts_command
+    from accounting.account import init_accounts_command
+    from accounting.currency import init_currencies_command
+
+    JournalEntryLineItem.query.delete()
+    JournalEntry.query.delete()
+    CurrencyL10n.query.delete()
+    Currency.query.delete()
+    AccountL10n.query.delete()
+    Account.query.delete()
+    BaseAccountL10n.query.delete()
+    BaseAccount.query.delete()
+    init_base_accounts_command()
+    init_accounts_command(session["user"])
+    init_currencies_command(session["user"])
+    db.session.commit()
 
 
 class SampleData(BaseTestData):
     """The sample data."""
 
     def _init_data(self) -> None:
         self.__add_recurring()
@@ -298,9 +357,14 @@
                 currency,
                 [JournalEntryLineItemData(
                     debit_account, debit_description, amount)],
                 [JournalEntryLineItemData(
                     credit_account, credit_description, amount)])]))
 
 
-if __name__ == "__main__":
-    main()
+def init_app(app: Flask) -> None:
+    """Initialize the localization.
+
+    :param app: The Flask application.
+    :return: None.
+    """
+    app.register_blueprint(bp)
```

### Comparing `mia-accounting-1.3.2/tests/test_account.py` & `mia-accounting-1.3.3/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_base_account.py` & `mia-accounting-1.3.3/tests/test_base_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_commands.py` & `mia-accounting-1.3.3/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_currency.py` & `mia-accounting-1.3.3/tests/test_currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_description_editor.py` & `mia-accounting-1.3.3/tests/test_description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_journal_entry.py` & `mia-accounting-1.3.3/tests/test_journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_offset.py` & `mia-accounting-1.3.3/tests/test_offset.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 import unittest
 from decimal import Decimal
 
 import httpx
 from flask import Flask
 
 from test_site import db
-from testlib import Accounts, create_test_app, get_client, \
-    match_journal_entry_detail, JournalEntryLineItemData, \
-    JournalEntryCurrencyData, JournalEntryData, BaseTestData
+from test_site.lib import JournalEntryLineItemData, JournalEntryCurrencyData, \
+    JournalEntryData, BaseTestData
+from testlib import NEXT_URI, Accounts, create_test_app, get_client, \
+    match_journal_entry_detail
 
 PREFIX: str = "/accounting/journal-entries"
 """The URL prefix for the journal entry management."""
 
 
 class OffsetTestCase(unittest.TestCase):
     """The offset test case."""
@@ -80,96 +81,97 @@
                      original_line_item=self.data.l_r_or1d),
                  JournalEntryLineItemData(
                      Accounts.RECEIVABLE,
                      self.data.l_r_or3d.description, "100",
                      original_line_item=self.data.l_r_or3d)])])
 
         # Non-existing original line item ID
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         form["currency-1-credit-1-original_line_item_id"] = "9999"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The same debit or credit
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         form["currency-1-credit-1-original_line_item_id"] \
             = str(self.data.l_p_or1c.id)
         form["currency-1-credit-1-account_code"] = self.data.l_p_or1c.account
         form["currency-1-credit-1-amount"] = "100"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The original line item does not need offset
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = False
             db.session.commit()
         response = self.client.post(
-            store_uri, data=journal_entry_data.new_form(self.csrf_token))
+            store_uri,
+            data=journal_entry_data.new_form(self.csrf_token, NEXT_URI))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         form["currency-1-credit-1-original_line_item_id"] \
             = str(self.data.l_p_of1d.id)
         form["currency-1-credit-1-account_code"] = self.data.l_p_of1d.account
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same currency
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         form["currency-1-code"] = "EUR"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same account
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         form["currency-1-credit-1-account_code"] = Accounts.NOTES_RECEIVABLE
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not exceeding net balance - partially offset
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   + Decimal("0.01"))
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not exceeding net balance - unmatched
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         form["currency-1-credit-3-amount"] \
             = str(journal_entry_data.currencies[0].credit[2].amount
                   + Decimal("0.01"))
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not before the original line items
         old_days = journal_entry_data.days
         journal_entry_data.days = old_days + 1
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
         journal_entry_data.days = old_days
 
         # Success
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             for offset in journal_entry.currencies[0].credit:
@@ -190,22 +192,22 @@
         journal_entry_data.days = self.data.j_r_or2.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("600")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("600")
         journal_entry_data.currencies[0].debit[2].amount = Decimal("600")
         journal_entry_data.currencies[0].credit[2].amount = Decimal("600")
 
         # Non-existing original line item ID
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-credit-1-original_line_item_id"] = "9999"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # The same debit or credit
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-credit-1-original_line_item_id"] \
             = str(self.data.l_p_or1c.id)
         form["currency-1-credit-1-account_code"] = self.data.l_p_or1c.account
         form["currency-1-debit-1-amount"] = "100"
         form["currency-1-credit-1-amount"] = "100"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
@@ -213,80 +215,81 @@
 
         # The original line item does not need offset
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = False
             db.session.commit()
         response = self.client.post(
-            update_uri, data=journal_entry_data.update_form(self.csrf_token))
+            update_uri,
+            data=journal_entry_data.update_form(self.csrf_token, NEXT_URI))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         with self.app.app_context():
             account = Account.find_by_code(Accounts.RECEIVABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-credit-1-original_line_item_id"] \
             = str(self.data.l_p_of1d.id)
         form["currency-1-credit-1-account_code"] = self.data.l_p_of1d.account
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same currency
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-code"] = "EUR"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same account
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-credit-1-account_code"] = Accounts.NOTES_RECEIVABLE
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not exceeding net balance - partially offset
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   + Decimal("0.01"))
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   + Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not exceeding net balance - unmatched
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-3-amount"] \
             = str(journal_entry_data.currencies[0].debit[2].amount
                   + Decimal("0.01"))
         form["currency-1-credit-3-amount"] \
             = str(journal_entry_data.currencies[0].credit[2].amount
                   + Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not before the original line items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days + 1
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         journal_entry_data.days = old_days
 
         # Success
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{journal_entry_data.id}?next=%2F_next")
 
     def test_edit_receivable_original_line_item(self) -> None:
         """Tests to edit the receivable original line item.
@@ -303,69 +306,69 @@
         journal_entry_data.days = self.data.j_r_of1.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("800")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("800")
         journal_entry_data.currencies[0].debit[1].amount = Decimal("3.4")
         journal_entry_data.currencies[0].credit[1].amount = Decimal("3.4")
 
         # Not the same currency
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-code"] = "EUR"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same account
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-1-account_code"] = Accounts.NOTES_RECEIVABLE
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not less than offset total - partially offset
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   - Decimal("0.01"))
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   - Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not less than offset total - fully offset
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-2-amount"] \
             = str(journal_entry_data.currencies[0].debit[1].amount
                   - Decimal("0.01"))
         form["currency-1-credit-2-amount"] \
             = str(journal_entry_data.currencies[0].credit[1].amount
                   - Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not after the offset items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days - 1
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         journal_entry_data.days = old_days
 
         # Not deleting matched original line items
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         del form["currency-1-debit-1-id"]
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Success
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{journal_entry_data.id}?next=%2F_next")
 
         # The original line item is always before the offset item, even when
         # they happen in the same day.
@@ -404,96 +407,97 @@
                  JournalEntryLineItemData(
                      Accounts.PAYABLE,
                      self.data.l_p_or3c.description, "120",
                      original_line_item=self.data.l_p_or3c)],
                 [])])
 
         # Non-existing original line item ID
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-1-original_line_item_id"] = "9999"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The same debit or credit
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-1-original_line_item_id"] \
             = str(self.data.l_r_or1d.id)
         form["currency-1-debit-1-account_code"] = self.data.l_r_or1d.account
         form["currency-1-debit-1-amount"] = "100"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # The original line item does not need offset
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = False
             db.session.commit()
         response = self.client.post(
-            store_uri, data=journal_entry_data.new_form(self.csrf_token))
+            store_uri,
+            data=journal_entry_data.new_form(self.csrf_token, NEXT_URI))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-1-original_line_item_id"] \
             = str(self.data.l_r_of1c.id)
         form["currency-1-debit-1-account_code"] = self.data.l_r_of1c.account
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same currency
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         form["currency-1-code"] = "EUR"
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not the same account
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-1-account_code"] = Accounts.NOTES_PAYABLE
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not exceeding net balance - partially offset
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   + Decimal("0.01"))
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not exceeding net balance - unmatched
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-3-amount"] \
             = str(journal_entry_data.currencies[0].debit[2].amount
                   + Decimal("0.01"))
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
 
         # Not before the original line items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days + 1
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], create_uri)
         journal_entry_data.days = old_days
 
         # Success
-        form = journal_entry_data.new_form(self.csrf_token)
+        form = journal_entry_data.new_form(self.csrf_token, NEXT_URI)
         response = self.client.post(store_uri, data=form)
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             for offset in journal_entry.currencies[0].debit:
@@ -514,22 +518,22 @@
         journal_entry_data.days = self.data.j_p_or2.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("1100")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("1100")
         journal_entry_data.currencies[0].debit[2].amount = Decimal("900")
         journal_entry_data.currencies[0].credit[2].amount = Decimal("900")
 
         # Non-existing original line item ID
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-1-original_line_item_id"] = "9999"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # The same debit or credit
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-1-original_line_item_id"] \
             = str(self.data.l_r_or1d.id)
         form["currency-1-debit-1-account_code"] = self.data.l_r_or1d.account
         form["currency-1-debit-1-amount"] = "100"
         form["currency-1-credit-1-amount"] = "100"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
@@ -537,80 +541,81 @@
 
         # The original line item does not need offset
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = False
             db.session.commit()
         response = self.client.post(
-            update_uri, data=journal_entry_data.update_form(self.csrf_token))
+            update_uri,
+            data=journal_entry_data.update_form(self.csrf_token, NEXT_URI))
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         with self.app.app_context():
             account = Account.find_by_code(Accounts.PAYABLE)
             account.is_need_offset = True
             db.session.commit()
 
         # The original line item is also an offset
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-1-original_line_item_id"] \
             = str(self.data.l_r_of1c.id)
         form["currency-1-debit-1-account_code"] = self.data.l_r_of1c.account
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same currency
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-code"] = "EUR"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same account
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-1-account_code"] = Accounts.NOTES_PAYABLE
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not exceeding net balance - partially offset
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   + Decimal("0.01"))
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   + Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not exceeding net balance - unmatched
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-3-amount"] \
             = str(journal_entry_data.currencies[0].debit[2].amount
                   + Decimal("0.01"))
         form["currency-1-credit-3-amount"] \
             = str(journal_entry_data.currencies[0].credit[2].amount
                   + Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not before the original line items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days + 1
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         journal_entry_data.days = old_days
 
         # Success
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         journal_entry_id: int \
             = match_journal_entry_detail(response.headers["Location"])
         with self.app.app_context():
             journal_entry = db.session.get(JournalEntry, journal_entry_id)
             for offset in journal_entry.currencies[0].debit:
@@ -631,69 +636,69 @@
         journal_entry_data.days = self.data.j_p_of1.days
         journal_entry_data.currencies[0].debit[0].amount = Decimal("1200")
         journal_entry_data.currencies[0].credit[0].amount = Decimal("1200")
         journal_entry_data.currencies[0].debit[1].amount = Decimal("0.9")
         journal_entry_data.currencies[0].credit[1].amount = Decimal("0.9")
 
         # Not the same currency
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-code"] = "EUR"
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not the same account
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-credit-1-account_code"] = Accounts.NOTES_PAYABLE
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not less than offset total - partially offset
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-1-amount"] \
             = str(journal_entry_data.currencies[0].debit[0].amount
                   - Decimal("0.01"))
         form["currency-1-credit-1-amount"] \
             = str(journal_entry_data.currencies[0].credit[0].amount
                   - Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not less than offset total - fully offset
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         form["currency-1-debit-2-amount"] \
             = str(journal_entry_data.currencies[0].debit[1].amount
                   - Decimal("0.01"))
         form["currency-1-credit-2-amount"] \
             = str(journal_entry_data.currencies[0].credit[1].amount
                   - Decimal("0.01"))
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Not after the offset items
         old_days: int = journal_entry_data.days
         journal_entry_data.days = old_days - 1
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
         journal_entry_data.days = old_days
 
         # Not deleting matched original line items
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         del form["currency-1-credit-1-id"]
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], edit_uri)
 
         # Success
-        form = journal_entry_data.update_form(self.csrf_token)
+        form = journal_entry_data.update_form(self.csrf_token, NEXT_URI)
         response = self.client.post(update_uri, data=form)
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"],
                          f"{PREFIX}/{journal_entry_data.id}?next=%2F_next")
 
         # The original line item is always before the offset item, even when
         # they happen in the same day
```

### Comparing `mia-accounting-1.3.2/tests/test_option.py` & `mia-accounting-1.3.3/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_report.py` & `mia-accounting-1.3.3/tests/test_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 """
 import unittest
 from datetime import date
 
 import httpx
 from flask import Flask
 
-from testlib import create_test_app, get_client, Accounts, BaseTestData
+from test_site.lib import BaseTestData
+from testlib import create_test_app, get_client, Accounts
 
 PREFIX: str = "/accounting"
 """The URL prefix for the reports."""
 CSV_MIME: str = "text/csv; charset=utf-8"
 """The MIME type of the downloaded CSV files."""
```

### Comparing `mia-accounting-1.3.2/tests/test_site/__init__.py` & `mia-accounting-1.3.3/tests/test_site/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_site/auth.py` & `mia-accounting-1.3.3/tests/test_site/auth.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The authentication for the Mia! Accounting demonstration website.
 
 """
+import typing as t
+
 from flask import Blueprint, render_template, Flask, redirect, url_for, \
-    session, request, g, Response
+    session, request, g, Response, abort
 
 from . import db
 
 bp: Blueprint = Blueprint("auth", __name__, url_prefix="/")
 
 
 class User(db.Model):
@@ -89,14 +91,39 @@
             g.user = None
         else:
             g.user = User.query.filter(
                 User.username == session["user"]).first()
     return g.user
 
 
+def admin_required(view: t.Callable) -> t.Callable:
+    """The view decorator to require the user to be an administrator.
+
+    :param view: The view.
+    :return: The decorated view.
+    """
+
+    def decorated_view(*args, **kwargs):
+        """The decorated view that tests against a permission rule.
+
+        :param args: The arguments of the view.
+        :param kwargs: The keyword arguments of the view.
+        :return: The response of the view.
+        :raise Forbidden: When the user is denied.
+        """
+        from accounting.utils.next_uri import append_next
+        if "user" not in session:
+            return redirect(append_next(url_for("auth.login")))
+        if session["user"] != "admin":
+            abort(403)
+        return view(*args, **kwargs)
+
+    return decorated_view
+
+
 def init_app(app: Flask) -> None:
     """Initialize the localization.
 
     :param app: The Flask application.
     :return: None.
     """
     app.register_blueprint(bp)
```

### Comparing `mia-accounting-1.3.2/tests/test_site/locale.py` & `mia-accounting-1.3.3/tests/test_site/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_site/static/favicon.svg` & `mia-accounting-1.3.3/tests/test_site/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_site/templates/base.html` & `mia-accounting-1.3.3/tests/test_site/templates/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_site/templates/home.html` & `mia-accounting-1.3.3/tests/test_site/templates/home.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_site/templates/login.html` & `mia-accounting-1.3.3/tests/test_site/templates/login.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_site/templates/reset.html` & `mia-accounting-1.3.3/tests/test_site/templates/reset.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_site/translations/messages.pot` & `mia-accounting-1.3.3/tests/test_site/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo` & `mia-accounting-1.3.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po` & `mia-accounting-1.3.3/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo` & `mia-accounting-1.3.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po` & `mia-accounting-1.3.3/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/test_unmatched_offset.py` & `mia-accounting-1.3.3/tests/test_unmatched_offset.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 """
 import unittest
 
 import httpx
 from flask import Flask
 
 from test_site import db
-from testlib import create_test_app, get_client, Accounts, \
-    JournalEntryCurrencyData, JournalEntryData, BaseTestData
+from test_site.lib import JournalEntryCurrencyData, JournalEntryData, \
+    BaseTestData
+from testlib import create_test_app, get_client, Accounts
 
 PREFIX: str = "/accounting/unmatched-offsets"
 """The URL prefix for the unmatched offset management."""
 
 
 class UnmatchedOffsetTestCase(unittest.TestCase):
     """The unmatched offset test case."""
```

### Comparing `mia-accounting-1.3.2/tests/test_utils.py` & `mia-accounting-1.3.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.3.2/tests/testlib.py` & `mia-accounting-1.3.3/tests/test_site/lib.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,172 +1,51 @@
-# The Mia! Accounting Project.
-# Author: imacat@mail.imacat.idv.tw (imacat), 2023/1/27
+# The Mia! Accounting Demonstration Website.
+# Author: imacat@mail.imacat.idv.tw (imacat), 2023/4/13
 
 #  Copyright (c) 2023 imacat.
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-"""The common test libraries.
+"""The common library for the Mia! Accounting demonstration website.
 
 """
 from __future__ import annotations
 
-import json
-import re
 import typing as t
 from abc import ABC, abstractmethod
 from datetime import date, timedelta
+from decimal import Decimal
 from secrets import randbelow
 
-from decimal import Decimal
 import sqlalchemy as sa
+from flask import Flask
 
-import httpx
-from flask import Flask, render_template_string
-
-from test_site import create_app, db
-from test_site.auth import User
-
-TEST_SERVER: str = "https://testserver"
-"""The test server URI."""
-NEXT_URI: str = "/_next"
-"""The next URI."""
+from . import db
+from .auth import User
 
 
 class Accounts:
     """The shortcuts to the common accounts."""
     CASH: str = "1111-001"
-    PETTY_CASH: str = "1112-001"
     BANK: str = "1113-001"
-    NOTES_RECEIVABLE: str = "1131-001"
     RECEIVABLE: str = "1141-001"
     MACHINERY: str = "1441-001"
-    PREPAID: str = "1258-001"
-    NOTES_PAYABLE: str = "2131-001"
     PAYABLE: str = "2141-001"
-    SALES: str = "4111-001"
     SERVICE: str = "4611-001"
-    AGENCY: str = "4711-001"
     RENT_EXPENSE: str = "6252-001"
-    OFFICE: str = "6253-001"
-    TRAVEL: str = "6254-001"
-    POSTAGE: str = "6256-001"
-    UTILITIES: str = "6261-001"
-    INSURANCE: str = "6262-001"
     MEAL: str = "6272-001"
-    INTEREST: str = "7111-001"
-    DONATION: str = "7481-001"
-    RENT_INCOME: str = "7482-001"
-
-
-def create_test_app() -> Flask:
-    """Creates and returns the testing Flask application.
-
-    :return: The testing Flask application.
-    """
-    app: Flask = create_app(is_testing=True)
-
-    @app.get("/.csrf-token")
-    def get_csrf_token_view() -> str:
-        """The test view to return the CSRF token."""
-        return render_template_string("{{csrf_token()}}")
-
-    @app.get("/.errors")
-    def get_errors_view() -> str:
-        """The test view to return the CSRF token."""
-        return render_template_string("{{get_flashed_messages()|tojson}}")
-
-    return app
-
-
-def get_csrf_token(client: httpx.Client) -> str:
-    """Returns the CSRF token.
-
-    :param client: The httpx client.
-    :return: The CSRF token.
-    """
-    return client.get("/.csrf-token").text
-
-
-def get_client(app: Flask, username: str) -> tuple[httpx.Client, str]:
-    """Returns a user client.
-
-    :param app: The Flask application.
-    :param username: The username.
-    :return: A tuple of the client and the CSRF token.
-    """
-    client: httpx.Client = httpx.Client(app=app, base_url=TEST_SERVER)
-    client.headers["Referer"] = TEST_SERVER
-    csrf_token: str = get_csrf_token(client)
-    response: httpx.Response = client.post("/login",
-                                           data={"csrf_token": csrf_token,
-                                                 "next": "/",
-                                                 "username": username})
-    assert response.status_code == 302
-    assert response.headers["Location"] == "/"
-    return client, csrf_token
-
-
-def set_locale(client: httpx.Client, csrf_token: str,
-               locale: t.Literal["en", "zh_Hant", "zh_Hans"]) -> None:
-    """Sets the current locale.
-
-    :param client: The test client.
-    :param csrf_token: The CSRF token.
-    :param locale: The locale.
-    :return: None.
-    """
-    response: httpx.Response = client.post("/locale",
-                                           data={"csrf_token": csrf_token,
-                                                 "locale": locale,
-                                                 "next": "/next"})
-    assert response.status_code == 302
-    assert response.headers["Location"] == "/next"
-
-
-def add_journal_entry(client: httpx.Client, form: dict[str, str]) -> int:
-    """Adds a transfer journal entry.
-
-    :param client: The client.
-    :param form: The form data.
-    :return: The newly-added journal entry ID.
-    """
-    prefix: str = "/accounting/journal-entries"
-    journal_entry_type: str = "transfer"
-    if len({x for x in form if "-debit-" in x}) == 0:
-        journal_entry_type = "receipt"
-    elif len({x for x in form if "-credit-" in x}) == 0:
-        journal_entry_type = "disbursement"
-    store_uri = f"{prefix}/store/{journal_entry_type}"
-    response: httpx.Response = client.post(store_uri, data=form)
-    assert response.status_code == 302
-    return match_journal_entry_detail(response.headers["Location"])
-
-
-def match_journal_entry_detail(location: str) -> int:
-    """Validates if the redirect location is the journal entry detail, and
-    returns the journal entry ID on success.
-
-    :param location: The redirect location.
-    :return: The journal entry ID.
-    :raise AssertionError: When the location is not the journal entry detail.
-    """
-    m: re.Match = re.match(
-        r"^/accounting/journal-entries/(\d+)\?next=%2F_next", location)
-    assert m is not None
-    return int(m.group(1))
 
 
 class JournalEntryLineItemData:
     """The journal entry line item data."""
 
     def __init__(self, account: str, description: str | None, amount: str,
                  original_line_item: JournalEntryLineItemData | None = None):
@@ -257,41 +136,44 @@
         self.note: str | None = None
         for currency in self.currencies:
             for line_item in currency.debit:
                 line_item.journal_entry = self
             for line_item in currency.credit:
                 line_item.journal_entry = self
 
-    def new_form(self, csrf_token: str) -> dict[str, str]:
+    def new_form(self, csrf_token: str, next_uri: str) -> dict[str, str]:
         """Returns the journal entry as a creation form.
 
         :param csrf_token: The CSRF token.
+        :param next_uri: The next URI.
         :return: The journal entry as a creation form.
         """
-        return self.__form(csrf_token, is_update=False)
+        return self.__form(csrf_token, next_uri, is_update=False)
 
-    def update_form(self, csrf_token: str) -> dict[str, str]:
+    def update_form(self, csrf_token: str, next_uri: str) -> dict[str, str]:
         """Returns the journal entry as an update form.
 
         :param csrf_token: The CSRF token.
+        :param next_uri: The next URI.
         :return: The journal entry as an update form.
         """
-        return self.__form(csrf_token, is_update=True)
+        return self.__form(csrf_token, next_uri, is_update=True)
 
-    def __form(self, csrf_token: str, is_update: bool = False) \
+    def __form(self, csrf_token: str, next_uri: str, is_update: bool = False) \
             -> dict[str, str]:
         """Returns the journal entry as a form.
 
         :param csrf_token: The CSRF token.
+        :param next_uri: The next URI.
         :param is_update: True for an update operation, or False otherwise
         :return: The journal entry as a form.
         """
         journal_entry_date: date = date.today() - timedelta(days=self.days)
         form: dict[str, str] = {"csrf_token": csrf_token,
-                                "next": NEXT_URI,
+                                "next": next_uri,
                                 "date": journal_entry_date.isoformat()}
         for i in range(len(self.currencies)):
             form.update(self.currencies[i].form(i + 1, is_update))
         if self.note is not None:
             form["note"] = self.note
         return form
 
@@ -301,16 +183,16 @@
 
     def __init__(self, app: Flask, username: str):
         """Constructs the test data.
 
         :param app: The Flask application.
         :param username: The username.
         """
-        self.__app: Flask = app
-        with self.__app.app_context():
+        self._app: Flask = app
+        with self._app.app_context():
             current_user: User | None = User.query\
                 .filter(User.username == username).first()
             assert current_user is not None
             self.__current_user_id: int = current_user.id
             self.__journal_entries: list[dict[str, t.Any]] = []
             self.__line_items: list[dict[str, t.Any]] = []
             self._init_data()
@@ -324,63 +206,20 @@
 
     def populate(self) -> None:
         """Populates the data into the database.
 
         :return: None
         """
         from accounting.models import JournalEntry, JournalEntryLineItem
-        with self.__app.app_context():
+        with self._app.app_context():
             db.session.execute(sa.insert(JournalEntry), self.__journal_entries)
             db.session.execute(sa.insert(JournalEntryLineItem),
                                self.__line_items)
             db.session.commit()
 
-    def json(self) -> str:
-        """Returns the data as JSON.
-
-        :return: The JSON string.
-        """
-        from accounting.models import Account
-        today: date = date.today()
-
-        def filter_journal_entry(data: dict[str, t.Any]) -> list[t.Any]:
-            """Filters the journal entry data for JSON encoding.
-
-            :param data: The journal entry data.
-            :return: The journal entry data for JSON encoding.
-            """
-            data = data.copy()
-            data["date"] = (today - data["date"]).days
-            del data["created_by_id"]
-            del data["updated_by_id"]
-            return [data[x] for x in ["id", "date", "no", "note"]]
-
-        def filter_line_item(data: dict[str, t.Any]) -> list[t.Any]:
-            """Filters the journal entry line item data for JSON encoding.
-
-            :param data: The journal entry line item data.
-            :return: The journal entry line item data for JSON encoding.
-            """
-            data = data.copy()
-            with self.__app.app_context():
-                data["account_id"] \
-                    = db.session.get(Account, data["account_id"]).code
-            data["amount"] = str(data["amount"])
-            if "original_line_item_id" not in data:
-                data["original_line_item_id"] = None
-            return [data[x] for x in ["id", "journal_entry_id",
-                                      "original_line_item_id", "is_debit",
-                                      "no", "account_id", "currency_code",
-                                      "description", "amount"]]
-
-        return json.dumps(
-            [[filter_journal_entry(x) for x in self.__journal_entries],
-             [filter_line_item(x) for x in self.__line_items]],
-            ensure_ascii=False, separators=(",", ":"))
-
     @staticmethod
     def _couple(description: str, amount: str, debit: str, credit: str) \
             -> tuple[JournalEntryLineItemData, JournalEntryLineItemData]:
         """Returns a couple of debit-credit line items.
 
         :param description: The description.
         :param amount: The amount.
```

### Comparing `mia-accounting-1.3.2/tests/testlib_journal_entry.py` & `mia-accounting-1.3.3/tests/testlib_journal_entry.py`

 * *Files identical despite different names*

