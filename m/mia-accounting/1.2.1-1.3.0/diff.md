# Comparing `tmp/mia-accounting-1.2.1.tar.gz` & `tmp/mia-accounting-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia-accounting-1.2.1.tar", last modified: Sun Apr  9 13:04:55 2023, max compression
+gzip compressed data, was "mia-accounting-1.3.0.tar", last modified: Mon Apr 10 16:09:35 2023, max compression
```

## Comparing `mia-accounting-1.2.1.tar` & `mia-accounting-1.3.0.tar`

### file list

```diff
@@ -1,303 +1,305 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.344353 mia-accounting-1.2.1/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.2.1/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.2.1/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     7024 2023-04-09 13:04:55.344353 mia-accounting-1.2.1/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     6225 2023-04-06 02:00:23.000000 mia-accounting-1.2.1/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.548368 mia-accounting-1.2.1/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.2.1/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.2.1/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.684365 mia-accounting-1.2.1/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.712365 mia-accounting-1.2.1/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.2.1/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.712365 mia-accounting-1.2.1/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.2.1/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-09 04:22:17.000000 mia-accounting-1.2.1/docs/source/accounting.account.rst
--rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-09 04:22:17.000000 mia-accounting-1.2.1/docs/source/accounting.base_account.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-09 04:22:17.000000 mia-accounting-1.2.1/docs/source/accounting.currency.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-09 04:22:17.000000 mia-accounting-1.2.1/docs/source/accounting.journal_entry.forms.rst
--rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-09 04:22:17.000000 mia-accounting-1.2.1/docs/source/accounting.journal_entry.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-09 04:22:17.000000 mia-accounting-1.2.1/docs/source/accounting.journal_entry.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-09 04:22:17.000000 mia-accounting-1.2.1/docs/source/accounting.option.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-09 04:22:17.000000 mia-accounting-1.2.1/docs/source/accounting.report.period.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2043 2023-04-09 04:22:17.000000 mia-accounting-1.2.1/docs/source/accounting.report.reports.rst
--rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-09 04:22:17.000000 mia-accounting-1.2.1/docs/source/accounting.report.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1775 2023-04-09 04:22:17.000000 mia-accounting-1.2.1/docs/source/accounting.report.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1186 2023-04-09 04:22:17.000000 mia-accounting-1.2.1/docs/source/accounting.rst
--rw-r--r--   0 imacat    (1000) users      (100)      615 2023-04-09 04:22:17.000000 mia-accounting-1.2.1/docs/source/accounting.unmatched_offset.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2756 2023-04-09 04:22:17.000000 mia-accounting-1.2.1/docs/source/accounting.utils.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-09 13:04:11.000000 mia-accounting-1.2.1/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.2.1/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.2.1/docs/source/history.rst
--rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.2.1/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     3969 2023-04-06 02:00:11.000000 mia-accounting-1.2.1/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.2.1/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-09 13:04:11.000000 mia-accounting-1.2.1/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-09 13:04:55.344353 mia-accounting-1.2.1/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.500369 mia-accounting-1.2.1/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.744364 mia-accounting-1.2.1/src/accounting/
--rw-r--r--   0 imacat    (1000) users      (100)     2981 2023-04-08 10:12:57.000000 mia-accounting-1.2.1/src/accounting/__init__.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.752364 mia-accounting-1.2.1/src/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1254 2023-04-04 09:21:36.000000 mia-accounting-1.2.1/src/accounting/account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     5589 2023-04-08 10:12:57.000000 mia-accounting-1.2.1/src/accounting/account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/src/accounting/account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.2.1/src/accounting/account/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/src/accounting/account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.2.1/src/accounting/account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.752364 mia-accounting-1.2.1/src/accounting/base_account/
--rw-r--r--   0 imacat    (1000) users      (100)     1296 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/src/accounting/base_account/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2018 2023-04-04 09:21:36.000000 mia-accounting-1.2.1/src/accounting/base_account/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/src/accounting/base_account/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.2.1/src/accounting/base_account/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.2.1/src/accounting/base_account/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.756364 mia-accounting-1.2.1/src/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1365 2023-04-04 09:21:36.000000 mia-accounting-1.2.1/src/accounting/currency/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3286 2023-04-04 09:21:34.000000 mia-accounting-1.2.1/src/accounting/currency/commands.py
--rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/src/accounting/currency/converters.py
--rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.2.1/src/accounting/currency/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.2.1/src/accounting/currency/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.2.1/src/accounting/currency/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.756364 mia-accounting-1.2.1/src/accounting/data/
--rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.2.1/src/accounting/data/base_accounts.csv
--rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.2.1/src/accounting/data/currencies.csv
--rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.2.1/src/accounting/forms.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.760364 mia-accounting-1.2.1/src/accounting/journal_entry/
--rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/src/accounting/journal_entry/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3345 2023-04-07 07:30:13.000000 mia-accounting-1.2.1/src/accounting/journal_entry/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.780363 mia-accounting-1.2.1/src/accounting/journal_entry/forms/
--rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.2.1/src/accounting/journal_entry/forms/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    11055 2023-04-08 10:12:54.000000 mia-accounting-1.2.1/src/accounting/journal_entry/forms/currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.2.1/src/accounting/journal_entry/forms/journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    19508 2023-04-07 16:44:13.000000 mia-accounting-1.2.1/src/accounting/journal_entry/forms/line_item.py
--rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/src/accounting/journal_entry/forms/reorder.py
--rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.2.1/src/accounting/journal_entry/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.780363 mia-accounting-1.2.1/src/accounting/journal_entry/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.2.1/src/accounting/journal_entry/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1729 2023-04-04 09:21:34.000000 mia-accounting-1.2.1/src/accounting/journal_entry/utils/account_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    12821 2023-04-04 09:21:31.000000 mia-accounting-1.2.1/src/accounting/journal_entry/utils/description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/src/accounting/journal_entry/utils/operators.py
--rw-r--r--   0 imacat    (1000) users      (100)     3787 2023-04-08 10:12:55.000000 mia-accounting-1.2.1/src/accounting/journal_entry/utils/original_line_items.py
--rw-r--r--   0 imacat    (1000) users      (100)     9472 2023-04-09 02:08:22.000000 mia-accounting-1.2.1/src/accounting/journal_entry/views.py
--rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.2.1/src/accounting/locale.py
--rw-r--r--   0 imacat    (1000) users      (100)    31691 2023-04-08 10:12:57.000000 mia-accounting-1.2.1/src/accounting/models.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.816363 mia-accounting-1.2.1/src/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/src/accounting/option/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.2.1/src/accounting/option/forms.py
--rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.2.1/src/accounting/option/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.864362 mia-accounting-1.2.1/src/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.2.1/src/accounting/report/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.2.1/src/accounting/report/converters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.868362 mia-accounting-1.2.1/src/accounting/report/period/
--rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.2.1/src/accounting/report/period/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.2.1/src/accounting/report/period/chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/src/accounting/report/period/description.py
--rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.2.1/src/accounting/report/period/month_end.py
--rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.2.1/src/accounting/report/period/parser.py
--rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.2.1/src/accounting/report/period/period.py
--rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.2.1/src/accounting/report/period/shortcuts.py
--rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.2.1/src/accounting/report/period/specification.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.880362 mia-accounting-1.2.1/src/accounting/report/reports/
--rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.2.1/src/accounting/report/reports/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.2.1/src/accounting/report/reports/balance_sheet.py
--rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.2.1/src/accounting/report/reports/income_expenses.py
--rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.2.1/src/accounting/report/reports/income_statement.py
--rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.2.1/src/accounting/report/reports/journal.py
--rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.2.1/src/accounting/report/reports/ledger.py
--rw-r--r--   0 imacat    (1000) users      (100)     8819 2023-04-09 13:02:35.000000 mia-accounting-1.2.1/src/accounting/report/reports/search.py
--rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.2.1/src/accounting/report/reports/trial_balance.py
--rw-r--r--   0 imacat    (1000) users      (100)     6975 2023-04-08 16:39:45.000000 mia-accounting-1.2.1/src/accounting/report/reports/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4555 2023-04-08 10:12:55.000000 mia-accounting-1.2.1/src/accounting/report/reports/unapplied_accounts.py
--rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.2.1/src/accounting/report/template_filters.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.008359 mia-accounting-1.2.1/src/accounting/report/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.2.1/src/accounting/report/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/src/accounting/report/utils/base_page_params.py
--rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.2.1/src/accounting/report/utils/base_report.py
--rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-09 04:04:18.000000 mia-accounting-1.2.1/src/accounting/report/utils/csv_export.py
--rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.2.1/src/accounting/report/utils/option_link.py
--rw-r--r--   0 imacat    (1000) users      (100)     6925 2023-04-08 10:12:55.000000 mia-accounting-1.2.1/src/accounting/report/utils/report_chooser.py
--rw-r--r--   0 imacat    (1000) users      (100)     1305 2023-04-08 03:26:33.000000 mia-accounting-1.2.1/src/accounting/report/utils/report_type.py
--rw-r--r--   0 imacat    (1000) users      (100)     2740 2023-04-08 10:12:55.000000 mia-accounting-1.2.1/src/accounting/report/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4477 2023-04-09 02:08:22.000000 mia-accounting-1.2.1/src/accounting/report/utils/urls.py
--rw-r--r--   0 imacat    (1000) users      (100)    10434 2023-04-09 02:08:22.000000 mia-accounting-1.2.1/src/accounting/report/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.500369 mia-accounting-1.2.1/src/accounting/static/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.008359 mia-accounting-1.2.1/src/accounting/static/css/
--rw-r--r--   0 imacat    (1000) users      (100)    13001 2023-04-08 16:39:45.000000 mia-accounting-1.2.1/src/accounting/static/css/style.css
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.016359 mia-accounting-1.2.1/src/accounting/static/js/
--rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.2.1/src/accounting/static/js/account-form.js
--rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.2.1/src/accounting/static/js/account-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.2.1/src/accounting/static/js/currency-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    38778 2023-04-04 10:05:35.000000 mia-accounting-1.2.1/src/accounting/static/js/description-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.2.1/src/accounting/static/js/drag-and-drop-reorder.js
--rw-r--r--   0 imacat    (1000) users      (100)     9092 2023-04-07 04:32:27.000000 mia-accounting-1.2.1/src/accounting/static/js/journal-entry-account-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    32504 2023-04-04 10:05:35.000000 mia-accounting-1.2.1/src/accounting/static/js/journal-entry-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    19866 2023-04-04 10:05:35.000000 mia-accounting-1.2.1/src/accounting/static/js/journal-entry-line-item-editor.js
--rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.2.1/src/accounting/static/js/journal-entry-order.js
--rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.2.1/src/accounting/static/js/material-fab-speed-dial.js
--rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.2.1/src/accounting/static/js/option-form.js
--rw-r--r--   0 imacat    (1000) users      (100)    11640 2023-04-04 10:05:35.000000 mia-accounting-1.2.1/src/accounting/static/js/original-line-item-selector.js
--rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.2.1/src/accounting/static/js/period-chooser.js
--rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.2.1/src/accounting/template_filters.py
--rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.2.1/src/accounting/template_globals.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.500369 mia-accounting-1.2.1/src/accounting/templates/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.016359 mia-accounting-1.2.1/src/accounting/templates/accounting/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.020359 mia-accounting-1.2.1/src/accounting/templates/accounting/account/
--rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/account/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/account/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.020359 mia-accounting-1.2.1/src/accounting/templates/accounting/account/include/
--rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/account/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/account/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.024359 mia-accounting-1.2.1/src/accounting/templates/accounting/base-account/
--rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/base-account/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/base-account/list.html
--rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/base.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.024359 mia-accounting-1.2.1/src/accounting/templates/accounting/currency/
--rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/currency/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/currency/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/currency/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.024359 mia-accounting-1.2.1/src/accounting/templates/accounting/currency/include/
--rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/currency/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/currency/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.028359 mia-accounting-1.2.1/src/accounting/templates/accounting/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3036 2023-04-08 16:39:45.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/include/nav.html
--rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/include/pagination.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.028359 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.052358 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/disbursement/
--rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/disbursement/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.052358 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/disbursement/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.084358 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/
--rw-r--r--   0 imacat    (1000) users      (100)     3373 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)    14459 2023-04-05 01:08:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3131 2023-04-07 06:56:44.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
--rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
--rw-r--r--   0 imacat    (1000) users      (100)     6161 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/form.html
--rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
--rw-r--r--   0 imacat    (1000) users      (100)     3490 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/order.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.084358 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/receipt/
--rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/receipt/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/receipt/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/receipt/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.088358 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/receipt/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.088358 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/transfer/
--rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/transfer/create.html
--rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/transfer/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/transfer/edit.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.092358 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/transfer/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
--rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.092358 mia-accounting-1.2.1/src/accounting/templates/accounting/option/
--rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/option/detail.html
--rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/option/form.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.092358 mia-accounting-1.2.1/src/accounting/templates/accounting/option/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
--rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/option/include/form-recurring-item.html
--rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.100358 mia-accounting-1.2.1/src/accounting/templates/accounting/report/
--rw-r--r--   0 imacat    (1000) users      (100)     5065 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/balance-sheet.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.108358 mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/
--rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
--rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/balance-sheet-section.html
--rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
--rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
--rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/period-chooser.html
--rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/search-modal.html
--rw-r--r--   0 imacat    (1000) users      (100)     5572 2023-04-04 23:56:52.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/toolbar-buttons.html
--rw-r--r--   0 imacat    (1000) users      (100)     4623 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/income-expenses.html
--rw-r--r--   0 imacat    (1000) users      (100)     4242 2023-04-04 10:04:12.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/income-statement.html
--rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/journal.html
--rw-r--r--   0 imacat    (1000) users      (100)     4745 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/ledger.html
--rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/search.html
--rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-04 10:04:10.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/trial-balance.html
--rw-r--r--   0 imacat    (1000) users      (100)     2201 2023-04-08 10:12:55.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/unapplied-accounts.html
--rw-r--r--   0 imacat    (1000) users      (100)     4086 2023-04-08 16:39:45.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/report/unapplied.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.108358 mia-accounting-1.2.1/src/accounting/templates/accounting/unmatched-offset/
--rw-r--r--   0 imacat    (1000) users      (100)     1212 2023-04-08 16:38:54.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/unmatched-offset/dashboard.html
--rw-r--r--   0 imacat    (1000) users      (100)     4668 2023-04-08 10:12:57.000000 mia-accounting-1.2.1/src/accounting/templates/accounting/unmatched-offset/list.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.108358 mia-accounting-1.2.1/src/accounting/translations/
--rw-r--r--   0 imacat    (1000) users      (100)    47460 2023-04-08 17:41:05.000000 mia-accounting-1.2.1/src/accounting/translations/accounting.pot
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.2.1/src/accounting/translations/babel.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.500369 mia-accounting-1.2.1/src/accounting/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.132357 mia-accounting-1.2.1/src/accounting/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.2.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.2.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.500369 mia-accounting-1.2.1/src/accounting/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.132357 mia-accounting-1.2.1/src/accounting/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.2.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
--rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.2.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.172356 mia-accounting-1.2.1/src/accounting/unmatched_offset/
--rw-r--r--   0 imacat    (1000) users      (100)     1032 2023-04-08 10:12:57.000000 mia-accounting-1.2.1/src/accounting/unmatched_offset/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-08 10:12:57.000000 mia-accounting-1.2.1/src/accounting/unmatched_offset/queries.py
--rw-r--r--   0 imacat    (1000) users      (100)     3178 2023-04-08 16:39:45.000000 mia-accounting-1.2.1/src/accounting/unmatched_offset/views.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.240355 mia-accounting-1.2.1/src/accounting/utils/
--rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.2.1/src/accounting/utils/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/src/accounting/utils/cast.py
--rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.2.1/src/accounting/utils/current_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/src/accounting/utils/flash_errors.py
--rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.2.1/src/accounting/utils/journal_entry_types.py
--rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/src/accounting/utils/next_uri.py
--rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.2.1/src/accounting/utils/offset_alias.py
--rw-r--r--   0 imacat    (1000) users      (100)     5198 2023-04-08 16:39:45.000000 mia-accounting-1.2.1/src/accounting/utils/offset_matcher.py
--rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.2.1/src/accounting/utils/options.py
--rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.2.1/src/accounting/utils/pagination.py
--rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.2.1/src/accounting/utils/permission.py
--rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.2.1/src/accounting/utils/query.py
--rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.2.1/src/accounting/utils/random_id.py
--rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.2.1/src/accounting/utils/strip_text.py
--rw-r--r--   0 imacat    (1000) users      (100)     3080 2023-04-08 10:12:56.000000 mia-accounting-1.2.1/src/accounting/utils/unapplied.py
--rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.2.1/src/accounting/utils/user.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.240355 mia-accounting-1.2.1/src/mia_accounting.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     7024 2023-04-09 13:04:54.000000 mia-accounting-1.2.1/src/mia_accounting.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)    11342 2023-04-09 13:04:54.000000 mia-accounting-1.2.1/src/mia_accounting.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-09 13:04:54.000000 mia-accounting-1.2.1/src/mia_accounting.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-09 13:04:54.000000 mia-accounting-1.2.1/src/mia_accounting.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-09 13:04:54.000000 mia-accounting-1.2.1/src/mia_accounting.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.260355 mia-accounting-1.2.1/tests/
--rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-04 09:21:35.000000 mia-accounting-1.2.1/tests/babel-utils-test-site.py
--rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-04 09:21:32.000000 mia-accounting-1.2.1/tests/babel-utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    35900 2023-04-09 03:46:55.000000 mia-accounting-1.2.1/tests/test_account.py
--rw-r--r--   0 imacat    (1000) users      (100)     5034 2023-04-04 09:21:36.000000 mia-accounting-1.2.1/tests/test_base_account.py
--rw-r--r--   0 imacat    (1000) users      (100)    27047 2023-04-09 03:46:55.000000 mia-accounting-1.2.1/tests/test_currency.py
--rw-r--r--   0 imacat    (1000) users      (100)    16820 2023-04-09 03:46:55.000000 mia-accounting-1.2.1/tests/test_description_editor.py
--rw-r--r--   0 imacat    (1000) users      (100)   106505 2023-04-09 03:46:55.000000 mia-accounting-1.2.1/tests/test_journal_entry.py
--rw-r--r--   0 imacat    (1000) users      (100)    39089 2023-04-09 03:46:55.000000 mia-accounting-1.2.1/tests/test_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    16738 2023-04-09 02:42:18.000000 mia-accounting-1.2.1/tests/test_option.py
--rw-r--r--   0 imacat    (1000) users      (100)    16219 2023-04-09 04:09:27.000000 mia-accounting-1.2.1/tests/test_report.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.260355 mia-accounting-1.2.1/tests/test_site/
--rw-r--r--   0 imacat    (1000) users      (100)     4143 2023-04-04 23:16:14.000000 mia-accounting-1.2.1/tests/test_site/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     2861 2023-04-04 09:28:44.000000 mia-accounting-1.2.1/tests/test_site/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.2.1/tests/test_site/locale.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.260355 mia-accounting-1.2.1/tests/test_site/static/
--rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.2.1/tests/test_site/static/favicon.svg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.284354 mia-accounting-1.2.1/tests/test_site/templates/
--rw-r--r--   0 imacat    (1000) users      (100)     6015 2023-04-05 18:00:22.000000 mia-accounting-1.2.1/tests/test_site/templates/base.html
--rw-r--r--   0 imacat    (1000) users      (100)      812 2023-04-04 10:04:53.000000 mia-accounting-1.2.1/tests/test_site/templates/home.html
--rw-r--r--   0 imacat    (1000) users      (100)     1419 2023-04-04 10:04:53.000000 mia-accounting-1.2.1/tests/test_site/templates/login.html
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.316354 mia-accounting-1.2.1/tests/test_site/translations/
--rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.2.1/tests/test_site/translations/babel.cfg
--rw-r--r--   0 imacat    (1000) users      (100)     1307 2023-04-05 18:34:06.000000 mia-accounting-1.2.1/tests/test_site/translations/messages.pot
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.500369 mia-accounting-1.2.1/tests/test_site/translations/zh_Hans/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.316354 mia-accounting-1.2.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)      797 2023-04-05 18:34:39.000000 mia-accounting-1.2.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     1540 2023-04-05 18:34:39.000000 mia-accounting-1.2.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:54.500369 mia-accounting-1.2.1/tests/test_site/translations/zh_Hant/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-09 13:04:55.316354 mia-accounting-1.2.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 imacat    (1000) users      (100)      797 2023-04-05 18:34:39.000000 mia-accounting-1.2.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 imacat    (1000) users      (100)     1540 2023-04-05 18:55:17.000000 mia-accounting-1.2.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
--rw-r--r--   0 imacat    (1000) users      (100)    29050 2023-04-09 03:46:55.000000 mia-accounting-1.2.1/tests/test_unmatched_offset.py
--rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.2.1/tests/test_utils.py
--rw-r--r--   0 imacat    (1000) users      (100)    14493 2023-04-09 03:46:55.000000 mia-accounting-1.2.1/tests/testlib.py
--rw-r--r--   0 imacat    (1000) users      (100)    16670 2023-04-09 03:46:55.000000 mia-accounting-1.2.1/tests/testlib_journal_entry.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.513632 mia-accounting-1.3.0/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2015-02-17 18:06:12.000000 mia-accounting-1.3.0/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)     1070 2023-04-05 11:25:31.000000 mia-accounting-1.3.0/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     6757 2023-04-10 16:09:35.513632 mia-accounting-1.3.0/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     5958 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.341635 mia-accounting-1.3.0/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-01-27 04:20:04.000000 mia-accounting-1.3.0/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-01-27 04:20:04.000000 mia-accounting-1.3.0/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.341635 mia-accounting-1.3.0/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.341635 mia-accounting-1.3.0/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:08.000000 mia-accounting-1.3.0/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.341635 mia-accounting-1.3.0/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-01-27 04:21:11.000000 mia-accounting-1.3.0/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-10 16:05:21.000000 mia-accounting-1.3.0/docs/source/accounting.account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      959 2023-04-10 16:05:21.000000 mia-accounting-1.3.0/docs/source/accounting.base_account.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1053 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.currency.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1089 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.journal_entry.forms.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      937 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.journal_entry.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1162 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.journal_entry.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      513 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.option.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1551 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.report.period.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2043 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.report.reports.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      861 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.report.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1775 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.report.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1332 2023-04-10 16:05:21.000000 mia-accounting-1.3.0/docs/source/accounting.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      615 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.unmatched_offset.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2756 2023-04-10 16:05:22.000000 mia-accounting-1.3.0/docs/source/accounting.utils.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1022 2023-04-10 16:08:23.000000 mia-accounting-1.3.0/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1508 2023-04-06 00:38:39.000000 mia-accounting-1.3.0/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     2837 2023-04-06 00:21:32.000000 mia-accounting-1.3.0/docs/source/history.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      508 2023-04-06 00:11:04.000000 mia-accounting-1.3.0/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     3702 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       53 2023-04-04 10:25:53.000000 mia-accounting-1.3.0/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1820 2023-04-10 16:08:23.000000 mia-accounting-1.3.0/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-04-10 16:09:35.513632 mia-accounting-1.3.0/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.337635 mia-accounting-1.3.0/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.345635 mia-accounting-1.3.0/src/accounting/
+-rw-r--r--   0 imacat    (1000) users      (100)     3065 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/__init__.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.345635 mia-accounting-1.3.0/src/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3868 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1512 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7145 2023-04-04 09:21:33.000000 mia-accounting-1.3.0/src/accounting/account/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2209 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     7416 2023-04-09 02:08:22.000000 mia-accounting-1.3.0/src/accounting/account/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.345635 mia-accounting-1.3.0/src/accounting/base_account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1240 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/base_account/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1800 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/base_account/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1592 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/base_account/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1769 2023-04-04 09:21:37.000000 mia-accounting-1.3.0/src/accounting/base_account/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1812 2023-04-09 02:08:22.000000 mia-accounting-1.3.0/src/accounting/base_account/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2138 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/commands.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.345635 mia-accounting-1.3.0/src/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1312 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/currency/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2212 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/src/accounting/currency/commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1556 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/currency/converters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3172 2023-04-04 09:21:36.000000 mia-accounting-1.3.0/src/accounting/currency/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1720 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/currency/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6609 2023-04-09 02:08:22.000000 mia-accounting-1.3.0/src/accounting/currency/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.345635 mia-accounting-1.3.0/src/accounting/data/
+-rw-r--r--   0 imacat    (1000) users      (100)    36368 2023-03-14 01:04:26.000000 mia-accounting-1.3.0/src/accounting/data/base_accounts.csv
+-rw-r--r--   0 imacat    (1000) users      (100)      370 2023-03-14 01:04:26.000000 mia-accounting-1.3.0/src/accounting/data/currencies.csv
+-rw-r--r--   0 imacat    (1000) users      (100)     3144 2023-04-04 09:21:33.000000 mia-accounting-1.3.0/src/accounting/forms.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.345635 mia-accounting-1.3.0/src/accounting/journal_entry/
+-rw-r--r--   0 imacat    (1000) users      (100)     1376 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/journal_entry/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3345 2023-04-07 07:30:13.000000 mia-accounting-1.3.0/src/accounting/journal_entry/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.349635 mia-accounting-1.3.0/src/accounting/journal_entry/forms/
+-rw-r--r--   0 imacat    (1000) users      (100)      934 2023-04-04 09:21:37.000000 mia-accounting-1.3.0/src/accounting/journal_entry/forms/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11055 2023-04-08 10:12:54.000000 mia-accounting-1.3.0/src/accounting/journal_entry/forms/currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    24553 2023-04-04 09:21:37.000000 mia-accounting-1.3.0/src/accounting/journal_entry/forms/journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    19508 2023-04-07 16:44:13.000000 mia-accounting-1.3.0/src/accounting/journal_entry/forms/line_item.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3408 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/journal_entry/forms/reorder.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2535 2023-04-04 09:21:32.000000 mia-accounting-1.3.0/src/accounting/journal_entry/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.349635 mia-accounting-1.3.0/src/accounting/journal_entry/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      729 2023-04-04 09:21:32.000000 mia-accounting-1.3.0/src/accounting/journal_entry/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1729 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/journal_entry/utils/account_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12821 2023-04-04 09:21:31.000000 mia-accounting-1.3.0/src/accounting/journal_entry/utils/description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)    12679 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/journal_entry/utils/operators.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3787 2023-04-08 10:12:55.000000 mia-accounting-1.3.0/src/accounting/journal_entry/utils/original_line_items.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9472 2023-04-09 02:08:22.000000 mia-accounting-1.3.0/src/accounting/journal_entry/views.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3809 2023-04-04 09:21:33.000000 mia-accounting-1.3.0/src/accounting/locale.py
+-rw-r--r--   0 imacat    (1000) users      (100)    31691 2023-04-08 10:12:57.000000 mia-accounting-1.3.0/src/accounting/models.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.349635 mia-accounting-1.3.0/src/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)      993 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/option/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     9762 2023-04-08 00:27:23.000000 mia-accounting-1.3.0/src/accounting/option/forms.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2827 2023-04-04 09:21:32.000000 mia-accounting-1.3.0/src/accounting/option/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.349635 mia-accounting-1.3.0/src/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     1362 2023-04-08 10:12:56.000000 mia-accounting-1.3.0/src/accounting/report/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-08 10:12:56.000000 mia-accounting-1.3.0/src/accounting/report/converters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.349635 mia-accounting-1.3.0/src/accounting/report/period/
+-rw-r--r--   0 imacat    (1000) users      (100)      793 2023-04-04 09:21:32.000000 mia-accounting-1.3.0/src/accounting/report/period/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3677 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/report/period/chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5530 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/report/period/description.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1045 2023-04-04 09:21:36.000000 mia-accounting-1.3.0/src/accounting/report/period/month_end.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4063 2023-04-04 09:21:31.000000 mia-accounting-1.3.0/src/accounting/report/period/parser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4513 2023-04-04 09:21:32.000000 mia-accounting-1.3.0/src/accounting/report/period/period.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4707 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/report/period/shortcuts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3894 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/report/period/specification.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.353635 mia-accounting-1.3.0/src/accounting/report/reports/
+-rw-r--r--   0 imacat    (1000) users      (100)      946 2023-04-04 09:21:36.000000 mia-accounting-1.3.0/src/accounting/report/reports/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17920 2023-04-06 01:50:58.000000 mia-accounting-1.3.0/src/accounting/report/reports/balance_sheet.py
+-rw-r--r--   0 imacat    (1000) users      (100)    18935 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/report/reports/income_expenses.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11733 2023-04-06 01:50:58.000000 mia-accounting-1.3.0/src/accounting/report/reports/income_statement.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8128 2023-04-07 22:59:57.000000 mia-accounting-1.3.0/src/accounting/report/reports/journal.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16685 2023-04-04 09:21:31.000000 mia-accounting-1.3.0/src/accounting/report/reports/ledger.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8819 2023-04-09 13:02:35.000000 mia-accounting-1.3.0/src/accounting/report/reports/search.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8853 2023-04-06 01:50:58.000000 mia-accounting-1.3.0/src/accounting/report/reports/trial_balance.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6975 2023-04-08 16:39:45.000000 mia-accounting-1.3.0/src/accounting/report/reports/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4555 2023-04-08 10:12:55.000000 mia-accounting-1.3.0/src/accounting/report/reports/unapplied_accounts.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1205 2023-04-04 09:21:33.000000 mia-accounting-1.3.0/src/accounting/report/template_filters.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.353635 mia-accounting-1.3.0/src/accounting/report/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      711 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/report/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2996 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/report/utils/base_page_params.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1143 2023-04-04 09:21:36.000000 mia-accounting-1.3.0/src/accounting/report/utils/base_report.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-09 04:04:18.000000 mia-accounting-1.3.0/src/accounting/report/utils/csv_export.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1368 2023-04-04 09:21:37.000000 mia-accounting-1.3.0/src/accounting/report/utils/option_link.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6925 2023-04-08 10:12:55.000000 mia-accounting-1.3.0/src/accounting/report/utils/report_chooser.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1305 2023-04-08 03:26:33.000000 mia-accounting-1.3.0/src/accounting/report/utils/report_type.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2740 2023-04-08 10:12:55.000000 mia-accounting-1.3.0/src/accounting/report/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4477 2023-04-09 02:08:22.000000 mia-accounting-1.3.0/src/accounting/report/utils/urls.py
+-rw-r--r--   0 imacat    (1000) users      (100)    10434 2023-04-09 02:08:22.000000 mia-accounting-1.3.0/src/accounting/report/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.337635 mia-accounting-1.3.0/src/accounting/static/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.353635 mia-accounting-1.3.0/src/accounting/static/css/
+-rw-r--r--   0 imacat    (1000) users      (100)    13001 2023-04-08 16:39:45.000000 mia-accounting-1.3.0/src/accounting/static/css/style.css
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.353635 mia-accounting-1.3.0/src/accounting/static/js/
+-rw-r--r--   0 imacat    (1000) users      (100)    10921 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/account-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1599 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/account-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     4955 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/currency-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    38778 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/description-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     3564 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/drag-and-drop-reorder.js
+-rw-r--r--   0 imacat    (1000) users      (100)     9092 2023-04-07 04:32:27.000000 mia-accounting-1.3.0/src/accounting/static/js/journal-entry-account-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    32504 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/journal-entry-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    19866 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/journal-entry-line-item-editor.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1366 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/journal-entry-order.js
+-rw-r--r--   0 imacat    (1000) users      (100)     1436 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/material-fab-speed-dial.js
+-rw-r--r--   0 imacat    (1000) users      (100)    28660 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/option-form.js
+-rw-r--r--   0 imacat    (1000) users      (100)    11640 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/original-line-item-selector.js
+-rw-r--r--   0 imacat    (1000) users      (100)    10374 2023-04-04 10:05:35.000000 mia-accounting-1.3.0/src/accounting/static/js/period-chooser.js
+-rw-r--r--   0 imacat    (1000) users      (100)     2708 2023-04-04 09:21:31.000000 mia-accounting-1.3.0/src/accounting/template_filters.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1126 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/template_globals.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.337635 mia-accounting-1.3.0/src/accounting/templates/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1034 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/account/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4266 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1081 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/account/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/account/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     5704 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/account/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3052 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/account/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/base-account/
+-rw-r--r--   0 imacat    (1000) users      (100)     1581 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/base-account/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/base-account/list.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1035 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/base.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/currency/
+-rw-r--r--   0 imacat    (1000) users      (100)     1039 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/currency/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3883 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/currency/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1152 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/currency/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/currency/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     2850 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/currency/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2576 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/currency/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3036 2023-04-08 16:39:45.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/include/nav.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1986 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/include/pagination.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/
+-rw-r--r--   0 imacat    (1000) users      (100)     1149 2023-04-04 23:56:52.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2028 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1213 2023-04-04 10:04:09.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.357635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1195 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2283 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.361635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     3373 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)    14459 2023-04-05 01:08:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3131 2023-04-07 06:56:44.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4568 2023-04-04 23:56:52.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2726 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2704 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html
+-rw-r--r--   0 imacat    (1000) users      (100)     6161 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4370 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4162 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2093 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3490 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3083 2023-04-04 23:56:52.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/order.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.361635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/
+-rw-r--r--   0 imacat    (1000) users      (100)     1134 2023-04-04 23:56:52.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2025 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1203 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.361635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1194 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2278 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.361635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/
+-rw-r--r--   0 imacat    (1000) users      (100)     1127 2023-04-04 23:56:52.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/create.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2691 2023-04-04 10:04:09.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1200 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.361635 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1649 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2845 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.361635 mia-accounting-1.3.0/src/accounting/templates/accounting/option/
+-rw-r--r--   0 imacat    (1000) users      (100)     2765 2023-04-08 10:12:54.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/option/detail.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4699 2023-04-08 00:27:23.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/option/form.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.361635 mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1851 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3214 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/form-recurring-item.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3301 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4276 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.365635 mia-accounting-1.3.0/src/accounting/templates/accounting/report/
+-rw-r--r--   0 imacat    (1000) users      (100)     5065 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/balance-sheet.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.365635 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/
+-rw-r--r--   0 imacat    (1000) users      (100)     1970 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1708 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1281 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1760 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1252 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1429 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html
+-rw-r--r--   0 imacat    (1000) users      (100)     8857 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/period-chooser.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1933 2023-04-04 23:56:52.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/search-modal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     5572 2023-04-04 23:56:52.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4623 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/income-expenses.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4242 2023-04-04 10:04:12.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/income-statement.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4202 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/journal.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4745 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/ledger.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4044 2023-04-04 10:04:11.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/search.html
+-rw-r--r--   0 imacat    (1000) users      (100)     3340 2023-04-04 10:04:10.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/trial-balance.html
+-rw-r--r--   0 imacat    (1000) users      (100)     2201 2023-04-08 10:12:55.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/unapplied-accounts.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4086 2023-04-08 16:39:45.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/report/unapplied.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.365635 mia-accounting-1.3.0/src/accounting/templates/accounting/unmatched-offset/
+-rw-r--r--   0 imacat    (1000) users      (100)     1212 2023-04-08 16:38:54.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/unmatched-offset/dashboard.html
+-rw-r--r--   0 imacat    (1000) users      (100)     4668 2023-04-08 10:12:57.000000 mia-accounting-1.3.0/src/accounting/templates/accounting/unmatched-offset/list.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.365635 mia-accounting-1.3.0/src/accounting/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)    47460 2023-04-08 17:41:05.000000 mia-accounting-1.3.0/src/accounting/translations/accounting.pot
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-01-27 03:33:36.000000 mia-accounting-1.3.0/src/accounting/translations/babel.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.337635 mia-accounting-1.3.0/src/accounting/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.365635 mia-accounting-1.3.0/src/accounting/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.337635 mia-accounting-1.3.0/src/accounting/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.365635 mia-accounting-1.3.0/src/accounting/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)    15686 2023-04-08 17:41:07.000000 mia-accounting-1.3.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo
+-rw-r--r--   0 imacat    (1000) users      (100)    52088 2023-04-08 17:41:07.000000 mia-accounting-1.3.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.365635 mia-accounting-1.3.0/src/accounting/unmatched_offset/
+-rw-r--r--   0 imacat    (1000) users      (100)     1032 2023-04-08 10:12:57.000000 mia-accounting-1.3.0/src/accounting/unmatched_offset/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2065 2023-04-08 10:12:57.000000 mia-accounting-1.3.0/src/accounting/unmatched_offset/queries.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3178 2023-04-08 16:39:45.000000 mia-accounting-1.3.0/src/accounting/unmatched_offset/views.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.369635 mia-accounting-1.3.0/src/accounting/utils/
+-rw-r--r--   0 imacat    (1000) users      (100)      778 2023-04-04 09:21:31.000000 mia-accounting-1.3.0/src/accounting/utils/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1385 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/utils/cast.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3361 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/utils/current_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1424 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/utils/flash_errors.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1030 2023-04-04 09:21:32.000000 mia-accounting-1.3.0/src/accounting/utils/journal_entry_types.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2863 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/src/accounting/utils/next_uri.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1198 2023-04-08 10:12:55.000000 mia-accounting-1.3.0/src/accounting/utils/offset_alias.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5198 2023-04-08 16:39:45.000000 mia-accounting-1.3.0/src/accounting/utils/offset_matcher.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6906 2023-04-08 10:12:55.000000 mia-accounting-1.3.0/src/accounting/utils/options.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11734 2023-04-04 09:21:36.000000 mia-accounting-1.3.0/src/accounting/utils/pagination.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4260 2023-04-04 09:21:37.000000 mia-accounting-1.3.0/src/accounting/utils/permission.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1638 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/utils/query.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1174 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/utils/random_id.py
+-rw-r--r--   0 imacat    (1000) users      (100)     1396 2023-04-04 09:21:37.000000 mia-accounting-1.3.0/src/accounting/utils/strip_text.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3080 2023-04-08 10:12:56.000000 mia-accounting-1.3.0/src/accounting/utils/unapplied.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4970 2023-04-04 09:21:34.000000 mia-accounting-1.3.0/src/accounting/utils/user.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.369635 mia-accounting-1.3.0/src/mia_accounting.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     6757 2023-04-10 16:09:35.000000 mia-accounting-1.3.0/src/mia_accounting.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)    11392 2023-04-10 16:09:35.000000 mia-accounting-1.3.0/src/mia_accounting.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-04-10 16:09:35.000000 mia-accounting-1.3.0/src/mia_accounting.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       93 2023-04-10 16:09:35.000000 mia-accounting-1.3.0/src/mia_accounting.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       11 2023-04-10 16:09:35.000000 mia-accounting-1.3.0/src/mia_accounting.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.369635 mia-accounting-1.3.0/tests/
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4341 2023-04-04 09:21:35.000000 mia-accounting-1.3.0/tests/babel-utils-test-site.py
+-rwxr-xr-x   0 imacat    (1000) users      (100)     4297 2023-04-04 09:21:32.000000 mia-accounting-1.3.0/tests/babel-utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    32736 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2409 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_base_account.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6113 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_commands.py
+-rw-r--r--   0 imacat    (1000) users      (100)    23824 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_currency.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15999 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_description_editor.py
+-rw-r--r--   0 imacat    (1000) users      (100)   103461 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_journal_entry.py
+-rw-r--r--   0 imacat    (1000) users      (100)    38268 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15935 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_option.py
+-rw-r--r--   0 imacat    (1000) users      (100)    15398 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_report.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.373635 mia-accounting-1.3.0/tests/test_site/
+-rw-r--r--   0 imacat    (1000) users      (100)     4348 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_site/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     2861 2023-04-04 09:28:44.000000 mia-accounting-1.3.0/tests/test_site/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)     3414 2023-04-04 09:28:44.000000 mia-accounting-1.3.0/tests/test_site/locale.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.373635 mia-accounting-1.3.0/tests/test_site/static/
+-rw-r--r--   0 imacat    (1000) users      (100)     1420 2023-04-03 07:56:03.000000 mia-accounting-1.3.0/tests/test_site/static/favicon.svg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.373635 mia-accounting-1.3.0/tests/test_site/templates/
+-rw-r--r--   0 imacat    (1000) users      (100)     6015 2023-04-05 18:00:22.000000 mia-accounting-1.3.0/tests/test_site/templates/base.html
+-rw-r--r--   0 imacat    (1000) users      (100)      812 2023-04-04 10:04:53.000000 mia-accounting-1.3.0/tests/test_site/templates/home.html
+-rw-r--r--   0 imacat    (1000) users      (100)     1419 2023-04-04 10:04:53.000000 mia-accounting-1.3.0/tests/test_site/templates/login.html
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.373635 mia-accounting-1.3.0/tests/test_site/translations/
+-rw-r--r--   0 imacat    (1000) users      (100)       80 2023-02-03 05:00:02.000000 mia-accounting-1.3.0/tests/test_site/translations/babel.cfg
+-rw-r--r--   0 imacat    (1000) users      (100)     1307 2023-04-05 18:34:06.000000 mia-accounting-1.3.0/tests/test_site/translations/messages.pot
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.337635 mia-accounting-1.3.0/tests/test_site/translations/zh_Hans/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.445633 mia-accounting-1.3.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)      797 2023-04-05 18:34:39.000000 mia-accounting-1.3.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     1540 2023-04-05 18:34:39.000000 mia-accounting-1.3.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.337635 mia-accounting-1.3.0/tests/test_site/translations/zh_Hant/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-04-10 16:09:35.513632 mia-accounting-1.3.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 imacat    (1000) users      (100)      797 2023-04-05 18:34:39.000000 mia-accounting-1.3.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 imacat    (1000) users      (100)     1540 2023-04-05 18:55:17.000000 mia-accounting-1.3.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po
+-rw-r--r--   0 imacat    (1000) users      (100)    28229 2023-04-10 15:59:48.000000 mia-accounting-1.3.0/tests/test_unmatched_offset.py
+-rw-r--r--   0 imacat    (1000) users      (100)    13640 2023-04-04 09:21:31.000000 mia-accounting-1.3.0/tests/test_utils.py
+-rw-r--r--   0 imacat    (1000) users      (100)    14493 2023-04-09 03:46:55.000000 mia-accounting-1.3.0/tests/testlib.py
+-rw-r--r--   0 imacat    (1000) users      (100)    16670 2023-04-09 03:46:55.000000 mia-accounting-1.3.0/tests/testlib_journal_entry.py
```

### Comparing `mia-accounting-1.2.1/LICENSE` & `mia-accounting-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/MANIFEST.in` & `mia-accounting-1.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/PKG-INFO` & `mia-accounting-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-accounting
-Version: 1.2.1
+Version: 1.3.0
 Summary: A Flask accounting module.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://mia-accounting.readthedocs.io
 Project-URL: Repository, https://github.com/imacat/mia-accounting
 Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
 Project-URL: Demonstration, https://accounting.imacat.idv.tw
 Keywords: mia,accounting,flask
