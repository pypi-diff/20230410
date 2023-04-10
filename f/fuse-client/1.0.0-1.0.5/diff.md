# Comparing `tmp/fuse_client-1.0.0.tar.gz` & `tmp/fuse_client-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuse_client-1.0.0.tar", last modified: Fri Apr  7 09:35:50 2023, max compression
+gzip compressed data, was "fuse_client-1.0.5.tar", last modified: Mon Apr 10 09:07:11 2023, max compression
```

## Comparing `fuse_client-1.0.0.tar` & `fuse_client-1.0.5.tar`

### file list

```diff
@@ -1,455 +1,122 @@
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.895591 fuse_client-1.0.0/
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-06 23:42:07.000000 fuse_client-1.0.0/LICENSE
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1158 2023-04-07 09:35:50.895678 fuse_client-1.0.0/PKG-INFO
--rw-r--r--   0 adibpournazari   (501) staff       (20)      796 2023-04-06 23:42:55.000000 fuse_client-1.0.0/README.md
--rw-r--r--   0 adibpournazari   (501) staff       (20)      577 2023-04-06 23:42:55.000000 fuse_client-1.0.0/pyproject.toml
--rw-r--r--   0 adibpournazari   (501) staff       (20)      573 2023-04-07 09:35:50.898982 fuse_client-1.0.0/setup.cfg
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.743319 fuse_client-1.0.0/src/
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.742618 fuse_client-1.0.0/src/3/
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.744143 fuse_client-1.0.0/src/3/4/
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.744778 fuse_client-1.0.0/src/3/4/5/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/__init__.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.745204 fuse_client-1.0.0/src/3/4/5/apis/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/apis/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    17509 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/apis/fuse_api.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      548 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/main.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.768843 fuse_client-1.0.0/src/3/4/5/models/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      534 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/account_subtype.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/account_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      522 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/aggregator.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/country_code.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1245 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/create_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1078 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/create_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1175 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/create_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1330 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/create_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1739 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/create_link_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      711 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/create_link_token_request_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      723 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/create_link_token_request_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      793 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/create_link_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1790 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/create_session_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      909 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/create_session_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1029 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/delete_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      801 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      812 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/exchange_financial_connections_public_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1113 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/exchange_financial_connections_public_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      125 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/extra_models.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      777 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2028 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connection_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      818 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connection_details_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      829 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connection_details_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      858 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connection_details_teller.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1960 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1441 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1328 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_cached_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      955 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1255 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_details_ach.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      748 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3646 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_liability.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2237 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_liability_all_of.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      983 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_liability_all_of_aprs.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1462 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_holding.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1977 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_investment_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1356 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_investment_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2316 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_investment_security.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      780 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_investment_security_currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      796 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_investment_security_exchange.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2491 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_investment_transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      910 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_investment_transaction_currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1604 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_owner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1066 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_owner_addresses_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1412 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_owner_addresses_inner_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      998 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_owner_emails_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      840 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_owner_names_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1034 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_connections_owner_phone_numbers_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1269 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      890 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/financial_institution_logo.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1323 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/fuse_api_error.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      934 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/fuse_api_error_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1347 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/fuse_api_warning.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1012 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/fuse_api_warning_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1284 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/fuse_api_warning_data_warnings_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      701 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      954 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1805 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_asset_report_response_report.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1847 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_asset_report_response_report_accounts_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1186 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_asset_report_response_report_accounts_inner_balances.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1254 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_asset_report_response_report_accounts_inner_historical_balances_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1500 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      972 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      769 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_account_details_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1331 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_account_details_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      745 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_accounts_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1245 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_accounts_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      741 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_balance_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      995 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_balance_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      737 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_owners_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      911 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_owners_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1190 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_owners_response_accounts_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1647 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1134 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      962 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_financial_institution_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      982 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_investment_holdings_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      798 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_investment_holdings_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1155 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_investment_holdings_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2000 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_investment_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      814 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_investment_transactions_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1586 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_investment_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      677 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_liabilities_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1003 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/get_liabilities_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1338 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/migrate_financial_connections_aggregator_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      978 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/migrate_financial_connections_aggregator_connection_data_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      817 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/migrate_financial_connections_aggregator_connection_data_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1550 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/migrate_financial_connections_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      768 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/migrate_financial_connections_token_request_entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1481 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/migrate_financial_connections_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      513 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/product.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1286 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/refresh_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      916 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/sync_financial_connections_data_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      951 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/sync_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1652 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/sync_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      780 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/sync_transactions_response_removed_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1761 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      672 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/transaction_merchant.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1060 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/update_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1330 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/update_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1370 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/webhook_event.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      531 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/webhook_source.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/models/webhook_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     8146 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/5/security_api.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/3/4/__init__.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.769365 fuse_client-1.0.0/src/fuse_client/
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.770817 fuse_client-1.0.0/src/fuse_client/apis/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/apis/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    17749 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/apis/fuse_api.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      554 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/main.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.792730 fuse_client-1.0.0/src/fuse_client/models/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      534 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/account_subtype.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/account_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      522 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/aggregator.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/country_code.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1245 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/create_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1078 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/create_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1181 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/create_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1336 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/create_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1757 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/create_link_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      711 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/create_link_token_request_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      723 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/create_link_token_request_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      793 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/create_link_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1814 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/create_session_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      909 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/create_session_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1029 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/delete_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      801 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      812 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/exchange_financial_connections_public_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1113 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/exchange_financial_connections_public_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      125 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/extra_models.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      777 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2052 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connection_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      818 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connection_details_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      829 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connection_details_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      858 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connection_details_teller.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1984 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1441 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1328 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_account_cached_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      961 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_account_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1255 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_account_details_ach.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      748 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_account_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3676 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_account_liability.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2243 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_account_liability_all_of.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      983 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_account_liability_all_of_aprs.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1468 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_holding.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1989 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_investment_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1356 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_investment_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2328 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_investment_security.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      780 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_investment_security_currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      796 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_investment_security_exchange.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2503 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_investment_transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      910 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_investment_transaction_currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1628 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_owner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1072 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_owner_addresses_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1412 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_owner_addresses_inner_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      998 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_owner_emails_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      840 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_owner_names_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1034 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_connections_owner_phone_numbers_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1281 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      890 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/financial_institution_logo.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1329 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/fuse_api_error.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      946 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/fuse_api_error_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1353 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/fuse_api_warning.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1024 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/fuse_api_warning_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1284 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/fuse_api_warning_data_warnings_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      701 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      960 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1817 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_asset_report_response_report.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1865 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_asset_report_response_report_accounts_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1186 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_asset_report_response_report_accounts_inner_balances.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1254 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_asset_report_response_report_accounts_inner_historical_balances_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1512 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      978 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      769 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_financial_connections_account_details_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1343 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_financial_connections_account_details_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      745 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_financial_connections_accounts_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1257 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_financial_connections_accounts_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      741 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_financial_connections_balance_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1001 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_financial_connections_balance_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      737 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_financial_connections_owners_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      917 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_financial_connections_owners_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1196 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_financial_connections_owners_response_accounts_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1647 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_financial_connections_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1140 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_financial_connections_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      968 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_financial_institution_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      988 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_investment_holdings_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      798 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_investment_holdings_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1167 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_investment_holdings_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2006 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_investment_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      814 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_investment_transactions_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1604 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_investment_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      677 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_liabilities_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1009 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/get_liabilities_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1350 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/migrate_financial_connections_aggregator_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      978 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/migrate_financial_connections_aggregator_connection_data_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      817 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/migrate_financial_connections_aggregator_connection_data_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1568 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/migrate_financial_connections_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      768 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/migrate_financial_connections_token_request_entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1487 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/migrate_financial_connections_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      513 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/product.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1286 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/refresh_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      916 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/sync_financial_connections_data_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      951 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/sync_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1664 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/sync_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      780 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/sync_transactions_response_removed_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1767 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      672 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/transaction_merchant.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1066 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/update_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1336 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/update_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1382 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/webhook_event.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      531 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/webhook_source.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/models/webhook_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     8152 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_client/security_api.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.770477 fuse_client-1.0.0/src/fuse_client.egg-info/
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1158 2023-04-07 09:35:50.000000 fuse_client-1.0.0/src/fuse_client.egg-info/PKG-INFO
--rw-r--r--   0 adibpournazari   (501) staff       (20)    25325 2023-04-07 09:35:50.000000 fuse_client-1.0.0/src/fuse_client.egg-info/SOURCES.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)        1 2023-04-07 09:35:50.000000 fuse_client-1.0.0/src/fuse_client.egg-info/dependency_links.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)       13 2023-04-07 09:35:50.000000 fuse_client-1.0.0/src/fuse_client.egg-info/requires.txt
--rw-r--r--   0 adibpournazari   (501) staff       (20)       42 2023-04-07 09:35:50.000000 fuse_client-1.0.0/src/fuse_client.egg-info/top_level.txt
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.793016 fuse_client-1.0.0/src/fuse_clients/
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.793370 fuse_client-1.0.0/src/fuse_clients/apis/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/apis/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    17789 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/apis/fuse_api.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      555 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/main.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.811315 fuse_client-1.0.0/src/fuse_clients/models/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      534 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/account_subtype.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/account_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      522 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/aggregator.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/country_code.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1245 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/create_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1078 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/create_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1182 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/create_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1337 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/create_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1760 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/create_link_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      711 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/create_link_token_request_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      723 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/create_link_token_request_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      793 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/create_link_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1818 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/create_session_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      909 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/create_session_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1029 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/delete_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      801 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      812 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/exchange_financial_connections_public_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1113 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/exchange_financial_connections_public_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      125 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/extra_models.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      777 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2056 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connection_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      818 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connection_details_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      829 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connection_details_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      858 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connection_details_teller.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1988 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1441 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1328 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_account_cached_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      962 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_account_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1255 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_account_details_ach.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      748 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_account_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3681 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_account_liability.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2244 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_account_liability_all_of.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      983 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_account_liability_all_of_aprs.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1469 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_holding.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1991 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_investment_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1356 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_investment_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2330 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_investment_security.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      780 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_investment_security_currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      796 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_investment_security_exchange.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2505 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_investment_transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      910 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_investment_transaction_currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1632 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_owner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1073 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_owner_addresses_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1412 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_owner_addresses_inner_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      998 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_owner_emails_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      840 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_owner_names_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1034 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_connections_owner_phone_numbers_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1283 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      890 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/financial_institution_logo.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1330 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/fuse_api_error.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      948 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/fuse_api_error_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1354 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/fuse_api_warning.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1026 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/fuse_api_warning_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1284 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/fuse_api_warning_data_warnings_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      701 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      961 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1819 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_asset_report_response_report.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1868 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_asset_report_response_report_accounts_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1186 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_asset_report_response_report_accounts_inner_balances.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1254 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_asset_report_response_report_accounts_inner_historical_balances_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1514 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      979 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      769 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_financial_connections_account_details_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1345 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_financial_connections_account_details_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      745 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_financial_connections_accounts_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1259 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_financial_connections_accounts_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      741 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_financial_connections_balance_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1002 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_financial_connections_balance_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      737 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_financial_connections_owners_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      918 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_financial_connections_owners_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1197 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_financial_connections_owners_response_accounts_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1647 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_financial_connections_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1141 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_financial_connections_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      969 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_financial_institution_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      989 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_investment_holdings_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      798 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_investment_holdings_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1169 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_investment_holdings_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2007 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_investment_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      814 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_investment_transactions_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1607 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_investment_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      677 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_liabilities_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1010 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/get_liabilities_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1352 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/migrate_financial_connections_aggregator_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      978 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/migrate_financial_connections_aggregator_connection_data_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      817 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/migrate_financial_connections_aggregator_connection_data_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1571 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/migrate_financial_connections_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      768 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/migrate_financial_connections_token_request_entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1488 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/migrate_financial_connections_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      513 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/product.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1286 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/refresh_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      916 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/sync_financial_connections_data_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      951 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/sync_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1666 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/sync_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      780 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/sync_transactions_response_removed_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1768 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      672 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/transaction_merchant.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/update_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1337 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/update_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1384 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/webhook_event.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      531 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/webhook_source.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/models/webhook_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     8153 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/fuse_clients/security_api.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.811698 fuse_client-1.0.0/src/openapi_server/
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.812584 fuse_client-1.0.0/src/openapi_server/apis/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/apis/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)    17869 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/apis/fuse_api.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      557 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/main.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.894940 fuse_client-1.0.0/src/openapi_server/models/
--rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/__init__.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      534 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/account_subtype.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/account_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      522 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/aggregator.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/country_code.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1245 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/create_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1078 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/create_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1184 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/create_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1339 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/create_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1766 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/create_link_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      711 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/create_link_token_request_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      723 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/create_link_token_request_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      793 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/create_link_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1826 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/create_session_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      909 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/create_session_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1029 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/delete_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      801 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      812 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/exchange_financial_connections_public_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1113 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/exchange_financial_connections_public_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      125 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/extra_models.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      777 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2064 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connection_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      818 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connection_details_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      829 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connection_details_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      858 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connection_details_teller.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1996 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1441 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1328 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_account_cached_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      964 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_account_details.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1255 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_account_details_ach.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      748 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_account_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     3691 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_account_liability.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2246 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_account_liability_all_of.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      983 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_account_liability_all_of_aprs.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1471 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_holding.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1995 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_investment_account.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1356 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_investment_account_balance.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2334 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_investment_security.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      780 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_investment_security_currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      796 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_investment_security_exchange.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2509 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_investment_transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      910 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_investment_transaction_currency.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1640 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_owner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1075 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_owner_addresses_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1412 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_owner_addresses_inner_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      998 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_owner_emails_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      840 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_owner_names_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1034 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_connections_owner_phone_numbers_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1287 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_institution.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      890 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/financial_institution_logo.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1332 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/fuse_api_error.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      952 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/fuse_api_error_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1356 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/fuse_api_warning.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1030 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/fuse_api_warning_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1284 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/fuse_api_warning_data_warnings_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      701 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      963 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_asset_report_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1823 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_asset_report_response_report.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1874 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_asset_report_response_report_accounts_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1186 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_asset_report_response_report_accounts_inner_balances.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1254 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_asset_report_response_report_accounts_inner_historical_balances_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1518 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      981 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_financial_connection_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      769 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_financial_connections_account_details_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1349 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_financial_connections_account_details_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      745 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_financial_connections_accounts_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1263 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_financial_connections_accounts_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      741 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_financial_connections_balance_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1004 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_financial_connections_balance_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      737 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_financial_connections_owners_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      920 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_financial_connections_owners_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1199 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_financial_connections_owners_response_accounts_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1647 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_financial_connections_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1143 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_financial_connections_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      971 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_financial_institution_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      991 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_investment_holdings_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      798 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_investment_holdings_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1173 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_investment_holdings_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     2009 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_investment_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      814 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_investment_transactions_request_options.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1613 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_investment_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      677 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_liabilities_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1012 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/get_liabilities_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1356 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/migrate_financial_connections_aggregator_connection_data.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      978 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/migrate_financial_connections_aggregator_connection_data_mx.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      817 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/migrate_financial_connections_aggregator_connection_data_plaid.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1577 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/migrate_financial_connections_token_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      768 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/migrate_financial_connections_token_request_entity.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1490 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/migrate_financial_connections_token_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      513 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/product.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1286 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/refresh_asset_report_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      916 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/sync_financial_connections_data_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      951 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/sync_transactions_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1670 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/sync_transactions_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      780 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/sync_transactions_response_removed_inner.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1770 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/transaction.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      672 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/transaction_merchant.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1069 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/update_entity_request.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1339 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/update_entity_response.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     1388 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/webhook_event.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      531 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/webhook_source.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/models/webhook_type.py
--rw-r--r--   0 adibpournazari   (501) staff       (20)     8155 2023-04-06 23:42:55.000000 fuse_client-1.0.0/src/openapi_server/security_api.py
-drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-07 09:35:50.895117 fuse_client-1.0.0/tests/
--rw-r--r--   0 adibpournazari   (501) staff       (20)    18025 2023-04-06 23:42:55.000000 fuse_client-1.0.0/tests/test_fuse_api.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-10 09:07:11.817603 fuse_client-1.0.5/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1067 2023-04-06 23:42:07.000000 fuse_client-1.0.5/LICENSE
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1158 2023-04-10 09:07:11.817671 fuse_client-1.0.5/PKG-INFO
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      796 2023-04-06 23:42:55.000000 fuse_client-1.0.5/README.md
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      577 2023-04-06 23:42:55.000000 fuse_client-1.0.5/pyproject.toml
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      573 2023-04-10 09:07:11.817983 fuse_client-1.0.5/setup.cfg
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-10 09:07:11.796019 fuse_client-1.0.5/src/
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-10 09:07:11.797143 fuse_client-1.0.5/src/fuse_client/
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-10 09:07:11.798030 fuse_client-1.0.5/src/fuse_client/apis/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/apis/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    16910 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/apis/fuse_api.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      554 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/main.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-10 09:07:11.817196 fuse_client-1.0.5/src/fuse_client/models/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        0 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/__init__.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      534 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/account_subtype.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/account_type.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      522 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/aggregator.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/country_code.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1245 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1078 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1181 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1336 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1583 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/models/create_link_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      711 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_link_token_request_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      723 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_link_token_request_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      793 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_link_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1814 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_session_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      909 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/create_session_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      705 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/models/currency.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1029 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/delete_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      801 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/entity.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      812 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/exchange_financial_connections_public_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1113 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/exchange_financial_connections_public_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      125 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/extra_models.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      777 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2052 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connection_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      818 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connection_details_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      829 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connection_details_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      858 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connection_details_teller.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1984 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1441 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1328 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_cached_balance.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      961 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_details.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1255 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_details_ach.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      748 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_institution.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     3676 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_liability.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2243 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_liability_all_of.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      983 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_liability_all_of_aprs.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1468 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_holding.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2210 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_investment_security.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      796 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_investment_security_exchange.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2196 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_investment_transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1628 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1072 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_addresses_inner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1412 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_addresses_inner_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      998 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_emails_inner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      840 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_names_inner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1034 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_phone_numbers_inner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1281 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_institution.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      890 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/financial_institution_logo.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1329 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/fuse_api_error.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      946 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/fuse_api_error_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1353 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/fuse_api_warning.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1024 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/fuse_api_warning_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1284 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/fuse_api_warning_data_warnings_inner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      701 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      960 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1817 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response_report.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1865 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response_report_accounts_inner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1186 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response_report_accounts_inner_balances.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1254 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response_report_accounts_inner_historical_balances_inner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1512 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      978 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connection_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      769 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_account_details_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1343 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_account_details_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      745 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_accounts_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1257 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_accounts_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1061 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_balance_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      834 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_balance_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1001 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_balance_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      737 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_owners_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      917 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_owners_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1196 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_owners_response_accounts_inner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1647 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1140 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      968 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_financial_institution_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      988 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_investment_holdings_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      798 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_investment_holdings_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1167 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_investment_holdings_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     2006 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_investment_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      814 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_investment_transactions_request_options.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1294 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/models/get_investment_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      677 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_liabilities_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1009 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/get_liabilities_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1350 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_aggregator_connection_data.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      978 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_aggregator_connection_data_mx.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      817 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_aggregator_connection_data_plaid.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1568 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_token_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      768 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_token_request_entity.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1487 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_token_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      513 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/product.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1286 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/refresh_asset_report_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      916 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/sync_financial_connections_data_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      951 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/sync_transactions_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1664 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/sync_transactions_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      780 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/sync_transactions_response_removed_inner.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1767 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/transaction.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      672 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/transaction_merchant.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1066 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/update_entity_request.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1336 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/update_entity_response.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1382 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/webhook_event.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      531 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/webhook_source.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)      525 2023-04-06 23:42:55.000000 fuse_client-1.0.5/src/fuse_client/models/webhook_type.py
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     8152 2023-04-10 09:05:42.000000 fuse_client-1.0.5/src/fuse_client/security_api.py
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-10 09:07:11.797838 fuse_client-1.0.5/src/fuse_client.egg-info/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     1158 2023-04-10 09:07:11.000000 fuse_client-1.0.5/src/fuse_client.egg-info/PKG-INFO
+-rw-r--r--   0 adibpournazari   (501) staff       (20)     6380 2023-04-10 09:07:11.000000 fuse_client-1.0.5/src/fuse_client.egg-info/SOURCES.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)        1 2023-04-10 09:07:11.000000 fuse_client-1.0.5/src/fuse_client.egg-info/dependency_links.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)       13 2023-04-10 09:07:11.000000 fuse_client-1.0.5/src/fuse_client.egg-info/requires.txt
+-rw-r--r--   0 adibpournazari   (501) staff       (20)       12 2023-04-10 09:07:11.000000 fuse_client-1.0.5/src/fuse_client.egg-info/top_level.txt
+drwxr-xr-x   0 adibpournazari   (501) staff       (20)        0 2023-04-10 09:07:11.817386 fuse_client-1.0.5/tests/
+-rw-r--r--   0 adibpournazari   (501) staff       (20)    16557 2023-04-10 09:05:42.000000 fuse_client-1.0.5/tests/test_fuse_api.py
```

### Comparing `fuse_client-1.0.0/LICENSE` & `fuse_client-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/PKG-INFO` & `fuse_client-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuse_client
-Version: 1.0.0
+Version: 1.0.5
 Summary: No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 Keywords: OpenAPI Fuse
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
```

### Comparing `fuse_client-1.0.0/README.md` & `fuse_client-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/pyproject.toml` & `fuse_client-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/setup.cfg` & `fuse_client-1.0.5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fuse_client
-version = 1.0.0
+version = 1.0.5
 description = No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 long_description = file: README.md
 keywords = OpenAPI Fuse
 python_requires = >= 3.7.*
 classifiers = 
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
```

### Comparing `fuse_client-1.0.0/src/3/4/5/apis/fuse_api.py` & `fuse_client-1.0.5/src/fuse_client/apis/fuse_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,54 +12,50 @@
     Path,
     Query,
     Response,
     Security,
     status,
 )
 
