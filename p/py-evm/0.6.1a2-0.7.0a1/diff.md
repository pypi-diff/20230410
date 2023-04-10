# Comparing `tmp/py-evm-0.6.1a2.tar.gz` & `tmp/py-evm-0.7.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-evm-0.6.1a2.tar", last modified: Fri Dec 16 17:41:29 2022, max compression
+gzip compressed data, was "py-evm-0.7.0a1.tar", last modified: Mon Apr 10 16:50:19 2023, max compression
```

## Comparing `py-evm-0.6.1a2.tar` & `py-evm-0.7.0a1.tar`

### file list

```diff
@@ -1,325 +1,337 @@
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.088637 py-evm-0.6.1a2/
--rw-r--r--   0 eve        (501) staff       (20)     1087 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/LICENSE
--rw-r--r--   0 eve        (501) staff       (20)      137 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/MANIFEST.in
--rw-r--r--   0 eve        (501) staff       (20)     2673 2022-12-16 17:41:29.088437 py-evm-0.6.1a2/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     1854 2021-11-05 20:04:27.000000 py-evm-0.6.1a2/README.md
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.060377 py-evm-0.6.1a2/eth/
--rw-r--r--   0 eve        (501) staff       (20)      368 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.062338 py-evm-0.6.1a2/eth/_utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/_utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      734 2022-12-07 18:37:56.000000 py-evm-0.6.1a2/eth/_utils/address.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.062724 py-evm-0.6.1a2/eth/_utils/blake2/
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-12-07 18:37:56.000000 py-evm-0.6.1a2/eth/_utils/blake2/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1791 2021-03-31 17:31:28.000000 py-evm-0.6.1a2/eth/_utils/blake2/coders.py
--rwxr-xr-x   0 eve        (501) staff       (20)     5784 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/_utils/blake2/compression.py
--rw-r--r--   0 eve        (501) staff       (20)      972 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/_utils/bn128.py
--rw-r--r--   0 eve        (501) staff       (20)     3900 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/_utils/datatypes.py
--rw-r--r--   0 eve        (501) staff       (20)     1001 2022-12-07 18:37:56.000000 py-evm-0.6.1a2/eth/_utils/db.py
--rw-r--r--   0 eve        (501) staff       (20)       40 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/_utils/empty.py
--rw-r--r--   0 eve        (501) staff       (20)     8214 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/_utils/env.py
--rw-r--r--   0 eve        (501) staff       (20)      613 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/_utils/generator.py
--rw-r--r--   0 eve        (501) staff       (20)     5037 2022-09-19 18:10:36.000000 py-evm-0.6.1a2/eth/_utils/headers.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2022-12-07 18:37:56.000000 py-evm-0.6.1a2/eth/_utils/logging.py
--rw-r--r--   0 eve        (501) staff       (20)     1532 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/_utils/module_loading.py
--rw-r--r--   0 eve        (501) staff       (20)     2801 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/_utils/numeric.py
--rw-r--r--   0 eve        (501) staff       (20)      338 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/_utils/padding.py
--rw-r--r--   0 eve        (501) staff       (20)     3338 2021-11-05 20:04:27.000000 py-evm-0.6.1a2/eth/_utils/rlp.py
--rw-r--r--   0 eve        (501) staff       (20)     1739 2022-12-07 18:37:56.000000 py-evm-0.6.1a2/eth/_utils/spoof.py
--rw-r--r--   0 eve        (501) staff       (20)     1352 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/_utils/state.py
--rw-r--r--   0 eve        (501) staff       (20)     3409 2021-03-31 17:31:28.000000 py-evm-0.6.1a2/eth/_utils/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)      376 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/_utils/version.py
--rw-r--r--   0 eve        (501) staff       (20)      346 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/_warnings.py
--rw-r--r--   0 eve        (501) staff       (20)   115671 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/abc.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.063068 py-evm-0.6.1a2/eth/chains/
--rw-r--r--   0 eve        (501) staff       (20)      223 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/chains/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    25615 2022-09-19 18:10:36.000000 py-evm-0.6.1a2/eth/chains/base.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.063341 py-evm-0.6.1a2/eth/chains/goerli/
--rw-r--r--   0 eve        (501) staff       (20)     1277 2021-03-31 17:31:28.000000 py-evm-0.6.1a2/eth/chains/goerli/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      262 2021-03-31 17:31:28.000000 py-evm-0.6.1a2/eth/chains/goerli/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     2599 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/chains/header.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.063670 py-evm-0.6.1a2/eth/chains/mainnet/
--rw-r--r--   0 eve        (501) staff       (20)     4485 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/chains/mainnet/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1191 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/chains/mainnet/constants.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.063884 py-evm-0.6.1a2/eth/chains/ropsten/
--rw-r--r--   0 eve        (501) staff       (20)     2105 2021-03-31 17:31:28.000000 py-evm-0.6.1a2/eth/chains/ropsten/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      839 2021-03-31 17:31:28.000000 py-evm-0.6.1a2/eth/chains/ropsten/constants.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.063981 py-evm-0.6.1a2/eth/chains/tester/
--rw-r--r--   0 eve        (501) staff       (20)     5965 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/chains/tester/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.064575 py-evm-0.6.1a2/eth/consensus/
--rw-r--r--   0 eve        (501) staff       (20)      313 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/consensus/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      956 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/consensus/applier.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.065326 py-evm-0.6.1a2/eth/consensus/clique/
--rw-r--r--   0 eve        (501) staff       (20)      270 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/consensus/clique/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     5106 2021-08-19 20:42:01.000000 py-evm-0.6.1a2/eth/consensus/clique/_utils.py
--rw-r--r--   0 eve        (501) staff       (20)     5468 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/consensus/clique/clique.py
--rw-r--r--   0 eve        (501) staff       (20)      477 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/consensus/clique/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     3380 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/consensus/clique/datatypes.py
--rw-r--r--   0 eve        (501) staff       (20)     2929 2021-03-31 17:31:28.000000 py-evm-0.6.1a2/eth/consensus/clique/encoding.py
--rw-r--r--   0 eve        (501) staff       (20)      149 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/consensus/clique/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)    11037 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/consensus/clique/snapshot_manager.py
--rw-r--r--   0 eve        (501) staff       (20)      188 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/consensus/context.py
--rw-r--r--   0 eve        (501) staff       (20)      732 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/consensus/noproof.py
--rw-r--r--   0 eve        (501) staff       (20)      834 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/consensus/pos.py
--rw-r--r--   0 eve        (501) staff       (20)     4037 2022-08-17 18:04:11.000000 py-evm-0.6.1a2/eth/consensus/pow.py
--rw-r--r--   0 eve        (501) staff       (20)     3853 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/constants.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.067133 py-evm-0.6.1a2/eth/db/
--rw-r--r--   0 eve        (501) staff       (20)      746 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     3434 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/accesslog.py
--rw-r--r--   0 eve        (501) staff       (20)    24116 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/db/account.py
--rw-r--r--   0 eve        (501) staff       (20)     4172 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/atomic.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.067475 py-evm-0.6.1a2/eth/db/backends/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/backends/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2494 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/backends/base.py
--rw-r--r--   0 eve        (501) staff       (20)     4410 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/backends/level.py
--rw-r--r--   0 eve        (501) staff       (20)      890 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/backends/memory.py
--rw-r--r--   0 eve        (501) staff       (20)     2811 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/batch.py
--rw-r--r--   0 eve        (501) staff       (20)      943 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/cache.py
--rw-r--r--   0 eve        (501) staff       (20)    17426 2022-09-19 18:10:36.000000 py-evm-0.6.1a2/eth/db/chain.py
--rw-r--r--   0 eve        (501) staff       (20)     5524 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/chain_gaps.py
--rw-r--r--   0 eve        (501) staff       (20)     7303 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/diff.py
--rw-r--r--   0 eve        (501) staff       (20)      488 2021-08-19 20:42:01.000000 py-evm-0.6.1a2/eth/db/hash_trie.py
--rw-r--r--   0 eve        (501) staff       (20)    24092 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/db/header.py
--rw-r--r--   0 eve        (501) staff       (20)    16683 2021-03-10 18:54:42.000000 py-evm-0.6.1a2/eth/db/journal.py
--rw-r--r--   0 eve        (501) staff       (20)     1291 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/keymap.py
--rw-r--r--   0 eve        (501) staff       (20)     1178 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/schema.py
--rw-r--r--   0 eve        (501) staff       (20)    16275 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/slow_journal.py
--rw-r--r--   0 eve        (501) staff       (20)    16229 2021-03-04 23:10:51.000000 py-evm-0.6.1a2/eth/db/storage.py
--rw-r--r--   0 eve        (501) staff       (20)     1331 2021-03-10 18:54:47.000000 py-evm-0.6.1a2/eth/db/trie.py
--rw-r--r--   0 eve        (501) staff       (20)     1667 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/db/witness.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.067667 py-evm-0.6.1a2/eth/estimators/
--rw-r--r--   0 eve        (501) staff       (20)      522 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/estimators/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     3285 2021-08-19 20:42:40.000000 py-evm-0.6.1a2/eth/estimators/gas.py
--rw-r--r--   0 eve        (501) staff       (20)     4076 2021-11-05 20:04:27.000000 py-evm-0.6.1a2/eth/exceptions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.068944 py-evm-0.6.1a2/eth/precompiles/
--rw-r--r--   0 eve        (501) staff       (20)      398 2021-02-26 19:54:17.000000 py-evm-0.6.1a2/eth/precompiles/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      919 2021-09-03 20:35:50.000000 py-evm-0.6.1a2/eth/precompiles/blake2.py
--rw-r--r--   0 eve        (501) staff       (20)     1487 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/precompiles/ecadd.py
--rw-r--r--   0 eve        (501) staff       (20)     1375 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/precompiles/ecmul.py
--rw-r--r--   0 eve        (501) staff       (20)     3261 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/precompiles/ecpairing.py
--rw-r--r--   0 eve        (501) staff       (20)     1511 2021-11-05 20:04:27.000000 py-evm-0.6.1a2/eth/precompiles/ecrecover.py
--rw-r--r--   0 eve        (501) staff       (20)      478 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/precompiles/identity.py
--rw-r--r--   0 eve        (501) staff       (20)     4026 2021-03-31 17:31:28.000000 py-evm-0.6.1a2/eth/precompiles/modexp.py
--rw-r--r--   0 eve        (501) staff       (20)      676 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/precompiles/ripemd160.py
--rw-r--r--   0 eve        (501) staff       (20)      548 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/precompiles/sha256.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/py.typed
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.069858 py-evm-0.6.1a2/eth/rlp/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/rlp/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1032 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/rlp/accounts.py
--rw-r--r--   0 eve        (501) staff       (20)      904 2021-03-01 17:34:33.000000 py-evm-0.6.1a2/eth/rlp/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     5423 2021-08-19 20:47:44.000000 py-evm-0.6.1a2/eth/rlp/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      669 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/rlp/logs.py
--rw-r--r--   0 eve        (501) staff       (20)     1312 2021-03-10 18:54:47.000000 py-evm-0.6.1a2/eth/rlp/receipts.py
--rw-r--r--   0 eve        (501) staff       (20)      370 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/rlp/sedes.py
--rw-r--r--   0 eve        (501) staff       (20)     3595 2021-08-19 20:42:01.000000 py-evm-0.6.1a2/eth/rlp/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.070107 py-evm-0.6.1a2/eth/tools/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.070876 py-evm-0.6.1a2/eth/tools/_utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/_utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      181 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/_utils/git.py
--rw-r--r--   0 eve        (501) staff       (20)      532 2021-08-19 20:42:01.000000 py-evm-0.6.1a2/eth/tools/_utils/hashing.py
--rw-r--r--   0 eve        (501) staff       (20)     1486 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/_utils/mappings.py
--rw-r--r--   0 eve        (501) staff       (20)    17880 2022-08-31 18:17:44.000000 py-evm-0.6.1a2/eth/tools/_utils/normalization.py
--rw-r--r--   0 eve        (501) staff       (20)     4314 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/_utils/slow_code_stream.py
--rw-r--r--   0 eve        (501) staff       (20)      886 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/_utils/vyper.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.070971 py-evm-0.6.1a2/eth/tools/builder/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/builder/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.071138 py-evm-0.6.1a2/eth/tools/builder/chain/
--rw-r--r--   0 eve        (501) staff       (20)     2858 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/tools/builder/chain/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    15160 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/tools/builder/chain/builders.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.071481 py-evm-0.6.1a2/eth/tools/db/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/db/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     5130 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/db/atomic.py
--rw-r--r--   0 eve        (501) staff       (20)     2260 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/db/base.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.072039 py-evm-0.6.1a2/eth/tools/fixtures/
--rw-r--r--   0 eve        (501) staff       (20)      615 2021-08-19 20:42:01.000000 py-evm-0.6.1a2/eth/tools/fixtures/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      878 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/fixtures/_utils.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.072792 py-evm-0.6.1a2/eth/tools/fixtures/fillers/
--rw-r--r--   0 eve        (501) staff       (20)      282 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/fixtures/fillers/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2461 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/fixtures/fillers/_utils.py
--rw-r--r--   0 eve        (501) staff       (20)    12490 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/fixtures/fillers/common.py
--rw-r--r--   0 eve        (501) staff       (20)     3108 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/fixtures/fillers/formatters.py
--rw-r--r--   0 eve        (501) staff       (20)     1305 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/fixtures/fillers/main.py
--rw-r--r--   0 eve        (501) staff       (20)     2617 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/fixtures/fillers/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1747 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/fixtures/fillers/vm.py
--rw-r--r--   0 eve        (501) staff       (20)     2136 2021-11-05 22:07:56.000000 py-evm-0.6.1a2/eth/tools/fixtures/generation.py
--rw-r--r--   0 eve        (501) staff       (20)     9320 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/tools/fixtures/helpers.py
--rw-r--r--   0 eve        (501) staff       (20)     3140 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/tools/fixtures/loading.py
--rw-r--r--   0 eve        (501) staff       (20)      759 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/tools/mining.py
--rw-r--r--   0 eve        (501) staff       (20)      449 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/tools/rlp.py
--rw-r--r--   0 eve        (501) staff       (20)     2790 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/typing.py
--rw-r--r--   0 eve        (501) staff       (20)     8852 2022-09-12 22:16:17.000000 py-evm-0.6.1a2/eth/validation.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.074993 py-evm-0.6.1a2/eth/vm/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    24957 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/base.py
--rw-r--r--   0 eve        (501) staff       (20)      615 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/chain_context.py
--rw-r--r--   0 eve        (501) staff       (20)     4247 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/code_stream.py
--rw-r--r--   0 eve        (501) staff       (20)    17531 2021-09-10 22:12:20.000000 py-evm-0.6.1a2/eth/vm/computation.py
--rw-r--r--   0 eve        (501) staff       (20)     2086 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/execution_context.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.075102 py-evm-0.6.1a2/eth/vm/forks/
--rw-r--r--   0 eve        (501) staff       (20)      843 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.075777 py-evm-0.6.1a2/eth/vm/forks/arrow_glacier/
--rw-r--r--   0 eve        (501) staff       (20)      856 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/arrow_glacier/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      951 2022-06-23 20:10:28.000000 py-evm-0.6.1a2/eth/vm/forks/arrow_glacier/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      267 2021-12-15 20:27:15.000000 py-evm-0.6.1a2/eth/vm/forks/arrow_glacier/computation.py
--rw-r--r--   0 eve        (501) staff       (20)     1074 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/arrow_glacier/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      463 2021-12-15 20:27:15.000000 py-evm-0.6.1a2/eth/vm/forks/arrow_glacier/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1132 2021-12-15 20:27:15.000000 py-evm-0.6.1a2/eth/vm/forks/arrow_glacier/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.076810 py-evm-0.6.1a2/eth/vm/forks/berlin/
--rw-r--r--   0 eve        (501) staff       (20)      760 2021-09-20 20:47:49.000000 py-evm-0.6.1a2/eth/vm/forks/berlin/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      760 2021-03-10 18:54:47.000000 py-evm-0.6.1a2/eth/vm/forks/berlin/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     2402 2021-03-31 17:31:28.000000 py-evm-0.6.1a2/eth/vm/forks/berlin/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      327 2021-08-30 21:22:29.000000 py-evm-0.6.1a2/eth/vm/forks/berlin/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      367 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/berlin/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     6462 2021-09-10 18:06:54.000000 py-evm-0.6.1a2/eth/vm/forks/berlin/logic.py
--rw-r--r--   0 eve        (501) staff       (20)     2888 2021-03-17 17:52:03.000000 py-evm-0.6.1a2/eth/vm/forks/berlin/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)     4521 2021-08-30 17:37:29.000000 py-evm-0.6.1a2/eth/vm/forks/berlin/receipts.py
--rw-r--r--   0 eve        (501) staff       (20)     1192 2021-03-17 17:52:03.000000 py-evm-0.6.1a2/eth/vm/forks/berlin/state.py
--rw-r--r--   0 eve        (501) staff       (20)    15608 2021-11-05 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/berlin/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.077686 py-evm-0.6.1a2/eth/vm/forks/byzantium/
--rw-r--r--   0 eve        (501) staff       (20)     3585 2021-09-20 20:47:49.000000 py-evm-0.6.1a2/eth/vm/forks/byzantium/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      483 2021-03-01 17:34:33.000000 py-evm-0.6.1a2/eth/vm/forks/byzantium/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      965 2021-02-26 17:26:20.000000 py-evm-0.6.1a2/eth/vm/forks/byzantium/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      226 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/byzantium/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     3483 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/byzantium/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     3499 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/byzantium/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      204 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/byzantium/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1442 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/byzantium/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.078647 py-evm-0.6.1a2/eth/vm/forks/constantinople/
--rw-r--r--   0 eve        (501) staff       (20)     1108 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/constantinople/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      482 2021-03-01 17:34:33.000000 py-evm-0.6.1a2/eth/vm/forks/constantinople/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      809 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/constantinople/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      321 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/constantinople/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      387 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/constantinople/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     1569 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/constantinople/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      211 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/constantinople/state.py
--rw-r--r--   0 eve        (501) staff       (20)      325 2021-03-17 17:52:03.000000 py-evm-0.6.1a2/eth/vm/forks/constantinople/storage.py
--rw-r--r--   0 eve        (501) staff       (20)     1446 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/constantinople/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.079596 py-evm-0.6.1a2/eth/vm/forks/frontier/
--rw-r--r--   0 eve        (501) staff       (20)     3820 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/frontier/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     3318 2021-08-19 20:42:40.000000 py-evm-0.6.1a2/eth/vm/forks/frontier/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     3706 2021-09-10 18:42:40.000000 py-evm-0.6.1a2/eth/vm/forks/frontier/computation.py
--rw-r--r--   0 eve        (501) staff       (20)       96 2021-09-20 20:47:49.000000 py-evm-0.6.1a2/eth/vm/forks/frontier/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     3546 2021-08-19 20:42:40.000000 py-evm-0.6.1a2/eth/vm/forks/frontier/headers.py
--rw-r--r--   0 eve        (501) staff       (20)    20208 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/frontier/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)     7722 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/frontier/state.py
--rw-r--r--   0 eve        (501) staff       (20)      131 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/frontier/transaction_context.py
--rw-r--r--   0 eve        (501) staff       (20)     6040 2021-08-19 20:42:01.000000 py-evm-0.6.1a2/eth/vm/forks/frontier/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)     1698 2021-08-19 20:42:01.000000 py-evm-0.6.1a2/eth/vm/forks/frontier/validation.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.080124 py-evm-0.6.1a2/eth/vm/forks/gray_glacier/
--rw-r--r--   0 eve        (501) staff       (20)      855 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/gray_glacier/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1017 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/gray_glacier/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      297 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/gray_glacier/computation.py
--rw-r--r--   0 eve        (501) staff       (20)     1118 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/gray_glacier/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      496 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/gray_glacier/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1168 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/gray_glacier/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.080895 py-evm-0.6.1a2/eth/vm/forks/homestead/
--rw-r--r--   0 eve        (501) staff       (20)     1210 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/homestead/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      463 2021-03-01 17:34:33.000000 py-evm-0.6.1a2/eth/vm/forks/homestead/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     2261 2021-03-05 23:32:34.000000 py-evm-0.6.1a2/eth/vm/forks/homestead/computation.py
--rw-r--r--   0 eve        (501) staff       (20)       61 2021-09-03 20:35:50.000000 py-evm-0.6.1a2/eth/vm/forks/homestead/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     9661 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/homestead/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      603 2021-03-05 23:31:28.000000 py-evm-0.6.1a2/eth/vm/forks/homestead/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      613 2021-03-05 23:32:34.000000 py-evm-0.6.1a2/eth/vm/forks/homestead/state.py
--rw-r--r--   0 eve        (501) staff       (20)     2292 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/homestead/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)      548 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/homestead/validation.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.081689 py-evm-0.6.1a2/eth/vm/forks/istanbul/
--rw-r--r--   0 eve        (501) staff       (20)      805 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/istanbul/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      467 2021-03-01 17:34:33.000000 py-evm-0.6.1a2/eth/vm/forks/istanbul/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     1466 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/istanbul/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      316 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/istanbul/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      371 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/istanbul/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     1637 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/istanbul/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      196 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/istanbul/state.py
--rw-r--r--   0 eve        (501) staff       (20)      883 2021-09-02 18:17:22.000000 py-evm-0.6.1a2/eth/vm/forks/istanbul/storage.py
--rw-r--r--   0 eve        (501) staff       (20)     2000 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/istanbul/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.082691 py-evm-0.6.1a2/eth/vm/forks/london/
--rw-r--r--   0 eve        (501) staff       (20)     2286 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/london/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     5671 2021-08-30 17:37:29.000000 py-evm-0.6.1a2/eth/vm/forks/london/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      772 2021-09-20 20:47:49.000000 py-evm-0.6.1a2/eth/vm/forks/london/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      470 2021-09-20 20:47:49.000000 py-evm-0.6.1a2/eth/vm/forks/london/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     5573 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/london/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      860 2021-09-20 20:47:49.000000 py-evm-0.6.1a2/eth/vm/forks/london/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      620 2021-08-30 17:37:29.000000 py-evm-0.6.1a2/eth/vm/forks/london/receipts.py
--rw-r--r--   0 eve        (501) staff       (20)     4940 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/london/state.py
--rw-r--r--   0 eve        (501) staff       (20)      527 2021-09-20 20:47:49.000000 py-evm-0.6.1a2/eth/vm/forks/london/storage.py
--rw-r--r--   0 eve        (501) staff       (20)     9548 2021-11-05 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/london/transactions.py
--rw-r--r--   0 eve        (501) staff       (20)      845 2021-08-19 20:42:40.000000 py-evm-0.6.1a2/eth/vm/forks/london/validation.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.083312 py-evm-0.6.1a2/eth/vm/forks/muir_glacier/
--rw-r--r--   0 eve        (501) staff       (20)      830 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/muir_glacier/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      470 2021-03-01 17:34:33.000000 py-evm-0.6.1a2/eth/vm/forks/muir_glacier/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      562 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/muir_glacier/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      424 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/muir_glacier/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      137 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/muir_glacier/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      199 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/muir_glacier/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1423 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/muir_glacier/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.083939 py-evm-0.6.1a2/eth/vm/forks/paris/
--rw-r--r--   0 eve        (501) staff       (20)     2109 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/paris/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     1014 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/paris/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      375 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/paris/computation.py
--rw-r--r--   0 eve        (501) staff       (20)     2323 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/paris/headers.py
--rw-r--r--   0 eve        (501) staff       (20)      649 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/paris/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      619 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/paris/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1119 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/paris/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.084652 py-evm-0.6.1a2/eth/vm/forks/petersburg/
--rw-r--r--   0 eve        (501) staff       (20)     1024 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/petersburg/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      470 2021-03-01 17:34:33.000000 py-evm-0.6.1a2/eth/vm/forks/petersburg/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)      556 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/petersburg/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      102 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/petersburg/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      367 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/petersburg/headers.py
--rw-r--r--   0 eve        (501) staff       (20)     1378 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/petersburg/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      199 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/petersburg/state.py
--rw-r--r--   0 eve        (501) staff       (20)     1422 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/petersburg/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.085427 py-evm-0.6.1a2/eth/vm/forks/spurious_dragon/
--rw-r--r--   0 eve        (501) staff       (20)      429 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/spurious_dragon/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2124 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/forks/spurious_dragon/_utils.py
--rw-r--r--   0 eve        (501) staff       (20)      481 2021-03-01 17:34:33.000000 py-evm-0.6.1a2/eth/vm/forks/spurious_dragon/blocks.py
--rw-r--r--   0 eve        (501) staff       (20)     2937 2021-09-20 20:47:49.000000 py-evm-0.6.1a2/eth/vm/forks/spurious_dragon/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      169 2021-09-03 20:35:50.000000 py-evm-0.6.1a2/eth/vm/forks/spurious_dragon/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     1180 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/spurious_dragon/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)     1486 2021-09-03 22:22:38.000000 py-evm-0.6.1a2/eth/vm/forks/spurious_dragon/state.py
--rw-r--r--   0 eve        (501) staff       (20)     2950 2021-03-10 18:54:47.000000 py-evm-0.6.1a2/eth/vm/forks/spurious_dragon/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.085943 py-evm-0.6.1a2/eth/vm/forks/tangerine_whistle/
--rw-r--r--   0 eve        (501) staff       (20)      469 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/tangerine_whistle/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      396 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/tangerine_whistle/computation.py
--rw-r--r--   0 eve        (501) staff       (20)      225 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/tangerine_whistle/constants.py
--rw-r--r--   0 eve        (501) staff       (20)     2067 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/tangerine_whistle/opcodes.py
--rw-r--r--   0 eve        (501) staff       (20)      209 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/forks/tangerine_whistle/state.py
--rw-r--r--   0 eve        (501) staff       (20)     2637 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/gas_meter.py
--rw-r--r--   0 eve        (501) staff       (20)      525 2022-09-12 22:16:17.000000 py-evm-0.6.1a2/eth/vm/header.py
--rw-r--r--   0 eve        (501) staff       (20)     3414 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/interrupt.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.087437 py-evm-0.6.1a2/eth/vm/logic/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/logic/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     4819 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/logic/arithmetic.py
--rw-r--r--   0 eve        (501) staff       (20)     1066 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/logic/block.py
--rw-r--r--   0 eve        (501) staff       (20)    14298 2021-03-17 17:52:03.000000 py-evm-0.6.1a2/eth/vm/logic/call.py
--rw-r--r--   0 eve        (501) staff       (20)     2831 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/logic/comparison.py
--rw-r--r--   0 eve        (501) staff       (20)     6448 2021-03-17 17:52:03.000000 py-evm-0.6.1a2/eth/vm/logic/context.py
--rw-r--r--   0 eve        (501) staff       (20)      948 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/logic/duplication.py
--rw-r--r--   0 eve        (501) staff       (20)     1518 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/logic/flow.py
--rw-r--r--   0 eve        (501) staff       (20)      480 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/logic/invalid.py
--rw-r--r--   0 eve        (501) staff       (20)     1342 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/logic/logging.py
--rw-r--r--   0 eve        (501) staff       (20)     1109 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/logic/memory.py
--rw-r--r--   0 eve        (501) staff       (20)      626 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/logic/sha3.py
--rw-r--r--   0 eve        (501) staff       (20)     2138 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/logic/stack.py
--rw-r--r--   0 eve        (501) staff       (20)     3921 2021-09-10 18:08:36.000000 py-evm-0.6.1a2/eth/vm/logic/storage.py
--rw-r--r--   0 eve        (501) staff       (20)      978 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/logic/swap.py
--rw-r--r--   0 eve        (501) staff       (20)     9441 2021-11-05 20:04:27.000000 py-evm-0.6.1a2/eth/vm/logic/system.py
--rw-r--r--   0 eve        (501) staff       (20)     2122 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/memory.py
--rw-r--r--   0 eve        (501) staff       (20)     3177 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/message.py
--rw-r--r--   0 eve        (501) staff       (20)     2769 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/mnemonics.py
--rw-r--r--   0 eve        (501) staff       (20)     1895 2021-08-30 21:41:40.000000 py-evm-0.6.1a2/eth/vm/opcode.py
--rw-r--r--   0 eve        (501) staff       (20)     2417 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/opcode_values.py
--rw-r--r--   0 eve        (501) staff       (20)      385 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/spoof.py
--rw-r--r--   0 eve        (501) staff       (20)     7675 2021-03-17 17:52:03.000000 py-evm-0.6.1a2/eth/vm/stack.py
--rw-r--r--   0 eve        (501) staff       (20)    10026 2022-12-09 20:04:27.000000 py-evm-0.6.1a2/eth/vm/state.py
--rw-r--r--   0 eve        (501) staff       (20)      857 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/eth/vm/transaction_context.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2022-12-16 17:41:29.088220 py-evm-0.6.1a2/py_evm.egg-info/
--rw-r--r--   0 eve        (501) staff       (20)     2673 2022-12-16 17:41:29.000000 py-evm-0.6.1a2/py_evm.egg-info/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     8112 2022-12-16 17:41:29.000000 py-evm-0.6.1a2/py_evm.egg-info/SOURCES.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2022-12-16 17:41:29.000000 py-evm-0.6.1a2/py_evm.egg-info/dependency_links.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2021-02-24 18:15:32.000000 py-evm-0.6.1a2/py_evm.egg-info/not-zip-safe
--rw-r--r--   0 eve        (501) staff       (20)     2057 2022-12-16 17:41:29.000000 py-evm-0.6.1a2/py_evm.egg-info/requires.txt
--rw-r--r--   0 eve        (501) staff       (20)        4 2022-12-16 17:41:29.000000 py-evm-0.6.1a2/py_evm.egg-info/top_level.txt
--rw-r--r--   0 eve        (501) staff       (20)     1024 2021-02-22 21:36:31.000000 py-evm-0.6.1a2/pyproject.toml
--rw-r--r--   0 eve        (501) staff       (20)       38 2022-12-16 17:41:29.088681 py-evm-0.6.1a2/setup.cfg
--rw-r--r--   0 eve        (501) staff       (20)     3674 2022-12-16 17:41:25.000000 py-evm-0.6.1a2/setup.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.798251 py-evm-0.7.0a1/
+-rw-r--r--   0 eve        (501) staff       (20)     1087 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/LICENSE
+-rw-r--r--   0 eve        (501) staff       (20)      137 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/MANIFEST.in
+-rw-r--r--   0 eve        (501) staff       (20)     2673 2023-04-10 16:50:19.798089 py-evm-0.7.0a1/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     1854 2021-11-05 20:04:27.000000 py-evm-0.7.0a1/README.md
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.767113 py-evm-0.7.0a1/eth/
+-rw-r--r--   0 eve        (501) staff       (20)      368 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.769086 py-evm-0.7.0a1/eth/_utils/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      734 2022-12-07 18:37:56.000000 py-evm-0.7.0a1/eth/_utils/address.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.769501 py-evm-0.7.0a1/eth/_utils/blake2/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2022-12-07 18:37:56.000000 py-evm-0.7.0a1/eth/_utils/blake2/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1791 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/_utils/blake2/coders.py
+-rwxr-xr-x   0 eve        (501) staff       (20)     5784 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/blake2/compression.py
+-rw-r--r--   0 eve        (501) staff       (20)      972 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/bn128.py
+-rw-r--r--   0 eve        (501) staff       (20)     3900 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/datatypes.py
+-rw-r--r--   0 eve        (501) staff       (20)     1001 2022-12-07 18:37:56.000000 py-evm-0.7.0a1/eth/_utils/db.py
+-rw-r--r--   0 eve        (501) staff       (20)       40 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/empty.py
+-rw-r--r--   0 eve        (501) staff       (20)     8214 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/env.py
+-rw-r--r--   0 eve        (501) staff       (20)      613 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/generator.py
+-rw-r--r--   0 eve        (501) staff       (20)     5061 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/_utils/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2022-12-07 18:37:56.000000 py-evm-0.7.0a1/eth/_utils/logging.py
+-rw-r--r--   0 eve        (501) staff       (20)     1532 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/module_loading.py
+-rw-r--r--   0 eve        (501) staff       (20)     2801 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/numeric.py
+-rw-r--r--   0 eve        (501) staff       (20)      338 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/padding.py
+-rw-r--r--   0 eve        (501) staff       (20)     3338 2021-11-05 20:04:27.000000 py-evm-0.7.0a1/eth/_utils/rlp.py
+-rw-r--r--   0 eve        (501) staff       (20)     1739 2022-12-07 18:37:56.000000 py-evm-0.7.0a1/eth/_utils/spoof.py
+-rw-r--r--   0 eve        (501) staff       (20)     1352 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_utils/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     3409 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/_utils/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)      376 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/_utils/version.py
+-rw-r--r--   0 eve        (501) staff       (20)      346 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/_warnings.py
+-rw-r--r--   0 eve        (501) staff       (20)   118518 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/abc.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.769802 py-evm-0.7.0a1/eth/chains/
+-rw-r--r--   0 eve        (501) staff       (20)      223 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/chains/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    26256 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/chains/base.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.770110 py-evm-0.7.0a1/eth/chains/goerli/
+-rw-r--r--   0 eve        (501) staff       (20)     1277 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/chains/goerli/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      262 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/chains/goerli/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     2599 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/chains/header.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.770339 py-evm-0.7.0a1/eth/chains/mainnet/
+-rw-r--r--   0 eve        (501) staff       (20)     4517 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/chains/mainnet/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1191 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/chains/mainnet/constants.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.770548 py-evm-0.7.0a1/eth/chains/ropsten/
+-rw-r--r--   0 eve        (501) staff       (20)     2105 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/chains/ropsten/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      839 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/chains/ropsten/constants.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.770648 py-evm-0.7.0a1/eth/chains/tester/
+-rw-r--r--   0 eve        (501) staff       (20)     5965 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/chains/tester/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.771225 py-evm-0.7.0a1/eth/consensus/
+-rw-r--r--   0 eve        (501) staff       (20)      313 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      956 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/applier.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.772023 py-evm-0.7.0a1/eth/consensus/clique/
+-rw-r--r--   0 eve        (501) staff       (20)      270 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/clique/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     5106 2021-08-19 20:42:01.000000 py-evm-0.7.0a1/eth/consensus/clique/_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     5468 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/clique/clique.py
+-rw-r--r--   0 eve        (501) staff       (20)      477 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/clique/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     3380 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/clique/datatypes.py
+-rw-r--r--   0 eve        (501) staff       (20)     2929 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/consensus/clique/encoding.py
+-rw-r--r--   0 eve        (501) staff       (20)      149 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/clique/exceptions.py
+-rw-r--r--   0 eve        (501) staff       (20)    11037 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/clique/snapshot_manager.py
+-rw-r--r--   0 eve        (501) staff       (20)      188 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/context.py
+-rw-r--r--   0 eve        (501) staff       (20)      732 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/consensus/noproof.py
+-rw-r--r--   0 eve        (501) staff       (20)      834 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/consensus/pos.py
+-rw-r--r--   0 eve        (501) staff       (20)     4037 2022-08-17 18:04:11.000000 py-evm-0.7.0a1/eth/consensus/pow.py
+-rw-r--r--   0 eve        (501) staff       (20)     3853 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/constants.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.773815 py-evm-0.7.0a1/eth/db/
+-rw-r--r--   0 eve        (501) staff       (20)      746 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     3434 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/accesslog.py
+-rw-r--r--   0 eve        (501) staff       (20)    24116 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/db/account.py
+-rw-r--r--   0 eve        (501) staff       (20)     4172 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/atomic.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.774173 py-evm-0.7.0a1/eth/db/backends/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/backends/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2494 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/backends/base.py
+-rw-r--r--   0 eve        (501) staff       (20)     4410 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/backends/level.py
+-rw-r--r--   0 eve        (501) staff       (20)      890 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/backends/memory.py
+-rw-r--r--   0 eve        (501) staff       (20)     2811 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/batch.py
+-rw-r--r--   0 eve        (501) staff       (20)      943 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/cache.py
+-rw-r--r--   0 eve        (501) staff       (20)    19392 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/db/chain.py
+-rw-r--r--   0 eve        (501) staff       (20)     5524 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/chain_gaps.py
+-rw-r--r--   0 eve        (501) staff       (20)     7303 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/diff.py
+-rw-r--r--   0 eve        (501) staff       (20)      488 2021-08-19 20:42:01.000000 py-evm-0.7.0a1/eth/db/hash_trie.py
+-rw-r--r--   0 eve        (501) staff       (20)    24092 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/db/header.py
+-rw-r--r--   0 eve        (501) staff       (20)    16683 2021-03-10 18:54:42.000000 py-evm-0.7.0a1/eth/db/journal.py
+-rw-r--r--   0 eve        (501) staff       (20)     1291 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/keymap.py
+-rw-r--r--   0 eve        (501) staff       (20)     1345 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/db/schema.py
+-rw-r--r--   0 eve        (501) staff       (20)    16275 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/slow_journal.py
+-rw-r--r--   0 eve        (501) staff       (20)    16229 2021-03-04 23:10:51.000000 py-evm-0.7.0a1/eth/db/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)     1363 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/db/trie.py
+-rw-r--r--   0 eve        (501) staff       (20)     1667 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/db/witness.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.774399 py-evm-0.7.0a1/eth/estimators/
+-rw-r--r--   0 eve        (501) staff       (20)      522 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/estimators/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     3285 2021-08-19 20:42:40.000000 py-evm-0.7.0a1/eth/estimators/gas.py
+-rw-r--r--   0 eve        (501) staff       (20)     4076 2021-11-05 20:04:27.000000 py-evm-0.7.0a1/eth/exceptions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.775590 py-evm-0.7.0a1/eth/precompiles/
+-rw-r--r--   0 eve        (501) staff       (20)      398 2021-02-26 19:54:17.000000 py-evm-0.7.0a1/eth/precompiles/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      919 2021-09-03 20:35:50.000000 py-evm-0.7.0a1/eth/precompiles/blake2.py
+-rw-r--r--   0 eve        (501) staff       (20)     1487 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/precompiles/ecadd.py
+-rw-r--r--   0 eve        (501) staff       (20)     1375 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/precompiles/ecmul.py
+-rw-r--r--   0 eve        (501) staff       (20)     3261 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/precompiles/ecpairing.py
+-rw-r--r--   0 eve        (501) staff       (20)     1511 2021-11-05 20:04:27.000000 py-evm-0.7.0a1/eth/precompiles/ecrecover.py
+-rw-r--r--   0 eve        (501) staff       (20)      478 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/precompiles/identity.py
+-rw-r--r--   0 eve        (501) staff       (20)     4026 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/precompiles/modexp.py
+-rw-r--r--   0 eve        (501) staff       (20)      676 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/precompiles/ripemd160.py
+-rw-r--r--   0 eve        (501) staff       (20)      548 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/precompiles/sha256.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/py.typed
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.776441 py-evm-0.7.0a1/eth/rlp/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/rlp/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1032 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/rlp/accounts.py
+-rw-r--r--   0 eve        (501) staff       (20)      904 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/rlp/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     5587 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/rlp/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      669 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/rlp/logs.py
+-rw-r--r--   0 eve        (501) staff       (20)     1312 2021-03-10 18:54:47.000000 py-evm-0.7.0a1/eth/rlp/receipts.py
+-rw-r--r--   0 eve        (501) staff       (20)      370 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/rlp/sedes.py
+-rw-r--r--   0 eve        (501) staff       (20)     3595 2021-08-19 20:42:01.000000 py-evm-0.7.0a1/eth/rlp/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.776722 py-evm-0.7.0a1/eth/tools/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.777921 py-evm-0.7.0a1/eth/tools/_utils/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/_utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      637 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/tools/_utils/deprecation.py
+-rw-r--r--   0 eve        (501) staff       (20)      181 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/_utils/git.py
+-rw-r--r--   0 eve        (501) staff       (20)      532 2021-08-19 20:42:01.000000 py-evm-0.7.0a1/eth/tools/_utils/hashing.py
+-rw-r--r--   0 eve        (501) staff       (20)     1486 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/_utils/mappings.py
+-rw-r--r--   0 eve        (501) staff       (20)    17880 2022-08-31 18:17:44.000000 py-evm-0.7.0a1/eth/tools/_utils/normalization.py
+-rw-r--r--   0 eve        (501) staff       (20)     4314 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/_utils/slow_code_stream.py
+-rw-r--r--   0 eve        (501) staff       (20)      886 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/_utils/vyper.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.778044 py-evm-0.7.0a1/eth/tools/builder/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/builder/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.778269 py-evm-0.7.0a1/eth/tools/builder/chain/
+-rw-r--r--   0 eve        (501) staff       (20)     2936 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/tools/builder/chain/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    15213 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/tools/builder/chain/builders.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.778684 py-evm-0.7.0a1/eth/tools/db/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/db/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     5130 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/db/atomic.py
+-rw-r--r--   0 eve        (501) staff       (20)     2260 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/db/base.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.779239 py-evm-0.7.0a1/eth/tools/fixtures/
+-rw-r--r--   0 eve        (501) staff       (20)      615 2021-08-19 20:42:01.000000 py-evm-0.7.0a1/eth/tools/fixtures/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      878 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/_utils.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.780043 py-evm-0.7.0a1/eth/tools/fixtures/fillers/
+-rw-r--r--   0 eve        (501) staff       (20)      282 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/fillers/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2461 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/fillers/_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)    12490 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/fillers/common.py
+-rw-r--r--   0 eve        (501) staff       (20)     3108 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/fillers/formatters.py
+-rw-r--r--   0 eve        (501) staff       (20)     1305 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/fillers/main.py
+-rw-r--r--   0 eve        (501) staff       (20)     2617 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/fillers/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1747 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/fixtures/fillers/vm.py
+-rw-r--r--   0 eve        (501) staff       (20)     2136 2021-11-05 22:07:56.000000 py-evm-0.7.0a1/eth/tools/fixtures/generation.py
+-rw-r--r--   0 eve        (501) staff       (20)     9639 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/tools/fixtures/helpers.py
+-rw-r--r--   0 eve        (501) staff       (20)     3140 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/tools/fixtures/loading.py
+-rw-r--r--   0 eve        (501) staff       (20)      759 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/tools/mining.py
+-rw-r--r--   0 eve        (501) staff       (20)      449 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/tools/rlp.py
+-rw-r--r--   0 eve        (501) staff       (20)     3085 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/typing.py
+-rw-r--r--   0 eve        (501) staff       (20)     8876 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/validation.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.782010 py-evm-0.7.0a1/eth/vm/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    26822 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/base.py
+-rw-r--r--   0 eve        (501) staff       (20)      615 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/chain_context.py
+-rw-r--r--   0 eve        (501) staff       (20)     4247 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/code_stream.py
+-rw-r--r--   0 eve        (501) staff       (20)    18099 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)     2086 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/execution_context.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.782120 py-evm-0.7.0a1/eth/vm/forks/
+-rw-r--r--   0 eve        (501) staff       (20)      899 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.782822 py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/
+-rw-r--r--   0 eve        (501) staff       (20)      856 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      951 2022-06-23 20:10:28.000000 py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      267 2021-12-15 20:27:15.000000 py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)     1088 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      463 2021-12-15 20:27:15.000000 py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1132 2021-12-15 20:27:15.000000 py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.783925 py-evm-0.7.0a1/eth/vm/forks/berlin/
+-rw-r--r--   0 eve        (501) staff       (20)      760 2021-09-20 20:47:49.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      760 2021-03-10 18:54:47.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     2402 2021-03-31 17:31:28.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      327 2021-08-30 21:22:29.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      381 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     6462 2021-09-10 18:06:54.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/logic.py
+-rw-r--r--   0 eve        (501) staff       (20)     2888 2021-03-17 17:52:03.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)     4521 2021-08-30 17:37:29.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/receipts.py
+-rw-r--r--   0 eve        (501) staff       (20)     1192 2021-03-17 17:52:03.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/state.py
+-rw-r--r--   0 eve        (501) staff       (20)    15608 2021-11-05 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/berlin/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.785022 py-evm-0.7.0a1/eth/vm/forks/byzantium/
+-rw-r--r--   0 eve        (501) staff       (20)     3585 2021-09-20 20:47:49.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      483 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      965 2021-02-26 17:26:20.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      226 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     3434 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     3499 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      204 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1442 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/byzantium/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.786005 py-evm-0.7.0a1/eth/vm/forks/constantinople/
+-rw-r--r--   0 eve        (501) staff       (20)     1108 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      482 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      809 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      321 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      401 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     1569 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      211 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      325 2021-03-17 17:52:03.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)     1446 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/constantinople/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.787002 py-evm-0.7.0a1/eth/vm/forks/frontier/
+-rw-r--r--   0 eve        (501) staff       (20)     3820 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     3318 2021-08-19 20:42:40.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     3696 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)       96 2021-09-20 20:47:49.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     3546 2021-08-19 20:42:40.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)    20208 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)     7722 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      131 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/transaction_context.py
+-rw-r--r--   0 eve        (501) staff       (20)     6040 2021-08-19 20:42:01.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)     1698 2021-08-19 20:42:01.000000 py-evm-0.7.0a1/eth/vm/forks/frontier/validation.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.787544 py-evm-0.7.0a1/eth/vm/forks/gray_glacier/
+-rw-r--r--   0 eve        (501) staff       (20)      855 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/gray_glacier/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1017 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/gray_glacier/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      297 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/gray_glacier/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)     1132 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/gray_glacier/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      496 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/gray_glacier/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1168 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/gray_glacier/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.788390 py-evm-0.7.0a1/eth/vm/forks/homestead/
+-rw-r--r--   0 eve        (501) staff       (20)     1210 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      463 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     2261 2021-03-05 23:32:34.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)       61 2021-09-03 20:35:50.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     9661 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      603 2021-03-05 23:31:28.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      613 2021-03-05 23:32:34.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     2292 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)      548 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/homestead/validation.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.789417 py-evm-0.7.0a1/eth/vm/forks/istanbul/
+-rw-r--r--   0 eve        (501) staff       (20)      805 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      467 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     1466 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      316 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      385 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     1637 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      196 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      883 2021-09-02 18:17:22.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)     2000 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/istanbul/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.790511 py-evm-0.7.0a1/eth/vm/forks/london/
+-rw-r--r--   0 eve        (501) staff       (20)     2286 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/london/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     5835 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/london/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      772 2021-09-20 20:47:49.000000 py-evm-0.7.0a1/eth/vm/forks/london/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      470 2021-09-20 20:47:49.000000 py-evm-0.7.0a1/eth/vm/forks/london/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     5587 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/london/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      860 2021-09-20 20:47:49.000000 py-evm-0.7.0a1/eth/vm/forks/london/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      620 2021-08-30 17:37:29.000000 py-evm-0.7.0a1/eth/vm/forks/london/receipts.py
+-rw-r--r--   0 eve        (501) staff       (20)     4940 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/london/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      527 2021-09-20 20:47:49.000000 py-evm-0.7.0a1/eth/vm/forks/london/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)     9548 2021-11-05 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/london/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)      845 2021-08-19 20:42:40.000000 py-evm-0.7.0a1/eth/vm/forks/london/validation.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.791208 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/
+-rw-r--r--   0 eve        (501) staff       (20)      830 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      470 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      562 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      438 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      137 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      199 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1423 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/muir_glacier/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.791879 py-evm-0.7.0a1/eth/vm/forks/paris/
+-rw-r--r--   0 eve        (501) staff       (20)     2088 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/paris/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1014 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/paris/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      375 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/paris/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)     2234 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/paris/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      649 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/paris/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      619 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/paris/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1119 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/paris/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.792661 py-evm-0.7.0a1/eth/vm/forks/petersburg/
+-rw-r--r--   0 eve        (501) staff       (20)     1024 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      470 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      556 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      102 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      381 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)     1378 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      199 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1422 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/petersburg/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.793716 py-evm-0.7.0a1/eth/vm/forks/shanghai/
+-rw-r--r--   0 eve        (501) staff       (20)      667 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     8631 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     1595 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      187 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      784 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/headers.py
+-rw-r--r--   0 eve        (501) staff       (20)      820 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/logic.py
+-rw-r--r--   0 eve        (501) staff       (20)     1474 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      717 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     1097 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)     1461 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/shanghai/withdrawals.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.794726 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/
+-rw-r--r--   0 eve        (501) staff       (20)      429 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2124 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)      481 2021-03-01 17:34:33.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)     3234 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      169 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     1180 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)     1486 2021-09-03 22:22:38.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     2950 2021-03-10 18:54:47.000000 py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.795297 py-evm-0.7.0a1/eth/vm/forks/tangerine_whistle/
+-rw-r--r--   0 eve        (501) staff       (20)      469 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/tangerine_whistle/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      396 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/tangerine_whistle/computation.py
+-rw-r--r--   0 eve        (501) staff       (20)      225 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/tangerine_whistle/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     2067 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/tangerine_whistle/opcodes.py
+-rw-r--r--   0 eve        (501) staff       (20)      209 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/forks/tangerine_whistle/state.py
+-rw-r--r--   0 eve        (501) staff       (20)     2637 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/gas_meter.py
+-rw-r--r--   0 eve        (501) staff       (20)      531 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/header.py
+-rw-r--r--   0 eve        (501) staff       (20)     3414 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/interrupt.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.797136 py-evm-0.7.0a1/eth/vm/logic/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     4819 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/arithmetic.py
+-rw-r--r--   0 eve        (501) staff       (20)     1066 2022-12-09 20:04:27.000000 py-evm-0.7.0a1/eth/vm/logic/block.py
+-rw-r--r--   0 eve        (501) staff       (20)    14298 2021-03-17 17:52:03.000000 py-evm-0.7.0a1/eth/vm/logic/call.py
+-rw-r--r--   0 eve        (501) staff       (20)     2831 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/comparison.py
+-rw-r--r--   0 eve        (501) staff       (20)     6448 2021-03-17 17:52:03.000000 py-evm-0.7.0a1/eth/vm/logic/context.py
+-rw-r--r--   0 eve        (501) staff       (20)      948 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/duplication.py
+-rw-r--r--   0 eve        (501) staff       (20)     1518 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/flow.py
+-rw-r--r--   0 eve        (501) staff       (20)      480 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/invalid.py
+-rw-r--r--   0 eve        (501) staff       (20)     1342 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/logging.py
+-rw-r--r--   0 eve        (501) staff       (20)     1109 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/memory.py
+-rw-r--r--   0 eve        (501) staff       (20)      626 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/sha3.py
+-rw-r--r--   0 eve        (501) staff       (20)     2181 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/logic/stack.py
+-rw-r--r--   0 eve        (501) staff       (20)     3921 2021-09-10 18:08:36.000000 py-evm-0.7.0a1/eth/vm/logic/storage.py
+-rw-r--r--   0 eve        (501) staff       (20)      978 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/logic/swap.py
+-rw-r--r--   0 eve        (501) staff       (20)     9441 2021-11-05 20:04:27.000000 py-evm-0.7.0a1/eth/vm/logic/system.py
+-rw-r--r--   0 eve        (501) staff       (20)     2122 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/memory.py
+-rw-r--r--   0 eve        (501) staff       (20)     3177 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/message.py
+-rw-r--r--   0 eve        (501) staff       (20)     2785 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/mnemonics.py
+-rw-r--r--   0 eve        (501) staff       (20)     1895 2021-08-30 21:41:40.000000 py-evm-0.7.0a1/eth/vm/opcode.py
+-rw-r--r--   0 eve        (501) staff       (20)     2430 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/opcode_values.py
+-rw-r--r--   0 eve        (501) staff       (20)      385 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/spoof.py
+-rw-r--r--   0 eve        (501) staff       (20)     7675 2021-03-17 17:52:03.000000 py-evm-0.7.0a1/eth/vm/stack.py
+-rw-r--r--   0 eve        (501) staff       (20)    10402 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/eth/vm/state.py
+-rw-r--r--   0 eve        (501) staff       (20)      857 2021-02-22 21:36:31.000000 py-evm-0.7.0a1/eth/vm/transaction_context.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-04-10 16:50:19.797881 py-evm-0.7.0a1/py_evm.egg-info/
+-rw-r--r--   0 eve        (501) staff       (20)     2673 2023-04-10 16:50:19.000000 py-evm-0.7.0a1/py_evm.egg-info/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     8485 2023-04-10 16:50:19.000000 py-evm-0.7.0a1/py_evm.egg-info/SOURCES.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-04-10 16:50:19.000000 py-evm-0.7.0a1/py_evm.egg-info/dependency_links.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2021-02-24 18:15:32.000000 py-evm-0.7.0a1/py_evm.egg-info/not-zip-safe
+-rw-r--r--   0 eve        (501) staff       (20)     2057 2023-04-10 16:50:19.000000 py-evm-0.7.0a1/py_evm.egg-info/requires.txt
+-rw-r--r--   0 eve        (501) staff       (20)        4 2023-04-10 16:50:19.000000 py-evm-0.7.0a1/py_evm.egg-info/top_level.txt
+-rw-r--r--   0 eve        (501) staff       (20)     1108 2023-04-10 16:24:16.000000 py-evm-0.7.0a1/pyproject.toml
+-rw-r--r--   0 eve        (501) staff       (20)       38 2023-04-10 16:50:19.798298 py-evm-0.7.0a1/setup.cfg
+-rw-r--r--   0 eve        (501) staff       (20)     3674 2023-04-10 16:50:15.000000 py-evm-0.7.0a1/setup.py
```

### Comparing `py-evm-0.6.1a2/LICENSE` & `py-evm-0.7.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/PKG-INFO` & `py-evm-0.7.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-evm
-Version: 0.6.1a2
+Version: 0.7.0a1
 Summary: Python implementation of the Ethereum Virtual Machine
 Home-page: https://github.com/ethereum/py-evm
 Author: Ethereum Foundation
 Author-email: piper@pipermerriam.com
 License: MIT
 Keywords: ethereum blockchain evm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `py-evm-0.6.1a2/README.md` & `py-evm-0.7.0a1/README.md`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/_utils/address.py` & `py-evm-0.7.0a1/eth/_utils/address.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/_utils/blake2/coders.py` & `py-evm-0.7.0a1/eth/_utils/blake2/coders.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/_utils/blake2/compression.py` & `py-evm-0.7.0a1/eth/_utils/blake2/compression.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/_utils/bn128.py` & `py-evm-0.7.0a1/eth/_utils/bn128.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/_utils/datatypes.py` & `py-evm-0.7.0a1/eth/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/_utils/db.py` & `py-evm-0.7.0a1/eth/_utils/db.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/_utils/env.py` & `py-evm-0.7.0a1/eth/_utils/env.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/_utils/generator.py` & `py-evm-0.7.0a1/eth/_utils/generator.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/_utils/headers.py` & `py-evm-0.7.0a1/eth/_utils/headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 from typing import (
     Dict,
+    Optional,
     Tuple,
 )
 
 from eth_typing import (
     Address,
 )
 