@@ -63,15 +63,16 @@
 start one, you may start with the test site.
 
 
 Prerequisites
 =============
 
 You need a running Flask application with database user login.
-The primary key of the user data model must be integer.
+The primary key of the user data model must be integer.  You also
+need at least one user.
 
 The following front-end JavaScript libraries must be loaded.  You may
 download it locally or use CDN_.
 
 * Bootstrap_ 5.2.3 or above
 * FontAwesome_ 6.2.1 or above
 * `Decimal.js`_ 6.4.3 or above
@@ -138,32 +139,21 @@
 
         return app
 
 
 Database Initialization
 =======================
 
-After the configuration, you need to run
-`flask_sqlalchemy.SQLAlchemy.create_all`_ to create the
-database tables that *Mia! Accounting* uses.
-
-*Mia! Accounting* adds three console commands:
-
-* ``accounting-init-base``
-* ``accounting-init-accounts``
-* ``accounting-init-currencies``
-
-After database tables are created, run
-``accounting-init-base`` first, and then the other two commands.
+After the configuration, run the ``accounting-init-db`` console
+command to initialize the accounting database.  You need to specify
+the username of a user as the data creator.
 
 ::
 
-    % flask --app myapp accounting-init-base
-    % flask --app myapp accounting-init-accounts
-    % flask --app myapp accounting-init-currencies
+    % flask --app myapp accounting-init-db -u username
 
 
 Navigation Menu
 ===============
 
 Include the navigation menu in the `Bootstrap navigation bar`_ in your
 base template:
```

### Comparing `mia-accounting-1.2.1/README.rst` & `mia-accounting-1.3.0/src/mia_accounting.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: mia-accounting
+Version: 1.3.0
+Summary: A Flask accounting module.
+Author-email: imacat <imacat@mail.imacat.idv.tw>
+Project-URL: Documentation, https://mia-accounting.readthedocs.io
+Project-URL: Repository, https://github.com/imacat/mia-accounting
+Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
+Project-URL: Demonstration, https://accounting.imacat.idv.tw
+Keywords: mia,accounting,flask
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Framework :: Flask
+Classifier: Topic :: Office/Business :: Financial :: Accounting
+Requires-Python: >=3.11
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+License-File: LICENSE
+
 ===============
 Mia! Accounting
 ===============
 
 
 Description
 ===========
@@ -43,15 +63,16 @@
 start one, you may start with the test site.
 
 
 Prerequisites
 =============
 
 You need a running Flask application with database user login.
-The primary key of the user data model must be integer.
+The primary key of the user data model must be integer.  You also
+need at least one user.
 
 The following front-end JavaScript libraries must be loaded.  You may
 download it locally or use CDN_.
 
 * Bootstrap_ 5.2.3 or above
 * FontAwesome_ 6.2.1 or above
 * `Decimal.js`_ 6.4.3 or above
