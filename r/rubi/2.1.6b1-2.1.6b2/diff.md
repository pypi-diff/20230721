# Comparing `tmp/rubi-2.1.6b1.tar.gz` & `tmp/rubi-2.1.6b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.1.6b1.tar", max compression
+gzip compressed data, was "rubi-2.1.6b2.tar", max compression
```

## Comparing `rubi-2.1.6b1.tar` & `rubi-2.1.6b2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.1.6b1/LICENSE
--rw-r--r--   0        0        0     2757 2023-07-18 23:38:58.047336 rubi-2.1.6b1/README.md
--rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.1.6b1/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.1.6b1/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.1.6b1/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.1.6b1/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      833 2023-07-19 19:13:00.615720 rubi-2.1.6b1/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.1.6b1/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.1.6b1/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      858 2023-07-19 19:13:00.615912 rubi-2.1.6b1/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.1.6b1/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.1.6b1/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      760 2023-07-19 19:13:00.616134 rubi-2.1.6b1/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.1.6b1/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.1.6b1/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      832 2023-07-19 19:13:00.616334 rubi-2.1.6b1/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0     1748 2023-07-19 19:13:56.019109 rubi-2.1.6b1/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-07 13:58:54.647129 rubi-2.1.6b1/rubi/__init__.py
--rw-r--r--   0        0        0    30130 2023-07-19 19:12:54.492656 rubi-2.1.6b1/rubi/client.py
--rw-r--r--   0        0        0      163 2023-06-30 02:50:06.554484 rubi-2.1.6b1/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    65755 2023-07-14 18:57:40.986583 rubi-2.1.6b1/rubi/contracts/aid.py
--rw-r--r--   0        0        0    12337 2023-07-19 19:12:54.493238 rubi-2.1.6b1/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0       74 2023-07-04 04:06:47.229802 rubi-2.1.6b1/rubi/contracts/contract_types/__init__.py
--rw-r--r--   0        0        0    15898 2023-07-14 18:57:40.986973 rubi-2.1.6b1/rubi/contracts/contract_types/events.py
--rw-r--r--   0        0        0     2805 2023-07-14 18:57:40.987143 rubi-2.1.6b1/rubi/contracts/contract_types/transaction_reciept.py
--rw-r--r--   0        0        0    18565 2023-07-14 20:13:22.360534 rubi-2.1.6b1/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24878 2023-07-14 18:57:40.987497 rubi-2.1.6b1/rubi/contracts/market.py
--rw-r--r--   0        0        0    14915 2023-07-14 18:57:40.987660 rubi-2.1.6b1/rubi/contracts/router.py
--rw-r--r--   0        0        0       77 2023-07-07 13:58:54.648079 rubi-2.1.6b1/rubi/data/README.md
--rw-r--r--   0        0        0       31 2023-07-07 13:58:54.648312 rubi-2.1.6b1/rubi/data/__init__.py
--rw-r--r--   0        0        0    17887 2023-07-19 19:13:00.616618 rubi-2.1.6b1/rubi/data/market.py
--rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.1.6b1/rubi/network/__init__.py
--rw-r--r--   0        0        0     8450 2023-07-19 19:13:00.616853 rubi-2.1.6b1/rubi/network/network.py
--rw-r--r--   0        0        0      121 2023-07-19 19:12:54.494446 rubi-2.1.6b1/rubi/rubicon_types/__init__.py
--rw-r--r--   0        0        0    15796 2023-07-15 17:29:20.578781 rubi-2.1.6b1/rubi/rubicon_types/order.py
--rw-r--r--   0        0        0    11554 2023-07-15 17:29:20.579083 rubi-2.1.6b1/rubi/rubicon_types/order_query.py
--rw-r--r--   0        0        0     6323 2023-07-15 17:29:20.579349 rubi-2.1.6b1/rubi/rubicon_types/orderbook.py
--rw-r--r--   0        0        0     2779 2023-07-14 18:57:40.988914 rubi-2.1.6b1/rubi/rubicon_types/pair.py
--rw-r--r--   0        0        0    11355 2023-07-19 19:12:54.494738 rubi-2.1.6b1/rubi/rubicon_types/trade_query.py
--rw-r--r--   0        0        0     3637 1970-01-01 00:00:00.000000 rubi-2.1.6b1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.1.6b2/LICENSE
+-rw-r--r--   0        0        0     2757 2023-07-18 23:38:58.047336 rubi-2.1.6b2/README.md
+-rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.1.6b2/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.1.6b2/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.1.6b2/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.1.6b2/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      833 2023-07-19 19:13:00.615720 rubi-2.1.6b2/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.1.6b2/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.1.6b2/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      858 2023-07-19 19:13:00.615912 rubi-2.1.6b2/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.1.6b2/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.1.6b2/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      760 2023-07-19 19:13:00.616134 rubi-2.1.6b2/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.1.6b2/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.1.6b2/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      832 2023-07-19 19:13:00.616334 rubi-2.1.6b2/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0     1748 2023-07-21 01:34:06.171481 rubi-2.1.6b2/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-07 13:58:54.647129 rubi-2.1.6b2/rubi/__init__.py
+-rw-r--r--   0        0        0    30603 2023-07-21 01:25:04.169604 rubi-2.1.6b2/rubi/client.py
+-rw-r--r--   0        0        0      163 2023-06-30 02:50:06.554484 rubi-2.1.6b2/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    65755 2023-07-14 18:57:40.986583 rubi-2.1.6b2/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    12337 2023-07-19 19:12:54.493238 rubi-2.1.6b2/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0       74 2023-07-04 04:06:47.229802 rubi-2.1.6b2/rubi/contracts/contract_types/__init__.py
+-rw-r--r--   0        0        0    15898 2023-07-14 18:57:40.986973 rubi-2.1.6b2/rubi/contracts/contract_types/events.py
+-rw-r--r--   0        0        0     2805 2023-07-14 18:57:40.987143 rubi-2.1.6b2/rubi/contracts/contract_types/transaction_reciept.py
+-rw-r--r--   0        0        0    18565 2023-07-14 20:13:22.360534 rubi-2.1.6b2/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24878 2023-07-20 19:29:23.201977 rubi-2.1.6b2/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14915 2023-07-14 18:57:40.987660 rubi-2.1.6b2/rubi/contracts/router.py
+-rw-r--r--   0        0        0       77 2023-07-07 13:58:54.648079 rubi-2.1.6b2/rubi/data/README.md
+-rw-r--r--   0        0        0       31 2023-07-07 13:58:54.648312 rubi-2.1.6b2/rubi/data/__init__.py
+-rw-r--r--   0        0        0    16515 2023-07-21 01:14:16.995206 rubi-2.1.6b2/rubi/data/market.py
+-rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.1.6b2/rubi/network/__init__.py
+-rw-r--r--   0        0        0     8450 2023-07-20 19:31:29.720610 rubi-2.1.6b2/rubi/network/network.py
+-rw-r--r--   0        0        0      121 2023-07-19 19:12:54.494446 rubi-2.1.6b2/rubi/rubicon_types/__init__.py
+-rw-r--r--   0        0        0    15796 2023-07-15 17:29:20.578781 rubi-2.1.6b2/rubi/rubicon_types/order.py
+-rw-r--r--   0        0        0    11554 2023-07-15 17:29:20.579083 rubi-2.1.6b2/rubi/rubicon_types/order_query.py
+-rw-r--r--   0        0        0     6323 2023-07-15 17:29:20.579349 rubi-2.1.6b2/rubi/rubicon_types/orderbook.py
+-rw-r--r--   0        0        0     2779 2023-07-14 18:57:40.988914 rubi-2.1.6b2/rubi/rubicon_types/pair.py
+-rw-r--r--   0        0        0    11316 2023-07-21 01:31:31.363956 rubi-2.1.6b2/rubi/rubicon_types/trade_query.py
+-rw-r--r--   0        0        0     3637 1970-01-01 00:00:00.000000 rubi-2.1.6b2/PKG-INFO
```

### Comparing `rubi-2.1.6b1/LICENSE` & `rubi-2.1.6b2/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/README.md` & `rubi-2.1.6b2/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/network_config/ERC20.json` & `rubi-2.1.6b2/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/network_config/README.md` & `rubi-2.1.6b2/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/network_config/abitrum_goerli/abis/market.json` & `rubi-2.1.6b2/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/network_config/abitrum_goerli/abis/router.json` & `rubi-2.1.6b2/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/network_config/abitrum_goerli/network.yaml` & `rubi-2.1.6b2/network_config/abitrum_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/network_config/optimism/abis/market.json` & `rubi-2.1.6b2/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/network_config/optimism/abis/router.json` & `rubi-2.1.6b2/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/network_config/optimism/network.yaml` & `rubi-2.1.6b2/network_config/optimism/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/network_config/optimism_goerli/abis/market.json` & `rubi-2.1.6b2/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/network_config/optimism_goerli/abis/router.json` & `rubi-2.1.6b2/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/network_config/optimism_goerli/network.yaml` & `rubi-2.1.6b2/network_config/optimism_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/network_config/polygon_mumbai/abis/market.json` & `rubi-2.1.6b2/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/network_config/polygon_mumbai/abis/router.json` & `rubi-2.1.6b2/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/network_config/polygon_mumbai/network.yaml` & `rubi-2.1.6b2/network_config/polygon_mumbai/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/pyproject.toml` & `rubi-2.1.6b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.1.6b1"
+version = "2.1.6b2"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `rubi-2.1.6b1/rubi/client.py` & `rubi-2.1.6b2/rubi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -687,40 +687,50 @@
             order_direction,
             formatted,
         )
         return df
 
     def get_trades(
         self,
+        first: int = 1000,
+        order_by: str = "timestamp",
+        order_direction: str = "desc",
+        formatted: bool = True,
+        book_side: OrderSide = OrderSide.NEUTRAL,
         taker: Optional[str] = None,
         from_address: Optional[str] = None,
-        pair_name: Optional[str] = None,
-        book_side: Optional[OrderSide] = OrderSide.NEUTRAL,
-        take_gem: Optional[str] = None,
-        give_gem: Optional[str] = None,
+        pair_name: Optional[str] = None,        
         start_time: Optional[int] = None,
         end_time: Optional[int] = None,
-        first: Optional[int] = 1000,
-        order_by: Optional[str] = "timestamp",
-        order_direction: Optional[str] = "desc",
-        formatted: Optional[bool] = True,
+
     ) -> pd.DataFrame:
+        
+        # handle the pair_name parameter
+        if pair_name:
+            base, quote = pair_name.split("/")
+            base_asset = ERC20.from_network(name=base, network=self.network)
+            quote_asset = ERC20.from_network(name=quote, network=self.network)
+        
+        # throw an error if the pair does not exist
+        if base_asset is None or quote_asset is None:
+            raise Exception(f"Pair {pair_name} does not exist")
+
         df = self.market_data.get_trades(
-            taker,
-            from_address,
-            pair_name,
-            book_side,
-            take_gem,
-            give_gem,
-            start_time,
-            end_time,
-            first,
-            order_by,
-            order_direction,
-            formatted,
+            taker=taker,
+            from_address=from_address,
+            pair_name=pair_name,
+            book_side=book_side,
+            take_gem=base_asset.address,
+            give_gem=quote_asset.address,
+            start_time=start_time,
+            end_time=end_time,
+            first=first,
+            order_by=order_by,
+            order_direction=order_direction,
+            formatted=formatted,
         )
         return df
 
     ######################################################################
     # helper methods
     ######################################################################
```