@@ -30,15 +31,15 @@
 def eth_now() -> int:
     """
     The timestamp is in UTC.
     """
     return int(datetime.datetime.utcnow().timestamp())
 
 
-def new_timestamp_from_parent(parent: BlockHeaderAPI) -> int:
+def new_timestamp_from_parent(parent: Optional[BlockHeaderAPI]) -> int:
     """
     Generate a timestamp to use on a new header.
 
     Generally, attempt to use the current time. If timestamp is too old (equal
     or less than parent), return `parent.timestamp + 1`. If parent is None,
     then consider this a genesis block.
     """
```

### Comparing `py-evm-0.6.1a2/eth/_utils/module_loading.py` & `py-evm-0.7.0a1/eth/_utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/_utils/numeric.py` & `py-evm-0.7.0a1/eth/_utils/numeric.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/_utils/rlp.py` & `py-evm-0.7.0a1/eth/_utils/rlp.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/_utils/spoof.py` & `py-evm-0.7.0a1/eth/_utils/spoof.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/_utils/state.py` & `py-evm-0.7.0a1/eth/_utils/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/_utils/transactions.py` & `py-evm-0.7.0a1/eth/_utils/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/abc.py` & `py-evm-0.7.0a1/eth/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,24 @@
         """
         Return the base fee per gas of the block.
 
         Set to None in pre-EIP-1559 (London) header.
         """
         ...
 