-from 3.4.5.models.extra_models import TokenModel  # noqa: F401
-from 3.4.5.models.create_asset_report_request import CreateAssetReportRequest
-from 3.4.5.models.create_asset_report_response import CreateAssetReportResponse
-from 3.4.5.models.create_entity_request import CreateEntityRequest
-from 3.4.5.models.create_entity_response import CreateEntityResponse
-from 3.4.5.models.create_link_token_request import CreateLinkTokenRequest
-from 3.4.5.models.create_link_token_response import CreateLinkTokenResponse
-from 3.4.5.models.create_session_request import CreateSessionRequest
-from 3.4.5.models.create_session_response import CreateSessionResponse
-from 3.4.5.models.delete_financial_connection_response import DeleteFinancialConnectionResponse
-from 3.4.5.models.exchange_financial_connections_public_token_request import ExchangeFinancialConnectionsPublicTokenRequest
-from 3.4.5.models.exchange_financial_connections_public_token_response import ExchangeFinancialConnectionsPublicTokenResponse
-from 3.4.5.models.get_asset_report_request import GetAssetReportRequest
-from 3.4.5.models.get_asset_report_response import GetAssetReportResponse
-from 3.4.5.models.get_entity_response import GetEntityResponse
-from 3.4.5.models.get_financial_connection_response import GetFinancialConnectionResponse
-from 3.4.5.models.get_financial_connections_account_details_request import GetFinancialConnectionsAccountDetailsRequest
-from 3.4.5.models.get_financial_connections_account_details_response import GetFinancialConnectionsAccountDetailsResponse
-from 3.4.5.models.get_financial_connections_accounts_request import GetFinancialConnectionsAccountsRequest
-from 3.4.5.models.get_financial_connections_accounts_response import GetFinancialConnectionsAccountsResponse
-from 3.4.5.models.get_financial_connections_balance_request import GetFinancialConnectionsBalanceRequest
-from 3.4.5.models.get_financial_connections_balance_response import GetFinancialConnectionsBalanceResponse
-from 3.4.5.models.get_financial_connections_owners_request import GetFinancialConnectionsOwnersRequest
-from 3.4.5.models.get_financial_connections_owners_response import GetFinancialConnectionsOwnersResponse
-from 3.4.5.models.get_financial_connections_transactions_request import GetFinancialConnectionsTransactionsRequest
-from 3.4.5.models.get_financial_connections_transactions_response import GetFinancialConnectionsTransactionsResponse
-from 3.4.5.models.get_financial_institution_response import GetFinancialInstitutionResponse
-from 3.4.5.models.get_investment_holdings_request import GetInvestmentHoldingsRequest
-from 3.4.5.models.get_investment_holdings_response import GetInvestmentHoldingsResponse
-from 3.4.5.models.get_investment_transactions_request import GetInvestmentTransactionsRequest
-from 3.4.5.models.get_investment_transactions_response import GetInvestmentTransactionsResponse
-from 3.4.5.models.get_liabilities_request import GetLiabilitiesRequest
-from 3.4.5.models.get_liabilities_response import GetLiabilitiesResponse
-from 3.4.5.models.refresh_asset_report_request import RefreshAssetReportRequest
-from 3.4.5.models.sync_financial_connections_data_response import SyncFinancialConnectionsDataResponse
-from 3.4.5.models.sync_transactions_request import SyncTransactionsRequest
-from 3.4.5.models.sync_transactions_response import SyncTransactionsResponse
-from 3.4.5.models.update_entity_request import UpdateEntityRequest
-from 3.4.5.models.update_entity_response import UpdateEntityResponse
-from 3.4.5.security_api import get_token_fuseApiKey, get_token_fuseClientId
+from fuse_client.models.extra_models import TokenModel  # noqa: F401
+from fuse_client.models.create_asset_report_request import CreateAssetReportRequest
+from fuse_client.models.create_asset_report_response import CreateAssetReportResponse
+from fuse_client.models.create_link_token_request import CreateLinkTokenRequest
+from fuse_client.models.create_link_token_response import CreateLinkTokenResponse
+from fuse_client.models.create_session_request import CreateSessionRequest
+from fuse_client.models.create_session_response import CreateSessionResponse
+from fuse_client.models.delete_financial_connection_response import DeleteFinancialConnectionResponse
+from fuse_client.models.exchange_financial_connections_public_token_request import ExchangeFinancialConnectionsPublicTokenRequest
+from fuse_client.models.exchange_financial_connections_public_token_response import ExchangeFinancialConnectionsPublicTokenResponse
+from fuse_client.models.get_asset_report_request import GetAssetReportRequest
+from fuse_client.models.get_asset_report_response import GetAssetReportResponse
+from fuse_client.models.get_entity_response import GetEntityResponse
+from fuse_client.models.get_financial_connection_response import GetFinancialConnectionResponse
+from fuse_client.models.get_financial_connections_account_details_request import GetFinancialConnectionsAccountDetailsRequest
+from fuse_client.models.get_financial_connections_account_details_response import GetFinancialConnectionsAccountDetailsResponse
+from fuse_client.models.get_financial_connections_accounts_request import GetFinancialConnectionsAccountsRequest
+from fuse_client.models.get_financial_connections_accounts_response import GetFinancialConnectionsAccountsResponse
+from fuse_client.models.get_financial_connections_balance_request import GetFinancialConnectionsBalanceRequest
+from fuse_client.models.get_financial_connections_balance_response import GetFinancialConnectionsBalanceResponse
+from fuse_client.models.get_financial_connections_owners_request import GetFinancialConnectionsOwnersRequest
+from fuse_client.models.get_financial_connections_owners_response import GetFinancialConnectionsOwnersResponse
+from fuse_client.models.get_financial_connections_transactions_request import GetFinancialConnectionsTransactionsRequest
+from fuse_client.models.get_financial_connections_transactions_response import GetFinancialConnectionsTransactionsResponse
+from fuse_client.models.get_financial_institution_response import GetFinancialInstitutionResponse
+from fuse_client.models.get_investment_holdings_request import GetInvestmentHoldingsRequest
+from fuse_client.models.get_investment_holdings_response import GetInvestmentHoldingsResponse
+from fuse_client.models.get_investment_transactions_request import GetInvestmentTransactionsRequest
+from fuse_client.models.get_investment_transactions_response import GetInvestmentTransactionsResponse
+from fuse_client.models.get_liabilities_request import GetLiabilitiesRequest
+from fuse_client.models.get_liabilities_response import GetLiabilitiesResponse
+from fuse_client.models.migrate_financial_connections_token_request import MigrateFinancialConnectionsTokenRequest
+from fuse_client.models.migrate_financial_connections_token_response import MigrateFinancialConnectionsTokenResponse
+from fuse_client.models.refresh_asset_report_request import RefreshAssetReportRequest
+from fuse_client.models.sync_financial_connections_data_response import SyncFinancialConnectionsDataResponse
+from fuse_client.security_api import get_token_fuseApiKey, get_token_fuseClientId
 
 router = APIRouter()
 
 
 @router.post(
     "/v1/asset_report/create",
     responses={
@@ -78,35 +74,14 @@
     ),
 ) -> CreateAssetReportResponse:
     """Use this endpoint to generate an Asset Report for a user."""
     ...
 
 
 @router.post(
-    "/v1/entities",
-    responses={
-        200: {"model": CreateEntityResponse, "description": "Success"},
-    },
-    tags=["Fuse"],
-    summary="Create entity",
-    response_model_by_alias=True,
-)
-async def create_entity(
-    create_entity_request: CreateEntityRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> CreateEntityResponse:
-    ...
-
-
-@router.post(
     "/v1/link/token",
     responses={
         200: {"model": CreateLinkTokenResponse, "description": "Response"},
     },
     tags=["Fuse"],
     response_model_by_alias=True,
 )
@@ -221,14 +196,15 @@
     token_fuseApiKey: TokenModel = Security(
         get_token_fuseApiKey
     ),
     token_fuseClientId: TokenModel = Security(
         get_token_fuseClientId
     ),
 ) -> GetEntityResponse:
+    """An entity is automatically created after a successful connection. The id of the entity is what is set when calling the &#39;create session&#39; endpoint"""
     ...
 
 
 @router.get(
     "/v1/financial_connections/{financial_connection_id}",
     responses={
         200: {"model": GetFinancialConnectionResponse, "description": "Success"},
@@ -415,96 +391,75 @@
         get_token_fuseClientId
     ),
 ) -> GetInvestmentTransactionsResponse:
     ...
 
 
 @router.post(
-    "/v1/asset_report/refresh",
+    "/v1/financial_connections/migrate",
     responses={
-        200: {"model": CreateAssetReportResponse, "description": "Response"},
+        200: {"model": MigrateFinancialConnectionsTokenResponse, "description": "Success"},
     },
     tags=["Fuse"],
+    summary="Migrate financial connection",
     response_model_by_alias=True,
 )
-async def refresh_asset_report(
-    refresh_asset_report_request: RefreshAssetReportRequest = Body(None, description=""),
+async def migrate_financial_connection(
+    migrate_financial_connections_token_request: MigrateFinancialConnectionsTokenRequest = Body(None, description=""),
     token_fuseApiKey: TokenModel = Security(
         get_token_fuseApiKey
     ),
     token_fuseClientId: TokenModel = Security(
         get_token_fuseClientId
     ),
-) -> CreateAssetReportResponse:
-    """Refreshes the Asset Report in JSON format."""
+) -> MigrateFinancialConnectionsTokenResponse:
+    """This endpoint migrates financial connections from Plaid or MX into the unified Fuse API. It accepts a POST request with connection data, aggregator, entity, and Fuse products, and responds with a JSON payload containing the migrated connection&#39;s data, access token, ID, and request ID."""
     ...
 
 
 @router.post(
-    "/v1/financial_connections/sync",
+    "/v1/asset_report/refresh",
     responses={
-        200: {"model": SyncFinancialConnectionsDataResponse, "description": "Successfully synchronized transactions"},
+        200: {"model": CreateAssetReportResponse, "description": "Response"},
     },
     tags=["Fuse"],
-    summary="Sync financial connections data",
     response_model_by_alias=True,
 )