@@ -118,32 +139,21 @@
 
         return app
 
 
 Database Initialization
 =======================
 
-After the configuration, you need to run
-`flask_sqlalchemy.SQLAlchemy.create_all`_ to create the
-database tables that *Mia! Accounting* uses.
-
-*Mia! Accounting* adds three console commands:
-
-* ``accounting-init-base``
-* ``accounting-init-accounts``
-* ``accounting-init-currencies``
-
-After database tables are created, run
-``accounting-init-base`` first, and then the other two commands.
+After the configuration, run the ``accounting-init-db`` console
+command to initialize the accounting database.  You need to specify
+the username of a user as the data creator.
 
 ::
 
-    % flask --app myapp accounting-init-base
-    % flask --app myapp accounting-init-accounts
-    % flask --app myapp accounting-init-currencies
+    % flask --app myapp accounting-init-db -u username
 
 
 Navigation Menu
 ===============
 
 Include the navigation menu in the `Bootstrap navigation bar`_ in your
 base template:
```

### Comparing `mia-accounting-1.2.1/docs/Makefile` & `mia-accounting-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/make.bat` & `mia-accounting-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/accounting.account.rst` & `mia-accounting-1.3.0/docs/source/accounting.account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/accounting.base_account.rst` & `mia-accounting-1.3.0/docs/source/accounting.base_account.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/accounting.currency.rst` & `mia-accounting-1.3.0/docs/source/accounting.currency.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/accounting.journal_entry.forms.rst` & `mia-accounting-1.3.0/docs/source/accounting.journal_entry.forms.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/accounting.journal_entry.rst` & `mia-accounting-1.3.0/docs/source/accounting.journal_entry.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/accounting.journal_entry.utils.rst` & `mia-accounting-1.3.0/docs/source/accounting.journal_entry.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/accounting.option.rst` & `mia-accounting-1.3.0/docs/source/accounting.option.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/accounting.report.period.rst` & `mia-accounting-1.3.0/docs/source/accounting.report.period.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/accounting.report.reports.rst` & `mia-accounting-1.3.0/docs/source/accounting.report.reports.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/accounting.report.rst` & `mia-accounting-1.3.0/docs/source/accounting.report.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/accounting.report.utils.rst` & `mia-accounting-1.3.0/docs/source/accounting.report.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/accounting.rst` & `mia-accounting-1.3.0/docs/source/accounting.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,22 @@
    accounting.report
    accounting.unmatched_offset
    accounting.utils
 
 Submodules
 ----------
 
