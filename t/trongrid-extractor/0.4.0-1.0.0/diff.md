# Comparing `tmp/trongrid_extractor-0.4.0.tar.gz` & `tmp/trongrid_extractor-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trongrid_extractor-0.4.0.tar", max compression
+gzip compressed data, was "trongrid_extractor-1.0.0.tar", max compression
```

## Comparing `trongrid_extractor-0.4.0.tar` & `trongrid_extractor-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1742 2023-07-02 01:23:16.068613 trongrid_extractor-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-0.4.0/LICENSE
--rw-r--r--   0        0        0     3788 2023-06-29 06:44:04.355607 trongrid_extractor-0.4.0/README.md
--rw-r--r--   0        0        0      710 2023-07-02 01:23:16.074603 trongrid_extractor-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      664 2023-07-02 01:06:33.646837 trongrid_extractor-0.4.0/trongrid_extractor/__init__.py
--rw-r--r--   0        0        0    10728 2023-07-02 00:36:08.783069 trongrid_extractor-0.4.0/trongrid_extractor/api.py
--rw-r--r--   0        0        0      256 2023-07-02 01:07:20.257342 trongrid_extractor-0.4.0/trongrid_extractor/config.py
--rw-r--r--   0        0        0     2416 2023-07-02 00:28:20.059440 trongrid_extractor-0.4.0/trongrid_extractor/helpers/address_helpers.py
--rw-r--r--   0        0        0     3281 2023-07-02 01:08:44.223494 trongrid_extractor-0.4.0/trongrid_extractor/helpers/argument_parser.py
--rw-r--r--   0        0        0     2177 2023-07-01 03:19:57.513786 trongrid_extractor-0.4.0/trongrid_extractor/helpers/csv_helper.py
--rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-0.4.0/trongrid_extractor/helpers/dict_helper.py
--rw-r--r--   0        0        0      328 2023-07-02 00:33:07.504060 trongrid_extractor-0.4.0/trongrid_extractor/helpers/rich_helpers.py
--rw-r--r--   0        0        0      408 2023-07-01 19:49:23.669130 trongrid_extractor-0.4.0/trongrid_extractor/helpers/string_constants.py
--rw-r--r--   0        0        0     1726 2023-07-02 01:02:30.797593 trongrid_extractor-0.4.0/trongrid_extractor/helpers/time_helpers.py
--rw-r--r--   0        0        0     4339 2023-07-02 00:33:40.029157 trongrid_extractor-0.4.0/trongrid_extractor/progress_tracker.py
--rw-r--r--   0        0        0     1781 2023-07-01 22:52:26.788565 trongrid_extractor-0.4.0/trongrid_extractor/request_params.py
--rw-r--r--   0        0        0     5531 2023-07-01 22:28:24.965541 trongrid_extractor-0.4.0/trongrid_extractor/response.py
--rw-r--r--   0        0        0     4544 2023-07-02 00:25:20.662207 trongrid_extractor-0.4.0/trongrid_extractor/trc20_txn.py
--rw-r--r--   0        0        0     4430 1970-01-01 00:00:00.000000 trongrid_extractor-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2082 2023-07-21 04:07:56.103083 trongrid_extractor-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-06-27 21:57:40.566976 trongrid_extractor-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4285 2023-07-20 21:33:51.204396 trongrid_extractor-1.0.0/README.md
+-rw-r--r--   0        0        0      710 2023-07-21 04:09:20.260330 trongrid_extractor-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      664 2023-07-07 20:10:24.551800 trongrid_extractor-1.0.0/trongrid_extractor/__init__.py
+-rw-r--r--   0        0        0     6306 2023-07-21 03:53:28.444528 trongrid_extractor-1.0.0/trongrid_extractor/api.py
+-rw-r--r--   0        0        0      256 2023-07-02 01:07:20.257342 trongrid_extractor-1.0.0/trongrid_extractor/config.py
+-rw-r--r--   0        0        0     2556 2023-07-07 17:52:23.460205 trongrid_extractor-1.0.0/trongrid_extractor/helpers/address_helpers.py
+-rw-r--r--   0        0        0     3281 2023-07-07 20:10:24.552907 trongrid_extractor-1.0.0/trongrid_extractor/helpers/argument_parser.py
+-rw-r--r--   0        0        0     2282 2023-07-21 03:57:18.162746 trongrid_extractor-1.0.0/trongrid_extractor/helpers/csv_helper.py
+-rw-r--r--   0        0        0      196 2023-06-28 02:11:34.501085 trongrid_extractor-1.0.0/trongrid_extractor/helpers/dict_helper.py
+-rw-r--r--   0        0        0      328 2023-07-02 00:33:07.504060 trongrid_extractor-1.0.0/trongrid_extractor/helpers/rich_helpers.py
+-rw-r--r--   0        0        0      452 2023-07-07 20:02:09.527800 trongrid_extractor-1.0.0/trongrid_extractor/helpers/string_constants.py
+-rw-r--r--   0        0        0     1726 2023-07-02 01:02:30.797593 trongrid_extractor-1.0.0/trongrid_extractor/helpers/time_helpers.py
+-rw-r--r--   0        0        0     4747 2023-07-20 22:04:21.872581 trongrid_extractor-1.0.0/trongrid_extractor/progress_tracker.py
+-rw-r--r--   0        0        0     1781 2023-07-01 22:52:26.788565 trongrid_extractor-1.0.0/trongrid_extractor/request_params.py
+-rw-r--r--   0        0        0     5248 2023-07-21 03:55:50.173322 trongrid_extractor-1.0.0/trongrid_extractor/response.py
+-rw-r--r--   0        0        0     4687 2023-07-07 18:41:19.685481 trongrid_extractor-1.0.0/trongrid_extractor/trc20_txn.py
+-rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 trongrid_extractor-1.0.0/PKG-INFO
```

### Comparing `trongrid_extractor-0.4.0/CHANGELOG.md` & `trongrid_extractor-1.0.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-# NEXT RELEASE
+# 1.0.0
+* As of mid July 2023 TronGrid seems to have repaired their API so it no longer just gives up after returning 5 pages of responses. This dramatically simplifies the code in this package.
+* Guarantee there is always a CSV with a header row at the end even if there's no rows returned by query.
+* enable `jUSDC` and `stUSDT` token shorthand symbols
 
 # 0.4.0
 * `--resume` option automatically determines the token address from the CSV
 * `--debug` option for `extract_tron_transactions` CLI
 * `--list-symbols` option for `extract_tron_transactions` CLI
 * Accept command line args without timezone (assume UTC)
 * Log count of rows extracted.
