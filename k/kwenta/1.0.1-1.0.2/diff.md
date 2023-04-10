# Comparing `tmp/kwenta-1.0.1.tar.gz` & `tmp/kwenta-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwenta-1.0.1.tar", last modified: Sun Apr  9 06:13:06 2023, max compression
+gzip compressed data, was "kwenta-1.0.2.tar", last modified: Mon Apr 10 21:47:10 2023, max compression
```

## Comparing `kwenta-1.0.1.tar` & `kwenta-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 06:13:06.234365 kwenta-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-09 06:13:06.234365 kwenta-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 06:13:06.230365 kwenta-1.0.1/kwenta/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-09 06:12:33.000000 kwenta-1.0.1/kwenta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-09 06:12:33.000000 kwenta-1.0.1/kwenta/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-09 06:12:33.000000 kwenta-1.0.1/kwenta/contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 06:13:06.234365 kwenta-1.0.1/kwenta/json/
--rw-r--r--   0 runner    (1001) docker     (123)    37178 2023-04-09 06:12:33.000000 kwenta-1.0.1/kwenta/json/PerpsV2Market.json
--rw-r--r--   0 runner    (1001) docker     (123)    43145 2023-04-09 06:12:33.000000 kwenta-1.0.1/kwenta/json/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 06:12:33.000000 kwenta-1.0.1/kwenta/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-04-09 06:12:33.000000 kwenta-1.0.1/kwenta/json/sUSD.json
--rw-r--r--   0 runner    (1001) docker     (123)    28698 2023-04-09 06:12:33.000000 kwenta-1.0.1/kwenta/kwenta.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-09 06:12:33.000000 kwenta-1.0.1/kwenta/kwenta_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-09 06:12:33.000000 kwenta-1.0.1/kwenta/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 06:13:06.230365 kwenta-1.0.1/kwenta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-09 06:13:06.000000 kwenta-1.0.1/kwenta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-09 06:13:06.000000 kwenta-1.0.1/kwenta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 06:13:06.000000 kwenta-1.0.1/kwenta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-09 06:13:06.000000 kwenta-1.0.1/kwenta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 06:13:06.000000 kwenta-1.0.1/kwenta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 06:13:06.234365 kwenta-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-09 06:12:33.000000 kwenta-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:47:10.482463 kwenta-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-10 21:47:10.482463 kwenta-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:47:10.478462 kwenta-1.0.2/kwenta/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 21:46:37.000000 kwenta-1.0.2/kwenta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-10 21:46:37.000000 kwenta-1.0.2/kwenta/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28866 2023-04-10 21:46:37.000000 kwenta-1.0.2/kwenta/kwenta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:47:10.478462 kwenta-1.0.2/kwenta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-10 21:47:10.000000 kwenta-1.0.2/kwenta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-10 21:47:10.000000 kwenta-1.0.2/kwenta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:47:10.000000 kwenta-1.0.2/kwenta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-10 21:47:10.000000 kwenta-1.0.2/kwenta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 21:47:10.000000 kwenta-1.0.2/kwenta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 21:47:10.482463 kwenta-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-10 21:46:37.000000 kwenta-1.0.2/setup.py
```

### Comparing `kwenta-1.0.1/PKG-INFO` & `kwenta-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwenta
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python SDK for Kwenta
 Author: Kwenta DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kwenta-1.0.1/kwenta/kwenta.py` & `kwenta-1.0.2/kwenta/kwenta.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 import time
 import warnings
-import requests
 from web3 import Web3
+from web3.types import TxParams
 from decimal import Decimal
+from .constants import DEFAULT_NETWORK_ID, DEFAULT_TRACKING_CODE, DEFAULT_SLIPPAGE, DEFAULT_GQL_ENDPOINT_PERPS, DEFAULT_GQL_ENDPOINT_RATES
 from .contracts import abis, addresses
-from .constants import DEFAULT_NETWORK_ID, DEFAULT_TRACKING_CODE, DEFAULT_SLIPPAGE
+from .alerts import Alerts
+from .queries import Queries
 
 warnings.filterwarnings('ignore')
 
-class kwenta:
-    def __init__(self, provider_rpc:str, wallet_address:str, private_key:str=None, network_id:int=None):
+
+class Kwenta:
+    def __init__(
+            self,
+            provider_rpc: str,
+            wallet_address: str,
+            private_key: str = None,
+            network_id: int = None,
+            gql_endpoint_perps: str = None,
+            gql_endpoint_rates: str = None,
+            telegram_token: str = None,
+            telegram_channel_name: str = None):
         # set default values
         if network_id is None:
             network_id = DEFAULT_NETWORK_ID
 
         # init account variables
         self.private_key = private_key
         self.wallet_address = wallet_address
@@ -23,18 +35,33 @@
         if w3.eth.chain_id != network_id:
             raise Exception("The RPC `chain_id` must match `network_id`")
         else:
             self.network_id = network_id
             self.web3 = w3
 
         # init contracts
-        self.markets, self.market_contracts, self.susd_token = self.init_markets()
+        self.markets, self.market_contracts, self.susd_token = self._load_markets()
         self.token_list = list(self.markets.keys())
 
