# Comparing `tmp/asyncoinpayments-0.0.2a0.tar.gz` & `tmp/asyncoinpayments-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncoinpayments-0.0.2a0.tar", last modified: Sat Jul  8 20:21:08 2023, max compression
+gzip compressed data, was "asyncoinpayments-0.0.3a0.tar", last modified: Thu Jul 20 22:13:59 2023, max compression
```

## Comparing `asyncoinpayments-0.0.2a0.tar` & `asyncoinpayments-0.0.3a0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-08 20:21:08.363525 asyncoinpayments-0.0.2a0/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1258 2023-07-08 20:21:08.363525 asyncoinpayments-0.0.2a0/PKG-INFO
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      432 2023-07-08 20:18:04.000000 asyncoinpayments-0.0.2a0/README.md
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-08 20:21:08.363525 asyncoinpayments-0.0.2a0/asyncoinpayments/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       43 2023-07-08 19:34:54.000000 asyncoinpayments-0.0.2a0/asyncoinpayments/__init__.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    16708 2023-07-08 19:53:58.000000 asyncoinpayments-0.0.2a0/asyncoinpayments/coinpayments.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      155 2023-07-08 15:55:02.000000 asyncoinpayments-0.0.2a0/asyncoinpayments/errors.py
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       51 2023-07-08 15:55:21.000000 asyncoinpayments-0.0.2a0/asyncoinpayments/utils.py
-drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-08 20:21:08.363525 asyncoinpayments-0.0.2a0/asyncoinpayments.egg-info/
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1258 2023-07-08 20:21:08.000000 asyncoinpayments-0.0.2a0/asyncoinpayments.egg-info/PKG-INFO
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      332 2023-07-08 20:21:08.000000 asyncoinpayments-0.0.2a0/asyncoinpayments.egg-info/SOURCES.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)        1 2023-07-08 20:21:08.000000 asyncoinpayments-0.0.2a0/asyncoinpayments.egg-info/dependency_links.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       37 2023-07-08 20:21:08.000000 asyncoinpayments-0.0.2a0/asyncoinpayments.egg-info/requires.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-08 20:21:08.000000 asyncoinpayments-0.0.2a0/asyncoinpayments.egg-info/top_level.txt
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       38 2023-07-08 20:21:08.363525 asyncoinpayments-0.0.2a0/setup.cfg
--rw-rw-r--   0 flalugli  (1000) flalugli  (1000)     1127 2023-07-08 20:20:54.000000 asyncoinpayments-0.0.2a0/setup.py
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-20 22:13:59.016072 asyncoinpayments-0.0.3a0/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       72 2023-07-20 22:07:25.000000 asyncoinpayments-0.0.3a0/.gitignore
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    11328 2023-07-08 21:40:35.000000 asyncoinpayments-0.0.3a0/LICENSE.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      928 2023-07-20 22:13:59.016072 asyncoinpayments-0.0.3a0/PKG-INFO
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      432 2023-07-08 20:18:04.000000 asyncoinpayments-0.0.3a0/README.md
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-20 22:13:59.016072 asyncoinpayments-0.0.3a0/asyncoinpayments/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       92 2023-07-18 17:18:09.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/__init__.py
+drwxrwxr-x   0 flalugli  (1000) flalugli  (1000)        0 2023-07-20 22:13:59.016072 asyncoinpayments-0.0.3a0/asyncoinpayments/asyncoinpayments.egg-info/
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      928 2023-07-20 22:13:58.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/asyncoinpayments.egg-info/PKG-INFO
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      455 2023-07-20 22:13:59.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/asyncoinpayments.egg-info/SOURCES.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)        1 2023-07-20 22:13:58.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/asyncoinpayments.egg-info/dependency_links.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       17 2023-07-20 22:13:58.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/asyncoinpayments.egg-info/requires.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)        1 2023-07-20 22:13:58.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/asyncoinpayments.egg-info/top_level.txt
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)    21181 2023-07-20 21:49:59.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/coinpayments.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      155 2023-07-08 15:55:02.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/errors.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      647 2023-07-20 21:10:50.000000 asyncoinpayments-0.0.3a0/asyncoinpayments/utils.py
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)      711 2023-07-20 22:08:43.000000 asyncoinpayments-0.0.3a0/pyproject.toml
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       38 2023-07-20 22:13:59.016072 asyncoinpayments-0.0.3a0/setup.cfg
+-rw-rw-r--   0 flalugli  (1000) flalugli  (1000)       68 2023-07-20 21:25:48.000000 asyncoinpayments-0.0.3a0/setup.py
```

### Comparing `asyncoinpayments-0.0.2a0/PKG-INFO` & `asyncoinpayments-0.0.3a0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 Metadata-Version: 2.1
 Name: asyncoinpayments