+    @property
+    @abstractmethod
+    def withdrawals_root(self) -> Optional[Hash32]:
+        """
+        Return the withdrawals root of the block.
+
+        Set to None in pre-Shanghai header.
+        """
+        ...
+
 
 class BlockHeaderSedesAPI(ABC):
     """
     Serialize and deserialize RLP for a header.
 
     The header may be one of several definitions, like a London (EIP-1559) or
     pre-London header.
@@ -704,29 +714,96 @@
         This encodes a transaction, no matter if it's: a legacy transaction, a
         typed transaction, or the payload of a typed transaction. See more
         context in decode.
         """
         ...
 
 
+class WithdrawalAPI(ABC):
+    """
+    A class to define a withdrawal.
+    """
+
+    @property
+    @abstractmethod
+    def index(self) -> int:
+        """
+        A monotonically increasing index, starting from 0, that increments by 1 per
+        withdrawal to uniquely identify each withdrawal.
+        """
+        ...
+
+    @property
+    @abstractmethod
+    def validator_index(self) -> int:
+        """
+        The index for the validator on the consensus layer the withdrawal corresponds
+        to.
+        """
+        ...
+
+    @property
+    @abstractmethod
+    def address(self) -> Address:
+        """
+        The recipient address for the withdrawn ether.
+        """
+        ...
+
+    @property
+    @abstractmethod
+    def amount(self) -> int:
+        """
+        The nonzero amount of ether to withdraw, given in gwei (10**9 wei).
+        """
+        ...
+
+    @property
+    @abstractmethod
+    def hash(self) -> Hash32:
+        """
+        Return the hash of the withdrawal.
+        """
+        ...
+
+    @abstractmethod
+    def validate(self) -> None:
+        """
+        Validate withdrawal fields.
+        """
+        ...
+
+    @abstractmethod
+    def encode(self) -> bytes:
+        """
+        Return the encoded withdrawal.
+        """
+        ...
+
+
 class BlockAPI(ABC):
     """
     A class to define a block.
     """
     header: BlockHeaderAPI
     transactions: Tuple[SignedTransactionAPI, ...]
