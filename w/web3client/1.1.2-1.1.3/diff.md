# Comparing `tmp/web3client-1.1.2.tar.gz` & `tmp/web3client-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3client-1.1.2.tar", last modified: Fri Apr  7 17:56:07 2023, max compression
+gzip compressed data, was "web3client-1.1.3.tar", last modified: Mon Apr 10 16:34:41 2023, max compression
```

## Comparing `web3client-1.1.2.tar` & `web3client-1.1.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     1069 2022-10-13 15:30:24.076003 web3client-1.1.2/LICENSE
--rw-r--r--   0        0        0     2647 2023-04-05 14:07:40.813589 web3client-1.1.2/README.md
--rw-r--r--   0        0        0     1983 2023-04-07 17:55:17.958503 web3client-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.879656 web3client-1.1.2/src/.DS_Store
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:28.884980 web3client-1.1.2/src/web3client/.DS_Store
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.603558 web3client-1.1.2/src/web3client/__init__.py
--rw-r--r--   0        0        0    11117 2022-10-18 14:47:37.604295 web3client-1.1.2/src/web3client/abi/erc20.json
--rw-r--r--   0        0        0    22535 2023-04-07 17:53:01.432987 web3client-1.1.2/src/web3client/base_client.py
--rw-r--r--   0        0        0     3320 2023-04-05 16:33:33.363845 web3client-1.1.2/src/web3client/erc20_client.py
--rw-r--r--   0        0        0      342 2022-10-19 17:40:52.208885 web3client-1.1.2/src/web3client/exceptions.py
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.604873 web3client-1.1.2/src/web3client/helpers/__init__.py
--rw-r--r--   0        0        0     1732 2023-02-13 20:06:35.817499 web3client-1.1.2/src/web3client/helpers/debug.py
--rw-r--r--   0        0        0     2438 2022-10-18 14:47:37.605628 web3client-1.1.2/src/web3client/helpers/general.py
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.601242 web3client-1.1.2/src/web3factory/__init__.py
--rw-r--r--   0        0        0     2190 2023-04-05 13:58:18.268337 web3client-1.1.2/src/web3factory/erc20_tokens.py
--rw-r--r--   0        0        0     1431 2023-02-13 20:30:39.832108 web3client-1.1.2/src/web3factory/factory.py
--rw-r--r--   0        0        0     2605 2023-04-05 13:58:18.268462 web3client-1.1.2/src/web3factory/networks.py
--rw-r--r--   0        0        0      621 2023-02-13 19:47:49.818983 web3client-1.1.2/src/web3factory/types.py
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.878800 web3client-1.1.2/tests/.DS_Store
--rw-r--r--   0        0        0        0 2023-02-23 10:04:23.399090 web3client-1.1.2/tests/__init__.py
--rw-r--r--   0        0        0     6148 2023-04-05 16:39:49.642961 web3client-1.1.2/tests/ape/.DS_Store
--rw-r--r--   0        0        0      779 2023-04-06 10:47:11.288879 web3client-1.1.2/tests/ape/.build/SafeMath.json
--rw-r--r--   0        0        0    14895 2023-04-06 10:47:11.290250 web3client-1.1.2/tests/ape/.build/Token.json
--rw-r--r--   0        0        0    20923 2023-04-07 17:55:22.865280 web3client-1.1.2/tests/ape/.build/__local__.json
--rw-r--r--   0        0        0      600 2023-02-23 10:18:28.269673 web3client-1.1.2/tests/ape/contracts/token/SafeMath.sol
--rw-r--r--   0        0        0     4082 2023-02-23 10:18:28.283242 web3client-1.1.2/tests/ape/contracts/token/Token.sol
--rw-r--r--   0        0        0     3529 2023-04-05 16:42:52.576613 web3client-1.1.2/tests/ape/fixtures.py
--rw-r--r--   0        0        0        0 2023-04-05 15:27:07.832128 web3client-1.1.2/tests/ape/scripts/__init__.py
--rw-r--r--   0        0        0      123 2023-04-05 14:37:05.616337 web3client-1.1.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-02-23 10:04:38.139397 web3client-1.1.2/tests/web3client/__init__.py
--rw-r--r--   0        0        0     1300 2023-04-06 11:08:05.647477 web3client-1.1.2/tests/web3client/fixtures.py
--rw-r--r--   0        0        0     1417 2023-02-13 20:04:46.649348 web3client-1.1.2/tests/web3client/test_networks.py
--rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 web3client-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-13 15:30:24.076003 web3client-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2647 2023-04-05 14:07:40.813589 web3client-1.1.3/README.md
+-rw-r--r--   0        0        0     1983 2023-04-10 16:33:25.656644 web3client-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.879656 web3client-1.1.3/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:28.884980 web3client-1.1.3/src/web3client/.DS_Store
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.603558 web3client-1.1.3/src/web3client/__init__.py
+-rw-r--r--   0        0        0    11117 2022-10-18 14:47:37.604295 web3client-1.1.3/src/web3client/abi/erc20.json
+-rw-r--r--   0        0        0    24177 2023-04-10 16:32:21.324544 web3client-1.1.3/src/web3client/base_client.py
+-rw-r--r--   0        0        0     3320 2023-04-05 16:33:33.363845 web3client-1.1.3/src/web3client/erc20_client.py
+-rw-r--r--   0        0        0      342 2022-10-19 17:40:52.208885 web3client-1.1.3/src/web3client/exceptions.py
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.604873 web3client-1.1.3/src/web3client/helpers/__init__.py
+-rw-r--r--   0        0        0     1732 2023-02-13 20:06:35.817499 web3client-1.1.3/src/web3client/helpers/debug.py
+-rw-r--r--   0        0        0     2438 2022-10-18 14:47:37.605628 web3client-1.1.3/src/web3client/helpers/general.py
+-rw-r--r--   0        0        0     1909 2023-04-10 15:26:30.878490 web3client-1.1.3/src/web3client/helpers/websockets.py
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.601242 web3client-1.1.3/src/web3factory/__init__.py
+-rw-r--r--   0        0        0     2190 2023-04-05 13:58:18.268337 web3client-1.1.3/src/web3factory/erc20_tokens.py
+-rw-r--r--   0        0        0     1431 2023-02-13 20:30:39.832108 web3client-1.1.3/src/web3factory/factory.py
+-rw-r--r--   0        0        0     2605 2023-04-05 13:58:18.268462 web3client-1.1.3/src/web3factory/networks.py
+-rw-r--r--   0        0        0      621 2023-02-13 19:47:49.818983 web3client-1.1.3/src/web3factory/types.py
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.878800 web3client-1.1.3/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2023-02-23 10:04:23.399090 web3client-1.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     6148 2023-04-05 16:39:49.642961 web3client-1.1.3/tests/ape/.DS_Store
+-rw-r--r--   0        0        0      779 2023-04-06 10:47:11.288879 web3client-1.1.3/tests/ape/.build/SafeMath.json
+-rw-r--r--   0        0        0    14895 2023-04-06 10:47:11.290250 web3client-1.1.3/tests/ape/.build/Token.json
+-rw-r--r--   0        0        0    20923 2023-04-10 16:33:31.235366 web3client-1.1.3/tests/ape/.build/__local__.json
+-rw-r--r--   0        0        0      600 2023-02-23 10:18:28.269673 web3client-1.1.3/tests/ape/contracts/token/SafeMath.sol
+-rw-r--r--   0        0        0     4082 2023-02-23 10:18:28.283242 web3client-1.1.3/tests/ape/contracts/token/Token.sol
+-rw-r--r--   0        0        0     3529 2023-04-05 16:42:52.576613 web3client-1.1.3/tests/ape/fixtures.py
+-rw-r--r--   0        0        0        0 2023-04-05 15:27:07.832128 web3client-1.1.3/tests/ape/scripts/__init__.py
+-rw-r--r--   0        0        0      123 2023-04-05 14:37:05.616337 web3client-1.1.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-02-23 10:04:38.139397 web3client-1.1.3/tests/web3client/__init__.py
+-rw-r--r--   0        0        0     1300 2023-04-06 11:08:05.647477 web3client-1.1.3/tests/web3client/fixtures.py
+-rw-r--r--   0        0        0     1417 2023-02-13 20:04:46.649348 web3client-1.1.3/tests/web3client/test_networks.py
+-rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 web3client-1.1.3/PKG-INFO
```

### Comparing `web3client-1.1.2/LICENSE` & `web3client-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/README.md` & `web3client-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/pyproject.toml` & `web3client-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "web3client"
-version = "1.1.2"
+version = "1.1.3"
 description = "Batteries-included client to interact with blockchains and smart contracts"
 authors = [
     { name = "coccoinomane", email = "coccoinomane@gmail.com" },
 ]
 readme = "README.md"
 keywords = [
     "web3",
```

### Comparing `web3client-1.1.2/src/.DS_Store` & `web3client-1.1.3/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/src/web3client/.DS_Store` & `web3client-1.1.3/src/web3client/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/src/web3client/abi/erc20.json` & `web3client-1.1.3/src/web3client/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/src/web3client/base_client.py` & `web3client-1.1.3/src/web3client/base_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import json
-from typing import Any, Callable, List, Tuple, Union, cast
+from typing import Any, Awaitable, Callable, List, Tuple, Union, cast
 
 from eth_account import Account
 from eth_account.datastructures import SignedMessage, SignedTransaction
 from eth_account.messages import encode_defunct
 from eth_account.signers.local import LocalAccount
 from eth_typing import Address
 from eth_typing.encoding import HexStr
@@ -22,14 +22,15 @@
     TxParams,
     TxReceipt,
     Wei,
 )
 from websockets.client import connect
 
 from web3client.exceptions import TransactionTooExpensive, Web3ClientException