+accounting.commands module
+--------------------------
+
+.. automodule:: accounting.commands
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 accounting.forms module
 -----------------------
 
 .. automodule:: accounting.forms
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `mia-accounting-1.2.1/docs/source/accounting.unmatched_offset.rst` & `mia-accounting-1.3.0/docs/source/accounting.unmatched_offset.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/accounting.utils.rst` & `mia-accounting-1.3.0/docs/source/accounting.utils.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/conf.py` & `mia-accounting-1.3.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Mia! Accounting'
 copyright = '2023, imacat'
 author = 'imacat'
-release = '1.2.1'
+release = '1.3.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc']
 
 templates_path = ['_templates']
```

### Comparing `mia-accounting-1.2.1/docs/source/examples.rst` & `mia-accounting-1.3.0/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/history.rst` & `mia-accounting-1.3.0/docs/source/history.rst`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/docs/source/intro.rst` & `mia-accounting-1.3.0/docs/source/intro.rst`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 start one, you may start with the test site.
 
 
 Prerequisites
 -------------
 
 You need a running Flask application with database user login.
-The primary key of the user data model must be integer.
+The primary key of the user data model must be integer.  You also
+need at least one user.
 
 The following front-end JavaScript libraries must be loaded.  You may
 download it locally or use CDN_.
 
 * Bootstrap_ 5.2.3 or above
 * FontAwesome_ 6.2.1 or above
 * `Decimal.js`_ 6.4.3 or above
@@ -63,32 +64,21 @@
 
 See an example in :ref:`example-userutils`.
 
 
 Database Initialization
 -----------------------
 
-After the configuration, you need to run
-`flask_sqlalchemy.SQLAlchemy.create_all`_ to create the
-database tables that *Mia! Accounting* uses.
-
-*Mia! Accounting* adds three console commands:
-
-* ``accounting-init-base``
-* ``accounting-init-accounts``
-* ``accounting-init-currencies``
-
-After database tables are created, run
-``accounting-init-base`` first, and then the other two commands.
+After the configuration, run the ``accounting-init-db`` console
+command to initialize the accounting database.  You need to specify
+the username of a user as the data creator.
 
 ::
 
-    % flask --app myapp accounting-init-base
-    % flask --app myapp accounting-init-accounts
-    % flask --app myapp accounting-init-currencies
+    % flask --app myapp accounting-init-db -u username
 
 
 Navigation Menu
 ---------------
 
 Include the navigation menu in the `Bootstrap navigation bar`_ in your
 base template:
```

### Comparing `mia-accounting-1.2.1/pyproject.toml` & `mia-accounting-1.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 [project]
 name = "mia-accounting"
-version = "1.2.1"
+version = "1.3.0"
 description = "A Flask accounting module."
 readme = "README.rst"
 requires-python = ">=3.11"
 authors = [
     {name = "imacat", email = "imacat@mail.imacat.idv.tw"},
 ]
 keywords = ["mia", "accounting", "flask"]
```

### Comparing `mia-accounting-1.2.1/src/accounting/__init__.py` & `mia-accounting-1.3.0/src/accounting/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,17 @@
 
     from .template_globals import currency_options, default_currency_code
     bp.add_app_template_global(currency_options,
                                "accounting_currency_options")
     bp.add_app_template_global(default_currency_code,
                                "accounting_default_currency_code")
 
+    from .commands import init_db_command
+    app.cli.add_command(init_db_command)
+
     from . import locale
     locale.init_app(app, bp)
 
     from .utils import permission
     permission.init_app(bp, user_utils)
 
     from .utils import next_uri
```

### Comparing `mia-accounting-1.2.1/src/accounting/account/__init__.py` & `mia-accounting-1.3.0/src/accounting/base_account/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # The Mia! Accounting Project.
-# Author: imacat@mail.imacat.idv.tw (imacat), 2023/1/30
+# Author: imacat@mail.imacat.idv.tw (imacat), 2023/1/25
 
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
-"""The account management.
+"""The base account management.
 
 """
 from flask import Flask, Blueprint
 
+from .commands import init_base_accounts_command
+
 
 def init_app(app: Flask, bp: Blueprint) -> None:
     """Initialize the application.
 
     :param app: The Flask application.
     :param bp: The blueprint of the accounting application.
     :return: None.
     """
-    from .converters import AccountConverter
-    app.url_map.converters["account"] = AccountConverter
-
-    from .views import bp as account_bp
-    bp.register_blueprint(account_bp, url_prefix="/accounts")
+    from .converters import BaseAccountConverter
+    app.url_map.converters["baseAccount"] = BaseAccountConverter
 
-    from .commands import init_accounts_command
-    app.cli.add_command(init_accounts_command)
+    from .views import bp as base_account_bp
+    bp.register_blueprint(base_account_bp, url_prefix="/base-accounts")
```

### Comparing `mia-accounting-1.2.1/src/accounting/account/converters.py` & `mia-accounting-1.3.0/src/accounting/account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/account/forms.py` & `mia-accounting-1.3.0/src/accounting/account/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/account/queries.py` & `mia-accounting-1.3.0/src/accounting/account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/account/views.py` & `mia-accounting-1.3.0/src/accounting/account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/base_account/__init__.py` & `mia-accounting-1.3.0/src/accounting/account/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # The Mia! Accounting Project.
-# Author: imacat@mail.imacat.idv.tw (imacat), 2023/1/25
+# Author: imacat@mail.imacat.idv.tw (imacat), 2023/1/30
 
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
-"""The base account management.
+"""The account management.
 
 """
 from flask import Flask, Blueprint
 
+from .commands import init_accounts_command
+
 
 def init_app(app: Flask, bp: Blueprint) -> None:
     """Initialize the application.
 
     :param app: The Flask application.
     :param bp: The blueprint of the accounting application.
     :return: None.
     """
-    from .converters import BaseAccountConverter
-    app.url_map.converters["baseAccount"] = BaseAccountConverter
-
-    from .views import bp as base_account_bp
-    bp.register_blueprint(base_account_bp, url_prefix="/base-accounts")
+    from .converters import AccountConverter
+    app.url_map.converters["account"] = AccountConverter
 
-    from .commands import init_base_accounts_command
-    app.cli.add_command(init_base_accounts_command)
+    from .views import bp as account_bp
+    bp.register_blueprint(account_bp, url_prefix="/accounts")
```

### Comparing `mia-accounting-1.2.1/src/accounting/base_account/commands.py` & `mia-accounting-1.3.0/src/accounting/base_account/commands.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,37 +15,31 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The console commands for the base account management.
 
 """
 import csv
 
-import click
-from flask.cli import with_appcontext
+import sqlalchemy as sa
 
 from accounting import data_dir
 from accounting import db
 from accounting.models import BaseAccount, BaseAccountL10n
 
 
-@click.command("accounting-init-base")
-@with_appcontext
 def init_base_accounts_command() -> None:
     """Initializes the base accounts."""
     if BaseAccount.query.first() is not None:
-        click.echo("Base accounts already exist.")
-        raise click.Abort
+        return
 
     with open(data_dir / "base_accounts.csv") as fp:
         data: list[dict[str, str]] = [x for x in csv.DictReader(fp)]
     account_data: list[dict[str, str]] = [{"code": x["code"],
                                            "title_l10n": x["title"]}
                                           for x in data]
     locales: list[str] = [x[5:] for x in data[0] if x.startswith("l10n-")]
     l10n_data: list[dict[str, str]] = [{"account_code": x["code"],
                                         "locale": y,
                                         "title": x[f"l10n-{y}"]}
                                        for x in data for y in locales]
-    db.session.bulk_insert_mappings(BaseAccount, account_data)
-    db.session.bulk_insert_mappings(BaseAccountL10n, l10n_data)
-    db.session.commit()
-    click.echo("Base accounts initialized.")
+    db.session.execute(sa.insert(BaseAccount), account_data)
+    db.session.execute(sa.insert(BaseAccountL10n), l10n_data)
```

### Comparing `mia-accounting-1.2.1/src/accounting/base_account/converters.py` & `mia-accounting-1.3.0/src/accounting/base_account/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/base_account/queries.py` & `mia-accounting-1.3.0/src/accounting/base_account/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/base_account/views.py` & `mia-accounting-1.3.0/src/accounting/base_account/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/currency/__init__.py` & `mia-accounting-1.3.0/src/accounting/currency/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,24 +15,23 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The currency management.
 
 """
 from flask import Flask, Blueprint
 
+from .commands import init_currencies_command
+
 
 def init_app(app: Flask, bp: Blueprint) -> None:
     """Initialize the application.
 
     :param app: The Flask application.
     :param bp: The blueprint of the accounting application.
     :return: None.
     """
     from .converters import CurrencyConverter
     app.url_map.converters["currency"] = CurrencyConverter
 
     from .views import bp as currency_bp, api_bp as currency_api_bp
     bp.register_blueprint(currency_bp, url_prefix="/currencies")
     bp.register_blueprint(currency_api_bp, url_prefix="/api/currencies")