+    uncles: Tuple[BlockHeaderAPI, ...]
+    withdrawals: Tuple[WithdrawalAPI, ...]
+
     transaction_builder: Type[TransactionBuilderAPI] = None
     receipt_builder: Type[ReceiptBuilderAPI] = None
-    uncles: Tuple[BlockHeaderAPI, ...]
 
     @abstractmethod
-    def __init__(self,
-                 header: BlockHeaderAPI,
-                 transactions: Sequence[SignedTransactionAPI],
-                 uncles: Sequence[BlockHeaderAPI]):
+    def __init__(
+        self,
+        header: BlockHeaderAPI,
+        transactions: Sequence[SignedTransactionAPI],
+        uncles: Sequence[BlockHeaderAPI],
+        withdrawals: Sequence[WithdrawalAPI] = None,  # only present post-Shanghai
+    ) -> None:
         ...
 
     @classmethod
     @abstractmethod
     def get_transaction_builder(cls) -> Type[TransactionBuilderAPI]:
         """
         Return the transaction builder for the block.
@@ -890,14 +967,22 @@
     @abstractmethod
     def make_transaction_hash_to_block_lookup_key(transaction_hash: Hash32) -> bytes:
         """
         Return the lookup key to retrieve a transaction key from a transaction hash.
         """
         ...
 
+    @staticmethod
+    @abstractmethod
+    def make_withdrawal_hash_to_block_lookup_key(withdrawal_hash: Hash32) -> bytes:
+        """
+        Return the lookup key to retrieve a withdrawal key from a withdrawal hash.
+        """
+        ...
+
 
 class DatabaseAPI(MutableMapping[bytes, bytes], ABC):
     """
     A class representing a database.
     """
     @abstractmethod
     def set(self, key: bytes, value: bytes) -> None:
@@ -1219,14 +1304,29 @@
 
         Raise ``TransactionNotFound`` if the transaction_hash is not found in the
         canonical chain.
         """
         ...
 
     #
+    # Withdrawals API
+    #
+
+    @abstractmethod
+    def get_block_withdrawals(
+        self,
+        block_header: BlockHeaderAPI,
+    ) -> Tuple[WithdrawalAPI, ...]:
+        """
+        Return an iterable of withdrawals for the block specified by the
+        given block header.
+        """
+        ...
+
+    #
     # Raw Database API
     #
     @abstractmethod
     def exists(self, key: bytes) -> bool:
         """
         Return ``True`` if the given key exists in the database.
         """
@@ -3036,14 +3136,23 @@
     def get_transaction_context(self,
                                 transaction: SignedTransactionAPI) -> TransactionContextAPI:
         """
         Return the :class:`~eth.abc.TransactionContextAPI` for the given ``transaction``
         """
         ...
 
+    #
+    # Withdrawals
+    #
+    def apply_withdrawal(self, withdrawal: WithdrawalAPI) -> None:
+        ...
+
+    def apply_all_withdrawals(self, withdrawals: Sequence[WithdrawalAPI]) -> None:
+        ...
+
 
 class ConsensusContextAPI(ABC):
     """
     A class representing a data context for the :class:`~eth.abc.ConsensusAPI` which is
     instantiated once per chain instance and stays in memory across VM runs.
     """
 
@@ -3248,14 +3357,23 @@
 
         :param transactions: an iterable of all transactions to apply
         :param base_header: the starting header to apply transactions to
         :return: the final header, the receipts of each transaction, and the computations
         """
         ...
 
+    def apply_all_withdrawals(self, withdrawals: Sequence[WithdrawalAPI]) -> None:
+        """
+        Updates the state by applying all withdrawals.
+        This does *not* update the current block or header of the VM.
+
+        :param withdrawals: an iterable of all withdrawals to apply
+        """
+        ...
+
     @abstractmethod
     def make_receipt(self,
                      base_header: BlockHeaderAPI,
                      transaction: SignedTransactionAPI,
                      computation: ComputationAPI,
                      state: StateAPI) -> ReceiptAPI:
         """
@@ -3284,21 +3402,24 @@
     def mine_block(self, block: BlockAPI, *args: Any, **kwargs: Any) -> BlockAndMetaWitness:
         """
         Mine the given block. Proxies to self.pack_block method.
         """
         ...
 
     @abstractmethod
-    def set_block_transactions(self,
-                               base_block: BlockAPI,
-                               new_header: BlockHeaderAPI,
-                               transactions: Sequence[SignedTransactionAPI],
-                               receipts: Sequence[ReceiptAPI]) -> BlockAPI:
+    def set_block_transactions_and_withdrawals(
+        self,
+        base_block: BlockAPI,
+        new_header: BlockHeaderAPI,
+        transactions: Sequence[SignedTransactionAPI],
+        receipts: Sequence[ReceiptAPI],
+        withdrawals: Sequence[WithdrawalAPI] = None,
+    ) -> BlockAPI:
         """
-        Create a new block with the given ``transactions``.
+        Create a new block with the given ``transactions`` and/or ``withdrawals``.
         """
         ...
 
     #
     # Finalization
     #
     @abstractmethod
@@ -3878,26 +3999,28 @@
 
         Raise ``BlockNotFound`` if there's no block with the given number in the
         canonical chain.
         """
         ...
 
     @abstractmethod
-    def build_block_with_transactions(
+    def build_block_with_transactions_and_withdrawals(
             self,
             transactions: Tuple[SignedTransactionAPI, ...],
-            parent_header: BlockHeaderAPI = None
+            parent_header: BlockHeaderAPI = None,
+            withdrawals: Tuple[WithdrawalAPI, ...] = None,
     ) -> Tuple[BlockAPI, Tuple[ReceiptAPI, ...], Tuple[ComputationAPI, ...]]:
         """
         Generate a block with the provided transactions. This does *not* import
         that block into your chain. If you want this new block in your chain,
         run :meth:`~import_block` with the result block from this method.
 
-        :param transactions: an iterable of transactions to insert to the block
+        :param transactions: an iterable of transactions to insert into the block
         :param parent_header: parent of the new block -- or canonical head if ``None``