-Version: 0.0.2a0
+Version: 0.0.3a0
 Summary: Python Asynchronous Wrapper of the CoinPayments API
-Home-page: https://github.com/flalugli/asyncoinpayments
-Author: flalugli
-Author-email: <flalugli.dev@gmail.com>
 License: Apache License 2.0
-Description: 
-        # AsynCoinpayments  
-        
-        An async/await compatible python wrapper for the CoinPayments API  
-        
-        ---
-        
-        ## How to install  
-        
-        ```
-        # run this in the command propt or terminal
-        pip install asyncoinpayments  
-        ```
-        
-        ## Features  
-        - Fast to setup and simple to use
-        - Easy to use async/await interface
-        - API calls using aiohttp requests  
-        - create your own API calls
-        
-        ### Contact me
-        
-        **Email** : <flalugli.dev@gmail.com>  
-        **Discord** : flalugli   
-        
 Keywords: python,crypto,cryptocurrency,payment gateway,async,aiohttp
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+License-File: LICENSE.txt
+
+# AsynCoinpayments  
+
+An async/await compatible python wrapper for the CoinPayments API  
+
+---
+
+## How to install  
+
+```
+# run this in the command propt or terminal
+pip install asyncoinpayments  
+```
+
+## Features  
+- Fast to setup and simple to use
+- Easy to use async/await interface
+- API calls using aiohttp requests  
+- create your own API calls
+
+### Contact me
+
+**Email** : <flalugli.dev@gmail.com>  
+**Discord** : flalugli
```

### Comparing `asyncoinpayments-0.0.2a0/asyncoinpayments/coinpayments.py` & `asyncoinpayments-0.0.3a0/asyncoinpayments/coinpayments.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import aiohttp
 import urllib.request, urllib.parse, urllib.error
 import urllib.request, urllib.error, urllib.parse
 import hmac
 import hashlib
+from typing import Union
 from tenacity import retry, stop_after_attempt
 from .errors import CoinPayementsError,CoinPaymentsInputError,FormatError 
-from .utils import ResponseFormat
+from .utils import ResponseFormat, JsonResponse, ApiResponseJson
 
 
 class AsyncCoinPayments:
     
     REQUEST_TRIES=3
 
     def __init__(self,_private_key:str,_public_key:str,_version:str='1', _format:ResponseFormat = ResponseFormat.JSON, _proxy:str = None, _proxy_auth:str = None) -> None:
@@ -22,29 +23,29 @@
         self._proxy_auth=_proxy_auth
         
         self.base_url='https://www.coinpayments.net/api.php'
         self._format=_format #the format of the http response can be json/xml
 
 
     def create_hmac(self, **params):
-        """ ## Generate an HMAC from the url arguments
-            
-            ### Note  
-
-            hmac on both sides depends from the order of the parameters, any
-            change in the order and the hmacs wouldn't match hence the api request would be invalid
         """
+        create hmac for api requests
+        """
+        
         encoded = urllib.parse.urlencode(params).encode('utf-8')
         #print(encoded) #to fix tx and multiple calls at once
         h=hmac.new(bytearray(self._private_key, 'utf-8'), encoded, hashlib.sha512).hexdigest()
 
         return encoded, h
 
     @retry(stop=stop_after_attempt(3)) #TODO ADD WAIT TIME MAYBE? -> hard with async and tenacity
     async def request(self, method, **params):
+        """
+        request handler
+        """
         
         encoded, h = self.create_hmac(**params)
         headers = {'hmac' : h}
         
         async with aiohttp.ClientSession() as session:
             #TODO
             #ERROR HANDLING
@@ -62,60 +63,66 @@
             elif self._format == "xml": 
                 response_formatted = await r.text()
         
         return response_formatted
 
     async def get(self, **params):
         """Performs a get request"""
+
         return await self.request(method='get',**params)
 
     async def post(self, **params):
         """Performs a post request"""
+
         return await self.request(method='post',**params)
 
-    def json_to_result(self, json_response:dict):
-        """
-        Pass a json response from the api
 
