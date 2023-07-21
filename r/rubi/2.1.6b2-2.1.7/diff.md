# Comparing `tmp/rubi-2.1.6b2.tar.gz` & `tmp/rubi-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.1.6b2.tar", max compression
+gzip compressed data, was "rubi-2.1.7.tar", max compression
```

## Comparing `rubi-2.1.6b2.tar` & `rubi-2.1.7.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.1.6b2/LICENSE
--rw-r--r--   0        0        0     2757 2023-07-18 23:38:58.047336 rubi-2.1.6b2/README.md
--rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.1.6b2/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.1.6b2/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.1.6b2/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.1.6b2/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      833 2023-07-19 19:13:00.615720 rubi-2.1.6b2/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.1.6b2/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.1.6b2/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      858 2023-07-19 19:13:00.615912 rubi-2.1.6b2/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.1.6b2/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.1.6b2/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      760 2023-07-19 19:13:00.616134 rubi-2.1.6b2/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.1.6b2/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.1.6b2/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      832 2023-07-19 19:13:00.616334 rubi-2.1.6b2/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0     1748 2023-07-21 01:34:06.171481 rubi-2.1.6b2/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-07 13:58:54.647129 rubi-2.1.6b2/rubi/__init__.py
--rw-r--r--   0        0        0    30603 2023-07-21 01:25:04.169604 rubi-2.1.6b2/rubi/client.py
--rw-r--r--   0        0        0      163 2023-06-30 02:50:06.554484 rubi-2.1.6b2/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    65755 2023-07-14 18:57:40.986583 rubi-2.1.6b2/rubi/contracts/aid.py
--rw-r--r--   0        0        0    12337 2023-07-19 19:12:54.493238 rubi-2.1.6b2/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0       74 2023-07-04 04:06:47.229802 rubi-2.1.6b2/rubi/contracts/contract_types/__init__.py
--rw-r--r--   0        0        0    15898 2023-07-14 18:57:40.986973 rubi-2.1.6b2/rubi/contracts/contract_types/events.py
--rw-r--r--   0        0        0     2805 2023-07-14 18:57:40.987143 rubi-2.1.6b2/rubi/contracts/contract_types/transaction_reciept.py
--rw-r--r--   0        0        0    18565 2023-07-14 20:13:22.360534 rubi-2.1.6b2/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24878 2023-07-20 19:29:23.201977 rubi-2.1.6b2/rubi/contracts/market.py
--rw-r--r--   0        0        0    14915 2023-07-14 18:57:40.987660 rubi-2.1.6b2/rubi/contracts/router.py
--rw-r--r--   0        0        0       77 2023-07-07 13:58:54.648079 rubi-2.1.6b2/rubi/data/README.md
--rw-r--r--   0        0        0       31 2023-07-07 13:58:54.648312 rubi-2.1.6b2/rubi/data/__init__.py
--rw-r--r--   0        0        0    16515 2023-07-21 01:14:16.995206 rubi-2.1.6b2/rubi/data/market.py
--rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.1.6b2/rubi/network/__init__.py
--rw-r--r--   0        0        0     8450 2023-07-20 19:31:29.720610 rubi-2.1.6b2/rubi/network/network.py
--rw-r--r--   0        0        0      121 2023-07-19 19:12:54.494446 rubi-2.1.6b2/rubi/rubicon_types/__init__.py
--rw-r--r--   0        0        0    15796 2023-07-15 17:29:20.578781 rubi-2.1.6b2/rubi/rubicon_types/order.py
--rw-r--r--   0        0        0    11554 2023-07-15 17:29:20.579083 rubi-2.1.6b2/rubi/rubicon_types/order_query.py
--rw-r--r--   0        0        0     6323 2023-07-15 17:29:20.579349 rubi-2.1.6b2/rubi/rubicon_types/orderbook.py
--rw-r--r--   0        0        0     2779 2023-07-14 18:57:40.988914 rubi-2.1.6b2/rubi/rubicon_types/pair.py
--rw-r--r--   0        0        0    11316 2023-07-21 01:31:31.363956 rubi-2.1.6b2/rubi/rubicon_types/trade_query.py
--rw-r--r--   0        0        0     3637 1970-01-01 00:00:00.000000 rubi-2.1.6b2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-21 19:33:23.027800 rubi-2.1.7/LICENSE
+-rw-r--r--   0        0        0     2757 2023-07-21 19:33:23.027800 rubi-2.1.7/README.md
+-rw-r--r--   0        0        0     6735 2023-07-21 19:33:23.031800 rubi-2.1.7/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-07-21 19:33:23.031800 rubi-2.1.7/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-07-21 19:33:23.031800 rubi-2.1.7/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-21 19:33:23.031800 rubi-2.1.7/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      833 2023-07-21 19:33:23.031800 rubi-2.1.7/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-21 19:33:23.031800 rubi-2.1.7/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-21 19:33:23.031800 rubi-2.1.7/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      858 2023-07-21 19:33:23.031800 rubi-2.1.7/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-21 19:33:23.031800 rubi-2.1.7/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-21 19:33:23.031800 rubi-2.1.7/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      760 2023-07-21 19:33:23.031800 rubi-2.1.7/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-21 19:33:23.031800 rubi-2.1.7/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-21 19:33:23.031800 rubi-2.1.7/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      832 2023-07-21 19:33:23.031800 rubi-2.1.7/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0     1746 2023-07-21 19:33:50.312103 rubi-2.1.7/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/__init__.py
+-rw-r--r--   0        0        0    29209 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/client.py
+-rw-r--r--   0        0        0      163 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    65755 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    12261 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0       74 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/contracts/contract_types/__init__.py
+-rw-r--r--   0        0        0    15898 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/contracts/contract_types/events.py
+-rw-r--r--   0        0        0     2805 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/contracts/contract_types/transaction_reciept.py
+-rw-r--r--   0        0        0    18565 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24880 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14915 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/contracts/router.py
+-rw-r--r--   0        0        0       77 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/data/README.md
+-rw-r--r--   0        0        0       31 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/data/__init__.py
+-rw-r--r--   0        0        0    10670 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/data/market.py
+-rw-r--r--   0        0        0       72 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/network/__init__.py
+-rw-r--r--   0        0        0     8450 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/network/network.py
+-rw-r--r--   0        0        0       94 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/rubicon_types/__init__.py
+-rw-r--r--   0        0        0    16249 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/rubicon_types/order.py
+-rw-r--r--   0        0        0    11554 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/rubicon_types/order_query.py
+-rw-r--r--   0        0        0     6323 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/rubicon_types/orderbook.py
+-rw-r--r--   0        0        0     2779 2023-07-21 19:33:23.031800 rubi-2.1.7/rubi/rubicon_types/pair.py
+-rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 rubi-2.1.7/PKG-INFO
```

### Comparing `rubi-2.1.6b2/LICENSE` & `rubi-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/README.md` & `rubi-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/network_config/ERC20.json` & `rubi-2.1.7/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/network_config/README.md` & `rubi-2.1.7/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/network_config/abitrum_goerli/abis/market.json` & `rubi-2.1.7/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/network_config/abitrum_goerli/abis/router.json` & `rubi-2.1.7/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/network_config/abitrum_goerli/network.yaml` & `rubi-2.1.7/network_config/abitrum_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/network_config/optimism/abis/market.json` & `rubi-2.1.7/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/network_config/optimism/abis/router.json` & `rubi-2.1.7/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/network_config/optimism/network.yaml` & `rubi-2.1.7/network_config/optimism/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/network_config/optimism_goerli/abis/market.json` & `rubi-2.1.7/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/network_config/optimism_goerli/abis/router.json` & `rubi-2.1.7/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/network_config/optimism_goerli/network.yaml` & `rubi-2.1.7/network_config/optimism_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/network_config/polygon_mumbai/abis/market.json` & `rubi-2.1.7/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/network_config/polygon_mumbai/abis/router.json` & `rubi-2.1.7/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/network_config/polygon_mumbai/network.yaml` & `rubi-2.1.7/network_config/polygon_mumbai/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/pyproject.toml` & `rubi-2.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.1.6b2"
+version = "2.1.7"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `rubi-2.1.6b2/rubi/client.py` & `rubi-2.1.7/rubi/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -685,55 +685,14 @@
             first,
             order_by,
             order_direction,
             formatted,
         )
         return df
 
-    def get_trades(
-        self,
-        first: int = 1000,
-        order_by: str = "timestamp",
-        order_direction: str = "desc",
-        formatted: bool = True,
-        book_side: OrderSide = OrderSide.NEUTRAL,
-        taker: Optional[str] = None,
-        from_address: Optional[str] = None,
-        pair_name: Optional[str] = None,        
-        start_time: Optional[int] = None,
-        end_time: Optional[int] = None,
-
-    ) -> pd.DataFrame:
-        
-        # handle the pair_name parameter
-        if pair_name:
-            base, quote = pair_name.split("/")
-            base_asset = ERC20.from_network(name=base, network=self.network)
-            quote_asset = ERC20.from_network(name=quote, network=self.network)
-        
-        # throw an error if the pair does not exist
-        if base_asset is None or quote_asset is None:
-            raise Exception(f"Pair {pair_name} does not exist")
-
-        df = self.market_data.get_trades(
-            taker=taker,
-            from_address=from_address,
-            pair_name=pair_name,
-            book_side=book_side,
-            take_gem=base_asset.address,
-            give_gem=quote_asset.address,
-            start_time=start_time,
-            end_time=end_time,
-            first=first,
-            order_by=order_by,
-            order_direction=order_direction,
-            formatted=formatted,
-        )
-        return df
-
     ######################################################################
     # helper methods
     ######################################################################
 
     def get_network_tokens(
         self,
     ) -> Dict[ChecksumAddress, ERC20]:
```

