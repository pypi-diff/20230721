# Comparing `tmp/neo-fairy-client-3.5.0.8.tar.gz` & `tmp/neo-fairy-client-3.5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo-fairy-client-3.5.0.8.tar", last modified: Wed Jul 19 10:06:41 2023, max compression
+gzip compressed data, was "neo-fairy-client-3.5.0.9.tar", last modified: Fri Jul 21 02:06:48 2023, max compression
```

## Comparing `neo-fairy-client-3.5.0.8.tar` & `neo-fairy-client-3.5.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 10:06:41.107616 neo-fairy-client-3.5.0.8/
--rw-rw-rw-   0        0        0     1085 2022-05-05 03:19:19.000000 neo-fairy-client-3.5.0.8/LICENSE
--rw-rw-rw-   0        0        0   139301 2023-07-19 10:06:41.107616 neo-fairy-client-3.5.0.8/PKG-INFO
--rw-rw-rw-   0        0        0   138843 2023-06-14 05:42:43.000000 neo-fairy-client-3.5.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 10:06:41.075965 neo-fairy-client-3.5.0.8/neo_fairy_client/
--rw-rw-rw-   0        0        0      109 2022-09-22 08:08:31.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 10:06:41.088590 neo-fairy-client-3.5.0.8/neo_fairy_client/rpc/
--rw-rw-rw-   0        0        0       74 2022-09-21 02:51:06.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/rpc/__init__.py
--rw-rw-rw-   0        0        0    55900 2023-07-19 08:33:35.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/rpc/fairy_client.py
-drwxrwxrwx   0        0        0        0 2023-07-19 10:06:41.099521 neo-fairy-client-3.5.0.8/neo_fairy_client/utils/
--rw-rw-rw-   0        0        0     1379 2022-09-21 06:25:56.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/utils/WitnessRule.py
--rw-rw-rw-   0        0        0      293 2023-04-26 05:30:10.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/utils/__init__.py
--rw-rw-rw-   0        0        0     1588 2022-10-25 06:12:11.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/utils/interpreters.py
--rw-rw-rw-   0        0        0      195 2022-09-28 04:32:29.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/utils/misc.py
--rw-rw-rw-   0        0        0     1319 2022-10-25 06:12:11.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/utils/timers.py
--rw-rw-rw-   0        0        0     5625 2022-10-10 02:34:50.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-07-19 10:06:41.102563 neo-fairy-client-3.5.0.8/neo_fairy_client/vm/
--rw-rw-rw-   0        0        0       58 2022-09-21 02:49:39.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/vm/__init__.py
--rw-rw-rw-   0        0        0    15030 2022-09-22 08:50:45.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/vm/fairy_engine.py
-drwxrwxrwx   0        0        0        0 2023-07-19 10:06:41.105567 neo-fairy-client-3.5.0.8/neo_fairy_client/websocket/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:00:53.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/websocket/__init__.py
--rw-rw-rw-   0        0        0     4694 2023-03-06 02:47:25.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/websocket/fairy_websocket.py
-drwxrwxrwx   0        0        0        0 2023-07-19 10:06:41.085550 neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/
--rw-rw-rw-   0        0        0   139301 2023-07-19 10:06:41.000000 neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-07-19 10:06:41.000000 neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 10:06:41.000000 neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-19 10:06:41.000000 neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-19 10:06:41.000000 neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 10:06:41.108619 neo-fairy-client-3.5.0.8/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-07-19 08:33:50.000000 neo-fairy-client-3.5.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:06:48.708897 neo-fairy-client-3.5.0.9/
+-rw-rw-rw-   0        0        0     1085 2022-05-05 03:19:19.000000 neo-fairy-client-3.5.0.9/LICENSE
+-rw-rw-rw-   0        0        0   139301 2023-07-21 02:06:48.708897 neo-fairy-client-3.5.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0   138843 2023-06-14 05:42:43.000000 neo-fairy-client-3.5.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 02:06:48.692909 neo-fairy-client-3.5.0.9/neo_fairy_client/
+-rw-rw-rw-   0        0        0      109 2022-09-22 08:08:31.000000 neo-fairy-client-3.5.0.9/neo_fairy_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:06:48.697913 neo-fairy-client-3.5.0.9/neo_fairy_client/rpc/
+-rw-rw-rw-   0        0        0       74 2022-09-21 02:51:06.000000 neo-fairy-client-3.5.0.9/neo_fairy_client/rpc/__init__.py
+-rw-rw-rw-   0        0        0    57117 2023-07-21 02:06:15.000000 neo-fairy-client-3.5.0.9/neo_fairy_client/rpc/fairy_client.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:06:48.703672 neo-fairy-client-3.5.0.9/neo_fairy_client/utils/
+-rw-rw-rw-   0        0        0     1379 2022-09-21 06:25:56.000000 neo-fairy-client-3.5.0.9/neo_fairy_client/utils/WitnessRule.py
+-rw-rw-rw-   0        0        0      962 2023-07-20 06:20:43.000000 neo-fairy-client-3.5.0.9/neo_fairy_client/utils/__init__.py
+-rw-rw-rw-   0        0        0     1588 2022-10-25 06:12:11.000000 neo-fairy-client-3.5.0.9/neo_fairy_client/utils/interpreters.py
+-rw-rw-rw-   0        0        0      195 2022-09-28 04:32:29.000000 neo-fairy-client-3.5.0.9/neo_fairy_client/utils/misc.py
+-rw-rw-rw-   0        0        0     1319 2022-10-25 06:12:11.000000 neo-fairy-client-3.5.0.9/neo_fairy_client/utils/timers.py
+-rw-rw-rw-   0        0        0     5625 2022-10-10 02:34:50.000000 neo-fairy-client-3.5.0.9/neo_fairy_client/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:06:48.705896 neo-fairy-client-3.5.0.9/neo_fairy_client/vm/
+-rw-rw-rw-   0        0        0       58 2022-09-21 02:49:39.000000 neo-fairy-client-3.5.0.9/neo_fairy_client/vm/__init__.py
+-rw-rw-rw-   0        0        0    15030 2022-09-22 08:50:45.000000 neo-fairy-client-3.5.0.9/neo_fairy_client/vm/fairy_engine.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:06:48.706897 neo-fairy-client-3.5.0.9/neo_fairy_client/websocket/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:00:53.000000 neo-fairy-client-3.5.0.9/neo_fairy_client/websocket/__init__.py
+-rw-rw-rw-   0        0        0     4694 2023-03-06 02:47:25.000000 neo-fairy-client-3.5.0.9/neo_fairy_client/websocket/fairy_websocket.py
+drwxrwxrwx   0        0        0        0 2023-07-21 02:06:48.696912 neo-fairy-client-3.5.0.9/neo_fairy_client.egg-info/
+-rw-rw-rw-   0        0        0   139301 2023-07-21 02:06:48.000000 neo-fairy-client-3.5.0.9/neo_fairy_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-07-21 02:06:48.000000 neo-fairy-client-3.5.0.9/neo_fairy_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 02:06:48.000000 neo-fairy-client-3.5.0.9/neo_fairy_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-21 02:06:48.000000 neo-fairy-client-3.5.0.9/neo_fairy_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-21 02:06:48.000000 neo-fairy-client-3.5.0.9/neo_fairy_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 02:06:48.708897 neo-fairy-client-3.5.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-07-20 02:38:59.000000 neo-fairy-client-3.5.0.9/setup.py
```

### Comparing `neo-fairy-client-3.5.0.8/LICENSE` & `neo-fairy-client-3.5.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.8/PKG-INFO` & `neo-fairy-client-3.5.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-fairy-client
-Version: 3.5.0.8
+Version: 3.5.0.9
 Summary: Test & debug your Neo3 smart contracts
 Home-page: https://github.com/Hecate2/neo-fairy-client
 Author: Hecate2
 Author-email: hecate2@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neo-fairy-client-3.5.0.8/README.md` & `neo-fairy-client-3.5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.8/neo_fairy_client/rpc/fairy_client.py` & `neo-fairy-client-3.5.0.9/neo_fairy_client/rpc/fairy_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 from typing import List, Union, Dict, Any, Callable
 import base64
 import json
 import os