+from web3client.helpers.websockets import parse_notification, subscribe_to_notification
 
 
 class BaseClient:
     """
     Client to interact with a blockchain, with smart contract
     support.
 
@@ -352,90 +353,123 @@
         )
         return signer_address == self.user_address
 
     ####################
     # Scan
     ####################
 
-    def subscribe_pending_txs(
+    def subscribe(
         self,
-        on_tx: Callable[[str], None],
-        on_subscribe: Callable[[str], None] = None,
+        on_notification: Callable[[Any], None],
+        on_subscribe: Callable[[Any], None] = None,
         once: bool = False,
         subscription_type: str = "newPendingTransactions",
     ) -> None:
-        """Asynchronously scan pending transactions with eth_subscribe and call the
-        given callback when one is found.
+        """Look for new pending transactions, blocks or events; when one is found,
+        call the 'on_notification' callback.
+
+        Notifications are processed one at a time; if you need concurrent execution,
+        use async_subscribe() instead.
+
+        Subscription types (same as eth_subscribe RPC method):
+
+         - Use 'newHeads' to listen to new blocks. The callback receives a dict with
+           the block parameters as argument.
+         - Use 'newPendingTransactions' to listen to pending transactions. The callback
+           receives the transaction hash as argument.
+         - Use 'logs' to listen to contract event logs. The callback receives a dict
+           with the smart contract address, block info and the 'data' field. [UNTESTED!]
+         - For a full reference, see https://geth.ethereum.org/docs/interacting-with-geth/rpc/pubsub
 
         Details:
-         - The callback is called with the transaction hash as argument.
-         - The subscription type is 'newPendingTransactions' by default.
-         - Provid once=True to stop the subscription after the first transaction is found.
+
+         - Provid once=True to stop the subscription after the first occurrency.
+         - If you use Alchemy, you might want to use 'alchemy_newPendingTransactions'
+           (https://docs.alchemy.com/reference/newpendingtransactions)
+         - Subscription is good to react fast to changes on the blockchain, but you might
+           miss some events. If you are ok with less but more reliable approach, use filters.
 
         Caveats:
+
          - The client must be configured with a websocket RPC endpoint (ws:// or wss://)
+           or a local IPC endpoint (ending in .ipc).
          - Not all chains support the 'newPendingTransactions' subscription type.
          - Not all chains have a mempool, e.g. Arbitrum. For these chains, the function will
-           just hang.
+           just hang if asking for 'newPendingTransactions'.
          - Some chains require a validator node with staked L1 funds to be able to
-           access to pending transactions in the mempool (e.g. Avalanche).
-         - If you use Alchemy, you might want to use 'alchemy_newPendingTransactions'
-           (https://docs.alchemy.com/reference/newpendingtransactions)
+           access to pending transactions while they are in the mempool (e.g. Avalanche).
+           On these chains, you might still receive pending transactions, but they will
+           likely be already mined.
         """
         # Raise if not a websocket uri
         rpc_url = self.node_uri