### Comparing `rubi-2.1.6b2/rubi/contracts/aid.py` & `rubi-2.1.7/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/rubi/contracts/base_contract.py` & `rubi-2.1.7/rubi/contracts/base_contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 from typing import Optional, Callable, Type, Dict, Any
 
 from eth_account.datastructures import SignedTransaction
 from eth_typing import ChecksumAddress
 from web3 import Web3
 from web3._utils.filters import LogFilter  # noqa
 from web3.contract import Contract
-from web3.contract.contract import (
-    ContractFunction,
-)  # TODO: figure out why jupyter notebook is complaining about this
+from web3.contract.contract import ContractFunction
 from web3.types import ABI, Nonce
 
 from rubi.contracts.contract_types import BaseEvent, TransactionReceipt
 
 
 class BaseContract:
     """Base class representation of a contract which defines the structure of a contract and provides several helpful
```

### Comparing `rubi-2.1.6b2/rubi/contracts/contract_types/events.py` & `rubi-2.1.7/rubi/contracts/contract_types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/rubi/contracts/contract_types/transaction_reciept.py` & `rubi-2.1.7/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/rubi/contracts/erc20.py` & `rubi-2.1.7/rubi/contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/rubi/contracts/market.py` & `rubi-2.1.7/rubi/contracts/market.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
     def offer(
         self,
         pay_amt: int,
         pay_gem: ChecksumAddress,
         buy_amt: int,
         buy_gem: ChecksumAddress,
         pos: int = 0,
-        rounding: bool = True,
+        rounding: bool = False,
         owner: Optional[ChecksumAddress] = None,
         recipient: Optional[ChecksumAddress] = None,
         nonce: Optional[int] = None,
         gas: Optional[int] = None,
         max_fee_per_gas: Optional[int] = None,
         max_priority_fee_per_gas: Optional[int] = None,
     ) -> TransactionReceipt:
@@ -237,15 +237,15 @@
         :param buy_amt: the amount of the token being bought
         :type buy_amt: int
         :param buy_gem: the address of the token being bought
         :type buy_gem: ChecksumAddress
         :param pos: position of the offer in the linked list, default to 0 unless the maker knows the position they want
             to insert the offer at
         :type pos: int
-        :param rounding: add rounding to match "close enough" orders, defaults to True
+        :param rounding: add rounding to match "close enough" orders, defaults to False
         :type: rounding: bool
         :param owner: the owner of the offer, defaults to the wallet that was provided in instantiating this class.
             (optional, default is None)
         :type owner: Optional[ChecksumAddress]
         :param recipient: the recipient of the offer's fill, defaults to the wallet that was provided in instantiating
             this class (optional, default is None)
         :type recipient: Optional[ChecksumAddress]
```

### Comparing `rubi-2.1.6b2/rubi/contracts/router.py` & `rubi-2.1.7/rubi/contracts/router.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/rubi/data/market.py` & `rubi-2.1.7/rubi/data/market.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 )
 from rubi.network import (
     Network,
 )
 from rubi.rubicon_types import (
     OrderSide,
     OrderQuery,
-    TradeQuery,
 )
 
 
 class MarketData:
     """This class represents the RubiconV2 Subgraph, which contains data primarily related to the RubiconMarket.sol
     contract. If a Network object is not passed in instantiation then this class will only be used to query data related
      to the subgraph.