+        :param withdrawals: an iterable of withdrawals to insert into the block
         :return: (new block, receipts, computations)
         """
         ...
 
     #
     # Transaction API
     #
```

### Comparing `py-evm-0.6.1a2/eth/chains/base.py` & `py-evm-0.7.0a1/eth/chains/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     ConsensusContextAPI,
     VirtualMachineAPI,
     ReceiptAPI,
     ComputationAPI,
     StateAPI,
     SignedTransactionAPI,
     UnsignedTransactionAPI,
+    WithdrawalAPI,
 )
 from eth.consensus import (
     ConsensusContext,
 )
 from eth.constants import (
     EMPTY_UNCLE_HASH,
     MAX_UNCLE_DEPTH,
@@ -342,24 +343,38 @@
     def get_canonical_block_by_number(self, block_number: BlockNumber) -> BlockAPI:
         validate_uint256(block_number, title="Block Number")
         return self.get_block_by_hash(self.chaindb.get_canonical_block_hash(block_number))
 
     def get_canonical_block_hash(self, block_number: BlockNumber) -> Hash32:
         return self.chaindb.get_canonical_block_hash(block_number)
 
-    def build_block_with_transactions(
+    def build_block_with_transactions_and_withdrawals(
             self,
             transactions: Sequence[SignedTransactionAPI],
-            parent_header: BlockHeaderAPI = None
+            parent_header: BlockHeaderAPI = None,
+            withdrawals: Sequence[WithdrawalAPI] = None,
     ) -> Tuple[BlockAPI, Tuple[ReceiptAPI, ...], Tuple[ComputationAPI, ...]]:
         base_header = self.ensure_header(parent_header)
         vm = self.get_vm(base_header)
 
-        new_header, receipts, computations = vm.apply_all_transactions(transactions, base_header)
-        new_block = vm.set_block_transactions(vm.get_block(), new_header, transactions, receipts)
+        new_header, receipts, computations = vm.apply_all_transactions(
+            transactions,
+            base_header,
+        )
+
+        if withdrawals:
+            vm.apply_all_withdrawals(withdrawals)
+
+        new_block = vm.set_block_transactions_and_withdrawals(
+            vm.get_block(),
+            new_header,
+            transactions,
+            receipts,
+            withdrawals=withdrawals,
+        )
 
         return new_block, receipts, computations
 
     #
     # Transaction API
     #
     def get_canonical_transaction_index(self, transaction_hash: Hash32) -> Tuple[BlockNumber, int]:
@@ -623,31 +638,37 @@
 class MiningChain(Chain, MiningChainAPI):
     header: BlockHeaderAPI = None
 
     def __init__(self, base_db: AtomicDatabaseAPI, header: BlockHeaderAPI = None) -> None:
         super().__init__(base_db)
         self.header = self.ensure_header(header)
 
-    def apply_transaction(self,
-                          transaction: SignedTransactionAPI
-                          ) -> Tuple[BlockAPI, ReceiptAPI, ComputationAPI]:
+    def apply_transaction(
+        self,
+        transaction: SignedTransactionAPI,
+    ) -> Tuple[BlockAPI, ReceiptAPI, ComputationAPI]:
         vm = self.get_vm(self.header)
         base_block = vm.get_block()
 
         receipt, computation = vm.apply_transaction(base_block.header, transaction)
         header_with_receipt = vm.add_receipt_to_header(base_block.header, receipt)
 
         # since we are building the block locally, we have to persist all the incremental state
         vm.state.persist()
         new_header: BlockHeaderAPI = header_with_receipt.copy(state_root=vm.state.state_root)
 
         transactions = base_block.transactions + (transaction, )
         receipts = base_block.get_receipts(self.chaindb) + (receipt, )
 
-        new_block = vm.set_block_transactions(base_block, new_header, transactions, receipts)
+        new_block = vm.set_block_transactions_and_withdrawals(
+            base_block,
+            new_header,
+            transactions,
+            receipts,
+        )
 
         self.header = new_block.header
 
         return new_block, receipt, computation
 
     def import_block(self,
                      block: BlockAPI,
@@ -669,33 +690,47 @@
         return base_header.copy(**header_params)
 
     def mine_all(
             self,
             transactions: Sequence[SignedTransactionAPI],
             *args: Any,
             parent_header: BlockHeaderAPI = None,
+            withdrawals: Sequence[WithdrawalAPI] = None,
             **kwargs: Any,
     ) -> Tuple[BlockImportResult, Tuple[ReceiptAPI, ...], Tuple[ComputationAPI, ...]]:
 
         if parent_header is None:
             base_header = self.header
         else:
             base_header = self.create_header_from_parent(parent_header)
 
         custom_header = self._custom_header(base_header, **kwargs)
         vm = self.get_vm(custom_header)
 
         new_header, receipts, computations = vm.apply_all_transactions(transactions, base_header)
-        filled_block = vm.set_block_transactions(vm.get_block(), new_header, transactions, receipts)
+
+        if withdrawals:
+            vm.apply_all_withdrawals(withdrawals)
+
+        filled_block = vm.set_block_transactions_and_withdrawals(
+            vm.get_block(),
+            new_header,
+            transactions,
+            receipts,
+            withdrawals=withdrawals,
+        )
 
         block_result = vm.mine_block(filled_block, *args, **kwargs)
         imported_block = block_result.block
 
         block_persist_result = self.persist_block(imported_block)
-        block_import_result = BlockImportResult(*block_persist_result, block_result.meta_witness)
+        block_import_result = BlockImportResult(
+            *block_persist_result,
+            block_result.meta_witness,
+        )
 
         self.header = self.create_header_from_parent(imported_block.header)
         return (block_import_result, receipts, computations)
 
     def mine_block(self, *args: Any, **kwargs: Any) -> BlockAPI:
         """
         Mine whatever transactions have been incrementally applied so far.
```

### Comparing `py-evm-0.6.1a2/eth/chains/goerli/__init__.py` & `py-evm-0.7.0a1/eth/chains/goerli/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/chains/header.py` & `py-evm-0.7.0a1/eth/chains/header.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/chains/mainnet/__init__.py` & `py-evm-0.7.0a1/eth/chains/mainnet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     GrayGlacierVM,
     HomesteadVM,
     IstanbulVM,
     LondonVM,
     MuirGlacierVM,
     ParisVM,
     PetersburgVM,
+    ShanghaiVM,
     SpuriousDragonVM,
     TangerineWhistleVM,
 )
 
 
 def validate_header_is_on_intended_dao_fork(support_dao_fork: bool,
                                             dao_fork_at: BlockNumber,
@@ -122,14 +123,15 @@
     BerlinVM,
     LondonVM,
     ArrowGlacierVM,
     GrayGlacierVM,
 )
 POS_MAINNET_VMS = (
     ParisVM,
+    ShanghaiVM,
 )
 
 MAINNET_VMS = MINING_MAINNET_VMS + POS_MAINNET_VMS
 MAINNET_VM_CONFIGURATION = tuple(zip(MAINNET_FORK_BLOCKS, MAINNET_VMS))
 
 
 class BaseMainnetChain:
```

### Comparing `py-evm-0.6.1a2/eth/chains/mainnet/constants.py` & `py-evm-0.7.0a1/eth/chains/mainnet/constants.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/chains/ropsten/__init__.py` & `py-evm-0.7.0a1/eth/chains/ropsten/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/chains/ropsten/constants.py` & `py-evm-0.7.0a1/eth/chains/ropsten/constants.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/chains/tester/__init__.py` & `py-evm-0.7.0a1/eth/chains/tester/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/consensus/applier.py` & `py-evm-0.7.0a1/eth/consensus/applier.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/consensus/clique/_utils.py` & `py-evm-0.7.0a1/eth/consensus/clique/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/consensus/clique/clique.py` & `py-evm-0.7.0a1/eth/consensus/clique/clique.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/consensus/clique/datatypes.py` & `py-evm-0.7.0a1/eth/consensus/clique/datatypes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/consensus/clique/encoding.py` & `py-evm-0.7.0a1/eth/consensus/clique/encoding.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/consensus/clique/snapshot_manager.py` & `py-evm-0.7.0a1/eth/consensus/clique/snapshot_manager.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/consensus/noproof.py` & `py-evm-0.7.0a1/eth/consensus/noproof.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/consensus/pos.py` & `py-evm-0.7.0a1/eth/consensus/pos.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/consensus/pow.py` & `py-evm-0.7.0a1/eth/consensus/pow.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/constants.py` & `py-evm-0.7.0a1/eth/constants.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/__init__.py` & `py-evm-0.7.0a1/eth/db/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/accesslog.py` & `py-evm-0.7.0a1/eth/db/accesslog.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/account.py` & `py-evm-0.7.0a1/eth/db/account.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/atomic.py` & `py-evm-0.7.0a1/eth/db/atomic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/backends/base.py` & `py-evm-0.7.0a1/eth/db/backends/base.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/backends/level.py` & `py-evm-0.7.0a1/eth/db/backends/level.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/backends/memory.py` & `py-evm-0.7.0a1/eth/db/backends/memory.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/batch.py` & `py-evm-0.7.0a1/eth/db/batch.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/cache.py` & `py-evm-0.7.0a1/eth/db/cache.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/chain.py` & `py-evm-0.7.0a1/eth/db/chain.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,17 @@
     Iterable,
     Sequence,
     Tuple,
     Type,
     cast,
 )
 
+from eth.vm.forks.shanghai.withdrawals import (
+    Withdrawal,
+)
 from eth_typing import (
     BlockNumber,
     Hash32
 )
 from eth_utils import (
     encode_hex,
 )
@@ -29,14 +32,15 @@
     ChainDatabaseAPI,
     DatabaseAPI,
     AtomicDatabaseAPI,
     ReceiptAPI,
     ReceiptDecoderAPI,
     SignedTransactionAPI,
     TransactionDecoderAPI,
+    WithdrawalAPI,
 )
 from eth.constants import (
     EMPTY_UNCLE_HASH,
     GENESIS_PARENT_HASH,
 )
 from eth.db.chain_gaps import (
     fill_gap,
@@ -68,15 +72,16 @@
     )
     from eth_utils import (
         to_tuple,
         ValidationError,
     )
 
 
-class TransactionKey(rlp.Serializable):
+class BlockDataKey(rlp.Serializable):
+    # used for transactions and withdrawals
     fields = [
         ('block_number', rlp.sedes.big_endian_int),
         ('index', rlp.sedes.big_endian_int),
     ]
 
 
 class ChainDB(HeaderDB, ChainDatabaseAPI):
@@ -255,14 +260,27 @@
                 tx_hashes = tuple(tx.hash for tx in block.transactions)
             else:
                 tx_hashes = cls._get_block_transaction_hashes(db, header)
 
             for index, transaction_hash in enumerate(tx_hashes):
                 cls._add_transaction_to_canonical_chain(db, transaction_hash, header, index)
 
+            # post-shanghai, look for withdrawals
+            if hasattr(block, "withdrawals") and block.withdrawals not in (None, ()):
+                withdrawal_hashes = tuple(
+                    withdrawal.hash for withdrawal in block.withdrawals
+                )
+                for index, withdrawal_hash in enumerate(withdrawal_hashes):
+                    cls._add_withdrawal_to_canonical_chain(
+                        db,
+                        withdrawal_hash,
+                        header,
+                        index,
+                    )
+
         if block.uncles:
             uncles_hash = cls._persist_uncles(db, block.uncles)
         else:
             uncles_hash = EMPTY_UNCLE_HASH
         if uncles_hash != block.header.uncles_hash:
             raise ValidationError(
                 "Block's uncles_hash (%s) does not match actual uncles' hash (%s)",
@@ -283,18 +301,41 @@
     def _persist_uncles(
             db: DatabaseAPI,
             uncles: Tuple[BlockHeaderAPI, ...]) -> Hash32:
 
         uncles_hash = keccak(rlp.encode(uncles))
         db.set(
             uncles_hash,
-            rlp.encode(uncles, sedes=rlp.sedes.CountableList(HeaderSedes)))
+            rlp.encode(uncles, sedes=rlp.sedes.CountableList(HeaderSedes)),
+        )
         return cast(Hash32, uncles_hash)
 
     #
+    # Block Data API (Transactions, Receipts, and Withdrawals)
+    #
+    @staticmethod
+    def _get_block_data_from_root_hash(
+        db: DatabaseAPI,
+        block_root_hash: Hash32,
+    ) -> Iterable[Hash32]:
+        """
+        Returns iterable of the encoded items from a root hash in a block. This can be
+        useful for retrieving encoded transactions or withdrawals from the
+        transaction_root or withdrawals_root of a block.
+        """
+        item_db = HexaryTrie(db, root_hash=block_root_hash)
+        for item_idx in itertools.count():
+            item_key = rlp.encode(item_idx)
+            encoded = item_db[item_key]
+            if encoded != b'':
+                yield encoded
+            else:
+                break
+
+    #
     # Transaction API
     #
     def add_receipt(self,
                     block_header: BlockHeaderAPI,
                     index_key: int, receipt: ReceiptAPI) -> Hash32:
         receipt_db = HexaryTrie(db=self.db, root_hash=block_header.receipt_root)
         receipt_db[index_key] = receipt.encode()
@@ -323,15 +364,15 @@
 
     @classmethod
     @to_tuple
     def _get_block_transaction_hashes(
             cls,
             db: DatabaseAPI,
             block_header: BlockHeaderAPI) -> Iterable[Hash32]:
-        all_encoded_transactions = cls._get_block_transaction_data(
+        all_encoded_transactions = cls._get_block_data_from_root_hash(
             db,
             block_header.transaction_root,
         )
         for encoded_transaction in all_encoded_transactions:
             yield cast(Hash32, keccak(encoded_transaction))
 
     @to_tuple
@@ -371,15 +412,15 @@
         try:
             encoded_key = self.db[key]
         except KeyError:
             raise TransactionNotFound(
                 f"Transaction {encode_hex(transaction_hash)} not found in canonical chain"
             )
 
-        transaction_key = rlp.decode(encoded_key, sedes=TransactionKey)
+        transaction_key = rlp.decode(encoded_key, sedes=BlockDataKey)
         return (transaction_key.block_number, transaction_key.index)
 
     def get_receipt_by_index(self,
                              block_number: BlockNumber,
                              receipt_index: int,
                              receipt_decoder: Type[ReceiptDecoderAPI],
                              ) -> ReceiptAPI:
@@ -394,38 +435,24 @@
         if receipt_data != b'':
             return receipt_decoder.decode(receipt_data)
         else:
             raise ReceiptNotFound(
                 f"Receipt with index {receipt_index} not found in block"
             )
 
-    @staticmethod
-    def _get_block_transaction_data(db: DatabaseAPI, transaction_root: Hash32) -> Iterable[Hash32]:
-        """
-        Returns iterable of the encoded transactions for the given block header
-        """
-        transaction_db = HexaryTrie(db, root_hash=transaction_root)
-        for transaction_idx in itertools.count():
-            transaction_key = rlp.encode(transaction_idx)
-            encoded = transaction_db[transaction_key]
-            if encoded != b'':
-                yield encoded
-            else:
-                break
-
     @functools.lru_cache(maxsize=32)
     @to_tuple
     def _get_block_transactions(
             self,
             transaction_root: Hash32,
             transaction_decoder: Type[TransactionDecoderAPI]) -> Iterable[SignedTransactionAPI]:
         """
         Memoizable version of `get_block_transactions`
         """
-        for encoded_transaction in self._get_block_transaction_data(self.db, transaction_root):
+        for encoded_transaction in self._get_block_data_from_root_hash(self.db, transaction_root):
             yield transaction_decoder.decode(encoded_transaction)
 
     @staticmethod
     def _remove_transaction_from_canonical_chain(db: DatabaseAPI, transaction_hash: Hash32) -> None:
         """
         Removes the transaction specified by the given hash from the canonical
         chain.
@@ -440,21 +467,58 @@
         """
         :param bytes transaction_hash: the hash of the transaction to add the lookup for
         :param block_header: The header of the block with the txn that is in the canonical chain
         :param int index: the position of the transaction in the block
         - add lookup from transaction hash to the block number and index that the body is stored at
         - remove transaction hash to body lookup in the pending pool
         """
-        transaction_key = TransactionKey(block_header.block_number, index)
+        transaction_key = BlockDataKey(block_header.block_number, index)
         db.set(
             SchemaV1.make_transaction_hash_to_block_lookup_key(transaction_hash),
             rlp.encode(transaction_key),
         )
 
     #
+    # Withdrawals API
+    #
+    def get_block_withdrawals(
+        self,
+        header: BlockHeaderAPI,
+    ) -> Tuple[WithdrawalAPI, ...]:
+        return self._get_block_withdrawals(header.withdrawals_root)
+
+    @functools.lru_cache(maxsize=32)
+    @to_tuple
+    def _get_block_withdrawals(
+        self,
+        withdrawals_root: Hash32,
+    ) -> Iterable[WithdrawalAPI]:
+        """
+        Memoizable version of `get_block_withdrawals`
+        """
+        for encoded_withdrawal in self._get_block_data_from_root_hash(
+            self.db,
+            withdrawals_root,
+        ):
+            yield rlp.decode(encoded_withdrawal, sedes=Withdrawal)
+
+    @staticmethod
+    def _add_withdrawal_to_canonical_chain(
+        db: DatabaseAPI,
+        withdrawal_hash: Hash32,
+        block_header: BlockHeaderAPI,
+        index: int
+    ) -> None:
+        withdrawal_key = BlockDataKey(block_header.block_number, index)
+        db.set(
+            SchemaV1.make_withdrawal_hash_to_block_lookup_key(withdrawal_hash),
+            rlp.encode(withdrawal_key),
+        )
+
+    #
     # Raw Database API
     #
     def exists(self, key: bytes) -> bool:
         return self.db.exists(key)
 
     def get(self, key: bytes) -> bytes:
         return self.db[key]
```

### Comparing `py-evm-0.6.1a2/eth/db/chain_gaps.py` & `py-evm-0.7.0a1/eth/db/chain_gaps.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/diff.py` & `py-evm-0.7.0a1/eth/db/diff.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/header.py` & `py-evm-0.7.0a1/eth/db/header.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/journal.py` & `py-evm-0.7.0a1/eth/db/journal.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/keymap.py` & `py-evm-0.7.0a1/eth/db/keymap.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/schema.py` & `py-evm-0.7.0a1/eth/db/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,7 +34,11 @@
         Checkpoint header hashes stored as concatenated 32 byte values
         """
         return b'v1:checkpoint-header-hashes-list'
 
     @staticmethod
     def make_transaction_hash_to_block_lookup_key(transaction_hash: Hash32) -> bytes:
         return b'transaction-hash-to-block:%s' % transaction_hash
+
+    @staticmethod
+    def make_withdrawal_hash_to_block_lookup_key(withdrawal_hash: Hash32) -> bytes:
+        return b'withdrawal-hash-to-block:%s' % withdrawal_hash
```

### Comparing `py-evm-0.6.1a2/eth/db/slow_journal.py` & `py-evm-0.7.0a1/eth/db/slow_journal.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/storage.py` & `py-evm-0.7.0a1/eth/db/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/db/trie.py` & `py-evm-0.7.0a1/eth/db/trie.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 )
 
 from eth_typing import Hash32
 
 from eth.abc import (
     ReceiptAPI,
     SignedTransactionAPI,
+    WithdrawalAPI,
 )
 from eth.constants import (
     BLANK_ROOT_HASH,
 )
 