-        if not rpc_url.startswith("ws"):
-            raise ValueError(
-                "Websocket RPC needed to subscribe to pending transactions"
-            )
+        if not rpc_url.startswith("ws") and not rpc_url.endswith(".ipc"):
+            raise ValueError("Websocket RPC needed to subscribe to node notifications")
+
+        def process_notification(
+            notification: Union[str, bytes], subscription_id: str
+        ) -> None:
+            id, data = parse_notification(notification, subscription_type)
+            if id == subscription_id:
+                on_notification(data)
 
-        async def get_event() -> None:
+        async def main() -> None:
             # Connect to websocket
             async with connect(self.node_uri) as ws:
-                # Subscribe to pending transactions
-                await ws.send(
-                    '{"jsonrpc": "2.0", "id": 1, "method": "eth_subscribe", "params": ["'
-                    + subscription_type
-                    + '"]}'
+                # Subscribe to the notification type
+                subscription_id = await subscribe_to_notification(
+                    ws, subscription_type, on_subscribe
                 )
-                subscription_response = await ws.recv()
-                try:
-                    subscription_id = json.loads(subscription_response)["result"]
-                except Exception as e:
-                    raise Web3ClientException(
-                        f"Failed to subscribe to pending transactions: {e}"
-                    )
-                # Call on_subscribe callback
-                if on_subscribe:
-                    on_subscribe(json.loads(subscription_response))
+                # Main loop
                 while True:
-                    # Wait for new transactions
-                    tx_response = await asyncio.wait_for(ws.recv(), timeout=15)
-                    try:
-                        tx_response_json = json.loads(tx_response)
-                        tx_subscription = tx_response_json["params"]["subscription"]
-                        tx_hash = tx_response_json["params"]["result"]
-                    except Exception as e:
-                        raise Web3ClientException(
-                            f"Failed to parse pending transaction: {e}"
-                        )
-                    # Call on_tx callback
-                    if tx_subscription == subscription_id:
-                        on_tx(tx_hash)
-                        if once:
-                            raise StopAsyncIteration
-
-        # Run loop asynchronously
-        loop = asyncio.get_event_loop()
-        while True:
-            try:
-                loop.run_until_complete(get_event())
-            except StopAsyncIteration:
-                loop.close()
-                break
+                    # Wait for new notifications
+                    notification = await asyncio.wait_for(ws.recv(), timeout=15)
+                    process_notification(notification, subscription_id)
+                    if once:
+                        return
+
+        asyncio.run(main())
+
+    async def async_subscribe(
+        self,
+        on_notification: Callable[[Any], Awaitable[None]],
+        on_subscribe: Callable[[Any], None] = None,
+        once: bool = False,
+        subscription_type: str = "newPendingTransactions",
+    ) -> None:
+        """Look for new pending transactions, blocks or events and, when one is found,
+        call the 'on_notification' callback concurrently.
+
+        For more details, see subscribe().
+        """
+        # Raise if not a websocket uri
+        rpc_url = self.node_uri
+        if not rpc_url.startswith("ws") and not rpc_url.endswith(".ipc"):
+            raise ValueError("Websocket RPC needed to subscribe to node notifications")
+
+        async def process_notification(
+            notification: Union[str, bytes], subscription_id: str
+        ) -> None:
+            id, data = parse_notification(notification, subscription_type)
+            if id == subscription_id:
+                asyncio.create_task(on_notification(data))  # type: ignore
+
+        # Connect to websocket
+        async with connect(self.node_uri) as ws:
+            # Subscribe to the notification type
+            subscription_id = await subscribe_to_notification(
+                ws, subscription_type, on_subscribe
+            )
+            # Main loop
+            while True:
+                # Wait for new notifications
+                notification = await asyncio.wait_for(ws.recv(), timeout=15)
+                await process_notification(notification, subscription_id)
+                if once:
+                    return
 
     ####################
     # Gas
     ####################
 
     def estimate_max_fee_in_gwei(
         self, max_priority_fee_in_gwei: float
```

### Comparing `web3client-1.1.2/src/web3client/erc20_client.py` & `web3client-1.1.3/src/web3client/erc20_client.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/src/web3client/helpers/debug.py` & `web3client-1.1.3/src/web3client/helpers/debug.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/src/web3client/helpers/general.py` & `web3client-1.1.3/src/web3client/helpers/general.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/src/web3factory/erc20_tokens.py` & `web3client-1.1.3/src/web3factory/erc20_tokens.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/src/web3factory/factory.py` & `web3client-1.1.3/src/web3factory/factory.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/src/web3factory/networks.py` & `web3client-1.1.3/src/web3factory/networks.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/src/web3factory/types.py` & `web3client-1.1.3/src/web3factory/types.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/tests/.DS_Store` & `web3client-1.1.3/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/tests/ape/.DS_Store` & `web3client-1.1.3/tests/ape/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/tests/ape/.build/SafeMath.json` & `web3client-1.1.3/tests/ape/.build/SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/tests/ape/.build/Token.json` & `web3client-1.1.3/tests/ape/.build/Token.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/tests/ape/.build/__local__.json` & `web3client-1.1.3/tests/ape/.build/__local__.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/tests/ape/contracts/token/SafeMath.sol` & `web3client-1.1.3/tests/ape/contracts/token/SafeMath.sol`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/tests/ape/contracts/token/Token.sol` & `web3client-1.1.3/tests/ape/contracts/token/Token.sol`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/tests/ape/fixtures.py` & `web3client-1.1.3/tests/ape/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/tests/web3client/fixtures.py` & `web3client-1.1.3/tests/web3client/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/tests/web3client/test_networks.py` & `web3client-1.1.3/tests/web3client/test_networks.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.2/PKG-INFO` & `web3client-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3client
-Version: 1.1.2
+Version: 1.1.3
 Summary: Batteries-included client to interact with blockchains and smart contracts
 License: MIT
 Keywords: web3,blockchain,ethereum,evm
 Author-email: coccoinomane <coccoinomane@gmail.com>
 Requires-Python: >=3.9,<3.11
 Project-URL: homepage, https://github.com/coccoinomane/web3client
 Project-URL: repository, https://github.com/coccoinomane/web3client
```