-async def sync_financial_connections_data(
-    body:  = Body(None, description=""),
+async def refresh_asset_report(
+    refresh_asset_report_request: RefreshAssetReportRequest = Body(None, description=""),
     token_fuseApiKey: TokenModel = Security(
         get_token_fuseApiKey
     ),
     token_fuseClientId: TokenModel = Security(
         get_token_fuseClientId
     ),
-) -> SyncFinancialConnectionsDataResponse:
-    """Call this endpoint upon receiving a SYNC_REQUIRED webhook. This will keep the financial connections data up to date."""
+) -> CreateAssetReportResponse:
+    """Refreshes the Asset Report in JSON format."""
     ...
 
 
 @router.post(
-    "/v1/financial_connections/transactions/sync",
-    responses={
-        200: {"model": SyncTransactionsResponse, "description": "Successfully synchronized transactions"},
-    },
-    tags=["Fuse"],
-    summary="Sync transactions",
-    response_model_by_alias=True,
-)
-async def sync_financial_connections_transactions(
-    sync_transactions_request: SyncTransactionsRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> SyncTransactionsResponse:
-    ...
-
-
-@router.put(
-    "/v1/entities/{entity_id_to_update}",
+    "/v1/financial_connections/sync",
     responses={
-        200: {"model": UpdateEntityResponse, "description": "Success"},
+        200: {"model": SyncFinancialConnectionsDataResponse, "description": "Successfully synchronized transactions"},
     },
     tags=["Fuse"],
-    summary="Update entity",
+    summary="Sync financial connections data",
     response_model_by_alias=True,
 )
-async def update_entity(
-    entity_id_to_update: str = Path(None, description=""),
-    update_entity_request: UpdateEntityRequest = Body(None, description=""),
+async def sync_financial_connections_data(
+    body:  = Body(None, description=""),
     token_fuseApiKey: TokenModel = Security(
         get_token_fuseApiKey
     ),
     token_fuseClientId: TokenModel = Security(
         get_token_fuseClientId
     ),
-) -> UpdateEntityResponse:
+) -> SyncFinancialConnectionsDataResponse:
+    """Call this endpoint upon receiving a financial_connection.sync_data webhook. This will keep the financial connections data up to date."""
     ...
 
 
 @router.post(
     "/v1/financial_connections/liabilities",
     responses={
         200: {"model": GetLiabilitiesResponse, "description": "Successful response"},
```

### Comparing `fuse_client-1.0.0/src/3/4/5/main.py` & `fuse_client-1.0.5/src/fuse_client/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 """
     Fuse
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.0.5
     Generated by: https://openapi-generator.tech
 """
 
 
 from fastapi import FastAPI
 
-from 3.4.5.apis.fuse_api import router as FuseApiRouter
+from fuse_client.apis.fuse_api import router as FuseApiRouter
 
 app = FastAPI(
     title="Fuse",
     description="No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)",
-    version="1.0.0",
+    version="1.0.5",
 )
 
 app.include_router(FuseApiRouter)
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/account_subtype.py` & `fuse_client-1.0.5/src/fuse_client/models/account_subtype.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/account_type.py` & `fuse_client-1.0.5/src/fuse_client/models/account_type.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/aggregator.py` & `fuse_client-1.0.5/src/fuse_client/models/aggregator.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/country_code.py` & `fuse_client-1.0.5/src/fuse_client/models/country_code.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/create_asset_report_request.py` & `fuse_client-1.0.5/src/fuse_client/models/create_asset_report_request.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/create_asset_report_response.py` & `fuse_client-1.0.5/src/fuse_client/models/create_asset_report_response.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/create_entity_request.py` & `fuse_client-1.0.5/src/fuse_client/models/create_entity_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.aggregator import Aggregator
+from fuse_client.models.aggregator import Aggregator
 
 
 class CreateEntityRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/create_entity_response.py` & `fuse_client-1.0.5/src/fuse_client/models/create_entity_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.aggregator import Aggregator
+from fuse_client.models.aggregator import Aggregator
 
 
 class CreateEntityResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/create_link_token_request.py` & `fuse_client-1.0.5/src/fuse_client/models/create_link_token_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,37 +3,35 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.create_link_token_request_mx import CreateLinkTokenRequestMx
-from 3.4.5.models.create_link_token_request_plaid import CreateLinkTokenRequestPlaid
-from 3.4.5.models.entity import Entity
+from fuse_client.models.create_link_token_request_mx import CreateLinkTokenRequestMx
+from fuse_client.models.create_link_token_request_plaid import CreateLinkTokenRequestPlaid
+from fuse_client.models.entity import Entity
 
 
 class CreateLinkTokenRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
     CreateLinkTokenRequest - a model defined in OpenAPI
 
         institution_id: The institution_id of this CreateLinkTokenRequest.
         entity: The entity of this CreateLinkTokenRequest.
-        reconnection_url: The reconnection_url of this CreateLinkTokenRequest [Optional].
         client_name: The client_name of this CreateLinkTokenRequest.
         session_client_secret: The session_client_secret of this CreateLinkTokenRequest.
         mx: The mx of this CreateLinkTokenRequest [Optional].
         plaid: The plaid of this CreateLinkTokenRequest [Optional].
     """
 
     institution_id: str = Field(alias="institution_id")
     entity: Entity = Field(alias="entity")
-    reconnection_url: Optional[str] = Field(alias="reconnection_url", default=None)
     client_name: str = Field(alias="client_name")
     session_client_secret: str = Field(alias="session_client_secret")
     mx: Optional[CreateLinkTokenRequestMx] = Field(alias="mx", default=None)
     plaid: Optional[CreateLinkTokenRequestPlaid] = Field(alias="plaid", default=None)
 
 CreateLinkTokenRequest.update_forward_refs()
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/create_link_token_request_mx.py` & `fuse_client-1.0.5/src/fuse_client/models/create_link_token_request_mx.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/create_link_token_request_plaid.py` & `fuse_client-1.0.5/src/fuse_client/models/create_link_token_request_plaid.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/create_link_token_response.py` & `fuse_client-1.0.5/src/fuse_client/models/create_link_token_response.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/create_session_request.py` & `fuse_client-1.0.5/src/fuse_client/models/create_session_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.aggregator import Aggregator
-from 3.4.5.models.country_code import CountryCode
-from 3.4.5.models.entity import Entity
-from 3.4.5.models.product import Product
+from fuse_client.models.aggregator import Aggregator
+from fuse_client.models.country_code import CountryCode
+from fuse_client.models.entity import Entity
+from fuse_client.models.product import Product
 
 
 class CreateSessionRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/create_session_response.py` & `fuse_client-1.0.5/src/fuse_client/models/create_session_response.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/delete_financial_connection_response.py` & `fuse_client-1.0.5/src/fuse_client/models/delete_financial_connection_response.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/entity.py` & `fuse_client-1.0.5/src/fuse_client/models/entity.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/exchange_financial_connections_public_token_request.py` & `fuse_client-1.0.5/src/fuse_client/models/exchange_financial_connections_public_token_request.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/exchange_financial_connections_public_token_response.py` & `fuse_client-1.0.5/src/fuse_client/models/exchange_financial_connections_public_token_response.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connection_data.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connection_data.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connection_details.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connection_details.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.aggregator import Aggregator
-from 3.4.5.models.financial_connection_details_mx import FinancialConnectionDetailsMx
-from 3.4.5.models.financial_connection_details_plaid import FinancialConnectionDetailsPlaid
-from 3.4.5.models.financial_connection_details_teller import FinancialConnectionDetailsTeller
+from fuse_client.models.aggregator import Aggregator
+from fuse_client.models.financial_connection_details_mx import FinancialConnectionDetailsMx
+from fuse_client.models.financial_connection_details_plaid import FinancialConnectionDetailsPlaid
+from fuse_client.models.financial_connection_details_teller import FinancialConnectionDetailsTeller
 
 
 class FinancialConnectionDetails(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connection_details_mx.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connection_details_mx.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connection_details_plaid.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connection_details_plaid.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connection_details_teller.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connection_details_teller.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_account.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_account.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.account_subtype import AccountSubtype
-from 3.4.5.models.account_type import AccountType
-from 3.4.5.models.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
-from 3.4.5.models.financial_connections_account_institution import FinancialConnectionsAccountInstitution
+from fuse_client.models.account_subtype import AccountSubtype
+from fuse_client.models.account_type import AccountType
+from fuse_client.models.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
+from fuse_client.models.financial_connections_account_institution import FinancialConnectionsAccountInstitution
 
 
 class FinancialConnectionsAccount(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_balance.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_balance.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_cached_balance.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_cached_balance.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_details.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connections_account_details_ach import FinancialConnectionsAccountDetailsAch
+from fuse_client.models.financial_connections_account_details_ach import FinancialConnectionsAccountDetailsAch
 
 
 class FinancialConnectionsAccountDetails(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_details_ach.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_details_ach.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_institution.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_institution.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_liability.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_liability.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.account_subtype import AccountSubtype
-from 3.4.5.models.account_type import AccountType
-from 3.4.5.models.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
-from 3.4.5.models.financial_connections_account_institution import FinancialConnectionsAccountInstitution
-from 3.4.5.models.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
+from fuse_client.models.account_subtype import AccountSubtype
+from fuse_client.models.account_type import AccountType
+from fuse_client.models.financial_connections_account_cached_balance import FinancialConnectionsAccountCachedBalance
+from fuse_client.models.financial_connections_account_institution import FinancialConnectionsAccountInstitution
+from fuse_client.models.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
 
 
 class FinancialConnectionsAccountLiability(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_liability_all_of.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_liability_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
+from fuse_client.models.financial_connections_account_liability_all_of_aprs import FinancialConnectionsAccountLiabilityAllOfAprs
 
 
 class FinancialConnectionsAccountLiabilityAllOf(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_account_liability_all_of_aprs.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_account_liability_all_of_aprs.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_holding.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_holding.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
+from fuse_client.models.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
 
 
 class FinancialConnectionsHolding(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_investment_security.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_investment_security.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connections_investment_security_currency import FinancialConnectionsInvestmentSecurityCurrency
-from 3.4.5.models.financial_connections_investment_security_exchange import FinancialConnectionsInvestmentSecurityExchange
+from fuse_client.models.currency import Currency
+from fuse_client.models.financial_connections_investment_security_exchange import FinancialConnectionsInvestmentSecurityExchange
 
 
 class FinancialConnectionsInvestmentSecurity(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
@@ -32,13 +32,13 @@
 
     remote_id: str = Field(alias="remote_id")
     symbol: str = Field(alias="symbol")
     isin: Optional[str] = Field(alias="isin", default=None)
     sedol: Optional[str] = Field(alias="sedol", default=None)
     cusip: Optional[str] = Field(alias="cusip", default=None)
     close_price: float = Field(alias="close_price")
-    currency: FinancialConnectionsInvestmentSecurityCurrency = Field(alias="currency")
+    currency: Currency = Field(alias="currency")
     name: Optional[str] = Field(alias="name", default=None)
     type: Optional[str] = Field(alias="type", default=None)
     exchange: Optional[FinancialConnectionsInvestmentSecurityExchange] = Field(alias="exchange", default=None)
 
 FinancialConnectionsInvestmentSecurity.update_forward_refs()
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_investment_security_currency.py` & `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_balance_request_options.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
 
-class FinancialConnectionsInvestmentSecurityCurrency(BaseModel):
+class GetFinancialConnectionsBalanceRequestOptions(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    FinancialConnectionsInvestmentSecurityCurrency - a model defined in OpenAPI
+    GetFinancialConnectionsBalanceRequestOptions - a model defined in OpenAPI
 
-        code: The code of this FinancialConnectionsInvestmentSecurityCurrency [Optional].
+        remote_account_ids: The remote_account_ids of this GetFinancialConnectionsBalanceRequestOptions [Optional].
     """
 
-    code: Optional[str] = Field(alias="code", default=None)
+    remote_account_ids: Optional[List[str]] = Field(alias="remote_account_ids", default=None)
 
-FinancialConnectionsInvestmentSecurityCurrency.update_forward_refs()
+GetFinancialConnectionsBalanceRequestOptions.update_forward_refs()
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_investment_security_exchange.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_investment_security_exchange.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_investment_transaction.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_investment_transaction.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,44 +3,41 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
-from 3.4.5.models.financial_connections_investment_transaction_currency import FinancialConnectionsInvestmentTransactionCurrency
+from fuse_client.models.financial_connections_investment_security import FinancialConnectionsInvestmentSecurity
 
 
 class FinancialConnectionsInvestmentTransaction(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
     FinancialConnectionsInvestmentTransaction - a model defined in OpenAPI
 
         remote_id: The remote_id of this FinancialConnectionsInvestmentTransaction.
         remote_account_id: The remote_account_id of this FinancialConnectionsInvestmentTransaction.
         account_name: The account_name of this FinancialConnectionsInvestmentTransaction [Optional].
         amount: The amount of this FinancialConnectionsInvestmentTransaction.
-        currency: The currency of this FinancialConnectionsInvestmentTransaction.
         description: The description of this FinancialConnectionsInvestmentTransaction.
         fees: The fees of this FinancialConnectionsInvestmentTransaction.
         date: The date of this FinancialConnectionsInvestmentTransaction.
         type: The type of this FinancialConnectionsInvestmentTransaction.
         quantity: The quantity of this FinancialConnectionsInvestmentTransaction.
         price: The price of this FinancialConnectionsInvestmentTransaction.
         security: The security of this FinancialConnectionsInvestmentTransaction.
     """
 
     remote_id: str = Field(alias="remote_id")
     remote_account_id: str = Field(alias="remote_account_id")
     account_name: Optional[str] = Field(alias="account_name", default=None)
     amount: float = Field(alias="amount")
-    currency: FinancialConnectionsInvestmentTransactionCurrency = Field(alias="currency")
     description: str = Field(alias="description")
     fees: float = Field(alias="fees")
     date: datetime = Field(alias="date")
     type: str = Field(alias="type")
     quantity: float = Field(alias="quantity")
     price: float = Field(alias="price")
     security: FinancialConnectionsInvestmentSecurity = Field(alias="security")
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_investment_transaction_currency.py` & `fuse_client-1.0.5/src/fuse_client/models/get_financial_connection_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
+from fuse_client.models.financial_connection_details import FinancialConnectionDetails
 
 
-class FinancialConnectionsInvestmentTransactionCurrency(BaseModel):
+class GetFinancialConnectionResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    FinancialConnectionsInvestmentTransactionCurrency - a model defined in OpenAPI
+    GetFinancialConnectionResponse - a model defined in OpenAPI
 
-        code: The code of this FinancialConnectionsInvestmentTransactionCurrency.
-        name: The name of this FinancialConnectionsInvestmentTransactionCurrency [Optional].
+        financial_connection: The financial_connection of this GetFinancialConnectionResponse.
+        request_id: The request_id of this GetFinancialConnectionResponse.
     """
 
-    code: str = Field(alias="code")
-    name: Optional[str] = Field(alias="name", default=None)
+    financial_connection: FinancialConnectionDetails = Field(alias="financial_connection")
+    request_id: str = Field(alias="request_id")
 
-FinancialConnectionsInvestmentTransactionCurrency.update_forward_refs()
+GetFinancialConnectionResponse.update_forward_refs()
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_owner.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connections_owner_addresses_inner import FinancialConnectionsOwnerAddressesInner
-from 3.4.5.models.financial_connections_owner_emails_inner import FinancialConnectionsOwnerEmailsInner
-from 3.4.5.models.financial_connections_owner_names_inner import FinancialConnectionsOwnerNamesInner
-from 3.4.5.models.financial_connections_owner_phone_numbers_inner import FinancialConnectionsOwnerPhoneNumbersInner
+from fuse_client.models.financial_connections_owner_addresses_inner import FinancialConnectionsOwnerAddressesInner
+from fuse_client.models.financial_connections_owner_emails_inner import FinancialConnectionsOwnerEmailsInner
+from fuse_client.models.financial_connections_owner_names_inner import FinancialConnectionsOwnerNamesInner
+from fuse_client.models.financial_connections_owner_phone_numbers_inner import FinancialConnectionsOwnerPhoneNumbersInner
 
 
 class FinancialConnectionsOwner(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_owner_addresses_inner.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_addresses_inner.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connections_owner_addresses_inner_data import FinancialConnectionsOwnerAddressesInnerData
+from fuse_client.models.financial_connections_owner_addresses_inner_data import FinancialConnectionsOwnerAddressesInnerData
 
 
 class FinancialConnectionsOwnerAddressesInner(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_owner_addresses_inner_data.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_addresses_inner_data.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_owner_emails_inner.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_emails_inner.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_owner_names_inner.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_names_inner.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_connections_owner_phone_numbers_inner.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_connections_owner_phone_numbers_inner.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_institution.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_institution.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.country_code import CountryCode
-from 3.4.5.models.financial_institution_logo import FinancialInstitutionLogo
+from fuse_client.models.country_code import CountryCode
+from fuse_client.models.financial_institution_logo import FinancialInstitutionLogo
 
 
 class FinancialInstitution(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/financial_institution_logo.py` & `fuse_client-1.0.5/src/fuse_client/models/financial_institution_logo.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/fuse_api_error.py` & `fuse_client-1.0.5/src/fuse_client/models/fuse_api_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.fuse_api_error_data import FuseApiErrorData
+from fuse_client.models.fuse_api_error_data import FuseApiErrorData
 
 
 class FuseApiError(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/fuse_api_error_data.py` & `fuse_client-1.0.5/src/fuse_client/models/fuse_api_warning_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.aggregator import Aggregator
-from 3.4.5.models.fuse_api_error import FuseApiError
+from fuse_client.models.aggregator import Aggregator
+from fuse_client.models.fuse_api_warning_data_warnings_inner import FuseApiWarningDataWarningsInner
 
 
-class FuseApiErrorData(BaseModel):
+class FuseApiWarningData(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    FuseApiErrorData - a model defined in OpenAPI
+    FuseApiWarningData - a model defined in OpenAPI
 
-        aggregator: The aggregator of this FuseApiErrorData [Optional].
-        errors: The errors of this FuseApiErrorData [Optional].
+        aggregator: The aggregator of this FuseApiWarningData [Optional].
+        warnings: The warnings of this FuseApiWarningData [Optional].
     """
 
     aggregator: Optional[Aggregator] = Field(alias="aggregator", default=None)
-    errors: Optional[List[FuseApiError]] = Field(alias="errors", default=None)
+    warnings: Optional[List[FuseApiWarningDataWarningsInner]] = Field(alias="warnings", default=None)
 
-FuseApiErrorData.update_forward_refs()
+FuseApiWarningData.update_forward_refs()
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/fuse_api_warning.py` & `fuse_client-1.0.5/src/fuse_client/models/fuse_api_warning.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.fuse_api_warning_data import FuseApiWarningData
+from fuse_client.models.fuse_api_warning_data import FuseApiWarningData
 
 
 class FuseApiWarning(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/fuse_api_warning_data.py` & `fuse_client-1.0.5/src/fuse_client/models/update_entity_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.aggregator import Aggregator
-from 3.4.5.models.fuse_api_warning_data_warnings_inner import FuseApiWarningDataWarningsInner
+from fuse_client.models.aggregator import Aggregator
 
 
-class FuseApiWarningData(BaseModel):
+class UpdateEntityRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    FuseApiWarningData - a model defined in OpenAPI
+    UpdateEntityRequest - a model defined in OpenAPI
 
-        aggregator: The aggregator of this FuseApiWarningData [Optional].
-        warnings: The warnings of this FuseApiWarningData [Optional].
+        email: The email of this UpdateEntityRequest [Optional].
+        aggregators: The aggregators of this UpdateEntityRequest [Optional].
+        institution_ids: The institution_ids of this UpdateEntityRequest [Optional].
     """
 
-    aggregator: Optional[Aggregator] = Field(alias="aggregator", default=None)
-    warnings: Optional[List[FuseApiWarningDataWarningsInner]] = Field(alias="warnings", default=None)
+    email: Optional[str] = Field(alias="email", default=None)
+    aggregators: Optional[List[Aggregator]] = Field(alias="aggregators", default=None)
+    institution_ids: Optional[List[str]] = Field(alias="institution_ids", default=None)
 
-FuseApiWarningData.update_forward_refs()
+UpdateEntityRequest.update_forward_refs()
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/fuse_api_warning_data_warnings_inner.py` & `fuse_client-1.0.5/src/fuse_client/models/fuse_api_warning_data_warnings_inner.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_asset_report_request.py` & `fuse_client-1.0.5/src/fuse_client/models/get_asset_report_request.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_asset_report_response.py` & `fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.get_asset_report_response_report import GetAssetReportResponseReport
+from fuse_client.models.get_asset_report_response_report import GetAssetReportResponseReport
 
 
 class GetAssetReportResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_asset_report_response_report.py` & `fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.fuse_api_warning import FuseApiWarning
-from 3.4.5.models.get_asset_report_response_report_accounts_inner import GetAssetReportResponseReportAccountsInner
+from fuse_client.models.fuse_api_warning import FuseApiWarning
+from fuse_client.models.get_asset_report_response_report_accounts_inner import GetAssetReportResponseReportAccountsInner
 
 
 class GetAssetReportResponseReport(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_asset_report_response_report_accounts_inner.py` & `fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response_report_accounts_inner.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connections_owner import FinancialConnectionsOwner
-from 3.4.5.models.get_asset_report_response_report_accounts_inner_balances import GetAssetReportResponseReportAccountsInnerBalances
-from 3.4.5.models.get_asset_report_response_report_accounts_inner_historical_balances_inner import GetAssetReportResponseReportAccountsInnerHistoricalBalancesInner
+from fuse_client.models.financial_connections_owner import FinancialConnectionsOwner
+from fuse_client.models.get_asset_report_response_report_accounts_inner_balances import GetAssetReportResponseReportAccountsInnerBalances
+from fuse_client.models.get_asset_report_response_report_accounts_inner_historical_balances_inner import GetAssetReportResponseReportAccountsInnerHistoricalBalancesInner
 
 
 class GetAssetReportResponseReportAccountsInner(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_asset_report_response_report_accounts_inner_balances.py` & `fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response_report_accounts_inner_balances.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_asset_report_response_report_accounts_inner_historical_balances_inner.py` & `fuse_client-1.0.5/src/fuse_client/models/get_asset_report_response_report_accounts_inner_historical_balances_inner.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_entity_response.py` & `fuse_client-1.0.5/src/fuse_client/models/get_entity_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.aggregator import Aggregator
-from 3.4.5.models.financial_connection_details import FinancialConnectionDetails
+from fuse_client.models.aggregator import Aggregator
+from fuse_client.models.financial_connection_details import FinancialConnectionDetails
 
 
 class GetEntityResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_financial_connection_response.py` & `fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_aggregator_connection_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connection_details import FinancialConnectionDetails
+from fuse_client.models.migrate_financial_connections_aggregator_connection_data_mx import MigrateFinancialConnectionsAggregatorConnectionDataMx
+from fuse_client.models.migrate_financial_connections_aggregator_connection_data_plaid import MigrateFinancialConnectionsAggregatorConnectionDataPlaid
 
 
-class GetFinancialConnectionResponse(BaseModel):
+class MigrateFinancialConnectionsAggregatorConnectionData(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    GetFinancialConnectionResponse - a model defined in OpenAPI
+    MigrateFinancialConnectionsAggregatorConnectionData - a model defined in OpenAPI
 
-        financial_connection: The financial_connection of this GetFinancialConnectionResponse.
-        request_id: The request_id of this GetFinancialConnectionResponse.
+        plaid: The plaid of this MigrateFinancialConnectionsAggregatorConnectionData [Optional].
+        mx: The mx of this MigrateFinancialConnectionsAggregatorConnectionData [Optional].
     """
 
-    financial_connection: FinancialConnectionDetails = Field(alias="financial_connection")
-    request_id: str = Field(alias="request_id")
+    plaid: Optional[MigrateFinancialConnectionsAggregatorConnectionDataPlaid] = Field(alias="plaid", default=None)
+    mx: Optional[MigrateFinancialConnectionsAggregatorConnectionDataMx] = Field(alias="mx", default=None)
 
-GetFinancialConnectionResponse.update_forward_refs()
+MigrateFinancialConnectionsAggregatorConnectionData.update_forward_refs()
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_account_details_request.py` & `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_account_details_request.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_account_details_response.py` & `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_account_details_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connection_data import FinancialConnectionData
-from 3.4.5.models.financial_connections_account_details import FinancialConnectionsAccountDetails
+from fuse_client.models.financial_connection_data import FinancialConnectionData
+from fuse_client.models.financial_connections_account_details import FinancialConnectionsAccountDetails
 
 
 class GetFinancialConnectionsAccountDetailsResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_accounts_request.py` & `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_accounts_request.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_accounts_response.py` & `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_accounts_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connection_data import FinancialConnectionData
-from 3.4.5.models.financial_connections_account import FinancialConnectionsAccount
+from fuse_client.models.financial_connection_data import FinancialConnectionData
+from fuse_client.models.financial_connections_account import FinancialConnectionsAccount
 
 
 class GetFinancialConnectionsAccountsResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_balance_request.py` & `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_owners_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
 
-class GetFinancialConnectionsBalanceRequest(BaseModel):
+class GetFinancialConnectionsOwnersRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    GetFinancialConnectionsBalanceRequest - a model defined in OpenAPI
+    GetFinancialConnectionsOwnersRequest - a model defined in OpenAPI
 
-        access_token: The access_token of this GetFinancialConnectionsBalanceRequest.
+        access_token: The access_token of this GetFinancialConnectionsOwnersRequest.
     """
 
     access_token: str = Field(alias="access_token")
 
-GetFinancialConnectionsBalanceRequest.update_forward_refs()
+GetFinancialConnectionsOwnersRequest.update_forward_refs()
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_balance_response.py` & `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_balance_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connections_account_balance import FinancialConnectionsAccountBalance
+from fuse_client.models.financial_connections_account_balance import FinancialConnectionsAccountBalance
 
 
 class GetFinancialConnectionsBalanceResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_owners_request.py` & `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_balance_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
+from fuse_client.models.get_financial_connections_balance_request_options import GetFinancialConnectionsBalanceRequestOptions
 
 
-class GetFinancialConnectionsOwnersRequest(BaseModel):
+class GetFinancialConnectionsBalanceRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    GetFinancialConnectionsOwnersRequest - a model defined in OpenAPI
+    GetFinancialConnectionsBalanceRequest - a model defined in OpenAPI
 
-        access_token: The access_token of this GetFinancialConnectionsOwnersRequest.
+        access_token: The access_token of this GetFinancialConnectionsBalanceRequest.
+        options: The options of this GetFinancialConnectionsBalanceRequest [Optional].
     """
 
     access_token: str = Field(alias="access_token")
+    options: Optional[GetFinancialConnectionsBalanceRequestOptions] = Field(alias="options", default=None)
 
-GetFinancialConnectionsOwnersRequest.update_forward_refs()
+GetFinancialConnectionsBalanceRequest.update_forward_refs()
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_owners_response.py` & `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_owners_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.get_financial_connections_owners_response_accounts_inner import GetFinancialConnectionsOwnersResponseAccountsInner
+from fuse_client.models.get_financial_connections_owners_response_accounts_inner import GetFinancialConnectionsOwnersResponseAccountsInner
 
 
 class GetFinancialConnectionsOwnersResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_owners_response_accounts_inner.py` & `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_owners_response_accounts_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connections_owner import FinancialConnectionsOwner
+from fuse_client.models.financial_connections_owner import FinancialConnectionsOwner
 
 
 class GetFinancialConnectionsOwnersResponseAccountsInner(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_transactions_request.py` & `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_transactions_request.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_financial_connections_transactions_response.py` & `fuse_client-1.0.5/src/fuse_client/models/get_financial_connections_transactions_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.transaction import Transaction
+from fuse_client.models.transaction import Transaction
 
 
 class GetFinancialConnectionsTransactionsResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_financial_institution_response.py` & `fuse_client-1.0.5/src/fuse_client/models/get_financial_institution_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_institution import FinancialInstitution
+from fuse_client.models.financial_institution import FinancialInstitution
 
 
 class GetFinancialInstitutionResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_investment_holdings_request.py` & `fuse_client-1.0.5/src/fuse_client/models/get_investment_holdings_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.get_investment_holdings_request_options import GetInvestmentHoldingsRequestOptions
+from fuse_client.models.get_investment_holdings_request_options import GetInvestmentHoldingsRequestOptions
 
 
 class GetInvestmentHoldingsRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_investment_holdings_request_options.py` & `fuse_client-1.0.5/src/fuse_client/models/get_investment_holdings_request_options.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_investment_holdings_response.py` & `fuse_client-1.0.5/src/fuse_client/models/get_investment_holdings_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connections_account import FinancialConnectionsAccount
-from 3.4.5.models.financial_connections_holding import FinancialConnectionsHolding
+from fuse_client.models.financial_connections_account import FinancialConnectionsAccount
+from fuse_client.models.financial_connections_holding import FinancialConnectionsHolding
 
 
 class GetInvestmentHoldingsResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_investment_transactions_request.py` & `fuse_client-1.0.5/src/fuse_client/models/get_investment_transactions_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.get_investment_transactions_request_options import GetInvestmentTransactionsRequestOptions
+from fuse_client.models.get_investment_transactions_request_options import GetInvestmentTransactionsRequestOptions
 
 
 class GetInvestmentTransactionsRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_investment_transactions_request_options.py` & `fuse_client-1.0.5/src/fuse_client/models/get_investment_transactions_request_options.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_liabilities_request.py` & `fuse_client-1.0.5/src/fuse_client/models/get_liabilities_request.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/get_liabilities_response.py` & `fuse_client-1.0.5/src/fuse_client/models/get_liabilities_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.financial_connections_account_liability import FinancialConnectionsAccountLiability
+from fuse_client.models.financial_connections_account_liability import FinancialConnectionsAccountLiability
 
 
 class GetLiabilitiesResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/migrate_financial_connections_aggregator_connection_data.py` & `fuse_client-1.0.5/src/fuse_client/models/sync_financial_connections_data_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,26 +3,24 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.migrate_financial_connections_aggregator_connection_data_mx import MigrateFinancialConnectionsAggregatorConnectionDataMx
-from 3.4.5.models.migrate_financial_connections_aggregator_connection_data_plaid import MigrateFinancialConnectionsAggregatorConnectionDataPlaid
 
 
-class MigrateFinancialConnectionsAggregatorConnectionData(BaseModel):
+class SyncFinancialConnectionsDataResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    MigrateFinancialConnectionsAggregatorConnectionData - a model defined in OpenAPI
+    SyncFinancialConnectionsDataResponse - a model defined in OpenAPI
 
-        plaid: The plaid of this MigrateFinancialConnectionsAggregatorConnectionData [Optional].
-        mx: The mx of this MigrateFinancialConnectionsAggregatorConnectionData [Optional].
+        message: The message of this SyncFinancialConnectionsDataResponse [Optional].
+        request_id: The request_id of this SyncFinancialConnectionsDataResponse [Optional].
     """
 
-    plaid: Optional[MigrateFinancialConnectionsAggregatorConnectionDataPlaid] = Field(alias="plaid", default=None)
-    mx: Optional[MigrateFinancialConnectionsAggregatorConnectionDataMx] = Field(alias="mx", default=None)
+    message: Optional[str] = Field(alias="message", default=None)
+    request_id: Optional[str] = Field(alias="request_id", default=None)
 
-MigrateFinancialConnectionsAggregatorConnectionData.update_forward_refs()
+SyncFinancialConnectionsDataResponse.update_forward_refs()
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/migrate_financial_connections_aggregator_connection_data_mx.py` & `fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_aggregator_connection_data_mx.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/migrate_financial_connections_aggregator_connection_data_plaid.py` & `fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_aggregator_connection_data_plaid.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/migrate_financial_connections_token_request.py` & `fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_token_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
-from 3.4.5.models.migrate_financial_connections_token_request_entity import MigrateFinancialConnectionsTokenRequestEntity
-from 3.4.5.models.product import Product
+from fuse_client.models.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
+from fuse_client.models.migrate_financial_connections_token_request_entity import MigrateFinancialConnectionsTokenRequestEntity
+from fuse_client.models.product import Product
 
 
 class MigrateFinancialConnectionsTokenRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/migrate_financial_connections_token_request_entity.py` & `fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_token_request_entity.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/migrate_financial_connections_token_response.py` & `fuse_client-1.0.5/src/fuse_client/models/migrate_financial_connections_token_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
+from fuse_client.models.migrate_financial_connections_aggregator_connection_data import MigrateFinancialConnectionsAggregatorConnectionData
 
 
 class MigrateFinancialConnectionsTokenResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/product.py` & `fuse_client-1.0.5/src/fuse_client/models/product.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/refresh_asset_report_request.py` & `fuse_client-1.0.5/src/fuse_client/models/refresh_asset_report_request.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/sync_financial_connections_data_response.py` & `fuse_client-1.0.5/src/fuse_client/models/update_entity_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,31 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
+from fuse_client.models.aggregator import Aggregator
 
 
-class SyncFinancialConnectionsDataResponse(BaseModel):
+class UpdateEntityResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    SyncFinancialConnectionsDataResponse - a model defined in OpenAPI
+    UpdateEntityResponse - a model defined in OpenAPI
 
-        message: The message of this SyncFinancialConnectionsDataResponse [Optional].
-        request_id: The request_id of this SyncFinancialConnectionsDataResponse [Optional].
+        id: The id of this UpdateEntityResponse [Optional].
+        email: The email of this UpdateEntityResponse [Optional].
+        aggregators: The aggregators of this UpdateEntityResponse [Optional].
+        institution_ids: The institution_ids of this UpdateEntityResponse [Optional].
+        request_id: The request_id of this UpdateEntityResponse [Optional].
     """
 
-    message: Optional[str] = Field(alias="message", default=None)
+    id: Optional[str] = Field(alias="id", default=None)
+    email: Optional[str] = Field(alias="email", default=None)
+    aggregators: Optional[List[Aggregator]] = Field(alias="aggregators", default=None)
+    institution_ids: Optional[List[str]] = Field(alias="institution_ids", default=None)
     request_id: Optional[str] = Field(alias="request_id", default=None)
 
-SyncFinancialConnectionsDataResponse.update_forward_refs()
+UpdateEntityResponse.update_forward_refs()
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/sync_transactions_request.py` & `fuse_client-1.0.5/src/fuse_client/models/sync_transactions_request.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/sync_transactions_response.py` & `fuse_client-1.0.5/src/fuse_client/models/sync_transactions_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.sync_transactions_response_removed_inner import SyncTransactionsResponseRemovedInner
-from 3.4.5.models.transaction import Transaction
+from fuse_client.models.sync_transactions_response_removed_inner import SyncTransactionsResponseRemovedInner
+from fuse_client.models.transaction import Transaction
 
 
 class SyncTransactionsResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/sync_transactions_response_removed_inner.py` & `fuse_client-1.0.5/src/fuse_client/models/sync_transactions_response_removed_inner.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/transaction.py` & `fuse_client-1.0.5/src/fuse_client/models/transaction.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.transaction_merchant import TransactionMerchant
+from fuse_client.models.transaction_merchant import TransactionMerchant
 
 
 class Transaction(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/transaction_merchant.py` & `fuse_client-1.0.5/src/fuse_client/models/transaction_merchant.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/update_entity_request.py` & `fuse_client-1.0.5/src/fuse_client/models/fuse_api_error_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.aggregator import Aggregator
+from fuse_client.models.aggregator import Aggregator
+from fuse_client.models.fuse_api_error import FuseApiError
 
 
-class UpdateEntityRequest(BaseModel):
+class FuseApiErrorData(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    UpdateEntityRequest - a model defined in OpenAPI
+    FuseApiErrorData - a model defined in OpenAPI
 
-        email: The email of this UpdateEntityRequest [Optional].
-        aggregators: The aggregators of this UpdateEntityRequest [Optional].
-        institution_ids: The institution_ids of this UpdateEntityRequest [Optional].
+        aggregator: The aggregator of this FuseApiErrorData [Optional].
+        errors: The errors of this FuseApiErrorData [Optional].
     """
 
-    email: Optional[str] = Field(alias="email", default=None)
-    aggregators: Optional[List[Aggregator]] = Field(alias="aggregators", default=None)
-    institution_ids: Optional[List[str]] = Field(alias="institution_ids", default=None)
+    aggregator: Optional[Aggregator] = Field(alias="aggregator", default=None)
+    errors: Optional[List[FuseApiError]] = Field(alias="errors", default=None)
 
-UpdateEntityRequest.update_forward_refs()
+FuseApiErrorData.update_forward_refs()
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/webhook_event.py` & `fuse_client-1.0.5/src/fuse_client/models/webhook_event.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
-from 3.4.5.models.webhook_source import WebhookSource
-from 3.4.5.models.webhook_type import WebhookType
+from fuse_client.models.webhook_source import WebhookSource
+from fuse_client.models.webhook_type import WebhookType
 
 
 class WebhookEvent(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
```

### Comparing `fuse_client-1.0.0/src/3/4/5/models/webhook_source.py` & `fuse_client-1.0.5/src/fuse_client/models/webhook_source.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/models/webhook_type.py` & `fuse_client-1.0.5/src/fuse_client/models/webhook_type.py`

 * *Files identical despite different names*

### Comparing `fuse_client-1.0.0/src/3/4/5/security_api.py` & `fuse_client-1.0.5/src/fuse_client/security_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     OAuth2,
     OAuth2AuthorizationCodeBearer,
     OAuth2PasswordBearer,
     SecurityScopes,
 )
 from fastapi.security.api_key import APIKeyCookie, APIKeyHeader, APIKeyQuery  # noqa: F401
 
-from 3.4.5.models.extra_models import TokenModel
+from fuse_client.models.extra_models import TokenModel
 
 
 def get_token_fuseApiKey(
     token_api_key_header: str = Security(
         APIKeyHeader(name="Fuse-Api-Key", auto_error=False)
     ),
 ) -> TokenModel:
@@ -53,232 +53,232 @@
     :return: Information attached to provided api_key or None if api_key is invalid or does not allow access to called API
     :rtype: TokenModel | None
     """
 
     ...
 
 
-def get_token_mxApiKey(
+def get_token_plaidClientId(
     token_api_key_header: str = Security(
-        APIKeyHeader(name="Mx-Api-Key", auto_error=False)
+        APIKeyHeader(name="Plaid-Client-Id", auto_error=False)
     ),
 ) -> TokenModel:
     """
     Check and retrieve authentication information from api_key.
 
-    :param token_api_key_header API key provided by Authorization[Mx-Api-Key] header
+    :param token_api_key_header API key provided by Authorization[Plaid-Client-Id] header
     
     
     :type token_api_key_header: str
     :return: Information attached to provided api_key or None if api_key is invalid or does not allow access to called API
     :rtype: TokenModel | None
     """
 
     ...
 
 
-def get_token_mxClientId(
+def get_token_plaidSecret(
     token_api_key_header: str = Security(
-        APIKeyHeader(name="Mx-Client-Id", auto_error=False)
+        APIKeyHeader(name="Plaid-Secret", auto_error=False)
     ),
 ) -> TokenModel:
     """
     Check and retrieve authentication information from api_key.
 
-    :param token_api_key_header API key provided by Authorization[Mx-Client-Id] header
+    :param token_api_key_header API key provided by Authorization[Plaid-Secret] header
     
     
     :type token_api_key_header: str
     :return: Information attached to provided api_key or None if api_key is invalid or does not allow access to called API
     :rtype: TokenModel | None
     """
 
     ...
 
 
-def get_token_plaidClientId(
+def get_token_tellerApplicationId(
     token_api_key_header: str = Security(
-        APIKeyHeader(name="Plaid-Client-Id", auto_error=False)
+        APIKeyHeader(name="Teller-Application-Id", auto_error=False)
     ),
 ) -> TokenModel:
     """
     Check and retrieve authentication information from api_key.
 
-    :param token_api_key_header API key provided by Authorization[Plaid-Client-Id] header
+    :param token_api_key_header API key provided by Authorization[Teller-Application-Id] header
     
     
     :type token_api_key_header: str
     :return: Information attached to provided api_key or None if api_key is invalid or does not allow access to called API
     :rtype: TokenModel | None
     """
 
     ...
 
 
-def get_token_plaidSecret(
+def get_token_tellerCertificate(
     token_api_key_header: str = Security(
-        APIKeyHeader(name="Plaid-Secret", auto_error=False)
+        APIKeyHeader(name="Teller-Certificate", auto_error=False)
     ),
 ) -> TokenModel:
     """
     Check and retrieve authentication information from api_key.
 
-    :param token_api_key_header API key provided by Authorization[Plaid-Secret] header
+    :param token_api_key_header API key provided by Authorization[Teller-Certificate] header
     
     
     :type token_api_key_header: str
     :return: Information attached to provided api_key or None if api_key is invalid or does not allow access to called API
     :rtype: TokenModel | None
     """
 
     ...
 
 
-def get_token_proxyUrlKey(
+def get_token_tellerPrivateKey(
     token_api_key_header: str = Security(
-        APIKeyHeader(name="Proxy-Url", auto_error=False)
+        APIKeyHeader(name="Teller-Private-Key", auto_error=False)
     ),
 ) -> TokenModel:
     """
     Check and retrieve authentication information from api_key.
 
-    :param token_api_key_header API key provided by Authorization[Proxy-Url] header
+    :param token_api_key_header API key provided by Authorization[Teller-Private-Key] header
     
     
     :type token_api_key_header: str
     :return: Information attached to provided api_key or None if api_key is invalid or does not allow access to called API
     :rtype: TokenModel | None
     """
 
     ...
 
 
-def get_token_snaptradeClientId(
+def get_token_tellerTokenSigningKey(
     token_api_key_header: str = Security(
-        APIKeyHeader(name="Snaptrade-Client-Id", auto_error=False)
+        APIKeyHeader(name="Teller-Token-Signing-Key", auto_error=False)
     ),
 ) -> TokenModel:
     """
     Check and retrieve authentication information from api_key.
 
-    :param token_api_key_header API key provided by Authorization[Snaptrade-Client-Id] header
+    :param token_api_key_header API key provided by Authorization[Teller-Token-Signing-Key] header
     
     
     :type token_api_key_header: str
     :return: Information attached to provided api_key or None if api_key is invalid or does not allow access to called API
     :rtype: TokenModel | None
     """
 
     ...
 
 
-def get_token_snaptradeConsumerKey(
+def get_token_tellerSigningSecret(
     token_api_key_header: str = Security(
-        APIKeyHeader(name="Snaptrade-Consumer-Id", auto_error=False)
+        APIKeyHeader(name="Teller-Signing-Secret", auto_error=False)
     ),
 ) -> TokenModel:
     """
     Check and retrieve authentication information from api_key.
 
-    :param token_api_key_header API key provided by Authorization[Snaptrade-Consumer-Id] header
+    :param token_api_key_header API key provided by Authorization[Teller-Signing-Secret] header
     
     
     :type token_api_key_header: str
     :return: Information attached to provided api_key or None if api_key is invalid or does not allow access to called API
     :rtype: TokenModel | None
     """
 
     ...
 
 
-def get_token_tellerApplicationId(
+def get_token_mxClientId(
     token_api_key_header: str = Security(
-        APIKeyHeader(name="Teller-Application-Id", auto_error=False)
+        APIKeyHeader(name="Mx-Client-Id", auto_error=False)
     ),
 ) -> TokenModel:
     """
     Check and retrieve authentication information from api_key.
 
-    :param token_api_key_header API key provided by Authorization[Teller-Application-Id] header
+    :param token_api_key_header API key provided by Authorization[Mx-Client-Id] header
     
     
     :type token_api_key_header: str
     :return: Information attached to provided api_key or None if api_key is invalid or does not allow access to called API
     :rtype: TokenModel | None
     """
 
     ...
 
 
-def get_token_tellerCertificate(
+def get_token_mxApiKey(
     token_api_key_header: str = Security(
-        APIKeyHeader(name="Teller-Certificate", auto_error=False)
+        APIKeyHeader(name="Mx-Api-Key", auto_error=False)
     ),
 ) -> TokenModel:
     """
     Check and retrieve authentication information from api_key.
 
-    :param token_api_key_header API key provided by Authorization[Teller-Certificate] header
+    :param token_api_key_header API key provided by Authorization[Mx-Api-Key] header
     
     
     :type token_api_key_header: str
     :return: Information attached to provided api_key or None if api_key is invalid or does not allow access to called API
     :rtype: TokenModel | None
     """
 
     ...
 
 
-def get_token_tellerPrivateKey(
+def get_token_snaptradeClientId(
     token_api_key_header: str = Security(
-        APIKeyHeader(name="Teller-Private-Key", auto_error=False)
+        APIKeyHeader(name="Snaptrade-Client-Id", auto_error=False)
     ),
 ) -> TokenModel:
     """
     Check and retrieve authentication information from api_key.
 
-    :param token_api_key_header API key provided by Authorization[Teller-Private-Key] header
+    :param token_api_key_header API key provided by Authorization[Snaptrade-Client-Id] header
     
     
     :type token_api_key_header: str
     :return: Information attached to provided api_key or None if api_key is invalid or does not allow access to called API
     :rtype: TokenModel | None
     """
 
     ...
 
 
-def get_token_tellerSigningSecret(
+def get_token_snaptradeConsumerKey(
     token_api_key_header: str = Security(
-        APIKeyHeader(name="Teller-Signing-Secret", auto_error=False)
+        APIKeyHeader(name="Snaptrade-Consumer-Id", auto_error=False)
     ),
 ) -> TokenModel:
     """
     Check and retrieve authentication information from api_key.
 
-    :param token_api_key_header API key provided by Authorization[Teller-Signing-Secret] header
+    :param token_api_key_header API key provided by Authorization[Snaptrade-Consumer-Id] header
     
     
     :type token_api_key_header: str
     :return: Information attached to provided api_key or None if api_key is invalid or does not allow access to called API
     :rtype: TokenModel | None
     """
 
     ...
 
 
-def get_token_tellerTokenSigningKey(
+def get_token_proxyUrlKey(
     token_api_key_header: str = Security(
-        APIKeyHeader(name="Teller-Token-Signing-Key", auto_error=False)
+        APIKeyHeader(name="Proxy-Url", auto_error=False)
     ),
 ) -> TokenModel:
     """
     Check and retrieve authentication information from api_key.
 
-    :param token_api_key_header API key provided by Authorization[Teller-Token-Signing-Key] header
+    :param token_api_key_header API key provided by Authorization[Proxy-Url] header
     
     
     :type token_api_key_header: str
     :return: Information attached to provided api_key or None if api_key is invalid or does not allow access to called API
     :rtype: TokenModel | None
     """
```

### Comparing `fuse_client-1.0.0/src/fuse_client/apis/fuse_api.py` & `fuse_client-1.0.5/tests/test_fuse_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,525 +1,472 @@
 # coding: utf-8
 
-from typing import Dict, List  # noqa: F401
+from fastapi.testclient import TestClient
+
+
+from fuse_client.models.create_asset_report_request import CreateAssetReportRequest  # noqa: F401
+from fuse_client.models.create_asset_report_response import CreateAssetReportResponse  # noqa: F401
+from fuse_client.models.create_link_token_request import CreateLinkTokenRequest  # noqa: F401
+from fuse_client.models.create_link_token_response import CreateLinkTokenResponse  # noqa: F401
+from fuse_client.models.create_session_request import CreateSessionRequest  # noqa: F401
+from fuse_client.models.create_session_response import CreateSessionResponse  # noqa: F401
+from fuse_client.models.delete_financial_connection_response import DeleteFinancialConnectionResponse  # noqa: F401
+from fuse_client.models.exchange_financial_connections_public_token_request import ExchangeFinancialConnectionsPublicTokenRequest  # noqa: F401
+from fuse_client.models.exchange_financial_connections_public_token_response import ExchangeFinancialConnectionsPublicTokenResponse  # noqa: F401
+from fuse_client.models.get_asset_report_request import GetAssetReportRequest  # noqa: F401
+from fuse_client.models.get_asset_report_response import GetAssetReportResponse  # noqa: F401
+from fuse_client.models.get_entity_response import GetEntityResponse  # noqa: F401
+from fuse_client.models.get_financial_connection_response import GetFinancialConnectionResponse  # noqa: F401
+from fuse_client.models.get_financial_connections_account_details_request import GetFinancialConnectionsAccountDetailsRequest  # noqa: F401
+from fuse_client.models.get_financial_connections_account_details_response import GetFinancialConnectionsAccountDetailsResponse  # noqa: F401
+from fuse_client.models.get_financial_connections_accounts_request import GetFinancialConnectionsAccountsRequest  # noqa: F401
+from fuse_client.models.get_financial_connections_accounts_response import GetFinancialConnectionsAccountsResponse  # noqa: F401
+from fuse_client.models.get_financial_connections_balance_request import GetFinancialConnectionsBalanceRequest  # noqa: F401
+from fuse_client.models.get_financial_connections_balance_response import GetFinancialConnectionsBalanceResponse  # noqa: F401
+from fuse_client.models.get_financial_connections_owners_request import GetFinancialConnectionsOwnersRequest  # noqa: F401
+from fuse_client.models.get_financial_connections_owners_response import GetFinancialConnectionsOwnersResponse  # noqa: F401
+from fuse_client.models.get_financial_connections_transactions_request import GetFinancialConnectionsTransactionsRequest  # noqa: F401
+from fuse_client.models.get_financial_connections_transactions_response import GetFinancialConnectionsTransactionsResponse  # noqa: F401
+from fuse_client.models.get_financial_institution_response import GetFinancialInstitutionResponse  # noqa: F401
+from fuse_client.models.get_investment_holdings_request import GetInvestmentHoldingsRequest  # noqa: F401
+from fuse_client.models.get_investment_holdings_response import GetInvestmentHoldingsResponse  # noqa: F401
+from fuse_client.models.get_investment_transactions_request import GetInvestmentTransactionsRequest  # noqa: F401
+from fuse_client.models.get_investment_transactions_response import GetInvestmentTransactionsResponse  # noqa: F401
+from fuse_client.models.get_liabilities_request import GetLiabilitiesRequest  # noqa: F401
+from fuse_client.models.get_liabilities_response import GetLiabilitiesResponse  # noqa: F401
+from fuse_client.models.migrate_financial_connections_token_request import MigrateFinancialConnectionsTokenRequest  # noqa: F401
+from fuse_client.models.migrate_financial_connections_token_response import MigrateFinancialConnectionsTokenResponse  # noqa: F401
+from fuse_client.models.refresh_asset_report_request import RefreshAssetReportRequest  # noqa: F401
+from fuse_client.models.sync_financial_connections_data_response import SyncFinancialConnectionsDataResponse  # noqa: F401
+
+
+def test_create_asset_report(client: TestClient):
+    """Test case for create_asset_report
+
+    
+    """
+    create_asset_report_request = {"access_token":"access_token","include_identity":1,"days_requested":30.15014613278082}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/asset_report/create",
+        headers=headers,
+        json=create_asset_report_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_create_link_token(client: TestClient):
+    """Test case for create_link_token
+
+    
+    """
+    create_link_token_request = {"session_client_secret":"session_client_secret","mx":{"config":"{}"},"plaid":{"config":"{}"},"client_name":"client_name","entity":{"name":"name","id":"id","email":"email"},"institution_id":"institution_id"}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/link/token",
+        headers=headers,
+        json=create_link_token_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_create_session(client: TestClient):
+    """Test case for create_session
+
+    
+    """
+    create_session_request = {"access_token":"access_token","supported_financial_institution_aggregators":[null,null],"country_codes":[null,null],"is_web_view":1,"entity":{"name":"name","id":"id","email":"email"},"products":[null,null]}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/session",
+        headers=headers,
+        json=create_session_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_delete_financial_connection(client: TestClient):
+    """Test case for delete_financial_connection
+
+    Delete a financial connection
+    """
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "DELETE",
+        "/v1/financial_connections/{financial_connection_id_to_delete}".format(financial_connection_id_to_delete='financial_connection_id_to_delete_example'),
+        headers=headers,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_exchange_financial_connections_public_token(client: TestClient):
+    """Test case for exchange_financial_connections_public_token
+
+    
+    """
+    exchange_financial_connections_public_token_request = {"public_token":"public_token"}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/financial_connections/public_token/exchange",
+        headers=headers,
+        json=exchange_financial_connections_public_token_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_get_asset_report(client: TestClient):
+    """Test case for get_asset_report
+
+    
+    """
+    get_asset_report_request = {"asset_report_token":"asset_report_token"}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/asset_report",
+        headers=headers,
+        json=get_asset_report_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_get_entity(client: TestClient):
+    """Test case for get_entity
+
+    Get entity
+    """
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "GET",
+        "/v1/entities/{entity_id}".format(entity_id='entity_id_example'),
+        headers=headers,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_get_financial_connection(client: TestClient):
+    """Test case for get_financial_connection
+
+    Get financial connection details
+    """
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "GET",
+        "/v1/financial_connections/{financial_connection_id}".format(financial_connection_id='financial_connection_id_example'),
+        headers=headers,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_get_financial_connections_account_details(client: TestClient):
+    """Test case for get_financial_connections_account_details
+
+    Get account details
+    """
+    get_financial_connections_account_details_request = {"access_token":"access_token"}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/financial_connections/accounts/details",
+        headers=headers,
+        json=get_financial_connections_account_details_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_get_financial_connections_accounts(client: TestClient):
+    """Test case for get_financial_connections_accounts
+
+    Get accounts
+    """
+    get_financial_connections_accounts_request = {"access_token":"access_token"}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/financial_connections/accounts",
+        headers=headers,
+        json=get_financial_connections_accounts_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_get_financial_connections_balances(client: TestClient):
+    """Test case for get_financial_connections_balances
+
+    Get balances
+    """
+    get_financial_connections_balance_request = {"access_token":"access_token","options":{"remote_account_ids":["remote_account_ids","remote_account_ids"]}}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/financial_connections/balances",
+        headers=headers,
+        json=get_financial_connections_balance_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_get_financial_connections_owners(client: TestClient):
+    """Test case for get_financial_connections_owners
+
+    Get account owners
+    """
+    get_financial_connections_owners_request = {"access_token":"access_token"}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/financial_connections/owners",
+        headers=headers,
+        json=get_financial_connections_owners_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_get_financial_connections_transactions(client: TestClient):
+    """Test case for get_financial_connections_transactions
+
+    Get transactions
+    """
+    get_financial_connections_transactions_request = {"access_token":"access_token","end_date":"end_date","records_per_page":64,"page":1,"start_date":"start_date"}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/financial_connections/transactions",
+        headers=headers,
+        json=get_financial_connections_transactions_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_get_financial_institution(client: TestClient):
+    """Test case for get_financial_institution
+
+    Get a financial institution
+    """
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "GET",
+        "/v1/financial_connections/institutions/{institution_id}".format(institution_id='institution_id_example'),
+        headers=headers,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_get_investment_holdings(client: TestClient):
+    """Test case for get_investment_holdings
+
+    Get investment holdings
+    """
+    get_investment_holdings_request = {"access_token":"access_token","options":{"remote_account_ids":["remote_account_ids","remote_account_ids"]}}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/financial_connections/investments/holdings",
+        headers=headers,
+        json=get_investment_holdings_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_get_investment_transactions(client: TestClient):
+    """Test case for get_investment_transactions
+
+    Get investment transactions
+    """
+    get_investment_transactions_request = {"access_token":"access_token","end_date":"end_date","records_per_page":64,"options":{"remote_account_ids":["remote_account_ids","remote_account_ids"]},"page":1,"start_date":"start_date"}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/financial_connections/investments/transactions",
+        headers=headers,
+        json=get_investment_transactions_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_migrate_financial_connection(client: TestClient):
+    """Test case for migrate_financial_connection
+
+    Migrate financial connection
+    """
+    migrate_financial_connections_token_request = {"aggregator":"plaid","connection_data":{"mx":{"member_guid":"member_guid","user_guid":"user_guid"},"plaid":{"access_token":"access_token"}},"entity":{"id":"id"},"fuse_products":[null,null]}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/financial_connections/migrate",
+        headers=headers,
+        json=migrate_financial_connections_token_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_refresh_asset_report(client: TestClient):
+    """Test case for refresh_asset_report
+
+    
+    """
+    refresh_asset_report_request = {"access_token":"access_token","include_identity":1,"days_requested":30.15014613278082}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/asset_report/refresh",
+        headers=headers,
+        json=refresh_asset_report_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_sync_financial_connections_data(client: TestClient):
+    """Test case for sync_financial_connections_data
+
+    Sync financial connections data
+    """
+    body = None
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/financial_connections/sync",
+        headers=headers,
+        json=body,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
+
+
+def test_v1_financial_connections_liabilities_post(client: TestClient):
+    """Test case for v1_financial_connections_liabilities_post
+
+    Get liabilities
+    """
+    get_liabilities_request = {"access_token":"access_token"}
+
+    headers = {
+        "fuseApiKey": "special-key",
+        "fuseClientId": "special-key",
+    }
+    response = client.request(
+        "POST",
+        "/v1/financial_connections/liabilities",
+        headers=headers,
+        json=get_liabilities_request,
+    )
+
+    # uncomment below to assert the status code of the HTTP response
+    #assert response.status_code == 200
 
-from fastapi import (  # noqa: F401
-    APIRouter,
-    Body,
-    Cookie,
-    Depends,
-    Form,
-    Header,
-    Path,
-    Query,
-    Response,
-    Security,
-    status,
-)
-
-from fuse_client.models.extra_models import TokenModel  # noqa: F401
-from fuse_client.models.create_asset_report_request import CreateAssetReportRequest
-from fuse_client.models.create_asset_report_response import CreateAssetReportResponse
-from fuse_client.models.create_entity_request import CreateEntityRequest
-from fuse_client.models.create_entity_response import CreateEntityResponse
-from fuse_client.models.create_link_token_request import CreateLinkTokenRequest
-from fuse_client.models.create_link_token_response import CreateLinkTokenResponse
-from fuse_client.models.create_session_request import CreateSessionRequest
-from fuse_client.models.create_session_response import CreateSessionResponse
-from fuse_client.models.delete_financial_connection_response import DeleteFinancialConnectionResponse
-from fuse_client.models.exchange_financial_connections_public_token_request import ExchangeFinancialConnectionsPublicTokenRequest
-from fuse_client.models.exchange_financial_connections_public_token_response import ExchangeFinancialConnectionsPublicTokenResponse
-from fuse_client.models.get_asset_report_request import GetAssetReportRequest
-from fuse_client.models.get_asset_report_response import GetAssetReportResponse
-from fuse_client.models.get_entity_response import GetEntityResponse
-from fuse_client.models.get_financial_connection_response import GetFinancialConnectionResponse
-from fuse_client.models.get_financial_connections_account_details_request import GetFinancialConnectionsAccountDetailsRequest
-from fuse_client.models.get_financial_connections_account_details_response import GetFinancialConnectionsAccountDetailsResponse
-from fuse_client.models.get_financial_connections_accounts_request import GetFinancialConnectionsAccountsRequest
-from fuse_client.models.get_financial_connections_accounts_response import GetFinancialConnectionsAccountsResponse
-from fuse_client.models.get_financial_connections_balance_request import GetFinancialConnectionsBalanceRequest
-from fuse_client.models.get_financial_connections_balance_response import GetFinancialConnectionsBalanceResponse
-from fuse_client.models.get_financial_connections_owners_request import GetFinancialConnectionsOwnersRequest
-from fuse_client.models.get_financial_connections_owners_response import GetFinancialConnectionsOwnersResponse
-from fuse_client.models.get_financial_connections_transactions_request import GetFinancialConnectionsTransactionsRequest
-from fuse_client.models.get_financial_connections_transactions_response import GetFinancialConnectionsTransactionsResponse
-from fuse_client.models.get_financial_institution_response import GetFinancialInstitutionResponse
-from fuse_client.models.get_investment_holdings_request import GetInvestmentHoldingsRequest
-from fuse_client.models.get_investment_holdings_response import GetInvestmentHoldingsResponse
-from fuse_client.models.get_investment_transactions_request import GetInvestmentTransactionsRequest
-from fuse_client.models.get_investment_transactions_response import GetInvestmentTransactionsResponse
-from fuse_client.models.get_liabilities_request import GetLiabilitiesRequest
-from fuse_client.models.get_liabilities_response import GetLiabilitiesResponse
-from fuse_client.models.refresh_asset_report_request import RefreshAssetReportRequest
-from fuse_client.models.sync_financial_connections_data_response import SyncFinancialConnectionsDataResponse
-from fuse_client.models.sync_transactions_request import SyncTransactionsRequest
-from fuse_client.models.sync_transactions_response import SyncTransactionsResponse
-from fuse_client.models.update_entity_request import UpdateEntityRequest
-from fuse_client.models.update_entity_response import UpdateEntityResponse
-from fuse_client.security_api import get_token_fuseApiKey, get_token_fuseClientId
-
-router = APIRouter()
-
-
-@router.post(
-    "/v1/asset_report/create",
-    responses={
-        200: {"model": CreateAssetReportResponse, "description": "Response"},
-    },
-    tags=["Fuse"],
-    response_model_by_alias=True,
-)
-async def create_asset_report(
-    create_asset_report_request: CreateAssetReportRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> CreateAssetReportResponse:
-    """Use this endpoint to generate an Asset Report for a user."""
-    ...
-
-
-@router.post(
-    "/v1/entities",
-    responses={
-        200: {"model": CreateEntityResponse, "description": "Success"},
-    },
-    tags=["Fuse"],
-    summary="Create entity",
-    response_model_by_alias=True,
-)
-async def create_entity(
-    create_entity_request: CreateEntityRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> CreateEntityResponse:
-    ...
-
-
-@router.post(
-    "/v1/link/token",
-    responses={
-        200: {"model": CreateLinkTokenResponse, "description": "Response"},
-    },
-    tags=["Fuse"],
-    response_model_by_alias=True,
-)
-async def create_link_token(
-    create_link_token_request: CreateLinkTokenRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> CreateLinkTokenResponse:
-    """Create a link token to start the process of a user connecting to a specific financial institution."""
-    ...
-
-
-@router.post(
-    "/v1/session",
-    responses={
-        200: {"model": CreateSessionResponse, "description": "Response"},
-    },
-    tags=["Fuse"],
-    response_model_by_alias=True,
-)
-async def create_session(
-    create_session_request: CreateSessionRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> CreateSessionResponse:
-    """Creates a session that returns a client_secret which is required as a parameter when initializing the Fuse SDK."""
-    ...
-
-
-@router.delete(
-    "/v1/financial_connections/{financial_connection_id_to_delete}",
-    responses={
-        200: {"model": DeleteFinancialConnectionResponse, "description": "Success"},
-    },
-    tags=["Fuse"],
-    summary="Delete a financial connection",
-    response_model_by_alias=True,
-)
-async def delete_financial_connection(
-    financial_connection_id_to_delete: str = Path(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> DeleteFinancialConnectionResponse:
-    ...
-
-
-@router.post(
-    "/v1/financial_connections/public_token/exchange",
-    responses={
-        200: {"model": ExchangeFinancialConnectionsPublicTokenResponse, "description": "Response"},
-    },
-    tags=["Fuse"],
-    response_model_by_alias=True,
-)
-async def exchange_financial_connections_public_token(
-    exchange_financial_connections_public_token_request: ExchangeFinancialConnectionsPublicTokenRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> ExchangeFinancialConnectionsPublicTokenResponse:
-    """API to exchange a public token for an access token and financial connection id"""
-    ...
-
-
-@router.post(
-    "/v1/asset_report",
-    responses={
-        200: {"model": GetAssetReportResponse, "description": "Response"},
-    },
-    tags=["Fuse"],
-    response_model_by_alias=True,
-)
-async def get_asset_report(
-    get_asset_report_request: GetAssetReportRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> GetAssetReportResponse:
-    """Retrieves the Asset Report in JSON format."""
-    ...
-
-
-@router.get(
-    "/v1/entities/{entity_id}",
-    responses={
-        200: {"model": GetEntityResponse, "description": "Success"},
-    },
-    tags=["Fuse"],
-    summary="Get entity",
-    response_model_by_alias=True,
-)
-async def get_entity(
-    entity_id: str = Path(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> GetEntityResponse:
-    ...
-
-
-@router.get(
-    "/v1/financial_connections/{financial_connection_id}",
-    responses={
-        200: {"model": GetFinancialConnectionResponse, "description": "Success"},
-    },
-    tags=["Fuse"],
-    summary="Get financial connection details",
-    response_model_by_alias=True,
-)
-async def get_financial_connection(
-    financial_connection_id: str = Path(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> GetFinancialConnectionResponse:
-    ...
-
-
-@router.post(
-    "/v1/financial_connections/accounts/details",
-    responses={
-        200: {"model": GetFinancialConnectionsAccountDetailsResponse, "description": "Success"},
-    },
-    tags=["Fuse"],
-    summary="Get account details",
-    response_model_by_alias=True,
-)
-async def get_financial_connections_account_details(
-    get_financial_connections_account_details_request: GetFinancialConnectionsAccountDetailsRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> GetFinancialConnectionsAccountDetailsResponse:
-    ...
-
-
-@router.post(
-    "/v1/financial_connections/accounts",
-    responses={
-        200: {"model": GetFinancialConnectionsAccountsResponse, "description": "Successful response"},
-    },
-    tags=["Fuse"],
-    summary="Get accounts",
-    response_model_by_alias=True,
-)
-async def get_financial_connections_accounts(
-    get_financial_connections_accounts_request: GetFinancialConnectionsAccountsRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> GetFinancialConnectionsAccountsResponse:
-    ...
-
-
-@router.post(
-    "/v1/financial_connections/balances",
-    responses={
-        200: {"model": GetFinancialConnectionsBalanceResponse, "description": "Successful response"},
-    },
-    tags=["Fuse"],
-    summary="Get balances",
-    response_model_by_alias=True,
-)
-async def get_financial_connections_balances(
-    get_financial_connections_balance_request: GetFinancialConnectionsBalanceRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> GetFinancialConnectionsBalanceResponse:
-    ...
-
-
-@router.post(
-    "/v1/financial_connections/owners",
-    responses={
-        200: {"model": GetFinancialConnectionsOwnersResponse, "description": "Success"},
-    },
-    tags=["Fuse"],
-    summary="Get account owners",
-    response_model_by_alias=True,
-)
-async def get_financial_connections_owners(
-    get_financial_connections_owners_request: GetFinancialConnectionsOwnersRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> GetFinancialConnectionsOwnersResponse:
-    ...
-
-
-@router.post(
-    "/v1/financial_connections/transactions",
-    responses={
-        200: {"model": GetFinancialConnectionsTransactionsResponse, "description": "Success"},
-    },
-    tags=["Fuse"],
-    summary="Get transactions",
-    response_model_by_alias=True,
-)
-async def get_financial_connections_transactions(
-    get_financial_connections_transactions_request: GetFinancialConnectionsTransactionsRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> GetFinancialConnectionsTransactionsResponse:
-    ...
-
-
-@router.get(
-    "/v1/financial_connections/institutions/{institution_id}",
-    responses={
-        200: {"model": GetFinancialInstitutionResponse, "description": "Financial institution metadata"},
-    },
-    tags=["Fuse"],
-    summary="Get a financial institution",
-    response_model_by_alias=True,
-)
-async def get_financial_institution(
-    institution_id: str = Path(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> GetFinancialInstitutionResponse:
-    """Receive metadata for a financial institution"""
-    ...
-
-
-@router.post(
-    "/v1/financial_connections/investments/holdings",
-    responses={
-        200: {"model": GetInvestmentHoldingsResponse, "description": "Successful response"},
-    },
-    tags=["Fuse"],
-    summary="Get investment holdings",
-    response_model_by_alias=True,
-)
-async def get_investment_holdings(
-    get_investment_holdings_request: GetInvestmentHoldingsRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> GetInvestmentHoldingsResponse:
-    ...
-
-
-@router.post(
-    "/v1/financial_connections/investments/transactions",
-    responses={
-        200: {"model": GetInvestmentTransactionsResponse, "description": "Successful response"},
-    },
-    tags=["Fuse"],
-    summary="Get investment transactions",
-    response_model_by_alias=True,
-)
-async def get_investment_transactions(
-    get_investment_transactions_request: GetInvestmentTransactionsRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> GetInvestmentTransactionsResponse:
-    ...
-
-
-@router.post(
-    "/v1/asset_report/refresh",
-    responses={
-        200: {"model": CreateAssetReportResponse, "description": "Response"},
-    },
-    tags=["Fuse"],
-    response_model_by_alias=True,
-)
-async def refresh_asset_report(
-    refresh_asset_report_request: RefreshAssetReportRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> CreateAssetReportResponse:
-    """Refreshes the Asset Report in JSON format."""
-    ...
-
-
-@router.post(
-    "/v1/financial_connections/sync",
-    responses={
-        200: {"model": SyncFinancialConnectionsDataResponse, "description": "Successfully synchronized transactions"},
-    },
-    tags=["Fuse"],
-    summary="Sync financial connections data",
-    response_model_by_alias=True,
-)
-async def sync_financial_connections_data(
-    body:  = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> SyncFinancialConnectionsDataResponse:
-    """Call this endpoint upon receiving a SYNC_REQUIRED webhook. This will keep the financial connections data up to date."""
-    ...
-
-
-@router.post(
-    "/v1/financial_connections/transactions/sync",
-    responses={
-        200: {"model": SyncTransactionsResponse, "description": "Successfully synchronized transactions"},
-    },
-    tags=["Fuse"],
-    summary="Sync transactions",
-    response_model_by_alias=True,
-)
-async def sync_financial_connections_transactions(
-    sync_transactions_request: SyncTransactionsRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> SyncTransactionsResponse:
-    ...
-
-
-@router.put(
-    "/v1/entities/{entity_id_to_update}",
-    responses={
-        200: {"model": UpdateEntityResponse, "description": "Success"},
-    },
-    tags=["Fuse"],
-    summary="Update entity",
-    response_model_by_alias=True,
-)
-async def update_entity(
-    entity_id_to_update: str = Path(None, description=""),
-    update_entity_request: UpdateEntityRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> UpdateEntityResponse:
-    ...
-
-
-@router.post(
-    "/v1/financial_connections/liabilities",
-    responses={
-        200: {"model": GetLiabilitiesResponse, "description": "Successful response"},
-    },
-    tags=["Fuse"],
-    summary="Get liabilities",
-    response_model_by_alias=True,
-)
-async def v1_financial_connections_liabilities_post(
-    get_liabilities_request: GetLiabilitiesRequest = Body(None, description=""),
-    token_fuseApiKey: TokenModel = Security(
-        get_token_fuseApiKey
-    ),
-    token_fuseClientId: TokenModel = Security(
-        get_token_fuseClientId
-    ),
-) -> GetLiabilitiesResponse:
-    ...
```

### Comparing `fuse_client-1.0.0/src/fuse_client/models/financial_institution_logo.py` & `fuse_client-1.0.5/src/fuse_client/models/currency.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,24 +5,22 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 
 
-class FinancialInstitutionLogo(BaseModel):
+class Currency(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    FinancialInstitutionLogo - a model defined in OpenAPI
+    Currency - a model defined in OpenAPI
 
-        image: The image of this FinancialInstitutionLogo.
-        type: The type of this FinancialInstitutionLogo.
-        format: The format of this FinancialInstitutionLogo [Optional].
+        code: The code of this Currency.
+        name: The name of this Currency [Optional].
     """
 
-    image: str = Field(alias="image")
-    type: str = Field(alias="type")
-    format: Optional[str] = Field(alias="format", default=None)
+    code: str = Field(alias="code")
+    name: Optional[str] = Field(alias="name", default=None)
 
-FinancialInstitutionLogo.update_forward_refs()
+Currency.update_forward_refs()
```

### Comparing `fuse_client-1.0.0/src/fuse_client/models/get_investment_holdings_response.py` & `fuse_client-1.0.5/src/fuse_client/models/get_investment_transactions_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, Field, validator  # noqa: F401
 from fuse_client.models.financial_connections_account import FinancialConnectionsAccount
-from fuse_client.models.financial_connections_holding import FinancialConnectionsHolding
+from fuse_client.models.financial_connections_investment_transaction import FinancialConnectionsInvestmentTransaction
 
 
-class GetInvestmentHoldingsResponse(BaseModel):
+class GetInvestmentTransactionsResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    GetInvestmentHoldingsResponse - a model defined in OpenAPI
+    GetInvestmentTransactionsResponse - a model defined in OpenAPI
 
-        accounts: The accounts of this GetInvestmentHoldingsResponse.
-        holdings: The holdings of this GetInvestmentHoldingsResponse.
-        request_id: The request_id of this GetInvestmentHoldingsResponse.
+        accounts: The accounts of this GetInvestmentTransactionsResponse.
+        investment_transactions: The investment_transactions of this GetInvestmentTransactionsResponse.
+        request_id: The request_id of this GetInvestmentTransactionsResponse.
     """
 
     accounts: List[FinancialConnectionsAccount] = Field(alias="accounts")
-    holdings: List[FinancialConnectionsHolding] = Field(alias="holdings")
+    investment_transactions: List[FinancialConnectionsInvestmentTransaction] = Field(alias="investment_transactions")
     request_id: str = Field(alias="request_id")
 
-GetInvestmentHoldingsResponse.update_forward_refs()
+GetInvestmentTransactionsResponse.update_forward_refs()
```

### Comparing `fuse_client-1.0.0/src/fuse_client.egg-info/PKG-INFO` & `fuse_client-1.0.5/src/fuse_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuse-client
-Version: 1.0.0
+Version: 1.0.5
 Summary: No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 Keywords: OpenAPI Fuse
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
```

