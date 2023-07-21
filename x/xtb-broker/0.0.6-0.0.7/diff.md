# Comparing `tmp/xtb_broker-0.0.6.tar.gz` & `tmp/xtb_broker-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtb_broker-0.0.6.tar", last modified: Fri Jul 21 09:14:41 2023, max compression
+gzip compressed data, was "xtb_broker-0.0.7.tar", last modified: Fri Jul 21 09:26:48 2023, max compression
```

## Comparing `xtb_broker-0.0.6.tar` & `xtb_broker-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:14:41.577326 xtb_broker-0.0.6/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      270 2023-07-21 09:14:41.577326 xtb_broker-0.0.6/PKG-INFO
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      526 2023-07-21 09:14:06.000000 xtb_broker-0.0.6/README.md
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      516 2023-07-20 21:52:23.000000 xtb_broker-0.0.6/pyproject.toml
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       38 2023-07-21 09:14:41.577326 xtb_broker-0.0.6/setup.cfg
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      397 2023-07-21 09:14:38.000000 xtb_broker-0.0.6/setup.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:14:41.573326 xtb_broker-0.0.6/xtb_broker/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/__init__.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)    12103 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/client.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:14:41.577326 xtb_broker-0.0.6/xtb_broker/config/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/config/__init__.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2065 2023-05-20 14:31:15.000000 xtb_broker-0.0.6/xtb_broker/config/constants.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1702 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/config/exception.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      701 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/config/frozen.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      289 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/config/logger.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:14:41.577326 xtb_broker-0.0.6/xtb_broker/models/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/__init__.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6028 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/arbitrage.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2198 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/position.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      583 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/shift.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     3091 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/symbol.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1824 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/timetable.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6465 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/trade.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1824 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/models/transaction.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      649 2023-05-20 13:45:08.000000 xtb_broker-0.0.6/xtb_broker/utils.py
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2651 2023-07-20 18:18:21.000000 xtb_broker-0.0.6/xtb_broker/xtb.py
-drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:14:41.573326 xtb_broker-0.0.6/xtb_broker.egg-info/
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      270 2023-07-21 09:14:41.000000 xtb_broker-0.0.6/xtb_broker.egg-info/PKG-INFO
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      636 2023-07-21 09:14:41.000000 xtb_broker-0.0.6/xtb_broker.egg-info/SOURCES.txt
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        1 2023-07-21 09:14:41.000000 xtb_broker-0.0.6/xtb_broker.egg-info/dependency_links.txt
--rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       11 2023-07-21 09:14:41.000000 xtb_broker-0.0.6/xtb_broker.egg-info/top_level.txt
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:26:48.829466 xtb_broker-0.0.7/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      270 2023-07-21 09:26:48.829466 xtb_broker-0.0.7/PKG-INFO
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      453 2023-07-21 09:26:18.000000 xtb_broker-0.0.7/README.md
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      516 2023-07-20 21:52:23.000000 xtb_broker-0.0.7/pyproject.toml
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       38 2023-07-21 09:26:48.829466 xtb_broker-0.0.7/setup.cfg
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      397 2023-07-21 09:26:43.000000 xtb_broker-0.0.7/setup.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:26:48.825466 xtb_broker-0.0.7/xtb_broker/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.7/xtb_broker/__init__.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)    12091 2023-07-21 09:26:18.000000 xtb_broker-0.0.7/xtb_broker/client.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:26:48.825466 xtb_broker-0.0.7/xtb_broker/config/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.7/xtb_broker/config/__init__.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2065 2023-05-20 14:31:15.000000 xtb_broker-0.0.7/xtb_broker/config/constants.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1702 2023-05-20 13:45:08.000000 xtb_broker-0.0.7/xtb_broker/config/exception.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      697 2023-07-21 09:26:18.000000 xtb_broker-0.0.7/xtb_broker/config/frozen.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      285 2023-07-21 09:26:18.000000 xtb_broker-0.0.7/xtb_broker/config/logger.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:26:48.829466 xtb_broker-0.0.7/xtb_broker/models/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-05-20 13:45:08.000000 xtb_broker-0.0.7/xtb_broker/models/__init__.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     5996 2023-07-21 09:26:28.000000 xtb_broker-0.0.7/xtb_broker/models/arbitrage.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2178 2023-07-21 09:26:28.000000 xtb_broker-0.0.7/xtb_broker/models/position.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      579 2023-07-21 09:26:18.000000 xtb_broker-0.0.7/xtb_broker/models/shift.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     3075 2023-07-21 09:26:28.000000 xtb_broker-0.0.7/xtb_broker/models/symbol.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1816 2023-07-21 09:26:28.000000 xtb_broker-0.0.7/xtb_broker/models/timetable.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     6445 2023-07-21 09:26:28.000000 xtb_broker-0.0.7/xtb_broker/models/trade.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     1816 2023-07-21 09:26:18.000000 xtb_broker-0.0.7/xtb_broker/models/transaction.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      649 2023-05-20 13:45:08.000000 xtb_broker-0.0.7/xtb_broker/utils.py
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)     2639 2023-07-21 09:26:28.000000 xtb_broker-0.0.7/xtb_broker/xtb.py
+drwxrwxr-x   0 rubengonzalez  (1000) rubengonzalez  (1000)        0 2023-07-21 09:26:48.825466 xtb_broker-0.0.7/xtb_broker.egg-info/
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      270 2023-07-21 09:26:48.000000 xtb_broker-0.0.7/xtb_broker.egg-info/PKG-INFO
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)      636 2023-07-21 09:26:48.000000 xtb_broker-0.0.7/xtb_broker.egg-info/SOURCES.txt
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)        1 2023-07-21 09:26:48.000000 xtb_broker-0.0.7/xtb_broker.egg-info/dependency_links.txt
+-rw-rw-r--   0 rubengonzalez  (1000) rubengonzalez  (1000)       11 2023-07-21 09:26:48.000000 xtb_broker-0.0.7/xtb_broker.egg-info/top_level.txt
```

### Comparing `xtb_broker-0.0.6/pyproject.toml` & `xtb_broker-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.6/xtb_broker/client.py` & `xtb_broker-0.0.7/xtb_broker/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from time import sleep
 import ssl
 from random import uniform
 from typing import Dict, List
 from datetime import datetime
 from retrying import retry
 