```

### Comparing `trongrid_extractor-0.4.0/README.md` & `trongrid_extractor-1.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -57,14 +57,21 @@
 ### Publishing
 1. Update `pyproject.toml` version number
 1. Update `CHANGELOG.md`
 1. `poetry publish --build --repository chain_argos_pypi`
 
 ## TODO
 1. Walk forward not backward
+1. Weird that this yielded dupes on the first page:
+   ```
+   {request_params.py:29} INFO - Request URL: https://api.trongrid.io/v1/contracts/TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t/events
+   Params requesting 'Transfer' events from 2021-04-01T04:00:01+00:00 to 2021-04-01T05:00:00+00:00 (no extra params).
+   {response.py:48} INFO - New query requesting data from 2021-04-01T04:00:01+00:00 to 2021-04-01T05:00:00+00:00.
+   {progress_tracker.py:67} INFO -   Removed 11 duplicate transactions...
+   ```
 1. USDT looks incomplete here as 9pm was the last time:
    ```
    WARNING - 0 txns found. We seem to be stuck at 2020-07-09T21:04:24+00:00.
    [2023-06-29, 06:34:36 UTC] {logging_mixin.py:137} INFO -                     WARNING    Last request params:                   api.py:127
                              {'only_confirmed': 'true', 'limit': 200,
                              'min_timestamp': 1594252801000.0,
                              'max_timestamp': 1594328664000.0,
```