-
-    from .commands import init_currencies_command
-    app.cli.add_command(init_currencies_command)
```

### Comparing `mia-accounting-1.2.1/src/accounting/currency/commands.py` & `mia-accounting-1.3.0/src/accounting/currency/commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,71 +14,40 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The console commands for the currency management.
 
 """
 import csv
-import os
 import typing as t
 
-import click
-from flask.cli import with_appcontext
+import sqlalchemy as sa
 
 from accounting import db, data_dir
 from accounting.models import Currency, CurrencyL10n
-from accounting.utils.user import has_user, get_user_pk
+from accounting.utils.user import get_user_pk
 
-CurrencyData = tuple[str, str, str, str]
 
-
-def __validate_username(ctx: click.core.Context, param: click.core.Option,
-                        value: str) -> str:
-    """Validates the username for the click console command.
-
-    :param ctx: The console command context.
-    :param param: The console command option.
-    :param value: The username.
-    :raise click.BadParameter: When validation fails.
-    :return: The username.
-    """
-    value = value.strip()
-    if value == "":
-        raise click.BadParameter("Username empty.")
-    if not has_user(value):
-        raise click.BadParameter(f"User {value} does not exist.")
-    return value
-
-
-@click.command("accounting-init-currencies")
-@click.option("-u", "--username", metavar="USERNAME", prompt=True,
-              help="The username.", callback=__validate_username,
-              default=lambda: os.getlogin())
-@with_appcontext
 def init_currencies_command(username: str) -> None:
     """Initializes the currencies."""
     existing_codes: set[str] = {x.code for x in Currency.query.all()}
 
     with open(data_dir / "currencies.csv") as fp:
         data: list[dict[str, str]] = [x for x in csv.DictReader(fp)]
     to_add: list[dict[str, str]] = [x for x in data
                                     if x["code"] not in existing_codes]
     if len(to_add) == 0:
-        click.echo("No more currency to add.")
         return
 
     creator_pk: int = get_user_pk(username)
     currency_data: list[dict[str, t.Any]] = [{"code": x["code"],
                                               "name_l10n": x["name"],
                                               "created_by_id": creator_pk,
                                               "updated_by_id": creator_pk}
                                              for x in to_add]
     locales: list[str] = [x[5:] for x in to_add[0] if x.startswith("l10n-")]
     l10n_data: list[dict[str, str]] = [{"currency_code": x["code"],
                                         "locale": y,
                                         "name": x[f"l10n-{y}"]}
                                        for x in to_add for y in locales]
-    db.session.bulk_insert_mappings(Currency, currency_data)
-    db.session.bulk_insert_mappings(CurrencyL10n, l10n_data)
-    db.session.commit()
-
-    click.echo(F"{len(to_add)} added.  Currencies initialized.")
+    db.session.execute(sa.insert(Currency), currency_data)
+    db.session.execute(sa.insert(CurrencyL10n), l10n_data)
```

### Comparing `mia-accounting-1.2.1/src/accounting/currency/converters.py` & `mia-accounting-1.3.0/src/accounting/currency/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/currency/forms.py` & `mia-accounting-1.3.0/src/accounting/currency/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/currency/queries.py` & `mia-accounting-1.3.0/src/accounting/currency/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/currency/views.py` & `mia-accounting-1.3.0/src/accounting/currency/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/data/base_accounts.csv` & `mia-accounting-1.3.0/src/accounting/data/base_accounts.csv`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/forms.py` & `mia-accounting-1.3.0/src/accounting/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/journal_entry/__init__.py` & `mia-accounting-1.3.0/src/accounting/journal_entry/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/journal_entry/converters.py` & `mia-accounting-1.3.0/src/accounting/journal_entry/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/journal_entry/forms/__init__.py` & `mia-accounting-1.3.0/src/accounting/journal_entry/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/journal_entry/forms/currency.py` & `mia-accounting-1.3.0/src/accounting/journal_entry/forms/currency.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/journal_entry/forms/journal_entry.py` & `mia-accounting-1.3.0/src/accounting/journal_entry/forms/journal_entry.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/journal_entry/forms/line_item.py` & `mia-accounting-1.3.0/src/accounting/journal_entry/forms/line_item.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/journal_entry/forms/reorder.py` & `mia-accounting-1.3.0/src/accounting/journal_entry/forms/reorder.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/journal_entry/template_filters.py` & `mia-accounting-1.3.0/src/accounting/journal_entry/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/journal_entry/utils/__init__.py` & `mia-accounting-1.3.0/src/accounting/journal_entry/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/journal_entry/utils/account_option.py` & `mia-accounting-1.3.0/src/accounting/journal_entry/utils/account_option.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/journal_entry/utils/description_editor.py` & `mia-accounting-1.3.0/src/accounting/journal_entry/utils/description_editor.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/journal_entry/utils/operators.py` & `mia-accounting-1.3.0/src/accounting/journal_entry/utils/operators.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/journal_entry/utils/original_line_items.py` & `mia-accounting-1.3.0/src/accounting/journal_entry/utils/original_line_items.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/journal_entry/views.py` & `mia-accounting-1.3.0/src/accounting/journal_entry/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/locale.py` & `mia-accounting-1.3.0/src/accounting/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/models.py` & `mia-accounting-1.3.0/src/accounting/models.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/option/__init__.py` & `mia-accounting-1.3.0/src/accounting/option/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/option/forms.py` & `mia-accounting-1.3.0/src/accounting/option/forms.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/option/views.py` & `mia-accounting-1.3.0/src/accounting/option/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/__init__.py` & `mia-accounting-1.3.0/src/accounting/report/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/converters.py` & `mia-accounting-1.3.0/src/accounting/report/converters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/period/__init__.py` & `mia-accounting-1.3.0/src/accounting/report/period/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/period/chooser.py` & `mia-accounting-1.3.0/src/accounting/report/period/chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/period/description.py` & `mia-accounting-1.3.0/src/accounting/report/period/description.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/period/month_end.py` & `mia-accounting-1.3.0/src/accounting/report/period/month_end.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/period/parser.py` & `mia-accounting-1.3.0/src/accounting/report/period/parser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/period/period.py` & `mia-accounting-1.3.0/src/accounting/report/period/period.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/period/shortcuts.py` & `mia-accounting-1.3.0/src/accounting/report/period/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/period/specification.py` & `mia-accounting-1.3.0/src/accounting/report/period/specification.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/reports/__init__.py` & `mia-accounting-1.3.0/src/accounting/report/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/reports/balance_sheet.py` & `mia-accounting-1.3.0/src/accounting/report/reports/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/reports/income_expenses.py` & `mia-accounting-1.3.0/src/accounting/report/reports/income_expenses.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/reports/income_statement.py` & `mia-accounting-1.3.0/src/accounting/report/reports/income_statement.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/reports/journal.py` & `mia-accounting-1.3.0/src/accounting/report/reports/journal.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/reports/ledger.py` & `mia-accounting-1.3.0/src/accounting/report/reports/ledger.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/reports/search.py` & `mia-accounting-1.3.0/src/accounting/report/reports/search.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/reports/trial_balance.py` & `mia-accounting-1.3.0/src/accounting/report/reports/trial_balance.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/reports/unapplied.py` & `mia-accounting-1.3.0/src/accounting/report/reports/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/reports/unapplied_accounts.py` & `mia-accounting-1.3.0/src/accounting/report/reports/unapplied_accounts.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/template_filters.py` & `mia-accounting-1.3.0/src/accounting/report/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/utils/__init__.py` & `mia-accounting-1.3.0/src/accounting/report/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/utils/base_page_params.py` & `mia-accounting-1.3.0/src/accounting/report/utils/base_page_params.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/utils/base_report.py` & `mia-accounting-1.3.0/src/accounting/report/utils/base_report.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/utils/csv_export.py` & `mia-accounting-1.3.0/src/accounting/report/utils/csv_export.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/utils/option_link.py` & `mia-accounting-1.3.0/src/accounting/report/utils/option_link.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/utils/report_chooser.py` & `mia-accounting-1.3.0/src/accounting/report/utils/report_chooser.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/utils/report_type.py` & `mia-accounting-1.3.0/src/accounting/report/utils/report_type.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/utils/unapplied.py` & `mia-accounting-1.3.0/src/accounting/report/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/utils/urls.py` & `mia-accounting-1.3.0/src/accounting/report/utils/urls.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/report/views.py` & `mia-accounting-1.3.0/src/accounting/report/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/static/css/style.css` & `mia-accounting-1.3.0/src/accounting/static/css/style.css`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/static/js/account-form.js` & `mia-accounting-1.3.0/src/accounting/static/js/account-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/static/js/account-order.js` & `mia-accounting-1.3.0/src/accounting/static/js/account-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/static/js/currency-form.js` & `mia-accounting-1.3.0/src/accounting/static/js/currency-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/static/js/description-editor.js` & `mia-accounting-1.3.0/src/accounting/static/js/description-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/static/js/drag-and-drop-reorder.js` & `mia-accounting-1.3.0/src/accounting/static/js/drag-and-drop-reorder.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/static/js/journal-entry-account-selector.js` & `mia-accounting-1.3.0/src/accounting/static/js/journal-entry-account-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/static/js/journal-entry-form.js` & `mia-accounting-1.3.0/src/accounting/static/js/journal-entry-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/static/js/journal-entry-line-item-editor.js` & `mia-accounting-1.3.0/src/accounting/static/js/journal-entry-line-item-editor.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/static/js/journal-entry-order.js` & `mia-accounting-1.3.0/src/accounting/static/js/journal-entry-order.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/static/js/material-fab-speed-dial.js` & `mia-accounting-1.3.0/src/accounting/static/js/material-fab-speed-dial.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/static/js/option-form.js` & `mia-accounting-1.3.0/src/accounting/static/js/option-form.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/static/js/original-line-item-selector.js` & `mia-accounting-1.3.0/src/accounting/static/js/original-line-item-selector.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/static/js/period-chooser.js` & `mia-accounting-1.3.0/src/accounting/static/js/period-chooser.js`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/template_filters.py` & `mia-accounting-1.3.0/src/accounting/template_filters.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/template_globals.py` & `mia-accounting-1.3.0/src/accounting/template_globals.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/account/create.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/account/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/account/detail.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/account/edit.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/account/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/account/include/form.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/account/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/account/list.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/account/order.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/account/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/base-account/detail.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/base-account/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/base-account/list.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/base-account/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/base.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/currency/create.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/currency/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/currency/detail.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/currency/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/currency/edit.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/currency/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/currency/include/form.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/currency/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/currency/list.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/currency/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/include/nav.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/include/nav.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/include/pagination.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/include/pagination.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/disbursement/create.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/disbursement/detail.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/disbursement/edit.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/disbursement/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/description-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/detail-line-items.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/detail.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/form-currency.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form-debit-credit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/form-line-item.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form-line-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/form.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/journal-entry-line-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/order-journal-entry.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/include/original-line-item-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/order.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/order.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/receipt/create.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/receipt/detail.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/receipt/edit.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/receipt/include/form.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/receipt/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/transfer/create.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/create.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/transfer/detail.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/transfer/edit.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/edit.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/include/form-currency.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/journal-entry/transfer/include/form.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/journal-entry/transfer/include/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/option/detail.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/option/detail.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/option/form.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/option/form.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/form-recurring-expense-income.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/option/include/form-recurring-item.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/form-recurring-item.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/recurring-account-selector-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/option/include/recurring-item-editor-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/balance-sheet.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/balance-sheet.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/add-journal-entry-material-fab.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/balance-sheet-section.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/balance-sheet-section.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/income-expenses-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/income-expenses-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/ledger-row-desktop.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/ledger-row-desktop.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/ledger-row-mobile.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/ledger-row-mobile.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/period-chooser.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/period-chooser.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/search-modal.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/search-modal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/include/toolbar-buttons.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/include/toolbar-buttons.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/income-expenses.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/income-expenses.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/income-statement.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/income-statement.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/journal.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/journal.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/ledger.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/ledger.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/search.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/search.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/trial-balance.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/trial-balance.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/unapplied-accounts.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/unapplied-accounts.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/report/unapplied.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/report/unapplied.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/unmatched-offset/dashboard.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/unmatched-offset/dashboard.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/templates/accounting/unmatched-offset/list.html` & `mia-accounting-1.3.0/src/accounting/templates/accounting/unmatched-offset/list.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/translations/accounting.pot` & `mia-accounting-1.3.0/src/accounting/translations/accounting.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo` & `mia-accounting-1.3.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po` & `mia-accounting-1.3.0/src/accounting/translations/zh_Hans/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo` & `mia-accounting-1.3.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po` & `mia-accounting-1.3.0/src/accounting/translations/zh_Hant/LC_MESSAGES/accounting.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/unmatched_offset/__init__.py` & `mia-accounting-1.3.0/src/accounting/unmatched_offset/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/unmatched_offset/queries.py` & `mia-accounting-1.3.0/src/accounting/unmatched_offset/queries.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/unmatched_offset/views.py` & `mia-accounting-1.3.0/src/accounting/unmatched_offset/views.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/__init__.py` & `mia-accounting-1.3.0/src/accounting/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/cast.py` & `mia-accounting-1.3.0/src/accounting/utils/cast.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/current_account.py` & `mia-accounting-1.3.0/src/accounting/utils/current_account.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/flash_errors.py` & `mia-accounting-1.3.0/src/accounting/utils/flash_errors.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/journal_entry_types.py` & `mia-accounting-1.3.0/src/accounting/utils/journal_entry_types.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/next_uri.py` & `mia-accounting-1.3.0/src/accounting/utils/next_uri.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/offset_alias.py` & `mia-accounting-1.3.0/src/accounting/utils/offset_alias.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/offset_matcher.py` & `mia-accounting-1.3.0/src/accounting/utils/offset_matcher.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/options.py` & `mia-accounting-1.3.0/src/accounting/utils/options.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/pagination.py` & `mia-accounting-1.3.0/src/accounting/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/permission.py` & `mia-accounting-1.3.0/src/accounting/utils/permission.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/query.py` & `mia-accounting-1.3.0/src/accounting/utils/query.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/random_id.py` & `mia-accounting-1.3.0/src/accounting/utils/random_id.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/strip_text.py` & `mia-accounting-1.3.0/src/accounting/utils/strip_text.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/unapplied.py` & `mia-accounting-1.3.0/src/accounting/utils/unapplied.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/accounting/utils/user.py` & `mia-accounting-1.3.0/src/accounting/utils/user.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/src/mia_accounting.egg-info/PKG-INFO` & `mia-accounting-1.3.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: mia-accounting
-Version: 1.2.1
-Summary: A Flask accounting module.
-Author-email: imacat <imacat@mail.imacat.idv.tw>
-Project-URL: Documentation, https://mia-accounting.readthedocs.io
-Project-URL: Repository, https://github.com/imacat/mia-accounting
-Project-URL: Bug Tracker, https://github.com/imacat/mia-accounting/issues
-Project-URL: Demonstration, https://accounting.imacat.idv.tw
-Keywords: mia,accounting,flask
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Flask
-Classifier: Topic :: Office/Business :: Financial :: Accounting
-Requires-Python: >=3.11
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-License-File: LICENSE
-
 ===============
 Mia! Accounting
 ===============
 
 
 Description
 ===========
@@ -63,15 +43,16 @@
 start one, you may start with the test site.
 
 
 Prerequisites
 =============
 
 You need a running Flask application with database user login.
-The primary key of the user data model must be integer.
+The primary key of the user data model must be integer.  You also
+need at least one user.
 
 The following front-end JavaScript libraries must be loaded.  You may
 download it locally or use CDN_.
 
 * Bootstrap_ 5.2.3 or above
 * FontAwesome_ 6.2.1 or above
 * `Decimal.js`_ 6.4.3 or above
@@ -138,32 +119,21 @@
 
         return app
 
 
 Database Initialization
 =======================
 
-After the configuration, you need to run
-`flask_sqlalchemy.SQLAlchemy.create_all`_ to create the
-database tables that *Mia! Accounting* uses.
-
-*Mia! Accounting* adds three console commands:
-
-* ``accounting-init-base``
-* ``accounting-init-accounts``
-* ``accounting-init-currencies``
-
-After database tables are created, run
-``accounting-init-base`` first, and then the other two commands.
+After the configuration, run the ``accounting-init-db`` console
+command to initialize the accounting database.  You need to specify
+the username of a user as the data creator.
 
 ::
 
-    % flask --app myapp accounting-init-base
-    % flask --app myapp accounting-init-accounts
-    % flask --app myapp accounting-init-currencies
+    % flask --app myapp accounting-init-db -u username
 
 
 Navigation Menu
 ===============
 
 Include the navigation menu in the `Bootstrap navigation bar`_ in your
 base template:
```

### Comparing `mia-accounting-1.2.1/src/mia_accounting.egg-info/SOURCES.txt` & `mia-accounting-1.3.0/src/mia_accounting.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 docs/source/history.rst
 docs/source/index.rst
 docs/source/intro.rst
 docs/source/modules.rst
 docs/source/_static/.keep
 docs/source/_templates/.keep
 src/accounting/__init__.py
+src/accounting/commands.py
 src/accounting/forms.py
 src/accounting/locale.py
 src/accounting/models.py
 src/accounting/template_filters.py
 src/accounting/template_globals.py
 src/accounting/account/__init__.py
 src/accounting/account/commands.py
@@ -212,14 +213,15 @@
 src/mia_accounting.egg-info/dependency_links.txt
 src/mia_accounting.egg-info/requires.txt
 src/mia_accounting.egg-info/top_level.txt
 tests/babel-utils-test-site.py
 tests/babel-utils.py
 tests/test_account.py
 tests/test_base_account.py
+tests/test_commands.py
 tests/test_currency.py
 tests/test_description_editor.py
 tests/test_journal_entry.py
 tests/test_offset.py
 tests/test_option.py
 tests/test_report.py
 tests/test_unmatched_offset.py
```

### Comparing `mia-accounting-1.2.1/tests/babel-utils-test-site.py` & `mia-accounting-1.3.0/tests/babel-utils-test-site.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/babel-utils.py` & `mia-accounting-1.3.0/tests/babel-utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/test_account.py` & `mia-accounting-1.3.0/tests/test_account.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,15 @@
 """The test for the account management.
 
 """
 import unittest
 from datetime import timedelta, date
 
 import httpx
-import sqlalchemy as sa
-from click.testing import Result
 from flask import Flask
-from flask.testing import FlaskCliRunner
 
 from test_site import db
 from testlib import NEXT_URI, create_test_app, get_client, set_locale, \
     add_journal_entry
 
 
 class AccountData:
@@ -61,87 +58,27 @@
 """The stock account."""
 LOAN: AccountData = AccountData("2112", 1, "Loan")
 """The loan account."""
 PREFIX: str = "/accounting/accounts"
 """The URL prefix for the account management."""
 
 
-class AccountCommandTestCase(unittest.TestCase):
-    """The account console command test case."""
-
-    def setUp(self) -> None:
-        """Sets up the test.
-        This is run once per test.
-
-        :return: None.
-        """
-        self.app: Flask = create_test_app()
-
-        runner: FlaskCliRunner = self.app.test_cli_runner()
-        with self.app.app_context():
-            from accounting.models import BaseAccount, Account, AccountL10n
-            result: Result
-            result = runner.invoke(args="init-db")
-            self.assertEqual(result.exit_code, 0)
-            if BaseAccount.query.first() is None:
-                result = runner.invoke(args="accounting-init-base")
-                self.assertEqual(result.exit_code, 0)
-            AccountL10n.query.delete()
-            Account.query.delete()
-            db.session.commit()
-
-    def test_init(self) -> None:
-        """Tests the "accounting-init-account" console command.
-
-        :return: None.
-        """
-        from accounting.models import BaseAccount, Account, AccountL10n
-        runner: FlaskCliRunner = self.app.test_cli_runner()
-        with self.app.app_context():
-            result: Result = runner.invoke(args=["accounting-init-accounts",
-                                                 "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
-        with self.app.app_context():
-            bases: list[BaseAccount] = BaseAccount.query\
-                .filter(sa.func.char_length(BaseAccount.code) == 4).all()
-            accounts: list[Account] = Account.query.all()
-            l10n: list[AccountL10n] = AccountL10n.query.all()
-        self.assertEqual({x.code for x in bases},
-                         {x.base_code for x in accounts})
-        self.assertEqual(len(accounts), len(bases))
-        self.assertEqual(len(l10n), len(bases) * 2)
-        base_dict: dict[str, BaseAccount] = {x.code: x for x in bases}
-        for account in accounts:
-            base: BaseAccount = base_dict[account.base_code]
-            self.assertEqual(account.no, 1)
-            self.assertEqual(account.title_l10n, base.title_l10n)
-            self.assertEqual({x.locale: x.title for x in account.l10n},
-                             {x.locale: x.title for x in base.l10n})
-
-
 class AccountTestCase(unittest.TestCase):
     """The account test case."""
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
         self.app: Flask = create_test_app()
 
-        runner: FlaskCliRunner = self.app.test_cli_runner()
         with self.app.app_context():
-            from accounting.models import BaseAccount, Account, AccountL10n
-            result: Result
-            result = runner.invoke(args="init-db")
-            self.assertEqual(result.exit_code, 0)
-            if BaseAccount.query.first() is None:
-                result = runner.invoke(args="accounting-init-base")
-                self.assertEqual(result.exit_code, 0)
+            from accounting.models import Account, AccountL10n
             AccountL10n.query.delete()
             Account.query.delete()
             db.session.commit()
 
         self.client, self.csrf_token = get_client(self.app, "editor")
         response: httpx.Response
 
@@ -648,22 +585,14 @@
         response = self.client.post(f"{PREFIX}/store",
                                     data={"csrf_token": self.csrf_token,
                                           "base_code": PETTY.base_code,
                                           "title": PETTY.title})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
 
-        response = self.client.post("/accounting/currencies/store",
-                                    data={"csrf_token": self.csrf_token,
-                                          "code": "USD",
-                                          "name": "US Dollars"})
-        self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"],
-                         "/accounting/currencies/USD")
-
         add_journal_entry(self.client,
                           form={"csrf_token": self.csrf_token,
                                 "next": NEXT_URI,
                                 "date": date.today().isoformat(),
                                 "currency-1-code": "USD",
                                 "currency-1-credit-1-account_code": BANK.code,
                                 "currency-1-credit-1-amount": "20"})
```

### Comparing `mia-accounting-1.2.1/tests/test_currency.py` & `mia-accounting-1.3.0/tests/test_currency.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,19 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """The test for the currency management.
 
 """
-import csv
-import typing as t
 import unittest
 from datetime import timedelta, date
 
 import httpx
-from click.testing import Result
 from flask import Flask
-from flask.testing import FlaskCliRunner
 
 from test_site import db
 from testlib import NEXT_URI, create_test_app, get_client, set_locale, \
     add_journal_entry
 
 
 class CurrencyData:
@@ -55,87 +51,27 @@
 """The Taiwan dollars."""
 JPY: CurrencyData = CurrencyData("JPY", "Japanese yen")
 """The Japanese yen."""
 PREFIX: str = "/accounting/currencies"
 """The URL prefix for the currency management."""
 
 
-class CurrencyCommandTestCase(unittest.TestCase):
-    """The account console command test case."""
-
-    def setUp(self) -> None:
-        """Sets up the test.
-        This is run once per test.
-
-        :return: None.
-        """
-        self.app: Flask = create_test_app()
-
-        runner: FlaskCliRunner = self.app.test_cli_runner()
-        with self.app.app_context():
-            from accounting.models import Currency, CurrencyL10n
-            result: Result
-            result = runner.invoke(args="init-db")
-            self.assertEqual(result.exit_code, 0)
-            CurrencyL10n.query.delete()
-            Currency.query.delete()
-            db.session.commit()
-
-    def test_init(self) -> None:
-        """Tests the "accounting-init-currencies" console command.
-
-        :return: None.
-        """
-        from accounting import data_dir
-        from accounting.models import Currency
-
-        with open(data_dir / "currencies.csv") as fp:
-            data: dict[dict[str, t.Any]] \
-                = {x["code"]: {"code": x["code"],
-                               "name": x["name"],
-                               "l10n": {y[5:]: x[y]
-                                        for y in x if y.startswith("l10n-")}}
-                   for x in csv.DictReader(fp)}
-
-        runner: FlaskCliRunner = self.app.test_cli_runner()
-        with self.app.app_context():
-            result: Result = runner.invoke(
-                args=["accounting-init-currencies", "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
-            currencies: list[Currency] = Currency.query.all()
-
-        self.assertEqual(len(currencies), len(data))
-        for currency in currencies:
-            self.assertIn(currency.code, data)
-            self.assertEqual(currency.name_l10n, data[currency.code]["name"])
-            l10n: dict[str, str] = {x.locale: x.name for x in currency.l10n}
-            self.assertEqual(len(l10n), len(data[currency.code]["l10n"]))
-            for locale in l10n:
-                self.assertIn(locale, data[currency.code]["l10n"])
-                self.assertEqual(l10n[locale],
-                                 data[currency.code]["l10n"][locale])
-
-
 class CurrencyTestCase(unittest.TestCase):
     """The currency test case."""
 
     def setUp(self) -> None:
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
         self.app: Flask = create_test_app()
 
-        runner: FlaskCliRunner = self.app.test_cli_runner()
         with self.app.app_context():
             from accounting.models import Currency, CurrencyL10n
-            result: Result
-            result = runner.invoke(args="init-db")
-            self.assertEqual(result.exit_code, 0)
             CurrencyL10n.query.delete()
             Currency.query.delete()
             db.session.commit()
 
         self.client, self.csrf_token = get_client(self.app, "editor")
         response: httpx.Response
 
@@ -584,29 +520,14 @@
         """
         from accounting.models import Currency
         detail_uri: str = f"{PREFIX}/{JPY.code}"
         delete_uri: str = f"{PREFIX}/{JPY.code}/delete"
         list_uri: str = PREFIX
         response: httpx.Response
 