-    def init_markets(self):
+        # init alerts
+        if telegram_token and telegram_channel_name:
+            self.alerts = Alerts(telegram_token, telegram_channel_name)
+
+        # init queries
+        if not gql_endpoint_perps:
+            gql_endpoint_perps = DEFAULT_GQL_ENDPOINT_PERPS[self.network_id]
+
+        if not gql_endpoint_rates:
+            gql_endpoint_rates = DEFAULT_GQL_ENDPOINT_RATES[self.network_id]
+
+        self.queries = Queries(
+            gql_endpoint_perps=gql_endpoint_perps,
+            gql_endpoint_rates=gql_endpoint_rates)
+
+    def _load_markets(self):
         """
         Initializes all market contracts
         ...
 
         Attributes
         ----------
         N/A
@@ -60,41 +87,46 @@
                 "takerFee": market[10][0],
                 "makerFee": market[10][1],
                 "takerFeeDelayedOrder": market[10][2],
                 "makerFeeDelayedOrder": market[10][3],
                 "takerFeeOffchainDelayedOrder": market[10][4],
                 "makerFeeOffchainDelayedOrder": market[10][5],
             }
-            
+
             # set them
             token_symbol = market[2].decode('utf-8').strip("\x00")[1:-4]
             markets[token_symbol] = normalized_market
             market_contracts[token_symbol] = self.web3.eth.contract(
-                self.web3.to_checksum_address(normalized_market['market_address']), abi=abis['PerpsV2Market'])
-            
+                self.web3.to_checksum_address(
+                    normalized_market['market_address']),
+                abi=abis['PerpsV2Market'])
+
         # load sUSD contract
-        susd_token = self.web3.eth.contract(
-            self.web3.to_checksum_address(addresses['sUSD'][self.network_id]), abi=abis['sUSD'])
+        susd_token = self.web3.eth.contract(self.web3.to_checksum_address(
+            addresses['sUSD'][self.network_id]), abi=abis['sUSD'])
 
         return markets, market_contracts, susd_token
 
-    def load_market_contract(self, token_symbol: str):
-        """
-        Loads market contract for specific token symbol
-        ...
+    def _get_tx_params(
+        self, value=0, to=None
+    ) -> TxParams:
+        """Get generic transaction parameters."""
+        params: TxParams = {
+            'from': self.wallet_address,
+            'to': to,
+            'chainId': self.network_id,
+            'value': value,
+            'gas': 1500000,
+            'gasPrice': self.web3.to_wei(
+                '0.4',
+                'gwei'),
+            'nonce': self.web3.eth.get_transaction_count(self.wallet_address)
+        }
 
-        Attributes
-        ----------
-        token_symbol : str
-            token symbol from list of supported asset
-        """
-        # load market contracts
-        proxy_contract = self.web3.eth.contract(self.web3.to_checksum_address(
-            self.markets[token_symbol]['market_address']), abi=abis['PerpsV2Market'])
-        return proxy_contract
+        return params
 
     def get_market_contract(self, token_symbol: str):
         """
         Run checks and return market contract if it exists
         ...
 
         Attributes
@@ -102,48 +134,48 @@
         token_symbol : str
             token symbol from list of supported asset
         """
         if not (token_symbol in self.token_list):
             raise Exception("Token Not in Supported Token List.")
         else:
             return self.market_contracts[token_symbol.upper()]
- 
+
     def execute_transaction(self, tx_data: dict):
         """
-        Execute a transaction given the TX data 
+        Execute a transaction given the TX data
         ...
 
         Attributes
         ----------
         tx_data : dict
             tx data to send transaction
         private_key : str
             private key of wallet sending transaction
         """
         if self.private_key is None:
             raise Exception("No private key specified.")
         signed_txn = self.web3.eth.account.sign_transaction(
             tx_data, private_key=self.private_key)
-        tx_token = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
+        tx_token = self.web3.eth.send_raw_transaction(
+            signed_txn.rawTransaction)
         return self.web3.to_hex(tx_token)
 
     def check_delayed_orders(self, token_symbol: str) -> bool:
         """
         Check if delayed order is in queue
         ...
 
         Attributes
         ----------
-        wallet_address : str
-            wallet_address of wallet to check
         token_symbol : str
             token symbol from list of supported asset
         """
         market_contract = self.market_contracts[token_symbol]
-        return (market_contract.functions.delayedOrders(self.wallet_address).call())[0]
+        return (market_contract.functions.delayedOrders(
+            self.wallet_address).call())[0]
 
     def get_current_asset_price(self, token_symbol: str) -> dict:
         """
         Gets current asset price for config asset.
         ...
 
         Attributes
@@ -156,45 +188,48 @@
         Dict with wei and USD price
         """
         market_contract = self.market_contracts[token_symbol.upper()]
         wei_price = (market_contract.functions.assetPrice().call())[0]
         usd_price = self.web3.from_wei(wei_price, 'ether')
         return {"usd": usd_price, "wei": wei_price}
 
-    def get_current_positions(self, token_symbol: str) -> dict:
+    def get_current_position(self, token_symbol: str) -> dict:
         """
         Gets Current Position Data
         ...
 
         Attributes
         ----------