-from xtb_config.constants import API_MAX_CONN_TRIES, API_MIN_SECONDS_BETWEEN_REQUESTS, API_READ_TIMEOUT, \
+from config.constants import API_MAX_CONN_TRIES, API_MIN_SECONDS_BETWEEN_REQUESTS, API_READ_TIMEOUT, \
     XAPI_PORT_DICT, XAPI_ADDRESS, Type
-from xtb_config.logger import logger
-from xtb_config.exception import LoginException, GetSymbolException, GetMarginLevel, GetMarginTrade, \
+from config.logger import logger
+from config.exception import LoginException, GetSymbolException, GetMarginLevel, GetMarginTrade, \
     GetTradingHoursException, GetTradeRecordsException, GetTradeException, NotReceivedDataError, \
     OrderNotSentException, OrderStatusNotSentException, GetTickPricesException, retry_if_get_tick_prices_exception
 from utils import unix_ts_to_ts, unix_t_to_ts, ts_to_unix_ts
 
 
 last_request = datetime.now()
```

### Comparing `xtb_broker-0.0.6/xtb_broker/config/constants.py` & `xtb_broker-0.0.7/xtb_broker/config/constants.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.6/xtb_broker/config/exception.py` & `xtb_broker-0.0.7/xtb_broker/config/exception.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.6/xtb_broker/config/frozen.py` & `xtb_broker-0.0.7/xtb_broker/config/frozen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xtb_config.exception import FrozenError
+from config.exception import FrozenError
 
 
 class Frozen(object):
     """
     Frozen class gives the ability to freeze the inheriting class attributes once an object is initialized
 
     Attributes
```

### Comparing `xtb_broker-0.0.6/xtb_broker/models/arbitrage.py` & `xtb_broker-0.0.7/xtb_broker/models/arbitrage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List, Dict, Optional
 from datetime import datetime
 from retrying import retry
 
-from xtb_config.exception import ArbitragePartiallyClosedException, TradeNotFoundException, \
+from config.exception import ArbitragePartiallyClosedException, TradeNotFoundException, \
     retry_if_arbitrage_partially_closed_exception
-from xtb_config.frozen import Frozen
-from xtb_config.constants import Cmd
-from xtb_config.logger import logger
-from xtb_models.position import Position
-from xtb_models.symbol import Symbol
-from xtb_models.shift import Shift
-from xtb_models.trade import Trade
+from config.frozen import Frozen
+from config.constants import Cmd
+from config.logger import logger
+from models.position import Position
+from models.symbol import Symbol
+from models.shift import Shift
+from models.trade import Trade
 from utils import get_today_ini, get_today_end
 from xtb import Xtb
 
 
 class Arbitrage(Frozen):
     def __init__(self,
                  xtb: Xtb,
```

### Comparing `xtb_broker-0.0.6/xtb_broker/models/position.py` & `xtb_broker-0.0.7/xtb_broker/models/position.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, Optional
 
-from xtb_config.frozen import Frozen
-from xtb_config.constants import Cmd
-from xtb_models.symbol import Symbol
-from xtb_models.shift import Shift
-from xtb_models.trade import Trade
+from config.frozen import Frozen
+from config.constants import Cmd
+from models.symbol import Symbol
+from models.shift import Shift
+from models.trade import Trade
 
 from xtb import Xtb
 
 
 class Position(Frozen):
     def __init__(self,
                  xtb: Xtb,
```

### Comparing `xtb_broker-0.0.6/xtb_broker/models/shift.py` & `xtb_broker-0.0.7/xtb_broker/models/shift.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 
-from xtb_config.frozen import Frozen
+from config.frozen import Frozen
 
 
 class Shift(Frozen):
     def __init__(self, from_ts: datetime, to_ts: datetime):
         self.__from_ts: datetime = from_ts
         self.__to_ts: datetime = to_ts
```

### Comparing `xtb_broker-0.0.6/xtb_broker/models/symbol.py` & `xtb_broker-0.0.7/xtb_broker/models/symbol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, Optional
 from datetime import datetime
 
-from xtb_config.frozen import Frozen
-from xtb_config.constants import WEEKDAY
-from xtb_models.timetable import Timetable
-from xtb_models.shift import Shift
+from config.frozen import Frozen
+from config.constants import WEEKDAY
+from models.timetable import Timetable
+from models.shift import Shift
 
 from xtb import Xtb
 
 
 
 class Symbol(Frozen):
     def __init__(self, xtb: Xtb, symbol: str):
```

### Comparing `xtb_broker-0.0.6/xtb_broker/models/timetable.py` & `xtb_broker-0.0.7/xtb_broker/models/timetable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Optional
 
-from xtb_models.shift import Shift
-from xtb_config.frozen import Frozen
+from models.shift import Shift
+from config.frozen import Frozen
 
 
 class Timetable(Frozen):
     def __init__(self):
         self.__monday: List[Shift] = []
         self.__tuesday: List[Shift] = []
         self.__wednesday: List[Shift] = []
```

### Comparing `xtb_broker-0.0.6/xtb_broker/models/trade.py` & `xtb_broker-0.0.7/xtb_broker/models/trade.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Dict, Optional
 from retrying import retry
 
-from xtb_config.frozen import Frozen
-from xtb_config.exception import OrderPendingException, \
+from config.frozen import Frozen
+from config.exception import OrderPendingException, \
     retry_if_order_not_sent_exception, retry_if_order_not_accepted_exception
-from xtb_config.constants import Type, CMD, Cmd, STATUS, Status
-from xtb_config.logger import logger
+from config.constants import Type, CMD, Cmd, STATUS, Status
+from config.logger import logger
 from xtb import Xtb
-from xtb_models.transaction import Transaction
+from models.transaction import Transaction
 
 
 class Trade(Frozen):
     def __init__(self, trade_raw: Dict):
         trade_raw['order'] = trade_raw.get('order', 0)
         trade_raw['offset'] = trade_raw.get('offset', 0)
         trade_raw['sl'] = trade_raw.get('sl', 0)
```

### Comparing `xtb_broker-0.0.6/xtb_broker/models/transaction.py` & `xtb_broker-0.0.7/xtb_broker/models/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Dict
 
-from xtb_config.frozen import Frozen
-from xtb_config.constants import Status
+from config.frozen import Frozen
+from config.constants import Status
 
 
 class Transaction(Frozen):
     def __init__(self, order: int):
         self.__order: int = order
         self.__status: str = ''
         self.__message: str = ''
```

### Comparing `xtb_broker-0.0.6/xtb_broker/utils.py` & `xtb_broker-0.0.7/xtb_broker/utils.py`

 * *Files identical despite different names*

### Comparing `xtb_broker-0.0.6/xtb_broker/xtb.py` & `xtb_broker-0.0.7/xtb_broker/xtb.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Optional, Dict
 from retrying import retry
 from datetime import datetime
 import sys
 import os
 
 sys.path.append(os.path.realpath(os.path.join(os.path.dirname(__file__), '.')))
-from xtb_config.constants import WEEKDAY
-from xtb_models.timetable import Timetable
-from xtb_models.shift import Shift
+from config.constants import WEEKDAY
+from models.timetable import Timetable
+from models.shift import Shift
 from utils import ts_to_unix_ts
 import client
 from client import XtbClient
 
 
 
 # Declared at cold-start, but only initialized if/when the function executes (initializing them lazily on demand)
```

### Comparing `xtb_broker-0.0.6/xtb_broker.egg-info/SOURCES.txt` & `xtb_broker-0.0.7/xtb_broker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