-        runner: FlaskCliRunner = self.app.test_cli_runner()
-        with self.app.app_context():
-            from accounting.models import BaseAccount
-            if BaseAccount.query.first() is None:
-                result = runner.invoke(args="accounting-init-base")
-                self.assertEqual(result.exit_code, 0)
-
-        response = self.client.post("/accounting/accounts/store",
-                                    data={"csrf_token": self.csrf_token,
-                                          "base_code": "1111",
-                                          "title": "Cash"})
-        self.assertEqual(response.status_code, 302)
-        self.assertEqual(response.headers["Location"],
-                         "/accounting/accounts/1111-001")
-
         response = self.client.post(f"{PREFIX}/store",
                                     data={"csrf_token": self.csrf_token,
                                           "code": JPY.code,
                                           "name": JPY.name})
         self.assertEqual(response.status_code, 302)
         self.assertEqual(response.headers["Location"], detail_uri)
```

### Comparing `mia-accounting-1.2.1/tests/test_description_editor.py` & `mia-accounting-1.3.0/tests/test_description_editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 #  limitations under the License.
 """The test for the description editor.
 
 """
 import unittest
 from datetime import date
 
-from click.testing import Result
 from flask import Flask
-from flask.testing import FlaskCliRunner
 
 from testlib import NEXT_URI, Accounts, create_test_app, get_client, \
     add_journal_entry
 
 
 class DescriptionEditorTestCase(unittest.TestCase):
     """The description editor test case."""
@@ -35,30 +33,16 @@
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
         self.app: Flask = create_test_app()
 
-        runner: FlaskCliRunner = self.app.test_cli_runner()
         with self.app.app_context():
