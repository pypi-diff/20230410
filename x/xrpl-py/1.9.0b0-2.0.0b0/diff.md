# Comparing `tmp/xrpl-py-1.9.0b0.tar.gz` & `tmp/xrpl-py-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrpl-py-1.9.0b0.tar", max compression
+gzip compressed data, was "xrpl-py-2.0.0b0.tar", max compression
```

## Comparing `xrpl-py-1.9.0b0.tar` & `xrpl-py-2.0.0b0.tar`

### file list

```diff
@@ -1,244 +1,223 @@
--rw-r--r--   0        0        0      740 2022-08-01 03:07:06.902817 xrpl-py-1.9.0b0/LICENSE
--rw-r--r--   0        0        0    16063 2023-01-09 23:03:27.477446 xrpl-py-1.9.0b0/README.md
--rw-r--r--   0        0        0     2234 2023-01-10 21:41:52.319952 xrpl-py-1.9.0b0/pyproject.toml
--rw-r--r--   0        0        0      348 2022-08-01 03:07:06.915966 xrpl-py-1.9.0b0/xrpl/__init__.py
--rw-r--r--   0        0        0      588 2022-08-01 03:07:06.916087 xrpl-py-1.9.0b0/xrpl/account/__init__.py
--rw-r--r--   0        0        0     4410 2023-01-09 23:03:27.484660 xrpl-py-1.9.0b0/xrpl/account/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.916219 xrpl-py-1.9.0b0/xrpl/account/py.typed
--rw-r--r--   0        0        0     2692 2023-01-09 23:03:27.484901 xrpl-py-1.9.0b0/xrpl/account/transaction_history.py
--rw-r--r--   0        0        0      189 2022-08-01 03:07:06.916458 xrpl-py-1.9.0b0/xrpl/asyncio/__init__.py
--rw-r--r--   0        0        0      610 2022-08-01 03:07:06.916563 xrpl-py-1.9.0b0/xrpl/asyncio/account/__init__.py
--rw-r--r--   0        0        0     5885 2023-01-09 23:03:27.485145 xrpl-py-1.9.0b0/xrpl/asyncio/account/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.916659 xrpl-py-1.9.0b0/xrpl/asyncio/account/py.typed
--rw-r--r--   0        0        0     3432 2023-01-09 23:03:27.485379 xrpl-py-1.9.0b0/xrpl/asyncio/account/transaction_history.py
--rw-r--r--   0        0        0      705 2022-08-01 03:07:06.916816 xrpl-py-1.9.0b0/xrpl/asyncio/clients/__init__.py
--rw-r--r--   0        0        0      692 2023-01-09 23:03:27.485595 xrpl-py-1.9.0b0/xrpl/asyncio/clients/async_client.py
--rw-r--r--   0        0        0      315 2022-08-01 03:07:06.916941 xrpl-py-1.9.0b0/xrpl/asyncio/clients/async_json_rpc_client.py
--rw-r--r--   0        0        0     7099 2023-01-09 23:03:27.485917 xrpl-py-1.9.0b0/xrpl/asyncio/clients/async_websocket_client.py
--rw-r--r--   0        0        0     1066 2023-01-09 23:03:27.486167 xrpl-py-1.9.0b0/xrpl/asyncio/clients/client.py
--rw-r--r--   0        0        0     1083 2022-08-01 03:07:06.917148 xrpl-py-1.9.0b0/xrpl/asyncio/clients/exceptions.py
--rw-r--r--   0        0        0     1612 2023-01-09 23:03:27.486437 xrpl-py-1.9.0b0/xrpl/asyncio/clients/json_rpc_base.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.917264 xrpl-py-1.9.0b0/xrpl/asyncio/clients/py.typed
--rw-r--r--   0        0        0     3341 2022-08-01 03:07:06.917343 xrpl-py-1.9.0b0/xrpl/asyncio/clients/utils.py
--rw-r--r--   0        0        0     7431 2023-01-09 23:03:27.486755 xrpl-py-1.9.0b0/xrpl/asyncio/clients/websocket_base.py
--rw-r--r--   0        0        0      328 2022-08-01 03:07:06.917510 xrpl-py-1.9.0b0/xrpl/asyncio/ledger/__init__.py
--rw-r--r--   0        0        0     3443 2023-01-09 23:03:27.487487 xrpl-py-1.9.0b0/xrpl/asyncio/ledger/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.917612 xrpl-py-1.9.0b0/xrpl/asyncio/ledger/py.typed
--rw-r--r--   0        0        0     2353 2022-08-01 03:07:06.917676 xrpl-py-1.9.0b0/xrpl/asyncio/ledger/utils.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.917699 xrpl-py-1.9.0b0/xrpl/asyncio/py.typed
--rw-r--r--   0        0        0      956 2023-01-09 23:03:27.487769 xrpl-py-1.9.0b0/xrpl/asyncio/transaction/__init__.py
--rw-r--r--   0        0        0     2077 2023-01-09 23:03:27.488005 xrpl-py-1.9.0b0/xrpl/asyncio/transaction/ledger.py
--rw-r--r--   0        0        0    13273 2023-01-09 23:03:27.488262 xrpl-py-1.9.0b0/xrpl/asyncio/transaction/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.917997 xrpl-py-1.9.0b0/xrpl/asyncio/transaction/py.typed
--rw-r--r--   0        0        0     3606 2023-01-09 23:03:27.488509 xrpl-py-1.9.0b0/xrpl/asyncio/transaction/reliable_submission.py
--rw-r--r--   0        0        0      219 2022-08-01 03:07:06.918169 xrpl-py-1.9.0b0/xrpl/asyncio/wallet/__init__.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.918193 xrpl-py-1.9.0b0/xrpl/asyncio/wallet/py.typed
--rw-r--r--   0        0        0     5704 2022-11-17 18:28:25.909555 xrpl-py-1.9.0b0/xrpl/asyncio/wallet/wallet_generation.py
--rw-r--r--   0        0        0      656 2022-08-01 03:07:06.918352 xrpl-py-1.9.0b0/xrpl/clients/__init__.py
--rw-r--r--   0        0        0      295 2022-08-01 03:07:06.918414 xrpl-py-1.9.0b0/xrpl/clients/json_rpc_client.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.918443 xrpl-py-1.9.0b0/xrpl/clients/py.typed
--rw-r--r--   0        0        0      705 2023-01-09 23:03:27.488832 xrpl-py-1.9.0b0/xrpl/clients/sync_client.py
--rw-r--r--   0        0        0     8780 2023-01-09 23:03:27.489223 xrpl-py-1.9.0b0/xrpl/clients/websocket_client.py
--rw-r--r--   0        0        0     1414 2022-08-01 03:07:06.918722 xrpl-py-1.9.0b0/xrpl/constants.py
--rw-r--r--   0        0        0      171 2022-08-01 03:07:06.918808 xrpl-py-1.9.0b0/xrpl/core/__init__.py
--rw-r--r--   0        0        0     1073 2022-08-01 03:07:06.918884 xrpl-py-1.9.0b0/xrpl/core/addresscodec/__init__.py
--rw-r--r--   0        0        0     7175 2022-08-01 03:07:06.918953 xrpl-py-1.9.0b0/xrpl/core/addresscodec/codec.py
--rw-r--r--   0        0        0      194 2022-08-01 03:07:06.919006 xrpl-py-1.9.0b0/xrpl/core/addresscodec/exceptions.py
--rw-r--r--   0        0        0     4874 2022-08-01 03:07:06.919071 xrpl-py-1.9.0b0/xrpl/core/addresscodec/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.919094 xrpl-py-1.9.0b0/xrpl/core/addresscodec/py.typed
--rw-r--r--   0        0        0      235 2022-08-01 03:07:06.919150 xrpl-py-1.9.0b0/xrpl/core/addresscodec/utils.py
--rw-r--r--   0        0        0      488 2022-08-01 03:07:06.919229 xrpl-py-1.9.0b0/xrpl/core/binarycodec/__init__.py
--rw-r--r--   0        0        0      296 2022-08-01 03:07:06.919308 xrpl-py-1.9.0b0/xrpl/core/binarycodec/binary_wrappers/__init__.py
--rw-r--r--   0        0        0     9076 2022-08-01 03:07:06.919401 xrpl-py-1.9.0b0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py
--rw-r--r--   0        0        0     4650 2022-08-01 03:07:06.919480 xrpl-py-1.9.0b0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py
--rw-r--r--   0        0        0     1025 2022-08-01 03:07:06.919564 xrpl-py-1.9.0b0/xrpl/core/binarycodec/definitions/__init__.py
--rw-r--r--   0        0        0    56658 2023-01-09 23:06:12.341941 xrpl-py-1.9.0b0/xrpl/core/binarycodec/definitions/definitions.json
--rw-r--r--   0        0        0     8431 2022-08-01 03:07:06.919791 xrpl-py-1.9.0b0/xrpl/core/binarycodec/definitions/definitions.py
--rw-r--r--   0        0        0     2060 2023-01-09 23:03:21.463927 xrpl-py-1.9.0b0/xrpl/core/binarycodec/definitions/field_header.py
--rw-r--r--   0        0        0     1192 2022-08-01 03:07:06.919903 xrpl-py-1.9.0b0/xrpl/core/binarycodec/definitions/field_info.py
--rw-r--r--   0        0        0     1931 2022-08-01 03:07:06.919964 xrpl-py-1.9.0b0/xrpl/core/binarycodec/definitions/field_instance.py
--rw-r--r--   0        0        0      191 2022-08-01 03:07:06.920016 xrpl-py-1.9.0b0/xrpl/core/binarycodec/exceptions.py
--rw-r--r--   0        0        0     3942 2022-08-01 03:07:06.920077 xrpl-py-1.9.0b0/xrpl/core/binarycodec/field_id_codec.py
--rw-r--r--   0        0        0     3708 2022-08-01 03:07:06.920141 xrpl-py-1.9.0b0/xrpl/core/binarycodec/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.920169 xrpl-py-1.9.0b0/xrpl/core/binarycodec/py.typed
--rw-r--r--   0        0        0     1525 2023-01-09 23:03:21.464227 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/__init__.py
--rw-r--r--   0        0        0     2956 2022-08-01 03:07:06.920334 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/account_id.py
--rw-r--r--   0        0        0    11234 2022-08-01 03:07:06.920446 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/amount.py
--rw-r--r--   0        0        0     1950 2022-08-01 03:07:06.920520 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/blob.py
--rw-r--r--   0        0        0     4347 2022-08-01 03:07:06.920602 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/currency.py
--rw-r--r--   0        0        0     2640 2022-08-01 03:07:06.920654 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/hash.py
--rw-r--r--   0        0        0      572 2022-08-01 03:07:06.920705 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/hash128.py
--rw-r--r--   0        0        0      571 2022-08-01 03:07:06.920764 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/hash160.py
--rw-r--r--   0        0        0      572 2022-08-01 03:07:06.920890 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/hash256.py
--rw-r--r--   0        0        0     3325 2023-01-09 22:47:59.322607 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/issue.py
--rw-r--r--   0        0        0     3335 2023-01-09 23:03:21.464401 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/issued_currency.py
--rw-r--r--   0        0        0     9067 2022-08-01 03:07:06.921018 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/path_set.py
--rw-r--r--   0        0        0     2493 2022-08-01 03:07:06.921099 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/serialized_type.py
--rw-r--r--   0        0        0     3301 2022-08-01 03:07:06.921166 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/st_array.py
--rw-r--r--   0        0        0     8394 2022-08-01 03:07:06.921261 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/st_object.py
--rw-r--r--   0        0        0     3383 2022-08-01 03:07:06.921335 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/uint.py
--rw-r--r--   0        0        0     2063 2022-08-01 03:07:06.921397 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/uint16.py
--rw-r--r--   0        0        0     2283 2022-08-01 03:07:06.921488 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/uint32.py
--rw-r--r--   0        0        0     2854 2022-08-01 03:07:06.921562 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/uint64.py
--rw-r--r--   0        0        0     1994 2022-08-01 03:07:06.921617 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/uint8.py
--rw-r--r--   0        0        0     2905 2022-08-01 03:07:06.921683 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/vector256.py
--rw-r--r--   0        0        0     3361 2023-01-09 23:03:21.464534 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/xchain_attestation_batch.py
--rw-r--r--   0        0        0     3413 2023-01-09 23:03:21.464712 xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/xchain_bridge.py
--rw-r--r--   0        0        0      447 2023-01-09 23:03:27.489834 xrpl-py-1.9.0b0/xrpl/core/keypairs/__init__.py
--rw-r--r--   0        0        0     1275 2022-08-01 03:07:06.921836 xrpl-py-1.9.0b0/xrpl/core/keypairs/crypto_implementation.py
--rw-r--r--   0        0        0     3595 2022-08-01 03:07:06.921941 xrpl-py-1.9.0b0/xrpl/core/keypairs/ed25519.py
--rw-r--r--   0        0        0      182 2022-08-01 03:07:06.921991 xrpl-py-1.9.0b0/xrpl/core/keypairs/exceptions.py
--rw-r--r--   0        0        0      893 2023-01-09 23:03:27.490087 xrpl-py-1.9.0b0/xrpl/core/keypairs/helpers.py
--rw-r--r--   0        0        0     4688 2022-08-01 03:07:06.922119 xrpl-py-1.9.0b0/xrpl/core/keypairs/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.922143 xrpl-py-1.9.0b0/xrpl/core/keypairs/py.typed
--rw-r--r--   0        0        0     7480 2022-08-01 03:07:06.922211 xrpl-py-1.9.0b0/xrpl/core/keypairs/secp256k1.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.922235 xrpl-py-1.9.0b0/xrpl/core/py.typed
--rw-r--r--   0        0        0      314 2022-08-01 03:07:06.922326 xrpl-py-1.9.0b0/xrpl/ledger/__init__.py
--rw-r--r--   0        0        0     2283 2022-08-01 03:07:06.922387 xrpl-py-1.9.0b0/xrpl/ledger/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.922410 xrpl-py-1.9.0b0/xrpl/ledger/py.typed
--rw-r--r--   0        0        0      997 2023-01-09 23:03:21.466231 xrpl-py-1.9.0b0/xrpl/models/__init__.py
--rw-r--r--   0        0        0      497 2022-08-01 03:07:06.922581 xrpl-py-1.9.0b0/xrpl/models/amounts/__init__.py
--rw-r--r--   0        0        0     1377 2022-08-01 03:07:06.922638 xrpl-py-1.9.0b0/xrpl/models/amounts/amount.py
--rw-r--r--   0        0        0     1349 2022-09-14 22:10:28.650164 xrpl-py-1.9.0b0/xrpl/models/amounts/issued_currency_amount.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.922737 xrpl-py-1.9.0b0/xrpl/models/amounts/py.typed
--rw-r--r--   0        0        0     2319 2023-01-09 22:47:59.324306 xrpl-py-1.9.0b0/xrpl/models/auth_account.py
--rw-r--r--   0        0        0    11018 2023-01-09 23:03:21.467241 xrpl-py-1.9.0b0/xrpl/models/base_model.py
--rw-r--r--   0        0        0      431 2023-01-09 22:47:59.325579 xrpl-py-1.9.0b0/xrpl/models/currencies/__init__.py
--rw-r--r--   0        0        0      319 2022-11-17 15:10:10.681283 xrpl-py-1.9.0b0/xrpl/models/currencies/currency.py
--rw-r--r--   0        0        0     1338 2023-01-09 22:47:59.326107 xrpl-py-1.9.0b0/xrpl/models/currencies/issue.py
--rw-r--r--   0        0        0     2237 2022-08-01 03:07:06.923061 xrpl-py-1.9.0b0/xrpl/models/currencies/issued_currency.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.923083 xrpl-py-1.9.0b0/xrpl/models/currencies/py.typed
--rw-r--r--   0        0        0     2500 2022-08-01 03:07:06.923150 xrpl-py-1.9.0b0/xrpl/models/currencies/xrp.py
--rw-r--r--   0        0        0      171 2022-08-01 03:07:06.923203 xrpl-py-1.9.0b0/xrpl/models/exceptions.py
--rw-r--r--   0        0        0     4835 2023-01-09 22:47:59.326811 xrpl-py-1.9.0b0/xrpl/models/flags.py
--rw-r--r--   0        0        0     2462 2023-01-09 23:03:27.490815 xrpl-py-1.9.0b0/xrpl/models/nested_model.py
--rw-r--r--   0        0        0     2088 2022-09-15 01:11:48.323392 xrpl-py-1.9.0b0/xrpl/models/path.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.923353 xrpl-py-1.9.0b0/xrpl/models/py.typed
--rw-r--r--   0        0        0     3561 2023-01-09 22:47:59.327832 xrpl-py-1.9.0b0/xrpl/models/requests/__init__.py
--rw-r--r--   0        0        0     1599 2022-08-01 03:07:06.923547 xrpl-py-1.9.0b0/xrpl/models/requests/account_channels.py
--rw-r--r--   0        0        0     1213 2022-08-01 03:07:06.923613 xrpl-py-1.9.0b0/xrpl/models/requests/account_currencies.py
--rw-r--r--   0        0        0     1166 2022-08-01 03:07:06.923671 xrpl-py-1.9.0b0/xrpl/models/requests/account_info.py
--rw-r--r--   0        0        0     1373 2022-08-01 03:07:06.923719 xrpl-py-1.9.0b0/xrpl/models/requests/account_lines.py
--rw-r--r--   0        0        0     1170 2022-08-01 03:07:06.923781 xrpl-py-1.9.0b0/xrpl/models/requests/account_nfts.py
--rw-r--r--   0        0        0     1870 2023-01-09 23:03:21.468405 xrpl-py-1.9.0b0/xrpl/models/requests/account_objects.py
--rw-r--r--   0        0        0     1211 2022-08-01 03:07:06.923885 xrpl-py-1.9.0b0/xrpl/models/requests/account_offers.py
--rw-r--r--   0        0        0     1257 2022-08-01 03:07:06.923930 xrpl-py-1.9.0b0/xrpl/models/requests/account_tx.py
--rw-r--r--   0        0        0     1014 2023-01-09 22:47:59.328117 xrpl-py-1.9.0b0/xrpl/models/requests/amm_info.py
--rw-r--r--   0        0        0     1074 2022-08-01 03:07:06.923987 xrpl-py-1.9.0b0/xrpl/models/requests/book_offers.py
--rw-r--r--   0        0        0     3020 2022-08-01 03:07:06.924055 xrpl-py-1.9.0b0/xrpl/models/requests/channel_authorize.py
--rw-r--r--   0        0        0     1130 2022-08-01 03:07:06.924111 xrpl-py-1.9.0b0/xrpl/models/requests/channel_verify.py
--rw-r--r--   0        0        0     1204 2022-08-01 03:07:06.924180 xrpl-py-1.9.0b0/xrpl/models/requests/deposit_authorized.py
--rw-r--r--   0        0        0      625 2022-08-01 03:07:06.924247 xrpl-py-1.9.0b0/xrpl/models/requests/federator_info.py
--rw-r--r--   0        0        0      775 2022-08-01 03:07:06.924306 xrpl-py-1.9.0b0/xrpl/models/requests/fee.py
--rw-r--r--   0        0        0     1119 2022-08-01 03:07:06.924384 xrpl-py-1.9.0b0/xrpl/models/requests/gateway_balances.py
--rw-r--r--   0        0        0     3068 2022-08-01 03:07:06.924450 xrpl-py-1.9.0b0/xrpl/models/requests/generic_request.py
--rw-r--r--   0        0        0      832 2022-08-01 03:07:06.924509 xrpl-py-1.9.0b0/xrpl/models/requests/ledger.py
--rw-r--r--   0        0        0      944 2022-08-01 03:07:06.924563 xrpl-py-1.9.0b0/xrpl/models/requests/ledger_closed.py
--rw-r--r--   0        0        0      726 2022-08-01 03:07:06.924621 xrpl-py-1.9.0b0/xrpl/models/requests/ledger_current.py
--rw-r--r--   0        0        0     1135 2022-08-01 03:07:06.924690 xrpl-py-1.9.0b0/xrpl/models/requests/ledger_data.py
--rw-r--r--   0        0        0     5703 2023-01-09 23:03:27.491203 xrpl-py-1.9.0b0/xrpl/models/requests/ledger_entry.py
--rw-r--r--   0        0        0      853 2022-08-01 03:07:06.924810 xrpl-py-1.9.0b0/xrpl/models/requests/manifest.py
--rw-r--r--   0        0        0      763 2022-08-01 03:07:06.924895 xrpl-py-1.9.0b0/xrpl/models/requests/nft_buy_offers.py
--rw-r--r--   0        0        0      770 2022-08-01 03:07:06.924953 xrpl-py-1.9.0b0/xrpl/models/requests/nft_sell_offers.py
--rw-r--r--   0        0        0     1496 2022-08-01 03:07:06.925015 xrpl-py-1.9.0b0/xrpl/models/requests/no_ripple_check.py
--rw-r--r--   0        0        0     4347 2022-08-01 03:07:06.925088 xrpl-py-1.9.0b0/xrpl/models/requests/path_find.py
--rw-r--r--   0        0        0      547 2022-08-01 03:07:06.925142 xrpl-py-1.9.0b0/xrpl/models/requests/ping.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.925165 xrpl-py-1.9.0b0/xrpl/models/requests/py.typed
--rw-r--r--   0        0        0      579 2022-08-01 03:07:06.925223 xrpl-py-1.9.0b0/xrpl/models/requests/random.py
--rw-r--r--   0        0        0     5691 2023-01-09 22:47:59.328662 xrpl-py-1.9.0b0/xrpl/models/requests/request.py
--rw-r--r--   0        0        0     2330 2022-08-01 03:07:06.925372 xrpl-py-1.9.0b0/xrpl/models/requests/ripple_path_find.py
--rw-r--r--   0        0        0      618 2022-08-01 03:07:06.925432 xrpl-py-1.9.0b0/xrpl/models/requests/server_info.py
--rw-r--r--   0        0        0     1194 2022-08-01 03:07:06.925493 xrpl-py-1.9.0b0/xrpl/models/requests/server_state.py
--rw-r--r--   0        0        0     4034 2022-08-01 03:07:06.925582 xrpl-py-1.9.0b0/xrpl/models/requests/sign.py
--rw-r--r--   0        0        0     5062 2022-08-01 03:07:06.925632 xrpl-py-1.9.0b0/xrpl/models/requests/sign_and_submit.py
--rw-r--r--   0        0        0     3274 2022-08-01 03:07:06.925686 xrpl-py-1.9.0b0/xrpl/models/requests/sign_for.py
--rw-r--r--   0        0        0     3758 2022-08-01 03:07:06.925767 xrpl-py-1.9.0b0/xrpl/models/requests/submit.py
--rw-r--r--   0        0        0     2478 2022-08-01 03:07:06.925860 xrpl-py-1.9.0b0/xrpl/models/requests/submit_multisigned.py
--rw-r--r--   0        0        0     2842 2022-08-01 03:07:06.925936 xrpl-py-1.9.0b0/xrpl/models/requests/submit_only.py
--rw-r--r--   0        0        0     2103 2022-08-01 03:07:06.926016 xrpl-py-1.9.0b0/xrpl/models/requests/subscribe.py
--rw-r--r--   0        0        0     1278 2022-08-01 03:07:06.926076 xrpl-py-1.9.0b0/xrpl/models/requests/transaction_entry.py
--rw-r--r--   0        0        0      817 2022-08-01 03:07:06.926139 xrpl-py-1.9.0b0/xrpl/models/requests/tx.py
--rw-r--r--   0        0        0     1595 2022-08-01 03:07:06.926195 xrpl-py-1.9.0b0/xrpl/models/requests/unsubscribe.py
--rw-r--r--   0        0        0      251 2022-08-01 03:07:06.926255 xrpl-py-1.9.0b0/xrpl/models/required.py
--rw-r--r--   0        0        0     3617 2022-08-01 03:07:06.926326 xrpl-py-1.9.0b0/xrpl/models/response.py
--rw-r--r--   0        0        0     4641 2023-01-09 23:03:21.469449 xrpl-py-1.9.0b0/xrpl/models/transactions/__init__.py
--rw-r--r--   0        0        0     1333 2022-08-01 03:07:06.926509 xrpl-py-1.9.0b0/xrpl/models/transactions/account_delete.py
--rw-r--r--   0        0        0     8629 2022-08-01 03:07:06.926615 xrpl-py-1.9.0b0/xrpl/models/transactions/account_set.py
--rw-r--r--   0        0        0     2641 2023-01-09 22:47:59.329792 xrpl-py-1.9.0b0/xrpl/models/transactions/amm_bid.py
--rw-r--r--   0        0        0     2135 2023-01-09 22:47:59.330301 xrpl-py-1.9.0b0/xrpl/models/transactions/amm_create.py
--rw-r--r--   0        0        0     3161 2023-01-09 22:47:59.330782 xrpl-py-1.9.0b0/xrpl/models/transactions/amm_deposit.py
--rw-r--r--   0        0        0     1981 2023-01-09 22:47:59.331133 xrpl-py-1.9.0b0/xrpl/models/transactions/amm_vote.py
--rw-r--r--   0        0        0     3283 2023-01-09 22:47:59.331513 xrpl-py-1.9.0b0/xrpl/models/transactions/amm_withdraw.py
--rw-r--r--   0        0        0     1101 2022-08-01 03:07:06.926693 xrpl-py-1.9.0b0/xrpl/models/transactions/check_cancel.py
--rw-r--r--   0        0        0     1993 2022-08-01 03:07:06.926771 xrpl-py-1.9.0b0/xrpl/models/transactions/check_cash.py
--rw-r--r--   0        0        0     1934 2022-08-01 03:07:06.926860 xrpl-py-1.9.0b0/xrpl/models/transactions/check_create.py
--rw-r--r--   0        0        0     1598 2022-08-01 03:07:06.926937 xrpl-py-1.9.0b0/xrpl/models/transactions/deposit_preauth.py
--rw-r--r--   0        0        0     1069 2022-08-01 03:07:06.927031 xrpl-py-1.9.0b0/xrpl/models/transactions/escrow_cancel.py
--rw-r--r--   0        0        0     2617 2022-08-01 03:07:06.927109 xrpl-py-1.9.0b0/xrpl/models/transactions/escrow_create.py
--rw-r--r--   0        0        0     2114 2022-08-01 03:07:06.927180 xrpl-py-1.9.0b0/xrpl/models/transactions/escrow_finish.py
--rw-r--r--   0        0        0     1923 2023-01-09 23:03:27.491471 xrpl-py-1.9.0b0/xrpl/models/transactions/metadata.py
--rw-r--r--   0        0        0     4537 2022-08-01 03:07:06.927331 xrpl-py-1.9.0b0/xrpl/models/transactions/nftoken_accept_offer.py
--rw-r--r--   0        0        0     1769 2022-08-01 03:07:06.927408 xrpl-py-1.9.0b0/xrpl/models/transactions/nftoken_burn.py
--rw-r--r--   0        0        0     2015 2022-08-01 03:07:06.927486 xrpl-py-1.9.0b0/xrpl/models/transactions/nftoken_cancel_offer.py
--rw-r--r--   0        0        0     4324 2022-08-01 03:07:06.927560 xrpl-py-1.9.0b0/xrpl/models/transactions/nftoken_create_offer.py
--rw-r--r--   0        0        0     4762 2022-08-09 19:51:34.686117 xrpl-py-1.9.0b0/xrpl/models/transactions/nftoken_mint.py
--rw-r--r--   0        0        0     1045 2022-08-01 03:07:06.927715 xrpl-py-1.9.0b0/xrpl/models/transactions/offer_cancel.py
--rw-r--r--   0        0        0     3866 2022-08-01 03:07:06.927795 xrpl-py-1.9.0b0/xrpl/models/transactions/offer_create.py
--rw-r--r--   0        0        0     5861 2022-08-01 03:07:06.927880 xrpl-py-1.9.0b0/xrpl/models/transactions/payment.py
--rw-r--r--   0        0        0     3917 2022-08-01 03:07:06.927963 xrpl-py-1.9.0b0/xrpl/models/transactions/payment_channel_claim.py
--rw-r--r--   0        0        0     2367 2022-08-01 03:07:06.928047 xrpl-py-1.9.0b0/xrpl/models/transactions/payment_channel_create.py
--rw-r--r--   0        0        0     1614 2022-08-01 03:07:06.928119 xrpl-py-1.9.0b0/xrpl/models/transactions/payment_channel_fund.py
--rw-r--r--   0        0        0      575 2022-08-01 03:07:06.928228 xrpl-py-1.9.0b0/xrpl/models/transactions/pseudo_transactions/__init__.py
--rw-r--r--   0        0        0     3651 2022-08-01 03:07:06.928326 xrpl-py-1.9.0b0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py
--rw-r--r--   0        0        0     1366 2022-08-01 03:07:06.928402 xrpl-py-1.9.0b0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py
--rw-r--r--   0        0        0     1874 2022-08-01 03:07:06.928467 xrpl-py-1.9.0b0/xrpl/models/transactions/pseudo_transactions/set_fee.py
--rw-r--r--   0        0        0     2262 2022-08-01 03:07:06.928526 xrpl-py-1.9.0b0/xrpl/models/transactions/pseudo_transactions/unl_modify.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.928554 xrpl-py-1.9.0b0/xrpl/models/transactions/py.typed
--rw-r--r--   0        0        0      959 2022-08-01 03:07:06.928643 xrpl-py-1.9.0b0/xrpl/models/transactions/set_regular_key.py
--rw-r--r--   0        0        0     4747 2022-09-15 19:56:17.566655 xrpl-py-1.9.0b0/xrpl/models/transactions/signer_list_set.py
--rw-r--r--   0        0        0      959 2022-08-01 03:07:06.928817 xrpl-py-1.9.0b0/xrpl/models/transactions/ticket_create.py
--rw-r--r--   0        0        0    14629 2023-01-09 23:03:27.491747 xrpl-py-1.9.0b0/xrpl/models/transactions/transaction.py
--rw-r--r--   0        0        0     2425 2022-08-01 03:07:06.929079 xrpl-py-1.9.0b0/xrpl/models/transactions/trust_set.py
--rw-r--r--   0        0        0      275 2022-08-01 03:07:06.929186 xrpl-py-1.9.0b0/xrpl/models/transactions/types/__init__.py
--rw-r--r--   0        0        0      287 2022-08-01 03:07:06.929265 xrpl-py-1.9.0b0/xrpl/models/transactions/types/pseudo_transaction_type.py
--rw-r--r--   0        0        0     1540 2023-01-09 23:03:21.470966 xrpl-py-1.9.0b0/xrpl/models/transactions/types/transaction_type.py
--rw-r--r--   0        0        0     1363 2023-01-09 23:03:27.491989 xrpl-py-1.9.0b0/xrpl/models/transactions/xchain_account_create_commit.py
--rw-r--r--   0        0        0     3167 2023-01-09 23:03:27.492272 xrpl-py-1.9.0b0/xrpl/models/transactions/xchain_add_attestation.py
--rw-r--r--   0        0        0     1534 2023-01-09 23:03:27.492552 xrpl-py-1.9.0b0/xrpl/models/transactions/xchain_claim.py
--rw-r--r--   0        0        0      908 2023-01-09 23:03:21.471836 xrpl-py-1.9.0b0/xrpl/models/transactions/xchain_commit.py
--rw-r--r--   0        0        0     2393 2023-01-09 23:03:27.492761 xrpl-py-1.9.0b0/xrpl/models/transactions/xchain_create_bridge.py
--rw-r--r--   0        0        0     1421 2023-01-09 23:03:27.492965 xrpl-py-1.9.0b0/xrpl/models/transactions/xchain_create_claim_id.py
--rw-r--r--   0        0        0     2228 2023-01-09 23:03:27.493143 xrpl-py-1.9.0b0/xrpl/models/transactions/xchain_modify_bridge.py
--rw-r--r--   0        0        0      749 2022-08-01 03:07:06.929418 xrpl-py-1.9.0b0/xrpl/models/types.py
--rw-r--r--   0        0        0     2174 2022-08-01 03:07:06.929500 xrpl-py-1.9.0b0/xrpl/models/utils.py
--rw-r--r--   0        0        0      532 2023-01-09 23:03:21.473406 xrpl-py-1.9.0b0/xrpl/models/xchain_bridge.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.929533 xrpl-py-1.9.0b0/xrpl/py.typed
--rw-r--r--   0        0        0     1024 2023-01-09 23:03:27.493372 xrpl-py-1.9.0b0/xrpl/transaction/__init__.py
--rw-r--r--   0        0        0     1951 2023-01-09 23:03:27.493660 xrpl-py-1.9.0b0/xrpl/transaction/ledger.py
--rw-r--r--   0        0        0     4259 2023-01-09 23:03:27.493938 xrpl-py-1.9.0b0/xrpl/transaction/main.py
--rw-r--r--   0        0        0     1071 2023-01-09 23:03:27.494085 xrpl-py-1.9.0b0/xrpl/transaction/multisign.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.929779 xrpl-py-1.9.0b0/xrpl/transaction/py.typed
--rw-r--r--   0        0        0     1163 2022-08-01 03:07:06.929854 xrpl-py-1.9.0b0/xrpl/transaction/reliable_submission.py
--rw-r--r--   0        0        0      933 2022-08-01 03:07:06.929961 xrpl-py-1.9.0b0/xrpl/utils/__init__.py
--rw-r--r--   0        0        0     3412 2022-08-01 03:07:06.930042 xrpl-py-1.9.0b0/xrpl/utils/parse_nftoken_id.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.930069 xrpl-py-1.9.0b0/xrpl/utils/py.typed
--rw-r--r--   0        0        0     1537 2022-08-01 03:07:06.930152 xrpl-py-1.9.0b0/xrpl/utils/sidechain.py
--rw-r--r--   0        0        0      788 2022-08-01 03:07:06.930218 xrpl-py-1.9.0b0/xrpl/utils/str_conversions.py
--rw-r--r--   0        0        0     4202 2022-08-01 03:07:06.930296 xrpl-py-1.9.0b0/xrpl/utils/time_conversions.py
--rw-r--r--   0        0        0      350 2022-08-01 03:07:06.930405 xrpl-py-1.9.0b0/xrpl/utils/txn_parser/__init__.py
--rw-r--r--   0        0        0     1717 2022-08-01 03:07:06.930477 xrpl-py-1.9.0b0/xrpl/utils/txn_parser/get_balance_changes.py
--rw-r--r--   0        0        0     1446 2022-08-01 03:07:06.930538 xrpl-py-1.9.0b0/xrpl/utils/txn_parser/get_final_balances.py
--rw-r--r--   0        0        0      641 2022-08-01 03:07:06.930603 xrpl-py-1.9.0b0/xrpl/utils/txn_parser/get_order_book_changes.py
--rw-r--r--   0        0        0      627 2022-08-01 03:07:06.930692 xrpl-py-1.9.0b0/xrpl/utils/txn_parser/utils/__init__.py
--rw-r--r--   0        0        0     5218 2022-08-01 03:07:06.930789 xrpl-py-1.9.0b0/xrpl/utils/txn_parser/utils/balance_parser.py
--rw-r--r--   0        0        0     2518 2023-01-09 23:03:27.494325 xrpl-py-1.9.0b0/xrpl/utils/txn_parser/utils/nodes.py
--rw-r--r--   0        0        0     6191 2022-08-01 03:07:06.930936 xrpl-py-1.9.0b0/xrpl/utils/txn_parser/utils/order_book_parser.py
--rw-r--r--   0        0        0     1192 2022-08-01 03:07:06.931006 xrpl-py-1.9.0b0/xrpl/utils/txn_parser/utils/parser.py
--rw-r--r--   0        0        0     1404 2023-01-09 23:03:27.494567 xrpl-py-1.9.0b0/xrpl/utils/txn_parser/utils/types.py
--rw-r--r--   0        0        0     3476 2022-08-01 03:07:06.931171 xrpl-py-1.9.0b0/xrpl/utils/xrp_conversions.py
--rw-r--r--   0        0        0      269 2022-08-01 03:07:06.931262 xrpl-py-1.9.0b0/xrpl/wallet/__init__.py
--rw-r--r--   0        0        0     3552 2023-01-09 23:03:21.475113 xrpl-py-1.9.0b0/xrpl/wallet/main.py
--rw-r--r--   0        0        0        0 2022-08-01 03:07:06.931385 xrpl-py-1.9.0b0/xrpl/wallet/py.typed
--rw-r--r--   0        0        0     1370 2022-08-01 03:07:06.931452 xrpl-py-1.9.0b0/xrpl/wallet/wallet_generation.py
--rw-r--r--   0        0        0    18342 2023-01-10 21:42:12.614357 xrpl-py-1.9.0b0/setup.py
--rw-r--r--   0        0        0    17300 2023-01-10 21:42:12.614992 xrpl-py-1.9.0b0/PKG-INFO
+-rw-r--r--   0        0        0      740 2021-07-28 20:35:08.759607 xrpl-py-2.0.0b0/LICENSE
+-rw-r--r--   0        0        0    15971 2022-12-15 20:10:31.004701 xrpl-py-2.0.0b0/README.md
+-rw-r--r--   0        0        0     2234 2022-12-15 20:19:30.899020 xrpl-py-2.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0      348 2021-07-28 20:35:08.796326 xrpl-py-2.0.0b0/xrpl/__init__.py
+-rw-r--r--   0        0        0      588 2022-09-15 21:17:14.712442 xrpl-py-2.0.0b0/xrpl/account/__init__.py
+-rw-r--r--   0        0        0     4410 2022-12-15 20:10:31.050399 xrpl-py-2.0.0b0/xrpl/account/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.923644 xrpl-py-2.0.0b0/xrpl/account/py.typed
+-rw-r--r--   0        0        0     2692 2022-12-15 20:10:31.051202 xrpl-py-2.0.0b0/xrpl/account/transaction_history.py
+-rw-r--r--   0        0        0      189 2021-07-28 20:35:08.798278 xrpl-py-2.0.0b0/xrpl/asyncio/__init__.py
+-rw-r--r--   0        0        0      610 2021-07-28 20:35:08.798757 xrpl-py-2.0.0b0/xrpl/asyncio/account/__init__.py
+-rw-r--r--   0        0        0     5885 2022-12-15 20:10:31.052617 xrpl-py-2.0.0b0/xrpl/asyncio/account/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.923758 xrpl-py-2.0.0b0/xrpl/asyncio/account/py.typed
+-rw-r--r--   0        0        0     3432 2022-12-15 20:10:31.053536 xrpl-py-2.0.0b0/xrpl/asyncio/account/transaction_history.py
+-rw-r--r--   0        0        0      705 2022-04-05 18:02:24.758557 xrpl-py-2.0.0b0/xrpl/asyncio/clients/__init__.py
+-rw-r--r--   0        0        0      692 2022-12-15 20:10:31.054509 xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_client.py
+-rw-r--r--   0        0        0      315 2021-07-28 20:35:08.800248 xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_json_rpc_client.py
+-rw-r--r--   0        0        0     7099 2022-12-15 20:10:31.055584 xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_websocket_client.py
+-rw-r--r--   0        0        0     1066 2022-12-15 20:10:31.056911 xrpl-py-2.0.0b0/xrpl/asyncio/clients/client.py
+-rw-r--r--   0        0        0     1083 2021-07-28 20:35:08.801049 xrpl-py-2.0.0b0/xrpl/asyncio/clients/exceptions.py
+-rw-r--r--   0        0        0     1612 2022-12-15 20:10:31.057676 xrpl-py-2.0.0b0/xrpl/asyncio/clients/json_rpc_base.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.923862 xrpl-py-2.0.0b0/xrpl/asyncio/clients/py.typed
+-rw-r--r--   0        0        0     3341 2021-12-07 22:32:02.034730 xrpl-py-2.0.0b0/xrpl/asyncio/clients/utils.py
+-rw-r--r--   0        0        0     7431 2022-12-15 20:10:31.058266 xrpl-py-2.0.0b0/xrpl/asyncio/clients/websocket_base.py
+-rw-r--r--   0        0        0      328 2021-07-28 20:35:08.802964 xrpl-py-2.0.0b0/xrpl/asyncio/ledger/__init__.py
+-rw-r--r--   0        0        0     3443 2022-12-15 20:10:31.059029 xrpl-py-2.0.0b0/xrpl/asyncio/ledger/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.923951 xrpl-py-2.0.0b0/xrpl/asyncio/ledger/py.typed
+-rw-r--r--   0        0        0     2353 2022-04-26 22:13:55.274282 xrpl-py-2.0.0b0/xrpl/asyncio/ledger/utils.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924038 xrpl-py-2.0.0b0/xrpl/asyncio/py.typed
+-rw-r--r--   0        0        0      956 2022-12-15 20:10:31.059741 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/__init__.py
+-rw-r--r--   0        0        0     2077 2022-12-15 20:10:31.060567 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/ledger.py
+-rw-r--r--   0        0        0    12247 2022-12-15 20:10:31.061290 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924123 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/py.typed
+-rw-r--r--   0        0        0     3606 2022-12-15 20:10:31.062028 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/reliable_submission.py
+-rw-r--r--   0        0        0      219 2021-07-28 20:35:08.805165 xrpl-py-2.0.0b0/xrpl/asyncio/wallet/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924197 xrpl-py-2.0.0b0/xrpl/asyncio/wallet/py.typed
+-rw-r--r--   0        0        0     5657 2022-12-15 20:10:31.062888 xrpl-py-2.0.0b0/xrpl/asyncio/wallet/wallet_generation.py
+-rw-r--r--   0        0        0      656 2021-07-28 20:35:08.805912 xrpl-py-2.0.0b0/xrpl/clients/__init__.py
+-rw-r--r--   0        0        0      295 2021-07-28 20:35:08.806161 xrpl-py-2.0.0b0/xrpl/clients/json_rpc_client.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924276 xrpl-py-2.0.0b0/xrpl/clients/py.typed
+-rw-r--r--   0        0        0      705 2022-12-15 20:10:31.064928 xrpl-py-2.0.0b0/xrpl/clients/sync_client.py
+-rw-r--r--   0        0        0     8780 2022-12-15 20:10:31.065768 xrpl-py-2.0.0b0/xrpl/clients/websocket_client.py
+-rw-r--r--   0        0        0     1414 2022-07-28 00:01:58.132202 xrpl-py-2.0.0b0/xrpl/constants.py
+-rw-r--r--   0        0        0      171 2021-07-28 20:35:08.807482 xrpl-py-2.0.0b0/xrpl/core/__init__.py
+-rw-r--r--   0        0        0     1131 2022-12-15 20:10:31.067161 xrpl-py-2.0.0b0/xrpl/core/addresscodec/__init__.py
+-rw-r--r--   0        0        0     7175 2022-08-23 17:19:34.990879 xrpl-py-2.0.0b0/xrpl/core/addresscodec/codec.py
+-rw-r--r--   0        0        0      194 2021-07-28 20:35:08.808480 xrpl-py-2.0.0b0/xrpl/core/addresscodec/exceptions.py
+-rw-r--r--   0        0        0     5735 2022-12-15 20:10:31.067991 xrpl-py-2.0.0b0/xrpl/core/addresscodec/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924387 xrpl-py-2.0.0b0/xrpl/core/addresscodec/py.typed
+-rw-r--r--   0        0        0      235 2021-07-28 20:35:08.808987 xrpl-py-2.0.0b0/xrpl/core/addresscodec/utils.py
+-rw-r--r--   0        0        0      488 2021-07-28 20:35:08.809400 xrpl-py-2.0.0b0/xrpl/core/binarycodec/__init__.py
+-rw-r--r--   0        0        0      296 2021-07-28 20:35:08.809791 xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/__init__.py
+-rw-r--r--   0        0        0     9076 2021-07-28 20:35:08.810078 xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py
+-rw-r--r--   0        0        0     4650 2021-12-07 22:32:02.051210 xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py
+-rw-r--r--   0        0        0     1025 2021-07-28 20:35:08.810736 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/__init__.py
+-rw-r--r--   0        0        0    44971 2022-08-23 17:19:34.991511 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/definitions.json
+-rw-r--r--   0        0        0     8431 2021-07-28 20:35:08.811725 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/definitions.py
+-rw-r--r--   0        0        0     1870 2021-07-28 20:35:08.812068 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_header.py
+-rw-r--r--   0        0        0     1192 2021-07-28 20:35:08.812380 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_info.py
+-rw-r--r--   0        0        0     1931 2022-07-05 22:56:20.051355 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_instance.py
+-rw-r--r--   0        0        0      191 2021-07-28 20:35:08.813180 xrpl-py-2.0.0b0/xrpl/core/binarycodec/exceptions.py
+-rw-r--r--   0        0        0     3942 2021-07-28 20:35:08.813524 xrpl-py-2.0.0b0/xrpl/core/binarycodec/field_id_codec.py
+-rw-r--r--   0        0        0     3708 2022-07-05 22:56:20.052317 xrpl-py-2.0.0b0/xrpl/core/binarycodec/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924565 xrpl-py-2.0.0b0/xrpl/core/binarycodec/py.typed
+-rw-r--r--   0        0        0     1255 2022-07-05 22:56:20.053538 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/__init__.py
+-rw-r--r--   0        0        0     2956 2022-01-20 00:05:30.497701 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/account_id.py
+-rw-r--r--   0        0        0    11234 2021-12-17 23:17:45.558659 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/amount.py
+-rw-r--r--   0        0        0     1950 2021-07-28 20:35:08.815354 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/blob.py
+-rw-r--r--   0        0        0     4347 2021-12-07 22:32:02.058589 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/currency.py
+-rw-r--r--   0        0        0     2640 2021-12-07 22:32:02.059722 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash.py
+-rw-r--r--   0        0        0      572 2021-07-28 20:35:08.816233 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash128.py
+-rw-r--r--   0        0        0      571 2021-07-28 20:35:08.816481 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash160.py
+-rw-r--r--   0        0        0      572 2021-07-28 20:35:08.816714 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash256.py
+-rw-r--r--   0        0        0     9067 2021-07-28 20:35:08.817068 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/path_set.py
+-rw-r--r--   0        0        0     2493 2022-07-05 22:56:20.055452 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/serialized_type.py
+-rw-r--r--   0        0        0     3301 2022-07-05 22:56:20.055743 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/st_array.py
+-rw-r--r--   0        0        0     8394 2022-07-05 22:56:20.056024 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/st_object.py
+-rw-r--r--   0        0        0     3383 2021-07-28 20:35:08.818405 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint.py
+-rw-r--r--   0        0        0     2063 2021-07-28 20:35:08.818693 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint16.py
+-rw-r--r--   0        0        0     2283 2021-07-28 20:35:08.819029 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint32.py
+-rw-r--r--   0        0        0     2854 2022-01-20 00:05:30.500382 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint64.py
+-rw-r--r--   0        0        0     1994 2021-07-28 20:35:08.819489 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint8.py
+-rw-r--r--   0        0        0     2905 2021-07-28 20:35:08.819794 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/vector256.py
+-rw-r--r--   0        0        0      447 2022-12-15 20:10:31.069734 xrpl-py-2.0.0b0/xrpl/core/keypairs/__init__.py
+-rw-r--r--   0        0        0     1275 2021-07-28 20:35:08.820427 xrpl-py-2.0.0b0/xrpl/core/keypairs/crypto_implementation.py
+-rw-r--r--   0        0        0     3662 2022-12-15 20:10:31.070556 xrpl-py-2.0.0b0/xrpl/core/keypairs/ed25519.py
+-rw-r--r--   0        0        0      182 2021-07-28 20:35:08.820941 xrpl-py-2.0.0b0/xrpl/core/keypairs/exceptions.py
+-rw-r--r--   0        0        0      893 2022-12-15 20:10:31.071456 xrpl-py-2.0.0b0/xrpl/core/keypairs/helpers.py
+-rw-r--r--   0        0        0     4788 2022-12-15 20:10:31.072827 xrpl-py-2.0.0b0/xrpl/core/keypairs/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924715 xrpl-py-2.0.0b0/xrpl/core/keypairs/py.typed
+-rw-r--r--   0        0        0     7480 2022-07-28 00:01:58.132708 xrpl-py-2.0.0b0/xrpl/core/keypairs/secp256k1.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924787 xrpl-py-2.0.0b0/xrpl/core/py.typed
+-rw-r--r--   0        0        0      314 2021-07-28 20:35:08.822692 xrpl-py-2.0.0b0/xrpl/ledger/__init__.py
+-rw-r--r--   0        0        0     2283 2022-04-26 22:13:55.277744 xrpl-py-2.0.0b0/xrpl/ledger/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924863 xrpl-py-2.0.0b0/xrpl/ledger/py.typed
+-rw-r--r--   0        0        0      858 2021-12-17 21:23:35.552124 xrpl-py-2.0.0b0/xrpl/models/__init__.py
+-rw-r--r--   0        0        0      497 2021-12-17 23:17:45.561082 xrpl-py-2.0.0b0/xrpl/models/amounts/__init__.py
+-rw-r--r--   0        0        0     1377 2021-12-17 23:17:45.561971 xrpl-py-2.0.0b0/xrpl/models/amounts/amount.py
+-rw-r--r--   0        0        0     1349 2021-12-17 21:23:35.554848 xrpl-py-2.0.0b0/xrpl/models/amounts/issued_currency_amount.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924950 xrpl-py-2.0.0b0/xrpl/models/amounts/py.typed
+-rw-r--r--   0        0        0    10663 2022-07-05 22:56:20.059672 xrpl-py-2.0.0b0/xrpl/models/base_model.py
+-rw-r--r--   0        0        0      371 2021-07-28 20:35:08.825266 xrpl-py-2.0.0b0/xrpl/models/currencies/__init__.py
+-rw-r--r--   0        0        0      319 2021-07-28 20:35:08.825634 xrpl-py-2.0.0b0/xrpl/models/currencies/currency.py
+-rw-r--r--   0        0        0     2237 2021-12-17 21:23:35.557608 xrpl-py-2.0.0b0/xrpl/models/currencies/issued_currency.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925039 xrpl-py-2.0.0b0/xrpl/models/currencies/py.typed
+-rw-r--r--   0        0        0     2500 2021-12-17 21:23:35.558615 xrpl-py-2.0.0b0/xrpl/models/currencies/xrp.py
+-rw-r--r--   0        0        0      171 2021-07-28 20:35:08.826501 xrpl-py-2.0.0b0/xrpl/models/exceptions.py
+-rw-r--r--   0        0        0     4300 2022-04-25 18:39:06.767427 xrpl-py-2.0.0b0/xrpl/models/flags.py
+-rw-r--r--   0        0        0     2462 2022-12-15 20:10:31.074348 xrpl-py-2.0.0b0/xrpl/models/nested_model.py
+-rw-r--r--   0        0        0     2088 2021-07-28 20:35:08.826856 xrpl-py-2.0.0b0/xrpl/models/path.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925126 xrpl-py-2.0.0b0/xrpl/models/py.typed
+-rw-r--r--   0        0        0     3428 2022-06-02 20:58:35.644160 xrpl-py-2.0.0b0/xrpl/models/requests/__init__.py
+-rw-r--r--   0        0        0     1599 2021-07-28 20:35:08.828304 xrpl-py-2.0.0b0/xrpl/models/requests/account_channels.py
+-rw-r--r--   0        0        0     1213 2021-07-28 20:35:08.828881 xrpl-py-2.0.0b0/xrpl/models/requests/account_currencies.py
+-rw-r--r--   0        0        0     1166 2021-07-28 20:35:08.829260 xrpl-py-2.0.0b0/xrpl/models/requests/account_info.py
+-rw-r--r--   0        0        0     1373 2021-07-28 20:35:08.829871 xrpl-py-2.0.0b0/xrpl/models/requests/account_lines.py
+-rw-r--r--   0        0        0     1170 2021-12-17 23:17:45.563593 xrpl-py-2.0.0b0/xrpl/models/requests/account_nfts.py
+-rw-r--r--   0        0        0     1760 2021-07-28 20:35:08.830168 xrpl-py-2.0.0b0/xrpl/models/requests/account_objects.py
+-rw-r--r--   0        0        0     1211 2021-07-28 20:35:08.830415 xrpl-py-2.0.0b0/xrpl/models/requests/account_offers.py
+-rw-r--r--   0        0        0     1257 2021-07-28 20:35:08.830671 xrpl-py-2.0.0b0/xrpl/models/requests/account_tx.py
+-rw-r--r--   0        0        0     1074 2021-07-28 20:35:08.830942 xrpl-py-2.0.0b0/xrpl/models/requests/book_offers.py
+-rw-r--r--   0        0        0     3020 2021-07-28 20:35:08.831227 xrpl-py-2.0.0b0/xrpl/models/requests/channel_authorize.py
+-rw-r--r--   0        0        0     1130 2021-07-28 20:35:08.831559 xrpl-py-2.0.0b0/xrpl/models/requests/channel_verify.py
+-rw-r--r--   0        0        0     1204 2021-07-28 20:35:08.831844 xrpl-py-2.0.0b0/xrpl/models/requests/deposit_authorized.py
+-rw-r--r--   0        0        0      625 2022-04-05 18:02:24.759920 xrpl-py-2.0.0b0/xrpl/models/requests/federator_info.py
+-rw-r--r--   0        0        0      775 2021-07-28 20:35:08.832085 xrpl-py-2.0.0b0/xrpl/models/requests/fee.py
+-rw-r--r--   0        0        0     1119 2021-07-28 20:35:08.832292 xrpl-py-2.0.0b0/xrpl/models/requests/gateway_balances.py
+-rw-r--r--   0        0        0     3068 2022-06-02 20:58:35.644917 xrpl-py-2.0.0b0/xrpl/models/requests/generic_request.py
+-rw-r--r--   0        0        0      832 2021-07-28 20:35:08.832476 xrpl-py-2.0.0b0/xrpl/models/requests/ledger.py
+-rw-r--r--   0        0        0      944 2021-07-28 20:35:08.832645 xrpl-py-2.0.0b0/xrpl/models/requests/ledger_closed.py
+-rw-r--r--   0        0        0      726 2021-07-28 20:35:08.832891 xrpl-py-2.0.0b0/xrpl/models/requests/ledger_current.py
+-rw-r--r--   0        0        0     1135 2021-07-28 20:35:08.833259 xrpl-py-2.0.0b0/xrpl/models/requests/ledger_data.py
+-rw-r--r--   0        0        0     4643 2021-07-28 20:35:08.833563 xrpl-py-2.0.0b0/xrpl/models/requests/ledger_entry.py
+-rw-r--r--   0        0        0      853 2021-07-28 20:35:08.833795 xrpl-py-2.0.0b0/xrpl/models/requests/manifest.py
+-rw-r--r--   0        0        0      763 2022-04-25 18:39:06.768162 xrpl-py-2.0.0b0/xrpl/models/requests/nft_buy_offers.py
+-rw-r--r--   0        0        0      770 2022-04-25 18:39:06.768739 xrpl-py-2.0.0b0/xrpl/models/requests/nft_sell_offers.py
+-rw-r--r--   0        0        0     1496 2021-07-28 20:35:08.834038 xrpl-py-2.0.0b0/xrpl/models/requests/no_ripple_check.py
+-rw-r--r--   0        0        0     4347 2021-07-28 20:35:08.834320 xrpl-py-2.0.0b0/xrpl/models/requests/path_find.py
+-rw-r--r--   0        0        0      547 2021-07-28 20:35:08.834534 xrpl-py-2.0.0b0/xrpl/models/requests/ping.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925225 xrpl-py-2.0.0b0/xrpl/models/requests/py.typed
+-rw-r--r--   0        0        0      579 2021-07-28 20:35:08.834709 xrpl-py-2.0.0b0/xrpl/models/requests/random.py
+-rw-r--r--   0        0        0     5646 2022-07-05 22:56:20.061515 xrpl-py-2.0.0b0/xrpl/models/requests/request.py
+-rw-r--r--   0        0        0     2330 2021-07-28 20:35:08.835181 xrpl-py-2.0.0b0/xrpl/models/requests/ripple_path_find.py
+-rw-r--r--   0        0        0      618 2021-07-28 20:35:08.835452 xrpl-py-2.0.0b0/xrpl/models/requests/server_info.py
+-rw-r--r--   0        0        0     1194 2021-07-28 20:35:08.835707 xrpl-py-2.0.0b0/xrpl/models/requests/server_state.py
+-rw-r--r--   0        0        0     4034 2022-07-05 22:56:20.063692 xrpl-py-2.0.0b0/xrpl/models/requests/sign.py
+-rw-r--r--   0        0        0     5062 2022-07-05 22:56:20.065263 xrpl-py-2.0.0b0/xrpl/models/requests/sign_and_submit.py
+-rw-r--r--   0        0        0     3274 2022-07-05 22:56:20.066563 xrpl-py-2.0.0b0/xrpl/models/requests/sign_for.py
+-rw-r--r--   0        0        0     3758 2022-07-05 22:56:20.068102 xrpl-py-2.0.0b0/xrpl/models/requests/submit.py
+-rw-r--r--   0        0        0     2478 2022-07-05 22:56:20.069204 xrpl-py-2.0.0b0/xrpl/models/requests/submit_multisigned.py
+-rw-r--r--   0        0        0     2842 2021-07-28 20:35:08.836916 xrpl-py-2.0.0b0/xrpl/models/requests/submit_only.py
+-rw-r--r--   0        0        0     2103 2021-07-28 20:35:08.837120 xrpl-py-2.0.0b0/xrpl/models/requests/subscribe.py
+-rw-r--r--   0        0        0     1278 2021-07-28 20:35:08.837698 xrpl-py-2.0.0b0/xrpl/models/requests/transaction_entry.py
+-rw-r--r--   0        0        0      817 2021-07-28 20:35:08.838021 xrpl-py-2.0.0b0/xrpl/models/requests/tx.py
+-rw-r--r--   0        0        0     1595 2021-07-28 20:35:08.838365 xrpl-py-2.0.0b0/xrpl/models/requests/unsubscribe.py
+-rw-r--r--   0        0        0      251 2021-07-28 20:35:08.838692 xrpl-py-2.0.0b0/xrpl/models/required.py
+-rw-r--r--   0        0        0     3617 2021-12-07 22:32:02.066250 xrpl-py-2.0.0b0/xrpl/models/response.py
+-rw-r--r--   0        0        0     3293 2022-06-02 20:58:35.645480 xrpl-py-2.0.0b0/xrpl/models/transactions/__init__.py
+-rw-r--r--   0        0        0     1333 2021-07-28 20:35:08.839736 xrpl-py-2.0.0b0/xrpl/models/transactions/account_delete.py
+-rw-r--r--   0        0        0     8629 2022-04-25 18:40:11.716081 xrpl-py-2.0.0b0/xrpl/models/transactions/account_set.py
+-rw-r--r--   0        0        0     1101 2021-07-28 20:35:08.840429 xrpl-py-2.0.0b0/xrpl/models/transactions/check_cancel.py
+-rw-r--r--   0        0        0     1993 2021-07-28 20:35:08.840706 xrpl-py-2.0.0b0/xrpl/models/transactions/check_cash.py
+-rw-r--r--   0        0        0     1934 2021-07-28 20:35:08.841015 xrpl-py-2.0.0b0/xrpl/models/transactions/check_create.py
+-rw-r--r--   0        0        0     1598 2021-07-28 20:35:08.841280 xrpl-py-2.0.0b0/xrpl/models/transactions/deposit_preauth.py
+-rw-r--r--   0        0        0     1069 2021-07-28 20:35:08.841539 xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_cancel.py
+-rw-r--r--   0        0        0     2617 2021-07-28 20:35:08.841747 xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_create.py
+-rw-r--r--   0        0        0     2114 2021-07-28 20:35:08.841923 xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_finish.py
+-rw-r--r--   0        0        0     1923 2022-12-15 20:10:31.075374 xrpl-py-2.0.0b0/xrpl/models/transactions/metadata.py
+-rw-r--r--   0        0        0     4537 2022-04-25 18:39:06.770393 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_accept_offer.py
+-rw-r--r--   0        0        0     1769 2022-04-25 18:39:06.771370 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_burn.py
+-rw-r--r--   0        0        0     2015 2022-04-25 18:39:06.771874 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_cancel_offer.py
+-rw-r--r--   0        0        0     4324 2022-04-25 18:40:20.537837 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_create_offer.py
+-rw-r--r--   0        0        0     4762 2022-04-25 18:40:11.718521 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_mint.py
+-rw-r--r--   0        0        0     1045 2021-07-28 20:35:08.842102 xrpl-py-2.0.0b0/xrpl/models/transactions/offer_cancel.py
+-rw-r--r--   0        0        0     3866 2022-04-25 18:40:11.719936 xrpl-py-2.0.0b0/xrpl/models/transactions/offer_create.py
+-rw-r--r--   0        0        0     5861 2022-04-25 18:40:11.721475 xrpl-py-2.0.0b0/xrpl/models/transactions/payment.py
+-rw-r--r--   0        0        0     3917 2022-04-25 18:40:11.722725 xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_claim.py
+-rw-r--r--   0        0        0     2367 2021-07-28 20:35:08.843065 xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_create.py
+-rw-r--r--   0        0        0     1614 2021-07-28 20:35:08.843590 xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_fund.py
+-rw-r--r--   0        0        0      575 2022-04-05 18:02:24.769631 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/__init__.py
+-rw-r--r--   0        0        0     3651 2022-04-05 18:02:24.770653 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py
+-rw-r--r--   0        0        0     1366 2021-07-28 20:35:08.845018 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py
+-rw-r--r--   0        0        0     1874 2021-07-28 20:35:08.845329 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/set_fee.py
+-rw-r--r--   0        0        0     2262 2021-07-28 20:35:08.845606 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/unl_modify.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925358 xrpl-py-2.0.0b0/xrpl/models/transactions/py.typed
+-rw-r--r--   0        0        0      959 2021-07-28 20:35:08.845886 xrpl-py-2.0.0b0/xrpl/models/transactions/set_regular_key.py
+-rw-r--r--   0        0        0     4747 2022-09-15 21:17:23.562048 xrpl-py-2.0.0b0/xrpl/models/transactions/signer_list_set.py
+-rw-r--r--   0        0        0      959 2021-12-07 22:32:02.070889 xrpl-py-2.0.0b0/xrpl/models/transactions/ticket_create.py
+-rw-r--r--   0        0        0    14500 2022-09-15 21:17:23.562911 xrpl-py-2.0.0b0/xrpl/models/transactions/transaction.py
+-rw-r--r--   0        0        0     2425 2022-04-25 18:40:11.724215 xrpl-py-2.0.0b0/xrpl/models/transactions/trust_set.py
+-rw-r--r--   0        0        0      275 2021-07-28 20:35:08.847122 xrpl-py-2.0.0b0/xrpl/models/transactions/types/__init__.py
+-rw-r--r--   0        0        0      287 2021-07-28 20:35:08.847388 xrpl-py-2.0.0b0/xrpl/models/transactions/types/pseudo_transaction_type.py
+-rw-r--r--   0        0        0     1069 2021-12-17 23:17:45.570774 xrpl-py-2.0.0b0/xrpl/models/transactions/types/transaction_type.py
+-rw-r--r--   0        0        0      749 2021-12-17 23:17:45.571050 xrpl-py-2.0.0b0/xrpl/models/types.py
+-rw-r--r--   0        0        0     2174 2021-12-17 21:23:35.561520 xrpl-py-2.0.0b0/xrpl/models/utils.py
+-rw-r--r--   0        0        0        0 2021-12-07 22:32:02.074339 xrpl-py-2.0.0b0/xrpl/py.typed
+-rw-r--r--   0        0        0      958 2022-12-15 20:10:31.076208 xrpl-py-2.0.0b0/xrpl/transaction/__init__.py
+-rw-r--r--   0        0        0     1951 2022-12-15 20:10:31.079134 xrpl-py-2.0.0b0/xrpl/transaction/ledger.py
+-rw-r--r--   0        0        0     3896 2022-12-15 20:10:31.080226 xrpl-py-2.0.0b0/xrpl/transaction/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925547 xrpl-py-2.0.0b0/xrpl/transaction/py.typed
+-rw-r--r--   0        0        0     1163 2021-12-07 22:32:02.077113 xrpl-py-2.0.0b0/xrpl/transaction/reliable_submission.py
+-rw-r--r--   0        0        0      933 2022-08-23 17:19:34.993522 xrpl-py-2.0.0b0/xrpl/utils/__init__.py
+-rw-r--r--   0        0        0     3412 2022-04-25 18:39:06.775209 xrpl-py-2.0.0b0/xrpl/utils/parse_nftoken_id.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925715 xrpl-py-2.0.0b0/xrpl/utils/py.typed
+-rw-r--r--   0        0        0     1537 2022-07-05 22:56:20.074990 xrpl-py-2.0.0b0/xrpl/utils/sidechain.py
+-rw-r--r--   0        0        0      788 2021-12-17 21:23:35.563169 xrpl-py-2.0.0b0/xrpl/utils/str_conversions.py
+-rw-r--r--   0        0        0     4202 2022-07-28 00:01:58.134040 xrpl-py-2.0.0b0/xrpl/utils/time_conversions.py
+-rw-r--r--   0        0        0      350 2022-08-23 17:19:34.994080 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/__init__.py
+-rw-r--r--   0        0        0     1717 2022-07-05 22:56:20.082815 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_balance_changes.py
+-rw-r--r--   0        0        0     1446 2022-07-05 22:56:20.083098 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_final_balances.py
+-rw-r--r--   0        0        0      641 2022-08-23 17:19:34.994400 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_order_book_changes.py
+-rw-r--r--   0        0        0      627 2022-08-23 17:19:34.995150 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/__init__.py
+-rw-r--r--   0        0        0     5218 2022-08-23 17:19:34.995970 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/balance_parser.py
+-rw-r--r--   0        0        0     2518 2022-12-15 20:10:31.082062 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/nodes.py
+-rw-r--r--   0        0        0     6191 2022-08-23 17:19:34.996288 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/order_book_parser.py
+-rw-r--r--   0        0        0     1192 2022-08-23 17:19:34.996460 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/parser.py
+-rw-r--r--   0        0        0     1404 2022-12-15 20:10:31.082853 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/types.py
+-rw-r--r--   0        0        0     3476 2022-07-28 00:01:58.134766 xrpl-py-2.0.0b0/xrpl/utils/xrp_conversions.py
+-rw-r--r--   0        0        0      269 2021-07-28 20:35:08.852350 xrpl-py-2.0.0b0/xrpl/wallet/__init__.py
+-rw-r--r--   0        0        0     8321 2022-12-15 20:10:31.083718 xrpl-py-2.0.0b0/xrpl/wallet/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925867 xrpl-py-2.0.0b0/xrpl/wallet/py.typed
+-rw-r--r--   0        0        0     1370 2022-04-05 18:02:24.775775 xrpl-py-2.0.0b0/xrpl/wallet/wallet_generation.py
+-rw-r--r--   0        0        0    18248 2022-12-15 20:19:48.363167 xrpl-py-2.0.0b0/setup.py
+-rw-r--r--   0        0        0    17208 2022-12-15 20:19:48.364332 xrpl-py-2.0.0b0/PKG-INFO
```

### Comparing `xrpl-py-1.9.0b0/LICENSE` & `xrpl-py-2.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/README.md` & `xrpl-py-2.0.0b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -163,25 +163,24 @@
 ```py
 from xrpl.models.transactions import Payment
 from xrpl.transaction import sign, send_reliable_submission
 from xrpl.ledger import get_latest_validated_ledger_sequence
 from xrpl.account import get_next_valid_seq_number
 
 current_validated_ledger = get_latest_validated_ledger_sequence(client)
-test_wallet.sequence = get_next_valid_seq_number(test_wallet.classic_address, client)
 
 # prepare the transaction
 # the amount is expressed in drops, not XRP
 # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
 my_tx_payment = Payment(
     account=test_wallet.classic_address,
     amount="2200000",
     destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",
     last_ledger_sequence=current_validated_ledger + 20,
-    sequence=test_wallet.sequence,
+    sequence=get_next_valid_seq_number(test_wallet.classic_address, client),
     fee="10",
 )
 # sign the transaction
 my_tx_payment_signed = sign(my_tx_payment,test_wallet)
 
 # submit the transaction
 tx_response = send_reliable_submission(my_tx_payment_signed, client)
@@ -281,25 +280,24 @@
 from xrpl.asyncio.account import get_next_valid_seq_number
 from xrpl.asyncio.clients import AsyncJsonRpcClient
 
 async_client = AsyncJsonRpcClient(JSON_RPC_URL)
 
 async def submit_sample_transaction():
     current_validated_ledger = await get_latest_validated_ledger_sequence(async_client)
-    test_wallet.sequence = await get_next_valid_seq_number(test_wallet.classic_address, async_client)
 
     # prepare the transaction
     # the amount is expressed in drops, not XRP
     # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
     my_tx_payment = Payment(
         account=test_wallet.classic_address,
         amount="2200000",
         destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",
         last_ledger_sequence=current_validated_ledger + 20,
-        sequence=test_wallet.sequence,
+        sequence=await get_next_valid_seq_number(test_wallet.classic_address, async_client),
         fee="10",
     )
     # sign the transaction
     my_tx_payment_signed = await sign(my_tx_payment,test_wallet)
 
     # submit the transaction
     tx_response = await send_reliable_submission(my_tx_payment_signed, async_client)
```