-        wallet_address : str
-            wallet_address of wallet to check
         token_symbol : str
             token symbol from list of supported asset
         Returns
         ----------
         Dict: position information
         """
         market_contract = self.get_market_contract(token_symbol)
         id, last_funding_index, margin, last_price, size = market_contract.functions.positions(
             self.wallet_address).call()
         current_asset_price = self.get_current_asset_price(token_symbol)
-        
+
         # clean usd values
         is_short = -1 if size < 0 else 1
         size_ether = self.web3.from_wei(abs(size), 'ether') * is_short
         last_price_usd = self.web3.from_wei(last_price, 'ether')
 
         # calculate pnl
         price_diff = current_asset_price['usd'] - last_price_usd
         pnl = size_ether * price_diff * is_short
 
-        positions_data = {"id": id, "last_funding_index": last_funding_index,
-                          "margin": margin, "last_price": last_price, "size": size,"pnl_usd": pnl}
+        positions_data = {
+            "id": id,
+            "last_funding_index": last_funding_index,
+            "margin": margin,
+            "last_price": last_price,
+            "size": size,
+            "pnl_usd": pnl}
         return positions_data
 
     def get_accessible_margin(self, token_symbol: str) -> dict:
         """
         Gets available account margin
         ...
 
@@ -208,15 +243,16 @@
         ----------
         Dict: Margin remaining in wei and usd
         """
         market_contract = self.get_market_contract(token_symbol)
         margin_allowed = (market_contract.functions.accessibleMargin(
             self.wallet_address).call())[0]
         margin_usd = self.web3.from_wei(margin_allowed, 'ether')
-        return {"margin_remaining": margin_allowed, "margin_remaining_usd": margin_usd}
+        return {"margin_remaining": margin_allowed,
+                "margin_remaining_usd": margin_usd}
 
     def can_liquidate(self, token_symbol: str) -> dict:
         """
         Checks if Liquidation is possible for wallet
         ...
 
         Attributes
@@ -228,15 +264,16 @@
         Dict: Liquidation Data
         """
         market_contract = self.get_market_contract(token_symbol)
         liquidation_check = market_contract.functions.canLiquidate(
             self.wallet_address).call()
         liquidation_price = market_contract.functions.liquidationPrice(
             self.wallet_address).call()
-        return {"liq_possible": liquidation_check, "liq_price": liquidation_price}
+        return {"liq_possible": liquidation_check,
+                "liq_price": liquidation_price}
 
     def get_market_skew(self, token_symbol: str) -> dict:
         """
         Gets current market long/short market skew
         ...
 
         Attributes
@@ -246,113 +283,135 @@
 
         Returns
         ----------
         Dict with market skew information
         """
         market_contract = self.get_market_contract(token_symbol)
         long, short = market_contract.functions.marketSizes().call()
-        total = long+short
+        total = long + short
         if total == 0:
             percent_long = 0
             percent_short = 0
         else:
-            percent_long = long/total*100
-            percent_short = short/total*100
-        return {"long": long, "short": short, "percent_long": percent_long, "percent_short": percent_short}
+            percent_long = long / total * 100
+            percent_short = short / total * 100
+        return {"long": long, "short": short,
+                "percent_long": percent_long, "percent_short": percent_short}
 
     def get_susd_balance(self) -> dict:
         """
         Gets current sUSD Balance in wallet
         ...
 
         Attributes
         ----------
         wallet_address : str
             wallet_address of wallet to check
         Returns
         ----------
         Dict: wei and usd sUSD balance
         """
-        balance = self.susd_token.functions.balanceOf(self.wallet_address).call()
+        balance = self.susd_token.functions.balanceOf(
+            self.wallet_address).call()
         balance_usd = self.web3.from_wei(balance, 'ether')
         return {"balance": balance, "balance_usd": balance_usd}
 
-    def transfer_margin(self, token_symbol: str, token_amount: int,execute_now:bool=False) -> str:
+    def get_leveraged_amount(self, token_symbol: str,
+                             leverage_multiplier: float) -> dict:
+        """
+        Get out amount of leverage available for account
+        ...
+
+        Attributes
+        ----------
+        token_symbol : str
+            token symbol from list of supported asset
+        leverage_multiplier : int
+            leverage multiplier amount. Must be within the range 0.1 - 24.7.
+
+        Returns
+        ----------
+        Dict: amount of leverage available and max amount of leverage available
+        """
+        if leverage_multiplier is not None:
+            if leverage_multiplier > 24.7 or leverage_multiplier < 0.1:
+                print("Leveraged_multiplier must be within the range 0.1 - 24.7!")
+                return None
+        margin = self.get_accessible_margin(token_symbol)
+        asset_price = self.get_current_asset_price(token_symbol)
+        print(f"SUSD Available: {margin['margin_remaining_usd']}")
+        print(f"Current Asset Price: {asset_price['usd']}")
+        # Using 24.7 to cover edge cases
+        max_leverage = self.web3.to_wei(
+            (margin['margin_remaining_usd'] /
+             asset_price['usd']) *
+            Decimal(24.7),
+            'ether')
+        print(f"Max Leveraged Asset Amount: {max_leverage}")
+        leveraged_amount = (
+            (margin['margin_remaining'] /
+             asset_price['wei']) *
+            leverage_multiplier)
+        return {"leveraged_amount": leveraged_amount,
+                "max_asset_leverage": max_leverage}
+
+    def transfer_margin(self, token_symbol: str,
+                        token_amount: int, execute_now: bool = False) -> str:
         """
         Transfers SUSD from wallet to Margin account
         ...
 
         Attributes
         ----------
         token_amount : int
             Token amount *in human readable* to send to Margin account
         wallet_address : str
             wallet_address of wallet to check
         token_symbol : str
             token symbol from list of supported asset
         Returns
         ----------