-            from accounting.models import BaseAccount, JournalEntry, \
-                JournalEntryLineItem
-            result: Result
-            result = runner.invoke(args="init-db")
-            self.assertEqual(result.exit_code, 0)
-            if BaseAccount.query.first() is None:
-                result = runner.invoke(args="accounting-init-base")
-                self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-currencies",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-accounts",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
+            from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
 
         self.client, self.csrf_token = get_client(self.app, "editor")
 
     def test_description_editor(self) -> None:
         """Test the description editor.
```

### Comparing `mia-accounting-1.2.1/tests/test_journal_entry.py` & `mia-accounting-1.3.0/tests/test_journal_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 
 """
 import unittest
 from datetime import date, timedelta
 from decimal import Decimal
 
 import httpx
-from click.testing import Result
 from flask import Flask
-from flask.testing import FlaskCliRunner
 
 from test_site import db
 from testlib import NEXT_URI, Accounts, create_test_app, get_client, \
     add_journal_entry, match_journal_entry_detail
 from testlib_journal_entry import NON_EMPTY_NOTE, EMPTY_NOTE, \
     get_add_form, get_unchanged_update_form, get_update_form, \
     set_negative_amount, remove_debit_in_a_currency, \
@@ -47,30 +45,16 @@
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
         self.app: Flask = create_test_app()
 
-        runner: FlaskCliRunner = self.app.test_cli_runner()
         with self.app.app_context():
-            from accounting.models import BaseAccount, JournalEntry, \
-                JournalEntryLineItem
-            result: Result
-            result = runner.invoke(args="init-db")
-            self.assertEqual(result.exit_code, 0)
-            if BaseAccount.query.first() is None:
-                result = runner.invoke(args="accounting-init-base")
-                self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-currencies",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-accounts",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
+            from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
 
         self.client, self.csrf_token = get_client(self.app, "editor")
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
@@ -666,30 +650,16 @@
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
         self.app: Flask = create_test_app()
 
-        runner: FlaskCliRunner = self.app.test_cli_runner()
         with self.app.app_context():
-            from accounting.models import BaseAccount, JournalEntry, \
-                JournalEntryLineItem
-            result: Result
-            result = runner.invoke(args="init-db")
-            self.assertEqual(result.exit_code, 0)
-            if BaseAccount.query.first() is None:
-                result = runner.invoke(args="accounting-init-base")
-                self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-currencies",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-accounts",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
+            from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
 
         self.client, self.csrf_token = get_client(self.app, "editor")
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
@@ -1261,30 +1231,17 @@
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
         self.app: Flask = create_test_app()
 
-        runner: FlaskCliRunner = self.app.test_cli_runner()
         with self.app.app_context():
-            from accounting.models import BaseAccount, JournalEntry, \
+            from accounting.models import JournalEntry, \
                 JournalEntryLineItem
-            result: Result
-            result = runner.invoke(args="init-db")
-            self.assertEqual(result.exit_code, 0)
-            if BaseAccount.query.first() is None:
-                result = runner.invoke(args="accounting-init-base")
-                self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-currencies",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-accounts",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
 
         self.client, self.csrf_token = get_client(self.app, "editor")
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
@@ -2135,30 +2092,16 @@
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
         self.app: Flask = create_test_app()
 
-        runner: FlaskCliRunner = self.app.test_cli_runner()
         with self.app.app_context():
-            from accounting.models import BaseAccount, JournalEntry, \
-                JournalEntryLineItem
-            result: Result
-            result = runner.invoke(args="init-db")
-            self.assertEqual(result.exit_code, 0)
-            if BaseAccount.query.first() is None:
-                result = runner.invoke(args="accounting-init-base")
-                self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-currencies",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-accounts",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
+            from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
 
         self.client, self.csrf_token = get_client(self.app, "editor")
 
     def test_change_date(self) -> None:
         """Tests to change the date of a journal entry.
```

### Comparing `mia-accounting-1.2.1/tests/test_offset.py` & `mia-accounting-1.3.0/tests/test_offset.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,15 @@
 """
 from __future__ import annotations
 
 import unittest
 from decimal import Decimal
 
 import httpx
-from click.testing import Result
 from flask import Flask
-from flask.testing import FlaskCliRunner
 
 from test_site import db
 from testlib import Accounts, create_test_app, get_client, \
     match_journal_entry_detail, JournalEntryLineItemData, \
     JournalEntryCurrencyData, JournalEntryData, BaseTestData
 
 PREFIX: str = "/accounting/journal-entries"
@@ -43,30 +41,16 @@
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
         self.app: Flask = create_test_app()
 
-        runner: FlaskCliRunner = self.app.test_cli_runner()
         with self.app.app_context():
-            from accounting.models import BaseAccount, JournalEntry, \
-                JournalEntryLineItem
-            result: Result
-            result = runner.invoke(args="init-db")
-            self.assertEqual(result.exit_code, 0)
-            if BaseAccount.query.first() is None:
-                result = runner.invoke(args="accounting-init-base")
-                self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-currencies",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-accounts",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
+            from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
 
         self.client, self.csrf_token = get_client(self.app, "editor")
         self.data: OffsetTestData = OffsetTestData(
             self.app, self.client, self.csrf_token)
```

### Comparing `mia-accounting-1.2.1/tests/test_option.py` & `mia-accounting-1.3.0/tests/test_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 """The test for the options.
 
 """
 import unittest
 from datetime import datetime, timedelta
 
 import httpx
-from click.testing import Result
 from flask import Flask
-from flask.testing import FlaskCliRunner
 
 from test_site import db
 from testlib import NEXT_URI, Accounts, create_test_app, get_client
 
 PREFIX: str = "/accounting/options"
 """The URL prefix for the option management."""
 DETAIL_URI: str = f"{PREFIX}?next=%2F_next"
@@ -45,29 +43,16 @@
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
         self.app: Flask = create_test_app()
 
-        runner: FlaskCliRunner = self.app.test_cli_runner()
         with self.app.app_context():
-            from accounting.models import BaseAccount, Option
-            result: Result
-            result = runner.invoke(args="init-db")
-            self.assertEqual(result.exit_code, 0)
-            if BaseAccount.query.first() is None:
-                result = runner.invoke(args="accounting-init-base")
-                self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-currencies",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-accounts",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
+            from accounting.models import Option
             Option.query.delete()
 
         self.client, self.csrf_token = get_client(self.app, "admin")
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
```

### Comparing `mia-accounting-1.2.1/tests/test_report.py` & `mia-accounting-1.3.0/tests/test_report.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 """The test for the reports.
 
 """
 import unittest
 from datetime import date
 
 import httpx
-from click.testing import Result
 from flask import Flask
-from flask.testing import FlaskCliRunner
 
 from testlib import create_test_app, get_client, Accounts, BaseTestData
 
 PREFIX: str = "/accounting"
 """The URL prefix for the reports."""
 CSV_MIME: str = "text/csv; charset=utf-8"
 """The MIME type of the downloaded CSV files."""
@@ -40,30 +38,16 @@
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
         self.app: Flask = create_test_app()
 
-        runner: FlaskCliRunner = self.app.test_cli_runner()
         with self.app.app_context():
-            from accounting.models import BaseAccount, JournalEntry, \
-                JournalEntryLineItem
-            result: Result
-            result = runner.invoke(args="init-db")
-            self.assertEqual(result.exit_code, 0)
-            if BaseAccount.query.first() is None:
-                result = runner.invoke(args="accounting-init-base")
-                self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-currencies",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-accounts",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
+            from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
 
         self.client, self.csrf_token = get_client(self.app, "editor")
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
```

### Comparing `mia-accounting-1.2.1/tests/test_site/__init__.py` & `mia-accounting-1.3.0/tests/test_site/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 """The Mia! Accounting demonstration website.
 
 """
 import os
 import typing as t
 from secrets import token_urlsafe
 
-import click
+from click.testing import Result
 from flask import Flask, Blueprint, render_template, redirect, Response
-from flask.cli import with_appcontext
+from flask.testing import FlaskCliRunner
 from flask_babel_js import BabelJS
 from flask_sqlalchemy import SQLAlchemy
 from flask_wtf import CSRFProtect
 from sqlalchemy import Column
 
 bp: Blueprint = Blueprint("home", __name__)
 """The global blueprint."""
@@ -59,15 +59,14 @@
         app.config["TESTING"] = True
 
     babel_js.init_app(app)
     csrf.init_app(app)
     db.init_app(app)
 
     app.register_blueprint(bp, url_prefix="/")
-    app.cli.add_command(init_db_command)
 
     from . import locale
     locale.init_app(app)
 
     from . import auth
     auth.init_app(app)
 
@@ -106,28 +105,35 @@
                 .filter(auth.User.username == username).first()
 
         def get_pk(self, user: auth.User) -> int:
             return user.id
 
     accounting.init_app(app, user_utils=UserUtilities())
 
+    with app.app_context():
+        init_db(app)
+
     return app
 
 
-@click.command("init-db")
-@with_appcontext
-def init_db_command() -> None:
-    """Initializes the database."""
+def init_db(app: Flask) -> None:
+    """Initializes the database.
+
+    :param app: The Flask application.
+    :return: None.
+    """
     db.create_all()
     from .auth import User
     for username in ["viewer", "editor", "admin", "nobody"]:
         if User.query.filter(User.username == username).first() is None:
             db.session.add(User(username=username))
     db.session.commit()
-    click.echo("Database initialized successfully.")
+    runner: FlaskCliRunner = app.test_cli_runner()
+    result: Result = runner.invoke(args=["accounting-init-db", "-u", "editor"])
+    assert result.exit_code == 0, result.output + str(result.exception)
 
 
 @bp.get("/", endpoint="home")
 def get_home() -> str:
     """Returns the home page.
 
     :return: The home page.
```

### Comparing `mia-accounting-1.2.1/tests/test_site/auth.py` & `mia-accounting-1.3.0/tests/test_site/auth.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/test_site/locale.py` & `mia-accounting-1.3.0/tests/test_site/locale.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/test_site/static/favicon.svg` & `mia-accounting-1.3.0/tests/test_site/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/test_site/templates/base.html` & `mia-accounting-1.3.0/tests/test_site/templates/base.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/test_site/templates/home.html` & `mia-accounting-1.3.0/tests/test_site/templates/home.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/test_site/templates/login.html` & `mia-accounting-1.3.0/tests/test_site/templates/login.html`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/test_site/translations/messages.pot` & `mia-accounting-1.3.0/tests/test_site/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo` & `mia-accounting-1.3.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po` & `mia-accounting-1.3.0/tests/test_site/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo` & `mia-accounting-1.3.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po` & `mia-accounting-1.3.0/tests/test_site/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/test_unmatched_offset.py` & `mia-accounting-1.3.0/tests/test_unmatched_offset.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 #  limitations under the License.
 """The test for the unmatched offsets.
 
 """
 import unittest
 
 import httpx
-from click.testing import Result
 from flask import Flask
-from flask.testing import FlaskCliRunner
 
 from test_site import db
 from testlib import create_test_app, get_client, Accounts, \
     JournalEntryCurrencyData, JournalEntryData, BaseTestData
 
 PREFIX: str = "/accounting/unmatched-offsets"
 """The URL prefix for the unmatched offset management."""
@@ -39,30 +37,16 @@
         """Sets up the test.
         This is run once per test.
 
         :return: None.
         """
         self.app: Flask = create_test_app()
 
-        runner: FlaskCliRunner = self.app.test_cli_runner()
         with self.app.app_context():
-            from accounting.models import BaseAccount, JournalEntry, \
-                JournalEntryLineItem
-            result: Result
-            result = runner.invoke(args="init-db")
-            self.assertEqual(result.exit_code, 0)
-            if BaseAccount.query.first() is None:
-                result = runner.invoke(args="accounting-init-base")
-                self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-currencies",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
-            result = runner.invoke(args=["accounting-init-accounts",
-                                         "-u", "editor"])
-            self.assertEqual(result.exit_code, 0)
+            from accounting.models import JournalEntry, JournalEntryLineItem
             JournalEntry.query.delete()
             JournalEntryLineItem.query.delete()
 
         self.client, self.csrf_token = get_client(self.app, "editor")
 
     def test_nobody(self) -> None:
         """Test the permission as nobody.
```

### Comparing `mia-accounting-1.2.1/tests/test_utils.py` & `mia-accounting-1.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/testlib.py` & `mia-accounting-1.3.0/tests/testlib.py`

 * *Files identical despite different names*

### Comparing `mia-accounting-1.2.1/tests/testlib_journal_entry.py` & `mia-accounting-1.3.0/tests/testlib_journal_entry.py`

 * *Files identical despite different names*