-        ## Raises 
-        CoinPayementsError
+    async def api_call(self, cmd:str, **params) -> Union[JsonResponse, str]:
+        """
+        perform an api call given a cmd and its parameters
         """
-
-        error=json_response['error']
-        if error == 'ok':
-            return json_response['result']
-        else:
-            raise CoinPayementsError(error)
-
-    async def api_call(self, cmd:str, **params):
 
         base_params={
             'cmd' : cmd,
             'key':self._public_key,
             'version': self._version,
             'format': self._format
             }
+        if self._format == "json":
+            data : ApiResponseJson = await self.post(**base_params,**params)
+            response : JsonResponse = JsonResponse(data=data)
+        else:
+            response: str = await self.post(**base_params,**params)
         
-        return await self.post(**base_params,**params)
-
+        return response
 
     ### INFORMATION COMMANDS
-    async def get_basic_info(self):
-        """# Get basic informations"""
+    async def get_basic_info(self) -> Union[JsonResponse, str]:
+        """
+        retrieves basic user info from the CoinPayments api
+
+        Returns
+        -------
+        Union[JsonResponse, str]
+            api response containing the basic user info
+        """
 
         cmd = 'get_basic_info'
 
         return await self.api_call(cmd)
     
-    async def rates(self, short:bool = True, specify_accepted:bool = True, only_accepted:bool = True):
-        """specify_accepted	: 
-        - The response will include if you have the coin enabled for acceptance on your Coin Acceptance Settings page.
+    async def rates(self, short:bool = True, specify_accepted:bool = True, only_accepted:bool = True) -> Union[JsonResponse, str]:
+        """
+        retrieves rates informations from the CoinPayments api
 
-        only_accepted:
-        - The response will include all fiat coins but only cryptocurrencies enabled for acceptance on your Coin Acceptance Settings page."""
+        Returns
+        -------
+        Union[JsonResponse, str]
+            api response containing the currency rates informations
+        """
 
         cmd = 'rates'
 
         if specify_accepted and only_accepted:
             accepted_option = 2  
         elif specify_accepted: 
             accepted_option = 1
@@ -126,19 +133,22 @@
             'short' : 1 if short else 0, 
             'accepted' : accepted_option
             }
         
         return await self.api_call(cmd, **params)
     
     ### RECEIVING PAYMENTS
-    async def create_transaction(self, amount:float, buyer_email:str, receive_currency:str, base_currency:str = 'USD', ipn_url:str = None, **params):
-        """# Create a CoinPayment transaction
-        
-        receive_currency : the currency you will receive   
-        if you want to handle refund yourself set buyer_email to your own email
+    async def create_transaction(self, amount:float, buyer_email:str, receive_currency:str, base_currency:str = 'USD', ipn_url:str = None, **params) -> Union[JsonResponse, str]:
+        """
+        creates a cryptocurrency transaction to receive client funds
+
+        Returns
+        -------
+        Union[JsonResponse, str]
+            api response containing the transaction informations
         """
 
         cmd='create_transaction'
 
         necessary_params = { 
             'amount' : amount, 
             'currency1' : base_currency,
@@ -147,46 +157,64 @@
             }
         
         if ipn_url:
             necessary_params |= {'ipn_url' : ipn_url}
 
         return await self.api_call(cmd, **necessary_params, **params)
     
-    async def get_callback_address(self, currency, ipn_url:str = None, **params):
-        """add docu"""
+    async def get_callback_address(self, currency, ipn_url:str = None, **params) -> Union[JsonResponse, str]:
+        """
+        retrieves basic user info from the CoinPayments api
+
+        Returns
+        -------
+        Union[JsonResponse, str]
+            api response containing the callback address
+        """
 
         necessary_params = {
             'currency' : currency,
             'ipn_url' : ipn_url
         }
 
         cmd = 'get_callback_address'
 
         return await self.api_call(cmd, **necessary_params, **params)
     
     async def get_tx_info_multi(self, txid): ...
         # TODO FIX THIS 	Lets you query up to 25 payment ID(s) (API key must belong to the seller.) 
         # Payment IDs should be separated with a | (pipe symbol.) 
     
-    async def get_tx_info(self, txid:str, full:bool = False):
-        """add docu"""
+    async def get_tx_info(self, txid:str, full:bool = False) -> Union[JsonResponse, str]:
+        """
+        retrieves transaction informations from the CoinPayments api
+
+        Returns
+        -------
+        Union[JsonResponse, str]
+            api response containing the transaction informations
+        """
 
         cmd = 'get_tx_info'
 
         params = {
             'txid' : txid,
             'full' : 1 if full else 0
         }
 
         return await self.api_call(cmd, **params)
     
-    async def get_tx_ids(self, limit:int=25, newer_than:int = 0, **params):
+    async def get_tx_ids(self, limit:int=25, newer_than:int = 0, **params) -> Union[JsonResponse, str]:
         """