-        str: token transfer Tx id 
+        str: token transfer Tx id
         """
         if token_amount == 0:
             raise Exception("Can not transfer 0 margin")
 
         is_withdrawal = -1 if token_amount < 0 else 1
-        token_amount = self.web3.to_wei(abs(token_amount), 'ether') * is_withdrawal
+        token_amount = self.web3.to_wei(
+            abs(token_amount), 'ether') * is_withdrawal
 
         susd_balance = self.get_susd_balance()
         market_contract = self.get_market_contract(token_symbol)
         print(f"sUSD Balance: {susd_balance['balance_usd']}")
         if (token_amount < susd_balance['balance']):
             data_tx = market_contract.encodeABI(
                 fn_name='transferMargin', args=[token_amount])
-            transfer_tx = {'value': 0, 'chainId': self.network_id, 'to': market_contract.address, 'from': self.wallet_address, 'gas': 1500000,
-                           'gasPrice': self.web3.to_wei('0.4', 'gwei'), 'nonce': self.web3.eth.get_transaction_count(self.wallet_address), 'data': data_tx}
+
+            tx_params = self._get_tx_params(
+                to=market_contract.address, value=0)
+            tx_params['data'] = data_tx
+
             if execute_now:
-                tx_token = self.execute_transaction(transfer_tx)
+                tx_token = self.execute_transaction(tx_params)
                 print(f"Updating Position by {token_amount}")
                 print(f"TX: {tx_token}")
                 time.sleep(1)
                 return tx_token
             else:
-                return {"token":token_symbol.upper(),'token_amount':token_amount/(10**18),"susd_balance":susd_balance,"tx_data":transfer_tx}
-
-    def get_leveraged_amount(self, token_symbol: str, leverage_multiplier: float) -> dict:
-        """
-        Get out amount of leverage available for account
-        ...
-
-        Attributes
-        ----------
-        token_symbol : str
-            token symbol from list of supported asset
-        leverage_multiplier : int
-            leverage multiplier amount. Must be within the range 0.1 - 24.7.
-
-        Returns
-        ----------
-        Dict: amount of leverage available and max amount of leverage available
-        """
-        if leverage_multiplier != None:
-            if leverage_multiplier > 24.7 or leverage_multiplier < 0.1:
-                print("Leveraged_multiplier must be within the range 0.1 - 24.7!")
-                return None
-        margin = self.get_accessible_margin(token_symbol)
-        asset_price = self.get_current_asset_price(token_symbol)
-        print(f"SUSD Available: {margin['margin_remaining_usd']}")
-        print(f"Current Asset Price: {asset_price['usd']}")
-        # Using 24.7 to cover edge cases
-        max_leverage = self.web3.to_wei(
-            (margin['margin_remaining_usd']/asset_price['usd']) * Decimal(24.7), 'ether')
-        print(f"Max Leveraged Asset Amount: {max_leverage}")
-        leveraged_amount = (
-            (margin['margin_remaining']/asset_price['wei'])*leverage_multiplier)
-        return {"leveraged_amount": leveraged_amount, "max_asset_leverage": max_leverage}
-
-    def modify_position(self, token_symbol: str, size_delta: float, slippage: float = DEFAULT_SLIPPAGE,execute_now: bool = False) -> str:
+                return {"token": token_symbol.upper(),
+                        'token_amount': token_amount / (10**18),
+                        "susd_balance": susd_balance,
+                        "tx_data": tx_params}
+
+    def modify_position(
+            self,
+            token_symbol: str,
+            size_delta: float,
+            slippage: float = DEFAULT_SLIPPAGE,
+            execute_now: bool = False) -> str:
         """
         Submits a delayed offchain order with a size of `size_delta`
         ...
 
         Attributes
         ----------
         size_delta : float