-TransactionsOrReceipts = Union[Sequence[ReceiptAPI], Sequence[SignedTransactionAPI]]
+BlockRootData = Union[
+    Sequence[ReceiptAPI], Sequence[SignedTransactionAPI], Sequence[WithdrawalAPI]
+]
 TrieRootAndData = Tuple[Hash32, Dict[Hash32, bytes]]
 
 
-def make_trie_root_and_nodes(items: TransactionsOrReceipts) -> TrieRootAndData:
+def make_trie_root_and_nodes(items: BlockRootData) -> TrieRootAndData:
     return _make_trie_root_and_nodes(tuple(item.encode() for item in items))
 
 
 # This cache is expected to be useful when importing blocks as we call this once when importing
 # and again when validating the imported block. But it should also help for post-Byzantium blocks
 # as it's common for them to have duplicate receipt_roots. Given that, it probably makes sense to
 # use a relatively small cache size here.
```

### Comparing `py-evm-0.6.1a2/eth/db/witness.py` & `py-evm-0.7.0a1/eth/db/witness.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/estimators/__init__.py` & `py-evm-0.7.0a1/eth/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/estimators/gas.py` & `py-evm-0.7.0a1/eth/estimators/gas.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/exceptions.py` & `py-evm-0.7.0a1/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/precompiles/blake2.py` & `py-evm-0.7.0a1/eth/precompiles/blake2.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/precompiles/ecadd.py` & `py-evm-0.7.0a1/eth/precompiles/ecadd.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/precompiles/ecmul.py` & `py-evm-0.7.0a1/eth/precompiles/ecmul.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/precompiles/ecpairing.py` & `py-evm-0.7.0a1/eth/precompiles/ecpairing.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/precompiles/ecrecover.py` & `py-evm-0.7.0a1/eth/precompiles/ecrecover.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/precompiles/modexp.py` & `py-evm-0.7.0a1/eth/precompiles/modexp.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/precompiles/ripemd160.py` & `py-evm-0.7.0a1/eth/precompiles/ripemd160.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/precompiles/sha256.py` & `py-evm-0.7.0a1/eth/precompiles/sha256.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/rlp/accounts.py` & `py-evm-0.7.0a1/eth/rlp/accounts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/rlp/blocks.py` & `py-evm-0.7.0a1/eth/rlp/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/rlp/headers.py` & `py-evm-0.7.0a1/eth/rlp/headers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import (
+    Optional,
     cast,
     overload,
 )
 
 import rlp
 from rlp.sedes import (
     big_endian_int,
@@ -174,7 +175,11 @@
         # validate_header stops trying to check the current header against a parent header.
         # Can someone trick us into following a high difficulty header with genesis parent hash?
         return self.parent_hash == GENESIS_PARENT_HASH and self.block_number == 0
 
     @property
     def base_fee_per_gas(self) -> int:
         raise AttributeError("Base fee per gas not available until London fork")
+
+    @property
+    def withdrawals_root(self) -> Optional[Hash32]:
+        raise AttributeError("Withdrawals root not available until Shanghai fork")
```

### Comparing `py-evm-0.6.1a2/eth/rlp/logs.py` & `py-evm-0.7.0a1/eth/rlp/logs.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/rlp/receipts.py` & `py-evm-0.7.0a1/eth/rlp/receipts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/rlp/transactions.py` & `py-evm-0.7.0a1/eth/rlp/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/_utils/hashing.py` & `py-evm-0.7.0a1/eth/tools/_utils/hashing.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/_utils/mappings.py` & `py-evm-0.7.0a1/eth/tools/_utils/mappings.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/_utils/normalization.py` & `py-evm-0.7.0a1/eth/tools/_utils/normalization.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/_utils/slow_code_stream.py` & `py-evm-0.7.0a1/eth/tools/_utils/slow_code_stream.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/_utils/vyper.py` & `py-evm-0.7.0a1/eth/tools/_utils/vyper.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/builder/chain/__init__.py` & `py-evm-0.7.0a1/eth/tools/builder/chain/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     istanbul_at,
     muir_glacier_at,
     berlin_at,
     london_at,
     arrow_glacier_at,
     gray_glacier_at,
     paris_at,
+    shanghai_at,
     latest_mainnet_at,
 )
 
 
 mining_mainnet_fork_at_fns = (
     byzantium_at,
     frontier_at,
@@ -47,14 +48,15 @@
     berlin_at,
     london_at,
     arrow_glacier_at,
     gray_glacier_at,
 )
 pos_mainnet_fork_at_fns = (
     paris_at,
+    shanghai_at,
 )
 mainnet_fork_at_fns = mining_mainnet_fork_at_fns + pos_mainnet_fork_at_fns
 
 
 class API:
     #
     # Chain Class Construction
@@ -82,14 +84,15 @@
     istanbul_at = staticmethod(istanbul_at)
     muir_glacier_at = staticmethod(muir_glacier_at)
     berlin_at = staticmethod(berlin_at)
     london_at = staticmethod(london_at)
     arrow_glacier_at = staticmethod(arrow_glacier_at)
     gray_glacier_at = staticmethod(gray_glacier_at)
     paris_at = staticmethod(paris_at)
+    shanghai_at = staticmethod(shanghai_at)
 
     # iterable of the fork specific functions
     mainnet_fork_at_fns = mainnet_fork_at_fns
     mining_mainnet_fork_at_fns = mining_mainnet_fork_at_fns
 
     # DAO Fork specific
     dao_fork_at = staticmethod(dao_fork_at)
```

### Comparing `py-evm-0.6.1a2/eth/tools/builder/chain/builders.py` & `py-evm-0.7.0a1/eth/tools/builder/chain/builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     IstanbulVM,
     MuirGlacierVM,
     BerlinVM,
     LondonVM,
     ArrowGlacierVM,
     GrayGlacierVM,
     ParisVM,
+    ShanghaiVM,
 )
 
 
 def build(obj: Any, *applicators: Callable[..., Any]) -> Any:
     """
     Run the provided object through the series of applicator functions.
 
@@ -246,16 +247,17 @@
 istanbul_at = fork_at(IstanbulVM)
 muir_glacier_at = fork_at(MuirGlacierVM)
 berlin_at = fork_at(BerlinVM)
 london_at = fork_at(LondonVM)
 arrow_glacier_at = fork_at(ArrowGlacierVM)
 gray_glacier_at = fork_at(GrayGlacierVM)
 paris_at = fork_at(ParisVM)
+shanghai_at = fork_at(ShanghaiVM)
 
-latest_mainnet_at = paris_at
+latest_mainnet_at = shanghai_at
 
 GENESIS_DEFAULTS = cast(
     Tuple[Tuple[str, Union[BlockNumber, int, None, bytes, Address, Hash32]], ...],
     # values that will automatically be default are commented out
     (
         ('difficulty', 1),
         ('extra_data', constants.GENESIS_EXTRA_DATA),
```

### Comparing `py-evm-0.6.1a2/eth/tools/db/atomic.py` & `py-evm-0.7.0a1/eth/tools/db/atomic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/db/base.py` & `py-evm-0.7.0a1/eth/tools/db/base.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/fixtures/__init__.py` & `py-evm-0.7.0a1/eth/tools/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/fixtures/_utils.py` & `py-evm-0.7.0a1/eth/tools/fixtures/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/fixtures/fillers/_utils.py` & `py-evm-0.7.0a1/eth/tools/fixtures/fillers/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/fixtures/fillers/common.py` & `py-evm-0.7.0a1/eth/tools/fixtures/fillers/common.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/fixtures/fillers/formatters.py` & `py-evm-0.7.0a1/eth/tools/fixtures/fillers/formatters.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/fixtures/fillers/main.py` & `py-evm-0.7.0a1/eth/tools/fixtures/fillers/main.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/fixtures/fillers/state.py` & `py-evm-0.7.0a1/eth/tools/fixtures/fillers/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/fixtures/fillers/vm.py` & `py-evm-0.7.0a1/eth/tools/fixtures/fillers/vm.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/fixtures/generation.py` & `py-evm-0.7.0a1/eth/tools/fixtures/generation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/fixtures/helpers.py` & `py-evm-0.7.0a1/eth/tools/fixtures/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     HomesteadVM as BaseHomesteadVM,
     SpuriousDragonVM,
     IstanbulVM,
     BerlinVM,
     LondonVM,
     GrayGlacierVM,
     ParisVM,
+    ShanghaiVM,
 )
 
 
 #
 # State Setup
 #
 def setup_state(desired_state: AccountState, state: StateAPI) -> None:
@@ -142,14 +143,18 @@
         return (
             (0, LondonVM),
         )
     elif network == 'Merge':
         return (
             (0, ParisVM),
         )
+    elif network == "Shanghai":
+        return (
+            (0, ShanghaiVM),
+        )
     elif network == 'FrontierToHomesteadAt5':
         HomesteadVM = BaseHomesteadVM.configure(support_dao_fork=False)
         return (
             (0, FrontierVM),
             (5, HomesteadVM),
         )
     elif network == 'HomesteadToEIP150At5':
@@ -186,14 +191,20 @@
         return (
             # These tests were written before Gray Glacier was a thing. Use
             # GrayGlacierVM instead since that's when PoW -> PoS transition happens.
             # They should both pass but this is the more logical transition to test.
             (0, GrayGlacierVM),
             (6, ParisVM),
         )
+    elif network == "MergeToShanghaiAtTime15k":
+        # Transition expected at 5 (timestamp==15000) for all tests written thus far
+        return (
+            (0, ParisVM),
+            (5, ShanghaiVM),
+        )
 
     else:
         raise ValueError(f"Network {network} does not match any known VM rules")
 
 
 def genesis_fields_from_fixture(fixture: Dict[str, Any]) -> Dict[str, Any]:
     """
```

### Comparing `py-evm-0.6.1a2/eth/tools/fixtures/loading.py` & `py-evm-0.7.0a1/eth/tools/fixtures/loading.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/tools/mining.py` & `py-evm-0.7.0a1/eth/tools/mining.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/typing.py` & `py-evm-0.7.0a1/eth/typing.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,29 +22,41 @@
     HexStr,
 )
 from mypy_extensions import (
     TypedDict,
 )
 
 if TYPE_CHECKING:
-    from eth.abc import VirtualMachineAPI  # noqa: F401
+    from eth.abc import (  # noqa: F401
+        BlockHeaderAPI,
+        SignedTransactionAPI,
+        VirtualMachineAPI,
+        WithdrawalAPI,
+    )
 
 
 JournalDBCheckpoint = NewType('JournalDBCheckpoint', int)
 
 AccountDetails = TypedDict('AccountDetails',
                            {'balance': int,
                             'nonce': int,
                             'code': bytes,
                             'storage': Dict[int, int]
                             })
 AccountState = Dict[Address, AccountDetails]
-
 AccountDiff = Iterable[Tuple[Address, str, Union[int, bytes], Union[int, bytes]]]
 