-        max limit is 100, if greater than that it will be set to 100
-        newer_than return payments started at the given Unix timestamp or later
+        retrieves the ids of from your transaction history using the CoinPayments api
+
+        Returns
+        -------
+        Union[JsonResponse, str]
+            api response containing the callback address
         """
 
         if limit > 100: limit = 100
 
         cmd = 'get_tx_ids'
         
         aux_params={
@@ -194,76 +222,133 @@
             'newer' : newer_than
         }
 
         return await self.api_call(cmd, **aux_params,**params)
     
     ## WALLET
 
-    async def balances(self, all_coins:bool = False):
+    async def balances(self, all_coins:bool = False) -> Union[JsonResponse, str]:
         """
         # Retrieve the balances of your CoinPayments account
 
         if all_coins is set to True it will return all balances, even if they are equal to 0
         """
         cmd = 'balances'
 
         #api accepts only 1/0 as True/False
         params = {'all': 1 if all_coins else 0}
 
         return await self.api_call(cmd, **params)
     
     #EXTRA
-    async def coin_balance(self, coin:str):
+    async def coin_balance(self, coin:str) -> Union[JsonResponse, str]:
+        """
+        get the current balance of a certain currency, this only works with json format
+
+        Parameters
+        ----------
+        coin : str
+            the currency of which the balance will be returned
+
+        Returns
+        -------
+        Union[JsonResponse, str]
+            api response containing the coin balance informations
+
+        Raises
+        ------
+        FormatError
+            the format passed is not json
+        CoinPaymentsInputError
+            the user input is incorrect, the coin passed does not exists
+        """
 
         if self._format != ResponseFormat.JSON:
             raise FormatError
         
         user_balance = await self.balances(True)
         #TODO ADD TRY BLOCK
-        result = self.json_to_result(user_balance)
+        result = user_balance.result
 
         try:
             coin_balance = {'error' : 'ok', 'result' : result[coin.upper()]}
         except KeyError:
             raise CoinPaymentsInputError("This coin is not currently supported")
         else:
             return coin_balance
         
     async def get_deposit_address(self, currency:str):
-        """currency : the currency the buyer will be sending."""
+        """
+        get the merchant deposit address for a currency  
+        currency :: str : the currency the buyer will be sending.
+        """
 
         cmd = 'get_deposit_address'
 
         return await self.api_call(cmd, currency=currency)
     
-    async def create_transfer(self, amount:float, currency:str , merchant_id:int, auto_confirm:bool = False, **params):
+    async def create_transfer(self, amount:float, currency:str , merchant_id:int, auto_confirm:bool = False, **params) -> Union[JsonResponse, str]:
+        """
+        create a withdrawal to another CoinPayments user
+
+        Parameters
+        ----------
+        amount : float
+            the amount to transfer
+        currency : str
+            the currency to transfer
+        merchant_id : int
+            the merchant id to send the funds to
+        auto_confirm : bool, optional
+            if set to True no 2fa will be required to confirm the command, by default False
+
+        Returns
+        -------
+        Union[JsonResponse, str]
+            api response containing the transfer informations
+        """
 
         cmd = 'create_transfer'
 
         necessary_params = {
             'amount' : amount,
             'currency' : currency,
             'merchant' : merchant_id,
             'auto_confirm' : auto_confirm
         }
 
         return await self.api_call(cmd, **necessary_params, **params)
 
-    async def create_withdrawal(self, amount:float, receive_currency:str, base_currency:str = None, address:str = None, ipn_url: str = None, auto_confirm:bool = False, **params):
+    async def create_withdrawal(self, amount:float, receive_currency:str, base_currency:str = None, address:str = None, ipn_url: str = None, auto_confirm:bool = False, **params) -> Union[JsonResponse, str]:
         """