@@ -367,318 +426,359 @@
         ----------
         str: token transfer Tx id
         """
         is_short = -1 if size_delta < 0 else 1
         market_contract = self.get_market_contract(token_symbol)
         size_delta = self.web3.to_wei(abs(size_delta), 'ether') * is_short
 
-        current_position = self.get_current_positions(token_symbol)
+        current_position = self.get_current_position(token_symbol)
         current_price = self.get_current_asset_price(token_symbol)
 
-        desired_fill_price = int(current_price['wei'] + current_price['wei'] * (slippage/100) * is_short)
+        desired_fill_price = int(
+            current_price['wei'] + current_price['wei'] * (slippage / 100) * is_short)
 
         print(f"Current Position Size: {current_position['size']}")
-        # check that position size is less than margin limit
-        if (size_delta < current_position['margin']):
-            data_tx = market_contract.encodeABI(fn_name='submitOffchainDelayedOrderWithTracking', args=[
+        data_tx = market_contract.encodeABI(
+            fn_name='submitOffchainDelayedOrderWithTracking', args=[
                 int(size_delta), desired_fill_price, DEFAULT_TRACKING_CODE])
-            transfer_tx = {'value': 0, 'chainId': self.network_id, 'to': market_contract.address, 'from': self.wallet_address, 'gas': 1500000,
-                           'gasPrice': self.web3.to_wei('0.4', 'gwei'), 'nonce': self.web3.eth.get_transaction_count(self.wallet_address), 'data': data_tx}
 
-            print(f"Updating Position by {size_delta}")
-            if execute_now:
-                tx_token = self.execute_transaction(transfer_tx)
-                print(f"TX: {tx_token}")
-                time.sleep(1)
-                return tx_token
-            else:
-                return {"token":token_symbol.upper(),'current_position':current_position['size'],"tx_data":transfer_tx}
+        tx_params = self._get_tx_params(to=market_contract.address, value=0)
+        tx_params['data'] = data_tx
 
-    def close_position(self, token_symbol: str,slippage:float=DEFAULT_SLIPPAGE,execute_now:bool=False) -> str:
+        print(f"Updating Position by {size_delta}")
+        if execute_now:
+            tx_token = self.execute_transaction(tx_params)
+            print(f"TX: {tx_token}")
+            time.sleep(1)
+            return tx_token
+        else:
+            return {
+                "token": token_symbol.upper(),
+                'current_position': current_position['size'],
+                "tx_data": tx_params}
+
+    def close_position(
+            self,
+            token_symbol: str,
+            slippage: float = DEFAULT_SLIPPAGE,
+            execute_now: bool = False) -> str:
         """
-        Fully closes account position 
+        Fully closes account position
         ...
 
         Attributes
         ----------
         token_symbol : str
             token symbol from list of supported asset
         slippage : float
             slippage percentage
-            
+
         Returns
         ----------
-        str: token transfer Tx id 
+        str: token transfer Tx id
         """
         market_contract = self.get_market_contract(token_symbol)
-        current_position = self.get_current_positions(token_symbol)
+        current_position = self.get_current_position(token_symbol)
         current_price = self.get_current_asset_price(token_symbol)
 
         is_short = -1 if -current_position['size'] < 0 else 1
         desired_fill_price = int(
-            current_price['wei'] + current_price['wei'] * (slippage/100) * is_short)
+            current_price['wei'] + current_price['wei'] * (slippage / 100) * is_short)
 
         print(f"Current Position Size: {current_position['size']}")
         if current_position['size'] == 0:
             print("Not in position!")
             return None
         # Flip position size to the opposite direction
-        data_tx = market_contract.encodeABI(fn_name='submitCloseOffchainDelayedOrderWithTracking', args=[
-            desired_fill_price, DEFAULT_TRACKING_CODE])
-        transfer_tx = {'value': 0, 'chainId': self.network_id, 'to': market_contract.address, 'from': self.wallet_address, 'gas': 1500000,
-                       'gasPrice': self.web3.to_wei('0.4', 'gwei'), 'nonce': self.web3.eth.get_transaction_count(self.wallet_address), 'data': data_tx}
+        data_tx = market_contract.encodeABI(
+            fn_name='submitCloseOffchainDelayedOrderWithTracking', args=[
+                desired_fill_price, DEFAULT_TRACKING_CODE])
+
+        tx_params = self._get_tx_params(to=market_contract.address, value=0)
+        tx_params['data'] = data_tx
+
         if execute_now:
-            tx_token = self.execute_transaction(transfer_tx)
+            tx_token = self.execute_transaction(tx_params)
             print(f"Closing Position by {-current_position['size']}")
             print(f"TX: {tx_token}")
             time.sleep(1)
             return tx_token
         else:
-            return {"token":token_symbol.upper(),'current_position':current_position['size'],"tx_data":transfer_tx}
-
-    def open_position(self, token_symbol: str, short: bool = False, position_amount: float = None,slippage:float=DEFAULT_SLIPPAGE,leverage_multiplier: float = None,execute_now:bool=False) -> str:
+            return {
+                "token": token_symbol.upper(),
+                'current_position': current_position['size'],
+                "tx_data": tx_params}
+
+    def open_position(
+            self,
+            token_symbol: str,
+            short: bool = False,
+            size_delta: float = None,
+            slippage: float = DEFAULT_SLIPPAGE,
+            leverage_multiplier: float = None,
+            execute_now: bool = False) -> str:
         """
         Open account position in a direction
         ...
 
         Attributes
         ----------
         token_symbol : str
             token symbol from list of supported asset