+
+class Block(TypedDict, total=False):
+    header: "BlockHeaderAPI"
+    transactions: Sequence["SignedTransactionAPI"]
+    uncles: Sequence["BlockHeaderAPI"]
+    withdrawals: Sequence["WithdrawalAPI"]
+
+
 BlockRange = Tuple[BlockNumber, BlockNumber]
 
 ChainGaps = Tuple[
     # series of gaps before the chain head
     Tuple[BlockRange, ...],
     # the first missing block number at the tip of the chain
     BlockNumber,
```

### Comparing `py-evm-0.6.1a2/eth/validation.py` & `py-evm-0.7.0a1/eth/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,30 +149,30 @@
         )
     if value < 0:
         raise ValidationError(
             f"{title} cannot be negative: Got: {value}"
         )
     if value > UINT_64_MAX:
         raise ValidationError(
-            f"{title} exeeds maximum UINT256 size.  Got: {value}"
+            f"{title} exceeds maximum uint64 size.  Got: {value}"
         )
 
 
 def validate_uint256(value: int, title: str = "Value") -> None:
     if not isinstance(value, int) or isinstance(value, bool):
         raise ValidationError(
             f"{title} must be an integer: Got: {type(value)}"
         )
     if value < 0:
         raise ValidationError(
             f"{title} cannot be negative: Got: {value}"
         )
     if value > UINT_256_MAX:
         raise ValidationError(
-            f"{title} exceeds maximum UINT256 size.  Got: {value}"
+            f"{title} exceeds maximum uint256 size.  Got: {value}"
         )
 
 
 def validate_stack_int(value: int) -> None:
     if 0 <= value <= UINT_256_MAX:
         return
     raise ValidationError(
@@ -271,14 +271,15 @@
     'timestamp',
     'extra_data',
     'mix_hash',
     'nonce',
     'uncles_hash',
     'transaction_root',
     'receipt_root',
+    'withdrawals_root',
 }
 
 
 def validate_header_params_for_configuration(header_params: Dict[str, Any]) -> None:
     extra_fields = set(header_params.keys()).difference(ALLOWED_HEADER_FIELDS)
     if extra_fields:
         raise ValidationError(
```

### Comparing `py-evm-0.6.1a2/eth/vm/base.py` & `py-evm-0.7.0a1/eth/vm/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import contextlib
 import itertools
 import logging
 from typing import (
+    TYPE_CHECKING,
     Any,
     ClassVar,
     Iterable,
     Iterator,
+    List,
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     Union,
 )
@@ -40,14 +42,15 @@
     ReceiptAPI,
     ReceiptBuilderAPI,
     SignedTransactionAPI,
     StateAPI,
     TransactionBuilderAPI,
     UnsignedTransactionAPI,
     VirtualMachineAPI,
+    WithdrawalAPI,
 )
 from eth.consensus.pow import (
     PowConsensus,
 )
 from eth.constants import (
     GENESIS_PARENT_HASH,
     MAX_PREV_HEADER_DEPTH,
@@ -80,14 +83,19 @@
 from eth.vm.interrupt import (
     EVMMissingData,
 )
 from eth.vm.message import (
     Message,
 )
 
+if TYPE_CHECKING:
+    from eth.typing import (  # noqa: F401
+        Block,
+    )
+
 
 class VM(Configurable, VirtualMachineAPI):
     block_class: Type[BlockAPI] = None
     consensus_class: Type[ConsensusAPI] = PowConsensus
     extra_data_max_bytes: ClassVar[int] = 32
     fork: str = None
     chaindb: ChainDatabaseAPI = None
@@ -286,87 +294,144 @@
 
         receipts_tuple = tuple(receipts)
         computations_tuple = tuple(computations)
 
         return result_header, receipts_tuple, computations_tuple
 
     #
+    # Withdrawals
+    #
+    def apply_withdrawal(
+        self,
+        withdrawal: WithdrawalAPI,
+    ) -> None:
+        self.state.apply_withdrawal(withdrawal)
+
+    def apply_all_withdrawals(self, withdrawals: Sequence[WithdrawalAPI]) -> None:
+        touched_addresses: List[Address] = []
+
+        for withdrawal in withdrawals:
+            # validate withdrawal fields
+            withdrawal.validate()
+
+            self.apply_withdrawal(withdrawal)
+
+            # collect all touched addresses
+            if withdrawal.address not in touched_addresses:
+                touched_addresses.append(withdrawal.address)
+
+        for address in touched_addresses:
+            # if account is empty after applying all withdrawals, delete it
+            if self.state.account_is_empty(address):
+                self.state.delete_account(address)
+
+    #
     # Importing blocks
     #
     def import_block(self, block: BlockAPI) -> BlockAndMetaWitness:
         if self.get_block().number != block.number:
             raise ValidationError(
                 f"This VM can only import blocks at number #{self.get_block().number},"
                 f" the attempted block was #{block.number}"
             )
 
-        self._block = self.get_block().copy(
-            header=self.configure_header(
-                coinbase=block.header.coinbase,
-                difficulty=block.header.difficulty,
-                gas_limit=block.header.gas_limit,
-                timestamp=block.header.timestamp,
-                extra_data=block.header.extra_data,
-                mix_hash=block.header.mix_hash,
-                nonce=block.header.nonce,
-                uncles_hash=keccak(rlp.encode(block.uncles)),
-            ),
-            uncles=block.uncles,
-        )
+        header_params = {
+            "coinbase": block.header.coinbase,
+            "difficulty": block.header.difficulty,
+            "gas_limit": block.header.gas_limit,
+            "timestamp": block.header.timestamp,
+            "extra_data": block.header.extra_data,
+            "mix_hash": block.header.mix_hash,
+            "nonce": block.header.nonce,
+            "uncles_hash": keccak(rlp.encode(block.uncles)),
+        }
+
+        block_params = {
+            "header": self.configure_header(**header_params),
+            "uncles": block.uncles,
+        }
+
+        if hasattr(block, "withdrawals"):
+            # post-shanghai blocks
+            block_params["withdrawals"] = block.withdrawals
+
+        self._block = self.get_block().copy(**block_params)
 
         execution_context = self.create_execution_context(
             block.header, self.previous_hashes, self.chain_context
         )
 
-        # Zero out the gas_used before applying transactions. Each applied transaction will
-        #   increase the gas used in the final new_header.
+        # Zero out the gas_used before applying transactions. Each applied transaction
+        # will increase the gas used in the final new_header.
         header = self.get_header().copy(gas_used=0)
+
         # we need to re-initialize the `state` to update the execution context.
         self._state = self.get_state_class()(self.chaindb.db, execution_context, header.state_root)
 
         # run all of the transactions.
         new_header, receipts, _ = self.apply_all_transactions(block.transactions, header)
 
-        block_with_transactions = self.set_block_transactions(
+        withdrawals = block.withdrawals if hasattr(block, "withdrawals") else None
+
+        if withdrawals:
+            # post-shanghai blocks
+            self.apply_all_withdrawals(block.withdrawals)
+
+        filled_block = self.set_block_transactions_and_withdrawals(
             self.get_block(),
             new_header,
             block.transactions,
             receipts,
+            withdrawals=withdrawals,
         )
 
-        return self.mine_block(block_with_transactions)
+        return self.mine_block(filled_block)
 
     def mine_block(self, block: BlockAPI, *args: Any, **kwargs: Any) -> BlockAndMetaWitness:
         packed_block = self.pack_block(block, *args, **kwargs)
         block_result = self.finalize_block(packed_block)
 
         # Perform validation
         self.validate_block(block_result.block)
 
         return block_result
 
-    def set_block_transactions(self,
-                               base_block: BlockAPI,
-                               new_header: BlockHeaderAPI,
-                               transactions: Sequence[SignedTransactionAPI],
-                               receipts: Sequence[ReceiptAPI]) -> BlockAPI:
+    def set_block_transactions_and_withdrawals(
+        self,
+        base_block: BlockAPI,
+        new_header: BlockHeaderAPI,
+        transactions: Sequence[SignedTransactionAPI],
+        receipts: Sequence[ReceiptAPI],
+        withdrawals: Sequence[WithdrawalAPI] = None,
+    ) -> BlockAPI:
 
         tx_root_hash, tx_kv_nodes = make_trie_root_and_nodes(transactions)
         self.chaindb.persist_trie_data_dict(tx_kv_nodes)
 
         receipt_root_hash, receipt_kv_nodes = make_trie_root_and_nodes(receipts)
         self.chaindb.persist_trie_data_dict(receipt_kv_nodes)
 
-        return base_block.copy(
-            transactions=transactions,
-            header=new_header.copy(
-                transaction_root=tx_root_hash,
-                receipt_root=receipt_root_hash,
-            ),
-        )
+        block_fields: "Block" = {"transactions": transactions}
+        block_header_fields = {
+            "transaction_root": tx_root_hash,
+            "receipt_root": receipt_root_hash,
+        }
+
+        if withdrawals:
+            withdrawals_root_hash, withdrawal_kv_nodes = make_trie_root_and_nodes(
+                withdrawals,
+            )
+            self.chaindb.persist_trie_data_dict(withdrawal_kv_nodes)
+
+            block_fields["withdrawals"] = withdrawals
+            block_header_fields["withdrawals_root"] = withdrawals_root_hash
+
+        block_fields["header"] = new_header.copy(**block_header_fields)
+
+        return base_block.copy(**block_fields)
 
     #
     # Finalization
     #
     def _assign_block_rewards(self, block: BlockAPI) -> None:
         block_reward = self.get_block_reward() + (
             len(block.uncles) * self.get_nephew_reward()
@@ -436,14 +501,15 @@
             raise AttributeError(
                 f"Unable to set the field(s) {', '.join(known_fields)} "
                 "on the `BlockHeader` class. "
                 f"Received the following unexpected fields: {', '.join(unknown_fields)}."
             )
 
         header: BlockHeaderAPI = block.header.copy(**kwargs)
+
         packed_block = block.copy(uncles=uncles, header=header)
 
         return packed_block
 
     #
     # Blocks
     #
```

### Comparing `py-evm-0.6.1a2/eth/vm/chain_context.py` & `py-evm-0.7.0a1/eth/vm/chain_context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/code_stream.py` & `py-evm-0.7.0a1/eth/vm/code_stream.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/computation.py` & `py-evm-0.7.0a1/eth/vm/computation.py`

 * *Files 3% similar despite different names*

```diff
@@ -274,14 +274,22 @@
 
     def get_gas_remaining(self) -> int:
         if self.should_burn_gas:
             return 0
         else:
             return self._gas_meter.gas_remaining
 
+    @classmethod
+    def consume_initcode_gas_cost(cls, computation: ComputationAPI) -> None:
+        # this method does not become relevant until the Shanghai hard fork
+        """
+        Before starting the computation, consume initcode gas cost.
+        """
+        pass
+
     #
     # Stack management
     #
     def stack_swap(self, position: int) -> None:
         return self._stack.swap(position)
 
     def stack_dup(self, position: int) -> None:
@@ -512,19 +520,28 @@
 
         return None
 
     #
     # State Transition
     #
     @classmethod
-    def apply_computation(cls,
-                          state: StateAPI,
-                          message: MessageAPI,
-                          transaction_context: TransactionContextAPI) -> ComputationAPI:
+    def apply_computation(
+        cls,
+        state: StateAPI,
+        message: MessageAPI,
+        transaction_context: TransactionContextAPI
+    ) -> ComputationAPI:
+
         with cls(state, message, transaction_context) as computation:
+            if message.is_create and computation.is_origin_computation:
+                # If computation is from a create transaction, consume initcode gas if
+                # >= Shanghai. CREATE and CREATE2 are handled in the opcode
+                # implementations.
+                cls.consume_initcode_gas_cost(computation)
+
             # Early exit on pre-compiles
             precompile = computation.precompiles.get(message.code_address, NO_RESULT)
             if precompile is not NO_RESULT:
                 precompile(computation)
                 return computation
 
             show_debug2 = computation.logger.show_debug2
@@ -547,14 +564,15 @@
                         base_comp._stack,
                     )
 
                 try:
                     opcode_fn(computation=computation)
                 except Halt:
                     break
+
         return computation
 
     #
     # Opcode API
     #
     @property
     def precompiles(self) -> Dict[Address, Callable[[ComputationAPI], Any]]:
```

### Comparing `py-evm-0.6.1a2/eth/vm/execution_context.py` & `py-evm-0.7.0a1/eth/vm/execution_context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/__init__.py` & `py-evm-0.7.0a1/eth/vm/forks/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,7 +36,10 @@
 )
 from .gray_glacier import (  # noqa: F401
     GrayGlacierVM,
 )
 from .paris import (  # noqa: F401
     ParisVM,
 )
+from .shanghai import (  # noqa: F401
+    ShanghaiVM,
+)
```

### Comparing `py-evm-0.6.1a2/eth/vm/forks/arrow_glacier/__init__.py` & `py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/arrow_glacier/blocks.py` & `py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/arrow_glacier/headers.py` & `py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     compute_difficulty,
 )
 from eth.vm.forks.byzantium.headers import (
     configure_header,
 )
 
 compute_arrow_glacier_difficulty = compute_difficulty(10_700_000)
-configure_arrow_glacier_header = configure_header(compute_arrow_glacier_difficulty)
+configure_arrow_glacier_header = configure_header(difficulty_fn=compute_arrow_glacier_difficulty)
 
 
 @curry
 def create_arrow_glacier_header_from_parent(
     difficulty_fn: Callable[[BlockHeaderAPI, int], int],
     parent_header: Optional[BlockHeaderAPI],
     **header_params: Any
```

### Comparing `py-evm-0.6.1a2/eth/vm/forks/arrow_glacier/transactions.py` & `py-evm-0.7.0a1/eth/vm/forks/arrow_glacier/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/berlin/__init__.py` & `py-evm-0.7.0a1/eth/vm/forks/berlin/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/berlin/blocks.py` & `py-evm-0.7.0a1/eth/vm/forks/berlin/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/berlin/computation.py` & `py-evm-0.7.0a1/eth/vm/forks/berlin/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/berlin/logic.py` & `py-evm-0.7.0a1/eth/vm/forks/berlin/logic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/berlin/opcodes.py` & `py-evm-0.7.0a1/eth/vm/forks/berlin/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/berlin/receipts.py` & `py-evm-0.7.0a1/eth/vm/forks/berlin/receipts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/berlin/state.py` & `py-evm-0.7.0a1/eth/vm/forks/berlin/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/berlin/transactions.py` & `py-evm-0.7.0a1/eth/vm/forks/berlin/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/byzantium/__init__.py` & `py-evm-0.7.0a1/eth/vm/forks/byzantium/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/byzantium/computation.py` & `py-evm-0.7.0a1/eth/vm/forks/byzantium/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/byzantium/headers.py` & `py-evm-0.7.0a1/eth/vm/forks/byzantium/headers.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,33 +88,35 @@
             parent_header,
             header_params['timestamp'],
         )
     return create_frontier_header_from_parent(parent_header, **header_params)
 
 
 @curry
-def configure_header(difficulty_fn: Callable[[BlockHeaderAPI, int], int],
-                     vm: VirtualMachineAPI,
-                     **header_params: Any) -> BlockHeaderAPI:
+def configure_header(
+    vm: VirtualMachineAPI,
+    difficulty_fn: Callable[[BlockHeaderAPI, int], int] = None,
+    **header_params: Any,
+) -> BlockHeaderAPI:
     validate_header_params_for_configuration(header_params)
 
     with vm.get_header().build_changeset(**header_params) as changeset:
         if (
             'timestamp' in header_params
             and changeset.block_number > 0
 
-            # check that we are pre-PoS and not using a constant for the difficulty
-            and not isinstance(difficulty_fn, int)
+            # post-POS does not use difficulty_fn
+            and difficulty_fn is not None
         ):
             parent_header = get_parent_header(changeset.build_rlp(), vm.chaindb)
             changeset.difficulty = difficulty_fn(
                 parent_header,
                 header_params['timestamp'],
             )
 
         header = changeset.commit()
     return header
 
 
 compute_byzantium_difficulty = compute_difficulty(3000000)
 create_byzantium_header_from_parent = create_header_from_parent(compute_byzantium_difficulty)
-configure_byzantium_header = configure_header(compute_byzantium_difficulty)
+configure_byzantium_header = configure_header(difficulty_fn=compute_byzantium_difficulty)
```

### Comparing `py-evm-0.6.1a2/eth/vm/forks/byzantium/opcodes.py` & `py-evm-0.7.0a1/eth/vm/forks/byzantium/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/byzantium/transactions.py` & `py-evm-0.7.0a1/eth/vm/forks/byzantium/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/constantinople/__init__.py` & `py-evm-0.7.0a1/eth/vm/forks/constantinople/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/constantinople/computation.py` & `py-evm-0.7.0a1/eth/vm/forks/constantinople/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/constantinople/opcodes.py` & `py-evm-0.7.0a1/eth/vm/forks/constantinople/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/constantinople/transactions.py` & `py-evm-0.7.0a1/eth/vm/forks/constantinople/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/frontier/__init__.py` & `py-evm-0.7.0a1/eth/vm/forks/frontier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/frontier/blocks.py` & `py-evm-0.7.0a1/eth/vm/forks/frontier/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/frontier/computation.py` & `py-evm-0.7.0a1/eth/vm/forks/frontier/computation.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,18 +46,19 @@
     """
     # Override
     opcodes = FRONTIER_OPCODES
     _precompiles = FRONTIER_PRECOMPILES     # type: ignore # https://github.com/python/mypy/issues/708 # noqa: E501
 
     @classmethod
     def apply_message(
-            cls,
-            state: StateAPI,
-            message: MessageAPI,
-            transaction_context: TransactionContextAPI) -> ComputationAPI:
+        cls,
+        state: StateAPI,
+        message: MessageAPI,
+        transaction_context: TransactionContextAPI,
+    ) -> ComputationAPI:
 
         snapshot = state.snapshot()
 
         if message.depth > STACK_DEPTH_LIMIT:
             raise StackDepthLimit("Stack depth limit reached")
 
         if message.should_transfer_value and message.value:
```

### Comparing `py-evm-0.6.1a2/eth/vm/forks/frontier/headers.py` & `py-evm-0.7.0a1/eth/vm/forks/frontier/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/frontier/opcodes.py` & `py-evm-0.7.0a1/eth/vm/forks/frontier/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/frontier/state.py` & `py-evm-0.7.0a1/eth/vm/forks/frontier/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/frontier/transactions.py` & `py-evm-0.7.0a1/eth/vm/forks/frontier/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/frontier/validation.py` & `py-evm-0.7.0a1/eth/vm/forks/frontier/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/gray_glacier/__init__.py` & `py-evm-0.7.0a1/eth/vm/forks/gray_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/gray_glacier/blocks.py` & `py-evm-0.7.0a1/eth/vm/forks/gray_glacier/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/gray_glacier/headers.py` & `py-evm-0.7.0a1/eth/vm/forks/gray_glacier/headers.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     compute_difficulty,
 )
 from eth.vm.forks.byzantium.headers import (
     configure_header,
 )
 
 compute_gray_glacier_difficulty = compute_difficulty(11_400_000)
-configure_gray_glacier_header = configure_header(compute_gray_glacier_difficulty)
+configure_gray_glacier_header = configure_header(difficulty_fn=compute_gray_glacier_difficulty)
 
 
 @curry
 def create_gray_glacier_header_from_parent(
     difficulty_fn: Callable[[BlockHeaderAPI, int], int],
     parent_header: Optional[BlockHeaderAPI],
     **header_params: Any
```

### Comparing `py-evm-0.6.1a2/eth/vm/forks/gray_glacier/transactions.py` & `py-evm-0.7.0a1/eth/vm/forks/gray_glacier/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/homestead/__init__.py` & `py-evm-0.7.0a1/eth/vm/forks/homestead/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/homestead/computation.py` & `py-evm-0.7.0a1/eth/vm/forks/homestead/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/homestead/headers.py` & `py-evm-0.7.0a1/eth/vm/forks/homestead/headers.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/homestead/opcodes.py` & `py-evm-0.7.0a1/eth/vm/forks/homestead/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/homestead/state.py` & `py-evm-0.7.0a1/eth/vm/forks/homestead/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/homestead/transactions.py` & `py-evm-0.7.0a1/eth/vm/forks/homestead/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/homestead/validation.py` & `py-evm-0.7.0a1/eth/vm/forks/homestead/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/istanbul/__init__.py` & `py-evm-0.7.0a1/eth/vm/forks/istanbul/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/istanbul/computation.py` & `py-evm-0.7.0a1/eth/vm/forks/istanbul/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/istanbul/opcodes.py` & `py-evm-0.7.0a1/eth/vm/forks/istanbul/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/istanbul/storage.py` & `py-evm-0.7.0a1/eth/vm/forks/istanbul/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/istanbul/transactions.py` & `py-evm-0.7.0a1/eth/vm/forks/istanbul/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/london/__init__.py` & `py-evm-0.7.0a1/eth/vm/forks/london/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/london/blocks.py` & `py-evm-0.7.0a1/eth/vm/forks/london/blocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import (
     List,
+    Optional,
     Type,
     cast,
 )
 
 from eth_hash.auto import keccak
 from eth_typing import (
     BlockNumber,
@@ -155,14 +156,18 @@
     @property
     def is_genesis(self) -> bool:
         # if removing the block_number == 0 test, consider the validation consequences.
         # validate_header stops trying to check the current header against a parent header.
         # Can someone trick us into following a high difficulty header with genesis parent hash?
         return self.parent_hash == GENESIS_PARENT_HASH and self.block_number == 0
 
+    @property
+    def withdrawals_root(self) -> Optional[Hash32]:
+        raise AttributeError("Withdrawals root not available until Shanghai fork")
+
 
 class LondonBackwardsHeader(BlockHeaderSedesAPI):
     """
     An rlp sedes class for block headers.
 
     It can serialize and deserialize *both* London and pre-London headers.
     """
```

### Comparing `py-evm-0.6.1a2/eth/vm/forks/london/computation.py` & `py-evm-0.7.0a1/eth/vm/forks/london/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/london/headers.py` & `py-evm-0.7.0a1/eth/vm/forks/london/headers.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             )
 
     new_header = LondonBlockHeader(**all_fields)  # type:ignore
     return new_header
 
 
 compute_london_difficulty = compute_difficulty(9700000)
-configure_london_header = configure_header(compute_london_difficulty)
+configure_london_header = configure_header(difficulty_fn=compute_london_difficulty)
 
 
 class LondonBackwardsHeader(BlockHeaderSedesAPI):
     """
     An rlp sedes class for block headers.
 
     It can serialize and deserialize *both* London and pre-London headers.