@@ -62,15 +61,14 @@
                     except:
                         raise ValueError(
                             f"Both subgraph_url: {self.subgraph_url} and fallback_url: {self.subgraph_fallback_url} failed when attempting to load. Error: {str(e)}"
                         )
 
         # Initialize the query classes
         self.offer_query = OrderQuery(self.sg, self.data, self.network, self.tokens)
-        self.trade_query = TradeQuery(self.sg, self.data, self.network, self.tokens)
 
     @classmethod
     def from_network_with_tokens(
         cls, network: Network, network_tokens: Dict[ChecksumAddress, ERC20]
     ) -> "MarketData":
         """Initialize a MarketData object using a Network object."""
         return cls(
@@ -87,15 +85,15 @@
 
     # TODO: refactor using a decorator to handle the parameter validation
     def get_offers(
         self,
         maker: Optional[str] = None,
         from_address: Optional[str] = None,
         pair_name: Optional[str] = None,
-        book_side: Optional[OrderSide] = OrderSide.NEUTRAL,
+        book_side: Optional[OrderSide] = None,
         pay_gem: Optional[
             str
         ] = None,  # TODO: maybe we should allow the user to pass in an address here?
         buy_gem: Optional[
             str
         ] = None,  # TODO: maybe we should allow the user to pass in an address here?
         open: Optional[bool] = None,
@@ -143,17 +141,15 @@
         # handle the pair_name parameter
         if pair_name:
             base, quote = pair_name.split("/")
             base_asset = ERC20.from_network(name=base, network=self.network)
             quote_asset = ERC20.from_network(name=quote, network=self.network)
 
         # handle the book_side parameter
-        if (
-            book_side and pair_name
-        ):  # TODO: we need to handle the case where neither of these are passed
+        if book_side and pair_name:
             match book_side:
                 case OrderSide.BUY:
                     buy_query = self.offer_query.offers_query(
                         order_by,
                         order_direction,
                         first,
                         maker,
@@ -249,136 +245,7 @@
                 start_time=start_time,
                 end_time=end_time,
             )
             fields = self.offer_query.offers_fields(query)
             df = self.offer_query.query_offers(fields)
 
             return df
-
-    def get_trades(
-        self,
-        taker: Optional[str] = None,
-        from_address: Optional[str] = None,
-        pair_name: Optional[str] = None,
-        book_side: Optional[OrderSide] = OrderSide.NEUTRAL,
-        take_gem: Optional[
-            str
-        ] = None,  # TODO: not sure we really need this given the pair_name parameter
-        give_gem: Optional[
-            str
-        ] = None,  # TODO: not sure we really need this given the pair_name parameter
-        start_time: Optional[int] = None,
-        end_time: Optional[int] = None,
-        first: Optional[
-            int
-        ] = 1000,  # TODO: maybe this should be a large number by default?
-        order_by: Optional[str] = "timestamp",
-        order_direction: Optional[str] = "desc",
-        formatted: Optional[bool] = False,
-    ) -> pd.DataFrame:
-        """Returns a dataframe of trades that have occurred on the market contract, with the option to pass in filters.
-
-        :param taker: the address of the taker of the trade
-        :type taker: str
-        :param from_address: the address that originated the transaction that created the trade
-        :type from_address: str
-        :param pair_name: the name of the pair that the trade occurred on (will override take_gem and give_gem if both are passed)
-        :type pair_name: str
-        :param book_side: the side of the order book that the trade occurred on (defaults to neutral, options: buy, sell, neutral)
-        :type book_side: OrderSide
-        :param take_gem: the address of the token that the taker received
-        :type take_gem: str
-        :param give_gem: the address of the token that the taker gave
-        :type give_gem: str
-        :param start_time: the timestamp of the earliest trade to return
-        :type start_time: int
-        :param end_time: the timestamp of the latest trade to return
-        :type end_time: int
-        :param first: the number of trades to return
-        :type first: int
-        :param order_by: the field to order the trades by (default: timestamp, options: timestamp) TODO: expand this list
-        :type order_by: str
-        :param order_direction: the direction to order the trades by (default: desc, options: asc, desc)
-        :type order_direction: str
-        :param formatted: whether or not to return the formatted fields (default: False, requires a network object to be passed)
-        :type formatted: bool
-        :return: a dataframe of trades that have occurred on the market contract
-        :rtype: pd.DataFrame
-        """
-
-        # if we want formatted fields, make sure we have a network object
-        if formatted and not self.network:
-            raise ValueError(
-                "Cannot return formatted fields without a network object initialized on the class."
-            )
-    
-        match book_side:
-            case OrderSide.BUY:
-                buy_query = self.trade_query.trades_query(
-                    order_by,
-                    order_direction,
-                    first,
-                    taker,
-                    from_address,
-                    take_gem=take_gem,
-                    give_gem=give_gem,
-                    start_time=start_time,
-                    end_time=end_time,
-                )
-                buy_fields = self.trade_query.trades_fields(buy_query, formatted)
-                buy_df = self.trade_query.query_trades(buy_fields, formatted)
-                buy_df["side"] = "buy"
-
-                return buy_df
-
-            case OrderSide.SELL:
-                sell_query = self.trade_query.trades_query(
-                    order_by,
-                    order_direction,
-                    first,
-                    taker,
-                    from_address,
-                    take_gem=give_gem,
-                    give_gem=take_gem,
-                    start_time=start_time,
-                    end_time=end_time,
-                )
-                sell_fields = self.trade_query.trades_fields(sell_query, formatted)
-                sell_df = self.trade_query.query_trades(sell_fields, formatted)
-                sell_df["side"] = "sell"
-
-                return sell_df
-
-            case OrderSide.NEUTRAL:
-                buy_query = self.trade_query.trades_query(
-                    order_by,
-                    order_direction,
-                    first,  # TODO: decide if we only want to pass half the values here
-                    taker,
-                    from_address,
-                    take_gem=take_gem,
-                    give_gem=give_gem,
-                    start_time=start_time,
-                    end_time=end_time,
-                )
-                buy_fields = self.trade_query.trades_fields(buy_query, formatted)
-                buy_df = self.trade_query.query_trades(buy_fields, formatted)
-                buy_df["side"] = "buy"
-
-                sell_query = self.trade_query.trades_query(
-                    order_by,
-                    order_direction,
-                    first,
-                    taker,
-                    from_address,
-                    take_gem=give_gem,
-                    give_gem=take_gem,
-                    start_time=start_time,
-                    end_time=end_time,
-                )
-                sell_fields = self.trade_query.trades_fields(sell_query, formatted)
-                sell_df = self.trade_query.query_trades(sell_fields, formatted)
-                sell_df["side"] = "sell"
-
-                return pd.concat([buy_df, sell_df]).reset_index(
-                    drop=True
-                )  # TODO: decide what we want to do here, maybe we just return both dataframes?
```

### Comparing `rubi-2.1.6b2/rubi/network/network.py` & `rubi-2.1.7/rubi/network/network.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/rubi/rubicon_types/order.py` & `rubi-2.1.7/rubi/rubicon_types/order.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,25 @@
 
             case OrderSide.BUY:
                 return 1
 
             case OrderSide.SELL:
                 return -1
 
+    def opposite(self) -> "OrderSide":
+        match self:
+            case OrderSide.NEUTRAL:
+                return OrderSide.NEUTRAL
+
+            case OrderSide.BUY:
+                return OrderSide.SELL
+
+            case OrderSide.SELL:
+                return OrderSide.BUY
+
 
 class OrderType(Enum):
     """Enumeration representing the order type."""
 
     MARKET = "MARKET"
     LIMIT = "LIMIT"
 
@@ -133,14 +144,18 @@
             order_type=OrderType.LIMIT,
             order_side=order_side,
         )
 
         self.size = size
         self.price = price
 
+    def __repr__(self):
+        items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
+        return "{}({})".format(type(self).__name__, ", ".join(items))
+
 
 class UpdateLimitOrder(BaseNewOrder):
     """Class representing an update to an existing limit order
 
     :param pair_name: The name of the pair being traded e.g. WETH/USDC.
     :type pair_name: str
     :param order_side: The side of the order (BUY or SELL).
```

### Comparing `rubi-2.1.6b2/rubi/rubicon_types/order_query.py` & `rubi-2.1.7/rubi/rubicon_types/order_query.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/rubi/rubicon_types/orderbook.py` & `rubi-2.1.7/rubi/rubicon_types/orderbook.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/rubi/rubicon_types/pair.py` & `rubi-2.1.7/rubi/rubicon_types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b2/PKG-INFO` & `rubi-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.1.6b2
+Version: 2.1.7
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