-        short : bool, optional 
+        short : bool, optional
             set to True when creating a short. (Implemented to double check side)
-        position_amount : int, optional 
+        size_delta : int, optional
             position amount in human readable format as trade asset i.e. 12 SOL. Exact position in a direction (Sign this It WILL MATTER).
-        leverage_multiplier : 
+        leverage_multiplier :
             Multiplier of Leverage to use when creating order. Based on available margin in account.
         slippage : float
             slippage percentage
-            
-        *Use either position_amount or leverage_multiplier.
+
+        *Use either size_delta or leverage_multiplier.
 
         Returns
         ----------
-        str: token transfer Tx id 
+        str: token transfer Tx id
         """
-        if (position_amount == None) and (leverage_multiplier == None):
+        if (size_delta is None) and (leverage_multiplier is None):
             print("Enter EITHER a position amount or a leverage multiplier!")
             return None
-        elif (position_amount != None) and (leverage_multiplier != None):
+        elif (size_delta is not None) and (leverage_multiplier is not None):
             print("Enter EITHER a position amount or a leverage multiplier!")
             return None
 
         market_contract = self.get_market_contract(token_symbol)
-        current_position = self.get_current_positions(token_symbol)
+        current_position = self.get_current_position(token_symbol)
         current_price = self.get_current_asset_price(token_symbol)
 
         # starting at zero otherwise use Update position
         if current_position['size'] != 0:
             print(f"You are already in a position, use modify_position() instead.")
             print(
                 f"Current Position Size: {self.web3.from_wei(current_position['size'], 'ether')}")
             return None
         if leverage_multiplier:
-            max_leverage = self.get_leveraged_amount(token_symbol,leverage_multiplier)['max_asset_leverage']
-            position_amount = self.get_leveraged_amount(
-                token_symbol, leverage_multiplier=leverage_multiplier)['leveraged_amount']
-        elif position_amount:
-            max_leverage = self.get_leveraged_amount(token_symbol,1)['max_asset_leverage']
-            position_amount = position_amount*(10**18)
+            leveraged_amount = self.get_leveraged_amount(
+                token_symbol, leverage_multiplier)
+            max_leverage = leveraged_amount['max_asset_leverage']
+
+            size_delta = leveraged_amount['leveraged_amount']
+            is_short = short
+            size_delta = self.web3.to_wei(abs(size_delta), 'ether') * is_short
+        elif size_delta:
+            max_leverage = self.get_leveraged_amount(
+                token_symbol, 1)['max_asset_leverage']
+
+            is_short = -1 if size_delta < 0 else 1
+            size_delta = self.web3.to_wei(abs(size_delta), 'ether') * is_short
         # check side
-        if short == True:
-            position_amount = position_amount * -1
-        if (position_amount < 0) and short == False:
+        if short == True & is_short != True:
             print(
                 "Position size is Negative & Short set to False! Double Check intention.")
             return None
         # checking available margin to make sure this is possible
-        if (abs(position_amount) < max_leverage):
+        if (abs(size_delta) < max_leverage):
             desired_fill_price = int(
-                current_price['wei'] + current_price['wei'] * (slippage/100) * short)
+                current_price['wei'] + current_price['wei'] * (slippage / 100) * is_short)
+
+            data_tx = market_contract.encodeABI(
+                fn_name='submitOffchainDelayedOrderWithTracking', args=[
+                    int(size_delta), desired_fill_price, DEFAULT_TRACKING_CODE])
+
+            tx_params = self._get_tx_params(
+                to=market_contract.address, value=0)
+            tx_params['data'] = data_tx
 
-            data_tx = market_contract.encodeABI(fn_name='submitOffchainDelayedOrderWithTracking', args=[
-                int(position_amount), desired_fill_price, DEFAULT_TRACKING_CODE])
-            transfer_tx = {'value': 0, 'chainId': self.network_id, 'to': market_contract.address, 'from': self.wallet_address, 'gas': 1500000,
-                           'gasPrice': self.web3.to_wei('0.4', 'gwei'), 'nonce': self.web3.eth.get_transaction_count(self.wallet_address), 'data': data_tx}
             if execute_now:
-                tx_token = self.execute_transaction(transfer_tx)
-                print(f"Updating Position by {position_amount}")
+                tx_token = self.execute_transaction(tx_params)
+                print(f"Updating Position by {size_delta}")
                 print(f"TX: {tx_token}")
                 time.sleep(1)
                 return tx_token
             else:
-                return {"token":token_symbol.upper(),'position_size':position_amount/(10**18),'current_position':current_position['size'],"max_leverage":max_leverage/(10**18),"leveraged_percent":(position_amount/max_leverage)*100,"tx_data":transfer_tx}
+                return {"token": token_symbol.upper(),
+                        'position_size': size_delta / (10**18),
+                        'current_position': current_position['size'],
+                        "max_leverage": max_leverage / (10**18),
+                        "leveraged_percent": (size_delta / max_leverage) * 100,
+                        "tx_data": tx_params}
         return 'some'
 
-    def open_limit(self, token_symbol: str, limit_price: float, position_amount: float = None, leverage_multiplier: float = None, slippage: float = DEFAULT_SLIPPAGE, short: bool = False, execute_now: bool = False) -> str:
+    def open_limit(
+            self,
+            token_symbol: str,
+            limit_price: float,
+            size_delta: float = None,
+            leverage_multiplier: float = None,
+            slippage: float = DEFAULT_SLIPPAGE,
+            short: bool = False,
+            execute_now: bool = False) -> str:
         """
         Open Limit position in a direction
         ...
 
         Attributes
         ----------
         token_symbol : str
             token symbol from list of supported asset