### Comparing `rubi-2.1.6b1/rubi/contracts/aid.py` & `rubi-2.1.6b2/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/rubi/contracts/base_contract.py` & `rubi-2.1.6b2/rubi/contracts/base_contract.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/rubi/contracts/contract_types/events.py` & `rubi-2.1.6b2/rubi/contracts/contract_types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/rubi/contracts/contract_types/transaction_reciept.py` & `rubi-2.1.6b2/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/rubi/contracts/erc20.py` & `rubi-2.1.6b2/rubi/contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/rubi/contracts/market.py` & `rubi-2.1.6b2/rubi/contracts/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/rubi/contracts/router.py` & `rubi-2.1.6b2/rubi/contracts/router.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/rubi/data/market.py` & `rubi-2.1.6b2/rubi/data/market.py`

 * *Files 4% similar despite different names*

```diff
@@ -306,107 +306,79 @@
         """
 
         # if we want formatted fields, make sure we have a network object
         if formatted and not self.network:
             raise ValueError(
                 "Cannot return formatted fields without a network object initialized on the class."
             )
-
-        # handle the pair_name parameter
-        if pair_name:
-            base, quote = pair_name.split("/")
-            base_asset = ERC20.from_network(name=base, network=self.network)
-            quote_asset = ERC20.from_network(name=quote, network=self.network)
-
-        # handle the book_side parameter
-        if (
-            book_side and pair_name
-        ):  # TODO: we need to handle the case where neither of these are passed
-            match book_side:
-                case OrderSide.BUY:
-                    buy_query = self.trade_query.trades_query(
-                        order_by,
-                        order_direction,
-                        first,
-                        taker,
-                        from_address,
-                        take_gem=base_asset.address,
-                        give_gem=quote_asset.address,
-                        start_time=start_time,
-                        end_time=end_time,
-                    )
-                    buy_fields = self.trade_query.trades_fields(buy_query, formatted)
-                    buy_df = self.trade_query.query_trades(buy_fields, formatted)
-                    buy_df["side"] = "buy"
-
-                    return buy_df
-
-                case OrderSide.SELL:
-                    sell_query = self.trade_query.trades_query(
-                        order_by,
-                        order_direction,
-                        first,
-                        taker,
-                        from_address,
-                        take_gem=quote_asset.address,
-                        give_gem=base_asset.address,
-                        start_time=start_time,
-                        end_time=end_time,
-                    )
-                    sell_fields = self.trade_query.trades_fields(sell_query, formatted)
-                    sell_df = self.trade_query.query_trades(sell_fields, formatted)
-                    sell_df["side"] = "sell"
-
-                    return sell_df
-
-                case OrderSide.NEUTRAL:
-                    buy_query = self.trade_query.trades_query(
-                        order_by,
-                        order_direction,
-                        first,  # TODO: decide if we only want to pass half the values here
-                        taker,
-                        from_address,
-                        take_gem=base_asset.address,
-                        give_gem=quote_asset.address,
-                        start_time=start_time,
-                        end_time=end_time,
-                    )
-                    buy_fields = self.trade_query.trades_fields(buy_query, formatted)
-                    buy_df = self.trade_query.query_trades(buy_fields, formatted)
-                    buy_df["side"] = "buy"
-
-                    sell_query = self.trade_query.trades_query(
-                        order_by,
-                        order_direction,
-                        first,
-                        taker,
-                        from_address,
-                        take_gem=quote_asset.address,
-                        give_gem=base_asset.address,
-                        start_time=start_time,
-                        end_time=end_time,
-                    )
-                    sell_fields = self.trade_query.trades_fields(sell_query, formatted)
-                    sell_df = self.trade_query.query_trades(sell_fields, formatted)
-                    sell_df["side"] = "sell"
-
-                    return pd.concat([buy_df, sell_df]).reset_index(
-                        drop=True
-                    )  # TODO: decide what we want to do here, maybe we just return both dataframes?
-
-        # handle the take_gem and give_gem parameters
-        elif take_gem and give_gem:
-            query = self.trade_query.trades_query(
-                order_by,
-                order_direction,
-                first,
-                taker,
-                from_address,
-                take_gem=take_gem,
-                give_gem=give_gem,
-                start_time=start_time,
-                end_time=end_time,
-            )
-            fields = self.trade_query.trades_fields(query, formatted)
-            df = self.trade_query.query_trades(fields, formatted)
-
-            return df
+    
+        match book_side:
+            case OrderSide.BUY:
+                buy_query = self.trade_query.trades_query(
+                    order_by,
+                    order_direction,
+                    first,
+                    taker,
+                    from_address,
+                    take_gem=take_gem,
+                    give_gem=give_gem,
+                    start_time=start_time,
+                    end_time=end_time,
+                )
+                buy_fields = self.trade_query.trades_fields(buy_query, formatted)
+                buy_df = self.trade_query.query_trades(buy_fields, formatted)
+                buy_df["side"] = "buy"
+
+                return buy_df
+
+            case OrderSide.SELL:
+                sell_query = self.trade_query.trades_query(
+                    order_by,
+                    order_direction,
+                    first,
+                    taker,
+                    from_address,
+                    take_gem=give_gem,
+                    give_gem=take_gem,
+                    start_time=start_time,
+                    end_time=end_time,
+                )
+                sell_fields = self.trade_query.trades_fields(sell_query, formatted)
+                sell_df = self.trade_query.query_trades(sell_fields, formatted)
+                sell_df["side"] = "sell"
+
+                return sell_df
+
+            case OrderSide.NEUTRAL:
+                buy_query = self.trade_query.trades_query(
+                    order_by,
+                    order_direction,
+                    first,  # TODO: decide if we only want to pass half the values here
+                    taker,
+                    from_address,
+                    take_gem=take_gem,
+                    give_gem=give_gem,
+                    start_time=start_time,
+                    end_time=end_time,
+                )
+                buy_fields = self.trade_query.trades_fields(buy_query, formatted)
+                buy_df = self.trade_query.query_trades(buy_fields, formatted)
+                buy_df["side"] = "buy"
+
+                sell_query = self.trade_query.trades_query(
+                    order_by,
+                    order_direction,
+                    first,
+                    taker,
+                    from_address,
+                    take_gem=give_gem,
+                    give_gem=take_gem,
+                    start_time=start_time,
+                    end_time=end_time,
+                )
+                sell_fields = self.trade_query.trades_fields(sell_query, formatted)
+                sell_df = self.trade_query.query_trades(sell_fields, formatted)
+                sell_df["side"] = "sell"
+
+                return pd.concat([buy_df, sell_df]).reset_index(
+                    drop=True
+                )  # TODO: decide what we want to do here, maybe we just return both dataframes?
```