### Comparing `xrpl-py-1.9.0b0/pyproject.toml` & `xrpl-py-2.0.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xrpl-py"
-version = "1.9.0-beta.0"
+version = "2.0.0-beta.0"
 description = "A complete Python library for interacting with the XRP ledger"
 readme = "README.md"
 repository = "https://github.com/XRPLF/xrpl-py"
 authors = [
   "Mayukha Vadari <mvadari@ripple.com>",
   "Greg Weisbrod <gweisbrod@ripple.com>",
   "Amie Corso <acorso@ripple.com>",
```

### Comparing `xrpl-py-1.9.0b0/xrpl/account/__init__.py` & `xrpl-py-2.0.0b0/xrpl/account/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/account/main.py` & `xrpl-py-2.0.0b0/xrpl/account/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/account/transaction_history.py` & `xrpl-py-2.0.0b0/xrpl/account/transaction_history.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/account/__init__.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/account/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/account/main.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/account/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/account/transaction_history.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/account/transaction_history.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/clients/__init__.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/clients/async_client.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_client.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/clients/async_websocket_client.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_websocket_client.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/clients/client.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/client.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/clients/exceptions.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/clients/json_rpc_base.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/json_rpc_base.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/clients/utils.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/clients/websocket_base.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/websocket_base.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/ledger/main.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/ledger/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/ledger/utils.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/ledger/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/transaction/__init__.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/transaction/ledger.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/transaction/ledger.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/transaction/main.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/transaction/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from typing_extensions import Final
 
 from xrpl.asyncio.account import get_next_valid_seq_number
 from xrpl.asyncio.clients import Client, XRPLRequestFailureException
 from xrpl.asyncio.ledger import get_fee, get_latest_validated_ledger_sequence
 from xrpl.constants import XRPLException
 from xrpl.core.addresscodec import is_valid_xaddress, xaddress_to_classic_address
-from xrpl.core.binarycodec import encode, encode_for_multisigning, encode_for_signing
+from xrpl.core.binarycodec import encode, encode_for_signing
 from xrpl.core.keypairs.main import sign as keypairs_sign
 from xrpl.models.requests import ServerState, SubmitOnly
 from xrpl.models.response import Response
 from xrpl.models.transactions import EscrowFinish
-from xrpl.models.transactions.transaction import Signer, Transaction
+from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.transaction import (
     transaction_json_to_binary_codec_form as model_transaction_to_binary_codec,
 )
 from xrpl.models.transactions.types.transaction_type import TransactionType
 from xrpl.utils import drops_to_xrp, xrp_to_drops
 from xrpl.wallet.main import Wallet
 
@@ -47,62 +47,42 @@
         check_fee: whether to check if the fee is higher than the expected transaction
             type fee. Defaults to True.
 
     Returns:
         The response from the ledger.
     """
     if autofill:
-        transaction = await autofill_and_sign(transaction, wallet, client, check_fee)
+        transaction = await safe_sign_and_autofill_transaction(
+            transaction, wallet, client, check_fee
+        )
     else:
         transaction = await sign(transaction, wallet, check_fee)
     return await submit(transaction, client)
 
 
 safe_sign_and_submit_transaction = sign_and_submit
 
 
 async def sign(
     transaction: Transaction,
     wallet: Wallet,
     check_fee: bool = True,
-    multisign: bool = False,
 ) -> Transaction:
     """
     Signs a transaction locally, without trusting external rippled nodes.
 
     Args:
         transaction: the transaction to be signed.
         wallet: the wallet with which to sign the transaction.
         check_fee: whether to check if the fee is higher than the expected transaction
             type fee. Defaults to True.
-        multisign: whether to sign the transaction for a multisignature transaction.
 
     Returns:
         The signed transaction blob.
     """
-    if multisign:
-        signature = keypairs_sign(
-            bytes.fromhex(
-                encode_for_multisigning(
-                    transaction.to_xrpl(),
-                    wallet.classic_address,
-                )
-            ),
-            wallet.private_key,
-        )
-        tx_dict = transaction.to_dict()
-        tx_dict["signers"] = [
-            Signer(
-                account=wallet.classic_address,
-                txn_signature=signature,
-                signing_pub_key=wallet.public_key,
-            )
-        ]
-        return Transaction.from_dict(tx_dict)
-
     if check_fee:
         await _check_fee(transaction)
     transaction_json = _prepare_transaction(transaction, wallet)
     serialized_for_signing = encode_for_signing(transaction_json)
     serialized_bytes = bytes.fromhex(serialized_for_signing)
     signature = keypairs_sign(serialized_bytes, wallet.private_key)
     transaction_json["TxnSignature"] = signature
@@ -206,38 +186,34 @@
     _convert_to_classic_address(transaction_json, "Owner")
     # SetRegularKey
     _convert_to_classic_address(transaction_json, "RegularKey")
 
     return transaction_json
 
 
-async def autofill(
-    transaction: Transaction, client: Client, signers_count: Optional[int] = None
-) -> Transaction:
+async def autofill(transaction: Transaction, client: Client) -> Transaction:
     """
     Autofills fields in a transaction. This will set `sequence`, `fee`, and
     `last_ledger_sequence` according to the current state of the server this Client is
     connected to. It also converts all X-Addresses to classic addresses.
 
     Args:
         transaction: the transaction to be signed.
         client: a network client.
-        signers_count: the expected number of signers for this transaction.
-            Only used for multisigned transactions.
 
     Returns:
         The autofilled transaction.
     """
     transaction_json = transaction.to_dict()
     if "sequence" not in transaction_json:
         sequence = await get_next_valid_seq_number(transaction_json["account"], client)
         transaction_json["sequence"] = sequence
     if "fee" not in transaction_json:
         transaction_json["fee"] = await _calculate_fee_per_transaction_type(
-            transaction, client, signers_count
+            transaction, client
         )
     if "last_ledger_sequence" not in transaction_json:
         ledger_sequence = await get_latest_validated_ledger_sequence(client)
         transaction_json["last_ledger_sequence"] = ledger_sequence + _LEDGER_OFFSET
     return Transaction.from_dict(transaction_json)
 
 
@@ -313,30 +289,26 @@
             f"Fee value: {str(drops_to_xrp(transaction.fee))} XRP is likely entered "
             "incorrectly, since it is much larger than the typical XRP transaction "
             "cost. If this is intentional, use `check_fee=False`."
         )
 
 
 async def _calculate_fee_per_transaction_type(
-    transaction: Transaction,
-    client: Optional[Client] = None,
-    signers_count: Optional[int] = None,
+    transaction: Transaction, client: Optional[Client] = None
 ) -> str:
     """
     Calculate the total fee in drops for a transaction based on:
     - the network fee
     - the transaction condition
 
     https://xrpl.org/transaction-cost.html#special-transaction-costs
 
     Args:
         transaction: the Transaction to be submitted.
         client: the network client with which to submit the transaction.
-        signers_count: the expected number of signers for this transaction.
-            Only used for multisigned transactions.
 
     Returns:
         The expected Transaction fee in drops
     """
     # Reference Transaction (Most transactions)
     if client is None:
         net_fee = 10  # 10 drops
@@ -359,16 +331,17 @@
         if client is None:
             base_fee = _ACCOUNT_DELETE_FEE
         else:
             base_fee = await _fetch_account_delete_fee(client)
 
     # Multi-signed Transaction
     # 10 drops × (1 + Number of Signatures Provided)
-    if signers_count is not None and signers_count > 0:
-        base_fee += net_fee * (1 + signers_count)
+    if transaction.signers and len(transaction.signers) > 0:
+        base_fee = net_fee * (1 + len(transaction.signers)) + base_fee
+
     # Round Up base_fee and return it as a String
     return str(math.ceil(base_fee))
 
 
 async def _fetch_account_delete_fee(client: Client) -> int:
     server_state = await client._request_impl(ServerState())
     fee = server_state.result["state"]["validated_ledger"]["reserve_inc"]
```

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/transaction/reliable_submission.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/transaction/reliable_submission.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/asyncio/wallet/wallet_generation.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/wallet/wallet_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,14 @@
             if current_balance > starting_balance:
                 if debug:
                     print("Faucet fund successful.")
                 is_funded = True
         else:  # wallet has been funded, now the ledger needs to know the account exists
             next_seq_num = await _try_to_get_next_seq(address, client)
             if next_seq_num is not None:
-                wallet.sequence = next_seq_num
                 return wallet
 
     raise XRPLFaucetException(
         "Unable to fund address with faucet after waiting {} seconds".format(
             _TIMEOUT_SECONDS
         )
     )
```

### Comparing `xrpl-py-1.9.0b0/xrpl/clients/__init__.py` & `xrpl-py-2.0.0b0/xrpl/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/clients/sync_client.py` & `xrpl-py-2.0.0b0/xrpl/clients/sync_client.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/clients/websocket_client.py` & `xrpl-py-2.0.0b0/xrpl/clients/websocket_client.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/constants.py` & `xrpl-py-2.0.0b0/xrpl/constants.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/addresscodec/__init__.py` & `xrpl-py-2.0.0b0/xrpl/core/addresscodec/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     encode_node_public_key,
     encode_seed,
     is_valid_classic_address,
 )
 from xrpl.core.addresscodec.exceptions import XRPLAddressCodecException
 from xrpl.core.addresscodec.main import (
     classic_address_to_xaddress,
+    ensure_classic_address,
     is_valid_xaddress,
     xaddress_to_classic_address,
 )
 from xrpl.core.addresscodec.utils import XRPL_ALPHABET
 
 __all__ = [
     "classic_address_to_xaddress",
@@ -25,14 +26,15 @@
     "decode_classic_address",
     "decode_node_public_key",
     "decode_seed",
     "encode_seed",
     "encode_account_public_key",
     "encode_classic_address",
     "encode_node_public_key",
+    "ensure_classic_address",
     "is_valid_classic_address",
     "is_valid_xaddress",
     "SEED_LENGTH",
     "xaddress_to_classic_address",
     "XRPLAddressCodecException",
     "XRPL_ALPHABET",
 ]
```

### Comparing `xrpl-py-1.9.0b0/xrpl/core/addresscodec/codec.py` & `xrpl-py-2.0.0b0/xrpl/core/addresscodec/codec.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/addresscodec/main.py` & `xrpl-py-2.0.0b0/xrpl/core/addresscodec/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -91,14 +91,45 @@
     classic_address_bytes = decoded[2:22]
     tag = _get_tag_from_buffer(decoded[22:])  # extracts the destination tag
 
     classic_address = encode_classic_address(classic_address_bytes)
     return (classic_address, tag, is_test_network)
 
 
+def ensure_classic_address(account: str) -> str:
+    """
+    If an address is an X-Address, converts it to a classic address.
+
+    Args:
+        account: A classic address or X-address.
+
+    Returns:
+        The account's classic address
+
+    Raises:
+        XRPLAddressCodecException: if the X-Address has an associated tag.
+    """
+    if is_valid_xaddress(account):
+        classic_address, tag, _ = xaddress_to_classic_address(account)
+
+        """
+        Except for special cases, X-addresses used for requests must not
+        have an embedded tag. In other words, `tag` should be None.
+        """
+        if tag is not None:
+            raise XRPLAddressCodecException(
+                "This command does not support the use of a tag. Use "
+                "an address without a tag"
+            )
+
+        return classic_address
+
+    return account
+
+
 def _is_test_address(prefix: bytes) -> bool:
     """
     Returns whether a decoded X-Address is a test address.
 
     Args:
         prefix: The first 2 bytes of an X-Address.
```

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/definitions/__init__.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/definitions/definitions.json` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/definitions.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9072246066700101%*

 * *Differences: {"'FIELDS'": '{delete: [262, 261, 260, 259, 258, 257, 251, 241, 240, 239, 238, 237, 236, 235, 234, '*

 * *             '233, 232, 231, 230, 208, 207, 206, 205, 204, 203, 197, 196, 195, 194, 193, 192, 191, '*

 * *             '189, 155, 154, 153, 152, 151, 150, 149, 148, 143, 142, 141, 113, 94, 93, 92, 74, 73, '*

 * *             '23, 18]}',*

 * * "'LEDGER_ENTRY_TYPES'": "{delete: ['Bridge', 'XChainClaimID', 'XChainCreateAccountClaimID', "*

 * *                         "'AMM']}",*

 * * "'TRANSACTION_RESULTS'": "{delete: ['temAMM_BAD_TOKE […]*

```diff
@@ -177,24 +177,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 18,
                 "type": "UInt8"
             }
         ],
         [
-            "WasLockingChainSend",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 19,
-                "type": "UInt8"
-            }
-        ],
-        [
             "LedgerEntryType",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 1,
                 "type": "UInt16"
@@ -227,24 +217,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 4,
                 "type": "UInt16"
             }
         ],
         [
-            "TradingFee",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 5,
-                "type": "UInt16"
-            }
-        ],
-        [
             "Version",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 16,
                 "type": "UInt16"
@@ -727,34 +707,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 46,
                 "type": "UInt32"
             }
         ],
         [
-            "VoteWeight",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 47,
-                "type": "UInt32"
-            }
-        ],
-        [
-            "DiscountedFee",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 48,
-                "type": "UInt32"
-            }
-        ],
-        [
             "IndexNext",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 1,
                 "type": "UInt64"
@@ -917,44 +877,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 19,
                 "type": "UInt64"
             }
         ],
         [
-            "XChainClaimID",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 20,
-                "type": "UInt64"
-            }
-        ],
-        [
-            "XChainAccountCreateCount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 21,
-                "type": "UInt64"
-            }
-        ],
-        [
-            "XChainAccountClaimCount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 22,
-                "type": "UInt64"
-            }
-        ],
-        [
             "EmailHash",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 1,
                 "type": "Hash128"
@@ -1127,24 +1057,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 13,
                 "type": "Hash256"
             }
         ],
         [
-            "AMMID",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 14,
-                "type": "Hash256"
-            }
-        ],
-        [
             "BookDirectory",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 16,
                 "type": "Hash256"
@@ -1407,44 +1327,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 10,
                 "type": "Amount"
             }
         ],
         [
-            "Amount2",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 11,
-                "type": "Amount"
-            }
-        ],
-        [
-            "BidMin",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 12,
-                "type": "Amount"
-            }
-        ],
-        [
-            "BidMax",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 13,
-                "type": "Amount"
-            }
-        ],
-        [
             "MinimumOffer",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 16,
                 "type": "Amount"
@@ -1477,94 +1367,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 19,
                 "type": "Amount"
             }
         ],
         [
-            "LPTokenOut",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 20,
-                "type": "Amount"
-            }
-        ],
-        [
-            "LPTokenIn",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 21,
-                "type": "Amount"
-            }
-        ],
-        [
-            "EPrice",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 22,
-                "type": "Amount"
-            }
-        ],
-        [
-            "Price",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 23,
-                "type": "Amount"
-            }
-        ],
-        [
-            "LPTokenBalance",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 24,
-                "type": "Amount"
-            }
-        ],
-        [
-            "XChainFee",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 28,
-                "type": "Amount"
-            }
-        ],
-        [
-            "SignatureReward",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 29,
-                "type": "Amount"
-            }
-        ],
-        [
-            "MinAccountCreateAmount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 30,
-                "type": "Amount"
-            }
-        ],
-        [
             "PublicKey",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": true,
                 "nth": 1,
                 "type": "Blob"
@@ -1887,104 +1697,24 @@
                 "isSigningField": true,
                 "isVLEncoded": true,
                 "nth": 10,
                 "type": "AccountID"
             }
         ],
         [
-            "AMMAccount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": true,
-                "nth": 11,
-                "type": "AccountID"
-            }
-        ],
-        [
             "HookAccount",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": true,
                 "nth": 16,
                 "type": "AccountID"
             }
         ],
         [
-            "ThisChainAccount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": true,
-                "nth": 17,
-                "type": "AccountID"
-            }
-        ],
-        [
-            "OtherChainSource",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": true,
-                "nth": 18,
-                "type": "AccountID"
-            }
-        ],
-        [
-            "OtherChainDestination",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": true,
-                "nth": 19,
-                "type": "AccountID"
-            }
-        ],
-        [
-            "AttestationSignerAccount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": true,
-                "nth": 20,
-                "type": "AccountID"
-            }
-        ],
-        [
-            "AttestationRewardAccount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": true,
-                "nth": 21,
-                "type": "AccountID"
-            }
-        ],
-        [
-            "LockingChainDoor",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": true,
-                "nth": 22,
-                "type": "AccountID"
-            }
-        ],
-        [
-            "IssuingChainDoor",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": true,
-                "nth": 23,
-                "type": "AccountID"
-            }
-        ],
-        [
             "Indexes",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": true,
                 "nth": 1,
                 "type": "Vector256"
@@ -2027,74 +1757,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 1,
                 "type": "PathSet"
             }
         ],
         [
-            "LockingChainIssue",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 1,
-                "type": "Issue"
-            }
-        ],
-        [
-            "Asset",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 3,
-                "type": "Issue"
-            }
-        ],
-        [
-            "IssuingChainIssue",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 2,
-                "type": "Issue"
-            }
-        ],
-        [
-            "Asset2",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 4,
-                "type": "Issue"
-            }
-        ],
-        [
-            "XChainBridge",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 1,
-                "type": "XChainBridge"
-            }
-        ],
-        [
-            "XChainAttestationBatch",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 1,
-                "type": "XChainAttestationBatch"
-            }
-        ],
-        [
             "TransactionMetaData",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 2,
                 "type": "STObject"
@@ -2297,134 +1967,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 24,
                 "type": "STObject"
             }
         ],
         [
-            "VoteEntry",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 25,
-                "type": "STObject"
-            }
-        ],
-        [
-            "AuctionSlot",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 27,
-                "type": "STObject"
-            }
-        ],
-        [
-            "AuthAccount",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 28,
-                "type": "STObject"
-            }
-        ],
-        [
-            "AMMToken",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 29,
-                "type": "STObject"
-            }
-        ],
-        [
-            "Token1",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 30,
-                "type": "STObject"
-            }
-        ],
-        [
-            "Token2",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 31,
-                "type": "STObject"
-            }
-        ],
-        [
-            "XChainClaimProofSig",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 32,
-                "type": "STObject"
-            }
-        ],
-        [
-            "XChainCreateAccountProofSig",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 33,
-                "type": "STObject"
-            }
-        ],
-        [
-            "XChainAttestationBatchElement",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 34,
-                "type": "STObject"
-            }
-        ],
-        [
-            "XChainClaimAttestationBatchElement",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 35,
-                "type": "STObject"
-            }
-        ],
-        [
-            "XChainCreateAccountAttestationBatchElement",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 36,
-                "type": "STObject"
-            }
-        ],
-        [
-            "XChainAttestationBatchInner",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 37,
-                "type": "STObject"
-            }
-        ],
-        [
             "Signers",
             {
                 "isSerialized": true,
                 "isSigningField": false,
                 "isVLEncoded": false,
                 "nth": 3,
                 "type": "STArray"
@@ -2507,24 +2057,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 11,
                 "type": "STArray"
             }
         ],
         [
-            "VoteSlots",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 14,
-                "type": "STArray"
-            }
-        ],
-        [
             "Majorities",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 16,
                 "type": "STArray"
@@ -2565,82 +2105,20 @@
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 20,
                 "type": "STArray"
             }
-        ],
-        [
-            "XChainProofSigs",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 21,
-                "type": "STArray"
-            }
-        ],
-        [
-            "XChainClaimAttestationBatch",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 22,
-                "type": "STArray"
-            }
-        ],
-        [
-            "XChainCreateAccountAttestationBatch",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 23,
-                "type": "STArray"
-            }
-        ],
-        [
-            "XChainClaimAttestations",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 24,
-                "type": "STArray"
-            }
-        ],
-        [
-            "XChainCreateAccountAttestations",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 25,
-                "type": "STArray"
-            }
-        ],
-        [
-            "AuthAccounts",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 26,
-                "type": "STArray"
-            }
         ]
     ],
     "LEDGER_ENTRY_TYPES": {
-        "AMM": 121,
         "AccountRoot": 97,
         "Amendments": 102,
         "Any": -3,
-        "Bridge": 105,
         "Check": 67,
         "Child": -2,
         "Contract": 99,
         "DepositPreauth": 112,
         "DirectoryNode": 100,
         "Escrow": 117,
         "FeeSettings": 115,
@@ -2651,27 +2129,17 @@
         "NFTokenPage": 80,
         "NegativeUNL": 78,
         "Nickname": 110,
         "Offer": 111,
         "PayChannel": 120,
         "RippleState": 114,
         "SignerList": 83,
-        "Ticket": 84,
-        "XChainClaimID": 113,
-        "XChainCreateAccountClaimID": 116
+        "Ticket": 84
     },
     "TRANSACTION_RESULTS": {
-        "tecAMM_BALANCE": 163,
-        "tecAMM_FAILED_BID": 167,
-        "tecAMM_FAILED_DEPOSIT": 164,
-        "tecAMM_FAILED_VOTE": 168,
-        "tecAMM_FAILED_WITHDRAW": 165,
-        "tecAMM_INVALID_TOKENS": 166,
-        "tecAMM_UNFUNDED": 162,
-        "tecBAD_XCHAIN_TRANSFER_ISSUE": 171,
         "tecCANT_ACCEPT_OWN_NFTOKEN_OFFER": 158,
         "tecCLAIM": 100,
         "tecCRYPTOCONDITION_ERROR": 146,
         "tecDIR_FULL": 121,
         "tecDST_TAG_NEEDED": 143,
         "tecDUPLICATE": 149,
         "tecEXPIRED": 148,
@@ -2710,29 +2178,14 @@
         "tecPATH_DRY": 128,
         "tecPATH_PARTIAL": 101,
         "tecTOO_SOON": 152,
         "tecUNFUNDED": 129,
         "tecUNFUNDED_ADD": 102,
         "tecUNFUNDED_OFFER": 103,
         "tecUNFUNDED_PAYMENT": 104,
-        "tecXCHAIN_ACCOUNT_CREATE_PAST": 183,
-        "tecXCHAIN_ACCOUNT_CREATE_TOO_MANY": 184,
-        "tecXCHAIN_BAD_CLAIM_ID": 173,
-        "tecXCHAIN_CLAIM_ACCOUNT_DST_EXISTS": 177,
-        "tecXCHAIN_CLAIM_NO_QUORUM": 174,
-        "tecXCHAIN_CREATE_ACCOUNT_NONXRP_ISSUE": 176,
-        "tecXCHAIN_INSUFF_CREATE_AMOUNT": 182,
-        "tecXCHAIN_NO_CLAIM_ID": 172,
-        "tecXCHAIN_NO_SIGNERS_LIST": 180,
-        "tecXCHAIN_PAYMENT_FAILED": 185,
-        "tecXCHAIN_PROOF_UNKNOWN_KEY": 175,
-        "tecXCHAIN_REWARD_MISMATCH": 179,
-        "tecXCHAIN_SELF_COMMIT": 186,
-        "tecXCHAIN_SENDING_ACCOUNT_MISMATCH": 181,
-        "tecXCHAIN_WRONG_CHAIN": 178,
         "tefALREADY": -198,
         "tefBAD_ADD_AUTH": -197,
         "tefBAD_AUTH": -196,
         "tefBAD_AUTH_MASTER": -183,
         "tefBAD_LEDGER": -195,
         "tefBAD_QUORUM": -185,
         "tefBAD_SIGNATURE": -186,
@@ -2759,15 +2212,14 @@
         "telCAN_NOT_QUEUE_BLOCKS": -390,
         "telCAN_NOT_QUEUE_FEE": -388,
         "telCAN_NOT_QUEUE_FULL": -387,
         "telFAILED_PROCESSING": -395,
         "telINSUF_FEE_P": -394,
         "telLOCAL_ERROR": -399,
         "telNO_DST_PARTIAL": -393,
-        "temAMM_BAD_TOKENS": -261,
         "temBAD_AMOUNT": -298,
         "temBAD_CURRENCY": -297,
         "temBAD_EXPIRATION": -296,
         "temBAD_FEE": -295,
         "temBAD_ISSUER": -294,
         "temBAD_LIMIT": -293,
         "temBAD_NFTOKEN_TRANSFER_FEE": -262,
@@ -2784,56 +2236,43 @@
         "temBAD_SEQUENCE": -283,
         "temBAD_SIGNATURE": -282,
         "temBAD_SIGNER": -272,
         "temBAD_SRC_ACCOUNT": -281,
         "temBAD_TICK_SIZE": -269,
         "temBAD_TRANSFER_RATE": -280,
         "temBAD_WEIGHT": -270,
-        "temBAD_XCHAIN_PROOF": -258,
         "temCANNOT_PREAUTH_SELF": -267,
         "temDISABLED": -273,
         "temDST_IS_SRC": -279,
         "temDST_NEEDED": -278,
-        "temEQUAL_DOOR_ACCOUNTS": -259,
         "temINVALID": -277,
         "temINVALID_ACCOUNT_ID": -268,
         "temINVALID_COUNT": -266,
         "temINVALID_FLAG": -276,
         "temMALFORMED": -299,
         "temREDUNDANT": -275,
         "temRIPPLE_EMPTY": -274,
         "temSEQ_AND_TICKET": -263,
-        "temSIDECHAIN_BAD_ISSUES": -257,
-        "temSIDECHAIN_NONDOOR_OWNER": -256,
         "temUNCERTAIN": -265,
         "temUNKNOWN": -264,
-        "temXCHAIN_BRIDGE_BAD_MIN_ACCOUNT_CREATE_AMOUNT": -255,
-        "temXCHAIN_BRIDGE_BAD_REWARD_AMOUNT": -254,
-        "temXCHAIN_TOO_MANY_ATTESTATIONS": -253,
         "terFUNDS_SPENT": -98,
         "terINSUF_FEE_B": -97,
         "terLAST": -91,
         "terNO_ACCOUNT": -96,
-        "terNO_AMM": -87,
         "terNO_AUTH": -95,
         "terNO_LINE": -94,
         "terNO_RIPPLE": -90,
         "terOWNERS": -93,
         "terPRE_SEQ": -92,
         "terPRE_TICKET": -88,
         "terQUEUED": -89,
         "terRETRY": -99,
         "tesSUCCESS": 0
     },
     "TRANSACTION_TYPES": {
-        "AMMBid": 39,
-        "AMMCreate": 35,
-        "AMMDeposit": 36,
-        "AMMVote": 38,
-        "AMMWithdraw": 37,
         "AccountDelete": 21,
         "AccountSet": 3,
         "CheckCancel": 18,
         "CheckCash": 17,
         "CheckCreate": 16,
         "Contract": 9,
         "DepositPreauth": 19,
@@ -2857,32 +2296,24 @@
         "SetFee": 101,
         "SetHook": 22,
         "SetRegularKey": 5,
         "SignerListSet": 12,
         "TicketCancel": 11,
         "TicketCreate": 10,
         "TrustSet": 20,
-        "UNLModify": 102,
-        "XChainAccountCreateCommit": 44,
-        "XChainAddAttestation": 45,
-        "XChainClaim": 43,
-        "XChainCommit": 42,
-        "XChainCreateBridge": 40,
-        "XChainCreateClaimID": 41,
-        "XChainModifyBridge": 46
+        "UNLModify": 102
     },
     "TYPES": {
         "AccountID": 8,
         "Amount": 6,
         "Blob": 7,
         "Done": -1,
         "Hash128": 4,
         "Hash160": 17,
         "Hash256": 5,
-        "Issue": 24,
         "LedgerEntry": 10002,
         "Metadata": 10004,
         "NotPresent": 0,
         "PathSet": 18,
         "STArray": 15,
         "STObject": 14,
         "Transaction": 10001,
@@ -2892,12 +2323,10 @@
         "UInt384": 22,
         "UInt512": 23,
         "UInt64": 3,
         "UInt8": 16,
         "UInt96": 20,
         "Unknown": -2,
         "Validation": 10003,
-        "Vector256": 19,
-        "XChainAttestationBatch": 26,
-        "XChainBridge": 25
+        "Vector256": 19
     }
 }
```

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/definitions/definitions.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/definitions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/definitions/field_header.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_header.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,11 +44,7 @@
                 header.append(self.field_code)
         elif self.field_code < 16:
             header += [self.field_code, self.type_code]
         else:
             header += [0, self.type_code, self.field_code]
 
         return bytes(header)
-
-    def __repr__(self: FieldHeader) -> str:
-        """Print a string representation of a FieldHeader (for debugging)."""
-        return f"FieldHeader({self.type_code}, {self.field_code})"
```

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/definitions/field_info.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_info.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/definitions/field_instance.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_instance.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/field_id_codec.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/field_id_codec.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/main.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/account_id.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/account_id.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/amount.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/amount.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/blob.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/blob.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/currency.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/currency.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/hash.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/hash128.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash128.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/hash160.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash160.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/hash256.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash256.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/issue.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/vector256.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,82 @@
-"""Codec for serializing and deserializing issued currency fields."""
-
+"""Codec for serializing and deserializing vectors of Hash256."""
 from __future__ import annotations
 
-from typing import Any, Dict, Optional, Type, Union
+from typing import List, Optional, Type
+
+from typing_extensions import Final
 
+from xrpl.core.binarycodec import XRPLBinaryCodecException
 from xrpl.core.binarycodec.binary_wrappers.binary_parser import BinaryParser
-from xrpl.core.binarycodec.exceptions import XRPLBinaryCodecException
-from xrpl.core.binarycodec.types.account_id import AccountID
-from xrpl.core.binarycodec.types.currency import Currency
+from xrpl.core.binarycodec.types.hash256 import Hash256
 from xrpl.core.binarycodec.types.serialized_type import SerializedType
-from xrpl.models.currencies import XRP as XRPModel
-from xrpl.models.currencies import IssuedCurrency as IssuedCurrencyModel
 
+_HASH_LENGTH_BYTES: Final[int] = 32
 
-class Issue(SerializedType):
-    """Codec for serializing and deserializing issued currency fields."""
 
-    def __init__(self: Issue, buffer: bytes) -> None:
-        """
-        Construct an Issue from given bytes.
+class Vector256(SerializedType):
+    """Codec for serializing and deserializing vectors of Hash256."""
 
-        Args:
-            buffer: The byte buffer that will be used to store the serialized
-                encoding of this field.
-        """
+    def __init__(self: Vector256, buffer: bytes) -> None:
+        """Construct a Vector256."""
         super().__init__(buffer)
 
     @classmethod
-    def from_value(cls: Type[Issue], value: Dict[str, str]) -> Issue:
-        """
-        Construct an Issue object from a string or dictionary representation
-        of an issued currency.
+    def from_value(cls: Type[Vector256], value: List[str]) -> Vector256:
+        """Construct a Vector256 from a list of strings.
 
         Args:
-            value: The dictionary to construct an Issue object from.
+            value: A list of hashes encoded as hex strings.
 
         Returns:
-            An Issue object constructed from value.
+            A Vector256 object representing these hashes.
 
         Raises:
-            XRPLBinaryCodecException: If the Issue representation is invalid.
+            XRPLBinaryCodecException: If the supplied value is of the wrong type.
         """
-        if XRPModel.is_dict_of_model(value):
-            currency_bytes = bytes(Currency.from_value(value["currency"]))
-            return cls(currency_bytes)
-
-        if IssuedCurrencyModel.is_dict_of_model(value):
-            currency_bytes = bytes(Currency.from_value(value["currency"]))
-            issuer_bytes = bytes(AccountID.from_value(value["issuer"]))
-            return cls(currency_bytes + issuer_bytes)
-
-        raise XRPLBinaryCodecException(
-            "Invalid type to construct an Issue: expected str or dict,"
-            f" received {value.__class__.__name__}."
-        )
+        if not isinstance(value, list):
+            raise XRPLBinaryCodecException(
+                "Invalid type to construct a Vector256: expected list,"
+                " received {value.__class__.__name__}."
+            )
+
+        byte_list = []
+        for string in value:
+            byte_list.append(bytes(Hash256.from_value(string)))
+        return cls(b"".join(byte_list))
 
     @classmethod
     def from_parser(
-        cls: Type[Issue],
-        parser: BinaryParser,
-        length_hint: Optional[int] = None,
-    ) -> Issue:
-        """
-        Construct an Issue object from an existing BinaryParser.
+        cls: Type[Vector256], parser: BinaryParser, length_hint: Optional[int] = None
+    ) -> SerializedType:
+        """Construct a Vector256 from a BinaryParser.
 
         Args:
-            parser: The parser to construct the Issue object from.
+            parser: The parser to construct a Vector256 from.
             length_hint: The number of bytes to consume from the parser.
 
         Returns:
-            The Issue object constructed from a parser.
+            A Vector256 object.
         """
-        currency = Currency.from_parser(parser)
-        if currency.to_json() == "XRP":
-            return cls(bytes(currency))
-
-        issuer = parser.read(20)  # the length in bytes of an account ID
-        return cls(bytes(currency) + issuer)
+        byte_list = []
+        num_bytes = length_hint if length_hint is not None else len(parser)
+        num_hashes = num_bytes // _HASH_LENGTH_BYTES
+        for i in range(num_hashes):
+            byte_list.append(bytes(Hash256.from_parser(parser)))
+        return cls(b"".join(byte_list))
 
-    def to_json(self: Issue) -> Union[str, Dict[Any, Any]]:
-        """
-        Returns the JSON representation of an issued currency.
+    def to_json(self: Vector256) -> List[str]:
+        """Return a list of hashes encoded as hex strings.
 
         Returns:
-            The JSON representation of an Issue.
-        """
-        parser = BinaryParser(str(self))
-        currency: Union[str, Dict[Any, Any]] = Currency.from_parser(parser).to_json()
-        if currency == "XRP":
-            return {"currency": currency}
+            The JSON representation of this Vector256.
 
-        issuer = AccountID.from_parser(parser)
-        return {"currency": currency, "issuer": issuer.to_json()}
+        Raises:
+            XRPLBinaryCodecException: If the number of bytes in the buffer
+                                        is not a multiple of the hash length.
+        """
+        if len(self.buffer) % _HASH_LENGTH_BYTES != 0:
+            raise XRPLBinaryCodecException("Invalid bytes for Vector256.")
+        hash_list = []
+        for i in range(0, len(self.buffer), _HASH_LENGTH_BYTES):
+            hash_list.append(self.buffer[i : i + _HASH_LENGTH_BYTES].hex().upper())
+        return hash_list
```

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/path_set.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/path_set.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/serialized_type.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/serialized_type.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/st_array.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/st_array.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/st_object.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/st_object.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/uint.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/uint16.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint16.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/uint32.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint32.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/uint64.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint64.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/binarycodec/types/uint8.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint8.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/keypairs/crypto_implementation.py` & `xrpl-py-2.0.0b0/xrpl/core/keypairs/crypto_implementation.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/keypairs/ed25519.py` & `xrpl-py-2.0.0b0/xrpl/core/keypairs/ed25519.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,8 +92,10 @@
 
     @classmethod
     def _public_key_to_str(cls: Type[ED25519], key: ECPublicKey) -> str:
         return cast(str, _CURVE.encode_point(key.W).hex())
 
     @classmethod
     def _format_key(cls: Type[ED25519], keystr: str) -> str:
+        if len(keystr) < 64:
+            keystr = keystr.zfill(64)
         return (PREFIX + keystr).upper()
```

### Comparing `xrpl-py-1.9.0b0/xrpl/core/keypairs/helpers.py` & `xrpl-py-2.0.0b0/xrpl/core/keypairs/helpers.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/core/keypairs/main.py` & `xrpl-py-2.0.0b0/xrpl/core/keypairs/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,27 +25,30 @@
     entropy: Optional[str] = None,
     algorithm: CryptoAlgorithm = CryptoAlgorithm.ED25519,
 ) -> str:
     """
     Generate a seed value that cryptographic keys can be derived from.
 
     Args:
-        entropy: Must be at least addresscodec.SEED_LENGTH bytes long and
-            will be truncated to that length
-        algorithm: CryptoAlgorithm to use for seed generation. The  default is
+        entropy: Hexadecimal string that is addresscodec.SEED_LENGTH bytes long
+        algorithm: CryptoAlgorithm to use for seed generation. The default is
             :data:`CryptoAlgorithm.ED25519 <xrpl.CryptoAlgorithm.ED25519>`.
 
     Returns:
         A seed value that can be used to derive a key pair with the given
-            cryptographic algorithm.
+        cryptographic algorithm.
+
+    Raises:
+        XRPLAddressCodecException: If entropy is not of length addresscodec.SEED_LENGTH,
+            this exception will be thrown in addresscodec.encode_seed.
     """
     if entropy is None:
         parsed_entropy = token_bytes(addresscodec.SEED_LENGTH)
     else:
-        parsed_entropy = bytes(entropy, "UTF-8")[: addresscodec.SEED_LENGTH]
+        parsed_entropy = bytes.fromhex(entropy)
     return addresscodec.encode_seed(parsed_entropy, algorithm)
 
 
 def derive_keypair(
     seed: str, validator: bool = False, algorithm: Optional[CryptoAlgorithm] = None
 ) -> Tuple[str, str]:
     """
```

### Comparing `xrpl-py-1.9.0b0/xrpl/core/keypairs/secp256k1.py` & `xrpl-py-2.0.0b0/xrpl/core/keypairs/secp256k1.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/ledger/main.py` & `xrpl-py-2.0.0b0/xrpl/ledger/main.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/__init__.py` & `xrpl-py-2.0.0b0/xrpl/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 """Top-level exports for the models package."""
 from xrpl.models import amounts, currencies, requests, transactions
 from xrpl.models.amounts import *  # noqa: F401, F403
-from xrpl.models.auth_account import AuthAccount
 from xrpl.models.currencies import *  # noqa: F401, F403
 from xrpl.models.exceptions import XRPLModelException
 from xrpl.models.path import Path, PathStep
 from xrpl.models.requests import *  # noqa: F401, F403
 from xrpl.models.response import Response
 from xrpl.models.transactions import *  # noqa: F401, F403
 from xrpl.models.transactions.pseudo_transactions import *  # noqa: F401, F403
-from xrpl.models.xchain_bridge import XChainBridge
 
 __all__ = [
     "XRPLModelException",
     "amounts",
     *amounts.__all__,
-    "AuthAccount",
     "currencies",
     *currencies.__all__,
     "requests",
     *requests.__all__,
     "transactions",
     *transactions.__all__,
     *transactions.pseudo_transactions.__all__,
     "Path",
     "PathStep",
     "Response",
-    "XChainBridge",
 ]
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/amounts/amount.py` & `xrpl-py-2.0.0b0/xrpl/models/amounts/amount.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/amounts/issued_currency_amount.py` & `xrpl-py-2.0.0b0/xrpl/models/amounts/issued_currency_amount.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/base_model.py` & `xrpl-py-2.0.0b0/xrpl/models/base_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import json
 import re
 from abc import ABC
 from dataclasses import fields
 from enum import Enum
 from typing import Any, Dict, List, Pattern, Type, TypeVar, Union, cast, get_type_hints
 
-from typing_extensions import Final, Literal, get_args, get_origin
+from typing_extensions import Final, get_args, get_origin
 
 from xrpl.models.exceptions import XRPLModelException
 from xrpl.models.required import REQUIRED
 from xrpl.models.types import XRPL_VALUE_TYPE
 
 # this regex splits words based on one of three cases:
 #
@@ -28,39 +28,29 @@
 # PascalCase like "Amount"
 _CAMEL_CASE_TYPICAL: Final[str] = "[A-Z][^A-Z]*"
 #
 # combining the above together into one regex:
 _CAMEL_TO_SNAKE_CASE_REGEX: Final[Pattern[str]] = re.compile(
     f"(?:{_CAMEL_CASE_LEADING_LOWER}|{_CAMEL_CASE_ABBREVIATION}|{_CAMEL_CASE_TYPICAL})"
 )
-
-# This is used to make exceptions when converting dictionary keys to xrpl JSON
-# keys. We snake case keys, but some keys are abbreviations.
-ABBREVIATIONS: Final[Dict[str, str]] = {
-    "amm": "AMM",
-    "id": "ID",
-    "lp": "LP",
-    "nftoken": "NFToken",
-    "unl": "UNL",
-    "uri": "URI",
-    "xchain": "XChain",
-}
+# used for converting special substrings inside CamelCase fields
+SPECIAL_CAMELCASE_STRINGS = ["NFToken"]
 
 BM = TypeVar("BM", bound="BaseModel")  # any type inherited from BaseModel
 
 
 def _key_to_json(field: str) -> str:
     """
     Transforms camelCase or PascalCase to snake_case. For example:
         1. 'TransactionType' becomes 'transaction_type'
         2. 'value' remains 'value'
         3. 'URI' becomes 'uri'
     """
     # convert all special CamelCase substrings to capitalized strings
-    for spec_str in ABBREVIATIONS.values():
+    for spec_str in SPECIAL_CAMELCASE_STRINGS:
         if spec_str in field:
             field = field.replace(spec_str, spec_str.capitalize())
 
     return "_".join(
         [word.lower() for word in _CAMEL_TO_SNAKE_CASE_REGEX.findall(field)]
     )
 
@@ -173,18 +163,14 @@
             # param_type is Any (e.g. will accept anything)
             return param_value
 
         if isinstance(param_type, type) and isinstance(param_value, param_type):
             # expected an object, received the correct object
             return param_value
 
-        if get_origin(param_type) == Literal:
-            if param_value in get_args(param_type):
-                return param_value
-
         if (
             isinstance(param_type, type)
             and issubclass(param_type, Enum)
             and param_value in list(param_type)
         ):
             # expected an Enum and received a valid value for it.
             # for some reason required for string enums.
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/currencies/issued_currency.py` & `xrpl-py-2.0.0b0/xrpl/models/currencies/issued_currency.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/currencies/xrp.py` & `xrpl-py-2.0.0b0/xrpl/models/currencies/xrp.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/flags.py` & `xrpl-py-2.0.0b0/xrpl/models/flags.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,30 +17,14 @@
         "asf_disable_master": 0x00000004,
         "asf_disallow_xrp": 0x00000003,
         "asf_global_freeze": 0x00000007,
         "asf_no_freeze": 0x00000006,
         "asf_require_auth": 0x00000002,
         "asf_require_dest": 0x00000001,
     },
-    "AMMDeposit": {
-        "tf_lp_token": 0x00010000,
-        "tf_single_asset": 0x00080000,
-        "tf_two_asset": 0x00100000,
-        "tf_one_asset_lp_token": 0x00200000,
-        "tf_limit_lp_token": 0x00400000,
-    },
-    "AMMWithdraw": {
-        "tf_lp_token": 0x00010000,
-        "tf_withdraw_all": 0x00020000,
-        "tf_one_asset_withdraw_all": 0x00040000,
-        "tf_single_asset": 0x00080000,
-        "tf_two_asset": 0x00100000,
-        "tf_one_asset_lp_token": 0x00200000,
-        "tf_limit_lp_token": 0x00400000,
-    },
     "NFTokenCreateOffer": {
         "tf_sell_token": 0x00000001,
     },
     "NFTokenMint": {
         "tf_burnable": 0x00000001,
         "tf_only_xrp": 0x00000002,
         "tf_trustline": 0x00000004,
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/nested_model.py` & `xrpl-py-2.0.0b0/xrpl/models/nested_model.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/path.py` & `xrpl-py-2.0.0b0/xrpl/models/path.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/__init__.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Request models."""
-from xrpl.models.auth_account import AuthAccount
 from xrpl.models.path import PathStep
 from xrpl.models.requests.account_channels import AccountChannels
 from xrpl.models.requests.account_currencies import AccountCurrencies
 from xrpl.models.requests.account_info import AccountInfo
 from xrpl.models.requests.account_lines import AccountLines
 from xrpl.models.requests.account_nfts import AccountNFTs
 from xrpl.models.requests.account_objects import AccountObjects, AccountObjectType
 from xrpl.models.requests.account_offers import AccountOffers
 from xrpl.models.requests.account_tx import AccountTx
-from xrpl.models.requests.amm_info import AMMInfo
 from xrpl.models.requests.book_offers import BookOffers
 from xrpl.models.requests.channel_authorize import ChannelAuthorize
 from xrpl.models.requests.channel_verify import ChannelVerify
 from xrpl.models.requests.deposit_authorized import DepositAuthorized
 from xrpl.models.requests.fee import Fee
 from xrpl.models.requests.gateway_balances import GatewayBalances
 from xrpl.models.requests.generic_request import GenericRequest
@@ -50,16 +48,14 @@
     "AccountInfo",
     "AccountLines",
     "AccountNFTs",
     "AccountObjects",
     "AccountObjectType",
     "AccountOffers",
     "AccountTx",
-    "AMMInfo",
-    "AuthAccount",
     "BookOffers",
     "ChannelAuthorize",
     "ChannelVerify",
     "DepositAuthorized",
     "Fee",
     "GatewayBalances",
     "GenericRequest",
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/account_channels.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_channels.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/account_currencies.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_currencies.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/account_info.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_info.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/account_lines.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_lines.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/account_nfts.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_nfts.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/account_objects.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,14 @@
     DEPOSIT_PREAUTH = "deposit_preauth"
     ESCROW = "escrow"
     OFFER = "offer"
     PAYMENT_CHANNEL = "payment_channel"
     SIGNER_LIST = "signer_list"
     STATE = "state"
     TICKET = "ticket"
-    XCHAIN_CREATE_ACCOUNT_CLAIM_ID = "xchain_create_account_claim_id"
-    XCHAIN_CLAIM_ID = "xchain_claim_id"
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class AccountObjects(Request):
     """
     This request returns the raw ledger format for all objects owned by an account.
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/account_offers.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_offers.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/account_tx.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_tx.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/book_offers.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/book_offers.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/channel_authorize.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/channel_authorize.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/channel_verify.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/channel_verify.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/deposit_authorized.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/deposit_authorized.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/federator_info.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/federator_info.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/fee.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/fee.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/gateway_balances.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/gateway_balances.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/generic_request.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/generic_request.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/ledger.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/ledger.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/ledger_closed.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/ledger_closed.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/ledger_current.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/ledger_current.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/ledger_data.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/ledger_data.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/ledger_entry.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/ledger_entry.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 """
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional, Union
 
 from xrpl.models.base_model import BaseModel
-from xrpl.models.currencies import Currency
 from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
-from xrpl.models.xchain_bridge import XChainBridge
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class DepositPreauth(BaseModel):
     """
     Required fields for requesting a DepositPreauth if not querying by
@@ -110,15 +108,15 @@
     :meta hide-value:
     """
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class RippleState(BaseModel):
-    """Required fields for requesting a RippleState if not querying by object ID."""
+    """Required fields for requesting a RippleState."""
 
     accounts: List[str] = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
@@ -130,15 +128,18 @@
     :meta hide-value:
     """
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class Ticket(BaseModel):
-    """Required fields for requesting a Ticket if not querying by object ID."""
+    """
+    Required fields for requesting a Ticket, if not querying by
+    object ID.
+    """
 
     owner: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
@@ -149,41 +150,14 @@
 
     :meta hide-value:
     """
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class XChainClaimID(BaseModel):
-    """Required fields for requesting an XChainClaimID if not querying by object ID."""
-
-    locking_chain_door: str
-    locking_chain_issue: Currency
-    issuing_chain_door: str
-    issuing_chain_issue: Currency
-    xchain_claim_id: Union[int, str]
-
-
-@require_kwargs_on_init
-@dataclass(frozen=True)
-class XChainCreateAccountClaimID(BaseModel):
-    """
-    Required fields for requesting an XChainCreateAccountClaimID if not querying by
-    object ID.
-    """
-
-    locking_chain_door: str
-    locking_chain_issue: Currency
-    issuing_chain_door: str
-    issuing_chain_issue: Currency
-    xchain_create_account_claim_id: Union[int, str]
-
-
-@require_kwargs_on_init
-@dataclass(frozen=True)
 class LedgerEntry(Request):
     """
     The ledger_entry method returns a single ledger
     object from the XRP Ledger in its raw format.
     See ledger format for information on the
     different types of objects you can retrieve.
     `See ledger entry <https://xrpl.org/ledger_entry.html>`_
@@ -196,20 +170,14 @@
     deposit_preauth: Optional[Union[str, DepositPreauth]] = None
     directory: Optional[Union[str, Directory]] = None
     escrow: Optional[Union[str, Escrow]] = None
     offer: Optional[Union[str, Offer]] = None
     payment_channel: Optional[str] = None
     ripple_state: Optional[RippleState] = None
     ticket: Optional[Union[str, Ticket]] = None
-    xchain_bridge: Optional[Union[str, XChainBridge]] = None
-    xchain_claim_id: Optional[Union[str, XChainClaimID]] = None
-    xchain_create_account_claim_id: Optional[
-        Union[str, XChainCreateAccountClaimID]
-    ] = None
-
     binary: bool = False
     ledger_hash: Optional[str] = None
     ledger_index: Optional[Union[str, int]] = None
 
     def _get_errors(self: LedgerEntry) -> Dict[str, str]:
         errors = super()._get_errors()
         query_params = [
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/manifest.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/manifest.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/nft_buy_offers.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/nft_buy_offers.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/nft_sell_offers.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/nft_sell_offers.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/no_ripple_check.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/no_ripple_check.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/path_find.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/path_find.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/ping.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/ping.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/random.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/random.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/request.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,17 +72,14 @@
     # utility methods
     PING = "ping"
     RANDOM = "random"
 
     # sidechain methods
     FEDERATOR_INFO = "federator_info"
 
-    # amm methods
-    AMM_INFO = "amm_info"
-
     # generic unknown/unsupported request
     # (there is no XRPL analog, this model is specific to xrpl-py)
     GENERIC_REQUEST = "zzgeneric_request"
 
 
 R = TypeVar("R", bound="Request")
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/ripple_path_find.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/ripple_path_find.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/server_info.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/server_info.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/server_state.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/server_state.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/sign.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/sign.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/sign_and_submit.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/sign_and_submit.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/sign_for.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/sign_for.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/submit.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/submit.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/submit_multisigned.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/submit_multisigned.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/submit_only.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/submit_only.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/subscribe.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/subscribe.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/transaction_entry.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/transaction_entry.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/tx.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/tx.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/requests/unsubscribe.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/response.py` & `xrpl-py-2.0.0b0/xrpl/models/response.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/account_delete.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/account_delete.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/account_set.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/account_set.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/amm_bid.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/check_cash.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,58 @@
-"""Model for AMMBid transaction type."""
-from __future__ import annotations
+"""Model for CheckCash transaction type."""
+from __future__ import annotations  # Requires Python 3.7+
 
 from dataclasses import dataclass, field
-from typing import Dict, List, Optional
-
-from typing_extensions import Final
+from typing import Dict, Optional
 
 from xrpl.models.amounts import Amount
-from xrpl.models.auth_account import AuthAccount
-from xrpl.models.currencies.issue import Issue
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
-_MAX_AUTH_ACCOUNTS: Final[int] = 4
-
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AMMBid(Transaction):
-    """
-    AMMBid is used to place a bid for the auction slot of obtaining trading advantages
-    of an AMM instance.
-
-    An AMM instance auctions off the trading advantages to users (arbitrageurs) at a
-    discounted TradingFee for a 24 hour slot.
+class CheckCash(Transaction):
     """
-
-    asset: Issue = REQUIRED  # type: ignore
-    """
-    Specifies one of the pool assets (XRP or token) of the AMM instance.
+    Represents a `CheckCash transaction <https://xrpl.org/checkcash.html>`_,
+    which redeems a Check object to receive up to the amount authorized by the
+    corresponding CheckCreate transaction. Only the Destination address of a
+    Check can cash it.
     """
 
-    asset2: Issue = REQUIRED  # type: ignore
-    """
-    Specifies the other pool asset of the AMM instance.
+    check_id: str = REQUIRED  # type: ignore
     """
+    The ID of the `Check ledger object
+    <https://xrpl.org/check.html>`_ to cash, as a 64-character
+    hexadecimal string. This field is required.
 
-    bid_min: Optional[Amount] = None
-    """
-    This field represents the minimum price that the bidder wants to pay for the slot.
-    It is specified in units of LPToken. If specified let MinSlotPrice be X and let
-    the slot-price computed by price scheduling algorithm be Y, then bidder always pays
-    the max(X, Y).
+    :meta hide-value:
     """
 
-    bid_max: Optional[Amount] = None
+    amount: Optional[Amount] = None
     """
-    This field represents the maximum price that the bidder wants to pay for the slot.
-    It is specified in units of LPToken.
+    Redeem the Check for exactly this amount, if possible. The currency must
+    match that of the SendMax of the corresponding CheckCreate transaction.
+    You must provide either this field or ``DeliverMin``.
     """
 
-    auth_accounts: Optional[List[AuthAccount]] = None
+    deliver_min: Optional[Amount] = None
     """
-    This field represents an array of XRPL account IDs that are authorized to trade
-    at the discounted fee against the AMM instance.
-    A maximum of four accounts can be provided.
+    Redeem the Check for at least this amount and for as much as possible.
+    The currency must match that of the ``SendMax`` of the corresponding
+    CheckCreate transaction. You must provide either this field or ``Amount``.
     """
 
     transaction_type: TransactionType = field(
-        default=TransactionType.AMM_BID,
+        default=TransactionType.CHECK_CASH,
         init=False,
     )
 
-    def _get_errors(self: AMMBid) -> Dict[str, str]:
-        return {
-            key: value
-            for key, value in {
-                **super()._get_errors(),
-                "auth_accounts": self._get_auth_accounts_error(),
-            }.items()
-            if value is not None
-        }
-
-    def _get_auth_accounts_error(self: AMMBid) -> Optional[str]:
-        if (
-            self.auth_accounts is not None
-            and len(self.auth_accounts) > _MAX_AUTH_ACCOUNTS
-        ):
-            return f"Length must not be greater than {_MAX_AUTH_ACCOUNTS}"
-        return None
+    def _get_errors(self: CheckCash) -> Dict[str, str]:
+        errors = super()._get_errors()
+        if not (self.amount is None) ^ (self.deliver_min is None):
+            errors[
+                "CheckCash"
+            ] = "either amount or deliver_min must be set but not both"
+        return errors
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/amm_create.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_cancel_offer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,58 @@
-"""Model for AMMCreate transaction type."""
+"""Model for NFTokenCancelOffer transaction type."""
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Dict, Optional
+from typing import Dict, List, Optional
 
-from typing_extensions import Final
-
-from xrpl.models.amounts import Amount
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
-AMM_MAX_TRADING_FEE: Final[int] = 1000
-
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AMMCreate(Transaction):
-    """
-    AMMCreate is used to create AccountRoot and the corresponding AMM
-    ledger entries.
-    This allows for the creation of only one AMM instance per unique asset pair.
+class NFTokenCancelOffer(Transaction):
     """
+    The NFTokenCancelOffer transaction deletes existing NFTokenOffer objects.
+    It is useful if you want to free up space on your account to lower your
+    reserve requirement.
 
-    amount: Amount = REQUIRED  # type: ignore
-    """
-    Specifies one of the pool assets (XRP or token) of the AMM instance.
-    This field is required.
+    The transaction can be executed by the account that originally created
+    the NFTokenOffer, the account in the `Recipient` field of the NFTokenOffer
+    (if present), or any account if the NFTokenOffer has an `Expiration` and
+    the NFTokenOffer has already expired.
     """
 
-    amount2: Amount = REQUIRED  # type: ignore
-    """
-    Specifies the other pool asset of the AMM instance. This field is required.
+    nftoken_offers: List[str] = REQUIRED  # type: ignore
     """
+    An array of identifiers of NFTokenOffer objects that should be cancelled
+    by this transaction.
 
-    trading_fee: int = REQUIRED  # type: ignore
-    """
-    Specifies the fee, in basis point, to be charged
-    to the traders for the trades executed against the AMM instance.
-    Trading fee is a percentage of the trading volume.
-    Valid values for this field are between 0 and 1000 inclusive.
-    A value of 1 is equivalent to 1/10 bps or 0.001%, allowing trading fee
-    between 0% and 1%. This field is required.
+    It is an error if an entry in this list points to an
+    object that is not an NFTokenOffer object. It is not an
+    error if an entry in this list points to an object that
+    does not exist. This field is required.
+
+    :meta hide-value:
     """
 
     transaction_type: TransactionType = field(
-        default=TransactionType.AMM_CREATE,
+        default=TransactionType.NFTOKEN_CANCEL_OFFER,
         init=False,
     )
 
-    def _get_errors(self: AMMCreate) -> Dict[str, str]:
+    def _get_errors(self: NFTokenCancelOffer) -> Dict[str, str]:
         return {
             key: value
             for key, value in {
                 **super()._get_errors(),
-                "trading_fee": self._get_trading_fee_error(),
+                "nftoken_offers": self._get_nftoken_offers_error(),
             }.items()
             if value is not None
         }
 
-    def _get_trading_fee_error(self: AMMCreate) -> Optional[str]:
-        if self.trading_fee < 0 or self.trading_fee > AMM_MAX_TRADING_FEE:
-            return f"Must be between 0 and {AMM_MAX_TRADING_FEE}"
+    def _get_nftoken_offers_error(self: NFTokenCancelOffer) -> Optional[str]:
+        if len(self.nftoken_offers) < 1:
+            return "Must specify at least one NFTokenOffer to cancel"
         return None
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/check_cancel.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/check_cancel.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/check_cash.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/check_create.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,63 @@
-"""Model for CheckCash transaction type."""
-from __future__ import annotations  # Requires Python 3.7+
-
+"""Model for CheckCreate transaction type."""
 from dataclasses import dataclass, field
-from typing import Dict, Optional
+from typing import Optional
 
 from xrpl.models.amounts import Amount
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class CheckCash(Transaction):
+class CheckCreate(Transaction):
+    """
+    Represents a `CheckCreate <https://xrpl.org/checkcreate.html>`_ transaction,
+    which creates a Check object. A Check object is a deferred payment
+    that can be cashed by its intended destination. The sender of this
+    transaction is the sender of the Check.
     """
-    Represents a `CheckCash transaction <https://xrpl.org/checkcash.html>`_,
-    which redeems a Check object to receive up to the amount authorized by the
-    corresponding CheckCreate transaction. Only the Destination address of a
-    Check can cash it.
+
+    destination: str = REQUIRED  # type: ignore
+    """
+    The address of the `account
+    <https://xrpl.org/accounts.html>`_ that can cash the Check. This field is
+    required.
+
+    :meta hide-value:
     """
 
-    check_id: str = REQUIRED  # type: ignore
+    send_max: Amount = REQUIRED  # type: ignore
     """
-    The ID of the `Check ledger object
-    <https://xrpl.org/check.html>`_ to cash, as a 64-character
-    hexadecimal string. This field is required.
+    Maximum amount of source token the Check is allowed to debit the
+    sender, including transfer fees on non-XRP tokens. The Check can only
+    credit the destination with the same token (from the same issuer, for
+    non-XRP tokens). This field is required.
 
     :meta hide-value:
     """
 
-    amount: Optional[Amount] = None
+    destination_tag: Optional[int] = None
     """
-    Redeem the Check for exactly this amount, if possible. The currency must
-    match that of the SendMax of the corresponding CheckCreate transaction.
-    You must provide either this field or ``DeliverMin``.
+    An arbitrary `destination tag
+    <https://xrpl.org/source-and-destination-tags.html>`_ that
+    identifies the reason for the Check, or a hosted recipient to pay.
     """
 
-    deliver_min: Optional[Amount] = None
+    expiration: Optional[int] = None
     """
-    Redeem the Check for at least this amount and for as much as possible.
-    The currency must match that of the ``SendMax`` of the corresponding
-    CheckCreate transaction. You must provide either this field or ``Amount``.
+    Time after which the Check is no longer valid, in seconds since the
+    Ripple Epoch.
+    """
+
+    invoice_id: Optional[str] = None
+    """
+    Arbitrary 256-bit hash representing a specific reason or identifier for
+    this Check.
     """
 
     transaction_type: TransactionType = field(
-        default=TransactionType.CHECK_CASH,
+        default=TransactionType.CHECK_CREATE,
         init=False,
     )
-
-    def _get_errors(self: CheckCash) -> Dict[str, str]:
-        errors = super()._get_errors()
-        if not (self.amount is None) ^ (self.deliver_min is None):
-            errors[
-                "CheckCash"
-            ] = "either amount or deliver_min must be set but not both"
-        return errors
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/check_create.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_create.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,75 @@
-"""Model for CheckCreate transaction type."""
+"""Model for PaymentChannelCreate transaction type."""
 from dataclasses import dataclass, field
 from typing import Optional
 
 from xrpl.models.amounts import Amount
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class CheckCreate(Transaction):
+class PaymentChannelCreate(Transaction):
     """
-    Represents a `CheckCreate <https://xrpl.org/checkcreate.html>`_ transaction,
-    which creates a Check object. A Check object is a deferred payment
-    that can be cashed by its intended destination. The sender of this
-    transaction is the sender of the Check.
+    Represents a `PaymentChannelCreate
+    <https://xrpl.org/paymentchannelcreate.html>`_ transaction, which creates a
+    `payment channel <https://xrpl.org/payment-channels.html>`_ and funds it with
+    XRP. The sender of this transaction is the "source address" of the payment
+    channel.
     """
 
-    destination: str = REQUIRED  # type: ignore
+    amount: Amount = REQUIRED  # type: ignore
     """
-    The address of the `account
-    <https://xrpl.org/accounts.html>`_ that can cash the Check. This field is
+    The amount of XRP, in drops, to set aside in this channel. This field is
     required.
 
     :meta hide-value:
     """
 
-    send_max: Amount = REQUIRED  # type: ignore
+    destination: str = REQUIRED  # type: ignore
     """
-    Maximum amount of source token the Check is allowed to debit the
-    sender, including transfer fees on non-XRP tokens. The Check can only
-    credit the destination with the same token (from the same issuer, for
-    non-XRP tokens). This field is required.
+    The account that can receive XRP from this channel, also known as the
+    "destination address" of the channel. Cannot be the same as the sender.
+    This field is required.
 
     :meta hide-value:
     """
 
-    destination_tag: Optional[int] = None
+    settle_delay: int = REQUIRED  # type: ignore
     """
-    An arbitrary `destination tag
-    <https://xrpl.org/source-and-destination-tags.html>`_ that
-    identifies the reason for the Check, or a hosted recipient to pay.
+    The amount of time, in seconds, the source address must wait between
+    requesting to close the channel and fully closing it. This field is
+    required.
+
+    :meta hide-value:
     """
 
-    expiration: Optional[int] = None
+    public_key: str = REQUIRED  # type: ignore
     """
-    Time after which the Check is no longer valid, in seconds since the
-    Ripple Epoch.
+    The public key of the key pair that the source will use to authorize
+    claims against this  channel, as hexadecimal. This can be any valid
+    secp256k1 or Ed25519 public key. This field is required.
+
+    :meta hide-value:
+    """
+
+    cancel_after: Optional[int] = None
+    """
+    An immutable expiration time for the channel, in seconds since the Ripple
+    Epoch. The channel can be closed sooner than this but cannot remain open
+    later than this time.
     """
 
-    invoice_id: Optional[str] = None
+    destination_tag: Optional[int] = None
     """
-    Arbitrary 256-bit hash representing a specific reason or identifier for
-    this Check.
+    An arbitrary `destination tag
+    <https://xrpl.org/source-and-destination-tags.html>`_ that
+    identifies the reason for the Payment Channel, or a hosted recipient to pay.
     """
 
     transaction_type: TransactionType = field(
-        default=TransactionType.CHECK_CREATE,
+        default=TransactionType.PAYMENT_CHANNEL_CREATE,
         init=False,
     )
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/deposit_preauth.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/deposit_preauth.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/escrow_cancel.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_cancel.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/escrow_create.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_create.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/escrow_finish.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_finish.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/metadata.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/metadata.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/nftoken_accept_offer.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_accept_offer.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/nftoken_burn.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_burn.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/nftoken_create_offer.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_create_offer.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/nftoken_mint.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_mint.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/offer_cancel.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/offer_cancel.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/offer_create.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/offer_create.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/payment.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/payment.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/payment_channel_claim.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_claim.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/payment_channel_create.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_fund.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,49 @@
-"""Model for PaymentChannelCreate transaction type."""
+"""Model for a PaymentChannelFund transaction type."""
 from dataclasses import dataclass, field
 from typing import Optional
 
-from xrpl.models.amounts import Amount
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class PaymentChannelCreate(Transaction):
+class PaymentChannelFund(Transaction):
     """
-    Represents a `PaymentChannelCreate
-    <https://xrpl.org/paymentchannelcreate.html>`_ transaction, which creates a
-    `payment channel <https://xrpl.org/payment-channels.html>`_ and funds it with
-    XRP. The sender of this transaction is the "source address" of the payment
-    channel.
+    Represents a `PaymentChannelFund <https://xrpl.org/paymentchannelfund.html>`_
+    transaction, adds additional XRP to an open `payment channel
+    <https://xrpl.org/payment-channels.html>`_, and optionally updates the
+    expiration time of the channel. Only the source address
+    of the channel can use this transaction.
     """
 
-    amount: Amount = REQUIRED  # type: ignore
+    channel: str = REQUIRED  # type: ignore
     """
-    The amount of XRP, in drops, to set aside in this channel. This field is
-    required.
+    The unique ID of the payment channel, as a 64-character hexadecimal
+    string. This field is required.
 
     :meta hide-value:
     """
 
-    destination: str = REQUIRED  # type: ignore
-    """
-    The account that can receive XRP from this channel, also known as the
-    "destination address" of the channel. Cannot be the same as the sender.
-    This field is required.
-
-    :meta hide-value:
+    amount: str = REQUIRED  # type: ignore
     """
-
-    settle_delay: int = REQUIRED  # type: ignore
-    """
-    The amount of time, in seconds, the source address must wait between
-    requesting to close the channel and fully closing it. This field is
+    The amount of XRP, in drops, to add to the channel. This field is
     required.
 
     :meta hide-value:
     """
 
-    public_key: str = REQUIRED  # type: ignore
-    """
-    The public key of the key pair that the source will use to authorize
-    claims against this  channel, as hexadecimal. This can be any valid
-    secp256k1 or Ed25519 public key. This field is required.
-
-    :meta hide-value:
-    """
-
-    cancel_after: Optional[int] = None
-    """
-    An immutable expiration time for the channel, in seconds since the Ripple
-    Epoch. The channel can be closed sooner than this but cannot remain open
-    later than this time.
-    """
-
-    destination_tag: Optional[int] = None
+    expiration: Optional[int] = None
     """
-    An arbitrary `destination tag
-    <https://xrpl.org/source-and-destination-tags.html>`_ that
-    identifies the reason for the Payment Channel, or a hosted recipient to pay.
+    A new mutable expiration time to set for the channel, in seconds since the
+    Ripple Epoch. This must be later than the existing expiration time of the
+    channel or later than the current time plus the settle delay of the channel.
+    This is separate from the immutable ``cancel_after`` time.
     """
 
     transaction_type: TransactionType = field(
-        default=TransactionType.PAYMENT_CHANNEL_CREATE,
+        default=TransactionType.PAYMENT_CHANNEL_FUND,
         init=False,
     )
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/payment_channel_fund.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/set_fee.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,63 @@
-"""Model for a PaymentChannelFund transaction type."""
+"""Model for SetFee pseudo-transaction type."""
+
 from dataclasses import dataclass, field
 from typing import Optional
 
 from xrpl.models.required import REQUIRED
-from xrpl.models.transactions.transaction import Transaction
-from xrpl.models.transactions.types import TransactionType
+from xrpl.models.transactions.pseudo_transactions.pseudo_transaction import (
+    PseudoTransaction,
+)
+from xrpl.models.transactions.types import PseudoTransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class PaymentChannelFund(Transaction):
+class SetFee(PseudoTransaction):
+    """
+    A SetFee pseudo-transaction marks a change in `transaction cost
+    <https://xrpl.org/transaction-cost.html>`_ or `reserve requirements
+    <https://xrpl.org/reserves.html>`_ as a result of `Fee Voting
+    <https://xrpl.org/fee-voting.html>`_.
+    """
+
+    base_fee: str = REQUIRED  # type: ignore
     """
-    Represents a `PaymentChannelFund <https://xrpl.org/paymentchannelfund.html>`_
-    transaction, adds additional XRP to an open `payment channel
-    <https://xrpl.org/payment-channels.html>`_, and optionally updates the
-    expiration time of the channel. Only the source address
-    of the channel can use this transaction.
+    The charge, in drops of XRP, for the reference transaction, as hex. (This is the
+    transaction cost before scaling for load.) This field is required.
+
+    :meta hide-value:
+    """
+
+    reference_fee_units: int = REQUIRED  # type: ignore
+    """
+    The cost, in fee units, of the reference transaction. This field is required.
+
+    :meta hide-value:
     """
 
-    channel: str = REQUIRED  # type: ignore
+    reserve_base: int = REQUIRED  # type: ignore
     """
-    The unique ID of the payment channel, as a 64-character hexadecimal
-    string. This field is required.
+    The base reserve, in drops. This field is required.
 
     :meta hide-value:
     """
 
-    amount: str = REQUIRED  # type: ignore
+    reserve_increment: int = REQUIRED  # type: ignore
     """
-    The amount of XRP, in drops, to add to the channel. This field is
-    required.
+    The incremental reserve, in drops. This field is required.
 
     :meta hide-value:
     """
 
-    expiration: Optional[int] = None
+    ledger_sequence: Optional[int] = None
     """
-    A new mutable expiration time to set for the channel, in seconds since the
-    Ripple Epoch. This must be later than the existing expiration time of the
-    channel or later than the current time plus the settle delay of the channel.
-    This is separate from the immutable ``cancel_after`` time.
+    The index of the ledger version where this pseudo-transaction appears. This
+    distinguishes the pseudo-transaction from other occurrences of the same change.
+    This field is omitted for some historical SetFee pseudo-transactions.
     """
 
-    transaction_type: TransactionType = field(
-        default=TransactionType.PAYMENT_CHANNEL_FUND,
+    transaction_type: PseudoTransactionType = field(
+        default=PseudoTransactionType.SET_FEE,
         init=False,
     )
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/pseudo_transactions/__init__.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/pseudo_transactions/set_fee.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/unl_modify.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,71 @@
-"""Model for SetFee pseudo-transaction type."""
+"""Model for UNLModify pseudo-transaction type."""
+
+from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Optional
+from typing import Dict
 
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.pseudo_transactions.pseudo_transaction import (
     PseudoTransaction,
 )
 from xrpl.models.transactions.types import PseudoTransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class SetFee(PseudoTransaction):
-    """
-    A SetFee pseudo-transaction marks a change in `transaction cost
-    <https://xrpl.org/transaction-cost.html>`_ or `reserve requirements
-    <https://xrpl.org/reserves.html>`_ as a result of `Fee Voting
-    <https://xrpl.org/fee-voting.html>`_.
-    """
-
-    base_fee: str = REQUIRED  # type: ignore
+class UNLModify(PseudoTransaction):
     """
-    The charge, in drops of XRP, for the reference transaction, as hex. (This is the
-    transaction cost before scaling for load.) This field is required.
-
-    :meta hide-value:
+    A UNLModify pseudo-transaction marks a change to the `Negative UNL
+    <https://xrpl.org/negative-unl.html>`_, indicating that a trusted validator has
+    gone offline or come back online.
     """
 
-    reference_fee_units: int = REQUIRED  # type: ignore
+    ledger_sequence: int = REQUIRED  # type: ignore
     """
-    The cost, in fee units, of the reference transaction. This field is required.
+    The ledger index where this pseudo-transaction appears. This distinguishes the
+    pseudo-transaction from other occurrences of the same change.
+    This field is required.
 
     :meta hide-value:
     """
 
-    reserve_base: int = REQUIRED  # type: ignore
+    unl_modify_disabling: int = REQUIRED  # type: ignore
     """
-    The base reserve, in drops. This field is required.
+    If 1, this change represents adding a validator to the Negative UNL. If 0, this
+    change represents removing a validator from the Negative UNL. (No other values
+    are allowed.) This field is required.
 
     :meta hide-value:
     """
 
-    reserve_increment: int = REQUIRED  # type: ignore
+    unl_modify_validator: str = REQUIRED  # type: ignore
     """
-    The incremental reserve, in drops. This field is required.
+    The validator to add or remove, as identified by its master public key.
+    This field is required.
 
     :meta hide-value:
     """
 
-    ledger_sequence: Optional[int] = None
-    """
-    The index of the ledger version where this pseudo-transaction appears. This
-    distinguishes the pseudo-transaction from other occurrences of the same change.
-    This field is omitted for some historical SetFee pseudo-transactions.
-    """
-
     transaction_type: PseudoTransactionType = field(
-        default=PseudoTransactionType.SET_FEE,
+        default=PseudoTransactionType.UNL_MODIFY,
         init=False,
     )
+
+    flags: int = 0
+    """
+    The Flags value of the EnableAmendment pseudo-transaction indicates the status
+    of the amendment at the time of the ledger including the pseudo-transaction.
+    A Flags value of 0 (no flags) or an omitted Flags field indicates that the
+    amendment has been enabled, and applies to all ledgers afterward.
+    """
+
+    def _get_errors(self: UNLModify) -> Dict[str, str]:
+        errors = super()._get_errors()
+        if self.unl_modify_disabling not in {0, 1}:
+            errors[
+                "unl_modify_disabling"
+            ] = "`unl_modify_disabling` is not equal to 0 or 1."
+
+        return errors
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/pseudo_transactions/unl_modify.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/trust_set.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,87 @@
-"""Model for UNLModify pseudo-transaction type."""
-
-from __future__ import annotations
+"""
+Represents a TrustSet transaction on the XRP Ledger.
+Creates or modifies a trust line linking two accounts.
 
+`See TrustSet <https://xrpl.org/trustset.html>`_
+"""
 from dataclasses import dataclass, field
-from typing import Dict
+from enum import Enum
+from typing import Optional
 
+from xrpl.models.amounts import IssuedCurrencyAmount
+from xrpl.models.flags import FlagInterface
 from xrpl.models.required import REQUIRED
-from xrpl.models.transactions.pseudo_transactions.pseudo_transaction import (
-    PseudoTransaction,
-)
-from xrpl.models.transactions.types import PseudoTransactionType
+from xrpl.models.transactions.transaction import Transaction
+from xrpl.models.transactions.types import TransactionType
 from xrpl.models.utils import require_kwargs_on_init
 
 
-@require_kwargs_on_init
-@dataclass(frozen=True)
-class UNLModify(PseudoTransaction):
+class TrustSetFlag(int, Enum):
     """
-    A UNLModify pseudo-transaction marks a change to the `Negative UNL
-    <https://xrpl.org/negative-unl.html>`_, indicating that a trusted validator has
-    gone offline or come back online.
+    Transactions of the TrustSet type support additional values in the Flags field.
+    This enum represents those options.
     """
 
-    ledger_sequence: int = REQUIRED  # type: ignore
+    TF_SET_AUTH = 0x00010000
+    """
+    Authorize the other party to hold
+    `currency issued by this account <https://xrpl.org/tokens.html>`_.
+    (No effect unless using the `asfRequireAuth AccountSet flag
+    <https://xrpl.org/accountset.html#accountset-flags>`_.) Cannot be unset.
     """
-    The ledger index where this pseudo-transaction appears. This distinguishes the
-    pseudo-transaction from other occurrences of the same change.
-    This field is required.
 
-    :meta hide-value:
+    TF_SET_NO_RIPPLE = 0x00020000
+    """
+    Enable the No Ripple flag, which blocks
+    `rippling <https://xrpl.org/rippling.html>`_ between two trust
+    lines of the same currency if this flag is enabled on both.
+    """
+
+    TF_CLEAR_NO_RIPPLE = 0x00040000
+    """Disable the No Ripple flag, allowing rippling on this trust line."""
+
+    TF_SET_FREEZE = 0x00100000
+    """Freeze the trust line."""
+
+    TF_CLEAR_FREEZE = 0x00200000
+    """Unfreeze the trust line."""
+
+
+class TrustSetFlagInterface(FlagInterface):
+    """
+    Transactions of the TrustSet type support additional values in the Flags field.
+    This TypedDict represents those options.
     """
 
-    unl_modify_disabling: int = REQUIRED  # type: ignore
+    TF_SET_AUTH: bool
+    TF_SET_NO_RIPPLE: bool
+    TF_CLEAR_NO_RIPPLE: bool
+    TF_SET_FREEZE: bool
+    TF_CLEAR_FREEZE: bool
+
+
+@require_kwargs_on_init
+@dataclass(frozen=True)
+class TrustSet(Transaction):
     """
-    If 1, this change represents adding a validator to the Negative UNL. If 0, this
-    change represents removing a validator from the Negative UNL. (No other values
-    are allowed.) This field is required.
+    Represents a TrustSet transaction on the XRP Ledger.
+    Creates or modifies a trust line linking two accounts.
 
-    :meta hide-value:
+    `See TrustSet <https://xrpl.org/trustset.html>`_
     """
 
-    unl_modify_validator: str = REQUIRED  # type: ignore
+    limit_amount: IssuedCurrencyAmount = REQUIRED  # type: ignore
     """
-    The validator to add or remove, as identified by its master public key.
     This field is required.
 
     :meta hide-value:
     """
 
-    transaction_type: PseudoTransactionType = field(
-        default=PseudoTransactionType.UNL_MODIFY,
-        init=False,
-    )
+    quality_in: Optional[int] = None
 
-    flags: int = 0
-    """
-    The Flags value of the EnableAmendment pseudo-transaction indicates the status
-    of the amendment at the time of the ledger including the pseudo-transaction.
-    A Flags value of 0 (no flags) or an omitted Flags field indicates that the
-    amendment has been enabled, and applies to all ledgers afterward.
-    """
-
-    def _get_errors(self: UNLModify) -> Dict[str, str]:
-        errors = super()._get_errors()
-        if self.unl_modify_disabling not in {0, 1}:
-            errors[
-                "unl_modify_disabling"
-            ] = "`unl_modify_disabling` is not equal to 0 or 1."
+    quality_out: Optional[int] = None
 
-        return errors
+    transaction_type: TransactionType = field(
+        default=TransactionType.TRUST_SET,
+        init=False,
+    )
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/set_regular_key.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/set_regular_key.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/signer_list_set.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/signer_list_set.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/ticket_create.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/ticket_create.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/transactions/transaction.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,33 @@
 from hashlib import sha512
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 from typing_extensions import Final
 
 from xrpl.core.binarycodec import encode
 from xrpl.models.amounts import IssuedCurrencyAmount
-from xrpl.models.base_model import ABBREVIATIONS, BaseModel
+from xrpl.models.base_model import BaseModel
 from xrpl.models.exceptions import XRPLModelException
 from xrpl.models.flags import check_false_flag_definition, interface_to_flag_list
 from xrpl.models.nested_model import NestedModel
 from xrpl.models.requests import PathStep
 from xrpl.models.required import REQUIRED
 from xrpl.models.transactions.types import PseudoTransactionType, TransactionType
 from xrpl.models.types import XRPL_VALUE_TYPE
 from xrpl.models.utils import require_kwargs_on_init
 
 _TRANSACTION_HASH_PREFIX: Final[int] = 0x54584E00
-
-# special cases that should not be snake cased and only contain primitive members
-_LOWER_CASE_MODELS: List[Type[BaseModel]] = [
-    IssuedCurrencyAmount,
-    PathStep,
-]
+# This is used to make exceptions when converting dictionary keys to xrpl JSON
+# keys. We snake case keys, but some keys are abbreviations.
+_ABBREVIATIONS: Final[Dict[str, str]] = {
+    "unl": "UNL",
+    "id": "ID",
+    "uri": "URI",
+    "nftoken": "NFToken",
+}
 
 
 def transaction_json_to_binary_codec_form(
     dictionary: Dict[str, XRPL_VALUE_TYPE]
 ) -> Dict[str, XRPL_VALUE_TYPE]:
     """
     Returns a new dictionary in which the keys have been formatted as CamelCase and
@@ -50,43 +52,36 @@
 
 def _key_to_tx_json(key: str) -> str:
     """
     Transforms snake_case to PascalCase. For example:
         1. 'transaction_type' becomes 'TransactionType'
         2. 'URI' becomes 'uri'
 
-    Known abbreviations (example 2 above) need to be enumerated in ABBREVIATIONS.
+    Known abbreviations (example 2 above) need to be enumerated in _ABBREVIATIONS.
     """
     return "".join(
         [
-            ABBREVIATIONS[word] if word in ABBREVIATIONS else word.capitalize()
+            _ABBREVIATIONS[word] if word in _ABBREVIATIONS else word.capitalize()
             for word in key.split("_")
         ]
     )
 
 
 def _value_to_tx_json(value: XRPL_VALUE_TYPE) -> XRPL_VALUE_TYPE:
-    if isinstance(value, dict) and "auth_account" in value:
-        return _auth_account_value_to_tx_json(value)
-    if any([model.is_dict_of_model(value) for model in _LOWER_CASE_MODELS]):
+    # IssuedCurrencyAmount and PathStep are special cases and should not be snake cased
+    # and only contain primitive members
+    if IssuedCurrencyAmount.is_dict_of_model(value) or PathStep.is_dict_of_model(value):
         return value
     if isinstance(value, dict):
         return transaction_json_to_binary_codec_form(value)
     if isinstance(value, list):
         return [_value_to_tx_json(sub_value) for sub_value in value]
     return value
 
 
-def _auth_account_value_to_tx_json(value: Dict[str, Any]) -> Dict[str, Any]:
-    return {
-        _key_to_tx_json(key): transaction_json_to_binary_codec_form(val)
-        for (key, val) in value.items()
-    }
-
-
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class Memo(NestedModel):
     """
     An arbitrary piece of data attached to a transaction. A transaction can
     have multiple Memo objects as an array in the Memos field.
     Must contain one or more of ``memo_data``, ``memo_format``, and
@@ -383,15 +378,15 @@
 
         Returns:
             The hash of the Transaction object.
 
         Raises:
             XRPLModelException: if the Transaction is unsigned.
         """
-        if self.txn_signature is None and self.signers is None:
+        if self.txn_signature is None:
             raise XRPLModelException(
                 "Cannot get the hash from an unsigned Transaction."
             )
         prefix = hex(_TRANSACTION_HASH_PREFIX)[2:].upper()
         encoded_str = bytes.fromhex(prefix + encode(self.to_xrpl()))
         return sha512(encoded_str).digest().hex().upper()[:64]
```

### Comparing `xrpl-py-1.9.0b0/xrpl/models/types.py` & `xrpl-py-2.0.0b0/xrpl/models/types.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/models/utils.py` & `xrpl-py-2.0.0b0/xrpl/models/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/transaction/__init__.py` & `xrpl-py-2.0.0b0/xrpl/transaction/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     safe_sign_and_submit_transaction,
     safe_sign_transaction,
     sign,
     sign_and_submit,
     submit,
     submit_transaction,
 )