+import random
 import traceback
 import requests
 import urllib3
 
 from neo_fairy_client.utils import Hash160Str, Hash256Str, PublicKeyStr, Signer
-from neo_fairy_client.utils import Interpreter, to_list
+from neo_fairy_client.utils import Interpreter, to_list, NeoAddress, GasAddress
 from neo3.core.types import UInt160, UInt256
-from neo3.contracts import (PolicyContract, NeoToken, GasToken, OracleContract, DesignationContract, ManagementContract, LedgerContract, CryptoContract, StdLibContract)
 from neo3vm import VMState
 
-PolicyAddress = Hash160Str.from_UInt160(PolicyContract().hash)
-NeoAddress = Hash160Str.from_UInt160(NeoToken().hash)
-GasAddress = Hash160Str.from_UInt160(GasToken().hash)
-OracleAddress = Hash160Str.from_UInt160(OracleContract().hash)
-DesignationAddress = Hash160Str.from_UInt160(DesignationContract().hash)
-ManagementAddress = Hash160Str.from_UInt160(ManagementContract().hash)
-LedgerAddress = Hash160Str.from_UInt160(LedgerContract().hash)
-CryptoLibAddress = Hash160Str.from_UInt160(CryptoContract().hash)
-StdLibAddress = Hash160Str.from_UInt160(StdLibContract().hash)
-
 RequestExceptions = (
     requests.RequestException,
     requests.ConnectionError,
     requests.HTTPError,
     requests.Timeout,
 )
 default_request_timeout = None  # 20