-        # Create a withdrawal from your funds
-    
-        if you do not pass the address you need to pass a paytag or an Unstoppable Domain
-        to send your funds to
-
-        receive_currency is the currency you will receive, while if you set a base currency 
-        'amount' of 'base_currency' will be sent in 'currency' 
-
-        Example: `to send 18$ worth of btc, 'btc' is the receive_currency and 'usd' is the base_currency`
+        create a withdrawal and send or transfer your funds to others
 
+        Parameters
+        ----------
+        amount : float
+            amount of base_currency to send
+        receive_currency : str
+            the currency the merchant will receive
+        base_currency : str, optional
+            the currency that determines the amount to send worth of receive_currency, by default None
+        address : str, optional
+            the receive_currency address, by default None
+        ipn_url : str, optional
+            the ipn url where the notifications will be sent, by default None
+        auto_confirm : bool, optional
+            if set to True 2fa won't be required, by default False
+
+        Returns
+        -------
+        Union[JsonResponse, str]
+            api response containing containing the withdrawal info
+
+        Example
+        -------
+            `to send 18$ worth of btc, 'btc' is the receive_currency and 'usd' is the base_currency`
         """
 
         cmd='create_withdrawal'
 
         necessary_params = {
             'amount' : amount, 
             'currency' : receive_currency,
@@ -282,34 +367,48 @@
         cmd='create_mass_withdrawal'
 
         # withdrawals is an associative array
 
     
     async def cancel_withdrawal(self, withdrawal_id:int):
         """
-        # Cancel a withdrawal
         Cancel a withdrawal given its id
         """
 
         cmd = 'cancel_withdrawal'
 
         return await self.api_call(cmd, id=withdrawal_id)
     
-    async def convert(self, amount:float, from_currency:str, to_currency:str, to_address:str = None, **params):
+    async def convert(self, amount:float, from_currency:str, to_currency:str, to_address:str = None, **params) -> Union[JsonResponse, str]:
         """
-        # Convert coins
-        Convert your coins and send them to a new address or your own if to_address is set to None
+        convert a currency to another and if passed, send it to another address
+
+        Parameters
+        ----------
+        amount : float
+            the amount of from_currency to convert 
+        from_currency : str
+            the currency to conver
+        to_currency : str
+            the currency to convert to
+        to_address : str, optional
+            the address that will receive the amount of to_currency, by default None
+
+        Returns
+        -------
+        Union[JsonResponse, str]
+            api response containing the convertion informations
         """
 
         cmd = 'convert'
 
         necessary_params = {
             'amount' : amount,
             'from' : from_currency,
-            'to' : to_address,
+            'to' : to_currency,
             'address' : to_address,
         }
 
         return await self.api_call(cmd, **necessary_params, **params)
     
     async def convert_limits(self, from_currency:str, to_currency:str):
 
@@ -440,49 +539,86 @@
             accepted_list = [c for c in accepted_currencies if accepted_currencies[c]['is_fiat'] == 0]
         else:
             accepted_list = [c for c in accepted_currencies]
         
         return accepted_list
 
     async def is_accepted(self, currency:str, fiat_included: bool = True) -> bool:
-        
+        """
+        Check if a currency is accepted by the merchant 
+
+        Parameters
+        ----------
+        currency : str
+            The currency that needs to be checked
+        fiat_included : bool, optional
+            If the command should accept fiat currencies as an input, by default True
+
+        Returns
+        -------
+        bool
+            True if the currency passed is accepted by the merchant else False
+        """
         currency = currency.upper()
         api_response = await self.rates()
         accepted_currencies = self.json_to_result(api_response)
 
         if not fiat_included:
             accepted_currencies = {c : 'accepted' for c in accepted_currencies if accepted_currencies[c]['is_fiat'] == 0}
         
         try:
             accepted_currencies[currency]
             return True
         except KeyError:
             return False
 
-    async def get_balance_accepted(self):
-        """get the balance as a floating of your accepted currencies"""
+    async def get_balance_accepted(self) -> dict:
+        """
+        Get the balance of the accepted currencies by the merchant
+
+        Returns
+        -------
+        dict
+            a dictionary cointaining the currency as the key and its balance as the value
+
+        """
 
         accepted = await self.get_accepted_list()
         balances = self.json_to_result(await self.balances())
         accepted_balances = {}
 
         for coin in accepted:
-            try:
-                balance = balances[coin]['balancef']    
-                accepted_balances |= {coin: balance}
-            except KeyError:
-                raise CoinPaymentsInputError("User input is incorrect")
+            
+            balance = balances[coin]['balancef']    
+            accepted_balances |= {coin: balance}
         
         return accepted_balances
     
-    async def conversion_fiat(self, coin1:str, base_currency:str, from_data:dict = None):
+    async def conversion_fiat(self, coin1:str, base_currency:str, from_data:dict = None) -> float:
         """