-from xrpl.transaction.multisign import multisign
 from xrpl.transaction.reliable_submission import send_reliable_submission
 
 __all__ = [
     "autofill",
     "autofill_and_sign",
     "get_transaction_from_hash",
     "safe_sign_transaction",
@@ -27,10 +26,9 @@
     "safe_sign_and_submit_transaction",
     "sign",
     "sign_and_submit",
     "submit",
     "submit_transaction",
     "transaction_json_to_binary_codec_form",
     "send_reliable_submission",
-    "multisign",
     "XRPLReliableSubmissionException",
 ]
```

### Comparing `xrpl-py-1.9.0b0/xrpl/transaction/ledger.py` & `xrpl-py-2.0.0b0/xrpl/transaction/ledger.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/transaction/main.py` & `xrpl-py-2.0.0b0/xrpl/transaction/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """High-level transaction methods with XRPL transactions."""
 import asyncio
-from typing import Optional
 
 from xrpl.asyncio.transaction import main
 from xrpl.clients.sync_client import SyncClient
 from xrpl.models.response import Response
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.wallet.main import Wallet
 
@@ -73,35 +72,32 @@
 submit_transaction = submit
 
 
 def sign(
     transaction: Transaction,
     wallet: Wallet,
     check_fee: bool = True,
-    multisign: bool = False,
 ) -> Transaction:
     """
     Signs a transaction locally, without trusting external rippled nodes.
 
     Args:
         transaction: the transaction to be signed.
         wallet: the wallet with which to sign the transaction.
         check_fee: whether to check if the fee is higher than the expected transaction
             type fee. Defaults to True.
-        multisign: whether to sign the transaction for a multisignature transaction.
 
     Returns:
         The signed transaction.
     """
     return asyncio.run(
         main.sign(
             transaction,
             wallet,
             check_fee,
-            multisign,
         )
     )
 
 
 safe_sign_transaction = sign
 
 