### Comparing `rubi-2.1.6b1/rubi/network/network.py` & `rubi-2.1.6b2/rubi/network/network.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/rubi/rubicon_types/order.py` & `rubi-2.1.6b2/rubi/rubicon_types/order.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/rubi/rubicon_types/order_query.py` & `rubi-2.1.6b2/rubi/rubicon_types/order_query.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/rubi/rubicon_types/orderbook.py` & `rubi-2.1.6b2/rubi/rubicon_types/orderbook.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/rubi/rubicon_types/pair.py` & `rubi-2.1.6b2/rubi/rubicon_types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.6b1/rubi/rubicon_types/trade_query.py` & `rubi-2.1.6b2/rubi/rubicon_types/trade_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,37 +296,33 @@
             df.columns = [col.replace("_id", "") for col in df.columns]
 
             # TODO: decide whether we should return the unformatted fields or not
             if formatted:
                 df = df.drop(
                     columns=[
                         "id",
-                        "take_amt",
-                        "give_amt",
-                        "take_gem",
-                        "give_gem",
-                        "timestamp",
-                        "index",
-                        "transaction_block_number",
-                        "transaction_block_index",
-                        "offer_transaction_block_number",
-                        "offer_transaction_block_index",
-                        "offer_index",
                     ]
                 )
                 df = df.rename(
                     columns={
                         "take_amt_formatted": "take_amt",
                         "give_amt_formatted": "give_amt",
+                        "take_gem_raw": "take_gem",
+                        "give_gem_raw": "give_gem",
                         "take_gem_symbol": "take_gem",
                         "give_gem_symbol": "give_gem",
+                        "take_gem_address": "take_gem",
+                        "give_gem_address": "give_gem",
                         "datetime": "timestamp",
                         "index": "log_index",
                         "transaction_block_number": "block_number",
                         "transaction_block_index": "block_index",
+                        "offer_transaction_block_number": "offer_block_number",
+                        "offer_transaction_block_index": "offer_block_index",
+                        "offer_index": "offer_log_index",
                     }
                 )
                 # TODO: we could also get smart with displaying price dependent upon the pair_name and direction of the
                 #  order
 
         # TODO: apply any data type conversions to the dataframe - possibly converting unformatted values to integers
         return df
```

### Comparing `rubi-2.1.6b1/PKG-INFO` & `rubi-2.1.6b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.1.6b1
+Version: 2.1.6b2
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