-        Returns the conversion rate of any available currency on the site. This is recomended to use only if needed.
-        ### Note
-        The conversion rate might be a bit imprecise depending on how recently the rates endpoint has been updated
+        Get the conversion rate in a fiat currency of any currency accepted by CoinPayments
+
+        Parameters
+        ----------
+        coin1 : str
+            The coin that we want the conversion rate of 
+        base_currency : str
+            The currency, should be fiat, against which we want to compare coin1
+        from_data : dict, optional
+            A previous cached call of the rates endpoint if not passed an api call to said endpoint will be made, by default None
+
+        Returns
+        -------
+        float
+            The exchange rate 
+
+        Raises
+        ------
+        CoinPaymentsInputError
+            If the currencies passed do not exist or are not accepted by CoinPayments
         """
         if from_data:
             rates = from_data
         else:
             rates = self.json_to_result(await self.rates())
         
         coin1 = coin1.upper()
@@ -493,16 +629,32 @@
             base_currency_btc = float(rates[base_currency]['rate_btc'])
         except KeyError:
             raise CoinPaymentsInputError("User input is incorrect")
         
         rate = coin1_btc/base_currency_btc
         return rate
     
-    async def balances_fiat(self, base_currency:str = 'USD', only_accepted:bool = False, all_coins:bool = False):
-        "Returns the amount of cryptocurrency in your wallet against the base coin"
+    async def balances_fiat(self, base_currency:str = 'USD', only_accepted:bool = False, all_coins:bool = False) -> dict:
+        """
+        Get the merchant's balances converted in a set base currency
+
+        Parameters
+        ----------
+        base_currency : str, optional
+            The currency in which the merchant balance will be returned, by default 'USD'
+        only_accepted : bool, optional
+            If set to True the function will return only the balances of the merchant's accepted coins, by default False
+        all_coins : bool, optional
+            If set to True the function will return all balances, even if empty, by default False
+
+        Returns
+        -------
+        dict
+            A dictionary containing the merchant's coin balances converted in the base currency
+        """
 
         new_balances = {}
 
         balances = self.json_to_result(await self.balances(all_coins = all_coins))
         #we call this function once and cache the result
         rates = self.json_to_result(await self.rates(only_accepted = only_accepted))
```

### Comparing `asyncoinpayments-0.0.2a0/asyncoinpayments.egg-info/PKG-INFO` & `asyncoinpayments-0.0.3a0/asyncoinpayments/asyncoinpayments.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 Metadata-Version: 2.1
 Name: asyncoinpayments
-Version: 0.0.2a0
+Version: 0.0.3a0
 Summary: Python Asynchronous Wrapper of the CoinPayments API
-Home-page: https://github.com/flalugli/asyncoinpayments
-Author: flalugli
-Author-email: <flalugli.dev@gmail.com>
 License: Apache License 2.0
-Description: 
-        # AsynCoinpayments  
-        
-        An async/await compatible python wrapper for the CoinPayments API  
-        
-        ---
-        
-        ## How to install  
-        
-        ```
-        # run this in the command propt or terminal
-        pip install asyncoinpayments  
-        ```
-        
-        ## Features  
-        - Fast to setup and simple to use
-        - Easy to use async/await interface
-        - API calls using aiohttp requests  
-        - create your own API calls
-        
-        ### Contact me
-        
-        **Email** : <flalugli.dev@gmail.com>  
-        **Discord** : flalugli   
-        
 Keywords: python,crypto,cryptocurrency,payment gateway,async,aiohttp
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+License-File: LICENSE.txt
+
+# AsynCoinpayments  
+
+An async/await compatible python wrapper for the CoinPayments API  
+
+---
+
+## How to install  
+
+```
+# run this in the command propt or terminal
+pip install asyncoinpayments  
+```
+
+## Features  
+- Fast to setup and simple to use
+- Easy to use async/await interface
+- API calls using aiohttp requests  
+- create your own API calls
+
+### Contact me
+
+**Email** : <flalugli.dev@gmail.com>  
+**Discord** : flalugli
```