@@ -56,19 +46,19 @@
     def from_raw_result(cls, result: Dict):
         result = result['result']
         return cls(result['state'], result['breakreason'], result['scripthash'], result['contractname'],
                    result['instructionpointer'], source_filename=result['sourcefilename'], source_line_num=result['sourcelinenum'], source_content=result['sourcecontent'])
     
     def __repr__(self):
         if self.state == VMState.HALT:
-            return f'''RpcBreakpoint {self.state} {self.result_stack}'''
+            return f'''{self.state} {self.result_stack}'''
         if self.source_filename and self.source_line_num:
-            return f'''RpcBreakpoint {self.state} {self.source_filename} line {self.source_line_num} instructionPointer {self.instruction_pointer}: {self.source_content}'''
+            return f'''{self.state} {self.break_reason} {self.source_filename} line {self.source_line_num} instructionPointer {self.instruction_pointer}: {self.source_content}'''
         else:
-            return f'''RpcBreakpoint {self.state} {self.contract_name} instructionPointer {self.instruction_pointer};'''
+            return f'''{self.state} {self.break_reason} {self.contract_name} instructionPointer {self.instruction_pointer};'''
 
 
 class FairyClient:
     def __init__(self, target_url: str = 'http://localhost:16868',
                  wallet_address_or_scripthash: Union[str, Hash160Str] = None,
                  contract_scripthash: Hash160Str = None, signers: Union[Signer, List[Signer], None] = None,
                  fairy_session: str = None, function_default_relay=True, script_default_relay=False,
@@ -203,14 +193,15 @@
             self.hook_function_after_rpc_call()
         return result
 
     def meta_rpc_method(self, method: str, parameters: List, relay: bool = None, do_not_raise_on_result=False) -> Any:
         post_data = self.request_body_builder(method, parameters)
         self.previous_post_data = post_data
         result = json.loads(self.requests_session.post(self.target_url, post_data, timeout=self.requests_timeout, verify=self.verify_SSL).text)
+        self.previous_raw_result = result
         if 'error' in result:
             raise ValueError(f"""{result['error']['message']}\r\n{result['error']['data']}""" if 'data' in result['error'] else result['error'])
         if type(result['result']) is dict:
             result_result: dict = result['result']
             if gas_consumed := result_result.get('gasconsumed'):
                 self.previous_gas_consumed = int(gas_consumed)
             if gas_consumed := result_result.get('networkfee'):
@@ -234,15 +225,14 @@
                     self.previous_txBase64Str = tx
                     if self.confirm_relay_to_blockchain is False \
                         or input(f"Write transaction {tx} to the actual blockchain instead of Fairy? "
                                  f"Y/[n]: ") == "Y":
                         self.sendrawtransaction(tx)
                 # else:
                 #     self.previous_txBase64Str = None
-        self.previous_raw_result = result
         self.previous_result = self.parse_stack_from_raw_result(result)
         if self.hook_function_after_rpc_call:
             self.hook_function_after_rpc_call()
         if self.verbose_return:
             return self.previous_result, result, post_data
         return self.previous_result
     
@@ -366,15 +356,15 @@
         if len(stack) > 1:  # typically happens when we invoke a script calling a series of methods
             return [self.parse_single_item(item) for item in stack]
         else:  # if the stack has only 1 item, we simply return the item without a wrapping list
             result: List = stack[0]
             return self.parse_single_item(result)
     
     @classmethod
-    def parse_params(cls, param: Union[str, int, dict, Hash160Str, UInt160, UInt256, bytes, bytearray]) -> Dict[str, str]:
+    def parse_param(cls, param: Union[str, int, dict, Hash160Str, UInt160, UInt256, bytes, bytearray]) -> Dict[str, str]:
         type_param = type(param)
         if type_param is UInt160:
             return {
                 'type': 'Hash160',
                 'value': str(Hash160Str.from_UInt160(param)),
             }
         elif type_param is Hash160Str:
@@ -423,56 +413,56 @@
                 return {
                     'type': 'ByteArray',
                     'value': base64.b64encode(param).decode()
                 }
         elif type_param is list:
             return {
                 'type': 'Array',
-                'value': [cls.parse_params(param_) for param_ in param]
+                'value': [cls.parse_param(param_) for param_ in param]
             }
         elif type_param is dict:
             return {
                 'type': 'Map',
-                'value': [{'key': cls.parse_params(k), 'value': cls.parse_params(v)} for k, v in param.items()]
+                'value': [{'key': cls.parse_param(k), 'value': cls.parse_param(v)} for k, v in param.items()]
             }
         elif param is None:
             return {
                 'type': 'Any',
             }
         raise ValueError(f'Unable to handle param {param} with type {type_param}')
     
     def invokefunction_of_any_contract(self, scripthash: Hash160Str, operation: str,
-                                       params: List[Union[str, int, dict, Hash160Str, UInt160, bytes, bytearray]] = None,
+                                       params: List[Union[List, str, int, dict, Hash160Str, UInt160, bytes, bytearray]] = None,
                                        signers: Union[Signer, List[Signer]] = None, relay: bool = None, do_not_raise_on_result=False,
                                        with_print=True, fairy_session: str = None) -> Any:
         fairy_session = fairy_session or self.fairy_session
         params = params or []
         signers = to_list(signers or self.signers)
         if self.with_print and with_print:
             if fairy_session:
                 print(f'{fairy_session}::{operation}{params} relay={relay} {signers}')
             else:
                 print(f'{operation}{params} relay={relay} {signers}')
         
         parameters = [
             str(scripthash),
             operation,
-            list(map(lambda param: self.parse_params(param), params)),
+            list(map(lambda param: self.parse_param(param), params)),
             list(map(lambda signer: signer.to_dict(), signers)),
         ]
         if fairy_session:
             result = self.meta_rpc_method(
                 'invokefunctionwithsession', [fairy_session, relay or (relay is None and self.function_default_relay)] + parameters, relay=False,
                 do_not_raise_on_result=do_not_raise_on_result)
         else:
             result = self.meta_rpc_method('invokefunction', parameters, relay=relay,
                                           do_not_raise_on_result=do_not_raise_on_result)
         return result
     
-    def invokefunction(self, operation: str, params: List[Union[str, int, Hash160Str, UInt160, bytes, bytearray]] = None,
+    def invokefunction(self, operation: str, params: List[Union[List, str, int, Hash160Str, UInt160, bytes, bytearray]] = None,
                        signers: Union[Signer, List[Signer]] = None, relay: bool = None, do_not_raise_on_result=False, with_print=True,
                        fairy_session: str = None) -> Any:
         if self.contract_scripthash is None or self.contract_scripthash == Hash160Str.zero():
             raise ValueError(f'Please set client.contract_scripthash before invoking function. Got {self.contract_scripthash}')
         return self.invokefunction_of_any_contract(self.contract_scripthash, operation, params,
                                                    signers=signers, relay=relay or (relay is None and self.function_default_relay),
                                                    do_not_raise_on_result=do_not_raise_on_result,
@@ -490,41 +480,44 @@
         if self.with_print and with_print:
             print(f'{fairy_session}::{call_arguments} relay={relay} {signers}')
     
         parsed_call_arguments = [  # [ [contract_scripthash: Hash160Str, operation: str, args[] ] ]
             [
                 str(call[0]) if type(call[0]) is Hash160Str else str(self.contract_scripthash),
                 call[1] if type(call[0]) is Hash160Str else call[0],
-                list(map(lambda param: self.parse_params(param), call[-1]) if len(call) >= 2 else [])
+                list(map(lambda param: self.parse_param(param), call[-1]) if len(call) >= 2 else [])
             ]
             for call in call_arguments
         ]
         return self.meta_rpc_method(
             'invokemanywithsession', [fairy_session, relay or (relay is None and self.function_default_relay), parsed_call_arguments, list(map(lambda signer: signer.to_dict(), signers))], relay=False,
             do_not_raise_on_result=do_not_raise_on_result)
 
-    def invokescript(self, script: Union[str, bytes], signers: Union[Signer, List[Signer]] = None, relay: bool = None,
+    def invokescript(self, script_base64_encoded: Union[str, bytes], signers: Union[Signer, List[Signer]] = None, relay: bool = None,
                      fairy_session: str = None) -> Any:
-        if type(script) is bytes:
-            script: str = script.decode()
+        if type(script_base64_encoded) is bytes:
+            script_base64_encoded: str = script_base64_encoded.decode()
         signers = to_list(signers or self.signers)
         fairy_session = fairy_session or self.fairy_session
         if fairy_session:
             relay = relay or (relay is None and self.script_default_relay)
             result = self.meta_rpc_method(
                 'invokescriptwithsession',
-                [fairy_session, relay, script, list(map(lambda signer: signer.to_dict(), signers))],
+                [fairy_session, relay, script_base64_encoded, list(map(lambda signer: signer.to_dict(), signers))],
                 relay=False)
         else:
             result = self.meta_rpc_method(
                 'invokescript',
-                [script, list(map(lambda signer: signer.to_dict(), signers))],
+                [script_base64_encoded, list(map(lambda signer: signer.to_dict(), signers))],
                 relay=relay)
         return result
     
+    def get_block_count(self) -> int:
+        return self.meta_rpc_method("getblockcount", [])
+    
     def sendfrom(self, asset_id: Hash160Str, from_address: str, to_address: str, value: int,
                  signers: List[Signer] = None):
         """
 
         :param asset_id: NEO: '0xef4073a0f2b305a38ec4050e4d3d28bc40ea63f5';
             GAS: '0xd2a4cff31913016155e38e474a2c06d08be276cf'
         :param from_address: "NgaiKFjurmNmiRzDRQGs44yzByXuSkdGPF"
@@ -600,14 +593,42 @@
 
     def set_session_fairy_wallet_with_WIF(self, wif: str, password: str, fairy_session: str = None) -> dict:
         open_wallet_result = self.meta_rpc_method("setsessionfairywalletwithwif", [fairy_session or self.fairy_session, wif, password])
         if not open_wallet_result:
             raise ValueError(f'Failed to open WIF wallet {wif} with given password.')
         return open_wallet_result
 
+    def force_sign_transaction(self, fairy_session: str = None, script_base64_encoded: Union[str, bytes, None] = None,
+                               signers: List[Signer] = None, system_fee: int = 1000_0000, network_fee: int = 0,
+                               valid_until_block: Union[int, None] = 0, nonce: int = 0) -> Dict[str, Any]:
+        """
+        Build and sign a transaction with the fairy wallet of the fairy_session,
+        even if the transaction cannot be run correctly
+        :param fairy_session:
+        :param script_base64_encoded:
+        :param signers:
+        :param system_fee:
+        :param network_fee:
+        :param valid_until_block:
+        :param nonce: WARNING: never publish multiple signatures using the same nonce! This will leak your private key!
+        :return:
+        """
+        fairy_session = fairy_session or self.fairy_session
+        if type(script_base64_encoded) is bytes:
+            script_base64_encoded: str = script_base64_encoded.decode()
+        script_base64_encoded: str = script_base64_encoded or self.previous_raw_result['result']['script']
+        signers = to_list(signers or self.signers)
+        valid_until_block = self.get_block_count() + 5760 if valid_until_block is None else valid_until_block
+        nonce = nonce or random.randint(0, 2**32 - 1)
+        result = self.meta_rpc_method("forcesigntransaction", [fairy_session, script_base64_encoded, list(map(lambda signer: signer.to_dict(), signers)), system_fee, network_fee, valid_until_block, nonce], relay=False)
+        if 'txHash' in result:
+            result['txHash'] = Hash256Str(result['txHash'])
+            self.previous_raw_result = result
+        return result['tx']
+
     def get_time_milliseconds(self) -> int:
         """
         :return: blockchain timestamp in milliseconds
         """
         return self.meta_rpc_method('gettime', [])['time']
 
     def new_snapshots_from_current_system(self, fairy_sessions: Union[List[str], str] = None):
@@ -888,15 +909,15 @@
                 print(f'debugfunction {operation}')
     
         params = params or []
         signers = to_list(signers or self.signers)
         parameters = [
             str(scripthash),
             operation,
-            list(map(lambda param: self.parse_params(param), params)),
+            list(map(lambda param: self.parse_param(param), params)),
             list(map(lambda signer: signer.to_dict(), signers)),
         ]
         raw_result = self.meta_rpc_method_with_raw_result(
             'debugfunctionwithsession',
             [fairy_session, relay or (relay is None and self.function_default_relay)] + parameters)
         result = raw_result['result']
         return RpcBreakpoint(result['state'], result['breakreason'],
```

### Comparing `neo-fairy-client-3.5.0.8/neo_fairy_client/utils/WitnessRule.py` & `neo-fairy-client-3.5.0.9/neo_fairy_client/utils/WitnessRule.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.8/neo_fairy_client/utils/interpreters.py` & `neo-fairy-client-3.5.0.9/neo_fairy_client/utils/interpreters.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.8/neo_fairy_client/utils/timers.py` & `neo-fairy-client-3.5.0.9/neo_fairy_client/utils/timers.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.8/neo_fairy_client/utils/types.py` & `neo-fairy-client-3.5.0.9/neo_fairy_client/utils/types.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.8/neo_fairy_client/vm/fairy_engine.py` & `neo-fairy-client-3.5.0.9/neo_fairy_client/vm/fairy_engine.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.8/neo_fairy_client/websocket/fairy_websocket.py` & `neo-fairy-client-3.5.0.9/neo_fairy_client/websocket/fairy_websocket.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/PKG-INFO` & `neo-fairy-client-3.5.0.9/neo_fairy_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-fairy-client
-Version: 3.5.0.8
+Version: 3.5.0.9
 Summary: Test & debug your Neo3 smart contracts
 Home-page: https://github.com/Hecate2/neo-fairy-client
 Author: Hecate2
 Author-email: hecate2@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/SOURCES.txt` & `neo-fairy-client-3.5.0.9/neo_fairy_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.8/setup.py` & `neo-fairy-client-3.5.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="neo-fairy-client",
-    version="3.5.0.8",
+    version="3.5.0.9",
     author="Hecate2",
     author_email="hecate2@qq.com",
     description="Test & debug your Neo3 smart contracts",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Hecate2/neo-fairy-client",
     packages=setuptools.find_packages(),
```