-        short : bool, optional 
+        short : bool, optional
             set to True when creating a short. (Implemented to double check side)
         limit_price : float
-            limit price in dollars to open position. 
-        position_amount : int, optional 
+            limit price in dollars to open position.
+        size_delta : int, optional
             position amount in human readable format as trade asset i.e. 12 SOL . Exact position in a direction (Sign this It WILL MATTER).
-        leverage_multiplier : 
+        leverage_multiplier :
             Multiplier of Leverage to use when creating order. Based on available margin in account.
         slippage : float
             slippage percentage
-        *Use either position_amount or leverage_multiplier.
+        *Use either size_delta or leverage_multiplier.
 
         Returns
         ----------
-        str: token transfer Tx id 
+        str: token transfer Tx id
         """
-        if (position_amount == None) and (leverage_multiplier == None):
+        if (size_delta is None) and (leverage_multiplier is None):
             print("Enter EITHER a position amount or a leverage multiplier!")
             return None
-        elif (position_amount != None) and (leverage_multiplier != None):
+        elif (size_delta is not None) and (leverage_multiplier is not None):
             print("Enter EITHER a position amount or a leverage multiplier!")
             return None
 
-        current_position = self.get_current_positions(token_symbol)
+        current_position = self.get_current_position(token_symbol)
         current_price = self.get_current_asset_price(token_symbol)
 
         if current_position['size'] != 0:
             print(f"You are already in a position, use modify_position() instead.")
             print(
                 f"Current Position Size: {self.web3.from_wei(current_position['size'], 'ether')}")
             return None
 
         # Case for position_amount manually set
-        if position_amount != None:
-            #check Short Position
-            if short == True:
+        if size_delta is not None:
+            # check Short Position
+            if short:
                 if current_price['usd'] >= limit_price:
-                    return self.open_position(token_symbol,short=True, slippage=slippage, position_amount=position_amount, execute_now=execute_now)
+                    return self.open_position(
+                        token_symbol,
+                        short=True,
+                        slippage=slippage,
+                        size_delta=size_delta,
+                        execute_now=execute_now)
             else:
                 if current_price['usd'] <= limit_price:
-                    return self.open_position(token_symbol, short=False, slippage=slippage, position_amount=position_amount, execute_now=execute_now)
-        
+                    return self.open_position(
+                        token_symbol,
+                        short=False,
+                        slippage=slippage,
+                        size_delta=size_delta,
+                        execute_now=execute_now)
+
         # Case for Leverage Multiplier
         else:
-            if short == True:
+            if short:
                 if current_price['usd'] >= limit_price:
-                    return self.open_position(token_symbol, short=True,  slippage=slippage,leverage_multiplier=leverage_multiplier, execute_now=execute_now)
+                    return self.open_position(
+                        token_symbol,
+                        short=True,
+                        slippage=slippage,
+                        leverage_multiplier=leverage_multiplier,
+                        execute_now=execute_now)
             else:
                 if current_price['usd'] <= limit_price:
-                    return self.open_position(token_symbol, short=False, slippage=slippage, leverage_multiplier=leverage_multiplier, execute_now=execute_now)
+                    return self.open_position(
+                        token_symbol,
+                        short=False,
+                        slippage=slippage,
+                        leverage_multiplier=leverage_multiplier,
+                        execute_now=execute_now)
         print(
             f"Limit not reached current : {current_price} | Entry: {current_position['last_price']/(10**18)} | Limit: {limit_price}")
         return None
 
-    def close_limit(self, token_symbol: str, limit_price: float, slippage:float=DEFAULT_SLIPPAGE, execute_now:bool=False):
+    def close_limit(
+            self,
+            token_symbol: str,
+            limit_price: float,
+            slippage: float = DEFAULT_SLIPPAGE,
+            execute_now: bool = False):
         """
         Close Limit position in a direction
         ...
 
         Attributes
         ----------
         token_symbol : str
             token symbol from list of supported asset
         limit_price : float
-            limit price in *dollars* to open position. 
+            limit price in *dollars* to open position.
         slippage : float
             slippage percentage
         Returns
         ----------
