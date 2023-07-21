# Comparing `tmp/py3cw-0.0.8.tar.gz` & `tmp/py3cw-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py3cw-0.0.8.tar", last modified: Wed Dec 25 16:44:43 2019, max compression
+gzip compressed data, was "py3cw-0.1.0.tar", last modified: Fri Jul 21 07:50:41 2023, max compression
```

## Comparing `py3cw-0.0.8.tar` & `py3cw-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-25 16:44:43.382048 py3cw-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (115)      350 2019-12-25 16:44:43.382048 py3cw-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     2084 2019-12-25 16:44:36.000000 py3cw-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-25 16:44:43.382048 py3cw-0.0.8/py3cw/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2019-12-25 16:44:36.000000 py3cw-0.0.8/py3cw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     2897 2019-12-25 16:44:36.000000 py3cw-0.0.8/py3cw/config.py
--rw-r--r--   0 runner    (1001) docker     (115)     2826 2019-12-25 16:44:36.000000 py3cw-0.0.8/py3cw/request.py
--rw-r--r--   0 runner    (1001) docker     (115)     1503 2019-12-25 16:44:36.000000 py3cw-0.0.8/py3cw/test_request.py
--rw-r--r--   0 runner    (1001) docker     (115)      899 2019-12-25 16:44:36.000000 py3cw-0.0.8/py3cw/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-25 16:44:43.382048 py3cw-0.0.8/py3cw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)      350 2019-12-25 16:44:43.000000 py3cw-0.0.8/py3cw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      250 2019-12-25 16:44:43.000000 py3cw-0.0.8/py3cw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2019-12-25 16:44:43.000000 py3cw-0.0.8/py3cw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)        9 2019-12-25 16:44:43.000000 py3cw-0.0.8/py3cw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)        6 2019-12-25 16:44:43.000000 py3cw-0.0.8/py3cw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)       38 2019-12-25 16:44:43.382048 py3cw-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)      517 2019-12-25 16:44:36.000000 py3cw-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:50:41.608322 py3cw-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-21 07:50:31.000000 py3cw-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 07:50:41.608322 py3cw-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-21 07:50:31.000000 py3cw-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:50:41.604322 py3cw-0.1.0/py3cw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:50:31.000000 py3cw-0.1.0/py3cw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-07-21 07:50:31.000000 py3cw-0.1.0/py3cw/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-21 07:50:31.000000 py3cw-0.1.0/py3cw/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-21 07:50:31.000000 py3cw-0.1.0/py3cw/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-21 07:50:31.000000 py3cw-0.1.0/py3cw/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:50:41.604322 py3cw-0.1.0/py3cw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 07:50:41.000000 py3cw-0.1.0/py3cw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-21 07:50:41.000000 py3cw-0.1.0/py3cw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:50:41.000000 py3cw-0.1.0/py3cw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 07:50:41.000000 py3cw-0.1.0/py3cw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 07:50:41.000000 py3cw-0.1.0/py3cw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:50:41.608322 py3cw-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-21 07:50:31.000000 py3cw-0.1.0/setup.py
```

### Comparing `py3cw-0.0.8/py3cw/config.py` & `py3cw-0.1.0/py3cw/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 API_URL = 'https://api.3commas.io'
-API_VERSION = '/public/api/ver1/'
+API_VERSION_V1 = '/public/api/ver1/'
+API_VERSION_V2 = '/public/api/v2/'
+API_VERSION_V2_ENTITIES = ['smart_trades', 'smart_trades_v2']
 
 # API methods from
 # https://github.com/3commas-io/3commas-official-api-docs
 API_METHODS = {
     'accounts': {
         '': ('GET', ''),
+        'account_info': ('GET', '{id}'),
         'new': ('POST', 'new'),
         'update': ('POST', 'update'),
         'market_list': ('GET', 'market_list'),
         'market_pairs': ('GET', 'market_pairs'),
         'currency_rates': ('GET', 'currency_rates'),
         'sell_all_to_usd': ('POST', '{id}/sell_all_to_usd'),
         'sell_all_to_btc': ('POST', '{id}/sell_all_to_btc'),
+        'convert_dust_to_bnb': ('POST', '{id}/convert_dust_to_bnb'),
+        'networks_info': ('GET', '{id}/networks_info'),
         'rename': ('POST', '{id}/rename'),
         'pie_chart_data': ('POST', '{id}/pie_chart_data'),
         'account_table_data': ('POST', '{id}/account_table_data'),
-        'remove': ('POST', '{id}/remove')
+        'remove': ('POST', '{id}/remove'),
+        'transfer': ('POST', 'transfer'),
+        'transfer_history': ('GET', 'transfer_history'),
+        'transfer_data': ('GET', 'transfer_data'),
+        'active_trading_entities': ('GET', '{id}/active_trading_entities'),
+        'balance_chart_data': ('GET', '{id}/balance_chart_data'),
+        'load_balances': ('POST', '{id}/load_balances')
     },
     'deals': {
         '': ('GET', ''),
         'update_max_safety_orders': ('POST', '{id}/update_max_safety_orders'),
         'panic_sell': ('POST', '{id}/panic_sell'),
         'cancel': ('POST', '{id}/cancel'),
         'update_deal': ('PATCH', '{id}/update_deal'),
         'update_tp': ('POST', '{id}/update_tp'),
         'show': ('GET', '{id}/show'),
         'cancel_order': ('POST', '{id}/cancel_order'),
         'market_orders': ('GET', '{id}/market_orders'),
         'add_funds': ('POST', '{id}/add_funds'),
         'data_for_adding_funds': ('GET', '{id}/data_for_adding_funds'),
+        'convert_to_smart_trade': ('POST', '{id}/convert_to_smart_trade'),
     },
     'bots': {
         '': ('GET', ''),
         'strategy_list': ('GET', 'strategy_list'),
         'pairs_black_list': ('GET', 'pairs_black_list'),
         'update_pairs_black_list': ('POST', 'update_pairs_black_list'),
         'create_bot': ('POST', 'create_bot'),
@@ -41,29 +53,71 @@
         'update': ('PATCH', '{id}/update'),
         'disable': ('POST', '{id}/disable'),
         'enable': ('POST', '{id}/enable'),
         'start_new_deal': ('POST', '{id}/start_new_deal'),
         'delete': ('POST', '{id}/delete'),
         'panic_sell_all_deals': ('POST', '{id}/panic_sell_all_deals'),
         'cancel_all_deals': ('POST', '{id}/cancel_all_deals'),
-        'show': ('GET', '{id}/show')
+        'copy_and_create': ('POST', '{id}/copy_and_create'),
+        'show': ('GET', '{id}/show'),
+        'deals_stats': ('GET', '{id}/deals_stats')
+    },
+    'grid_bots': {
+        '': ('GET', ''),
+        'ai': ('POST', 'ai'),
+        'manual': ('POST', 'manual'),
+        'ai_settings': ('GET', 'ai_settings'),
+        'market_orders': ('GET', '{id}/market_orders'),
+        'profits': ('GET', '{id}/profits'),
+        'ai_update': ('PATCH', '{id}/ai'),
+        'manual_update': ('PATCH', '{id}/manual'),
+        'get': ('GET', '{id}'),
+        'delete': ('DELETE', '{id}'),
+        'disable': ('POST', '{id}/disable'),
+        'enable': ('POST', '{id}/enable'),
+        'required_balances': ('GET', '{id}/required_balances')
     },
     'marketplace': {
         'items': ('GET', 'items'),
-        'signals': ('GET', '{id}/signals')
+        'signals': ('GET', '{id}/signals'),
+        'presets': ('GET', 'presets')
     },
-    'smart_trades': {
+    # smart_trades has been deprecated
+    # Please don't use it anymore. Left here only for history reference
+    'smart_trades_deprecated': {
         '': ('GET', ''),
         'create_simple_sell': ('POST', 'create_simple_sell'),
         'create_simple_buy': ('POST', 'create_simple_buy'),
         'create_smart_sell': ('POST', 'create_smart_sell'),
         'create_smart_cover': ('POST', 'create_smart_cover'),
         'create_smart_trade': ('POST', 'create_smart_trade'),
         'cancel_order': ('POST', '{id}/cancel_order'),
         'add_funds': ('POST', '{id}/add_funds'),
         'step_panic_sell': ('POST', '{id}/step_panic_sell'),
         'update': ('PATCH', '{id}/update'),
         'cancel': ('POST', '{id}/cancel'),
         'panic_sell': ('POST', '{id}/panic_sell'),
-        'force_process': ('POST', '{id}/force_process'),
+        'force_process': ('POST', '{id}/force_process')
+    },
+    'smart_trades_v2': {
+        '': ('GET', ''),
+        'new': ('POST', ''),
+        'get_by_id': ('GET', '{id}'),
+        'update': ('PATCH', '{id}'),
+        'cancel': ('DELETE', '{id}'),
+        'get_trades': ('GET', '{id}/trades'),
+        'add_funds': ('POST', '{id}/add_funds'),
+        'reduce_funds': ('POST', '{id}/reduce_funds'),
+        'close_by_market': ('POST', '{id}/close_by_market'),
+        'cancel_trade': ('DELETE', '{id}/trades/{sub_id}'),
+        'panic_close_by_market': ('POST', '{id}/trades/{sub_id}/close_by_market'),
+        'set_note': ('POST', '{id}/set_note'),
+        'force_start': ('POST', '{id}/force_start'),
+        'force_process': ('POST', '{id}/force_process')
+    },
+    'users': {
+        'change_mode': ('POST', 'change_mode'),
+        'current_mode': ('GET', 'current_mode'),
+        'locale': ('PUT', 'locale'),
+        'permissions_info': ('GET', 'permissions_info')
     }
 }
```

### Comparing `py3cw-0.0.8/py3cw/test_request.py` & `py3cw-0.1.0/py3cw/test_request.py`

 * *Files identical despite different names*

### Comparing `py3cw-0.0.8/py3cw/utils.py` & `py3cw-0.1.0/py3cw/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     def wrapper(*args, **kw):
         """
         Raises an error if on of the arguments is missing or if the specific action requires and ID
         and it is not sent.
         """
 
         entity = kw.get('entity')
-        action = kw.get('action')
+        action = kw.get('action', '')
         action_id = kw.get('action_id')
         api = API_METHODS[entity][action]
         method, api_path = api
 
         if entity is None or entity == '':
             raise ValueError('Missing entity')
         if entity not in API_METHODS:
```

### Comparing `py3cw-0.0.8/setup.py` & `py3cw-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='py3cw',
-    version='0.0.8',
+    version='0.1.0',
 
     description='3commas Python wrapper',
 
     url='https://github.com/bogdanteodoru/py3cw',
 
     author='Bogdan Teodoru',
     author_email='me@bogdanteodoru.com',
```