@@ -134,31 +130,26 @@
         )
     )
 
 
 safe_sign_and_autofill_transaction = autofill_and_sign
 
 
-def autofill(
-    transaction: Transaction, client: SyncClient, signers_count: Optional[int] = None
-) -> Transaction:
+def autofill(transaction: Transaction, client: SyncClient) -> Transaction:
     """
     Autofills fields in a transaction. This will set `sequence`, `fee`, and
     `last_ledger_sequence` according to the current state of the server this Client is
     connected to. It also converts all X-Addresses to classic addresses.
 
     Args:
         transaction: the transaction to be signed.
         client: a network client.
-        signers_count: the expected number of signers for this transaction.
-            Only used for multisigned transactions.
 
     Returns:
         The autofilled transaction.
     """
     return asyncio.run(
         main.autofill(
             transaction,
             client,
-            signers_count,
         )
     )
```

### Comparing `xrpl-py-1.9.0b0/xrpl/transaction/reliable_submission.py` & `xrpl-py-2.0.0b0/xrpl/transaction/reliable_submission.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/__init__.py` & `xrpl-py-2.0.0b0/xrpl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/parse_nftoken_id.py` & `xrpl-py-2.0.0b0/xrpl/utils/parse_nftoken_id.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/sidechain.py` & `xrpl-py-2.0.0b0/xrpl/utils/sidechain.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/str_conversions.py` & `xrpl-py-2.0.0b0/xrpl/utils/str_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/time_conversions.py` & `xrpl-py-2.0.0b0/xrpl/utils/time_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/txn_parser/get_balance_changes.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_balance_changes.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/txn_parser/get_final_balances.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_final_balances.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/txn_parser/get_order_book_changes.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_order_book_changes.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/txn_parser/utils/__init__.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/txn_parser/utils/balance_parser.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/balance_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/txn_parser/utils/nodes.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/nodes.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/txn_parser/utils/order_book_parser.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/order_book_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/txn_parser/utils/parser.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/parser.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/txn_parser/utils/types.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/types.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/utils/xrp_conversions.py` & `xrpl-py-2.0.0b0/xrpl/utils/xrp_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/xrpl/wallet/wallet_generation.py` & `xrpl-py-2.0.0b0/xrpl/wallet/wallet_generation.py`

 * *Files identical despite different names*

### Comparing `xrpl-py-1.9.0b0/setup.py` & `xrpl-py-2.0.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 
 extras_require = \
 {':python_version >= "3.10" and python_version < "4.0"': ['websockets>=10.0,<11.0'],
  ':python_version >= "3.7" and python_version < "3.10"': ['websockets>=9.0.1,<11.0']}
 
 setup_kwargs = {
     'name': 'xrpl-py',
-    'version': '1.9.0b0',
+    'version': '2.0.0b0',
     'description': 'A complete Python library for interacting with the XRP ledger',
-    'long_description': '[![Documentation Status](https://readthedocs.org/projects/xrpl-py/badge)](https://xrpl-py.readthedocs.io/)\n\n# xrpl-py\n\nA pure Python implementation for interacting with the XRP Ledger, the `xrpl-py` library simplifies the hardest parts of XRP Ledger interaction, like serialization and transaction signing, by providing native Python methods and models for [XRP Ledger transactions](https://xrpl.org/transaction-formats.html) and core server [API](https://xrpl.org/api-conventions.html) ([`rippled`](https://github.com/ripple/rippled)) objects.\n\n\n\n```py\n# create a network client\nfrom xrpl.clients import JsonRpcClient\nclient = JsonRpcClient("https://s.altnet.rippletest.net:51234")\n\n# create a wallet on the testnet\nfrom xrpl.wallet import generate_faucet_wallet\ntest_wallet = generate_faucet_wallet(client)\nprint(test_wallet)\npublic_key: ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56\nprivate_key: -HIDDEN-\nclassic_address: rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo\n\n# look up account info\nfrom xrpl.models.requests.account_info import AccountInfo\nacct_info = AccountInfo(\n    account="rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",\n    ledger_index="current",\n    queue=True,\n    strict=True,\n)\nresponse = client.request(acct_info)\nresult = response.result\nimport json\nprint(json.dumps(result["account_data"], indent=4, sort_keys=True))\n# {\n#     "Account": "rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",\n#     "Balance": "1000000000",\n#     "Flags": 0,\n#     "LedgerEntryType": "AccountRoot",\n#     "OwnerCount": 0,\n#     "PreviousTxnID": "73CD4A37537A992270AAC8472F6681F44E400CBDE04EC8983C34B519F56AB107",\n#     "PreviousTxnLgrSeq": 16233962,\n#     "Sequence": 16233962,\n#     "index": "FD66EC588B52712DCE74831DCB08B24157DC3198C29A0116AA64D310A58512D7"\n# }\n```\n\n[![Downloads](https://pepy.tech/badge/xrpl-py/month)](https://pepy.tech/project/xrpl-py/month)\n[![Contributors](https://img.shields.io/github/contributors/xpring-eng/xrpl-py.svg)](https://github.com/xpring-eng/xrpl-py/graphs/contributors)\n\n## Installation and supported versions\n\nThe `xrpl-py` library is available on [PyPI](https://pypi.org/). Install with `pip`:\n\n\n```\npip3 install xrpl-py\n```\n\nThe library supports [Python 3.7](https://www.python.org/downloads/) and later.\n\n[![Supported Versions](https://img.shields.io/pypi/pyversions/xrpl-py.svg)](https://pypi.org/project/xrpl-py)\n\n\n## Features\n\nUse `xrpl-py` to build Python applications that leverage the [XRP Ledger](https://xrpl.org/). The library helps with all aspects of interacting with the XRP Ledger, including:\n\n* Key and wallet management\n* Serialization\n* Transaction Signing\n\n`xrpl-py` also provides:\n\n* A network client — See [`xrpl.clients`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.clients.html) for more information.\n* Methods for inspecting accounts — See [XRPL Account Methods](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.account.html) for more information.\n* Codecs for encoding and decoding addresses and other objects — See [Core Codecs](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.html) for more information.\n\n## [➡️ Reference Documentation](https://xrpl-py.readthedocs.io/en/stable/)\n\nSee the complete [`xrpl-py` reference documentation on Read the Docs](https://xrpl-py.readthedocs.io/en/stable/index.html).\n\n\n## Usage\n\nThe following sections describe some of the most commonly used modules in the `xrpl-py` library and provide sample code.\n\n### Network client\n\nUse the `xrpl.clients` library to create a network client for connecting to the XRP Ledger.\n\n```py\nfrom xrpl.clients import JsonRpcClient\nJSON_RPC_URL = "https://s.altnet.rippletest.net:51234"\nclient = JsonRpcClient(JSON_RPC_URL)\n```\n\n### Manage keys and wallets\n\n#### `xrpl.wallet`\n\nUse the [`xrpl.wallet`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.wallet.html) module to create a wallet from a given seed or or via a [Testnet faucet](https://xrpl.org/xrp-testnet-faucet.html).\n\nTo create a wallet from a seed (in this case, the value generated using [`xrpl.keypairs`](#xrpl-keypairs)):\n\n```py\nwallet_from_seed = xrpl.wallet.Wallet(seed, 0)\nprint(wallet_from_seed)\n# pub_key: ED46949E414A3D6D758D347BAEC9340DC78F7397FEE893132AAF5D56E4D7DE77B0\n# priv_key: -HIDDEN-\n# classic_address: rG5ZvYsK5BPi9f1Nb8mhFGDTNMJhEhufn6\n```\n\nTo create a wallet from a Testnet faucet:\n\n```py\ntest_wallet = generate_faucet_wallet(client)\ntest_account = test_wallet.classic_address\nprint("Classic address:", test_account)\n# Classic address: rEQB2hhp3rg7sHj6L8YyR4GG47Cb7pfcuw\n```\n\n#### `xrpl.core.keypairs`\n\nUse the [`xrpl.core.keypairs`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.keypairs.html#module-xrpl.core.keypairs) module to generate seeds and derive keypairs and addresses from those seed values.\n\nHere\'s an example of how to generate a `seed` value and derive an [XRP Ledger "classic" address](https://xrpl.org/cryptographic-keys.html#account-id-and-address) from that seed.\n\n\n```py\nfrom xrpl.core import keypairs\nseed = keypairs.generate_seed()\npublic, private = keypairs.derive_keypair(seed)\ntest_account = keypairs.derive_classic_address(public)\nprint("Here\'s the public key:")\nprint(public)\nprint("Here\'s the private key:")\nprint(private)\nprint("Store this in a secure place!")\n# Here\'s the public key:\n# ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56\n# Here\'s the private key:\n# EDE65EE7882847EF5345A43BFB8E6F5EEC60F45461696C384639B99B26AAA7A5CD\n# Store this in a secure place!\n```\n\n**Note:** You can use `xrpl.core.keypairs.sign` to sign transactions but `xrpl-py` also provides explicit methods for safely signing and submitting transactions. See [Transaction Signing](#transaction-signing) and [XRPL Transaction Methods](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#module-xrpl.transaction) for more information.\n\n\n### Serialize and sign transactions\n\nTo securely submit transactions to the XRP Ledger, you need to first serialize data from JSON and other formats into the [XRP Ledger\'s canonical format](https://xrpl.org/serialization.html), then to [authorize the transaction](https://xrpl.org/transaction-basics.html#authorizing-transactions) by digitally [signing it](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.keypairs.html?highlight=sign#xrpl.core.keypairs.sign) with the account\'s private key. The `xrpl-py` library provides several methods to simplify this process.\n\n\nUse the [`xrpl.transaction`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html) module to sign and submit transactions. The module offers three ways to do this:\n\n* [`sign_and_submit`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign_and_submit) — Signs a transaction locally, then submits it to the XRP Ledger. This method does not implement [reliable transaction submission](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission) best practices, so only use it for development or testing purposes.\n\n* [`sign`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign) — Signs a transaction locally. This method **does  not** submit the transaction to the XRP Ledger.\n\n* [`send_reliable_submission`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.send_reliable_submission) — An implementation of the [reliable transaction submission guidelines](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission), this method submits a signed transaction to the XRP Ledger and then verifies that it has been included in a validated ledger (or has failed to do so). Use this method to submit transactions for production purposes.\n\n\n```py\nfrom xrpl.models.transactions import Payment\nfrom xrpl.transaction import sign, send_reliable_submission\nfrom xrpl.ledger import get_latest_validated_ledger_sequence\nfrom xrpl.account import get_next_valid_seq_number\n\ncurrent_validated_ledger = get_latest_validated_ledger_sequence(client)\ntest_wallet.sequence = get_next_valid_seq_number(test_wallet.classic_address, client)\n\n# prepare the transaction\n# the amount is expressed in drops, not XRP\n# see https://xrpl.org/basic-data-types.html#specifying-currency-amounts\nmy_tx_payment = Payment(\n    account=test_wallet.classic_address,\n    amount="2200000",\n    destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",\n    last_ledger_sequence=current_validated_ledger + 20,\n    sequence=test_wallet.sequence,\n    fee="10",\n)\n# sign the transaction\nmy_tx_payment_signed = sign(my_tx_payment,test_wallet)\n\n# submit the transaction\ntx_response = send_reliable_submission(my_tx_payment_signed, client)\n```\n\n#### Get fee from the XRP Ledger\n\n\nIn most cases, you can specify the minimum [transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) of `"10"` for the `fee` field unless you have a strong reason not to. But if you want to get the [current load-balanced transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) from the network, you can use the `get_fee` function:\n\n```py\nfrom xrpl.ledger import get_fee\nfee = get_fee(client)\nprint(fee)\n# 10\n```\n\n#### Auto-filled fields\n\nThe `xrpl-py` library automatically populates the `fee`, `sequence` and `last_ledger_sequence` fields when you create transactions. In the example above, you could omit those fields and let the library fill them in for you.\n\n```py\nfrom xrpl.models.transactions import Payment\nfrom xrpl.transaction import send_reliable_submission, autofill_and_sign\n# prepare the transaction\n# the amount is expressed in drops, not XRP\n# see https://xrpl.org/basic-data-types.html#specifying-currency-amounts\nmy_tx_payment = Payment(\n    account=test_wallet.classic_address,\n    amount="2200000",\n    destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe"\n)\n\n# sign the transaction with the autofill method\n# (this will auto-populate the fee, sequence, and last_ledger_sequence)\nmy_tx_payment_signed = autofill_and_sign(my_tx_payment, test_wallet, client)\nprint(my_tx_payment_signed)\n# Payment(\n#     account=\'rMPUKmzmDWEX1tQhzQ8oGFNfAEhnWNFwz\',\n#     transaction_type=<TransactionType.PAYMENT: \'Payment\'>,\n#     fee=\'10\',\n#     sequence=16034065,\n#     account_txn_id=None,\n#     flags=0,\n#     last_ledger_sequence=10268600,\n#     memos=None,\n#     signers=None,\n#     source_tag=None,\n#     signing_pub_key=\'EDD9540FA398915F0BCBD6E65579C03BE5424836CB68B7EB1D6573F2382156B444\',\n#     txn_signature=\'938FB22AE7FE76CF26FD11F8F97668E175DFAABD2977BCA397233117E7E1C4A1E39681091CC4D6DF21403682803AB54CC21DC4FA2F6848811DEE10FFEF74D809\',\n#     amount=\'2200000\',\n#     destination=\'rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe\',\n#     destination_tag=None,\n#     invoice_id=None,\n#     paths=None,\n#     send_max=None,\n#     deliver_min=None\n# )\n\n# submit the transaction\ntx_response = send_reliable_submission(my_tx_payment_signed, client)\n```\n\n\n### Subscribe to ledger updates\n\nYou can send `subscribe` and `unsubscribe` requests only using the WebSocket network client. These request methods allow you to be alerted of certain situations as they occur, such as when a new ledger is declared.\n\n```py\nfrom xrpl.clients import WebsocketClient\nurl = "wss://s.altnet.rippletest.net/"\nfrom xrpl.models.requests import Subscribe, StreamParameter\nreq = Subscribe(streams=[StreamParameter.LEDGER])\n# NOTE: this code will run forever without a timeout, until the process is killed\nwith WebsocketClient(url) as client:\n    client.send(req)\n    for message in client:\n        print(message)\n# {\'result\': {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'7CD50477F23FF158B430772D8E82A961376A7B40E13C695AA849811EDF66C5C0\', \'ledger_index\': 18183504, \'ledger_time\': 676412962, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'validated_ledgers\': \'17469391-18183504\'}, \'status\': \'success\', \'type\': \'response\'}\n# {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'BAA743DABD168BD434804416C8087B7BDEF7E6D7EAD412B9102281DD83B10D00\', \'ledger_index\': 18183505, \'ledger_time\': 676412970, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'txn_count\': 0, \'type\': \'ledgerClosed\', \'validated_ledgers\': \'17469391-18183505\'}\n# {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'D8227DAF8F745AE3F907B251D40B4081E019D013ABC23B68C0B1431DBADA1A46\', \'ledger_index\': 18183506, \'ledger_time\': 676412971, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'txn_count\': 0, \'type\': \'ledgerClosed\', \'validated_ledgers\': \'17469391-18183506\'}\n# {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'CFC412B6DDB9A402662832A781C23F0F2E842EAE6CFC539FEEB287318092C0DE\', \'ledger_index\': 18183507, \'ledger_time\': 676412972, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'txn_count\': 0, \'type\': \'ledgerClosed\', \'validated_ledgers\': \'17469391-18183507\'}\n```\n\n\n### Asynchronous Code\n\nThis library supports Python\'s [`asyncio`](https://docs.python.org/3/library/asyncio.html) package, which is used to run asynchronous code. All the async code is in [`xrpl.asyncio`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.asyncio.html) If you are writing asynchronous code, please note that you will not be able to use any synchronous sugar functions, due to how event loops are handled. However, every synchronous method has a corresponding asynchronous method that you can use.\n\nThis sample code is the asynchronous equivalent of the above section on submitting a transaction.\n\n```py\nimport asyncio\nfrom xrpl.models.transactions import Payment\nfrom xrpl.asyncio.transaction import sign, send_reliable_submission\nfrom xrpl.asyncio.ledger import get_latest_validated_ledger_sequence\nfrom xrpl.asyncio.account import get_next_valid_seq_number\nfrom xrpl.asyncio.clients import AsyncJsonRpcClient\n\nasync_client = AsyncJsonRpcClient(JSON_RPC_URL)\n\nasync def submit_sample_transaction():\n    current_validated_ledger = await get_latest_validated_ledger_sequence(async_client)\n    test_wallet.sequence = await get_next_valid_seq_number(test_wallet.classic_address, async_client)\n\n    # prepare the transaction\n    # the amount is expressed in drops, not XRP\n    # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts\n    my_tx_payment = Payment(\n        account=test_wallet.classic_address,\n        amount="2200000",\n        destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",\n        last_ledger_sequence=current_validated_ledger + 20,\n        sequence=test_wallet.sequence,\n        fee="10",\n    )\n    # sign the transaction\n    my_tx_payment_signed = await sign(my_tx_payment,test_wallet)\n\n    # submit the transaction\n    tx_response = await send_reliable_submission(my_tx_payment_signed, async_client)\n\nasyncio.run(submit_sample_transaction())\n```\n\n### Encode addresses\n\nUse [`xrpl.core.addresscodec`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.addresscodec.html) to encode and decode addresses into and from the ["classic" and X-address formats](https://xrpl.org/accounts.html#addresses).\n\n```py\n# convert classic address to x-address\nfrom xrpl.core import addresscodec\ntestnet_xaddress = (\n    addresscodec.classic_address_to_xaddress(\n        "rMPUKmzmDWEX1tQhzQ8oGFNfAEhnWNFwz",\n        tag=0,\n        is_test_network=True,\n    )\n)\nprint(testnet_xaddress)\n# T7QDemmxnuN7a52A62nx2fxGPWcRahLCf3qaswfrsNW9Lps\n```\n\n\n## Contributing\n\nIf you want to contribute to this project, see [CONTRIBUTING.md].\n\n### Mailing Lists\n\nWe have a low-traffic mailing list for announcements of new `xrpl.js` releases. (About 1 email per week)\n\n+ [Subscribe to xrpl-announce](https://groups.google.com/g/xrpl-announce)\n\nIf you\'re using the XRP Ledger in production, you should run a [rippled server](https://github.com/ripple/rippled) and subscribe to the ripple-server mailing list as well.\n\n+ [Subscribe to ripple-server](https://groups.google.com/g/ripple-server)\n\n### Report an issue\n\nExperienced an issue? Report it [here](https://github.com/XRPLF/xrpl-py/issues/new).\n\n## License\n\nThe `xrpl-py` library is licensed under the ISC License. See [LICENSE] for more information.\n\n\n\n[CONTRIBUTING.md]: CONTRIBUTING.md\n[LICENSE]: LICENSE\n',
+    'long_description': '[![Documentation Status](https://readthedocs.org/projects/xrpl-py/badge)](https://xrpl-py.readthedocs.io/)\n\n# xrpl-py\n\nA pure Python implementation for interacting with the XRP Ledger, the `xrpl-py` library simplifies the hardest parts of XRP Ledger interaction, like serialization and transaction signing, by providing native Python methods and models for [XRP Ledger transactions](https://xrpl.org/transaction-formats.html) and core server [API](https://xrpl.org/api-conventions.html) ([`rippled`](https://github.com/ripple/rippled)) objects.\n\n\n\n```py\n# create a network client\nfrom xrpl.clients import JsonRpcClient\nclient = JsonRpcClient("https://s.altnet.rippletest.net:51234")\n\n# create a wallet on the testnet\nfrom xrpl.wallet import generate_faucet_wallet\ntest_wallet = generate_faucet_wallet(client)\nprint(test_wallet)\npublic_key: ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56\nprivate_key: -HIDDEN-\nclassic_address: rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo\n\n# look up account info\nfrom xrpl.models.requests.account_info import AccountInfo\nacct_info = AccountInfo(\n    account="rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",\n    ledger_index="current",\n    queue=True,\n    strict=True,\n)\nresponse = client.request(acct_info)\nresult = response.result\nimport json\nprint(json.dumps(result["account_data"], indent=4, sort_keys=True))\n# {\n#     "Account": "rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",\n#     "Balance": "1000000000",\n#     "Flags": 0,\n#     "LedgerEntryType": "AccountRoot",\n#     "OwnerCount": 0,\n#     "PreviousTxnID": "73CD4A37537A992270AAC8472F6681F44E400CBDE04EC8983C34B519F56AB107",\n#     "PreviousTxnLgrSeq": 16233962,\n#     "Sequence": 16233962,\n#     "index": "FD66EC588B52712DCE74831DCB08B24157DC3198C29A0116AA64D310A58512D7"\n# }\n```\n\n[![Downloads](https://pepy.tech/badge/xrpl-py/month)](https://pepy.tech/project/xrpl-py/month)\n[![Contributors](https://img.shields.io/github/contributors/xpring-eng/xrpl-py.svg)](https://github.com/xpring-eng/xrpl-py/graphs/contributors)\n\n## Installation and supported versions\n\nThe `xrpl-py` library is available on [PyPI](https://pypi.org/). Install with `pip`:\n\n\n```\npip3 install xrpl-py\n```\n\nThe library supports [Python 3.7](https://www.python.org/downloads/) and later.\n\n[![Supported Versions](https://img.shields.io/pypi/pyversions/xrpl-py.svg)](https://pypi.org/project/xrpl-py)\n\n\n## Features\n\nUse `xrpl-py` to build Python applications that leverage the [XRP Ledger](https://xrpl.org/). The library helps with all aspects of interacting with the XRP Ledger, including:\n\n* Key and wallet management\n* Serialization\n* Transaction Signing\n\n`xrpl-py` also provides:\n\n* A network client — See [`xrpl.clients`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.clients.html) for more information.\n* Methods for inspecting accounts — See [XRPL Account Methods](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.account.html) for more information.\n* Codecs for encoding and decoding addresses and other objects — See [Core Codecs](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.html) for more information.\n\n## [➡️ Reference Documentation](https://xrpl-py.readthedocs.io/en/stable/)\n\nSee the complete [`xrpl-py` reference documentation on Read the Docs](https://xrpl-py.readthedocs.io/en/stable/index.html).\n\n\n## Usage\n\nThe following sections describe some of the most commonly used modules in the `xrpl-py` library and provide sample code.\n\n### Network client\n\nUse the `xrpl.clients` library to create a network client for connecting to the XRP Ledger.\n\n```py\nfrom xrpl.clients import JsonRpcClient\nJSON_RPC_URL = "https://s.altnet.rippletest.net:51234"\nclient = JsonRpcClient(JSON_RPC_URL)\n```\n\n### Manage keys and wallets\n\n#### `xrpl.wallet`\n\nUse the [`xrpl.wallet`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.wallet.html) module to create a wallet from a given seed or or via a [Testnet faucet](https://xrpl.org/xrp-testnet-faucet.html).\n\nTo create a wallet from a seed (in this case, the value generated using [`xrpl.keypairs`](#xrpl-keypairs)):\n\n```py\nwallet_from_seed = xrpl.wallet.Wallet(seed, 0)\nprint(wallet_from_seed)\n# pub_key: ED46949E414A3D6D758D347BAEC9340DC78F7397FEE893132AAF5D56E4D7DE77B0\n# priv_key: -HIDDEN-\n# classic_address: rG5ZvYsK5BPi9f1Nb8mhFGDTNMJhEhufn6\n```\n\nTo create a wallet from a Testnet faucet:\n\n```py\ntest_wallet = generate_faucet_wallet(client)\ntest_account = test_wallet.classic_address\nprint("Classic address:", test_account)\n# Classic address: rEQB2hhp3rg7sHj6L8YyR4GG47Cb7pfcuw\n```\n\n#### `xrpl.core.keypairs`\n\nUse the [`xrpl.core.keypairs`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.keypairs.html#module-xrpl.core.keypairs) module to generate seeds and derive keypairs and addresses from those seed values.\n\nHere\'s an example of how to generate a `seed` value and derive an [XRP Ledger "classic" address](https://xrpl.org/cryptographic-keys.html#account-id-and-address) from that seed.\n\n\n```py\nfrom xrpl.core import keypairs\nseed = keypairs.generate_seed()\npublic, private = keypairs.derive_keypair(seed)\ntest_account = keypairs.derive_classic_address(public)\nprint("Here\'s the public key:")\nprint(public)\nprint("Here\'s the private key:")\nprint(private)\nprint("Store this in a secure place!")\n# Here\'s the public key:\n# ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56\n# Here\'s the private key:\n# EDE65EE7882847EF5345A43BFB8E6F5EEC60F45461696C384639B99B26AAA7A5CD\n# Store this in a secure place!\n```\n\n**Note:** You can use `xrpl.core.keypairs.sign` to sign transactions but `xrpl-py` also provides explicit methods for safely signing and submitting transactions. See [Transaction Signing](#transaction-signing) and [XRPL Transaction Methods](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#module-xrpl.transaction) for more information.\n\n\n### Serialize and sign transactions\n\nTo securely submit transactions to the XRP Ledger, you need to first serialize data from JSON and other formats into the [XRP Ledger\'s canonical format](https://xrpl.org/serialization.html), then to [authorize the transaction](https://xrpl.org/transaction-basics.html#authorizing-transactions) by digitally [signing it](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.keypairs.html?highlight=sign#xrpl.core.keypairs.sign) with the account\'s private key. The `xrpl-py` library provides several methods to simplify this process.\n\n\nUse the [`xrpl.transaction`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html) module to sign and submit transactions. The module offers three ways to do this:\n\n* [`sign_and_submit`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign_and_submit) — Signs a transaction locally, then submits it to the XRP Ledger. This method does not implement [reliable transaction submission](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission) best practices, so only use it for development or testing purposes.\n\n* [`sign`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign) — Signs a transaction locally. This method **does  not** submit the transaction to the XRP Ledger.\n\n* [`send_reliable_submission`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.send_reliable_submission) — An implementation of the [reliable transaction submission guidelines](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission), this method submits a signed transaction to the XRP Ledger and then verifies that it has been included in a validated ledger (or has failed to do so). Use this method to submit transactions for production purposes.\n\n\n```py\nfrom xrpl.models.transactions import Payment\nfrom xrpl.transaction import sign, send_reliable_submission\nfrom xrpl.ledger import get_latest_validated_ledger_sequence\nfrom xrpl.account import get_next_valid_seq_number\n\ncurrent_validated_ledger = get_latest_validated_ledger_sequence(client)\n\n# prepare the transaction\n# the amount is expressed in drops, not XRP\n# see https://xrpl.org/basic-data-types.html#specifying-currency-amounts\nmy_tx_payment = Payment(\n    account=test_wallet.classic_address,\n    amount="2200000",\n    destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",\n    last_ledger_sequence=current_validated_ledger + 20,\n    sequence=get_next_valid_seq_number(test_wallet.classic_address, client),\n    fee="10",\n)\n# sign the transaction\nmy_tx_payment_signed = sign(my_tx_payment,test_wallet)\n\n# submit the transaction\ntx_response = send_reliable_submission(my_tx_payment_signed, client)\n```\n\n#### Get fee from the XRP Ledger\n\n\nIn most cases, you can specify the minimum [transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) of `"10"` for the `fee` field unless you have a strong reason not to. But if you want to get the [current load-balanced transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) from the network, you can use the `get_fee` function:\n\n```py\nfrom xrpl.ledger import get_fee\nfee = get_fee(client)\nprint(fee)\n# 10\n```\n\n#### Auto-filled fields\n\nThe `xrpl-py` library automatically populates the `fee`, `sequence` and `last_ledger_sequence` fields when you create transactions. In the example above, you could omit those fields and let the library fill them in for you.\n\n```py\nfrom xrpl.models.transactions import Payment\nfrom xrpl.transaction import send_reliable_submission, autofill_and_sign\n# prepare the transaction\n# the amount is expressed in drops, not XRP\n# see https://xrpl.org/basic-data-types.html#specifying-currency-amounts\nmy_tx_payment = Payment(\n    account=test_wallet.classic_address,\n    amount="2200000",\n    destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe"\n)\n\n# sign the transaction with the autofill method\n# (this will auto-populate the fee, sequence, and last_ledger_sequence)\nmy_tx_payment_signed = autofill_and_sign(my_tx_payment, test_wallet, client)\nprint(my_tx_payment_signed)\n# Payment(\n#     account=\'rMPUKmzmDWEX1tQhzQ8oGFNfAEhnWNFwz\',\n#     transaction_type=<TransactionType.PAYMENT: \'Payment\'>,\n#     fee=\'10\',\n#     sequence=16034065,\n#     account_txn_id=None,\n#     flags=0,\n#     last_ledger_sequence=10268600,\n#     memos=None,\n#     signers=None,\n#     source_tag=None,\n#     signing_pub_key=\'EDD9540FA398915F0BCBD6E65579C03BE5424836CB68B7EB1D6573F2382156B444\',\n#     txn_signature=\'938FB22AE7FE76CF26FD11F8F97668E175DFAABD2977BCA397233117E7E1C4A1E39681091CC4D6DF21403682803AB54CC21DC4FA2F6848811DEE10FFEF74D809\',\n#     amount=\'2200000\',\n#     destination=\'rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe\',\n#     destination_tag=None,\n#     invoice_id=None,\n#     paths=None,\n#     send_max=None,\n#     deliver_min=None\n# )\n\n# submit the transaction\ntx_response = send_reliable_submission(my_tx_payment_signed, client)\n```\n\n\n### Subscribe to ledger updates\n\nYou can send `subscribe` and `unsubscribe` requests only using the WebSocket network client. These request methods allow you to be alerted of certain situations as they occur, such as when a new ledger is declared.\n\n```py\nfrom xrpl.clients import WebsocketClient\nurl = "wss://s.altnet.rippletest.net/"\nfrom xrpl.models.requests import Subscribe, StreamParameter\nreq = Subscribe(streams=[StreamParameter.LEDGER])\n# NOTE: this code will run forever without a timeout, until the process is killed\nwith WebsocketClient(url) as client:\n    client.send(req)\n    for message in client:\n        print(message)\n# {\'result\': {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'7CD50477F23FF158B430772D8E82A961376A7B40E13C695AA849811EDF66C5C0\', \'ledger_index\': 18183504, \'ledger_time\': 676412962, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'validated_ledgers\': \'17469391-18183504\'}, \'status\': \'success\', \'type\': \'response\'}\n# {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'BAA743DABD168BD434804416C8087B7BDEF7E6D7EAD412B9102281DD83B10D00\', \'ledger_index\': 18183505, \'ledger_time\': 676412970, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'txn_count\': 0, \'type\': \'ledgerClosed\', \'validated_ledgers\': \'17469391-18183505\'}\n# {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'D8227DAF8F745AE3F907B251D40B4081E019D013ABC23B68C0B1431DBADA1A46\', \'ledger_index\': 18183506, \'ledger_time\': 676412971, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'txn_count\': 0, \'type\': \'ledgerClosed\', \'validated_ledgers\': \'17469391-18183506\'}\n# {\'fee_base\': 10, \'fee_ref\': 10, \'ledger_hash\': \'CFC412B6DDB9A402662832A781C23F0F2E842EAE6CFC539FEEB287318092C0DE\', \'ledger_index\': 18183507, \'ledger_time\': 676412972, \'reserve_base\': 20000000, \'reserve_inc\': 5000000, \'txn_count\': 0, \'type\': \'ledgerClosed\', \'validated_ledgers\': \'17469391-18183507\'}\n```\n\n\n### Asynchronous Code\n\nThis library supports Python\'s [`asyncio`](https://docs.python.org/3/library/asyncio.html) package, which is used to run asynchronous code. All the async code is in [`xrpl.asyncio`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.asyncio.html) If you are writing asynchronous code, please note that you will not be able to use any synchronous sugar functions, due to how event loops are handled. However, every synchronous method has a corresponding asynchronous method that you can use.\n\nThis sample code is the asynchronous equivalent of the above section on submitting a transaction.\n\n```py\nimport asyncio\nfrom xrpl.models.transactions import Payment\nfrom xrpl.asyncio.transaction import sign, send_reliable_submission\nfrom xrpl.asyncio.ledger import get_latest_validated_ledger_sequence\nfrom xrpl.asyncio.account import get_next_valid_seq_number\nfrom xrpl.asyncio.clients import AsyncJsonRpcClient\n\nasync_client = AsyncJsonRpcClient(JSON_RPC_URL)\n\nasync def submit_sample_transaction():\n    current_validated_ledger = await get_latest_validated_ledger_sequence(async_client)\n\n    # prepare the transaction\n    # the amount is expressed in drops, not XRP\n    # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts\n    my_tx_payment = Payment(\n        account=test_wallet.classic_address,\n        amount="2200000",\n        destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",\n        last_ledger_sequence=current_validated_ledger + 20,\n        sequence=await get_next_valid_seq_number(test_wallet.classic_address, async_client),\n        fee="10",\n    )\n    # sign the transaction\n    my_tx_payment_signed = await sign(my_tx_payment,test_wallet)\n\n    # submit the transaction\n    tx_response = await send_reliable_submission(my_tx_payment_signed, async_client)\n\nasyncio.run(submit_sample_transaction())\n```\n\n### Encode addresses\n\nUse [`xrpl.core.addresscodec`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.addresscodec.html) to encode and decode addresses into and from the ["classic" and X-address formats](https://xrpl.org/accounts.html#addresses).\n\n```py\n# convert classic address to x-address\nfrom xrpl.core import addresscodec\ntestnet_xaddress = (\n    addresscodec.classic_address_to_xaddress(\n        "rMPUKmzmDWEX1tQhzQ8oGFNfAEhnWNFwz",\n        tag=0,\n        is_test_network=True,\n    )\n)\nprint(testnet_xaddress)\n# T7QDemmxnuN7a52A62nx2fxGPWcRahLCf3qaswfrsNW9Lps\n```\n\n\n## Contributing\n\nIf you want to contribute to this project, see [CONTRIBUTING.md].\n\n### Mailing Lists\n\nWe have a low-traffic mailing list for announcements of new `xrpl.js` releases. (About 1 email per week)\n\n+ [Subscribe to xrpl-announce](https://groups.google.com/g/xrpl-announce)\n\nIf you\'re using the XRP Ledger in production, you should run a [rippled server](https://github.com/ripple/rippled) and subscribe to the ripple-server mailing list as well.\n\n+ [Subscribe to ripple-server](https://groups.google.com/g/ripple-server)\n\n### Report an issue\n\nExperienced an issue? Report it [here](https://github.com/XRPLF/xrpl-py/issues/new).\n\n## License\n\nThe `xrpl-py` library is licensed under the ISC License. See [LICENSE] for more information.\n\n\n\n[CONTRIBUTING.md]: CONTRIBUTING.md\n[LICENSE]: LICENSE\n',
     'author': 'Mayukha Vadari',
     'author_email': 'mvadari@ripple.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/XRPLF/xrpl-py',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `xrpl-py-1.9.0b0/PKG-INFO` & `xrpl-py-2.0.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrpl-py
-Version: 1.9.0b0
+Version: 2.0.0b0
 Summary: A complete Python library for interacting with the XRP ledger
 Home-page: https://github.com/XRPLF/xrpl-py
 License: ISC
 Keywords: xrp,xrpl,cryptocurrency
 Author: Mayukha Vadari
 Author-email: mvadari@ripple.com
 Requires-Python: >=3.7,<4.0
@@ -192,25 +192,24 @@
 ```py
 from xrpl.models.transactions import Payment
 from xrpl.transaction import sign, send_reliable_submission
 from xrpl.ledger import get_latest_validated_ledger_sequence
 from xrpl.account import get_next_valid_seq_number
 
 current_validated_ledger = get_latest_validated_ledger_sequence(client)
-test_wallet.sequence = get_next_valid_seq_number(test_wallet.classic_address, client)
 
 # prepare the transaction
 # the amount is expressed in drops, not XRP
 # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
 my_tx_payment = Payment(
     account=test_wallet.classic_address,
     amount="2200000",
     destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",
     last_ledger_sequence=current_validated_ledger + 20,
-    sequence=test_wallet.sequence,
+    sequence=get_next_valid_seq_number(test_wallet.classic_address, client),
     fee="10",
 )
 # sign the transaction
 my_tx_payment_signed = sign(my_tx_payment,test_wallet)
 
 # submit the transaction
 tx_response = send_reliable_submission(my_tx_payment_signed, client)
@@ -310,25 +309,24 @@
 from xrpl.asyncio.account import get_next_valid_seq_number
 from xrpl.asyncio.clients import AsyncJsonRpcClient
 
 async_client = AsyncJsonRpcClient(JSON_RPC_URL)
 
 async def submit_sample_transaction():
     current_validated_ledger = await get_latest_validated_ledger_sequence(async_client)
-    test_wallet.sequence = await get_next_valid_seq_number(test_wallet.classic_address, async_client)
 
     # prepare the transaction
     # the amount is expressed in drops, not XRP
     # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
     my_tx_payment = Payment(
         account=test_wallet.classic_address,
         amount="2200000",
         destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",
         last_ledger_sequence=current_validated_ledger + 20,
-        sequence=test_wallet.sequence,
+        sequence=await get_next_valid_seq_number(test_wallet.classic_address, async_client),
         fee="10",
     )
     # sign the transaction
     my_tx_payment_signed = await sign(my_tx_payment,test_wallet)
 
     # submit the transaction
     tx_response = await send_reliable_submission(my_tx_payment_signed, async_client)
```