```

### Comparing `py-evm-0.6.1a2/eth/vm/forks/london/opcodes.py` & `py-evm-0.7.0a1/eth/vm/forks/london/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/london/receipts.py` & `py-evm-0.7.0a1/eth/vm/forks/london/receipts.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/london/state.py` & `py-evm-0.7.0a1/eth/vm/forks/london/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/london/storage.py` & `py-evm-0.7.0a1/eth/vm/forks/london/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/london/transactions.py` & `py-evm-0.7.0a1/eth/vm/forks/london/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/london/validation.py` & `py-evm-0.7.0a1/eth/vm/forks/london/validation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/muir_glacier/__init__.py` & `py-evm-0.7.0a1/eth/vm/forks/muir_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/muir_glacier/computation.py` & `py-evm-0.7.0a1/eth/vm/forks/muir_glacier/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/muir_glacier/transactions.py` & `py-evm-0.7.0a1/eth/vm/forks/muir_glacier/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/paris/__init__.py` & `py-evm-0.7.0a1/eth/vm/forks/paris/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     # classes
     block_class: Type[BaseBlock] = ParisBlock
     _state_class: Type[BaseState] = ParisState
     consensus_class: Type[ConsensusAPI] = PosConsensus
 
     # Methods
     create_header_from_parent = staticmethod(  # type: ignore
-        create_paris_header_from_parent(POST_MERGE_DIFFICULTY)
+        create_paris_header_from_parent()
     )
     configure_header = configure_paris_header
 
     @staticmethod
     def get_block_reward() -> int:
         return 0
```

### Comparing `py-evm-0.6.1a2/eth/vm/forks/paris/blocks.py` & `py-evm-0.7.0a1/eth/vm/forks/paris/blocks.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/paris/headers.py` & `py-evm-0.7.0a1/eth/vm/forks/paris/headers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Optional
+from typing import Any, Optional
 
 from toolz import curry
 
 from eth.abc import BlockHeaderAPI
 from eth.constants import (
     POST_MERGE_DIFFICULTY,
     POST_MERGE_MIX_HASH,
@@ -32,15 +32,14 @@
             f"{constant_value}, got: {actual}"
         )
     return constant_value
 
 
 @curry
 def create_paris_header_from_parent(
-    _difficulty_fn: Callable[[BlockHeaderAPI, int], int],
     parent_header: Optional[BlockHeaderAPI],
     **header_params: Any,
 ) -> BlockHeaderAPI:
     # `mix_hash` is not strictly validated; take the value from the `header_params`,
     # if present; else, set to the EIP-3675-defined constant value.
     header_params["mix_hash"] = header_params.get("mix_hash", POST_MERGE_MIX_HASH)
 
@@ -59,8 +58,8 @@
 
     # extract params validated up to gray glacier (previous VM)
     # and plug into a `ParisBlockHeader` class
     all_fields = gray_glacier_validated_header.as_dict()
     return ParisBlockHeader(**all_fields)
 
 
-configure_paris_header = configure_header(POST_MERGE_DIFFICULTY)
+configure_paris_header = configure_header()
```

### Comparing `py-evm-0.6.1a2/eth/vm/forks/paris/opcodes.py` & `py-evm-0.7.0a1/eth/vm/forks/paris/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/paris/state.py` & `py-evm-0.7.0a1/eth/vm/forks/paris/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/paris/transactions.py` & `py-evm-0.7.0a1/eth/vm/forks/paris/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/petersburg/__init__.py` & `py-evm-0.7.0a1/eth/vm/forks/petersburg/__init__.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/petersburg/computation.py` & `py-evm-0.7.0a1/eth/vm/forks/petersburg/computation.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/petersburg/opcodes.py` & `py-evm-0.7.0a1/eth/vm/forks/petersburg/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/petersburg/transactions.py` & `py-evm-0.7.0a1/eth/vm/forks/petersburg/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/spurious_dragon/_utils.py` & `py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/_utils.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/spurious_dragon/computation.py` & `py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/computation.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,16 @@
             transaction_context: TransactionContextAPI) -> ComputationAPI:
 
         snapshot = state.snapshot()
 
         # EIP161 nonce incrementation
         state.increment_nonce(message.storage_address)
 
+        cls.validate_create_message(message)
+
         computation = cls.apply_message(state, message, transaction_context)
 
         if computation.is_error:
             state.revert(snapshot)
             return computation
         else:
             contract_code = computation.output
@@ -78,13 +80,21 @@
                     state.set_code(message.storage_address, contract_code)
                     state.commit(snapshot)
             else:
                 state.commit(snapshot)
             return computation
 
     @classmethod
+    def validate_create_message(cls, message: MessageAPI) -> None:
+        # this method does not become relevant until the Shanghai hard fork
+        """
+        Class method for validating a create message.
+        """
+        pass
+
+    @classmethod
     def validate_contract_code(cls, contract_code: bytes) -> None:
-        if len(contract_code) >= EIP170_CODE_SIZE_LIMIT:
+        if len(contract_code) > EIP170_CODE_SIZE_LIMIT:
             raise OutOfGas(
                 f"Contract code size exceeds EIP170 limit of {EIP170_CODE_SIZE_LIMIT}."
                 f"  Got code of size: {len(contract_code)}"
             )
```

### Comparing `py-evm-0.6.1a2/eth/vm/forks/spurious_dragon/opcodes.py` & `py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/spurious_dragon/state.py` & `py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/state.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/spurious_dragon/transactions.py` & `py-evm-0.7.0a1/eth/vm/forks/spurious_dragon/transactions.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/forks/tangerine_whistle/opcodes.py` & `py-evm-0.7.0a1/eth/vm/forks/tangerine_whistle/opcodes.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/gas_meter.py` & `py-evm-0.7.0a1/eth/vm/gas_meter.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/interrupt.py` & `py-evm-0.7.0a1/eth/vm/interrupt.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/logic/arithmetic.py` & `py-evm-0.7.0a1/eth/vm/logic/arithmetic.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/logic/block.py` & `py-evm-0.7.0a1/eth/vm/logic/block.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/logic/call.py` & `py-evm-0.7.0a1/eth/vm/logic/call.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/logic/comparison.py` & `py-evm-0.7.0a1/eth/vm/logic/comparison.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/logic/context.py` & `py-evm-0.7.0a1/eth/vm/logic/context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/logic/duplication.py` & `py-evm-0.7.0a1/eth/vm/logic/duplication.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/logic/flow.py` & `py-evm-0.7.0a1/eth/vm/logic/flow.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/logic/logging.py` & `py-evm-0.7.0a1/eth/vm/logic/logging.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/logic/memory.py` & `py-evm-0.7.0a1/eth/vm/logic/memory.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/logic/sha3.py` & `py-evm-0.7.0a1/eth/vm/logic/sha3.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/logic/stack.py` & `py-evm-0.7.0a1/eth/vm/logic/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     if raw_len == size:
         computation.stack_push_bytes(raw_value)
     else:
         padded_value = raw_value.ljust(size, b'\x00')
         computation.stack_push_bytes(padded_value)
 
 
+push0 = functools.partial(push_XX, size=0)
 push1 = functools.partial(push_XX, size=1)
 push2 = functools.partial(push_XX, size=2)
 push3 = functools.partial(push_XX, size=3)
 push4 = functools.partial(push_XX, size=4)
 push5 = functools.partial(push_XX, size=5)
 push6 = functools.partial(push_XX, size=6)
 push7 = functools.partial(push_XX, size=7)
```

### Comparing `py-evm-0.6.1a2/eth/vm/logic/storage.py` & `py-evm-0.7.0a1/eth/vm/logic/storage.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/logic/swap.py` & `py-evm-0.7.0a1/eth/vm/logic/swap.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/logic/system.py` & `py-evm-0.7.0a1/eth/vm/logic/system.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/memory.py` & `py-evm-0.7.0a1/eth/vm/memory.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/message.py` & `py-evm-0.7.0a1/eth/vm/message.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/mnemonics.py` & `py-evm-0.7.0a1/eth/vm/mnemonics.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 MSIZE = 'MSIZE'
 GAS = 'GAS'
 JUMPDEST = 'JUMPDEST'
 REVERT = 'REVERT'
 #
 # Push Operations
 #
+PUSH0 = 'PUSH0'
 PUSH1 = 'PUSH1'
 PUSH2 = 'PUSH2'
 PUSH3 = 'PUSH3'
 PUSH4 = 'PUSH4'
 PUSH5 = 'PUSH5'
 PUSH6 = 'PUSH6'
 PUSH7 = 'PUSH7'
```

### Comparing `py-evm-0.6.1a2/eth/vm/opcode.py` & `py-evm-0.7.0a1/eth/vm/opcode.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/opcode_values.py` & `py-evm-0.7.0a1/eth/vm/opcode_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 GAS = 0x5a
 JUMPDEST = 0x5b
 
 
 #
 # Push Operations
 #
+PUSH0 = 0x5f
 PUSH1 = 0x60
 PUSH2 = 0x61
 PUSH3 = 0x62
 PUSH4 = 0x63
 PUSH5 = 0x64
 PUSH6 = 0x65
 PUSH7 = 0x66
```

### Comparing `py-evm-0.6.1a2/eth/vm/stack.py` & `py-evm-0.7.0a1/eth/vm/stack.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/eth/vm/state.py` & `py-evm-0.7.0a1/eth/vm/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import contextlib
 from typing import (
     Iterator,
+    Sequence,
     Tuple,
     Type,
 )
 
 from eth_typing import (
     Address,
     BlockNumber,
@@ -23,14 +24,15 @@
     ExecutionContextAPI,
     MessageAPI,
     SignedTransactionAPI,
     StateAPI,
     TransactionContextAPI,
     TransactionExecutorAPI,
     MetaWitnessAPI,
+    WithdrawalAPI,
 )
 from eth.constants import (
     MAX_PREV_HEADER_DEPTH,
 )
 from eth.typing import JournalDBCheckpoint
 from eth._utils.datatypes import (
     Configurable,
@@ -286,14 +288,26 @@
     def get_transaction_context(self,
                                 transaction: SignedTransactionAPI) -> TransactionContextAPI:
         return self.get_transaction_context_class()(
             gas_price=transaction.gas_price,
             origin=transaction.sender,
         )
 
+    #
+    # Withdrawals
+    #
+
+    def apply_withdrawal(self, withdrawal: WithdrawalAPI) -> None:
+        # withdrawals not implemented until the Shanghai hard fork
+        pass
+
+    def apply_all_withdrawals(self, withdrawals: Sequence[WithdrawalAPI]) -> None:
+        # withdrawals not implemented until the Shanghai hard fork
+        pass
+
 
 class BaseTransactionExecutor(TransactionExecutorAPI):
     def __init__(self, vm_state: StateAPI) -> None:
         self.vm_state = vm_state
 
     def __call__(self, transaction: SignedTransactionAPI) -> ComputationAPI:
         self.validate_transaction(transaction)
```

### Comparing `py-evm-0.6.1a2/eth/vm/transaction_context.py` & `py-evm-0.7.0a1/eth/vm/transaction_context.py`

 * *Files identical despite different names*

### Comparing `py-evm-0.6.1a2/py_evm.egg-info/PKG-INFO` & `py-evm-0.7.0a1/py_evm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-evm
-Version: 0.6.1a2
+Version: 0.7.0a1
 Summary: Python implementation of the Ethereum Virtual Machine
 Home-page: https://github.com/ethereum/py-evm
 Author: Ethereum Foundation
 Author-email: piper@pipermerriam.com
 License: MIT
 Keywords: ethereum blockchain evm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `py-evm-0.6.1a2/py_evm.egg-info/SOURCES.txt` & `py-evm-0.7.0a1/py_evm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 eth/rlp/receipts.py
 eth/rlp/sedes.py
 eth/rlp/transactions.py
 eth/tools/__init__.py
 eth/tools/mining.py
 eth/tools/rlp.py
 eth/tools/_utils/__init__.py
+eth/tools/_utils/deprecation.py
 eth/tools/_utils/git.py
 eth/tools/_utils/hashing.py
 eth/tools/_utils/mappings.py
 eth/tools/_utils/normalization.py
 eth/tools/_utils/slow_code_stream.py
 eth/tools/_utils/vyper.py
 eth/tools/builder/__init__.py
@@ -241,14 +242,24 @@
 eth/vm/forks/petersburg/blocks.py
 eth/vm/forks/petersburg/computation.py
 eth/vm/forks/petersburg/constants.py
 eth/vm/forks/petersburg/headers.py
 eth/vm/forks/petersburg/opcodes.py
 eth/vm/forks/petersburg/state.py
 eth/vm/forks/petersburg/transactions.py
+eth/vm/forks/shanghai/__init__.py
+eth/vm/forks/shanghai/blocks.py
+eth/vm/forks/shanghai/computation.py
+eth/vm/forks/shanghai/constants.py
+eth/vm/forks/shanghai/headers.py
+eth/vm/forks/shanghai/logic.py
+eth/vm/forks/shanghai/opcodes.py
+eth/vm/forks/shanghai/state.py
+eth/vm/forks/shanghai/transactions.py
+eth/vm/forks/shanghai/withdrawals.py
 eth/vm/forks/spurious_dragon/__init__.py
 eth/vm/forks/spurious_dragon/_utils.py
 eth/vm/forks/spurious_dragon/blocks.py
 eth/vm/forks/spurious_dragon/computation.py
 eth/vm/forks/spurious_dragon/constants.py
 eth/vm/forks/spurious_dragon/opcodes.py
 eth/vm/forks/spurious_dragon/state.py
```

### Comparing `py-evm-0.6.1a2/py_evm.egg-info/requires.txt` & `py-evm-0.7.0a1/py_evm.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cached-property<2,>=1.5.1
 eth-bloom>=1.0.3
 eth-keys<0.5.0,>=0.4.0
-eth-typing<4.0.0,>=3.2.0
+eth-typing<4.0.0,>=3.3.0
 eth-utils<3.0.0,>=2.0.0
 lru-dict>=1.1.6
 mypy_extensions<1.0.0,>=0.4.1
 py-ecc<7.0.0,>=1.4.7
 pyethash<1.0.0,>=0.1.27
 rlp<4,>=3
 trie<3,>=2.0.0
@@ -21,15 +21,15 @@
 idna==2.7
 requests<3,>=2.20
 tox==2.7.0
 twine
 cached-property<2,>=1.5.1
 eth-bloom>=1.0.3
 eth-keys<0.5.0,>=0.4.0
-eth-typing<4.0.0,>=3.2.0
+eth-typing<4.0.0,>=3.3.0
 eth-utils<3.0.0,>=2.0.0
 lru-dict>=1.1.6
 mypy_extensions<1.0.0,>=0.4.1
 py-ecc<7.0.0,>=1.4.7
 pyethash<1.0.0,>=0.1.27
 rlp<4,>=3
 trie<3,>=2.0.0
@@ -66,15 +66,15 @@
 sphinxcontrib-asyncio<0.4,>=0.2.0
 towncrier<22,>=21
 
 [eth]
 cached-property<2,>=1.5.1
 eth-bloom>=1.0.3
 eth-keys<0.5.0,>=0.4.0
-eth-typing<4.0.0,>=3.2.0
+eth-typing<4.0.0,>=3.3.0
 eth-utils<3.0.0,>=2.0.0
 lru-dict>=1.1.6
 mypy_extensions<1.0.0,>=0.4.1
 py-ecc<7.0.0,>=1.4.7
 pyethash<1.0.0,>=0.1.27
 rlp<4,>=3
 trie<3,>=2.0.0
```

### Comparing `py-evm-0.6.1a2/pyproject.toml` & `py-evm-0.7.0a1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,19 @@
 [[tool.towncrier.type]]
 directory = "removal"
 name = "Deprecations and Removals"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "internal"
-name = "Internal Changes - for Contributors"
+name = "Internal Changes - For Contributors"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "misc"
-name = "Miscellaneous internal changes"
+name = "Miscellaneous changes"
 showcontent = false
+
+[[tool.towncrier.type]]
+directory = "breaking"
+name = "Breaking changes"
+showcontent = true
```

### Comparing `py-evm-0.6.1a2/setup.py` & `py-evm-0.7.0a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 deps = {
     'eth': [
         "cached-property>=1.5.1,<2",
         "eth-bloom>=1.0.3",
         "eth-keys>=0.4.0,<0.5.0",
-        "eth-typing>=3.2.0,<4.0.0",
+        "eth-typing>=3.3.0,<4.0.0",
         "eth-utils>=2.0.0,<3.0.0",
         "lru-dict>=1.1.6",
         "mypy_extensions>=0.4.1,<1.0.0",
         "py-ecc>=1.4.7,<7.0.0",
         "pyethash>=0.1.27,<1.0.0",
         "rlp>=3,<4",
         "trie>=2.0.0,<3",
@@ -90,15 +90,15 @@
 
 with open('README.md') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='py-evm',
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version='0.6.1-alpha.2',
+    version='0.7.0-alpha.1',
     description='Python implementation of the Ethereum Virtual Machine',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ethereum Foundation',
     author_email='piper@pipermerriam.com',
     url='https://github.com/ethereum/py-evm',
     include_package_data=True,
```