### Comparing `trongrid_extractor-0.4.0/pyproject.toml` & `trongrid_extractor-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trongrid-extractor"
-version = "0.4.0"
+version = "1.0.0"
 description = "Extract transactions from the Trongrid API."
 authors = ["Chain Argos"]
 readme = "README.md"
 packages = [{include = "trongrid_extractor"}]
 homepage = "https://chainargos.com"
 
 include = [
```

### Comparing `trongrid_extractor-0.4.0/trongrid_extractor/__init__.py` & `trongrid_extractor-1.0.0/trongrid_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.4.0/trongrid_extractor/helpers/address_helpers.py` & `trongrid_extractor-1.0.0/trongrid_extractor/helpers/address_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """
+Methods to work with tron addresses.
 https://stackoverflow.com/questions/57200685/how-to-convert-tron-address-to-different-format
 """
 import logging
 from typing import Optional
 
 import base58
 from rich.console import Console
@@ -14,15 +15,17 @@
 TOKEN_ADDRESSES = {
     'TFczxzPhnThNSqr5by8tvxsdCFRRz6cPNq': 'APENFT',
     'TN3W4H6rK2ce4vX9YnFQHwKENnHjoxb3m9': 'BTCT',   # BTC on Tron (?!)
     'TAFjULxiVgT4qWk6UZwjqwZXTSaGaqnVp4': 'BTT',
     'TMz2SWatiAtZVVcH2ebpsbVtYwUPT9EdjH': 'BUSD',
     'THbVQp8kMjStKNnf2iCY6NEzThKMK5aBHg': 'DOGET',  # DOGEcoin on Tron (?!)
     'TDyvndWuvX5xTBwHPYJi7J3Yq8pq8yh62h': 'HT',     # Huobi Token
+    'TNSBA6KvSvMoTqQcEgpVK7VhHT3z7wifxy': 'jUSDC',
     'TCFLL5dx5ZJdKnWuesXxi1VPwjLVmWZZy9': 'JST',
+    'TVh1PF9xr4zC5uAqRcCbxF1By6ucp95G4i': 'stUSDT',
     'TSSMHYeV2uE9qYH95DqyoCuNCzEL1NvU3S': 'SUN',
     'TUpMhErZL2fhh4sVNULAbNKLokS4GjC1F4': 'TUSD',
     'TEkxiTehnzSmSe2XqrBj4w32RUN966rdz8': 'USDC',
     'TPYmHEhy5n8TCEfYGqW2rPxsghSfzghPDn': 'USDD',
     'TMwFHYXLJaRUPeW6421aqXL4ZEzPRFGkGT': 'USDJ',
     'TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t': 'USDT',
     'TLa2f6VPqDgRE67v1736s7bJ8Ray5wYjU7': 'WIN',
```

### Comparing `trongrid_extractor-0.4.0/trongrid_extractor/helpers/argument_parser.py` & `trongrid_extractor-1.0.0/trongrid_extractor/helpers/argument_parser.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.4.0/trongrid_extractor/helpers/csv_helper.py` & `trongrid_extractor-1.0.0/trongrid_extractor/helpers/csv_helper.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,33 +5,34 @@
 from typing import Any, Dict, List, Optional, Union
 
 from trongrid_extractor.config import log
 from trongrid_extractor.helpers.address_helpers import *
 from trongrid_extractor.trc20_txn import Trc20Txn
 
 
-def write_rows(file_path: Union[str, Path], rows: List[Trc20Txn]) -> None:
-    if len(rows) == 0:
-        log.warning(f"No rows to write!")
-        return
-
+def write_rows(file_path: Union[str, Path], rows: List[Trc20Txn], _klass = Trc20Txn) -> None:
     log.info(f"Writing {len(rows)} rows...")
-    _fields = [fld.name for fld in fields(type(rows[0]))]
+    _fields = [fld.name for fld in fields(_klass)]
 
     if Path(file_path).exists():
         file_mode = 'a'
     else:
         file_mode = 'w'
 
     with open(file_path, file_mode) as f:
         csv_writer = csv.DictWriter(f, _fields)
 
         if file_mode == 'w':
             csv_writer.writeheader()
 
+        # Put this after the header is written so there is always an output file
+        if len(rows) == 0:
+            log.warning(f"No rows to write!")
+            return
+
         csv_writer.writerows([asdict(row) for row in rows])
 
 
 def output_csv_path(address: str, dir: Optional[Path] = None, suffix: Optional[str] = None) -> Path:
     """Build a filename that contains the address and (if available) the symbol."""
     dir = dir or Path('')
     filename = csv_prefix(address)
```

### Comparing `trongrid_extractor-0.4.0/trongrid_extractor/helpers/time_helpers.py` & `trongrid_extractor-1.0.0/trongrid_extractor/helpers/time_helpers.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.4.0/trongrid_extractor/progress_tracker.py` & `trongrid_extractor-1.0.0/trongrid_extractor/progress_tracker.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,14 +23,16 @@
             resume_from_csv: bool = False,
             token_address: Optional[str] = None,
         ) -> None:
         self.output_csv_path = output_csv_path
         self.already_processed_uniq_ids = set()
         self.earliest_timestamp_seen_ms = None
         self.latest_timestamp_seen_ms = None
+        self.min_block_number_seen = None
+        self.max_block_number_seen = None
         self.token_address = token_address
         self.rows_in_scanned_csv = 0
 
         # Resume from CSV if requested
         if resume_from_csv:
             self._load_csv_progress()
         elif self.output_csv_path.exists():
@@ -53,14 +55,18 @@
                 log.debug(f"Already processed: {txn}")
                 continue
 
             if self.earliest_timestamp_seen_ms is None or txn.ms_from_epoch < self.earliest_timestamp_seen_ms:
                 self.earliest_timestamp_seen_ms = txn.ms_from_epoch
             if self.latest_timestamp_seen_ms is None or txn.ms_from_epoch > self.latest_timestamp_seen_ms:
                 self.latest_timestamp_seen_ms = txn.ms_from_epoch
+            if self.min_block_number_seen is None or txn.block_number < self.min_block_number_seen:
+                self.min_block_number_seen = txn.block_number
+            if self.max_block_number_seen is None or txn.block_number > self.max_block_number_seen:
+                self.max_block_number_seen = txn.block_number
 
             filtered_txns.append(txn)
             self.already_processed_uniq_ids.add(txn.unique_id)
 
         removed_txn_count = len(txns) - len(filtered_txns)
 
         if removed_txn_count > 0:
```

### Comparing `trongrid_extractor-0.4.0/trongrid_extractor/request_params.py` & `trongrid_extractor-1.0.0/trongrid_extractor/request_params.py`

 * *Files identical despite different names*

### Comparing `trongrid_extractor-0.4.0/trongrid_extractor/response.py` & `trongrid_extractor-1.0.0/trongrid_extractor/response.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,60 +18,62 @@
 from trongrid_extractor.helpers.time_helpers import *
 
 # If the distance between min and max_timestamp is less than this don't consider a 0 row
 # result a failure.
 OK_DURATION_FOR_ZERO_TXNS_MS = 10000
 JSON_HEADERS = {'Accept': 'application/json'}
 
+TRONGRID_RETRY_KWARGS = {
+    'wait': wait_exponential(multiplier=1, min=15, max=300),
+    'stop': stop_after_attempt(5),
+    'after': after_log(log, logging.DEBUG),
+}
+
 
 @dataclass
 class Response:
     raw_response: requests.models.Response
     params: Dict[str, Any]
 
     def __post_init__(self):
         log.debug(dump.dump_all(self.raw_response).decode('utf-8'))
         self.response = self.raw_response.json()
 
     @classmethod
-    @retry(wait=wait_exponential(multiplier=1, min=15, max=300), stop=stop_after_attempt(5), after=after_log(log, logging.DEBUG))
-    def get_response(cls, url: str, params: Optional[Dict[str, Union[str, int, float]]] = None) -> 'Response':
+    @retry(**TRONGRID_RETRY_KWARGS)
+    def get_response(
+            cls,
+            url: str,
+            params: Optional[Dict[str, Union[str, int, float]]] = None
+        ) -> 'Response':
         """Alternate constructor that calls the API with retries."""
         params = params or {}
 
         # If an API call yields too many rows to fit in one response a 'next URL' is given and
         # our requests use that URL without params.
         is_new_query = (MIN_TIMESTAMP in params) and (MAX_TIMESTAMP in params)
 
         # Min/Max timestamps are INCLUSIVE.
         if is_new_query:
-            msg = f"New query requesting data from {ms_to_datetime(params[MIN_TIMESTAMP])} to {ms_to_datetime(params[MAX_TIMESTAMP])}."
+            msg = f"Requesting data from {ms_to_datetime(params[MIN_TIMESTAMP])} " \
+                  f"to {ms_to_datetime(params[MAX_TIMESTAMP])}."
             log.info(msg)
 
         log.debug(f"Request URL: {url}\nParams: {params}")
         raw_response = requests.get(url, headers=JSON_HEADERS, params=params)
         response = cls(raw_response, deepcopy(params))
 
         # Sometimes TronGrid will return 0 rows for no apparent reason. Retrying usually fixes it
         # so we throw an exception to get a tenacity retry.
         # It also seems that if the number of responses to a query is a multiple of 200 (the page sizez)
         # Trongrid may page through to an empty response. That case is not well handled here.
-        if response.is_false_complete_response():
-            log.info("Empty response that perhaps should not be empty...")
-
-            if is_new_query:
-                duration_queried_ms = params[MAX_TIMESTAMP] - params[MIN_TIMESTAMP]
-                log.info(f"{duration_queried_ms}ms duration from min to max_timestamp in query")
-
-                if duration_queried_ms <= OK_DURATION_FOR_ZERO_TXNS_MS:
-                    log.warning(f"Looks like a bad false empty response but only {duration_queried_ms}ms in range so OK.")
-                    return response
-
+        if response.is_false_complete_response() and not is_new_query:
+            log.warning("Empty response that perhaps should not be empty...")
             msg = f"Seems like an actual error: response shouldn't be empty. Response:\n{response.response}\n\nRetrying.."
-            log.error(msg)
+            log.warning(msg)
             response.pretty_print()
             raise ValueError(msg)
 
         return response
 
     def is_continuable_response(self) -> bool:
         """Return True if the response contains a link to the next page via a url."""
```

### Comparing `trongrid_extractor-0.4.0/trongrid_extractor/trc20_txn.py` & `trongrid_extractor-1.0.0/trongrid_extractor/trc20_txn.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 from trongrid_extractor.config import log
 from trongrid_extractor.helpers.address_helpers import hex_to_tron
 from trongrid_extractor.helpers.rich_helpers import console
 from trongrid_extractor.helpers.string_constants import DATA, RESULT
 from trongrid_extractor.helpers.time_helpers import ms_to_datetime
 
 # Some tokens use src/dst/wad instead of from/to/value
-SRC_DST_WAD = ('src', 'dst', 'wad')
+FROM_TO_AMOUNT = ('from', 'to', 'amount')
 FROM_TO_VALUE = ('from', 'to', 'value')
+SRC_DST_WAD = ('src', 'dst', 'wad')
 
 
 @dataclass(kw_only=True)
 class Trc20Txn:
     token_address: str
     from_address: str
     to_address: str
@@ -107,14 +108,16 @@
         log.debug(f"Extracted {len(txns)} txns from the response...")
         return txns
 
     @staticmethod
     def identify_txn_keys(result_type: Dict[str, str]) -> Tuple[str, str, str]:
         if sorted(result_type.keys()) == sorted(SRC_DST_WAD):
             return SRC_DST_WAD
+        elif sorted(result_type.keys()) == sorted(FROM_TO_AMOUNT):
+            return FROM_TO_AMOUNT
         else:
             return FROM_TO_VALUE
 
     def event_time(self) -> pendulum.DateTime:
         return ms_to_datetime(self.ms_from_epoch)
 
     def __str__(self) -> str:
```

### Comparing `trongrid_extractor-0.4.0/PKG-INFO` & `trongrid_extractor-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trongrid-extractor
-Version: 0.4.0
+Version: 1.0.0
 Summary: Extract transactions from the Trongrid API.
 Home-page: https://chainargos.com
 Author: Chain Argos
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -75,14 +75,21 @@
 ### Publishing
 1. Update `pyproject.toml` version number
 1. Update `CHANGELOG.md`
 1. `poetry publish --build --repository chain_argos_pypi`
 
 ## TODO
 1. Walk forward not backward
+1. Weird that this yielded dupes on the first page:
+   ```
+   {request_params.py:29} INFO - Request URL: https://api.trongrid.io/v1/contracts/TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t/events
+   Params requesting 'Transfer' events from 2021-04-01T04:00:01+00:00 to 2021-04-01T05:00:00+00:00 (no extra params).
+   {response.py:48} INFO - New query requesting data from 2021-04-01T04:00:01+00:00 to 2021-04-01T05:00:00+00:00.
+   {progress_tracker.py:67} INFO -   Removed 11 duplicate transactions...
+   ```
 1. USDT looks incomplete here as 9pm was the last time:
    ```
    WARNING - 0 txns found. We seem to be stuck at 2020-07-09T21:04:24+00:00.
    [2023-06-29, 06:34:36 UTC] {logging_mixin.py:137} INFO -                     WARNING    Last request params:                   api.py:127
                              {'only_confirmed': 'true', 'limit': 200,
                              'min_timestamp': 1594252801000.0,
                              'max_timestamp': 1594328664000.0,
```