-        str: token transfer Tx id 
+        str: token transfer Tx id
         """
-        current_position = self.get_current_positions(token_symbol)
+        current_position = self.get_current_position(token_symbol)
         current_price = self.get_current_asset_price(token_symbol)
 
         # Check if you are in Position
         if current_position['size'] == 0:
             print("Not in position!")
             return None
-        
+
         short = True if current_position['size'] < 0 else False
-        if short == True:
+        if short:
             if current_price['usd'] <= limit_price:
-                return self.close_position(token_symbol,slippage=slippage, execute_now=execute_now)
+                return self.close_position(
+                    token_symbol, slippage=slippage, execute_now=execute_now)
         else:
             if current_price['usd'] >= limit_price:
-                return self.close_position(token_symbol,slippage=slippage, execute_now=execute_now)
+                return self.close_position(
+                    token_symbol, slippage=slippage, execute_now=execute_now)
         print(
             f"Limit not reached current : {current_price['usd']} | Entry: {current_position['last_price']/(10**18)} | Limit: {limit_price}")
         return None
 
-    def close_stop_limit(self, token_symbol: str, limit_price: float, stop_price: float,slippage:float=DEFAULT_SLIPPAGE) -> str:
+    def close_stop_limit(
+            self,
+            token_symbol: str,
+            limit_price: float,
+            stop_price: float,
+            slippage: float = DEFAULT_SLIPPAGE) -> str:
         """
         Close Limit position in a direction with Stop price
         ...
 
         Attributes
         ----------
         token_symbol : str
             token symbol from list of supported asset
         limit_price : float
-            limit price in dollars to open position. 
-        stop_price : float 
-            Set to stop price incase of bad position, will exit position if triggered 
+            limit price in dollars to open position.
+        stop_price : float
+            Set to stop price incase of bad position, will exit position if triggered
         slippage : float
             slippage percentage
         Returns
         ----------
-        str: token transfer Tx id 
+        str: token transfer Tx id
         """
-        current_position = self.get_current_positions(token_symbol)
+        current_position = self.get_current_position(token_symbol)
         current_price = self.get_current_asset_price(token_symbol)
         # Check if you are in Position
         if current_position['size'] == 0:
             print("Not in position!")
             return None
-    
+
         short = True if current_position['size'] < 0 else False
-        if short == True:
+        if short:
             if current_price['usd'] <= limit_price:
-                return self.close_position(token_symbol,slippage=slippage)
+                return self.close_position(token_symbol, slippage=slippage)
             elif current_price['usd'] >= stop_price:
-                return self.close_position(token_symbol,slippage=slippage)
+                return self.close_position(token_symbol, slippage=slippage)
         else:
             if current_price['usd'] >= limit_price:
-                return self.close_position(token_symbol,slippage=slippage)
+                return self.close_position(token_symbol, slippage=slippage)
             elif current_price['usd'] <= stop_price:
-                return self.close_position(token_symbol,slippage=slippage)
+                return self.close_position(token_symbol, slippage=slippage)
         print(
             f"Limit not reached current : {current_price['usd']} | Entry: {current_position['last_price']/(10**18)} | Limit: {limit_price} | Stop Limit: {stop_price}")
         return None
-
-    def get_historicals(self, token_symbol, time_back=72, period=1800):
-        """
-        Gets historical data from subgraph
-        ...
-
-        Attributes
-        ----------
-        token_symbol : str
-            token symbol from list of supported asset
-        time_back : int
-            How many hours back to get historical data from
-        period : int
-            Timescale of candles in seconds 
-
-        Returns
-        ----------
-        str: token transfer Tx id 
-        """
-        current_timestamp = int(time.time())
-        # Subtract 4 hours from current timestamp
-        day_ago = current_timestamp - (time_back * 60 * 60)
-        url = f'https://api.thegraph.com/subgraphs/name/kwenta/optimism-latest-rates'
-        headers = {'accept': 'application/json, text/plain, */*',
-            'content-type': 'application/json'}
-        payload = {
-            "query": f"{{candles(first:1000,where:{{synth:\"{token_symbol.upper()}\",timestamp_gt:{day_ago},timestamp_lt:{current_timestamp},period:{period}}},orderBy:\"timestamp\",orderDirection:\"asc\"){{id synth open high low close timestamp average period aggregatedPrices}}}}"
-        }
-        try:
-            response = requests.post(url, headers=headers, json=payload)
-            return response.json()
-        except Exception as e:
-            print(e)
-            return None
```

### Comparing `kwenta-1.0.1/kwenta.egg-info/PKG-INFO` & `kwenta-1.0.2/kwenta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwenta
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python SDK for Kwenta
 Author: Kwenta DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kwenta-1.0.1/setup.py` & `kwenta-1.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='kwenta',
-    version='1.0.1',
+    version='1.0.2',
     description='Python SDK for Kwenta',
     long_description='Python SDK for Kwenta',
     author='Kwenta DAO',
     packages=['kwenta'],
     install_requires=[
         "numpy",
         "pandas",
@@ -19,13 +19,10 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     python_requires=">=3.8",
-    package_data={"kwenta":["json/*"]},
+    package_data={"kwenta": ["json/*"]},
     include_package_data=True,
 )
-# Local Install
-# python .\setup.py sdist bdist_wheel
-# pip install .
```

