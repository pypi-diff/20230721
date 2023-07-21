# Comparing `tmp/rave_python-1.2.9.tar.gz` & `tmp/rave_python-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rave_python-1.2.9.tar", last modified: Sat Jan 23 01:35:53 2021, max compression
+gzip compressed data, was "dist/rave_python-1.4.0.tar", last modified: Fri Jul 21 14:56:23 2023, max compression
```

## Comparing `rave_python-1.2.9.tar` & `rave_python-1.4.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-23 01:35:53.864280 rave_python-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (116)   104876 2021-01-23 01:35:53.864280 rave_python-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    82254 2021-01-23 01:35:44.000000 rave_python-1.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-23 01:35:53.864280 rave_python-1.2.9/rave_python/
--rw-r--r--   0 runner    (1001) docker     (116)      262 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2808 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave.py
--rw-r--r--   0 runner    (1001) docker     (116)     3221 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_account.py
--rw-r--r--   0 runner    (1001) docker     (116)     7807 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_base.py
--rw-r--r--   0 runner    (1001) docker     (116)     3506 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_bills.py
--rw-r--r--   0 runner    (1001) docker     (116)     7104 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_card.py
--rw-r--r--   0 runner    (1001) docker     (116)     3747 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_ebills.py
--rw-r--r--   0 runner    (1001) docker     (116)     8446 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     3706 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_francophone.py
--rw-r--r--   0 runner    (1001) docker     (116)     1924 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_ghmobile.py
--rw-r--r--   0 runner    (1001) docker     (116)     5280 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_misc.py
--rw-r--r--   0 runner    (1001) docker     (116)     2359 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_mpesa.py
--rw-r--r--   0 runner    (1001) docker     (116)    17801 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_payment.py
--rw-r--r--   0 runner    (1001) docker     (116)     5335 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_paymentplan.py
--rw-r--r--   0 runner    (1001) docker     (116)     3709 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_preauth.py
--rw-r--r--   0 runner    (1001) docker     (116)     3946 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_recepient.py
--rw-r--r--   0 runner    (1001) docker     (116)     3946 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_recipient.py
--rw-r--r--   0 runner    (1001) docker     (116)     1968 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_rwmobile.py
--rw-r--r--   0 runner    (1001) docker     (116)     3042 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_settlement.py
--rw-r--r--   0 runner    (1001) docker     (116)     5617 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_subaccounts.py
--rw-r--r--   0 runner    (1001) docker     (116)     4031 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_subscription.py
--rw-r--r--   0 runner    (1001) docker     (116)     9243 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_transfer.py
--rw-r--r--   0 runner    (1001) docker     (116)     1939 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_ugmobile.py
--rw-r--r--   0 runner    (1001) docker     (116)     3318 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_ussd.py
--rw-r--r--   0 runner    (1001) docker     (116)     3547 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_verify.py
--rw-r--r--   0 runner    (1001) docker     (116)     4045 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_virtualaccount.py
--rw-r--r--   0 runner    (1001) docker     (116)     8248 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_virtualcard.py
--rw-r--r--   0 runner    (1001) docker     (116)     1937 2021-01-23 01:35:44.000000 rave_python-1.2.9/rave_python/rave_zbmobile.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-23 01:35:53.864280 rave_python-1.2.9/rave_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)   104876 2021-01-23 01:35:53.000000 rave_python-1.2.9/rave_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      989 2021-01-23 01:35:53.000000 rave_python-1.2.9/rave_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-23 01:35:53.000000 rave_python-1.2.9/rave_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       22 2021-01-23 01:35:53.000000 rave_python-1.2.9/rave_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2021-01-23 01:35:53.000000 rave_python-1.2.9/rave_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-23 01:35:53.864280 rave_python-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1102 2021-01-23 01:35:44.000000 rave_python-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:56:23.000000 rave_python-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)   121422 2023-07-21 14:56:23.000000 rave_python-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    95161 2023-07-21 14:56:07.000000 rave_python-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:56:23.000000 rave_python-1.4.0/rave_python/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_banktransfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_bills.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_ebills.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_enaira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_francophone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_ghmobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_mpesa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20137 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_paymentplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_preauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_recepient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_rwmobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_settlement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_subaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_tzmobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_ugmobile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_ussd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_virtualaccount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_virtualcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-21 14:56:07.000000 rave_python-1.4.0/rave_python/rave_zbmobile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:56:23.000000 rave_python-1.4.0/rave_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)   121422 2023-07-21 14:56:23.000000 rave_python-1.4.0/rave_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-21 14:56:23.000000 rave_python-1.4.0/rave_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:56:23.000000 rave_python-1.4.0/rave_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 14:56:23.000000 rave_python-1.4.0/rave_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 14:56:23.000000 rave_python-1.4.0/rave_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 14:56:23.000000 rave_python-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-21 14:56:07.000000 rave_python-1.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `rave_python-1.2.9/PKG-INFO` & `rave_python-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,77 @@
 Metadata-Version: 2.1
 Name: rave_python
-Version: 1.2.9
-Summary: Official Rave Python Wrapper By Flutterwave
+Version: 1.4.0
+Summary: Python library for Flutterwave for Business (F4B) v2 APIs.
 Home-page: https://github.com/Flutterwave/rave-python
 Author: Flutterwave
 Author-email: developers@flutterwavego.com
 License: MIT
 Description: <p align="center">
-            <img title="Flutterwave" height="200" src="https://flutterwave.com/images/logo-colored.svg" width="50%"/>
+            <img title="Flutterwave" height="200" src="https://flutterwave.com/images/logo/full.svg" width="50%"/>
         </p>
         
-        # Rave Python Library.
+        # Flutterwave Python Library.
         ![Upload Python Package](https://github.com/Flutterwave/rave-python/workflows/Upload%20Python%20Package/badge.svg)
         ![PyPI](https://img.shields.io/pypi/v/rave_python)
         ![PyPI - Downloads](https://img.shields.io/pypi/dm/rave_python)
         ![PyPI - License](https://img.shields.io/pypi/l/rave_python)
         
         
         ## Introduction
-        This is a Python wrapper around the [API](https://flutterwavedevelopers.readme.io/v2.0/reference) for [Rave by Flutterwave](https://rave.flutterwave.com).
+        The Python library provides easy access to Flutterwave for Business (F4B) v2 APIs from Django, Flask, and other Python apps. It abstracts the complexity involved in direct integration and allows you to make quick calls to the APIs.
+        
+        Available features include:
+        
+        - Collections: Card, Account, Mobile money, Bank Transfers, USSD, Barter, NQR.
+        - Payouts and Beneficiaries.
+        - Recurring payments: Tokenization and Subscriptions.
+        - Split payments
+        - Card issuing
+        - Transactions dispute management: Refunds.
+        - Transaction reporting: Collections, Payouts, Settlements, and Refunds.
+        - Bill payments: Airtime, Data bundle, Cable, Power, Toll, E-bills, and Remitta.
+        - Identity verification: Resolve bank account, resolve BVN information.
+        
+        ## Table of Contents
+        1. [Requirements](#requirements)
+        2. [Installation](#installation)
+        3. [Initialization](#initialization)
+        4. [Usage](#usage)
+        5. [Testing](#testing)
+        6. [Debugging Errors](#debugging-errors)
+        7. [Support](#support)
+        8. [Contribution guidelines](#)
+        9. [License](#)
+        10. [Changelog](#)
+        
+        ## Requirements
+        1. Flutterwave for business [API Keys](https://developer.flutterwave.com/docs/integration-guides/authentication)
+        2. Supported Python versions: >=2.7, !=3.0.\*, !=3.1.\*, !=3.2.\*, !=3.3.\*, !=3.4.\*
         
-        #### Payment types implemented:
-        * Card Payments
-        * Bank Account Payments
-        * Ghana Mobile Money Payments
-        * Mpesa Payments
-        * Rwanda Mobile Money Payments
-        * Uganda Mobile Money Payments
-        * Zambia Mobile Money Payments
-        * Mobile Money Payments for Francophone countries
-        * Subaccounts
-        * Transfer
-        * Subscription (Recurring Payments)
-        * Bills payment
-        * Payment Plan
-        * USSD Payments (Still in Beta Mode)
-        
-        #### Other features include:
-        * Preauthorization charges
-        * Refunds
-        * Transaction Verification
-        * Transfer Recipients
-        * Virtual Cards
-        * Virtual Accounts
         
         ## Installation
-        To install, run
+        To install the library, run
         
         ```sh
         pip install rave_python
         ```
         
         Note: This is currently under active development
-        ## Import Package
+        
+        
+        ## Initialization
+        
+        ### Import Package
         The base class for this package is 'Rave'. To use this class, add:
         
         ```py
         from rave_python import Rave
         ```
         
-        ## Initialization
-        
         #### To instantiate in sandbox:
         To use Rave, instantiate the Rave class with your public key. We recommend that you store your secret key in an environment variable named, ```RAVE_SECRET_KEY```. Instantiating your rave object is therefore as simple as:
         
         ```py
         rave = Rave("YOUR_PUBLIC_KEY")
         ```
         
@@ -79,15 +86,17 @@
         #### To instantiate in production:
         To initialize in production, simply set the ```production``` flag to ```True```. It is highly discouraged but if you choose to not use environment variables, you can do so in the same way mentioned above.
         
         ```py
         rave = Rave("YOUR_PUBLIC_KEY", production=True)
         ```
         
-        # Rave Objects
+        
+        
+        # Usage
         This is the documentation for all of the components of rave_python
         
         ## ```rave.Card```
         This is used to facilitate card transactions.
         
         **Functions included:**
         
@@ -244,15 +253,15 @@
         This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
         
         Sample
         ```py
         {'flwRef': None, 'cardToken': u'flw-t1nf-5b0f12d565cd961f73c51370b1340f1f-m03k', 'chargedAmount': 100, 'amount': 100, 'transactionComplete': True, 'error': False, 'txRef': u'MC-1538095718251'}
         ```
         
-        #### Please note that after charging a card successfully on rave, if you wish to save the card for further charges, in your verify payment response you will find an object: "cardtoken": "flw-t0-f6f915f53a094671d98560272572993e-m03k".  This is the token you will use for card tokenization. Details are provided below.
+        > Please note that after charging a card successfully on rave, if you wish to save the card for further charges, in your verify payment response you will find an object: `"cardtoken": "flw-t0-f6f915f53a094671d98560272572993e-m03k"`.  This is the token you will use for card tokenization. Details are provided below.
         
         If your call could not be completed successfully, a ```TransactionVerificationError``` is raised.
         
         <br>
         
         ### ```.charge(payload_for_saved_card, chargeWithToken=True)```
         This is called to start a card transaction with a card that has been saved. The payload should be a dictionary containing card information. It should have the parameters:
@@ -399,40 +408,33 @@
         except RaveExceptions.TransactionVerificationError as e:
             print(e.err["errMsg"])
             print(e.err["txRef"])
         ```
         
         <br><br>
         ## ```rave.Account```
-        This is used to facilitate account transactions.
+        This is used to facilitate account transactions. Transactions initiated via this method are authorized by the user on their Banking platform.
         
         **Functions included:**
         
         * ```.charge```
-        
-        * ```.validate```
-        
         * ```.verify```
         
         <br>
         
         ### ```.charge(payload)```
-        This is called to start an account transaction. The payload should be a dictionary containing card information. It should have the parameters:
-        
-        * ```accountbank```, 
-        
-        * ```accountnumber```, 
-        
-        * ```amount```, 
+        This is called to start an account transaction. The payload should be a dictionary containing payment information. It should have the parameters:
         
+        * ```amount``` (The min amount for NGN account payments is N200. For GBP and EUR payments, the min amount is 1), 
+        * ```currency``` (This payment option supports NGN, GBP and EUR),  
         * ```email```, 
-        
-        * ```phonenumber```, 
-        
-        * ```IP```
+        * ```firstname```, 
+        * ```lastname```, 
+        * ```IP``` (optional)
+        * ```redirectUrl``` (optional)
         
         Optionally, you can add a custom transaction reference using the ```txRef``` parameter. Note that if you do not specify one, it would be automatically generated. We do provide a function for generating transaction references in the [Misc library](https://github.com/Flutterwave/rave-python/blob/master/rave_python/rave_misc.py).
         
         
         A sample call is:
         
         ```py
@@ -440,15 +442,22 @@
         ```
         
         #### Returns
         
         This call returns a dictionary. A sample response is:
         
         ```py
-         {'error': False, 'validationRequired': True, 'txRef': 'MC-1530899106006', 'flwRef': 'ACHG-1530899109682', 'authUrl': None}
+        # sample response for NGN account payments
+         {
+           "validationRequired":True,
+           "authUrl":"https://api.ravepay.co/flwv3-pug/getpaid/api/short-url/vHWOLuy89",
+           "flwRef":"XINH44931689941420152189",
+           "txRef":"MC-1689941418883",
+           "error":False
+        }
         ```
         
          This call raises an ```AccountChargeError``` if there was a problem processing your transaction. The ```AccountChargeError``` contains some information about your transaction. You can handle this as such:
         
         ```py
         try: 
             #Your charge call
@@ -461,77 +470,57 @@
         
         ```py
         {'error': True, 'txRef': 'MC-1530897824739', 'flwRef': None, 'errMsg': 'Sorry, that account number is invalid, please check and try again'}
         ```
         
         <br>
         
-        ### ```.validate(txRef)```
-        
-        After a successful charge, most times you will be asked to verify with OTP. To check if this is required, check the ```validationRequired``` key in the ```res``` of the charge call.
-        
-        In the case that an ```authUrl``` is returned from your charge call, you may skip the validation step and simply pass your authUrl to the end-user. 
-        
-        ```py
-        authUrl = res['authUrl']
-        ```
-        
-        To validate, you need to pass the ```flwRef``` from the ```res``` of the charge call as well as the OTP.
-        
-        A sample validate call is: 
-        
-        ```py
-        res2 = rave.Account.validate(res["flwRef"], "12345")
-        ```
-        
-        
-        #### Returns
-        
-        This call returns a dictionary containing the ```txRef```, ```flwRef``` among others if successful.
-        
-        This call raises a ```TransactionValidationError``` if the OTP is not correct or there was a problem processing your request. 
-        
-        To handle this, write:
-        
-        ```py
-        try:
-            # Your charge call
-        except RaveExceptions.TransactionValidationError as e:
-            print(e.err["errMsg"])
-            print(e.err["flwRef"])
-        ```
-        
-        A sample ``` e.err ``` contains:
-        
-        ```py
-        {'error': True, 'txRef': 'MC-1530899869968', 'flwRef': 'ACHG-1530899873118', 'errMsg': 'Pending OTP validation'}
-        ```
-        
-        
-        
-        <br>
-        
         ### ```.verify(txRef)```
         
-        You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned any of the calls (```charge``` or ```validate```). 
+        You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned any the ```charge```call. 
         
         A sample verify call is:
         
         ```py
         res = rave.Account.verify(data["txRef"])
         ```
         
         #### Returns
         
         This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
         
         Sample
         
         ```py
-        {'status': u'success', 'vbvcode': u'N/A', 'chargedamount': 500, 'vbvmessage': u'N/A', 'error': False, 'flwRef': u'ACHG-1538093023787', 'currency': u'NGN', 'amount': 500, 'transactionComplete': True, 'acctmessage': u'Approved Or Completed Successfully', 'chargecode': u'00', 'txRef': u'MC-1538093008498'}
+        {
+           "status":"success",
+           "vbvcode":"57",
+           "chargemessage":"Pending validation",
+           "chargedamount":200,
+           "vbvmessage":"transaction was abandoned",
+           "error":True,
+           "flwRef":"XINH44931689941420152189",
+           "currency":"NGN",
+           "amount":200,
+           "meta":[
+              {
+                 "getpaidTransactionId":984928641,
+                 "metavalue":"12383",
+                 "metaname":"test",
+                 "updatedAt":"2023-07-21T12:10:19.000Z",
+                 "deletedAt":"None",
+                 "id":2168360293,
+                 "createdAt":"2023-07-21T12:10:19.000Z"
+              }
+           ],
+           "transactionComplete":False,
+           "acctmessage":None,
+           "chargecode":"02",
+           "txRef":"MC-1689941418883"
+        }
         ```
         
         If your call could not be completed successfully or if a wrong ```txRef``` is passed, a ```TransactionVerificationError``` is raised. You can handle that as such
         ```py
         try: 
             #Your charge call
         except RaveExceptions.TransactionVerificationError as e:
@@ -564,22 +553,27 @@
         ### Complete account flow
         
         ```py
         from rave_python import Rave, RaveExceptions, Misc
         rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
         # account payload
         payload = {
-          "accountbank": "044",  # get the bank code from the bank list endpoint.
-          "accountnumber": "0690000031",
-          "currency": "NGN",
-          "country": "NG",
-          "amount": "100",
-          "email": "test@test.com",
-          "phonenumber": "0902620185",
-          "IP": "355426087298442",
+           "amount":2,
+           "PBFPubKey":"ENTER_YOUR_PUBLIC_KEY",
+           "currency":"GBP",
+           "email":"user@example.com",
+           "meta":[
+              {
+                 "metaname":"test",
+                 "metavalue":"12383"
+              }
+           ],
+           "ip":"123.0.1.3",
+           "firstname":"Flutterwave",
+           "lastname":"Tester"
         }
         
         try:
             res = rave.Account.charge(payload)
             if res["authUrl"]:
                 print(res["authUrl"])
         
@@ -606,21 +600,20 @@
         ## ```rave.GhMobile```
         This is used to facilitate Ghanaian mobile money transactions.
         
         **Functions included:**
         
         * ```.charge```
         
-        
         * ```.verify```
         
         <br>
         
         ### ```.charge(payload)```
-        This is called to start a Ghana mobile money transaction. The payload should be a dictionary containing account information. It should have the parameters:
+        This is called to start a Ghana mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
         
         * ```amount```,
         
         * ```email```, 
         
         * ```phonenumber```,
         
@@ -640,17 +633,29 @@
         ```
         
         #### Returns
         
         This call returns a dictionary. A sample response is:
         
         ```py
-        {'error': False, 'validationRequired': True, 'txRef': 'MC-1530910216380', 'flwRef': 'N/A'}
+        {
+            "status": "success",
+            "message": "Momo initiated",
+            "data": {
+                "code": "02",
+                "status": "pending",
+                "ts": 1591798138846,
+                "link": "https://ravemodal-dev.herokuapp.com/captcha/verify/123:49fa60c0db04f0017d717a0a662194cd"
+            }
+        }
         ```
         
+        
+        In order to complete the charge, kindly redirect users to the link returned as `data.link` from the charge response.
+        
          This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
         
         ```py
         try: 
             #Your charge call
         except RaveExceptions.TransactionChargeError as e:
             print(e.err["errMsg"])
@@ -873,15 +878,15 @@
         
         
         * ```.verify```
         
         <br>
         
         ### ```.charge(payload)```
-        This is called to start a Ugandan mobile money transaction. The payload should be a dictionary containing account information. It should have the parameters:
+        This is called to start a Ugandan mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
         
         * ```amount```,
         
         * ```email```, 
         
         * ```phonenumber```,
         
@@ -899,17 +904,29 @@
         ```
         
         #### Returns
         
         This call returns a dictionary. A sample response is:
         
         ```py
-        {'error': False, 'status': 'success', 'validationRequired': True, 'txRef': 'MC-1544013787279', 'flwRef': 'flwm3s4m0c1544013788481'}
+        {
+            "status": "success",
+            "message": "Momo initiated",
+            "data": {
+                "code": "02",
+                "status": "pending",
+                "ts": 1591798138846,
+                "link": "https://ravemodal-dev.herokuapp.com/captcha/verify/123:49fa60c0db04f0017d717a0a662194cd"
+            }
+        }
         ```
         
+        
+        In order to complete the charge, kindly redirect users to the link returned as `data.link` from the charge response.
+        
          This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
         
         ```py
         try: 
             #Your charge call
         except RaveExceptions.TransactionChargeError as e:
             print(e.err["errMsg"])
@@ -1003,15 +1020,15 @@
         
         
         * ```.verify```
         
         <br>
         
         ### ```.charge(payload)```
-        This is called to start a Zambian mobile money transaction. The payload should be a dictionary containing account information. It should have the parameters:
+        This is called to start a Zambian mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
         
         * ```amount```,
         
         * ```email```, 
         
         * ```phonenumber```,
         
@@ -1029,17 +1046,28 @@
         ```
         
         #### Returns
         
         This call returns a dictionary. A sample response is:
         
         ```py
-        {'error': False, 'status': 'success', 'validationRequired': True, 'txRef': 'MC-1544013787279', 'flwRef': 'flwm3s4m0c1544013788481'}
+        {
+            "status": "success",
+            "message": "Momo initiated",
+            "data": {
+                "code": "02",
+                "status": "pending",
+                "ts": 1591798138846,
+                "link": "https://ravemodal-dev.herokuapp.com/captcha/verify/123:49fa60c0db04f0017d717a0a662194cd"
+            }
+        }
         ```
         
+        In order to complete the charge, kindly redirect users to the link returned as `data.link` from the charge response.
+        
          This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
         
         ```py
         try: 
             #Your charge call
         except RaveExceptions.TransactionChargeError as e:
             print(e.err["errMsg"])
@@ -1134,15 +1162,15 @@
         
         
         * ```.verify```
         
         <br>
         
         ### ```.charge(payload)```
-        This is called to start a francophone mobile money transaction. The payload should be a dictionary containing account information. It should have the parameters:
+        This is called to start a francophone mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
         
         * ```amount```,
         
         * ```email```, 
         
         * ```phonenumber```,
         
@@ -1232,14 +1260,372 @@
         except RaveExceptions.TransactionVerificationError as e:
           print(e.err["errMsg"])
           print(e.err["txRef"])
         ```
         
         <br><br>
         
+        ## ```rave.TZSMobile```
+        This is used to collect Tanzanian mobile money collections.
+        
+        **Functions included:**
+        
+        * ```.charge```
+        
+        * ```.verify```
+        
+        <br>
+        
+        ### ```.charge(payload)```
+        This is called to start a Tanzanian mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
+        
+        * ```amount```,
+        
+        * ```email```, 
+        
+        * ```phonenumber```,
+        
+        * ```IP``` (optional),
+        
+        * ```redirect_url``` (optional)
+        
+        Optionally, you can add a custom transaction reference using the ```txRef``` parameter. Note that if you do not specify one, it would be automatically generated. We do provide a function for generating transaction references in the [Misc library](https://github.com/Flutterwave/rave-python/blob/master/rave_python/rave_misc.py).
+        
+        
+        A sample call is:
+        
+        ```py
+        res = rave.TZSMobile.charge(payload)
+        ```
+        
+        #### Returns
+        
+        This call returns a dictionary. A sample response is:
+        
+        ```py
+        {}
+        ```
+        
+        
+         This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
+        
+        ```py
+        try: 
+            #Your charge call
+        except RaveExceptions.TransactionChargeError as e:
+            print(e.err["errMsg"])
+            print(e.err["flwRef"])
+        
+        ```
+        
+        A sample ``` e.err ``` contains:
+        
+        ```py
+        {
+           "error":true,
+           "txRef":"MC-1530911537060",
+           "flwRef":None,
+           "errMsg":None
+        }
+        ```
+        
+        
+        <br>
+        
+        ### ```.verify(txRef)```
+        
+        You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned in the ```charge``` call. 
+        
+        A sample verify call is:
+        
+        ```py
+        res = rave.TZSMobile.verify(data["txRef"])
+        ```
+        
+        #### Returns
+        
+        This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
+        
+        If your call could not be completed successfully, a ```TransactionVerificationError``` is raised.
+        
+        
+        ### Complete Tanzania mobile money charge flow
+        
+        ```py
+        from rave_python import Rave, RaveExceptions, Misc
+        rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
+        
+        # mobile payload
+        payload = {
+          "amount": "50",
+          "email": "",
+          "phonenumber": "054709929220",
+          "redirect_url": "https://rave-webhook.herokuapp.com/receivepayment",
+          "IP":""
+        }
+        
+        try:
+          res = rave.TZSMobile.charge(payload)
+          res = rave.TZSMobile.verify(res["txRef"])
+          print(res)
+        
+        except RaveExceptions.TransactionChargeError as e:
+          print(e.err)
+          print(e.err["flwRef"])
+        
+        except RaveExceptions.TransactionVerificationError as e:
+          print(e.err["errMsg"])
+          print(e.err["txRef"])
+        ```
+        
+        <br><br>
+        
+        ## ```rave.BankTransfer```
+        This is used to create a virtual account for a Bank transfer payment.
+        
+        **Functions included:**
+        * ```.charge```
+        * ```.verify```
+        
+        <br>
+        
+        ### ```.charge(payload)```
+        This is called to initiate the Bank transfer payment. The payload should be a dictionary containing payment information. It should have the parameters:
+        
+        * ```amount```,
+        * ```email```,
+        * ```firstname```,
+        * ```lastname```,
+        * ```phonenumber``` (optional),
+        * ```IP``` (optional),
+        * ```redirect_url``` (optional)
+        
+        Optionally, you can add a custom transaction reference using the ```txRef``` parameter. Note that if you do not specify one, it would be automatically generated. We do provide a function for generating transaction references in the [Misc library](https://github.com/Flutterwave/rave-python/blob/master/rave_python/rave_misc.py).
+        
+        
+        A sample call is:
+        
+        ```py
+        res = rave.BankTransfer.charge(payload)
+        ```
+        
+        #### Returns
+        
+        This call returns a dictionary. A sample response is:
+        
+        ```py
+        {
+           "expiresIn":"2023-07-21 13:56:15",
+           "flwRef":"CTNT35701689940575038134",
+           "error":False,
+           "validationRequired":False,
+           "accountNumber":"8526418059",
+           "bankName":"Sterling Bank",
+           "transferNote":"Please make a bank transfer to Flutterwave Developers  FLW",
+           "txRef":"MC-1689940569118"
+        }
+        ```
+        
+        
+         This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
+        
+        ```py
+        try: 
+            #Your charge call
+        except RaveExceptions.TransactionChargeError as e:
+            print(e.err["errMsg"])
+            print(e.err["flwRef"])
+        
+        ```
+        
+        A sample ``` e.err ``` contains:
+        
+        ```py
+        {
+            "error":true,
+           "txRef":"MC-1689940569118",
+           "flwRef":None,
+           "errMsg":None
+        }
+        ```
+        
+        
+        <br>
+        
+        ### ```.verify(txRef)```
+        
+        You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned in the ```charge``` call. 
+        
+        A sample verify call is:
+        
+        ```py
+        res = rave.BankTransfer.verify(data["txRef"])
+        ```
+        
+        #### Returns
+        
+        This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
+        
+        If your call could not be completed successfully, a ```TransactionVerificationError``` is raised.
+        
+        
+        ### Complete Bank Transfer charge flow
+        
+        ```py
+        from rave_python import Rave, RaveExceptions, Misc
+        rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
+        
+        # mobile payload
+        payload = {
+          "amount": "50",
+          "email": "",
+          "phonenumber": "054709929220",
+          "redirect_url": "https://rave-webhook.herokuapp.com/receivepayment",
+          "IP":""
+        }
+        
+        try:
+          res = rave.BankTransfer.charge(payload)
+          res = rave.BankTransfer.verify(res["txRef"])
+          print(res)
+        
+        except RaveExceptions.TransactionChargeError as e:
+          print(e.err)
+          print(e.err["flwRef"])
+        
+        except RaveExceptions.TransactionVerificationError as e:
+          print(e.err["errMsg"])
+          print(e.err["txRef"])
+        ```
+        
+        <br><br>
+        
+        ===
+        ## ```rave.Enaira```
+        This is used to create Enaira wallet payments.
+        
+        **Functions included:**
+        * ```.charge```
+        * ```.verify```
+        
+        <br>
+        
+        ### ```.charge(payload)```
+        This is called to initiate the Enaira payment. The payload should be a dictionary containing payment information. It should have the parameters:
+        
+        * ```amount```,
+        * ```email```,
+        * ```firstname```,
+        * ```lastname```,
+        * ```ìs_token```,
+        * ```phonenumber``` (optional),
+        * ```IP``` (optional),
+        * ```redirect_url``` (optional)
+        
+        Optionally, you can add a custom transaction reference using the ```txRef``` parameter. Note that if you do not specify one, it would be automatically generated. We do provide a function for generating transaction references in the [Misc library](https://github.com/Flutterwave/rave-python/blob/master/rave_python/rave_misc.py).
+        
+        
+        A sample call is:
+        
+        ```py
+        res = rave.Enaira.charge(payload)
+        ```
+        
+        #### Returns
+        This call returns a dictionary. A sample response is:
+        
+        ```py
+        {
+           "txRef":"MC-1689947009435",
+           "error":False,
+           "validationRequired":True,
+           "image":"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAJQAAACUCAYAAAB1PADUAAAAAklEQVR4AewaftIAAAUZSURBVO3BQW4kwZEAQfdE///LvjzGqYBCJ7kaKczsB2tdcljrosNaFx3Wuuiw1kWHtS46rHXRYa2LDmtddFjrosNaFx3Wuuiw1kWHtS46rHXRYa2LPnxJ5S9VvKEyVUwqTyqeqDypeKIyVUwqf6niG4e1LjqsddFhrYs+XFZxk8oTlaniicpU8UTlJpVvVNykctNhrYsOa110WOuiD79M5Y2KNyomlaliUplU3qiYVKaKNyq+ofJGxW86rHXRYa2LDmtd9OF/TMUTlScqU8UTlScqU8W/7LDWRYe1LjqsddGHf5zKE5WpYlKZKiaVqeKJyhsV/00Oa110WOuiw1oXffhlFb+pYlJ5ojJVTCpTxTcqJpVJZap4o+I/yWGtiw5rXXRY66IPl6n8JZWpYlKZKiaVqWJSmSomlaliUpkqJpU3VP6THda66LDWRYe1LjLvuAYxO8DAAAAMklEQVR42mJ89x+CIQjIwMx2mlcDAAZLM2XBEGSJcs1PQwBAHQ6UAA2NhvTwAAAAAElFTkSuQmCC",
+           "validateInstructions":"Please scan the qr image in your eNaira app.",
+           "flwref":"AXOO81561689947011229191"
+        }
+        ```
+        
+        
+         This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
+        
+        ```py
+        try: 
+            #Your charge call
+        except RaveExceptions.TransactionChargeError as e:
+            print(e.err["errMsg"])
+            print(e.err["flwRef"])
+        
+        ```
+        
+        A sample ``` e.err ``` contains:
+        
+        ```py
+        {
+            "error":true,
+           "txRef":"MC-1689940569118",
+           "flwRef":None,
+           "errMsg":None
+        }
+        ```
+        
+        
+        <br>
+        
+        ### ```.verify(txRef)```
+        
+        You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned in the ```charge``` call. 
+        
+        A sample verify call is:
+        
+        ```py
+        res = rave.BankTransfer.verify(data["txRef"])
+        ```
+        
+        #### Returns
+        
+        This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
+        
+        If your call could not be completed successfully, a ```TransactionVerificationError``` is raised.
+        
+        
+        ### Complete Enaira charge flow
+        
+        ```py
+        from rave_python import Rave, RaveExceptions, Misc
+        rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
+        
+        # mobile payload
+        payload = {
+            "amount": 30,
+            "PBFPubKey": "ENTER_YOUR_PUBLIC_KEY",
+            "currency": "NGN",
+            "email": "user@example.com",
+            "meta": [{"metaname": "test", "metavalue": "12383"}],
+            "ip": "123.0.1.3",
+            "firstname": "Flutterwave",
+            "lastname": "Tester",
+            "is_token": False
+        }
+        
+        try:
+          res = rave.Enaira.charge(payload)
+          res = rave.Enaira.verify(res["txRef"])
+          print(res)
+        
+        except RaveExceptions.TransactionChargeError as e:
+          print(e.err)
+          print(e.err["flwRef"])
+        
+        except RaveExceptions.TransactionVerificationError as e:
+          print(e.err["errMsg"])
+          print(e.err["txRef"])
+        ```
+        
+        <br><br>
+        
         ## ```rave.Preauth```
         This is used to facilitate preauthorized card transactions. This inherits the Card class so any task you can do on Card, you can do with preauth.
         
         **Functions included:**
         
         * ```.charge```
         
@@ -1625,14 +2011,18 @@
         
         * ```.all```
         
         * ```.getFee```
         
         * ```.getBalance```
         
+        *```.retryTransfer```
+        
+        *```fetchRetries```
+        
         <br>
         
         ### ```.initiate(transferDetails)```
         
         This initiates a transfer to a customer's account. When a transfer is initiated, it comes with a status NEW this means the transfer has been queued for processing.
         
         **Please note that you must pass ```beneficiary_name``` as part of the initiate call. Else an error will be thrown.**
@@ -1821,16 +2211,53 @@
         This call returns a dictionary. A sample response is:
         
         ```py
         {'error': False, 'returnedData': {'status': 'success', 'message': 'WALLET-BALANCE', 'data': {'Id': 27122, 'ShortName': 'EUR', 'WalletNumber': '3855000502677', 'AvailableBalance': 0, 'LedgerBalance': 0}}}
         ```
         
         
+        ### ```.retryTransfer(transfer_id)```
+        
+        This allows you to retry a previously failed transfer attempt. You are expected to pass the id for the failed transfer into this call (ids can be gotten in data object from the initial transfer response)
+        
+        A sample fetch call is:
+        
+        ```py
+        res2 = rave.retryTransfer.Balance("169680")
+        ```
+        
+        #### Returns
+        
+        This call returns a dictionary. A sample response is:
+        
+        ```py
+        {'error': False, 'returnedData': {'status': 'success', 'message': 'Transfer retry attempt queued.', 'data': {'id': 169681, 'account_number': '0690000044', 'bank_code': '044', 'fullname': 'Mercedes Daniel', 'date_created': '2021-02-19T15:56:57.000Z', 'currency': 'NGN', 'amount': 500, 'fee': 10.75, 'status': 'NEW', 'reference': 'SampleTransfer4_PMCK_ST_FDU_1_RETRY_1', 'meta': None, 'narration': 'Test_Transfer_for_new_features', 'complete_message': '', 'requires_approval': 0, 'is_approved': 1, 'bank_name': 'ACCESS BANK NIGERIA'}}}
+        ```
+        
         <br>
         
+        ### ```.fetchRetries(transfer_id)```
+        
+        This allows you to get all retry attempts for all previously failed transfer attempts.
+        
+        A sample fetch call is:
+        
+        ```py
+        res2 = rave.fetchRetries.Balance("169680")
+        ```
+        
+        #### Returns
+        
+        This call returns a dictionary. A sample response is:
+        
+        ```py
+        {'error': False, 'returnedData': {'status': 'success', 'message': 'Transfer retry attempts retrieved.', 'data': [{'id': 169681, 'account_number': '0690000044', 'bank_code': '044', 'bank_name': 'ACCESS BANK NIGERIA', 'fullname': 'Mercedes Daniel', 'currency': 'NGN', 'debit_currency': None, 'amount': 500, 'fee': 10.75, 'status': 'FAILED', 'reference': 'SampleTransfer4_PMCK_ST_FDU_1_RETRY_1', 'narration': 'Test_Transfer_for_new_features', 'complete_message': 'DISBURSE FAILED: Transfer failed. Please contact support', 'meta': None, 'requires_approval': 0, 'is_approved': 1, 'date_created': '2021-02-19T15:56:57.000Z'}]}}
+        ```
+        
+        
         ### Complete transfer flow
         
         ```py
         from rave_python import Rave, RaveExceptions
         try:
             rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
         
@@ -2703,15 +3130,16 @@
             "Status": "success",
             "Message": "Withdrawal successful",
             "Reference": null
         }
         ```
         <br>
         
-        ## Run Tests
+        
+        ## Testing
         
         All of the SDK's tests are written with Python's ```unittest``` module. The tests currently test:
         ```rave.Account```
         ```rave.Card```
         ```rave.Transfer```
         ```rave.Preauth```
         ```rave.Subaccount```
@@ -2725,16 +3153,41 @@
         ```
         
         >**NOTE:** If the test fails for creating a subaccount, just change the ```account_number``` ```account_bank```  and ```businesss_email``` to something different
         
         >**NOTE:** The test may fail for account validation - ``` Pending OTP validation``` depending on whether the service is down or not
         <br>
         
+        
+        ## Debugging Errors
+        We understand that you may run into some errors while integrating our library. You can read more about our error messages [here](https://developer.flutterwave.com/docs/integration-guides/errors).
+        
+        For `authorization` and `validation` error responses, double-check your API keys and request. If you get a `server` error, kindly engage the team for support.
+        
+        
+        
         ## Support
-        For further assistance in using the SDK, you can contact the Developers on [Slack](https://join.slack.com/t/flutterwavedevelopers/shared_invite/enQtNTk3MjgxMjU3ODI5LWFkMjBkYTc0ZGJhM2Q5MTY3YjFkYzAyYmM1ZDZjZjUwMjE4YTc2NjQ1ZGM5ZWE4NDUxMzc4MmExYmI1Yjg5ZWU) and [Email](mailto:developers@flutterwavego.com). You can get more information about the amazing features here [here](https://developer.flutterwave.com/reference#introduction).
+        For additional assistance using this library, contact the developer experience (DX) team via [email](mailto:developers@flutterwavego.com) or on [slack](https://bit.ly/34Vkzcg). 
+        
+        You can also follow us [@FlutterwaveEng](https://twitter.com/FlutterwaveEng) and let us know what you think 😊.
+        
+        
+        ## Contribution guidelines
+        Read more about our community contribution guidelines [here](/CONTRIBUTING.md)
+        
+        
+        ## License
+        
+        By contributing to this library, you agree that your contributions will be licensed under its [MIT license](/LICENSE).
+        Copyright (c) Flutterwave Inc.
+        
+        ## Test section
+        Sample Description for teset file. 
+        
+        Final test 3 out of 10. Fingers crossed
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rave_python-1.2.9/README.md` & `rave_python-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,69 @@
 <p align="center">
-    <img title="Flutterwave" height="200" src="https://flutterwave.com/images/logo-colored.svg" width="50%"/>
+    <img title="Flutterwave" height="200" src="https://flutterwave.com/images/logo/full.svg" width="50%"/>
 </p>
 
-# Rave Python Library.
+# Flutterwave Python Library.
 ![Upload Python Package](https://github.com/Flutterwave/rave-python/workflows/Upload%20Python%20Package/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/rave_python)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/rave_python)
 ![PyPI - License](https://img.shields.io/pypi/l/rave_python)
 
 
 ## Introduction
-This is a Python wrapper around the [API](https://flutterwavedevelopers.readme.io/v2.0/reference) for [Rave by Flutterwave](https://rave.flutterwave.com).
+The Python library provides easy access to Flutterwave for Business (F4B) v2 APIs from Django, Flask, and other Python apps. It abstracts the complexity involved in direct integration and allows you to make quick calls to the APIs.
+
+Available features include:
+
+- Collections: Card, Account, Mobile money, Bank Transfers, USSD, Barter, NQR.
+- Payouts and Beneficiaries.
+- Recurring payments: Tokenization and Subscriptions.
+- Split payments
+- Card issuing
+- Transactions dispute management: Refunds.
+- Transaction reporting: Collections, Payouts, Settlements, and Refunds.
+- Bill payments: Airtime, Data bundle, Cable, Power, Toll, E-bills, and Remitta.
+- Identity verification: Resolve bank account, resolve BVN information.
+
+## Table of Contents
+1. [Requirements](#requirements)
+2. [Installation](#installation)
+3. [Initialization](#initialization)
+4. [Usage](#usage)
+5. [Testing](#testing)
+6. [Debugging Errors](#debugging-errors)
+7. [Support](#support)
+8. [Contribution guidelines](#)
+9. [License](#)
+10. [Changelog](#)
+
+## Requirements
+1. Flutterwave for business [API Keys](https://developer.flutterwave.com/docs/integration-guides/authentication)
+2. Supported Python versions: >=2.7, !=3.0.\*, !=3.1.\*, !=3.2.\*, !=3.3.\*, !=3.4.\*
 
-#### Payment types implemented:
-* Card Payments
-* Bank Account Payments
-* Ghana Mobile Money Payments
-* Mpesa Payments
-* Rwanda Mobile Money Payments
-* Uganda Mobile Money Payments
-* Zambia Mobile Money Payments
-* Mobile Money Payments for Francophone countries
-* Subaccounts
-* Transfer
-* Subscription (Recurring Payments)
-* Bills payment
-* Payment Plan
-* USSD Payments (Still in Beta Mode)
-
-#### Other features include:
-* Preauthorization charges
-* Refunds
-* Transaction Verification
-* Transfer Recipients
-* Virtual Cards
-* Virtual Accounts
 
 ## Installation
-To install, run
+To install the library, run
 
 ```sh
 pip install rave_python
 ```
 
 Note: This is currently under active development
-## Import Package
+
+
+## Initialization
+
+### Import Package
 The base class for this package is 'Rave'. To use this class, add:
 
 ```py
 from rave_python import Rave
 ```
 
-## Initialization
-
 #### To instantiate in sandbox:
 To use Rave, instantiate the Rave class with your public key. We recommend that you store your secret key in an environment variable named, ```RAVE_SECRET_KEY```. Instantiating your rave object is therefore as simple as:
 
 ```py
 rave = Rave("YOUR_PUBLIC_KEY")
 ```
 
@@ -71,15 +78,17 @@
 #### To instantiate in production:
 To initialize in production, simply set the ```production``` flag to ```True```. It is highly discouraged but if you choose to not use environment variables, you can do so in the same way mentioned above.
 
 ```py
 rave = Rave("YOUR_PUBLIC_KEY", production=True)
 ```
 
-# Rave Objects
+
+
+# Usage
 This is the documentation for all of the components of rave_python
 
 ## ```rave.Card```
 This is used to facilitate card transactions.
 
 **Functions included:**
 
@@ -236,15 +245,15 @@
 This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
 
 Sample
 ```py
 {'flwRef': None, 'cardToken': u'flw-t1nf-5b0f12d565cd961f73c51370b1340f1f-m03k', 'chargedAmount': 100, 'amount': 100, 'transactionComplete': True, 'error': False, 'txRef': u'MC-1538095718251'}
 ```
 
-#### Please note that after charging a card successfully on rave, if you wish to save the card for further charges, in your verify payment response you will find an object: "cardtoken": "flw-t0-f6f915f53a094671d98560272572993e-m03k".  This is the token you will use for card tokenization. Details are provided below.
+> Please note that after charging a card successfully on rave, if you wish to save the card for further charges, in your verify payment response you will find an object: `"cardtoken": "flw-t0-f6f915f53a094671d98560272572993e-m03k"`.  This is the token you will use for card tokenization. Details are provided below.
 
 If your call could not be completed successfully, a ```TransactionVerificationError``` is raised.
 
 <br>
 
 ### ```.charge(payload_for_saved_card, chargeWithToken=True)```
 This is called to start a card transaction with a card that has been saved. The payload should be a dictionary containing card information. It should have the parameters:
@@ -391,40 +400,33 @@
 except RaveExceptions.TransactionVerificationError as e:
     print(e.err["errMsg"])
     print(e.err["txRef"])
 ```
 
 <br><br>
 ## ```rave.Account```
-This is used to facilitate account transactions.
+This is used to facilitate account transactions. Transactions initiated via this method are authorized by the user on their Banking platform.
 
 **Functions included:**
 
 * ```.charge```
-
-* ```.validate```
-
 * ```.verify```
 
 <br>
 
 ### ```.charge(payload)```
-This is called to start an account transaction. The payload should be a dictionary containing card information. It should have the parameters:
-
-* ```accountbank```, 
-
-* ```accountnumber```, 
-
-* ```amount```, 
+This is called to start an account transaction. The payload should be a dictionary containing payment information. It should have the parameters:
 
+* ```amount``` (The min amount for NGN account payments is N200. For GBP and EUR payments, the min amount is 1), 
+* ```currency``` (This payment option supports NGN, GBP and EUR),  
 * ```email```, 
-
-* ```phonenumber```, 
-
-* ```IP```
+* ```firstname```, 
+* ```lastname```, 
+* ```IP``` (optional)
+* ```redirectUrl``` (optional)
 
 Optionally, you can add a custom transaction reference using the ```txRef``` parameter. Note that if you do not specify one, it would be automatically generated. We do provide a function for generating transaction references in the [Misc library](https://github.com/Flutterwave/rave-python/blob/master/rave_python/rave_misc.py).
 
 
 A sample call is:
 
 ```py
@@ -432,15 +434,22 @@
 ```
 
 #### Returns
 
 This call returns a dictionary. A sample response is:
 
 ```py
- {'error': False, 'validationRequired': True, 'txRef': 'MC-1530899106006', 'flwRef': 'ACHG-1530899109682', 'authUrl': None}
+# sample response for NGN account payments
+ {
+   "validationRequired":True,
+   "authUrl":"https://api.ravepay.co/flwv3-pug/getpaid/api/short-url/vHWOLuy89",
+   "flwRef":"XINH44931689941420152189",
+   "txRef":"MC-1689941418883",
+   "error":False
+}
 ```
 
  This call raises an ```AccountChargeError``` if there was a problem processing your transaction. The ```AccountChargeError``` contains some information about your transaction. You can handle this as such:
 
 ```py
 try: 
     #Your charge call
@@ -453,77 +462,57 @@
 
 ```py
 {'error': True, 'txRef': 'MC-1530897824739', 'flwRef': None, 'errMsg': 'Sorry, that account number is invalid, please check and try again'}
 ```
 
 <br>
 
-### ```.validate(txRef)```
-
-After a successful charge, most times you will be asked to verify with OTP. To check if this is required, check the ```validationRequired``` key in the ```res``` of the charge call.
-
-In the case that an ```authUrl``` is returned from your charge call, you may skip the validation step and simply pass your authUrl to the end-user. 
-
-```py
-authUrl = res['authUrl']
-```
-
-To validate, you need to pass the ```flwRef``` from the ```res``` of the charge call as well as the OTP.
-
-A sample validate call is: 
-
-```py
-res2 = rave.Account.validate(res["flwRef"], "12345")
-```
-
-
-#### Returns
-
-This call returns a dictionary containing the ```txRef```, ```flwRef``` among others if successful.
-
-This call raises a ```TransactionValidationError``` if the OTP is not correct or there was a problem processing your request. 
-
-To handle this, write:
-
-```py
-try:
-    # Your charge call
-except RaveExceptions.TransactionValidationError as e:
-    print(e.err["errMsg"])
-    print(e.err["flwRef"])
-```
-
-A sample ``` e.err ``` contains:
-
-```py
-{'error': True, 'txRef': 'MC-1530899869968', 'flwRef': 'ACHG-1530899873118', 'errMsg': 'Pending OTP validation'}
-```
-
-
-
-<br>
-
 ### ```.verify(txRef)```
 
-You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned any of the calls (```charge``` or ```validate```). 
+You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned any the ```charge```call. 
 
 A sample verify call is:
 
 ```py
 res = rave.Account.verify(data["txRef"])
 ```
 
 #### Returns
 
 This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
 
 Sample
 
 ```py
-{'status': u'success', 'vbvcode': u'N/A', 'chargedamount': 500, 'vbvmessage': u'N/A', 'error': False, 'flwRef': u'ACHG-1538093023787', 'currency': u'NGN', 'amount': 500, 'transactionComplete': True, 'acctmessage': u'Approved Or Completed Successfully', 'chargecode': u'00', 'txRef': u'MC-1538093008498'}
+{
+   "status":"success",
+   "vbvcode":"57",
+   "chargemessage":"Pending validation",
+   "chargedamount":200,
+   "vbvmessage":"transaction was abandoned",
+   "error":True,
+   "flwRef":"XINH44931689941420152189",
+   "currency":"NGN",
+   "amount":200,
+   "meta":[
+      {
+         "getpaidTransactionId":984928641,
+         "metavalue":"12383",
+         "metaname":"test",
+         "updatedAt":"2023-07-21T12:10:19.000Z",
+         "deletedAt":"None",
+         "id":2168360293,
+         "createdAt":"2023-07-21T12:10:19.000Z"
+      }
+   ],
+   "transactionComplete":False,
+   "acctmessage":None,
+   "chargecode":"02",
+   "txRef":"MC-1689941418883"
+}
 ```
 
 If your call could not be completed successfully or if a wrong ```txRef``` is passed, a ```TransactionVerificationError``` is raised. You can handle that as such
 ```py
 try: 
     #Your charge call
 except RaveExceptions.TransactionVerificationError as e:
@@ -556,22 +545,27 @@
 ### Complete account flow
 
 ```py
 from rave_python import Rave, RaveExceptions, Misc
 rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
 # account payload
 payload = {
-  "accountbank": "044",  # get the bank code from the bank list endpoint.
-  "accountnumber": "0690000031",
-  "currency": "NGN",
-  "country": "NG",
-  "amount": "100",
-  "email": "test@test.com",
-  "phonenumber": "0902620185",
-  "IP": "355426087298442",
+   "amount":2,
+   "PBFPubKey":"ENTER_YOUR_PUBLIC_KEY",
+   "currency":"GBP",
+   "email":"user@example.com",
+   "meta":[
+      {
+         "metaname":"test",
+         "metavalue":"12383"
+      }
+   ],
+   "ip":"123.0.1.3",
+   "firstname":"Flutterwave",
+   "lastname":"Tester"
 }
 
 try:
     res = rave.Account.charge(payload)
     if res["authUrl"]:
         print(res["authUrl"])
 
@@ -598,21 +592,20 @@
 ## ```rave.GhMobile```
 This is used to facilitate Ghanaian mobile money transactions.
 
 **Functions included:**
 
 * ```.charge```
 
-
 * ```.verify```
 
 <br>
 
 ### ```.charge(payload)```
-This is called to start a Ghana mobile money transaction. The payload should be a dictionary containing account information. It should have the parameters:
+This is called to start a Ghana mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
 
 * ```amount```,
 
 * ```email```, 
 
 * ```phonenumber```,
 
@@ -632,17 +625,29 @@
 ```
 
 #### Returns
 
 This call returns a dictionary. A sample response is:
 
 ```py
-{'error': False, 'validationRequired': True, 'txRef': 'MC-1530910216380', 'flwRef': 'N/A'}
+{
+    "status": "success",
+    "message": "Momo initiated",
+    "data": {
+        "code": "02",
+        "status": "pending",
+        "ts": 1591798138846,
+        "link": "https://ravemodal-dev.herokuapp.com/captcha/verify/123:49fa60c0db04f0017d717a0a662194cd"
+    }
+}
 ```
 
+
+In order to complete the charge, kindly redirect users to the link returned as `data.link` from the charge response.
+
  This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
 
 ```py
 try: 
     #Your charge call
 except RaveExceptions.TransactionChargeError as e:
     print(e.err["errMsg"])
@@ -865,15 +870,15 @@
 
 
 * ```.verify```
 
 <br>
 
 ### ```.charge(payload)```
-This is called to start a Ugandan mobile money transaction. The payload should be a dictionary containing account information. It should have the parameters:
+This is called to start a Ugandan mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
 
 * ```amount```,
 
 * ```email```, 
 
 * ```phonenumber```,
 
@@ -891,17 +896,29 @@
 ```
 
 #### Returns
 
 This call returns a dictionary. A sample response is:
 
 ```py
-{'error': False, 'status': 'success', 'validationRequired': True, 'txRef': 'MC-1544013787279', 'flwRef': 'flwm3s4m0c1544013788481'}
+{
+    "status": "success",
+    "message": "Momo initiated",
+    "data": {
+        "code": "02",
+        "status": "pending",
+        "ts": 1591798138846,
+        "link": "https://ravemodal-dev.herokuapp.com/captcha/verify/123:49fa60c0db04f0017d717a0a662194cd"
+    }
+}
 ```
 
+
+In order to complete the charge, kindly redirect users to the link returned as `data.link` from the charge response.
+
  This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
 
 ```py
 try: 
     #Your charge call
 except RaveExceptions.TransactionChargeError as e:
     print(e.err["errMsg"])
@@ -995,15 +1012,15 @@
 
 
 * ```.verify```
 
 <br>
 
 ### ```.charge(payload)```
-This is called to start a Zambian mobile money transaction. The payload should be a dictionary containing account information. It should have the parameters:
+This is called to start a Zambian mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
 
 * ```amount```,
 
 * ```email```, 
 
 * ```phonenumber```,
 
@@ -1021,17 +1038,28 @@
 ```
 
 #### Returns
 
 This call returns a dictionary. A sample response is:
 
 ```py
-{'error': False, 'status': 'success', 'validationRequired': True, 'txRef': 'MC-1544013787279', 'flwRef': 'flwm3s4m0c1544013788481'}
+{
+    "status": "success",
+    "message": "Momo initiated",
+    "data": {
+        "code": "02",
+        "status": "pending",
+        "ts": 1591798138846,
+        "link": "https://ravemodal-dev.herokuapp.com/captcha/verify/123:49fa60c0db04f0017d717a0a662194cd"
+    }
+}
 ```
 
+In order to complete the charge, kindly redirect users to the link returned as `data.link` from the charge response.
+
  This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
 
 ```py
 try: 
     #Your charge call
 except RaveExceptions.TransactionChargeError as e:
     print(e.err["errMsg"])
@@ -1126,15 +1154,15 @@
 
 
 * ```.verify```
 
 <br>
 
 ### ```.charge(payload)```
-This is called to start a francophone mobile money transaction. The payload should be a dictionary containing account information. It should have the parameters:
+This is called to start a francophone mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
 
 * ```amount```,
 
 * ```email```, 
 
 * ```phonenumber```,
 
@@ -1224,14 +1252,372 @@
 except RaveExceptions.TransactionVerificationError as e:
   print(e.err["errMsg"])
   print(e.err["txRef"])
 ```
 
 <br><br>
 
+## ```rave.TZSMobile```
+This is used to collect Tanzanian mobile money collections.
+
+**Functions included:**
+
+* ```.charge```
+
+* ```.verify```
+
+<br>
+
+### ```.charge(payload)```
+This is called to start a Tanzanian mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
+
+* ```amount```,
+
+* ```email```, 
+
+* ```phonenumber```,
+
+* ```IP``` (optional),
+
+* ```redirect_url``` (optional)
+
+Optionally, you can add a custom transaction reference using the ```txRef``` parameter. Note that if you do not specify one, it would be automatically generated. We do provide a function for generating transaction references in the [Misc library](https://github.com/Flutterwave/rave-python/blob/master/rave_python/rave_misc.py).
+
+
+A sample call is:
+
+```py
+res = rave.TZSMobile.charge(payload)
+```
+
+#### Returns
+
+This call returns a dictionary. A sample response is:
+
+```py
+{}
+```
+
+
+ This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
+
+```py
+try: 
+    #Your charge call
+except RaveExceptions.TransactionChargeError as e:
+    print(e.err["errMsg"])
+    print(e.err["flwRef"])
+
+```
+
+A sample ``` e.err ``` contains:
+
+```py
+{
+   "error":true,
+   "txRef":"MC-1530911537060",
+   "flwRef":None,
+   "errMsg":None
+}
+```
+
+
+<br>
+
+### ```.verify(txRef)```
+
+You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned in the ```charge``` call. 
+
+A sample verify call is:
+
+```py
+res = rave.TZSMobile.verify(data["txRef"])
+```
+
+#### Returns
+
+This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
+
+If your call could not be completed successfully, a ```TransactionVerificationError``` is raised.
+
+
+### Complete Tanzania mobile money charge flow
+
+```py
+from rave_python import Rave, RaveExceptions, Misc
+rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
+
+# mobile payload
+payload = {
+  "amount": "50",
+  "email": "",
+  "phonenumber": "054709929220",
+  "redirect_url": "https://rave-webhook.herokuapp.com/receivepayment",
+  "IP":""
+}
+
+try:
+  res = rave.TZSMobile.charge(payload)
+  res = rave.TZSMobile.verify(res["txRef"])
+  print(res)
+
+except RaveExceptions.TransactionChargeError as e:
+  print(e.err)
+  print(e.err["flwRef"])
+
+except RaveExceptions.TransactionVerificationError as e:
+  print(e.err["errMsg"])
+  print(e.err["txRef"])
+```
+
+<br><br>
+
+## ```rave.BankTransfer```
+This is used to create a virtual account for a Bank transfer payment.
+
+**Functions included:**
+* ```.charge```
+* ```.verify```
+
+<br>
+
+### ```.charge(payload)```
+This is called to initiate the Bank transfer payment. The payload should be a dictionary containing payment information. It should have the parameters:
+
+* ```amount```,
+* ```email```,
+* ```firstname```,
+* ```lastname```,
+* ```phonenumber``` (optional),
+* ```IP``` (optional),
+* ```redirect_url``` (optional)
+
+Optionally, you can add a custom transaction reference using the ```txRef``` parameter. Note that if you do not specify one, it would be automatically generated. We do provide a function for generating transaction references in the [Misc library](https://github.com/Flutterwave/rave-python/blob/master/rave_python/rave_misc.py).
+
+
+A sample call is:
+
+```py
+res = rave.BankTransfer.charge(payload)
+```
+
+#### Returns
+
+This call returns a dictionary. A sample response is:
+
+```py
+{
+   "expiresIn":"2023-07-21 13:56:15",
+   "flwRef":"CTNT35701689940575038134",
+   "error":False,
+   "validationRequired":False,
+   "accountNumber":"8526418059",
+   "bankName":"Sterling Bank",
+   "transferNote":"Please make a bank transfer to Flutterwave Developers  FLW",
+   "txRef":"MC-1689940569118"
+}
+```
+
+
+ This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
+
+```py
+try: 
+    #Your charge call
+except RaveExceptions.TransactionChargeError as e:
+    print(e.err["errMsg"])
+    print(e.err["flwRef"])
+
+```
+
+A sample ``` e.err ``` contains:
+
+```py
+{
+    "error":true,
+   "txRef":"MC-1689940569118",
+   "flwRef":None,
+   "errMsg":None
+}
+```
+
+
+<br>
+
+### ```.verify(txRef)```
+
+You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned in the ```charge``` call. 
+
+A sample verify call is:
+
+```py
+res = rave.BankTransfer.verify(data["txRef"])
+```
+
+#### Returns
+
+This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
+
+If your call could not be completed successfully, a ```TransactionVerificationError``` is raised.
+
+
+### Complete Bank Transfer charge flow
+
+```py
+from rave_python import Rave, RaveExceptions, Misc
+rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
+
+# mobile payload
+payload = {
+  "amount": "50",
+  "email": "",
+  "phonenumber": "054709929220",
+  "redirect_url": "https://rave-webhook.herokuapp.com/receivepayment",
+  "IP":""
+}
+
+try:
+  res = rave.BankTransfer.charge(payload)
+  res = rave.BankTransfer.verify(res["txRef"])
+  print(res)
+
+except RaveExceptions.TransactionChargeError as e:
+  print(e.err)
+  print(e.err["flwRef"])
+
+except RaveExceptions.TransactionVerificationError as e:
+  print(e.err["errMsg"])
+  print(e.err["txRef"])
+```
+
+<br><br>
+
+===
+## ```rave.Enaira```
+This is used to create Enaira wallet payments.
+
+**Functions included:**
+* ```.charge```
+* ```.verify```
+
+<br>
+
+### ```.charge(payload)```
+This is called to initiate the Enaira payment. The payload should be a dictionary containing payment information. It should have the parameters:
+
+* ```amount```,
+* ```email```,
+* ```firstname```,
+* ```lastname```,
+* ```ìs_token```,
+* ```phonenumber``` (optional),
+* ```IP``` (optional),
+* ```redirect_url``` (optional)
+
+Optionally, you can add a custom transaction reference using the ```txRef``` parameter. Note that if you do not specify one, it would be automatically generated. We do provide a function for generating transaction references in the [Misc library](https://github.com/Flutterwave/rave-python/blob/master/rave_python/rave_misc.py).
+
+
+A sample call is:
+
+```py
+res = rave.Enaira.charge(payload)
+```
+
+#### Returns
+This call returns a dictionary. A sample response is:
+
+```py
+{
+   "txRef":"MC-1689947009435",
+   "error":False,
+   "validationRequired":True,
+   "image":"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAJQAAACUCAYAAAB1PADUAAAAAklEQVR4AewaftIAAAUZSURBVO3BQW4kwZEAQfdE///LvjzGqYBCJ7kaKczsB2tdcljrosNaFx3Wuuiw1kWHtS46rHXRYa2LDmtddFjrosNaFx3Wuuiw1kWHtS46rHXRYa2LPnxJ5S9VvKEyVUwqTyqeqDypeKIyVUwqf6niG4e1LjqsddFhrYs+XFZxk8oTlaniicpU8UTlJpVvVNykctNhrYsOa110WOuiD79M5Y2KNyomlaliUplU3qiYVKaKNyq+ofJGxW86rHXRYa2LDmtd9OF/TMUTlScqU8UTlScqU8W/7LDWRYe1LjqsddGHf5zKE5WpYlKZKiaVqeKJyhsV/00Oa110WOuiw1oXffhlFb+pYlJ5ojJVTCpTxTcqJpVJZap4o+I/yWGtiw5rXXRY66IPl6n8JZWpYlKZKiaVqWJSmSomlaliUpkqJpU3VP6THda66LDWRYe1LjLvuAYxO8DAAAAMklEQVR42mJ89x+CIQjIwMx2mlcDAAZLM2XBEGSJcs1PQwBAHQ6UAA2NhvTwAAAAAElFTkSuQmCC",
+   "validateInstructions":"Please scan the qr image in your eNaira app.",
+   "flwref":"AXOO81561689947011229191"
+}
+```
+
+
+ This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
+
+```py
+try: 
+    #Your charge call
+except RaveExceptions.TransactionChargeError as e:
+    print(e.err["errMsg"])
+    print(e.err["flwRef"])
+
+```
+
+A sample ``` e.err ``` contains:
+
+```py
+{
+    "error":true,
+   "txRef":"MC-1689940569118",
+   "flwRef":None,
+   "errMsg":None
+}
+```
+
+
+<br>
+
+### ```.verify(txRef)```
+
+You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned in the ```charge``` call. 
+
+A sample verify call is:
+
+```py
+res = rave.BankTransfer.verify(data["txRef"])
+```
+
+#### Returns
+
+This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
+
+If your call could not be completed successfully, a ```TransactionVerificationError``` is raised.
+
+
+### Complete Enaira charge flow
+
+```py
+from rave_python import Rave, RaveExceptions, Misc
+rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
+
+# mobile payload
+payload = {
+    "amount": 30,
+    "PBFPubKey": "ENTER_YOUR_PUBLIC_KEY",
+    "currency": "NGN",
+    "email": "user@example.com",
+    "meta": [{"metaname": "test", "metavalue": "12383"}],
+    "ip": "123.0.1.3",
+    "firstname": "Flutterwave",
+    "lastname": "Tester",
+    "is_token": False
+}
+
+try:
+  res = rave.Enaira.charge(payload)
+  res = rave.Enaira.verify(res["txRef"])
+  print(res)
+
+except RaveExceptions.TransactionChargeError as e:
+  print(e.err)
+  print(e.err["flwRef"])
+
+except RaveExceptions.TransactionVerificationError as e:
+  print(e.err["errMsg"])
+  print(e.err["txRef"])
+```
+
+<br><br>
+
 ## ```rave.Preauth```
 This is used to facilitate preauthorized card transactions. This inherits the Card class so any task you can do on Card, you can do with preauth.
 
 **Functions included:**
 
 * ```.charge```
 
@@ -1617,14 +2003,18 @@
 
 * ```.all```
 
 * ```.getFee```
 
 * ```.getBalance```
 
+*```.retryTransfer```
+
+*```fetchRetries```
+
 <br>
 
 ### ```.initiate(transferDetails)```
 
 This initiates a transfer to a customer's account. When a transfer is initiated, it comes with a status NEW this means the transfer has been queued for processing.
 
 **Please note that you must pass ```beneficiary_name``` as part of the initiate call. Else an error will be thrown.**
@@ -1813,16 +2203,53 @@
 This call returns a dictionary. A sample response is:
 
 ```py
 {'error': False, 'returnedData': {'status': 'success', 'message': 'WALLET-BALANCE', 'data': {'Id': 27122, 'ShortName': 'EUR', 'WalletNumber': '3855000502677', 'AvailableBalance': 0, 'LedgerBalance': 0}}}
 ```
 
 
+### ```.retryTransfer(transfer_id)```
+
+This allows you to retry a previously failed transfer attempt. You are expected to pass the id for the failed transfer into this call (ids can be gotten in data object from the initial transfer response)
+
+A sample fetch call is:
+
+```py
+res2 = rave.retryTransfer.Balance("169680")
+```
+
+#### Returns
+
+This call returns a dictionary. A sample response is:
+
+```py
+{'error': False, 'returnedData': {'status': 'success', 'message': 'Transfer retry attempt queued.', 'data': {'id': 169681, 'account_number': '0690000044', 'bank_code': '044', 'fullname': 'Mercedes Daniel', 'date_created': '2021-02-19T15:56:57.000Z', 'currency': 'NGN', 'amount': 500, 'fee': 10.75, 'status': 'NEW', 'reference': 'SampleTransfer4_PMCK_ST_FDU_1_RETRY_1', 'meta': None, 'narration': 'Test_Transfer_for_new_features', 'complete_message': '', 'requires_approval': 0, 'is_approved': 1, 'bank_name': 'ACCESS BANK NIGERIA'}}}
+```
+
 <br>
 
+### ```.fetchRetries(transfer_id)```
+
+This allows you to get all retry attempts for all previously failed transfer attempts.
+
+A sample fetch call is:
+
+```py
+res2 = rave.fetchRetries.Balance("169680")
+```
+
+#### Returns
+
+This call returns a dictionary. A sample response is:
+
+```py
+{'error': False, 'returnedData': {'status': 'success', 'message': 'Transfer retry attempts retrieved.', 'data': [{'id': 169681, 'account_number': '0690000044', 'bank_code': '044', 'bank_name': 'ACCESS BANK NIGERIA', 'fullname': 'Mercedes Daniel', 'currency': 'NGN', 'debit_currency': None, 'amount': 500, 'fee': 10.75, 'status': 'FAILED', 'reference': 'SampleTransfer4_PMCK_ST_FDU_1_RETRY_1', 'narration': 'Test_Transfer_for_new_features', 'complete_message': 'DISBURSE FAILED: Transfer failed. Please contact support', 'meta': None, 'requires_approval': 0, 'is_approved': 1, 'date_created': '2021-02-19T15:56:57.000Z'}]}}
+```
+
+
 ### Complete transfer flow
 
 ```py
 from rave_python import Rave, RaveExceptions
 try:
     rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
 
@@ -2695,15 +3122,16 @@
     "Status": "success",
     "Message": "Withdrawal successful",
     "Reference": null
 }
 ```
 <br>
 
-## Run Tests
+
+## Testing
 
 All of the SDK's tests are written with Python's ```unittest``` module. The tests currently test:
 ```rave.Account```
 ```rave.Card```
 ```rave.Transfer```
 ```rave.Preauth```
 ```rave.Subaccount```
@@ -2717,9 +3145,34 @@
 ```
 
 >**NOTE:** If the test fails for creating a subaccount, just change the ```account_number``` ```account_bank```  and ```businesss_email``` to something different
 
 >**NOTE:** The test may fail for account validation - ``` Pending OTP validation``` depending on whether the service is down or not
 <br>
 
+
+## Debugging Errors
+We understand that you may run into some errors while integrating our library. You can read more about our error messages [here](https://developer.flutterwave.com/docs/integration-guides/errors).
+
+For `authorization` and `validation` error responses, double-check your API keys and request. If you get a `server` error, kindly engage the team for support.
+
+
+
 ## Support
-For further assistance in using the SDK, you can contact the Developers on [Slack](https://join.slack.com/t/flutterwavedevelopers/shared_invite/enQtNTk3MjgxMjU3ODI5LWFkMjBkYTc0ZGJhM2Q5MTY3YjFkYzAyYmM1ZDZjZjUwMjE4YTc2NjQ1ZGM5ZWE4NDUxMzc4MmExYmI1Yjg5ZWU) and [Email](mailto:developers@flutterwavego.com). You can get more information about the amazing features here [here](https://developer.flutterwave.com/reference#introduction).
+For additional assistance using this library, contact the developer experience (DX) team via [email](mailto:developers@flutterwavego.com) or on [slack](https://bit.ly/34Vkzcg). 
+
+You can also follow us [@FlutterwaveEng](https://twitter.com/FlutterwaveEng) and let us know what you think 😊.
+
+
+## Contribution guidelines
+Read more about our community contribution guidelines [here](/CONTRIBUTING.md)
+
+
+## License
+
+By contributing to this library, you agree that your contributions will be licensed under its [MIT license](/LICENSE).
+Copyright (c) Flutterwave Inc.
+
+## Test section
+Sample Description for teset file. 
+
+Final test 3 out of 10. Fingers crossed
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rave_python-1.2.9/rave_python/rave.py` & `rave_python-1.4.0/rave_python/rave.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,42 +16,68 @@
 from rave_python.rave_transfer import Transfer
 from rave_python.rave_ugmobile import UGMobile
 from rave_python.rave_ussd import Ussd
 from rave_python.rave_verify import Verify
 from rave_python.rave_virtualaccount import VirtualAccount
 from rave_python.rave_virtualcard import VirtualCard
 from rave_python.rave_zbmobile import ZBMobile
+from rave_python.rave_banktransfer import BankTransfer
+from rave_python.rave_enaira import Enaira
+from rave_python.rave_tzmobile import TZSMobile
 
 
 class Rave:
-    
+
     def __init__(self, publicKey, secretKey, production=False, usingEnv=True):
         """ This is main organizing object. It contains the following:\n
             rave.Account -- For bank account transactions\n
+            rave.BankTransfer -- For pay with bank transfer transaction\n
             rave.Bills -- For Bills payments\n
             rave.Card -- For card transactions\n
+            rave.Enaira -- For enaira wallet payments\n
             rave.Francophone -- For West African Francophone mobile money transactions\n
             rave.GhMobile -- For Ghana mobile money transactions\n
             rave.Mpesa -- For mpesa transactions\n
             rave.PaymentPlan -- For payment plan creation and operation\n
             rave.Preauth -- For preauthorized transactions\n
             rave.RWMobile -- For Rwanda mobile money transactions\n
             rave.Settlement -- For settled transactions\n
             rave.SubAccount -- For creation of subaccounts for split payment operations\n
+            rave.TZSMobile -- For Tanzania mobile money transactions\n
             rave.Transfer -- For Payouts and transfers\n
             rave.UGMobile -- For Uganda mobile money transactions\n
             rave.Ussd -- For ussd transactions\n
             rave.VirtualAccount -- For virtual account transactions\n
-            rave.VirtualCard -- For virtual card transactions\n 
+            rave.VirtualCard -- For virtual card transactions\n
             rave.ZBMobile -- For Zambia mobile money transactions\n
-            
+
         """
 
         classes = (
-            Account, Bills, Card, Ebills, Francophone, GhMobile, Mpesa, PaymentPlan, Preauth, Recipient, RWMobile, Settlement, SubAccount, Subscriptions, Transfer, UGMobile, Ussd, Verify, VirtualAccount, VirtualCard, ZBMobile
-        )
+            Account,
+            BankTransfer,
+            Bills,
+            Card,
+            Ebills,
+            Enaira,
+            Francophone,
+            GhMobile,
+            Mpesa,
+            PaymentPlan,
+            Preauth,
+            Recipient,
+            RWMobile,
+            Settlement,
+            SubAccount,
+            Subscriptions,
+            Transfer,
+            TZSMobile,
+            UGMobile,
+            Ussd,
+            Verify,
+            VirtualAccount,
+            VirtualCard,
+            ZBMobile)
 
         for _class in classes:
             attr = _class(publicKey, secretKey, production, usingEnv)
             setattr(self, _class.__name__, attr)
-        
-
```

### Comparing `rave_python-1.2.9/rave_python/rave_account.py` & `rave_python-1.4.0/rave_python/rave_enaira.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,91 @@
+from rave_python.rave_payment import Payment
 from rave_python.rave_exceptions import AccountChargeError
 from rave_python.rave_misc import generateTransactionReference
-from rave_python.rave_payment import Payment
-
 
-class Account(Payment):
-    """ This is the rave object for account transactions. It contains the following public functions:\n
-        .charge -- This is for making an account charge\n
-        .validate -- This is called if further action is required i.e. OTP validation\n
+class Enaira(Payment):
+    """ This is the rave object for eNaira wallet transactions. It contains the following public functions:\n
+        .charge -- This is for charging the eNaira wallet\n
         .verify -- This checks the status of your transaction\n
+        .refunds -- This initiates the refund for the transaction\n
     """
+
     def _handleChargeResponse(self, response, txRef, request=None):
         """ This handles account charge responses """
         # This checks if we can parse the json successfully
-        res =  self._preliminaryResponseChecks(response, AccountChargeError, txRef=txRef)
+        res = self._preliminaryResponseChecks(
+            response, AccountChargeError, txRef=txRef)
 
         response_json = res['json']
         # change - added data before flwRef
         response_data = response_json['data']
         flw_ref = response_data['flwRef']
 
-        # If all preliminary checks are passed
         data = {
             'error': False,
             'validationRequired': True,
             'txRef': txRef,
-            'flwRef': flw_ref,
-            'authUrl': None,
+            'flwref': flw_ref
         }
-        if response_data.get("chargeResponseCode") != "00":
-            # If contains authurl
-            data['authUrl'] = response_data.get("authurl")  # None by default
+        
+        if 'qr_image' in response_data:
+            data.update({
+                'validateInstructions': "Please scan the qr image in your eNaira app.",
+                'image': response_data['qr_image']
+                })
         else:
-            data['validateInstructions'] = response_data['validateInstructions']
-        return data
+            data.update({
+                'validateInstructions': response_data['validate_instructions'],
+                'image': None
+                })
 
+        # If all preliminary checks are passed
+        return data
+    
     # Charge account function
     def charge(self, accountDetails, hasFailed=False):
         """ This is the direct account charge call.\n
              Parameters include:\n
             accountDetails (dict) -- These are the parameters passed to the function for processing\n
             hasFailed (boolean) -- This is a flag to determine if the attempt had previously failed due to a timeout\n
         """
 
         # setting the endpoint
         endpoint = self._baseUrl + self._endpointMap['account']['charge']
-        feature_name = "Initiate-Account-charge"
+        feature_name = "eNaira Payments"
 
-        # It is faster to just update rather than check if it is already present
-        accountDetails.update({'payment_type': 'account'})
+        # It is faster to just update rather than check if it is already
+        # present
+
+        if accountDetails.get("is_token") == True:
+            accountDetails.update({'payment_type': 'enaira', 'is_token': True, 'country': 'NG'})
+        else:
+            accountDetails.update({'payment_type': 'enaira', 'is_qr': True, 'country': 'NG'})
 
         # Generate transaction reference if txRef doesn't exist
         accountDetails.setdefault('txRef', generateTransactionReference())
 
         # Checking for required account components
-        requiredParameters = ['accountbank', 'accountnumber', 'amount', 'email', 'phonenumber', 'IP']
+        requiredParameters = [
+            'amount',
+            'email',
+            'firstname',
+            'lastname'
+            ]
 
-        return super().charge(feature_name, accountDetails, requiredParameters, endpoint)
+        return super(Enaira, self).charge(feature_name, accountDetails, requiredParameters, endpoint)
 
     def validate(self, flwRef, otp):
         endpoint = self._baseUrl + self._endpointMap['account']['validate']
         feature_name = "Account-charge-validate"
         return super().validate(feature_name, flwRef, endpoint)
-
+    
     def verify(self, txRef):
         endpoint = self._baseUrl + self._endpointMap['account']['verify']
-        feature_name = "Account-charge-verify"
-        return super().verify(feature_name, txRef, endpoint)
+        feature_name = "Verify eNaira"
+        return super(Enaira, self).verify(feature_name, txRef, endpoint)
 
     def refund(self, flwRef, amount):
-        feature_name = "Account-charge-refund"
+        feature_name = "Refund eNaira"
         endpoint = self._baseUrl + self._endpointMap["account"]["refund"]
-        return super().refund(feature_name, flwRef, amount)
+        return super(Enaira, self).refund(feature_name, flwRef, amount)
+
```

### Comparing `rave_python-1.2.9/rave_python/rave_base.py` & `rave_python-1.4.0/rave_python/rave_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,35 @@
-import os, hashlib, warnings, requests, json
+import os
+import hashlib
+import warnings
+import requests
+import json
 from rave_python.rave_exceptions import ServerError, RefundError
 import base64
 from Crypto.Cipher import DES3
+
+
 class RaveBase(object):
     """ This is the core of the implementation. It contains the encryption and initialization functions. It also contains all direct rave functions that require publicKey or secretKey (refund) """
-    def __init__(self, publicKey=None, secretKey=None, production=False, usingEnv=True):
+
+    def __init__(
+            self,
+            publicKey=None,
+            secretKey=None,
+            production=False,
+            usingEnv=True):
 
         # config variables (protected)
-        self._baseUrlMap = ["https://ravesandboxapi.flutterwave.com/", "https://api.ravepay.co/"]
+        self._baseUrlMap = [
+            "https://ravesandboxapi.flutterwave.com/",
+            "https://api.ravepay.co/"]
         self._trackingMap = "https://kgelfdz7mf.execute-api.us-east-1.amazonaws.com/staging/sendevent"
         self._endpointMap = {
             "bills": {
-                "create":"v2/services/confluence",
+                "create": "v2/services/confluence",
             },
             "bvn": {
                 "verify": "v2/kyc/bvn/",
             },
             "card": {
                 "charge": "flwv3-pug/getpaidx/api/charge",
                 "validate": "flwv3-pug/getpaidx/api/validatecharge",
@@ -39,21 +53,21 @@
                 "refund": "gpx/merchant/transactions/refund"
             },
             "payment_plan": {
                 "create": "v2/gpx/paymentplans/create",
                 "fetch": "v2/gpx/paymentplans/query",
                 "list": "v2/gpx/paymentplans/query",
                 "cancel": "v2/gpx/paymentplans/",
-                "edit" :  "v2/gpx/paymentplans/"
+                "edit": "v2/gpx/paymentplans/"
             },
             "subscriptions": {
                 "fetch": "v2/gpx/subscriptions/query",
                 "list": "v2/gpx/subscriptions/query",
                 "cancel": "v2/gpx/subscriptions/",
-                "activate" : "v2/gpx/subscriptions/"
+                "activate": "v2/gpx/subscriptions/"
             },
             "settlements": {
                 "list": "v2/merchant/settlements",
                 "fetch": "v2/merchant/settlements/",
             },
             "subaccount": {
                 "create": "v2/gpx/subaccounts/create",
@@ -64,17 +78,19 @@
             },
             "transfer": {
                 "initiate": "v2/gpx/transfers/create",
                 "bulk": "v2/gpx/transfers/create_bulk",
                 "fetch": "v2/gpx/transfers",
                 "fee": "v2/gpx/transfers/fee",
                 "balance": "v2/gpx/balance",
-                "accountVerification": "flwv3-pug/getpaidx/api/resolve_account"
+                "accountVerification": "flwv3-pug/getpaidx/api/resolve_account",
+                "retry": "v2/gpx/transfers/retry",
+                "inter_wallet": "v2/gpx/transfers/wallet"
             },
-            "recipient":{
+            "recipient": {
                 "create": "v2/gpx/transfers/beneficiaries/create",
                 "list": "v2/gpx/transfers/beneficiaries",
                 "fetch": "v2/gpx/transfers/beneficiaries",
                 "delete": "v2/gpx/transfers/beneficiaries/delete",
             },
             "virtual_card": {
                 "create": "v2/services/virtualcards/new",
@@ -83,91 +99,88 @@
                 "terminate": "v2/services/virtualcards/",
                 "fund": "v2/services/virtualcards/fund",
                 "transactions": "v2/services/virtualcards/",
                 "withdraw": "v2/services/virtualcards/withdraw",
                 "freeze": "v2/services/virtualcards/",
                 "unfreeze": "v2/services/virtualcards/",
             },
-            "virtual_account":{
-                "create" : "v2/banktransfers/accountnumbers",
+            "virtual_account": {
+                "create": "v2/banktransfers/accountnumbers",
             },
             "verify": "flwv3-pug/getpaidx/api/v2/verify",
             "refund": "gpx/merchant/transactions/refund"
-            
+
         }
-        
 
         # Setting up public and private keys (private)
         # If we are using environment variables to store secretKey
-        if(usingEnv):  
+        if (usingEnv):
             self.__publicKey = publicKey
             self.__secretKey = os.getenv("RAVE_SECRET_KEY", None)
 
             if (not self.__publicKey) or (not self.__secretKey):
-                raise ValueError("Please set your RAVE_SECRET_KEY environment variable. Otherwise, pass publicKey and secretKey as arguments and set usingEnv to false")
+                raise ValueError(
+                    "Please set your RAVE_SECRET_KEY environment variable. Otherwise, pass publicKey and secretKey as arguments and set usingEnv to false")
 
         # If we are not using environment variables
         else:
             if (not publicKey) or (not secretKey):
                 raise ValueError("\n Please provide as arguments your publicKey and secretKey. \n It is advised however that you provide secret key as an environment variables. \n To do this, remove the usingEnv flag and save your keys as environment variables, RAVE_PUBLIC_KEY and RAVE_SECRET_KEY")
-    
+
             else:
                 self.__publicKey = publicKey
                 self.__secretKey = secretKey
 
                 # Raise warning about not using environment variables
-                warnings.warn("Though you can use the usingEnv flag to pass secretKey as an argument, it is advised to store it in an environment variable, especially in production.", SyntaxWarning)
+                warnings.warn(
+                    "Though you can use the usingEnv flag to pass secretKey as an argument, it is advised to store it in an environment variable, especially in production.",
+                    SyntaxWarning)
 
         # Setting instance variables
-        # 
+        #
         # production/non-production variables (protected)
-        self._isProduction = production 
+        self._isProduction = production
         self._baseUrl = self._baseUrlMap[production]
 
         # encryption key (protected)
         self._encryptionKey = self.__getEncryptionKey()
 
-    
-
     # This generates the encryption key (private)
+
     def __getEncryptionKey(self):
         """ This generates the encryption key """
-        if(self.__secretKey):
-            hashedseckey = hashlib.md5(self.__secretKey.encode("utf-8")).hexdigest()
+        if (self.__secretKey):
+            hashedseckey = hashlib.md5(
+                self.__secretKey.encode("utf-8")).hexdigest()
             hashedseckeylast12 = hashedseckey[-12:]
             seckeyadjusted = self.__secretKey.replace('FLWSECK-', '')
             seckeyadjustedfirst12 = seckeyadjusted[:12]
             key = seckeyadjustedfirst12 + hashedseckeylast12
             return key
 
         raise ValueError("Please initialize RavePay")
-    
+
     # This returns the public key
     def _getPublicKey(self):
         return self.__publicKey
-    
+
     # This returns the secret key
     def _getSecretKey(self):
         return self.__secretKey
 
     # This encrypts text
     def _encrypt(self, plainText):
         """ This is the encryption function.\n
-             Parameters include:\n 
+             Parameters include:\n
             plainText (string) -- This is the text you wish to encrypt
         """
         blockSize = 8
         padDiff = blockSize - (len(plainText) % blockSize)
         key = self.__getEncryptionKey()
         cipher = DES3.new(key, DES3.MODE_ECB)
         plainText = "{}{}".format(plainText, "".join(chr(padDiff) * padDiff))
-        # cipher.encrypt - the C function that powers this doesn't accept plain string, rather it accepts byte strings, hence the need for the conversion below
+        # cipher.encrypt - the C function that powers this doesn't accept plain
+        # string, rather it accepts byte strings, hence the need for the
+        # conversion below
         test = plainText.encode('utf-8')
         encrypted = base64.b64encode(cipher.encrypt(test)).decode("utf-8")
         return encrypted
-        
-
-
-
-
-
-
```

### Comparing `rave_python-1.2.9/rave_python/rave_bills.py` & `rave_python-1.4.0/rave_python/rave_bills.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,102 @@
-import json, requests, copy
+import json
+import requests
+import copy
 from rave_python.rave_base import RaveBase
 from rave_python.rave_misc import checkIfParametersAreComplete
 from rave_python.rave_exceptions import ServerError, IncompleteCardDetailsError, BillCreationError, BillStatusError
 
+
 class Bills(RaveBase):
     def __init__(self, publicKey, secretKey, production, usingEnv):
         self.headers = {
-            'content-type' : 'application/json'
+            'content-type': 'application/json'
         }
         super(Bills, self).__init__(publicKey, secretKey, production, usingEnv)
 
     def _preliminaryResponseChecks(self, response, TypeOfErrorToRaise, name):
-        #check if we can get json
+        # check if we can get json
         try:
             responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "name": name, "errMsg": response})
+        except BaseException:
+            raise ServerError(
+                {"error": True, "name": name, "errMsg": response})
 
-        #check for data parameter in response 
+        # check for data parameter in response
         if not responseJson.get("data", None):
-            raise TypeOfErrorToRaise({"error": True, "name": name, "errMsg": responseJson.get("message", "Server is down")})
+            raise TypeOfErrorToRaise({"error": True,
+                                      "name": name,
+                                      "errMsg": responseJson.get("message",
+                                                                 "Server is down")})
 
-        #check for 200 response
+        # check for 200 response
         if not response.ok:
             errMsg = response["data"].get("message", None)
             raise TypeOfErrorToRaise({"error": True, "errMsg": errMsg})
 
         return responseJson
 
     def _handleCreateResponse(self, response, details):
-        responseJson = self._preliminaryResponseChecks(response, BillCreationError, details["service"])
+        responseJson = self._preliminaryResponseChecks(
+            response, BillCreationError, details["service"])
 
         if responseJson["status"] == "success":
-            return {"error": False, "id": responseJson["data"].get("id", None), "data": responseJson["data"] }
+            return {
+                "error": False,
+                "id": responseJson["data"].get(
+                    "id",
+                    None),
+                "data": responseJson["data"]}
 
         else:
-            raise BillCreationError({"error": True, "data": responseJson["data"]})
+            raise BillCreationError(
+                {"error": True, "data": responseJson["data"]})
 
+    # function to create a Bill
+    # Params: details - a dict containing service, service_method,
+    # service_version, service_channel and service_payload
 
-    #function to create a Bill
-    #Params: details - a dict containing service, service_method, service_version, service_channel and service_payload
     def create(self, details):
-        
-        # Performing shallow copy of planDetails to avoid public exposing payload with secret key
+
+        # Performing shallow copy of planDetails to avoid public exposing
+        # payload with secret key
         details = copy.copy(details)
         details.update({"seckey": self._getSecretKey()})
-        requiredParameters = ["service", "service_method", "service_version", "service_channel"]
+        requiredParameters = [
+            "service",
+            "service_method",
+            "service_version",
+            "service_channel"]
         checkIfParametersAreComplete(requiredParameters, details)
         endpoint = self._baseUrl + self._endpointMap["bills"]["create"]
-        response = requests.post(endpoint, headers=self.headers, data=json.dumps(details))
+        response = requests.post(
+            endpoint,
+            headers=self.headers,
+            data=json.dumps(details))
 
         # feature logging
-        if response.ok == False:
+        if not response.ok:
             tracking_endpoint = self._trackingMap
             responseTime = response.elapsed.total_seconds()
             tracking_payload = {
                 "publicKey": self._getPublicKey(),
-                "language": "Python v2", 
-                "version": "1.2.9", 
-                "title": "Create-Bills-error", 
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": "Create-Bills-error",
                 "message": responseTime
-                }
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
+            }
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
         else:
             tracking_endpoint = self._trackingMap
             responseTime = response.elapsed.total_seconds()
             tracking_payload = {
                 "publicKey": self._getPublicKey(),
-                "language": "Python v2", 
-                "version": "1.2.9", 
-                "title": "Create-Bills", 
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": "Create-Bills",
                 "message": responseTime
-                }
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
+            }
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
 
         return self._handleCreateResponse(response, details)
```

### Comparing `rave_python-1.2.9/rave_python/rave_card.py` & `rave_python-1.4.0/rave_python/rave_card.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,198 @@
 from rave_python.rave_exceptions import RaveError, IncompletePaymentDetailsError, CardChargeError, TransactionVerificationError, ServerError
 from rave_python.rave_payment import Payment
 from rave_python.rave_misc import generateTransactionReference
 
+
 class Card(Payment):
     """ This is the rave object for card transactions. It contains the following public functions:\n
         .charge -- This is for making a card charge\n
         .validate -- This is called if further action is required i.e. OTP validation\n
         .verify -- This checks the status of your transaction\n
     """
+
     def __init__(self, publicKey, secretKey, production, usingEnv):
         super(Card, self).__init__(publicKey, secretKey, production, usingEnv)
 
+    # returns true if further action is required, false if it isn't
 
-    # returns true if further action is required, false if it isn't    
     def _handleChargeResponse(self, response, txRef, request=None):
         """ This handles charge responses """
-        res =  self._preliminaryResponseChecks(response, CardChargeError, txRef=txRef)
+        res = self._preliminaryResponseChecks(
+            response, CardChargeError, txRef=txRef)
 
         responseJson = res["json"]
         flwRef = res["flwRef"]
 
         # Checking if there is auth url
         if responseJson["data"].get("authurl", "N/A") == "N/A":
             authUrl = None
         else:
             authUrl = responseJson["data"]["authurl"]
 
         # If all preliminary checks passed
         if not (responseJson["data"].get("chargeResponseCode", None) == "00"):
-            # Otherwise we return that further action is required, along with the response
+            # Otherwise we return that further action is required, along with
+            # the response
             suggestedAuth = responseJson["data"].get("suggested_auth", None)
-            return {"error": False,  "validationRequired": True, "txRef": txRef, "flwRef": flwRef, "suggestedAuth": suggestedAuth, "authUrl": authUrl}
+            return {
+                "error": False,
+                "validationRequired": True,
+                "txRef": txRef,
+                "flwRef": flwRef,
+                "suggestedAuth": suggestedAuth,
+                "authUrl": authUrl}
         else:
-            return {"error": False, "status": responseJson["status"],  "validationRequired": False, "txRef": txRef, "flwRef": flwRef, "suggestedAuth": None, "authUrl": authUrl}
+            return {
+                "error": False,
+                "status": responseJson["status"],
+                "validationRequired": False,
+                "txRef": txRef,
+                "flwRef": flwRef,
+                "suggestedAuth": None,
+                "authUrl": authUrl}
 
-    
     def _handleRefundorVoidResponse(self, response, txRef, request=None):
         """ This handles charge responses """
-        res =  self._preliminaryResponseChecks(response, CardChargeError, txRef=txRef)
+        res = self._preliminaryResponseChecks(
+            response, CardChargeError, txRef=txRef)
 
         responseJson = res["json"]
         flwRef = responseJson["data"]["data"]["authorizeId"]
 
         # If all preliminary checks passed
-        if not (responseJson["data"]["data"].get("responsecode", None) == "RR"):
+        if not (
+            responseJson["data"]["data"].get(
+                "responsecode",
+                None) == "RR"):
             # Refund or Void could not be completed
-            return {"error": True, "status": responseJson["status"], "message": responseJson["message"], "flwRef": flwRef}
+            return {
+                "error": True,
+                "status": responseJson["status"],
+                "message": responseJson["message"],
+                "flwRef": flwRef}
         else:
-            return {"error": False, "status": responseJson["status"], "message": responseJson["message"], "flwRef": flwRef}
-
-    
+            return {
+                "error": False,
+                "status": responseJson["status"],
+                "message": responseJson["message"],
+                "flwRef": flwRef}
 
     # This can be altered by implementing classes but this is the default behaviour
     # Returns True and the data if successful
+
     def _handleVerifyResponse(self, response, txRef):
         """ This handles all responses from the verify call.\n
              Parameters include:\n
             response (dict) -- This is the response Http object returned from the verify call
          """
 
-        # Checking if there was a server error during the call (in this case html is returned instead of json)
-        res =  self._preliminaryResponseChecks(response, TransactionVerificationError, txRef=txRef)
+        # Checking if there was a server error during the call (in this case
+        # html is returned instead of json)
+        res = self._preliminaryResponseChecks(
+            response, TransactionVerificationError, txRef=txRef)
         responseJson = res["json"]
 
         flwRef = responseJson["data"]["flwref"]
         amount = responseJson["data"]["amount"]
         chargedamount = responseJson["data"]["chargedamount"]
         cardToken = responseJson["data"]["card"]["card_tokens"][0]["embedtoken"]
         vbvmessage = responseJson["data"]["vbvmessage"]
         chargemessage = responseJson["data"]["chargemessage"]
         chargecode = responseJson["data"]["chargecode"]
         currency = responseJson["data"]["currency"]
- 
+        meta = responseJson["data"]["meta"]
+
         # Check if the call returned something other than a 200
         if not response.ok:
-            errMsg = responseJson["data"].get("message", "Your call failed with no response")
-            raise TransactionVerificationError({"error": True, "txRef": txRef, "flwRef": flwRef, "errMsg": errMsg})
-        
+            errMsg = responseJson["data"].get(
+                "message", "Your call failed with no response")
+            raise TransactionVerificationError(
+                {"error": True, "txRef": txRef, "flwRef": flwRef, "errMsg": errMsg})
+
         # if the chargecode is not 00
         elif not (responseJson["data"].get("chargecode", None) == "00"):
-            return {"error": False, "transactionComplete": False, "txRef": txRef, "flwRef":flwRef, "amount": amount, "chargedamount": chargedamount, "cardToken": cardToken, "vbvmessage": vbvmessage, "chargemessage": chargemessage, "chargecode": chargecode, "currency": currency}
-        
+            return {
+                "error": False,
+                "transactionComplete": False,
+                "txRef": txRef,
+                "flwRef": flwRef,
+                "amount": amount,
+                "chargedamount": chargedamount,
+                "cardToken": cardToken,
+                "vbvmessage": vbvmessage,
+                "chargemessage": chargemessage,
+                "chargecode": chargecode,
+                "currency": currency,
+                "meta": meta}
+
         else:
-            return {"error":False, "transactionComplete": True, "txRef": txRef, "flwRef": flwRef, "amount": amount, "chargedamount": chargedamount, "cardToken": cardToken, "vbvmessage": vbvmessage, "chargemessage": chargemessage, "chargecode": chargecode, "currency": currency}
+            return {
+                "error": False,
+                "transactionComplete": True,
+                "txRef": txRef,
+                "flwRef": flwRef,
+                "amount": amount,
+                "chargedamount": chargedamount,
+                "cardToken": cardToken,
+                "vbvmessage": vbvmessage,
+                "chargemessage": chargemessage,
+                "chargecode": chargecode,
+                "currency": currency,
+                "meta": meta}
 
-    
     # Charge card function
+
     def charge(self, cardDetails, hasFailed=False, chargeWithToken=False):
         """ This is called to initiate the charge process.\n
              Parameters include:\n
             cardDetails (dict) -- This is a dictionary comprising payload parameters.\n
             hasFailed (bool) -- This indicates whether the request had previously failed for timeout handling
         """
         # setting the endpoint
         feature_name = "Initiate-Card-charge"
         if not chargeWithToken:
             endpoint = self._baseUrl + self._endpointMap["card"]["charge"]
-            requiredParameters = ["cardno", "cvv", "expirymonth", "expiryyear", "amount", "email"]
+            requiredParameters = [
+                "cardno",
+                "cvv",
+                "expirymonth",
+                "expiryyear",
+                "amount",
+                "email"]
             # optionalParameters = ["phonenumber", "firstname", "lastname"]
-        else: 
+        else:
             if "charge_type" in cardDetails and cardDetails["charge_type"] == 'preauth':
-                endpoint = self._baseUrl + self._endpointMap["preauth"]["charge"]
-            else: 
-                endpoint = self._baseUrl + self._endpointMap["card"]["chargeSavedCard"]
-
-            requiredParameters = ["currency", "token", "country", "amount", "email", "txRef"]
+                endpoint = self._baseUrl + \
+                    self._endpointMap["preauth"]["charge"]
+            else:
+                endpoint = self._baseUrl + \
+                    self._endpointMap["card"]["chargeSavedCard"]
+
+            requiredParameters = [
+                "currency",
+                "token",
+                "country",
+                "amount",
+                "email",
+                "txRef"]
             # optionalParameters = ["firstname", "lastname"]
             # add token to requiredParameters
             # requiredParameters.append("token")
 
         if not ("txRef" in cardDetails):
-            cardDetails.update({"txRef":generateTransactionReference()})
+            cardDetails.update({"txRef": generateTransactionReference()})
 
-        return super(Card, self).charge(feature_name, cardDetails, requiredParameters, endpoint)
-    
+        return super(
+            Card,
+            self).charge(
+            feature_name,
+            cardDetails,
+            requiredParameters,
+            endpoint)
 
     def validate(self, flwRef, otp):
         feature_name = "Validate-Card-charge"
         endpoint = self._baseUrl + self._endpointMap["card"]["validate"]
         return super(Card, self).validate(feature_name, flwRef, otp, endpoint)
 
     def verify(self, txRef):
@@ -125,7 +200,8 @@
         endpoint = self._baseUrl + self._endpointMap["card"]["verify"]
         return super(Card, self).verify(feature_name, txRef, endpoint)
 
     def refund(self, flwRef, amount):
         feature_name = "Card-refund"
         endpoint = self._baseUrl + self._endpointMap["card"]["refund"]
         return super(Card, self).refund(feature_name, flwRef, amount)
+
```

### Comparing `rave_python-1.2.9/rave_python/rave_ebills.py` & `rave_python-1.4.0/rave_python/rave_verify.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,110 @@
-import json, requests, copy
+import json
+import requests
+import copy
 from rave_python.rave_base import RaveBase
 from rave_python.rave_misc import checkIfParametersAreComplete
-from rave_python.rave_exceptions import ServerError, IncompleteCardDetailsError, BillCreationError, BillStatusError
+from rave_python.rave_exceptions import ServerError, BVNFetchError
 
-class Ebills(RaveBase):
+
+class Verify(RaveBase):
     def __init__(self, publicKey, secretKey, production, usingEnv):
-        self.headers = {
-            'content-type' : 'application/json'
-        }
-        super(Ebills, self).__init__(publicKey, secretKey, production, usingEnv)
+        super(
+            Verify,
+            self).__init__(
+            publicKey,
+            secretKey,
+            production,
+            usingEnv)
 
     def _preliminaryResponseChecks(self, response, TypeOfErrorToRaise, name):
-        #check if we can get json
+        # check if we can get json
         try:
             responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "name": name, "errMsg": response})
+        except BaseException:
+            raise ServerError(
+                {"error": True, "name": name, "errMsg": response})
 
-        #check for data parameter in response 
+        # check for data parameter in response
         if not responseJson.get("data", None):
-            raise TypeOfErrorToRaise({"error": True, "name": name, "errMsg": responseJson.get("message", "Server is down")})
+            raise TypeOfErrorToRaise({"error": True,
+                                      "name": name,
+                                      "errMsg": responseJson.get("message",
+                                                                 "Server is down")})
 
-        #check for 200 response
+        # check for 200 response
         if not response.ok:
             errMsg = response["data"].get("message", None)
             raise TypeOfErrorToRaise({"error": True, "errMsg": errMsg})
 
         return responseJson
 
-    def _handleCreateResponse(self, response, details):
-        responseJson = self._preliminaryResponseChecks(response, BillCreationError, details["SECKEY"])
-
-        if responseJson["status"] == "success":
-            return {"error": False, "id": responseJson["data"].get("id", None), "data": responseJson["data"] }
-
-        else:
-            raise BillCreationError({"error": True, "data": responseJson["data"]})
+    # def _handleCreateResponse(self, response, details):
+    #     responseJson = self._preliminaryResponseChecks(response, CardCreationError, details["billing_name"])
 
-    def _handleBillStatusRequests(self, type, endpoint, isPostRequest=False, data=None):
-        #check if resposnse is a post response
+    #     if responseJson["status"] == "success":
+    # return {"error": False, "id": responseJson["data"].get("id", None),
+    # "data": responseJson["data"] }
+
+    #     else:
+    #         raise CardCreationError({"error": True, "data": responseJson["data"]})
+
+    def _handleVerifyStatusRequests(
+            self,
+            endpoint,
+            feature_name,
+            isPostRequest=False,
+            data=None):
+        self.headers = {
+            'content-type': 'application/json'
+        }
+        # check if resposnse is a post response
         if isPostRequest:
-            response = requests.post(endpoint, headers=self.headers, data=json.dumps(data))
+            response = requests.post(
+                endpoint,
+                headers=self.headers,
+                data=json.dumps(data))
         else:
             response = requests.get(endpoint, headers=self.headers)
-        
-        #check if it can be parsed to JSON
+
+        # check if it can be parsed to JSON
         try:
             responseJson = response.json()
-        except:
+        except BaseException:
             raise ServerError({"error": True, "errMsg": response.text})
 
         if response.ok:
+            # feature logging
+            tracking_endpoint = self._trackingMap
+            responseTime = response.elapsed.total_seconds()
+            tracking_payload = {
+                "publicKey": self._getPublicKey(),
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": feature_name,
+                "message": responseTime}
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
             return {"error": False, "returnedData": responseJson}
         else:
-            raise BillStatusError(type, {"error": True, "returnedData": responseJson })
-
-    
-    # def createOrder(self, order_details):
-    #     # Performing shallow copy of planDetails to avoid public exposing payload with secret key
-    #     order_details = copy.copy(order_details)
-    #     order_details.update({"seckey": self._getSecretKey()})
-
-    #     requiredParameters = ["seckey", "numberofunits", "currency", "amount", "email", "txRef", "country"]
-    #     checkIfParametersAreComplete(requiredParameters, order_details)
-
-    #     endpoint = self._baseUrl + self._endpointMap["ebills"]["create"]
-    #     response = requests.post(endpoint, headers=self.headers, data=json.dumps(order_details))
-    #     return self._handleCreateResponse(response, order_details)
-
-    def create(self, details):
-        # Performing shallow copy of planDetails to avoid public exposing payload with secret key
-        details = copy.copy(details)
-        details.update({"SECKEY": self._getSecretKey()})
-
-        requiredParameters = ["numberofunits", "currency", "amount", "email", "txRef", "country"]
-        checkIfParametersAreComplete(requiredParameters, details)
-
-        endpoint = self._baseUrl + self._endpointMap["ebills"]["create"]
-        response = requests.post(endpoint, headers=self.headers, data=json.dumps(details))
-        return self._handleCreateResponse(response, details)
+            tracking_endpoint = self._trackingMap
+            responseTime = response.elapsed.total_seconds()
+            tracking_payload = {
+                "publicKey": self._getPublicKey(),
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": feature_name + "-error",
+                "message": responseTime}
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
+
+            raise BVNFetchError({"error": True, "returnedData": responseJson})
+
+    def bvnVerify(self, bvn):
+
+        # feature logic
+        if not bvn:
+            return "BVN was not supplied. Kindly supply one"
+        feature_name = "BVN-verification"
+        endpoint = self._baseUrl + \
+            self._endpointMap["bvn"]["verify"] + str(bvn) + "?seckey=" + self._getSecretKey()
+        return self._handleVerifyStatusRequests(endpoint, feature_name)
```

### Comparing `rave_python-1.2.9/rave_python/rave_exceptions.py` & `rave_python-1.4.0/rave_python/rave_exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,230 +1,306 @@
 class RaveError(Exception):
     def __init__(self, msg):
         """ This is an error pertaining to the usage of one of the functions in Rave """
         super(RaveError, self).__init__(msg)
         pass
 
+
 class AccountChargeError(RaveError):
     """ Raised when account charge has failed """
+
     def __init__(self, err):
         self.err = err
+
     def __str__(self):
-        return "Your account charge call failed with message: "+self.err["errMsg"]
+        return "Your account charge call failed with message: " + \
+            self.err["errMsg"]
+
 
 class AccountCreationError(RaveError):
     """ Raised when creating a virtual account fails """
+
     def __init__(self, err):
         self.err = err
-    
-    def  __str__(self):
-        return "Virtual account creation failed with error: " +self.err["errMsg"]
+
+    def __str__(self):
+        return "Virtual account creation failed with error: " + \
+            self.err["errMsg"]
+
 
 class AccountStatusError(RaveError):
     """Raised when fetching a Virtual account status"""
+
     def __init__(self, type, err):
         self.err = err
         self.type = type
 
     def __str__(self):
-        return self.type +"ing account failed with error: " + self.err["errMsg"]
+        return self.type + "ing account failed with error: " + \
+            self.err["errMsg"]
+
 
 class AuthMethodNotSupportedError(RaveError):
     """ Raised when user requests for an auth method not currently supported by rave-python """
+
     def __init__(self, message):
-        msg = "\n We do not currently support authMethod: \""+str(message)+"\". If you need this to be supported, please report in GitHub issues page"
+        msg = "\n We do not currently support authMethod: \"" + \
+            str(message) + "\". If you need this to be supported, please report in GitHub issues page"
         super(AuthMethodNotSupportedError, self).__init__(msg)
 
+
 class BillCreationError(RaveError):
     """ Raised when creating a Bill fails """
+
     def __init__(self, err):
         self.err = err
-    
-    def  __str__(self):
-        return "Bill creation failed with error: " +self.err["errMsg"]
+
+    def __str__(self):
+        return "Bill creation failed with error: " + self.err["errMsg"]
+
 
 class BillStatusError(RaveError):
     """Raised when fetching a Bill status"""
+
     def __init__(self, type, err):
         self.err = err
         self.type = type
 
     def __str__(self):
-        return self.type +"ing bill failed with error: " + self.err["errMsg"]
+        return self.type + "ing bill failed with error: " + self.err["errMsg"]
+
 
 class BVNFetchError(RaveError):
     """ Raised when fetching bvn fails """
+
     def __init__(self, err):
         self.err = err
-    
+
     def __str__(self):
         return "BVN fetch failed with error: " + self.err["errMsg"]
 
+
 class CardCreationError(RaveError):
     """ Raised when creating a virtual card fails """
+
     def __init__(self, err):
         self.err = err
-    
-    def  __str__(self):
-        return "Virtual Card creation failed with error: " +self.err["errMsg"]
+
+    def __str__(self):
+        return "Virtual Card creation failed with error: " + self.err["errMsg"]
+
 
 class CardChargeError(RaveError):
     """ Raised when card charge has failed """
+
     def __init__(self, err):
         self.err = err
+
     def __str__(self):
-        return "Your card charge call failed with message: "+self.err["errMsg"]
+        return "Your card charge call failed with message: " + \
+            self.err["errMsg"]
+
 
 class CardStatusError(RaveError):
     """Raised when fetching a Virtual Card status"""
+
     def __init__(self, type, err):
         self.err = err
         self.type = type
 
     def __str__(self):
-        return self.type +"ing card failed with error: " + self.err["errMsg"]
+        return self.type + "ing card failed with error: " + self.err["errMsg"]
+
 
 class InitiateTransferError(RaveError):
     """ Raised when transfer initiation fails """
+
     def __init__(self, err):
         self.err = err
-    
+
     def __str__(self):
         return "Transfer initiation failed with error: " + self.err["errMsg"]
 
+
 class IncompleteAccountDetailsError(RaveError):
     """ Raised when details for card creation are incomplete"""
+
     def __init__(self, value, requiredParameters):
-        msg = "\n\""+value+"\" was not defined in your dictionary. Please ensure you have supplied the following in the payload: \n "+' \n '.join(requiredParameters)
+        msg = "\n\"" + value + "\" was not defined in your dictionary. Please ensure you have supplied the following in the payload: \n " + \
+            ' \n '.join(requiredParameters)
         super(IncompleteAccountDetailsError, self).__init__(msg)
 
+
 class IncompleteCardDetailsError(RaveError):
     """ Raised when details for card creation are incomplete"""
+
     def __init__(self, value, requiredParameters):
-        msg = "\n\""+value+"\" was not defined in your dictionary. Please ensure you have supplied the following in the payload: \n "+' \n '.join(requiredParameters)
+        msg = "\n\"" + value + "\" was not defined in your dictionary. Please ensure you have supplied the following in the payload: \n " + \
+            ' \n '.join(requiredParameters)
         super(IncompleteCardDetailsError, self).__init__(msg)
 
+
 class IncompletePaymentDetailsError(RaveError):
     """ Raised when card details are incomplete """
+
     def __init__(self, value, requiredParameters):
-        msg =  "\n\""+value+"\" was not defined in your dictionary. Please ensure you have supplied the following in the payload: \n "+'  \n '.join(requiredParameters)
+        msg = "\n\"" + value + "\" was not defined in your dictionary. Please ensure you have supplied the following in the payload: \n " + \
+            '  \n '.join(requiredParameters)
         super(IncompletePaymentDetailsError, self).__init__(msg)
 
 
 class MobileChargeError(RaveError):
     """ Raised when mobile money charge has failed """
+
     def __init__(self, err):
         self.err = err
 
     def __str__(self):
-        return "Your mobile money charge call failed with message: "+self.err["errMsg"]
+        return "Your mobile money charge call failed with message: " + \
+            self.err["errMsg"]
+
 
 class PlanCreationError(RaveError):
     """ Raised when creating a payment plan fails """
+
     def __init__(self, err):
         self.err = err
 
     def __str__(self):
-        return "Plan Creation failed with error: " +self.err["errMsg"]
+        return "Plan Creation failed with error: " + self.err["errMsg"]
+
 
 class PlanStatusError(RaveError):
     """ Raised when fetching plan fails """
+
     def __init__(self, type, err):
         self.err = err
         self.type = type
-    
+
     def __str__(self):
-        return self.type +"ing plan failed with error: " + self.err["errMsg"]
+        return self.type + "ing plan failed with error: " + self.err["errMsg"]
+
 
 class PreauthCaptureError(RaveError):
     """ Raised when capturing a preauthorized transaction could not be completed """
+
     def __init__(self, err):
         self.err = err
-        
+
     def __str__(self):
-        return "Your preauth capture call failed with message: "+self.err["errMsg"]
+        return "Your preauth capture call failed with message: " + \
+            self.err["errMsg"]
+
 
 class PreauthRefundVoidError(RaveError):
     """ Raised when capturing a preauthorized refund/void transaction could not be completed """
+
     def __init__(self, err):
         self.err = err
-        
+
     def __str__(self):
-        return "Your preauth refund/void call failed with message: "+self.err["errMsg"]
+        return "Your preauth refund/void call failed with message: " + \
+            self.err["errMsg"]
+
 
 class RecipientCreationError(RaveError):
     """ Raised when creating a transfer recepient fails """
+
     def __init__(self, err):
         self.err = err
 
     def __str__(self):
-        return "Recepient Creation failed with error: " +self.err["errMsg"]
+        return "Recepient Creation failed with error: " + self.err["errMsg"]
+
 
 class RecipientStatusError(RaveError):
     """ Raised when fetching transfer recepients fails """
+
     def __init__(self, type, err):
         self.err = err
         self.type = type
-    
+
     def __str__(self):
-        return self.type +"ing recepient failed with error: " + self.err["errMsg"]
+        return self.type + "ing recepient failed with error: " + \
+            self.err["errMsg"]
+
 
 class RefundError(RaveError):
     """ Raised when refund fails """
+
     def __init__(self, message):
-        msg = "Your refund call failed with message: "+str(message)
+        msg = "Your refund call failed with message: " + str(message)
         super(RefundError, self).__init__(msg)
 
+
 class ServerError(RaveError):
     """ Raised when the server is down or when it could not process your request """
+
     def __init__(self, err):
         self.err = err
-        
+
     def __str__(self):
         return " Server is down with error: " + self.err["errMsg"]
 
+
 class SubaccountCreationError(RaveError):
     """ Raised when creating a payment plan fails """
+
     def __init__(self, err):
         self.err = err
 
     def __str__(self):
-        return "Subaccount Creation failed with error: " +self.err["errMsg"]
+        return "Subaccount Creation failed with error: " + self.err["errMsg"]
+
 
 class TransactionChargeError(RaveError):
     """ Raised when a transaction charge has failed """
+
     def __init__(self, err):
         self.err = err
+
     def __str__(self):
-        return "Your account charge call failed with message: "+self.err["errMsg"]
+        return "Your account charge call failed with message: " + \
+            self.err["errMsg"]
+
 
 class TransferFetchError(RaveError):
     """ Raised when fetching transfer fails """
+
     def __init__(self, err):
         self.err = err
-    
+
     def __str__(self):
         return "Transfer fetch failed with error: " + self.err["errMsg"]
 
+
 class TransactionValidationError(RaveError):
     """ Raised when validation (usually otp validation) fails """
+
     def __init__(self, err):
         self.err = err
 
     def __str__(self):
-        return "Your transaction validation call failed with message: "+self.err["errMsg"]
+        return "Your transaction validation call failed with message: " + \
+            self.err["errMsg"]
+
 
 class TransactionVerificationError(RaveError):
     """ Raised when transaction could not be verified """
+
     def __init__(self, err):
         self.err = err
 
     def __str__(self):
-        return "Your transaction verification call failed with message: "+self.err["errMsg"]
+        return "Your transaction verification call failed with message: " + \
+            self.err["errMsg"]
+
 
 class UssdChargeError(RaveError):
     """ Raised when ussd charge has failed """
+
     def __init__(self, err):
         self.err = err
 
     def __str__(self):
-        return "Your ussd charge call failed with message: "+self.err["errMsg"]
+        return "Your ussd charge call failed with message: " + \
+            self.err["errMsg"]
```

### Comparing `rave_python-1.2.9/rave_python/rave_francophone.py` & `rave_python-1.4.0/rave_python/rave_ussd.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,95 @@
-from rave_python.rave_exceptions import RaveError, IncompletePaymentDetailsError, MobileChargeError, TransactionVerificationError, TransactionValidationError, ServerError
+from rave_python.rave_exceptions import UssdChargeError, ServerError
+
 from rave_python.rave_payment import Payment
 from rave_python.rave_misc import generateTransactionReference
 import json
-import webbrowser
 
-class Francophone(Payment):
-    
-    def __init__(self, publicKey, secretKey, production, usingEnv):
-        super(Francophone, self).__init__(publicKey, secretKey, production, usingEnv)
 
+class Ussd(Payment):
+    def __init__(self, publicKey, secretKey, production, usingEnv):
+        """ This is the rave object for ussd transactions. It contains the following public functions:\n
+        .charge -- This is for making a ussd charge\n
+        .verify -- This checks the status of your transaction\n
+        """
+        super(Ussd, self).__init__(publicKey, secretKey, production, usingEnv)
 
-    # returns true if further action is required, false if it isn't    
-    # def _handleChargeResponse(self, response, txRef, request=None):
-    #     """ This handles charge responses """
-    #     res =  self._preliminaryResponseChecks(response, MobileChargeError, txRef=txRef)
-
-    #     responseJson = res["json"]
-    #     flwRef = res["flwRef"]
-
-    #     # Checking if there is redirect url
-
-    #     if responseJson["data"]["data"].get("redirect_url", "N/A") == "N/A":
-    #         redirectUrl = None
-    #     else:
-    #         redirectUrl = responseJson["data"]["data"]["redirect_url"]
-
-    #     # If all preliminary checks passed
-    #     if not (responseJson["data"].get("chargeResponseCode", None) == "00"):
-    #         # Otherwise we return that further action is required, along with the response
-    #         # suggestedAuth = responseJson["data"].get("suggested_auth", None)
-    #         return {
-    #                     "error": False, 
-    #                     "status": responseJson["status"],  
-    #                     "message": responseJson["message"],
-    #                     "code": responseJson["data"]["code"],
-    #                     "transaction status": responseJson["data"]["status"],
-    #                     "ts": responseJson["data"]["ts"],
-    #                     "link": responseJson["data"]["link"]
-    #                 }
-    #     else:
-    #         return {"error": False, "status": responseJson["status"],  "validationRequired": False, "txRef": txRef, "flwRef": flwRef, "suggestedAuth": None, "redirectUrl": redirectUrl}
-    
-    # Charge mobile money function
-    def charge(self, accountDetails, hasFailed=False):
-        """ This is the charge call for central francophone countries.
-             Parameters include:\n
-            accountDetails (dict) -- These are the parameters passed to the function for processing\n
-            hasFailed (boolean) -- This is a flag to determine if the attempt had previously failed due to a timeout\n
+    def _handleChargeResponse(self, response, txRef, request):
+        bankList = {"gtb": "058", "zenith": "057"}
+        gtbResponseText = "To complete this transaction, please dial *737*50*charged_amount*159#"
+        # This checks if we can parse the json successfully
+
+        res = self._preliminaryResponseChecks(
+            response, UssdChargeError, txRef=txRef)
+
+        responseJson = res["json"]
+        flwRef = res["flwRef"]
+
+        # Charge response code of 00 means successful, 02 means failed. Here we
+        # check if the code is not 00
+        if not (responseJson["data"].get("chargeResponseCode", None) == "00"):
+            # If it is we return that further action is required
+            # If it is a gtbank account
+            if request["accountbank"] == bankList["gtb"]:
+                return {
+                    "error": False,
+                    "validationRequired": True,
+                    "txRef": txRef,
+                    "flwRef": flwRef,
+                    "validationInstruction": gtbResponseText}
+            else:
+                return {
+                    "error": False,
+                    "validationRequired": True,
+                    "txRef": txRef,
+                    "flwRef": flwRef,
+                    "validationInstruction": responseJson["data"].get(
+                        "validateInstructions",
+                        None)}
+
+        # If a charge is successful, we return that further action is not
+        # required, along with the response
+        else:
+            return {
+                "error": False,
+                "validationRequired": False,
+                "txRef": txRef,
+                "flwRef": flwRef,
+                "validationInstruction": None}
+
+    # Charge ussd function
+
+    def charge(self, ussdDetails, hasFailed=False):
+        """ This is used to charge through ussd.\n
+             Parameters are:\n
+            ussdDetails (dict) -- This is a dictionary comprising payload parameters.\n
+            hasFailed (bool) -- This indicates whether the request had previously failed for timeout handling
         """
 
-        feature_name = "Initiate-Francophone-mobile-money-charge"
         endpoint = self._baseUrl + self._endpointMap["account"]["charge"]
 
-        # It is faster to add boilerplate than to check if each one is present
-        accountDetails.update({"payment_type": "mobilemoneyfrancophone", "is_mobile_money_franco":"1"})
-        
-        # If transaction reference is not set 
-        if not ("txRef" in accountDetails):
-            accountDetails.update({"txRef": generateTransactionReference()})
-
-        # If order reference is not set
-        if not ("orderRef" in accountDetails):
-            accountDetails.update({"orderRef": generateTransactionReference()})
-
-        # Checking for required account components
-        # requiredParameters = ["amount", "email", "phonenumber", "IP", "redirect_url"]
-        requiredParameters = ["amount"]
-        return super(Francophone, self).charge(feature_name, accountDetails, requiredParameters, endpoint)
-
-    def refund(self, flwRef, amount):
-        feature_name = "Francophone-charge-refund"
-        endpoint = self._baseUrl + self._endpointMap["refund"]
-        return super(Francophone, self).refund(feature_name, flwRef, amount)
+        # Add boilerplate ussd code
+        ussdDetails.update({"is_ussd": "1", "payment_type": "ussd"})
+        # if transaction reference is not present, generate
+        if not ("txRef" in ussdDetails):
+            ussdDetails.update({"txRef": generateTransactionReference()})
+        if not ("orderRef" in ussdDetails):
+            ussdDetails.update({"orderRef": generateTransactionReference()})
+        # Checking for required ussd components (not checking for payment_type,
+        # is_ussd, txRef or orderRef again to increase efficiency)
+        requiredParameters = [
+            "accountbank",
+            "accountnumber",
+            "amount",
+            "email",
+            "phonenumber",
+            "IP"]
+
+        # Should return request is a less efficient call but it is required
+        # here because we need bank code in _handleResponses
+        return super(
+            Ussd,
+            self).charge(
+            ussdDetails,
+            requiredParameters,
+            endpoint,
+            shouldReturnRequest=True)
```

### Comparing `rave_python-1.2.9/rave_python/rave_ghmobile.py` & `rave_python-1.4.0/rave_python/rave_ghmobile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 from rave_python.rave_payment import Payment
 from rave_python.rave_misc import generateTransactionReference
-import json, requests
+import json
+import requests
+
 
 class GhMobile(Payment):
-    
+
     def __init__(self, publicKey, secretKey, production, usingEnv):
         super(GhMobile, self).__init__(publicKey, secretKey, production, usingEnv)
 
-
     # Charge mobile money function
+
     def charge(self, accountDetails, hasFailed=False):
-        
         """ This is the ghMobile charge call.
              Parameters include:\n
             accountDetails (dict) -- These are the parameters passed to the function for processing\n
             hasFailed (boolean) -- This is a flag to determine if the attempt had previously failed due to a timeout\n
         """
-        
+
         endpoint = self._baseUrl + self._endpointMap["account"]["charge"]
-        feature_name = "Initiate-Ghana-mobile-money-charge"
-        
+        feature_name = "GHS Mobile Money Payments"
+
         # It is faster to add boilerplate than to check if each one is present
-        accountDetails.update({"payment_type": "mobilemoneygh", "country":"GH", "is_mobile_money_gh":"1", "currency":"GHS"})
-        
-        # If transaction reference is not set 
+        accountDetails.update({
+            "payment_type": "mobilemoneygh",
+            "country": "GH",
+            "is_mobile_money_gh": "1",
+            "currency": "GHS"
+            })
+
+        # If transaction reference is not set
         if not ("txRef" in accountDetails):
             accountDetails.update({"txRef": generateTransactionReference()})
-        
+
         # If order reference is not set
         if not ("orderRef" in accountDetails):
             accountDetails.update({"orderRef": generateTransactionReference()})
 
         # Checking for required account components
-        requiredParameters = ["amount", "email", "phonenumber", "network", "IP", "redirect_url"]
+        requiredParameters = ["amount", "email", "phonenumber", "network"]
+        
         return super(GhMobile, self).charge(feature_name, accountDetails, requiredParameters, endpoint)
 
     def refund(self, flwRef, amount):
-        feature_name = "Ghana-mobile-money-charge-refund"
+        feature_name = "GHS Payments Refund"
         endpoint = self._baseUrl + self._endpointMap["refund"]
         return super(GhMobile, self).refund(feature_name, flwRef, amount)
 
+    def verify(self, txRef):
+        feature_name = "Verify GHS Payment"
+        endpoint = self._baseUrl + self._endpointMap["verify"]
+        return super(GhMobile, self).verify(feature_name, txRef)
```

### Comparing `rave_python-1.2.9/rave_python/rave_misc.py` & `rave_python-1.4.0/rave_python/rave_misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,109 +1,140 @@
 """ Miscellaneous helper functions """
 import time
 from rave_python.rave_exceptions import IncompletePaymentDetailsError, AuthMethodNotSupportedError
 # Helper function to generate unique transaction reference
+
+
 def generateTransactionReference(merchantId=None):
     """ This is a helper function for generating unique transaction  references.\n
          Parameters include:\n
         merchantId (string) -- (optional) You can specify a merchant id to start references e.g. merchantId-12345678
     """
     rawTime = round(time.time() * 1000)
     timestamp = int(rawTime)
     if merchantId:
-        return merchantId+"-"+str(timestamp)
+        return merchantId + "-" + str(timestamp)
     else:
-        return "MC-"+str(timestamp)
+        return "MC-" + str(timestamp)
 
 
 def checkTransferParameters(requiredParameters, paymentDetails):
     # Transfer specific meta parameters
-    requiredTransferMetaParams = ['AccountNumber','RoutingNumber', 'BankName', 'BeneficiaryName','BeneficiaryAddress', 'BeneficiaryCountry']
+    requiredTransferMetaParams = [
+        'AccountNumber',
+        'RoutingNumber',
+        'BankName',
+        'BeneficiaryName',
+        'BeneficiaryAddress',
+        'BeneficiaryCountry']
     excludedCurrencies = ["NGN", "GHS", "KES", "UGX", "TZS"]
-    #end Transfer specific meta parameters
+    # end Transfer specific meta parameters
 
     # International transfer check block
     if "bulk_data" in requiredParameters:
         for i in paymentDetails["bulk_data"]:
             if "debit_currency" not in i:
                 if i["Currency"] not in excludedCurrencies:
                     if "meta" in i:
                         for j in requiredTransferMetaParams:
                             if j not in i["meta"][0]:
-                                raise IncompletePaymentDetailsError(i, requiredTransferMetaParams)
+                                raise IncompletePaymentDetailsError(
+                                    i, requiredTransferMetaParams)
                     else:
-                        raise IncompletePaymentDetailsError("meta", requiredParameters)
+                        raise IncompletePaymentDetailsError(
+                            "meta", requiredParameters)
     else:
         if "debit_currency" not in paymentDetails:
             if paymentDetails["currency"] not in excludedCurrencies:
                 if "meta" in paymentDetails:
                     for i in requiredTransferMetaParams:
                         if i not in paymentDetails["meta"][0]:
-                            raise IncompletePaymentDetailsError(i, requiredTransferMetaParams)
+                            raise IncompletePaymentDetailsError(
+                                i, requiredTransferMetaParams)
                 else:
-                    raise IncompletePaymentDetailsError("meta", requiredParameters)
+                    raise IncompletePaymentDetailsError(
+                        "meta", requiredParameters)
+
+    # end international transfer check block
+
+# If parameters are complete, returns true. If not returns false with
+# parameter missing
 
-    #end international transfer check block
 
-# If parameters are complete, returns true. If not returns false with parameter missing
 def checkIfParametersAreComplete(requiredParameters, paymentDetails):
     """ This returns true/false depending on if the paymentDetails match the required parameters """
     for i in requiredParameters:
         if i not in paymentDetails:
             raise IncompletePaymentDetailsError(i, requiredParameters)
     return True, None
 
+
 def getTypeOfArgsRequired(suggestedAuth):
     """ This is used to get the type of argument needed to complete your charge call.\n
             Parameters include:\n
         suggestedAuth (dict) -- This is the action returned from the charge call\n
 
         Returns:\n
         pin -- This means that the updatePayload call requires a pin. Pin is passed as a string argument to updatePayload\n
         address -- This means that the updatePayload call requires an address dict. The dict must contain "billingzip", "billingcity", "billingaddress", "billingstate", "billingcountry".
     """
-    keywordMap = {"PIN": "pin", "AVS_VBVSECURECODE": "address", "NOAUTH_INTERNATIONAL": "address", "AVS_NOAUTH": "address"}
-    # Checks if the auth method passed is included in keywordMapping i.e. if it is supported
+    keywordMap = {
+        "PIN": "pin",
+        "AVS_VBVSECURECODE": "address",
+        "NOAUTH_INTERNATIONAL": "address",
+        "AVS_NOAUTH": "address"}
+    # Checks if the auth method passed is included in keywordMapping i.e. if
+    # it is supported
     if not keywordMap.get(suggestedAuth, None):
         raise AuthMethodNotSupportedError(suggestedAuth)
-    
+
     return keywordMap[suggestedAuth]
 
 # Update payload
-def updatePayload(suggestedAuth, payload, **kwargs): 
+
+
+def updatePayload(suggestedAuth, payload, **kwargs):
     """ This is used to update the payload of your request upon a charge that requires more parameters. It maintains the transaction refs and all the original parameters of the request.\n
             Parameters include:\n
         suggestedAuth (dict) -- This is what is returned from the charge call\n
         payload (dict) -- This is the original payload\n
         \n
         ## This updates payload directly
-    """ 
+    """
 
-    # Sets the keyword to check for in kwargs (it maps the suggestedAuth to keywords)
+    # Sets the keyword to check for in kwargs (it maps the suggestedAuth to
+    # keywords)
     keyword = getTypeOfArgsRequired(suggestedAuth)
 
     # Checks
 
     # 1) Checks if keyword is present in kwargs
     if not kwargs.get(keyword, None):
-        # Had to split variable assignment and raising ValueError because of error message python displayed
-        errorMsg = "Please provide the appropriate argument for the auth method. For {}, we require a \"{}\" argument.".format(suggestedAuth["suggested_auth"], keyword)
+        # Had to split variable assignment and raising ValueError because of
+        # error message python displayed
+        errorMsg = "Please provide the appropriate argument for the auth method. For {}, we require a \"{}\" argument.".format(
+            suggestedAuth["suggested_auth"], keyword)
         raise ValueError(errorMsg)
 
-    # 2) If keyword is address, checks if all required address parameters are present
+    # 2) If keyword is address, checks if all required address parameters are
+    # present
     if keyword == "address":
-        requiredAddressParameters = ["billingzip", "billingcity", "billingaddress", "billingstate", "billingcountry"]
-        checkIfParametersAreComplete(requiredAddressParameters, kwargs[keyword])
-        
+        requiredAddressParameters = [
+            "billingzip",
+            "billingcity",
+            "billingaddress",
+            "billingstate",
+            "billingcountry"]
+        checkIfParametersAreComplete(
+            requiredAddressParameters, kwargs[keyword])
+
     # All checks passed
 
     # Add items to payload
     # If the argument is a dictionary, we add the argument as is
     if isinstance(kwargs[keyword], dict):
         payload.update(kwargs[keyword])
 
     # If it's not we add it manually
     else:
         payload.update({"suggested_auth": suggestedAuth})
         payload.update({keyword: kwargs[keyword]})
-            
-
```

### Comparing `rave_python-1.2.9/rave_python/rave_mpesa.py` & `rave_python-1.4.0/rave_python/rave_mpesa.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,60 @@
 from rave_python.rave_exceptions import RaveError, IncompletePaymentDetailsError, AccountChargeError, TransactionVerificationError, TransactionValidationError, ServerError
 from rave_python.rave_payment import Payment
 from rave_python.rave_misc import generateTransactionReference
-import json, requests
+import json
+import requests
+
 
 class Mpesa(Payment):
-    
+
     def __init__(self, publicKey, secretKey, production, usingEnv):
         super(Mpesa, self).__init__(publicKey, secretKey, production, usingEnv)
 
     # Charge mobile money function
     def charge(self, accountDetails, hasFailed=False):
-        
         """ This is the mpesa charge call.\n
              Parameters include:\n
             accountDetails (dict) -- These are the parameters passed to the function for processing\n
             hasFailed (boolean) -- This is a flag to determine if the attempt had previously failed due to a timeout\n
         """
-        ## feature logic
+        # feature logic
         # Setting the endpoint
-        feature_name = "Initiate-Mpesa-charge"
+        feature_name = "Mpesa-charge"
         endpoint = self._baseUrl + self._endpointMap["account"]["charge"]
-        
+
         # Adding boilerplate mpesa requirements
-        accountDetails.update({"payment_type": "mpesa", "country":"KE", "is_mpesa":"1", "is_mpesa_lipa":"1", "currency":"KES"})
-        
-        # If transaction reference is not set 
+        accountDetails.update({"payment_type": "mpesa",
+                               "country": "KE",
+                               "is_mpesa": "1",
+                               "is_mpesa_lipa": "1",
+                               "currency": "KES"})
+
+        # If transaction reference is not set
         if not ("txRef" in accountDetails):
             accountDetails.update({"txRef": generateTransactionReference()})
-        
+
         # If order reference is not set
         if not ("orderRef" in accountDetails):
             accountDetails.update({"orderRef": generateTransactionReference()})
 
         # Checking for required account components
         requiredParameters = ["amount", "email", "phonenumber", "IP"]
-        res = super(Mpesa, self).charge(feature_name, accountDetails, requiredParameters, endpoint, isMpesa=True)
+        res = super(
+            Mpesa,
+            self).charge(
+            feature_name,
+            accountDetails,
+            requiredParameters,
+            endpoint,
+            isMpesa=True)
         return res
 
     def verify(self, txRef):
-        feature_name = "Verify-Mpesa_charge"
+        feature_name = "Verify-Mpesa"
         endpoint = self._baseUrl + self._endpointMap["account"]["verify"]
         return super(Mpesa, self).verify(feature_name, txRef, endpoint)
 
     def refund(self, flwRef, amount):
-        feature_name = "Mpesa-charge-refund"
+        feature_name = "Mpesa-refund"
         endpoint = self._baseUrl + self._endpointMap["account"]["refund"]
         return super(Mpesa, self).refund(feature_name, flwRef, amount)
```

### Comparing `rave_python-1.2.9/rave_python/rave_payment.py` & `rave_python-1.4.0/rave_python/rave_payment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import requests, json, copy
+import requests
+import json
+import copy
 from rave_python.rave_base import RaveBase
 from rave_python.rave_exceptions import RaveError, IncompletePaymentDetailsError, AuthMethodNotSupportedError, TransactionChargeError, TransactionVerificationError, TransactionValidationError, ServerError, RefundError, PreauthCaptureError
 from rave_python.rave_misc import checkIfParametersAreComplete
 
 response_object = {
     "error": False,
     "transactionComplete": False,
@@ -11,274 +13,384 @@
     "chargecode": '00',
     "status": "",
     "vbvcode": "",
     "vbvmessage": "",
     "acctmessage": "",
     "currency": "",
     "chargedamount": 00,
-    "chargemessage": ""
+    "chargemessage": "",
+    "meta": ""
 }
 
 # All payment subclasses are encrypted classes
+
+
 class Payment(RaveBase):
     """ This is the base class for all the payments """
+
     def __init__(self, publicKey, secretKey, production, usingEnv):
         # Instantiating the base class
-        super(Payment, self).__init__(publicKey, secretKey, production, usingEnv)
+        super(
+            Payment,
+            self).__init__(
+            publicKey,
+            secretKey,
+            production,
+            usingEnv)
 
     @classmethod
-    def retrieve(cls, mapping, *keys): 
-        return (mapping[key] for key in keys) 
+    def retrieve(cls, mapping, *keys):
+        return (mapping[key] for key in keys)
 
     @classmethod
-    def deleteUnnecessaryKeys(cls,response_dict, *keys):
+    def deleteUnnecessaryKeys(cls, response_dict, *keys):
         for key in keys:
             del response_dict[key]
         return response_dict
 
-    def _preliminaryResponseChecks(self, response, TypeOfErrorToRaise, txRef=None, flwRef=None):
+    def _preliminaryResponseChecks(
+            self,
+            response,
+            TypeOfErrorToRaise,
+            txRef=None,
+            flwRef=None):
         preliminary_error_response = copy.deepcopy(response_object)
-        preliminary_error_response = Payment.deleteUnnecessaryKeys(preliminary_error_response, "transactionComplete", "chargecode", "vbvmessage", "vbvcode", "acctmessage", "currency")
+        preliminary_error_response = Payment.deleteUnnecessaryKeys(
+            preliminary_error_response,
+            "transactionComplete",
+            "chargecode",
+            "vbvmessage",
+            "vbvcode",
+            "acctmessage",
+            "currency")
 
         # Check if we can obtain a json
         try:
             responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "txRef": txRef, "flwRef": flwRef, "errMsg": response})
-
+        except BaseException:
+            raise ServerError({"error": True, "txRef": txRef,
+                              "flwRef": flwRef, "errMsg": response})
 
         # Check if the response contains data parameter
         if responseJson.get("data", None):
             if txRef:
                 flwRef = responseJson["data"].get("flwRef", None)
             if flwRef:
                 txRef = responseJson["data"].get("txRef", None)
         else:
-            raise TypeOfErrorToRaise({"error": True, "txRef": txRef, "flwRef": flwRef, "errMsg": responseJson.get("message", "Server is down")})
-        
+            raise TypeOfErrorToRaise({"error": True,
+                                      "txRef": txRef,
+                                      "flwRef": flwRef,
+                                      "errMsg": responseJson.get("message",
+                                                                 "Server is down")})
+
         # Check if it is returning a 200
         if not response.ok:
             errMsg = responseJson["data"].get("message", None)
-            raise TypeOfErrorToRaise({"error": True, "txRef": txRef, "flwRef": flwRef, "errMsg": errMsg})
-        
+            raise TypeOfErrorToRaise(
+                {"error": True, "txRef": txRef, "flwRef": flwRef, "errMsg": errMsg})
+
         return {"json": responseJson, "flwRef": flwRef, "txRef": txRef}
 
-    def _handleChargeResponse(self, response, txRef, request=None, isMpesa=False):
+    def _handleChargeResponse(self,response,txRef,request=None,isMpesa=False):
         """ This handles transaction charge responses """
 
         # If we cannot parse the json, it means there is a server error
-        res = self._preliminaryResponseChecks(response, TransactionChargeError, txRef=txRef)
-        
-        
+        res = self._preliminaryResponseChecks(
+            response, TransactionChargeError, txRef=txRef)
         responseJson = res["json"]
 
         if isMpesa:
             return {
-                "error": False, 
-                "status": responseJson["status"], 
-                "validationRequired": True, 
-                "txRef": txRef, 
-                "flwRef": responseJson["data"]["flwRef"], 
-                "narration": responseJson["data"]["narration"]
-                }
+                "error": False,
+                "status": responseJson["status"],
+                "validationRequired": True,
+                "txRef": txRef,
+                "flwRef": responseJson["data"]["flwRef"],
+                "narration": responseJson["data"]["narration"],
+            }
         else:
             # if all preliminary tests pass
-            if not (responseJson["data"].get("chargeResponseCode", None) == "00"):
+            if not (
+                responseJson["data"].get(
+                    "chargeResponseCode",
+                    None) == "00"):
                 if responseJson.get("message", 'None') == 'Momo initiated':
                     return {
-                            "error": False, 
-                            "status": responseJson["status"],  
-                            "message": responseJson["message"],
-                            "code": responseJson["data"]["code"],
-                            "transaction status": responseJson["data"]["status"],
-                            "ts": responseJson["data"]["ts"],
-                            "link": responseJson["data"]["link"]
-                        }
-
-                return {"error": False, "status": responseJson["status"],"validationRequired": True, "txRef": txRef, "flwRef": responseJson["data"]["flwRef"], "chargeResponseMessage": responseJson["data"]["chargeResponseMessage"]}
+                        "error": False,
+                        "status": responseJson["status"],
+                        "message": responseJson["message"],
+                        "code": responseJson["data"]["code"],
+                        "transaction status": responseJson["data"]["status"],
+                        "ts": responseJson["data"]["ts"],
+                        "link": responseJson["data"]["link"]
+                    }
+                return {
+                    "error": False,
+                    "status": responseJson["status"],
+                    "validationRequired": True,
+                    "txRef": txRef,
+                    "flwRef": responseJson["data"]["flwRef"],
+                    "chargeResponseMessage": responseJson["data"]["chargeResponseMessage"]}
             else:
-                return {"error": True,  "validationRequired": False, "txRef": txRef, "flwRef": responseJson["data"]["flwRef"]}
-    
+                return {
+                    "error": True,
+                    "validationRequired": False,
+                    "txRef": txRef,
+                    "flwRef": responseJson["data"]["flwRef"]}
+
     def _handleCaptureResponse(self, response, request=None):
         """ This handles transaction charge responses """
 
         # If we cannot parse the json, it means there is a server error
-        res = self._preliminaryResponseChecks(response, PreauthCaptureError, txRef='')
-        
+        res = self._preliminaryResponseChecks(
+            response, PreauthCaptureError, txRef='')
+
         responseJson = res["json"]
         flwRef = responseJson["data"]["flwRef"]
         txRef = responseJson["data"]["txRef"]
-        
+
         # if all preliminary tests pass
         if not (responseJson["data"].get("chargeResponseCode", None) == "00"):
-            return {"error": False,  "validationRequired": True, "txRef": txRef, "flwRef": flwRef}
+            return {
+                "error": False,
+                "validationRequired": True,
+                "txRef": txRef,
+                "flwRef": flwRef}
         else:
-            return {"error": False, "status":responseJson["status"], "message": responseJson["message"],  "validationRequired": False, "txRef": txRef, "flwRef": flwRef}
-
+            return {
+                "error": False,
+                "status": responseJson["status"],
+                "message": responseJson["message"],
+                "validationRequired": False,
+                "txRef": txRef,
+                "flwRef": flwRef}
 
     # This can be altered by implementing classes but this is the default behaviour
     # Returns True and the data if successful
+
     def _handleVerifyResponse(self, response, txRef):
         """ This handles all responses from the verify call.\n
              Parameters include:\n
             response (dict) -- This is the response Http object returned from the verify call
          """
         verify_response = copy.deepcopy(response_object)
-        res = self._preliminaryResponseChecks(response, TransactionVerificationError, txRef=txRef)
-
+        res = self._preliminaryResponseChecks(
+            response, TransactionVerificationError, txRef=txRef)
 
         responseJson = res["json"]
-        # retrieve necessary properties from response 
+        # retrieve necessary properties from response
         verify_response["status"] = responseJson['status']
-        verify_response['flwRef'], verify_response["txRef"], verify_response["vbvcode"], verify_response["vbvmessage"], verify_response["acctmessage"], verify_response["currency"], verify_response["chargecode"], verify_response["amount"], verify_response["chargedamount"], verify_response["chargemessage"] = Payment.retrieve(responseJson['data'], "flwref", "txref", "vbvcode", "vbvmessage", "acctmessage", "currency", "chargecode", "amount", "chargedamount", "chargemessage")
+        verify_response['flwRef'], verify_response["txRef"], verify_response["vbvcode"], verify_response["vbvmessage"], verify_response["acctmessage"], verify_response["currency"], verify_response["chargecode"], verify_response["amount"], verify_response[
+            "chargedamount"], verify_response["chargemessage"], verify_response["meta"] = Payment.retrieve(responseJson['data'], "flwref", "txref", "vbvcode", "vbvmessage", "acctmessage", "currency", "chargecode", "amount", "chargedamount", "chargemessage", "meta")
 
         # Check if the chargecode is 00
         if verify_response['chargecode'] == "00":
             verify_response["error"] = False
             verify_response["transactionComplete"] = True
             return verify_response
-        
+
         else:
-            verify_response["error"] = True # changed to True on 15/10/2018
+            verify_response["error"] = True  # changed to True on 15/10/2018
             verify_response["transactionComplete"] = False
             return verify_response
-        
+
         # # Check if the chargecode is 00
         # if not (responseJson["data"].get("chargecode", None) == "00"):
-        #     return {"error": False, "transactionComplete": False, "txRef": txRef, "flwRef":flwRef}
-        
+        # return {"error": False, "transactionComplete": False, "txRef": txRef,
+        # "flwRef":flwRef}
+
         # else:
-        #     return {"error": False, "transactionComplete": True, "txRef": txRef, "flwRef":flwRef}
+        # return {"error": False, "transactionComplete": True, "txRef": txRef,
+        # "flwRef":flwRef}
+
+    # returns true if further action is required, false if it isn't
 
-    
-    # returns true if further action is required, false if it isn't    
     def _handleValidateResponse(self, response, flwRef, request=None):
         """ This handles validation responses """
 
         # If json is not parseable, it means there is a problem in server
-            
-        res = self._preliminaryResponseChecks(response, TransactionValidationError, flwRef=flwRef)
+
+        res = self._preliminaryResponseChecks(
+            response, TransactionValidationError, flwRef=flwRef)
 
         responseJson = res["json"]
-        if responseJson["data"].get("tx") == None:
+        if responseJson["data"].get("tx") is None:
             txRef = responseJson["data"]["txRef"]
         else:
             txRef = responseJson["data"]["tx"]["txRef"]
 
         # Of all preliminary checks passed
-        if not (responseJson["data"].get("tx", responseJson["data"]).get("chargeResponseCode", None) == "00"):
-            errMsg = responseJson["data"].get("tx", responseJson["data"]).get("chargeResponseMessage", None)
-            raise TransactionValidationError({"error": True, "txRef": txRef, "flwRef": flwRef , "errMsg": errMsg})
+        if not (
+            responseJson["data"].get(
+                "tx",
+                responseJson["data"]).get(
+                "chargeResponseCode",
+                None) == "00"):
+            errMsg = responseJson["data"].get(
+                "tx", responseJson["data"]).get(
+                "chargeResponseMessage", None)
+            raise TransactionValidationError(
+                {"error": True, "txRef": txRef, "flwRef": flwRef, "errMsg": errMsg})
 
         else:
-            return {"status": responseJson["status"], "message": responseJson["message"], "error": False, "txRef": txRef, "flwRef": flwRef}
-
-
-    # Charge function (hasFailed is a flag that indicates there is a timeout), shouldReturnRequest indicates whether to send the request back to the _handleResponses function
-    def charge(self, feature_name, paymentDetails, requiredParameters, endpoint, shouldReturnRequest=False, isMpesa=False):
+            return {
+                "status": responseJson["status"],
+                "message": responseJson["message"],
+                "error": False,
+                "txRef": txRef,
+                "flwRef": flwRef}
+
+    # Charge function (hasFailed is a flag that indicates there is a timeout),
+    # shouldReturnRequest indicates whether to send the request back to the
+    # _handleResponses function
+
+    def charge(
+            self,
+            feature_name,
+            paymentDetails,
+            requiredParameters,
+            endpoint,
+            shouldReturnRequest=False,
+            isMpesa=False):
         """ This is the base charge call. It is usually overridden by implementing classes.\n
              Parameters include:\n
             paymentDetails (dict) -- These are the parameters passed to the function for processing\n
             requiredParameters (list) -- These are the parameters required for the specific call\n
             hasFailed (boolean) -- This is a flag to determine if the attempt had previously failed due to a timeout\n
             shouldReturnRequest -- This determines whether a request is passed to _handleResponses\n
         """
         # Checking for required components
         try:
             checkIfParametersAreComplete(requiredParameters, paymentDetails)
-        except: 
+        except BaseException:
             raise
-        
-        # Performing shallow copy of payment details to prevent tampering with original
+
+        # Performing shallow copy of payment details to prevent tampering with
+        # original
         paymentDetails = copy.copy(paymentDetails)
-        
+
         # Adding PBFPubKey param to paymentDetails
         paymentDetails.update({"PBFPubKey": self._getPublicKey()})
 
         # Collating request headers
         headers = {
             'content-type': 'application/json',
         }
         if "token" in paymentDetails:
             paymentDetails.update({"SECKEY": self._getSecretKey()})
             # print(json.dumps(paymentDetails))
-            response = requests.post(endpoint, headers=headers, data=json.dumps(paymentDetails))
+            response = requests.post(
+                endpoint,
+                headers=headers,
+                data=json.dumps(paymentDetails))
         else:
-            # Encrypting payment details (_encrypt is inherited from RaveEncryption)
+            # Encrypting payment details (_encrypt is inherited from
+            # RaveEncryption)
             encryptedPaymentDetails = self._encrypt(json.dumps(paymentDetails))
-            
+
             # Collating the payload for the request
             payload = {
                 "PBFPubKey": paymentDetails["PBFPubKey"],
                 "client": encryptedPaymentDetails,
                 "alg": "3DES-24"
             }
-            response = requests.post(endpoint, headers=headers, data=json.dumps(payload))
-            
-            #feature logging
+            response = requests.post(
+                endpoint, headers=headers, data=json.dumps(payload))
+
+            # feature logging
             if response.ok:
                 tracking_endpoint = self._trackingMap
                 responseTime = response.elapsed.total_seconds()
-                tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": feature_name, "message": responseTime}
-                tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
+                tracking_payload = {
+                    "publicKey": self._getPublicKey(),
+                    "language": "Python v2",
+                    "version": "1.2.13",
+                    "title": feature_name,
+                    "message": responseTime}
+                tracking_response = requests.post(
+                    tracking_endpoint, data=json.dumps(tracking_payload))
             else:
                 tracking_endpoint = self._trackingMap
                 responseTime = response.elapsed.total_seconds()
-                tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": feature_name + "-error", "message": responseTime}
-                tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
-        
+                tracking_payload = {
+                    "publicKey": self._getPublicKey(),
+                    "language": "Python v2",
+                    "version": "1.2.13",
+                    "title": feature_name + " error",
+                    "message": responseTime}
+                tracking_response = requests.post(
+                    tracking_endpoint, data=json.dumps(tracking_payload))
+
         if shouldReturnRequest:
             if isMpesa:
-                return self._handleChargeResponse(response, paymentDetails["txRef"], paymentDetails, True)
-            return self._handleChargeResponse(response, paymentDetails["txRef"], paymentDetails)
+                return self._handleChargeResponse(
+                    response, paymentDetails["txRef"], paymentDetails, True)
+            return self._handleChargeResponse(
+                response, paymentDetails["txRef"], paymentDetails)
         else:
             if isMpesa:
-                return self._handleChargeResponse(response, paymentDetails["txRef"], paymentDetails, True)
-            return self._handleChargeResponse(response, paymentDetails["txRef"])
-        
-       
+                return self._handleChargeResponse(
+                    response, paymentDetails["txRef"], paymentDetails, True)
+            return self._handleChargeResponse(
+                response, paymentDetails["txRef"])
 
     def validate(self, feature_name, flwRef, otp, endpoint=None):
         """ This is the base validate call.\n
              Parameters include:\n
             flwRef (string) -- This is the flutterwave reference returned from a successful charge call. You can access this from action["flwRef"] returned from the charge call\n
             otp (string) -- This is the otp sent to the user \n
         """
 
-        if not endpoint: 
+        if not endpoint:
             endpoint = self._baseUrl + self._endpointMap["account"]["validate"]
-            
+
         # Collating request headers
         headers = {
             'content-type': 'application/json',
         }
-        
+
         payload = {
             "PBFPubKey": self._getPublicKey(),
-            "transactionreference": flwRef, 
+            "transactionreference": flwRef,
             "transaction_reference": flwRef,
             "otp": otp
         }
-        
-        response = requests.post(endpoint, headers = headers, data=json.dumps(payload))
 
-        #feature logging
+        response = requests.post(
+            endpoint,
+            headers=headers,
+            data=json.dumps(payload))
+
+        # feature logging
         if response.ok:
             tracking_endpoint = self._trackingMap
             responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": feature_name, "message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
+            tracking_payload = {
+                "publicKey": self._getPublicKey(),
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": feature_name,
+                "message": responseTime}
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
         else:
             tracking_endpoint = self._trackingMap
             responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": feature_name + "-error", "message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
+            tracking_payload = {
+                "publicKey": self._getPublicKey(),
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": feature_name + "-error",
+                "message": responseTime}
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
 
         return self._handleValidateResponse(response, flwRef)
-        
+
     # Verify charge
     def verify(self, feature_name, txRef, endpoint=None):
         """ This is used to check the status of a transaction.\n
              Parameters include:\n
             txRef (string) -- This is the transaction reference that you passed to your charge call. If you didn't define a reference, you can access the auto-generated one from payload["txRef"] or action["txRef"] from the charge call\n
         """
         if not endpoint:
@@ -290,68 +402,95 @@
         }
 
         # Payload for the request headers
         payload = {
             "txref": txRef,
             "SECKEY": self._getSecretKey()
         }
-        response = requests.post(endpoint, headers=headers, data=json.dumps(payload))
+        response = requests.post(
+            endpoint,
+            headers=headers,
+            data=json.dumps(payload))
 
-        #feature logging
+        # feature logging
         if response.ok:
             tracking_endpoint = self._trackingMap
             responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": feature_name, "message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
+            tracking_payload = {
+                "publicKey": self._getPublicKey(),
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": feature_name,
+                "message": responseTime}
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
         else:
             tracking_endpoint = self._trackingMap
             responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": feature_name + "-error", "message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
+            tracking_payload = {
+                "publicKey": self._getPublicKey(),
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": feature_name + "-error",
+                "message": responseTime}
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
 
         return self._handleVerifyResponse(response, txRef)
 
-    #Refund call
+    # Refund call
     def refund(self, feature_name, flwRef, amount, ):
-        """ This is used to refund a transaction from any of Rave's component objects.\n 
+        """ This is used to refund a transaction from any of Rave's component objects.\n
              Parameters include:\n
             flwRef (string) -- This is the flutterwave reference returned from a successful call from any component. You can access this from action["flwRef"] returned from the charge call
         """
         payload = {
             "ref": flwRef,
             "seckey": self._getSecretKey(),
             "amount": amount,
         }
         headers = {
-            "Content-Type":"application/json"
+            "Content-Type": "application/json"
         }
         endpoint = self._baseUrl + self._endpointMap["refund"]
 
-        response = requests.post(endpoint, headers = headers, data=json.dumps(payload))
+        response = requests.post(
+            endpoint,
+            headers=headers,
+            data=json.dumps(payload))
 
-        #feature logging
+        # feature logging
         if response.ok:
             tracking_endpoint = self._trackingMap
             responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": feature_name, "message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
+            tracking_payload = {
+                "publicKey": self._getPublicKey(),
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": feature_name,
+                "message": responseTime}
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
         else:
             tracking_endpoint = self._trackingMap
             responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": feature_name + "-error", "message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
+            tracking_payload = {
+                "publicKey": self._getPublicKey(),
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": feature_name + "-error",
+                "message": responseTime}
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
 
         try:
             responseJson = response.json()
         except ValueError:
             raise ServerError(response)
-        
+
         if responseJson.get("status", None) == "error":
             raise RefundError(responseJson.get("message", None))
         elif responseJson.get("status", None) == "success":
             return True, responseJson.get("data", None)
 
         # responseJson =response.json()
         # return responseJson.get("data", None)
-        
-
-
```

### Comparing `rave_python-1.2.9/rave_python/rave_paymentplan.py` & `rave_python-1.4.0/rave_python/rave_paymentplan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,106 +1,152 @@
-import requests, json, copy
+import requests
+import json
+import copy
 from rave_python.rave_base import RaveBase
 from rave_python.rave_misc import checkIfParametersAreComplete, generateTransactionReference
-from rave_python.rave_exceptions import  ServerError, IncompletePaymentDetailsError, PlanCreationError, PlanStatusError
+from rave_python.rave_exceptions import ServerError, IncompletePaymentDetailsError, PlanCreationError, PlanStatusError
 
-class PaymentPlan(RaveBase) :
+
+class PaymentPlan(RaveBase):
     def __init__(self, publicKey, secretKey, production, usingEnv):
         self.headers = {
             'content-type': 'application/json'
         }
-        super(PaymentPlan, self).__init__(publicKey, secretKey, production, usingEnv)
-    
+        super(
+            PaymentPlan,
+            self).__init__(
+            publicKey,
+            secretKey,
+            production,
+            usingEnv)
+
     def _preliminaryResponseChecks(self, response, TypeOfErrorToRaise, name):
         # Check if we can obtain a json
-        
+
         try:
             responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "name": name, "errMsg": response})
+        except BaseException:
+            raise ServerError(
+                {"error": True, "name": name, "errMsg": response})
 
         # Check if the response contains data parameter
         if not responseJson.get("data", None):
-            raise TypeOfErrorToRaise({"error": True, "name": name, "errMsg": responseJson.get("message", "Server is down")})
-        
+            raise TypeOfErrorToRaise({"error": True,
+                                      "name": name,
+                                      "errMsg": responseJson.get("message",
+                                                                 "Server is down")})
+
         # Check if it is returning a 200
         if not response.ok:
             errMsg = responseJson["data"].get("message", None)
             raise TypeOfErrorToRaise({"error": True, "errMsg": errMsg})
-        
+
         return responseJson
-    
+
     def _handleCreateResponse(self, response, planDetails):
-        responseJson = self._preliminaryResponseChecks(response, PlanCreationError, planDetails["name"])
-        
+        responseJson = self._preliminaryResponseChecks(
+            response, PlanCreationError, planDetails["name"])
+
         if responseJson["status"] == "success":
-            return {"error": False, "id": responseJson["data"].get("id", None), "data": responseJson["data"]}
-        
+            return {
+                "error": False,
+                "id": responseJson["data"].get(
+                    "id",
+                    None),
+                "data": responseJson["data"]}
+
         else:
-            raise PlanCreationError({"error": True, "data": responseJson["data"]})
+            raise PlanCreationError(
+                {"error": True, "data": responseJson["data"]})
 
-    # This makes and handles all requests pertaining to the status of your payment plans
-    def _handlePlanStatusRequests(self, type, endpoint, isPostRequest=False, data=None):
+    # This makes and handles all requests pertaining to the status of your
+    # payment plans
+    def _handlePlanStatusRequests(
+            self,
+            type,
+            endpoint,
+            isPostRequest=False,
+            data=None):
 
         # Checks if it is a post request
         if isPostRequest:
-            response = requests.post(endpoint, headers=self.headers, data=json.dumps(data))
+            response = requests.post(
+                endpoint,
+                headers=self.headers,
+                data=json.dumps(data))
         else:
             response = requests.get(endpoint, headers=self.headers)
         # Checks if it can be parsed to json
         try:
             responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "errMsg": response.text })
+        except BaseException:
+            raise ServerError({"error": True, "errMsg": response.text})
 
         # Checks if it returns a 2xx code
         if response.ok:
             return {"error": False, "returnedData": responseJson}
         else:
-            raise PlanStatusError(type, {"error": True, "returnedData": responseJson })
-    
-    #function to create a payment plan
-    #Params: planDetails - a dict containing amount, name, interval, duration
-    #if duration is not passed, any subscribed customer will be charged #indefinitely
+            raise PlanStatusError(
+                type, {"error": True, "returnedData": responseJson})
+
+    # function to create a payment plan
+    # Params: planDetails - a dict containing amount, name, interval, duration
+    # if duration is not passed, any subscribed customer will be charged
+    # #indefinitely
     def create(self, planDetails):
-        # Performing shallow copy of planDetails to avoid public exposing payload with secret key
+        # Performing shallow copy of planDetails to avoid public exposing
+        # payload with secret key
         planDetails = copy.copy(planDetails)
         planDetails.update({"seckey": self._getSecretKey()})
 
         requiredParameters = ["amount", "name", "interval"]
         checkIfParametersAreComplete(requiredParameters, planDetails)
 
         endpoint = self._baseUrl + self._endpointMap["payment_plan"]["create"]
-        response = requests.post(endpoint, headers=self.headers, data=json.dumps(planDetails))
+        response = requests.post(
+            endpoint,
+            headers=self.headers,
+            data=json.dumps(planDetails))
         return self._handleCreateResponse(response, planDetails)
 
-    #gets all payment plans connected to a merchant's account
+    # gets all payment plans connected to a merchant's account
     def all(self):
-        endpoint = self._baseUrl + self._endpointMap["payment_plan"]["list"] + "?seckey="+self._getSecretKey()
+        endpoint = self._baseUrl + \
+            self._endpointMap["payment_plan"]["list"] + "?seckey=" + self._getSecretKey()
         return self._handlePlanStatusRequests("List", endpoint)
-    
+
     def fetch(self, plan_id=None, plan_name=None):
         if plan_id:
-            endpoint = self._baseUrl + self._endpointMap["payment_plan"]["fetch"] + "?seckey="+self._getSecretKey() + "&id="+str(plan_id)
+            endpoint = self._baseUrl + \
+                self._endpointMap["payment_plan"]["fetch"] + "?seckey=" + self._getSecretKey() + "&id=" + str(plan_id)
         elif plan_name:
-            endpoint = self._baseUrl + self._endpointMap["payment_plan"]["fetch"] + "?seckey="+self._getSecretKey() + "&1="+plan_name
+            endpoint = self._baseUrl + \
+                self._endpointMap["payment_plan"]["fetch"] + "?seckey=" + self._getSecretKey() + "&1=" + plan_name
         else:
             return "You must pass either plan id or plan name in order to fetch a plan's details"
         return self._handlePlanStatusRequests("Fetch", endpoint)
-    
+
     def cancelPlan(self, plan_id):
         if not id:
             return "Plan id was not supplied. Kindly supply one"
-        endpoint = self._baseUrl + self._endpointMap["payment_plan"]["cancel"] + str(plan_id) + "/cancel"
+        endpoint = self._baseUrl + \
+            self._endpointMap["payment_plan"]["cancel"] + str(plan_id) + "/cancel"
         data = {"seckey": self._getSecretKey()}
-        return self._handlePlanStatusRequests("Cancel", endpoint, isPostRequest=True, data=data)
-    
+        return self._handlePlanStatusRequests(
+            "Cancel", endpoint, isPostRequest=True, data=data)
+
     # edits a payment plan
     # Params
     # id: payment plan id *required
-    # newData: dict that contains the information to be updated i.e name and status-cancelled/active
+    # newData: dict that contains the information to be updated i.e name and
+    # status-cancelled/active
     def edit(self, plan_id, newData={}):
         if not id:
             return "Plan id was not supplied. Kindly supply one"
-        endpoint = self._baseUrl + self._endpointMap["payment_plan"]["edit"] + str(plan_id) + "/edit"
-        data = {"seckey": self._getSecretKey(), "name": newData.get("name", None), "status": newData.get("status", None)}
-        return self._handlePlanStatusRequests("Edit", endpoint, isPostRequest=True, data=data)
+        endpoint = self._baseUrl + \
+            self._endpointMap["payment_plan"]["edit"] + str(plan_id) + "/edit"
+        data = {
+            "seckey": self._getSecretKey(), "name": newData.get(
+                "name", None), "status": newData.get(
+                "status", None)}
+        return self._handlePlanStatusRequests(
+            "Edit", endpoint, isPostRequest=True, data=data)
```

### Comparing `rave_python-1.2.9/rave_python/rave_preauth.py` & `rave_python-1.4.0/rave_python/rave_preauth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,111 @@
 import requests
 import json
 from rave_python.rave_exceptions import ServerError, TransactionVerificationError, PreauthCaptureError, PreauthRefundVoidError
 from rave_python.rave_card import Card
 from rave_python.rave_misc import generateTransactionReference
 
+
 class Preauth(Card):
     """ This is the rave object for preauthorized transactions. It contains the following public functions:\n
         .charge -- This is for preauthorising a specified amount\n
         .capture -- This is for capturing a preauthorized amount\n
         .validate -- This is called if further action is required i.e. OTP validation\n
         .verify -- This checks the status of your transaction\n
     """
 
     def __init__(self, publicKey, secretKey, production, usingEnv):
-        super(Preauth, self).__init__(publicKey, secretKey, production, usingEnv)
+        super(
+            Preauth,
+            self).__init__(
+            publicKey,
+            secretKey,
+            production,
+            usingEnv)
 
     # Initiate preauth
     def charge(self, cardDetails, chargeWithToken=False, hasFailed=False):
         """ This is called to initiate the preauth process.\n
              Parameters include:\n
             cardDetails (dict) -- This is a dictionary comprising payload parameters.\n
             hasFailed (bool) -- This indicates whether the request had previously failed for timeout handling
         """
 
         # Add the charge_type
-        cardDetails.update({"charge_type":"preauth"})
+        cardDetails.update({"charge_type": "preauth"})
         if not chargeWithToken:
-            return super(Preauth, self).charge(cardDetails, chargeWithToken=False)
+            return super(
+                Preauth,
+                self).charge(
+                cardDetails,
+                chargeWithToken=False)
         else:
-            return super(Preauth, self).charge(cardDetails, chargeWithToken=True)
-    
+            return super(
+                Preauth,
+                self).charge(
+                cardDetails,
+                chargeWithToken=True)
 
     # capture payment
-    def capture(self, flwRef ):
+
+    def capture(self, flwRef):
         """ This is called to complete the transaction.\n
              Parameters include:
             flwRef (string) -- This is the flutterwave reference you receive from action["flwRef"]
         """
         payload = {
             "SECKEY": self._getSecretKey(),
             "flwRef": flwRef
         }
-        headers ={
-            "Content-Type":"application/json"
+        headers = {
+            "Content-Type": "application/json"
         }
         endpoint = self._baseUrl + self._endpointMap["preauth"]["capture"]
-        response = requests.post(endpoint, headers=headers, data=json.dumps(payload))
+        response = requests.post(
+            endpoint,
+            headers=headers,
+            data=json.dumps(payload))
         return self._handleCaptureResponse(response, '')
-    
 
     def void(self, flwRef):
-        """ This is called to void a transaction.\n 
+        """ This is called to void a transaction.\n
              Parameters include:\n
             flwRef (string) -- This is the flutterwave reference you receive from action["flwRef"]\n
         """
         payload = {
             "SECKEY": self._getSecretKey(),
             "ref": flwRef,
-            "action":"void"
+            "action": "void"
         }
-        headers ={
-            "Content-Type":"application/json"
+        headers = {
+            "Content-Type": "application/json"
         }
         endpoint = self._baseUrl + self._endpointMap["preauth"]["refundorvoid"]
-        response = requests.post(endpoint, headers=headers, data=json.dumps(payload))
+        response = requests.post(
+            endpoint,
+            headers=headers,
+            data=json.dumps(payload))
         return self._handleRefundorVoidResponse(response, endpoint)
-    
-    
+
     def refund(self, flwRef, amount=None):
         """ This is called to refund the transaction.\n
              Parameters include:\n
             flwRef (string) -- This is the flutterwave reference you receive from action["flwRef"]\n
             amount (Number) -- (optional) This is called if you want a partial refund
         """
         payload = {
             "SECKEY": self._getSecretKey(),
             "ref": flwRef,
-            "action":"refund"
+            "action": "refund"
         }
         if amount:
             payload["amount"] = amount
 
-        headers ={
-            "Content-Type":"application/json"
+        headers = {
+            "Content-Type": "application/json"
         }
         endpoint = self._baseUrl + self._endpointMap["preauth"]["refundorvoid"]
-        response = requests.post(endpoint, headers=headers, data=json.dumps(payload))
+        response = requests.post(
+            endpoint,
+            headers=headers,
+            data=json.dumps(payload))
         return self._handleRefundorVoidResponse(response, endpoint)
```

### Comparing `rave_python-1.2.9/rave_python/rave_recepient.py` & `rave_python-1.4.0/rave_python/rave_settlement.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,93 @@
-import json, requests, copy
+import json
+import requests
+import copy
 from rave_python.rave_base import RaveBase
 from rave_python.rave_misc import checkIfParametersAreComplete
-from rave_python.rave_exceptions import ServerError, IncompleteCardDetailsError, RecepientCreationError, RecepientStatusError
+from rave_python.rave_exceptions import ServerError, IncompleteCardDetailsError, CardCreationError, CardStatusError
 
-class Recepient(RaveBase):
+
+class Settlement(RaveBase):
     def __init__(self, publicKey, secretKey, production, usingEnv):
         self.headers = {
-            'content-type' : 'application/json'
+            'content-type': 'application/json'
         }
-        super(Recepient, self).__init__(publicKey, secretKey, production, usingEnv)
+        super(
+            Settlement,
+            self).__init__(
+            publicKey,
+            secretKey,
+            production,
+            usingEnv)
 
     def _preliminaryResponseChecks(self, response, TypeOfErrorToRaise, name):
-        #check if we can get json
+        # check if we can get json
         try:
             responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "name": name, "errMsg": response})
+        except BaseException:
+            raise ServerError(
+                {"error": True, "name": name, "errMsg": response})
 
-        #check for data parameter in response 
+        # check for data parameter in response
         if not responseJson.get("data", None):
-            raise TypeOfErrorToRaise({"error": True, "name": name, "errMsg": responseJson.get("message", "Server is down")})
+            raise TypeOfErrorToRaise({"error": True,
+                                      "name": name,
+                                      "errMsg": responseJson.get("message",
+                                                                 "Server is down")})
 
-        #check for 200 response
+        # check for 200 response
         if not response.ok:
             errMsg = response["data"].get("message", None)
             raise TypeOfErrorToRaise({"error": True, "errMsg": errMsg})
 
         return responseJson
 
-    def _handleCreateResponse(self, response, details):
-        responseJson = self._preliminaryResponseChecks(response, RecepientCreationError, details["account_number"])
-
-        if responseJson["status"] == "success":
-            return {"error": False, "id": responseJson["data"].get("id", None), "data": responseJson["data"] }
-
-        else:
-            raise RecepientCreationError({"error": True, "data": responseJson["data"]})
+    # def _handleCreateResponse(self, response, details):
+    #     responseJson = self._preliminaryResponseChecks(response, CardCreationError, details["billing_name"])
 
-    def _handleCardStatusRequests(self, type, endpoint, isPostRequest=False, data=None):
-        #check if resposnse is a post response
+    #     if responseJson["status"] == "success":
+    # return {"error": False, "id": responseJson["data"].get("id", None),
+    # "data": responseJson["data"] }
+
+    #     else:
+    #         raise CardCreationError({"error": True, "data": responseJson["data"]})
+
+    def _handleCardStatusRequests(
+            self,
+            type,
+            endpoint,
+            isPostRequest=False,
+            data=None):
+        # check if response is a post response
         if isPostRequest:
-            response = requests.post(endpoint, headers=self.headers, data=json.dumps(data))
+            response = requests.post(
+                endpoint,
+                headers=self.headers,
+                data=json.dumps(data))
         else:
             response = requests.get(endpoint, headers=self.headers)
-        
-        #check if it can be parsed to JSON
+
+        # check if it can be parsed to JSON
         try:
             responseJson = response.json()
-        except:
+        except BaseException:
             raise ServerError({"error": True, "errMsg": response.text})
 
         if response.ok:
             return {"error": False, "returnedData": responseJson}
         else:
-            raise RecepientStatusError(type, {"error": True, "returnedData": responseJson })
+            raise CardStatusError(
+                type, {"error": True, "returnedData": responseJson})
 
-    #function to create a beneficiary or transfer recepient 
-    #Params: details - a dict containing currency, amount,
-    def create(self, details):
-        details = copy.copy(details)
-        details.update({"seckey": self._getSecretKey()})
-        
-        requiredParameters = ["account_number", "account_bank"]
-        checkIfParametersAreComplete(requiredParameters, details)
-
-        endpoint = self._baseUrl + self._endpointMap["recepient"]["create"]
-        response = requests.post(endpoint, headers=self.headers, data=json.dumps(details))
-        return self._handleCreateResponse(response, details)
+    # function to list and fetch settlements
+    # Params: details - a dict containing service, service_method,
+    # service_version, service_channel and service_payload
 
     def all(self):
-        endpoint = self._baseUrl + self._endpointMap["recepient"]["list"] + "?seckey=" + self._getSecretKey()
+        endpoint = self._baseUrl + \
+            self._endpointMap["settlements"]["list"] + "?seckey=" + self._getSecretKey()
         return self._handleCardStatusRequests("List", endpoint)
 
-    def fetch(self, recepient_id):
-        endpoint = self._baseUrl + self._endpointMap["recepient"]["fetch"] + "/" + str(recepient_id) + "?seckey="+self._getSecretKey()
+    def fetch(self, settlement_id):
+        endpoint = self._baseUrl + self._endpointMap["settlements"]["fetch"] + str(
+            settlement_id) + "?seckey=" + self._getSecretKey()
         return self._handleCardStatusRequests("Fetch", endpoint)
-
-    def cancel(self, recepient_id):
-        if not recepient_id:
-            return "Recepient id was not supplied. Kindly supply one"
-        endpoint = self._baseUrl + self._endpointMap["recepient"]["delete"]
-        data = {
-            "seckey": self._getSecretKey(),
-            "id": recepient_id,
-        }
-        return self._handleCardStatusRequests("Cancel", endpoint, isPostRequest=True, data=data)
-
-
```

### Comparing `rave_python-1.2.9/rave_python/rave_recipient.py` & `rave_python-1.4.0/rave_python/rave_recepient.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,89 +1,122 @@
-import json, requests, copy
+import json
+import requests
+import copy
 from rave_python.rave_base import RaveBase
 from rave_python.rave_misc import checkIfParametersAreComplete
-from rave_python.rave_exceptions import ServerError, IncompleteCardDetailsError, RecipientCreationError, RecipientStatusError
+from rave_python.rave_exceptions import ServerError, IncompleteCardDetailsError, RecepientCreationError, RecepientStatusError
 
-class Recipient(RaveBase):
+
+class Recepient(RaveBase):
     def __init__(self, publicKey, secretKey, production, usingEnv):
         self.headers = {
-            'content-type' : 'application/json'
+            'content-type': 'application/json'
         }
-        super(Recipient, self).__init__(publicKey, secretKey, production, usingEnv)
+        super(
+            Recepient,
+            self).__init__(
+            publicKey,
+            secretKey,
+            production,
+            usingEnv)
 
     def _preliminaryResponseChecks(self, response, TypeOfErrorToRaise, name):
-        #check if we can get json
+        # check if we can get json
         try:
             responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "name": name, "errMsg": response})
+        except BaseException:
+            raise ServerError(
+                {"error": True, "name": name, "errMsg": response})
 
-        #check for data parameter in response 
+        # check for data parameter in response
         if not responseJson.get("data", None):
-            raise TypeOfErrorToRaise({"error": True, "name": name, "errMsg": responseJson.get("message", "Server is down")})
+            raise TypeOfErrorToRaise({"error": True,
+                                      "name": name,
+                                      "errMsg": responseJson.get("message",
+                                                                 "Server is down")})
 
-        #check for 200 response
+        # check for 200 response
         if not response.ok:
             errMsg = response["data"].get("message", None)
             raise TypeOfErrorToRaise({"error": True, "errMsg": errMsg})
 
         return responseJson
 
     def _handleCreateResponse(self, response, details):
-        responseJson = self._preliminaryResponseChecks(response, RecipientCreationError, details["account_number"])
+        responseJson = self._preliminaryResponseChecks(
+            response, RecepientCreationError, details["account_number"])
 
         if responseJson["status"] == "success":
-            return {"error": False, "id": responseJson["data"].get("id", None), "data": responseJson["data"] }
+            return {
+                "error": False,
+                "id": responseJson["data"].get(
+                    "id",
+                    None),
+                "data": responseJson["data"]}
 
         else:
-            raise RecipientCreationError({"error": True, "data": responseJson["data"]})
+            raise RecepientCreationError(
+                {"error": True, "data": responseJson["data"]})
 
-    def _handleCardStatusRequests(self, type, endpoint, isPostRequest=False, data=None):
-        #check if resposnse is a post response
+    def _handleCardStatusRequests(
+            self,
+            type,
+            endpoint,
+            isPostRequest=False,
+            data=None):
+        # check if resposnse is a post response
         if isPostRequest:
-            response = requests.post(endpoint, headers=self.headers, data=json.dumps(data))
+            response = requests.post(
+                endpoint,
+                headers=self.headers,
+                data=json.dumps(data))
         else:
             response = requests.get(endpoint, headers=self.headers)
-        
-        #check if it can be parsed to JSON
+
+        # check if it can be parsed to JSON
         try:
             responseJson = response.json()
-        except:
+        except BaseException:
             raise ServerError({"error": True, "errMsg": response.text})
 
         if response.ok:
             return {"error": False, "returnedData": responseJson}
         else:
-            raise RecipientStatusError(type, {"error": True, "returnedData": responseJson })
+            raise RecepientStatusError(
+                type, {"error": True, "returnedData": responseJson})
 
-    #function to create a beneficiary or transfer recipient 
-    #Params: details - a dict containing currency, amount,
+    # function to create a beneficiary or transfer recepient
+    # Params: details - a dict containing currency, amount,
     def create(self, details):
         details = copy.copy(details)
         details.update({"seckey": self._getSecretKey()})
-        
+
         requiredParameters = ["account_number", "account_bank"]
         checkIfParametersAreComplete(requiredParameters, details)
 
-        endpoint = self._baseUrl + self._endpointMap["recipient"]["create"]
-        response = requests.post(endpoint, headers=self.headers, data=json.dumps(details))
+        endpoint = self._baseUrl + self._endpointMap["recepient"]["create"]
+        response = requests.post(
+            endpoint,
+            headers=self.headers,
+            data=json.dumps(details))
         return self._handleCreateResponse(response, details)
 
     def all(self):
-        endpoint = self._baseUrl + self._endpointMap["recipient"]["list"] + "?seckey=" + self._getSecretKey()
+        endpoint = self._baseUrl + \
+            self._endpointMap["recepient"]["list"] + "?seckey=" + self._getSecretKey()
         return self._handleCardStatusRequests("List", endpoint)
 
-    def fetch(self, recipient_id):
-        endpoint = self._baseUrl + self._endpointMap["recipient"]["fetch"] + "/" + str(recipient_id) + "?seckey="+self._getSecretKey()
+    def fetch(self, recepient_id):
+        endpoint = self._baseUrl + self._endpointMap["recepient"]["fetch"] + "/" + str(
+            recepient_id) + "?seckey=" + self._getSecretKey()
         return self._handleCardStatusRequests("Fetch", endpoint)
 
-    def cancel(self, recipient_id):
-        if not recipient_id:
-            return "recipient id was not supplied. Kindly supply one"
-        endpoint = self._baseUrl + self._endpointMap["recipient"]["delete"]
+    def cancel(self, recepient_id):
+        if not recepient_id:
+            return "Recepient id was not supplied. Kindly supply one"
+        endpoint = self._baseUrl + self._endpointMap["recepient"]["delete"]
         data = {
             "seckey": self._getSecretKey(),
-            "id": recipient_id,
+            "id": recepient_id,
         }
-        return self._handleCardStatusRequests("Cancel", endpoint, isPostRequest=True, data=data)
-
-    
+        return self._handleCardStatusRequests(
+            "Cancel", endpoint, isPostRequest=True, data=data)
```

### Comparing `rave_python-1.2.9/rave_python/rave_rwmobile.py` & `rave_python-1.4.0/rave_python/rave_zbmobile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,67 @@
 from rave_python.rave_payment import Payment
 from rave_python.rave_misc import generateTransactionReference
-import json, requests
+import json
+import requests
 
-class RWMobile(Payment):
-    
-    def __init__(self, publicKey, secretKey, production, usingEnv):
-        super(RWMobile, self).__init__(publicKey, secretKey, production, usingEnv)
 
+class ZBMobile(Payment):
+
+    def __init__(self, publicKey, secretKey, production, usingEnv):
+        super(
+            ZBMobile,
+            self).__init__(
+            publicKey,
+            secretKey,
+            production,
+            usingEnv)
 
     # Charge mobile money function
+
     def charge(self, accountDetails, hasFailed=False):
-        
-        """ This is the RWMobile charge call.
+        """ This is the ghMobile charge call.
              Parameters include:\n
             accountDetails (dict) -- These are the parameters passed to the function for processing\n
             hasFailed (boolean) -- This is a flag to determine if the attempt had previously failed due to a timeout\n
         """
-
-        #feature logic
-        feature_name = "Initiate-Rwanda-mobile-money-charge" 
+        feature_name = "Zambia-MoMo-charge"
         endpoint = self._baseUrl + self._endpointMap["account"]["charge"]
-        
+
         # It is faster to add boilerplate than to check if each one is present
-        accountDetails.update({"payment_type": "mobilemoneygh", "country":"NG", "is_mobile_money_gh":"1", "currency":"RWF", "network": "RWF"})
-        # If transaction reference is not set 
-        
+        accountDetails.update({"payment_type": "mobilemoneyzambia",
+                               "country": "NG",
+                               "is_mobile_money_ug": "1",
+                               "currency": "ZMW"})
+
+        # If transaction reference is not set
         if not ("txRef" in accountDetails):
             accountDetails.update({"txRef": generateTransactionReference()})
+
         # If order reference is not set
-        
         if not ("orderRef" in accountDetails):
             accountDetails.update({"orderRef": generateTransactionReference()})
+
         # Checking for required account components
-        
-        requiredParameters = ["amount", "email", "phonenumber", "network", "IP", "redirect_url"]
-        return super(RWMobile, self).charge(feature_name, accountDetails, requiredParameters, endpoint)
+        requiredParameters = [
+            "amount",
+            "email",
+            "phonenumber",
+            "network",
+            "IP",
+            "redirect_url"]
+        return super(
+            ZBMobile,
+            self).charge(
+            feature_name,
+            accountDetails,
+            requiredParameters,
+            endpoint)
 
     def refund(self, flwRef, amount):
-        feature_name = "Rwanda-mobile-money-charge-refund"
+        feature_name = "Zambia-MoMo-refund"
         endpoint = self._baseUrl + self._endpointMap["refund"]
-        return super(RWMobile, self).refund(feature_name, flwRef, amount)
+        return super(ZBMobile, self).refund(feature_name, flwRef, amount)
 
+    def verify(self, txRef):
+        feature_name = "Zambia-MoMo-verify"
+        endpoint = self._baseUrl + self._endpointMap["verify"]
+        return super(ZBMobile, self).verify(feature_name, txRef)
```

### Comparing `rave_python-1.2.9/rave_python/rave_subaccounts.py` & `rave_python-1.4.0/rave_python/rave_subaccounts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,110 +1,157 @@
-import requests, json, copy
+import requests
+import json
+import copy
 from rave_python.rave_base import RaveBase
 from rave_python.rave_misc import checkIfParametersAreComplete, generateTransactionReference
-from rave_python.rave_exceptions import  ServerError, IncompletePaymentDetailsError, SubaccountCreationError, PlanStatusError
+from rave_python.rave_exceptions import ServerError, IncompletePaymentDetailsError, SubaccountCreationError, PlanStatusError
 
-class SubAccount(RaveBase) :
+
+class SubAccount(RaveBase):
     def __init__(self, publicKey, secretKey, production, usingEnv):
         self.headers = {
             'content-type': 'application/json'
         }
-        super(SubAccount, self).__init__(publicKey, secretKey, production, usingEnv)
-    
+        super(
+            SubAccount,
+            self).__init__(
+            publicKey,
+            secretKey,
+            production,
+            usingEnv)
+
     def _preliminaryResponseChecks(self, response, TypeOfErrorToRaise, name):
         # Check if we can obtain a json
         try:
             responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "name": name, "errMsg": response})
+        except BaseException:
+            raise ServerError(
+                {"error": True, "name": name, "errMsg": response})
 
         # Check if the response contains data parameter
         if not responseJson.get("data", None):
-            raise TypeOfErrorToRaise({"error": True, "name": name, "errMsg": responseJson.get("message", "Server is down")})
-        
+            raise TypeOfErrorToRaise({"error": True,
+                                      "name": name,
+                                      "errMsg": responseJson.get("message",
+                                                                 "Server is down")})
+
         # Check if it is returning a 200
         if not response.ok:
             errMsg = responseJson["data"].get("message", None)
             raise TypeOfErrorToRaise({"error": True, "errMsg": errMsg})
-        
+
         return responseJson
-    
+
     def _handleCreateResponse(self, response, accountDetails):
-        responseJson = self._preliminaryResponseChecks(response, SubaccountCreationError, accountDetails["business_email"])
-        
+        responseJson = self._preliminaryResponseChecks(
+            response, SubaccountCreationError, accountDetails["business_email"])
+
         if responseJson["status"] == "success":
-            return {"error": False, "id": responseJson["data"].get("id", None), "data": responseJson["data"]}
-        
+            return {
+                "error": False,
+                "id": responseJson["data"].get(
+                    "id",
+                    None),
+                "data": responseJson["data"]}
+
         else:
-            raise SubaccountCreationError({"error": True, "data": responseJson["data"]})
+            raise SubaccountCreationError(
+                {"error": True, "data": responseJson["data"]})
 
-    # This makes and handles all requests pertaining to the status of your payment plans
-    def _handleAccountStatusRequests(self, type, endpoint, isPostRequest=False, data=None):
+    # This makes and handles all requests pertaining to the status of your
+    # payment plans
+    def _handleAccountStatusRequests(
+            self,
+            type,
+            endpoint,
+            isPostRequest=False,
+            data=None):
 
         # Checks if it is a post request
         if isPostRequest:
-            response = requests.post(endpoint, headers=self.headers, data=json.dumps(data))
+            response = requests.post(
+                endpoint,
+                headers=self.headers,
+                data=json.dumps(data))
         else:
             response = requests.get(endpoint, headers=self.headers)
 
         # Checks if it can be parsed to json
         try:
             responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "errMsg": response.text })
+        except BaseException:
+            raise ServerError({"error": True, "errMsg": response.text})
 
         # Checks if it returns a 2xx code
         if response.ok:
             return {"error": False, "returnedData": responseJson}
         else:
-            raise PlanStatusError(type, {"error": True, "returnedData": responseJson })
-    
-    #function to create a payment plan
-    #Params: accountDetails - a dict containing account_bank, account_number, business_name, business_email, business_contact, business_contact_mobile, business_mobile, split_type, split_value
-    #if duration is not passed, any subscribed customer will be charged #indefinitely
+            raise PlanStatusError(
+                type, {"error": True, "returnedData": responseJson})
+
+    # function to create a payment plan
+    # Params: accountDetails - a dict containing account_bank, account_number, business_name, business_email, business_contact, business_contact_mobile, business_mobile, split_type, split_value
+    # if duration is not passed, any subscribed customer will be charged
+    # #indefinitely
     def create(self, accountDetails):
-        # Performing shallow copy of planDetails to avoid public exposing payload with secret key
+        # Performing shallow copy of planDetails to avoid public exposing
+        # payload with secret key
         accountDetails = copy.copy(accountDetails)
         accountDetails.update({"seckey": self._getSecretKey()})
-        requiredParameters = ["account_bank", "account_number", "business_name", "business_email", "business_contact", "business_contact_mobile", "business_mobile", "split_type", "split_value"]
+        requiredParameters = [
+            "account_bank",
+            "account_number",
+            "business_name",
+            "business_email",
+            "business_contact",
+            "business_contact_mobile",
+            "business_mobile",
+            "split_type",
+            "split_value"]
         checkIfParametersAreComplete(requiredParameters, accountDetails)
 
         endpoint = self._baseUrl + self._endpointMap["subaccount"]["create"]
-        response = requests.post(endpoint, headers=self.headers, data=json.dumps(accountDetails))
+        response = requests.post(
+            endpoint,
+            headers=self.headers,
+            data=json.dumps(accountDetails))
         return self._handleCreateResponse(response, accountDetails)
 
-    #gets all subaccounts connected to a merchant's account
+    # gets all subaccounts connected to a merchant's account
     def all(self):
-        endpoint = self._baseUrl + self._endpointMap["subaccount"]["list"] + "?seckey="+self._getSecretKey()
+        endpoint = self._baseUrl + \
+            self._endpointMap["subaccount"]["list"] + "?seckey=" + self._getSecretKey()
         return self._handleAccountStatusRequests("List", endpoint)
-    
+
     def fetch(self, subaccount_id):
         if not subaccount_id:
             return "No subaccount id supplied. Kindly pass one in"
-        endpoint = self._baseUrl + self._endpointMap["subaccount"]["fetch"] + "/" +str(subaccount_id) + "?seckey="+self._getSecretKey()
+        endpoint = self._baseUrl + self._endpointMap["subaccount"]["fetch"] + "/" + str(
+            subaccount_id) + "?seckey=" + self._getSecretKey()
         return self._handleAccountStatusRequests("Fetch", endpoint)
 
     def edit(self, Subaccount_id, newData={}):
         if not id:
             return "Plan id was not supplied. Kindly supply one"
         endpoint = self._baseUrl + self._endpointMap["subaccount"]["update"]
         data = {
-            "seckey": self._getSecretKey(), 
-            "account_number": newData.get("account_number", None), 
+            "seckey": self._getSecretKey(),
+            "account_number": newData.get("account_number", None),
             "account_bank": newData.get("account_bank", None),
             "business_name": newData.get("business_name", None),
             "business_email": newData.get("business_email", None),
             "split_type": newData.get("split_type", None),
             "split_value": newData.get("split_value", None),
-            }
-        return self._handlePlanStatusRequests("Edit", endpoint, isPostRequest=True, data=data)
-    
+        }
+        return self._handlePlanStatusRequests(
+            "Edit", endpoint, isPostRequest=True, data=data)
+
     def cancel(self, subaccount_id):
         if not subbacount_id:
             return "Subaccount id was not supplied. Kindly supply one"
         endpoint = self._baseUrl + self._endpointMap["subaccount"]["delete"]
         data = {
             "seckey": self._getSecretKey(),
             "id": subaccount_id,
-            }
-        return self._handlePlanStatusRequests("Cancel", endpoint, isPostRequest=True, data=data)
-    
+        }
+        return self._handlePlanStatusRequests(
+            "Cancel", endpoint, isPostRequest=True, data=data)
```

### Comparing `rave_python-1.2.9/rave_python/rave_subscription.py` & `rave_python-1.4.0/rave_python/rave_subscription.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,82 +1,112 @@
-import requests, json, copy
+import requests
+import json
+import copy
 from rave_python.rave_base import RaveBase
 from rave_python.rave_misc import checkIfParametersAreComplete, generateTransactionReference
-from rave_python.rave_exceptions import  ServerError, IncompletePaymentDetailsError, PlanCreationError, PlanStatusError
+from rave_python.rave_exceptions import ServerError, IncompletePaymentDetailsError, PlanCreationError, PlanStatusError
 
-class Subscriptions(RaveBase) :
+
+class Subscriptions(RaveBase):
     def __init__(self, publicKey, secretKey, production, usingEnv):
         self.headers = {
             'content-type': 'application/json'
         }
-        super(Subscriptions, self).__init__(publicKey, secretKey, production, usingEnv)
-    
+        super(
+            Subscriptions,
+            self).__init__(
+            publicKey,
+            secretKey,
+            production,
+            usingEnv)
+
     def _preliminaryResponseChecks(self, response, TypeOfErrorToRaise, name):
         # Check if we can obtain a json
         try:
             responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "name": name, "errMsg": response})
+        except BaseException:
+            raise ServerError(
+                {"error": True, "name": name, "errMsg": response})
 
         # Check if the response contains data parameter
         if not responseJson.get("data", None):
-            raise TypeOfErrorToRaise({"error": True, "name": name, "errMsg": responseJson.get("message", "Server is down")})
-        
+            raise TypeOfErrorToRaise({"error": True,
+                                      "name": name,
+                                      "errMsg": responseJson.get("message",
+                                                                 "Server is down")})
+
         # Check if it is returning a 200
         if not response.ok:
             errMsg = responseJson["data"].get("message", None)
             raise TypeOfErrorToRaise({"error": True, "errMsg": errMsg})
-        
+
         return responseJson
-        
-    
-    # This makes and handles all requests pertaining to the status of your payment plans
-    def _handlePlanStatusRequests(self, type, endpoint, isPostRequest=False, data=None):
+
+    # This makes and handles all requests pertaining to the status of your
+    # payment plans
+
+    def _handlePlanStatusRequests(
+            self,
+            type,
+            endpoint,
+            isPostRequest=False,
+            data=None):
 
         # Checks if it is a post request
         if isPostRequest:
-            response = requests.post(endpoint, headers=self.headers, data=json.dumps(data))
+            response = requests.post(
+                endpoint,
+                headers=self.headers,
+                data=json.dumps(data))
         else:
             response = requests.get(endpoint, headers=self.headers)
-    
+
         # Checks if it can be parsed to json
         try:
             responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "errMsg": response.text })
+        except BaseException:
+            raise ServerError({"error": True, "errMsg": response.text})
 
         # Checks if it returns a 2xx code
         if response.ok:
             return {"error": False, "returnedData": responseJson}
         else:
-            raise PlanStatusError(type, {"error": True, "returnedData": str(responseJson) })
+            raise PlanStatusError(
+                type, {"error": True, "returnedData": str(responseJson)})
 
-    #gets all subscriptions connected to a merchant's account
+    # gets all subscriptions connected to a merchant's account
     def all(self):
-        endpoint = self._baseUrl + self._endpointMap["subscriptions"]["list"] + "?seckey="+self._getSecretKey()
+        endpoint = self._baseUrl + \
+            self._endpointMap["subscriptions"]["list"] + "?seckey=" + self._getSecretKey()
         return self._handlePlanStatusRequests("List", endpoint)
-    
+
     def fetch(self, subscription_id=None, subscription_email=None):
         if subscription_id:
-            endpoint = self._baseUrl + self._endpointMap["subscriptions"]["fetch"] + "?seckey="+self._getSecretKey() + "&id="+str(subscription_id)
+            endpoint = self._baseUrl + self._endpointMap["subscriptions"]["fetch"] + \
+                "?seckey=" + self._getSecretKey() + "&id=" + str(subscription_id)
         elif subscription_email:
-            endpoint = self._baseUrl + self._endpointMap["subscriptions"]["fetch"] + "?seckey="+self._getSecretKey() + "&1="+subscription_email
+            endpoint = self._baseUrl + \
+                self._endpointMap["subscriptions"]["fetch"] + "?seckey=" + self._getSecretKey() + "&1=" + subscription_email
         else:
             return "You must pass either plan id or plan name in order to fetch a plan's details"
         return self._handlePlanStatusRequests("Fetch", endpoint)
-    
+
     def cancel(self, subscription_id):
         if not subscription_id:
             return "Subscription id was not supplied. Kindly supply one"
-        endpoint = self._baseUrl + self._endpointMap["subscriptions"]["cancel"] + str(subscription_id) + "/cancel"
+        endpoint = self._baseUrl + \
+            self._endpointMap["subscriptions"]["cancel"] + str(subscription_id) + "/cancel"
         data = {"seckey": self._getSecretKey()}
-        return self._handlePlanStatusRequests("Cancel", endpoint, isPostRequest=True, data=data)
-    
+        return self._handlePlanStatusRequests(
+            "Cancel", endpoint, isPostRequest=True, data=data)
+
     # activates a subscription plan
     # Params
     # id: subscription_id *required
     def activate(self, subscription_id):
         if not subscription_id:
             return "Subscription id was not supplied. Kindly supply one"
-        endpoint = self._baseUrl + self._endpointMap["subscriptions"]["activate"] + str(subscription_id) + "/activate"
+        endpoint = self._baseUrl + \
+            self._endpointMap["subscriptions"]["activate"] + str(subscription_id) + "/activate"
         data = {"seckey": self._getSecretKey()}
-        return self._handlePlanStatusRequests("Activat", endpoint, isPostRequest=True, data=data)
+        return self._handlePlanStatusRequests(
+            "Activat", endpoint, isPostRequest=True, data=data)
```

### Comparing `rave_python-1.2.9/rave_python/rave_transfer.py` & `rave_python-1.4.0/rave_python/rave_virtualcard.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,195 +1,255 @@
-import requests, json, copy
+import json
+import requests
+import copy
 from rave_python.rave_base import RaveBase
-from rave_python.rave_misc import checkIfParametersAreComplete, generateTransactionReference, checkTransferParameters
-from rave_python.rave_exceptions import InitiateTransferError, ServerError, TransferFetchError, IncompletePaymentDetailsError
+from rave_python.rave_misc import checkIfParametersAreComplete
+from rave_python.rave_exceptions import ServerError, IncompleteCardDetailsError, CardCreationError, CardStatusError
 
 
-class Transfer(RaveBase):
+class VirtualCard(RaveBase):
     def __init__(self, publicKey, secretKey, production, usingEnv):
-        super(Transfer, self).__init__(publicKey, secretKey, production, usingEnv)
-    
-    def _preliminaryResponseChecks(self, response, TypeOfErrorToRaise, reference):
-        # Check if we can obtain a json
+        self.headers = {
+            'content-type': 'application/json'
+        }
+        super(
+            VirtualCard,
+            self).__init__(
+            publicKey,
+            secretKey,
+            production,
+            usingEnv)
+
+    def _preliminaryResponseChecks(self, response, TypeOfErrorToRaise, name):
+        # check if we can get json
         try:
             responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "reference": reference, "errMsg": response})
+        except BaseException:
+            raise ServerError(
+                {"error": True, "name": name, "errMsg": response})
 
-        # Check if the response contains data parameter
+        # check for data parameter in response
         if not responseJson.get("data", None):
-            raise TypeOfErrorToRaise({"error": True, "reference": reference, "errMsg": responseJson.get("message", "Server is down")})
-        
-        # Check if it is returning a 200
+            raise TypeOfErrorToRaise({"error": True,
+                                      "name": name,
+                                      "errMsg": responseJson.get("message",
+                                                                 "Server is down")})
+
+        # check for 200 response
         if not response.ok:
-            errMsg = responseJson["data"].get("message", None)
+            errMsg = response["data"].get("message", None)
             raise TypeOfErrorToRaise({"error": True, "errMsg": errMsg})
 
         return responseJson
 
-
-    def _handleInitiateResponse(self, response, transferDetails):
-        responseJson = self._preliminaryResponseChecks(response, InitiateTransferError, transferDetails["reference"])
-        
-        if responseJson["status"] == "success":
-            return {"error": False, "id": responseJson["data"].get("id", None), "data": responseJson["data"]}
-        
-        else:
-            raise InitiateTransferError({"error": True, "data": responseJson["data"]})
-
-    def _handleBulkResponse(self, response, bulkDetails):
-        responseJson = self._preliminaryResponseChecks(response, InitiateTransferError, None)
+    def _handleCreateResponse(self, response, vcardDetails):
+        responseJson = self._preliminaryResponseChecks(
+            response, CardCreationError, vcardDetails["billing_name"])
 
         if responseJson["status"] == "success":
-            return {"error": False, "status": responseJson["status"], "message":responseJson["message"], "id": responseJson["data"].get("id", None), "data": responseJson["data"]}
+            return {
+                "error": False,
+                "id": responseJson["data"].get(
+                    "id",
+                    None),
+                "data": responseJson["data"]}
+
+        else:
+            raise CardCreationError(
+                {"error": True, "data": responseJson["data"]})
+
+    def _handleCardStatusRequests(
+            self,
+            type,
+            endpoint,
+            feature_name,
+            isPostRequest=False,
+            data=None):
+        # check if response is a post response
+        if isPostRequest:
+            response = requests.post(
+                endpoint,
+                headers=self.headers,
+                data=json.dumps(data))
         else:
-            raise InitiateTransferError({"error": True, "data": responseJson["data"]})
-
-            
-    def initiate(self, transferDetails):
-        
-        
-        ## feature logic
-        # Performing shallow copy of transferDetails to avoid public exposing payload with secret key
-        transferDetails = copy.copy(transferDetails)
-        
-        # adding reference if not already included
-        if not ("reference" in transferDetails):
-            transferDetails.update({"reference": generateTransactionReference()})
-        transferDetails.update({"seckey": self._getSecretKey()})
-        
-        # These are the parameters required to initiate a transfer
-        requiredParameters = ["amount", "currency","beneficiary_name"]
-        checkIfParametersAreComplete(requiredParameters, transferDetails)
-        checkTransferParameters(requiredParameters, transferDetails)
-        
-        # Collating request headers
-        headers = {
-            'content-type': 'application/json',
-        }
+            response = requests.get(endpoint, headers=self.headers)
 
-        endpoint = self._baseUrl + self._endpointMap["transfer"]["initiate"]
-        response = requests.post(endpoint, headers=headers, data=json.dumps(transferDetails))
+        # check if it can be parsed to JSON
+        try:
+            responseJson = response.json()
+        except BaseException:
+            raise ServerError({"error": True, "errMsg": response.text})
 
-        if response.ok == False:
-            #feature logging
+        if response.ok:
+            # feature logging
             tracking_endpoint = self._trackingMap
             responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": "Initiate-Transfer-error","message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
+            tracking_payload = {
+                "publicKey": self._getPublicKey(),
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": feature_name,
+                "message": responseTime}
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
+
+            return {"error": False, "returnedData": responseJson}
         else:
             tracking_endpoint = self._trackingMap
             responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": "Initiate-Transfer","message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
-        return self._handleInitiateResponse(response, transferDetails)
-
-
-
-    def bulk(self, bulkDetails):
-        
-        # feature logic
-        bulkDetails = copy.copy(bulkDetails)
-        
-        # Collating request headers
-        headers = {
-            'content-type': 'application/json',
-        }
+            tracking_payload = {
+                "publicKey": self._getPublicKey(),
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": feature_name + "-error",
+                "message": responseTime}
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
+
+            raise CardStatusError(
+                type, {"error": True, "returnedData": responseJson})
+
+    # function to create a virtual card
+    # Params: vcardDetails - a dict containing currency, amount, billing_name,
+    # billing_address, billing_city, billing_state, billing_postal_code,
+    # billing_country
+
+    def create(self, vcardDetails):
+
+        # card creating logic
+        vcardDetails = copy.copy(vcardDetails)
+        vcardDetails.update({"seckey": self._getSecretKey()})
+        requiredParameters = [
+            "currency",
+            "amount",
+            "billing_name",
+            "billing_address",
+            "billing_city",
+            "billing_state",
+            "billing_postal_code",
+            "billing_country"]
+        checkIfParametersAreComplete(requiredParameters, vcardDetails)
+        endpoint = self._baseUrl + self._endpointMap["virtual_card"]["create"]
+        response = requests.post(
+            endpoint,
+            headers=self.headers,
+            data=json.dumps(vcardDetails))
 
-        bulkDetails.update({"seckey": self._getSecretKey()})
-        requiredParameters = ["title", "bulk_data"]
-        checkIfParametersAreComplete(requiredParameters, bulkDetails)
-        checkTransferParameters(requiredParameters, bulkDetails)
-        endpoint = self._baseUrl + self._endpointMap["transfer"]["bulk"]
-        
-        # Collating request headers
-        headers = {
-            'content-type': 'application/json',
-        }
-        response = requests.post(endpoint, headers=headers, data=json.dumps(bulkDetails))
-        
-        if response.ok == False:
-            #feature logging
+        # feature logging
+        if not response.ok:
             tracking_endpoint = self._trackingMap
             responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": "Initiate-Bulk-error","message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
+            tracking_payload = {
+                "publicKey": self._getPublicKey(),
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": "Create-card-error",
+                "message": responseTime}
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
         else:
             tracking_endpoint = self._trackingMap
             responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": "Initiate-Bulk","message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
+            tracking_payload = {
+                "publicKey": self._getPublicKey(),
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": "Create-card",
+                "message": responseTime}
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
 
-        return self._handleBulkResponse(response, bulkDetails)
+        return self._handleCreateResponse(response, vcardDetails)
 
-    
-    # This makes and handles all requests pertaining to the status of your transfer or account
-    def _handleTransferStatusRequests(self, endpoint, feature_name, isPostRequest=False, data=None):
-        
-        # Request headers
-        headers = {
-            'content-type': 'application/json',
-        }
+    # gets all virtual cards connected to a merchant's account
 
-        # Checks if it is a post request
-        if isPostRequest:
-            response = requests.post(endpoint, headers=headers, data=json.dumps(data))
-        else:
-            response = requests.get(endpoint, headers=headers)
+    def all(self):
 
-        # Checks if it can be parsed to json
-        try:
-            responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "errMsg": response.text })
+        # logic for listing all cards
+        label = "List-all-cards"
+        endpoint = self._baseUrl + \
+            self._endpointMap["virtual_card"]["list"] + "?seckey=" + self._getSecretKey()
+        data = {"seckey": self._getSecretKey()}
+        return self._handleCardStatusRequests(
+            "List", endpoint, label, isPostRequest=True, data=data)
+
+    # permanently deletes a card with specified id
+
+    def cancel(self, card_id):
+
+        if not card_id:
+            return "Card id was not supplied. Kindly supply one"
+
+        # card cancel feature logic
+        label = "Delete-card"
+        endpoint = self._baseUrl + \
+            self._endpointMap["virtual_card"]["terminate"] + str(card_id) + "/terminate"
+        data = {"seckey": self._getSecretKey()}
+        return self._handleCardStatusRequests(
+            "Cancel", endpoint, label, isPostRequest=True, data=data)
+
+    # fetches Card details and transactions for a cars with specified id
+
+    def get(self, card_id):
+
+        # fetch card logic
+        label = "Fetch-card"
+        endpoint = self._baseUrl + self._endpointMap["virtual_card"]["get"]
+        data = {"seckey": self._getSecretKey()}
+        return self._handleCardStatusRequests(
+            "Get", endpoint, label, isPostRequest=True, data=data)
 
-        # Checks if it returns a 2xx code
-        if response.ok:
-            tracking_endpoint = self._trackingMap
-            responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": feature_name,"message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
-            return {"error": False, "returnedData": responseJson}
-        else:
-            tracking_endpoint = self._trackingMap
-            responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": feature_name + "-error","message": responseTime}
-            raise TransferFetchError({"error": True, "returnedData": responseJson })
+    # temporarily suspends the use of card
 
-    # Not elegant but supports python 2 and 3
-    def fetch(self, reference=None):
-        
-        #feature logic
-        label = "Fetch-Transfer"
-        endpoint = self._baseUrl + self._endpointMap["transfer"]["fetch"] + "?seckey="+self._getSecretKey()+'&reference='+str(reference)
-        return self._handleTransferStatusRequests(label, endpoint)
+    def freeze(self, card_id):
 
-    def all(self):
-        
-        #feature logic
-        label = "List-all-Transfers"
-        endpoint = self._baseUrl + self._endpointMap["transfer"]["fetch"] + "?seckey="+self._getSecretKey()
-        return self._handleTransferStatusRequests(label, endpoint)
+        # feature logic
+        label = "Block-card"
+        endpoint = self._baseUrl + \
+            self._endpointMap["virtual_card"]["freeze"] + str(card_id) + "/status/block"
+        data = {"seckey": self._getSecretKey()}
+        return self._handleCardStatusRequests(
+            "Freeze", endpoint, label, isPostRequest=True, data=data)
+
+    # reverses the freeze card operation
+
+    def unfreeze(self, card_id):
 
-    def getFee(self, currency=None):
-        
         # feature logic
-        label = "Get-Transfer-fee-by-Currency"
-        endpoint = self._baseUrl + self._endpointMap["transfer"]["fee"] + "?seckey="+self._getSecretKey() + "&currency="+str(currency)
-        return self._handleTransferStatusRequests(label, endpoint)
-        
-    def getBalance(self, currency):
-        
+        label = "Unblock-card"
+        endpoint = self._baseUrl + \
+            self._endpointMap["virtual_card"]["unfreeze"] + str(card_id) + "/status/unblock"
+        data = {"seckey": self._getSecretKey()}
+        return self._handleCardStatusRequests(
+            "Unfreeze", endpoint, label, isPostRequest=True, data=data)
+
+    # funds a card with specified balance for online transactions
+
+    def fund(self, card_id, currency, amount):
+
         # feature logic
-        label = "Get-Balance-fee-by-Currency"
-        if not currency: # i made currency compulsory because if it is not assed in, an error message is returned from the server
-            raise IncompletePaymentDetailsError("currency", ["currency"])
-        endpoint =  self._baseUrl + self._endpointMap["transfer"]["balance"] 
         data = {
+            "card_id": card_id,
+            "amount": amount,
+            "debit_currency": currency,
             "seckey": self._getSecretKey(),
-            "currency": currency
         }
+        label = "Fund-card"
+        endpoint = self._baseUrl + self._endpointMap["virtual_card"]["fund"]
+        return self._handleCardStatusRequests(
+            "Fund", endpoint, label, isPostRequest=True, data=data)
+
+    # withdraws funds from Virtual card. Withdrawn funds are added to Rave
+    # Balance
+    def withdraw(self, card_id, amount):
 
-        return self._handleTransferStatusRequests(label, endpoint, data=data, isPostRequest=True)
-
-    
-
+        # feature logic
+        data = {
+            "card_id": card_id,
+            "amount": amount,
+            "seckey": self._getSecretKey(),
+        }
+        label = "Withdraw-card-funds"
+        endpoint = self._baseUrl + \
+            self._endpointMap["virtual_card"]["withdraw"]
+        return self._handleCardStatusRequests(
+            "Fund", endpoint, label, isPostRequest=True, data=data)
```

### Comparing `rave_python-1.2.9/rave_python/rave_ugmobile.py` & `rave_python-1.4.0/rave_python/rave_rwmobile.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,70 @@
 from rave_python.rave_payment import Payment
 from rave_python.rave_misc import generateTransactionReference
-import json, requests
+import json
+import requests
+
+
+class RWMobile(Payment):
 
-class UGMobile(Payment):
-    
     def __init__(self, publicKey, secretKey, production, usingEnv):
-        super(UGMobile, self).__init__(publicKey, secretKey, production, usingEnv)
+        super(
+            RWMobile,
+            self).__init__(
+            publicKey,
+            secretKey,
+            production,
+            usingEnv)
 
     # Charge mobile money function
+
     def charge(self, accountDetails, hasFailed=False):
-        
-        """ This is the ghMobile charge call.
+        """ This is the RWMobile charge call.
              Parameters include:\n
             accountDetails (dict) -- These are the parameters passed to the function for processing\n
             hasFailed (boolean) -- This is a flag to determine if the attempt had previously failed due to a timeout\n
         """
-        
-        feature_name = "Initiate-Uganda-mobile-money-charge"
+
+        # feature logic
+        feature_name = "Rwanda-MoMo-charge"
         endpoint = self._baseUrl + self._endpointMap["account"]["charge"]
-        
+
         # It is faster to add boilerplate than to check if each one is present
-        accountDetails.update({"payment_type": "mobilemoneyuganda", "country":"NG", "is_mobile_money_ug":"1", "currency":"UGX", "network": "UGX"})
-        
-        # If transaction reference is not set 
+        accountDetails.update({"payment_type": "mobilemoneygh",
+                               "country": "NG",
+                               "is_mobile_money_gh": "1",
+                               "currency": "RWF",
+                               "network": "RWF"})
+        # If transaction reference is not set
+
         if not ("txRef" in accountDetails):
             accountDetails.update({"txRef": generateTransactionReference()})
-        
         # If order reference is not set
+
         if not ("orderRef" in accountDetails):
             accountDetails.update({"orderRef": generateTransactionReference()})
-        
         # Checking for required account components
-        requiredParameters = ["amount", "email", "phonenumber", "network", "IP"]
-        return super(UGMobile, self).charge(feature_name, accountDetails, requiredParameters, endpoint)
+
+        requiredParameters = [
+            "amount",
+            "email",
+            "phonenumber",
+            "network",
+            "IP",
+            "redirect_url"]
+        return super(
+            RWMobile,
+            self).charge(
+            feature_name,
+            accountDetails,
+            requiredParameters,
+            endpoint)
 
     def refund(self, flwRef, amount):
-        feature_name = "Uganda-mobile-money-charge-refund"
+        feature_name = "Rwanda-MoMo-refund"
         endpoint = self._baseUrl + self._endpointMap["refund"]
-        return super(UGMobile, self).refund(feature_name, flwRef, amount)
+        return super(RWMobile, self).refund(feature_name, flwRef, amount)
 
+    def verify(self, txRef):
+        feature_name = "Rwanda-MoMo-verify"
+        endpoint = self._baseUrl + self._endpointMap["verify"]
+        return super(RWMobile, self).verify(feature_name, txRef)
```

### Comparing `rave_python-1.2.9/rave_python/rave_verify.py` & `rave_python-1.4.0/rave_python/rave_virtualaccount.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,120 @@
-import json, requests, copy
+import json
+import requests
+import copy
 from rave_python.rave_base import RaveBase
 from rave_python.rave_misc import checkIfParametersAreComplete
-from rave_python.rave_exceptions import ServerError, BVNFetchError
+from rave_python.rave_exceptions import ServerError, IncompleteAccountDetailsError, AccountCreationError, AccountStatusError
 
-class Verify(RaveBase):
+
+class VirtualAccount(RaveBase):
     def __init__(self, publicKey, secretKey, production, usingEnv):
-        super(Verify, self).__init__(publicKey, secretKey, production, usingEnv)
+        self.headers = {
+            'content-type': 'application/json'
+        }
+        super(
+            VirtualAccount,
+            self).__init__(
+            publicKey,
+            secretKey,
+            production,
+            usingEnv)
 
     def _preliminaryResponseChecks(self, response, TypeOfErrorToRaise, name):
-        #check if we can get json
+        # check if we can get json
         try:
             responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "name": name, "errMsg": response})
+        except BaseException:
+            raise ServerError(
+                {"error": True, "name": name, "errMsg": response})
 
-        #check for data parameter in response 
+        # check for data parameter in response
         if not responseJson.get("data", None):
-            raise TypeOfErrorToRaise({"error": True, "name": name, "errMsg": responseJson.get("message", "Server is down")})
+            raise TypeOfErrorToRaise({"error": True,
+                                      "name": name,
+                                      "errMsg": responseJson.get("message",
+                                                                 "Server is down")})
 
-        #check for 200 response
+        # check for 200 response
         if not response.ok:
             errMsg = response["data"].get("message", None)
             raise TypeOfErrorToRaise({"error": True, "errMsg": errMsg})
 
         return responseJson
 
-    # def _handleCreateResponse(self, response, details):
-    #     responseJson = self._preliminaryResponseChecks(response, CardCreationError, details["billing_name"])
+    def _handleCreateResponse(self, response, accountDetails):
+        responseJson = self._preliminaryResponseChecks(
+            response, AccountCreationError, accountDetails["email"])
+
+        if responseJson["status"] == "success":
+            return {
+                "error": False,
+                "id": responseJson["data"].get(
+                    "id",
+                    None),
+                "data": responseJson["data"]}
 
-    #     if responseJson["status"] == "success":
-    #         return {"error": False, "id": responseJson["data"].get("id", None), "data": responseJson["data"] }
+        else:
+            raise AccountCreationError(
+                {"error": True, "data": responseJson["data"]})
 
+    # def _handleCardStatusRequests(self, type, endpoint, isPostRequest=False, data=None):
+    #     #check if response is a post response
+    #     if isPostRequest:
+    #         response = requests.post(endpoint, headers=self.headers, data=json.dumps(data))
     #     else:
-    #         raise CardCreationError({"error": True, "data": responseJson["data"]})
+    #         response = requests.get(endpoint, headers=self.headers)
 
-    def _handleVerifyStatusRequests(self, endpoint, feature_name, isPostRequest=False, data=None):
-        self.headers = {
-            'content-type' : 'application/json'
-        }
-        #check if resposnse is a post response
-        if isPostRequest:
-            response = requests.post(endpoint, headers=self.headers, data=json.dumps(data))
-        else:
-            response = requests.get(endpoint, headers=self.headers)
-        
-        #check if it can be parsed to JSON
-        try:
-            responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "errMsg": response.text})
+    #     #check if it can be parsed to JSON
+    #     try:
+    #         responseJson = response.json()
+    #     except:
+    #         raise ServerError({"error": True, "errMsg": response.text})
 
-        if response.ok:
-            #feature logging
+    #     if response.ok:
+    #         return {"error": False, "returnedData": responseJson}
+    #     else:
+    #         raise AccountStatusError(type, {"error": True, "returnedData": responseJson })
+
+    # function to create a virtual card
+    # Params: cardDetails - a dict containing email, is_permanent, frequency,
+    # duration, narration
+
+    def create(self, accountDetails):
+
+        # feature logic
+        accountDetails = copy.copy(accountDetails)
+        accountDetails.update({"seckey": self._getSecretKey()})
+        requiredParameters = ["email", "narration"]
+        checkIfParametersAreComplete(requiredParameters, accountDetails)
+        endpoint = self._baseUrl + \
+            self._endpointMap["virtual_account"]["create"]
+        response = requests.post(
+            endpoint,
+            headers=self.headers,
+            data=json.dumps(accountDetails))
+
+        # feature logging
+        if not response.ok:
             tracking_endpoint = self._trackingMap
             responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": feature_name,"message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
-            return {"error": False, "returnedData": responseJson}
+            tracking_payload = {
+                "publicKey": self._getPublicKey(),
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": "Create-virtual-account-error",
+                "message": responseTime}
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
         else:
             tracking_endpoint = self._trackingMap
             responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": feature_name + "-error", "message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
-
-            raise BVNFetchError({"error": True, "returnedData": responseJson })
+            tracking_payload = {
+                "publicKey": self._getPublicKey(),
+                "language": "Python v2",
+                "version": "1.2.13",
+                "title": "Create-virtual-account",
+                "message": responseTime}
+            tracking_response = requests.post(
+                tracking_endpoint, data=json.dumps(tracking_payload))
 
-    def bvnVerify(self, bvn):
-
-        # feature logic
-        if not bvn:
-            return "BVN was not supplied. Kindly supply one"
-        feature_name = "BVN-verification"
-        endpoint = self._baseUrl + self._endpointMap["bvn"]["verify"] +str(bvn)+"?seckey=" + self._getSecretKey()
-        return self._handleVerifyStatusRequests(endpoint, feature_name)
+        return self._handleCreateResponse(response, accountDetails)
```

### Comparing `rave_python-1.2.9/rave_python/rave_virtualaccount.py` & `rave_python-1.4.0/rave_python/rave_ebills.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,119 @@
-import json, requests, copy
+import json
+import requests
+import copy
 from rave_python.rave_base import RaveBase
 from rave_python.rave_misc import checkIfParametersAreComplete
-from rave_python.rave_exceptions import ServerError, IncompleteAccountDetailsError, AccountCreationError, AccountStatusError
+from rave_python.rave_exceptions import ServerError, IncompleteCardDetailsError, BillCreationError, BillStatusError
 
-class VirtualAccount(RaveBase):
+
+class Ebills(RaveBase):
     def __init__(self, publicKey, secretKey, production, usingEnv):
         self.headers = {
-            'content-type' : 'application/json'
+            'content-type': 'application/json'
         }
-        super(VirtualAccount, self).__init__(publicKey, secretKey, production, usingEnv)
+        super(
+            Ebills,
+            self).__init__(
+            publicKey,
+            secretKey,
+            production,
+            usingEnv)
 
     def _preliminaryResponseChecks(self, response, TypeOfErrorToRaise, name):
-        #check if we can get json
+        # check if we can get json
         try:
             responseJson = response.json()
-        except:
-            raise ServerError({"error": True, "name": name, "errMsg": response})
+        except BaseException:
+            raise ServerError(
+                {"error": True, "name": name, "errMsg": response})
 
-        #check for data parameter in response 
+        # check for data parameter in response
         if not responseJson.get("data", None):
-            raise TypeOfErrorToRaise({"error": True, "name": name, "errMsg": responseJson.get("message", "Server is down")})
+            raise TypeOfErrorToRaise({"error": True,
+                                      "name": name,
+                                      "errMsg": responseJson.get("message",
+                                                                 "Server is down")})
 
-        #check for 200 response
+        # check for 200 response
         if not response.ok:
             errMsg = response["data"].get("message", None)
             raise TypeOfErrorToRaise({"error": True, "errMsg": errMsg})
 
         return responseJson
 
-    def _handleCreateResponse(self, response, accountDetails):
-        responseJson = self._preliminaryResponseChecks(response, AccountCreationError, accountDetails["email"])
+    def _handleCreateResponse(self, response, details):
+        responseJson = self._preliminaryResponseChecks(
+            response, BillCreationError, details["SECKEY"])
 
         if responseJson["status"] == "success":
-            return {"error": False, "id": responseJson["data"].get("id", None), "data": responseJson["data"] }
+            return {
+                "error": False,
+                "id": responseJson["data"].get(
+                    "id",
+                    None),
+                "data": responseJson["data"]}
+
+        else:
+            raise BillCreationError(
+                {"error": True, "data": responseJson["data"]})
 
+    def _handleBillStatusRequests(
+            self,
+            type,
+            endpoint,
+            isPostRequest=False,
+            data=None):
+        # check if resposnse is a post response
+        if isPostRequest:
+            response = requests.post(
+                endpoint,
+                headers=self.headers,
+                data=json.dumps(data))
         else:
-            raise AccountCreationError({"error": True, "data": responseJson["data"]})
+            response = requests.get(endpoint, headers=self.headers)
+
+        # check if it can be parsed to JSON
+        try:
+            responseJson = response.json()
+        except BaseException:
+            raise ServerError({"error": True, "errMsg": response.text})
 
-    # def _handleCardStatusRequests(self, type, endpoint, isPostRequest=False, data=None):
-    #     #check if response is a post response
-    #     if isPostRequest:
-    #         response = requests.post(endpoint, headers=self.headers, data=json.dumps(data))
-    #     else:
-    #         response = requests.get(endpoint, headers=self.headers)
-        
-    #     #check if it can be parsed to JSON
-    #     try:
-    #         responseJson = response.json()
-    #     except:
-    #         raise ServerError({"error": True, "errMsg": response.text})
-
-    #     if response.ok:
-    #         return {"error": False, "returnedData": responseJson}
-    #     else:
-    #         raise AccountStatusError(type, {"error": True, "returnedData": responseJson })
-
-
-    #function to create a virtual card 
-    #Params: cardDetails - a dict containing email, is_permanent, frequency, duration, narration
-    def create(self, accountDetails):
-
-        # feature logic
-        accountDetails = copy.copy(accountDetails)
-        accountDetails.update({"seckey": self._getSecretKey()})
-        requiredParameters = ["email", "narration"]
-        checkIfParametersAreComplete(requiredParameters, accountDetails)
-        endpoint = self._baseUrl + self._endpointMap["virtual_account"]["create"]
-        response = requests.post(endpoint, headers=self.headers, data=json.dumps(accountDetails))
-
-        #feature logging
-        if response.ok == False:
-            tracking_endpoint = self._trackingMap
-            responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": "Create-virtual-account-error","message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
+        if response.ok:
+            return {"error": False, "returnedData": responseJson}
         else:
-            tracking_endpoint = self._trackingMap
-            responseTime = response.elapsed.total_seconds()
-            tracking_payload = {"publicKey": self._getPublicKey(),"language": "Python v2", "version": "1.2.9", "title": "Create-virtual-account","message": responseTime}
-            tracking_response = requests.post(tracking_endpoint, data=json.dumps(tracking_payload))
+            raise BillStatusError(
+                type, {"error": True, "returnedData": responseJson})
 
-        return self._handleCreateResponse(response, accountDetails)
+    # def createOrder(self, order_details):
+    #     # Performing shallow copy of planDetails to avoid public exposing payload with secret key
+    #     order_details = copy.copy(order_details)
+    #     order_details.update({"seckey": self._getSecretKey()})
+
+    #     requiredParameters = ["seckey", "numberofunits", "currency", "amount", "email", "txRef", "country"]
+    #     checkIfParametersAreComplete(requiredParameters, order_details)
+
+    #     endpoint = self._baseUrl + self._endpointMap["ebills"]["create"]
+    #     response = requests.post(endpoint, headers=self.headers, data=json.dumps(order_details))
+    #     return self._handleCreateResponse(response, order_details)
+
+    def create(self, details):
+        # Performing shallow copy of planDetails to avoid public exposing
+        # payload with secret key
+        details = copy.copy(details)
+        details.update({"SECKEY": self._getSecretKey()})
+
+        requiredParameters = [
+            "numberofunits",
+            "currency",
+            "amount",
+            "email",
+            "txRef",
+            "country"]
+        checkIfParametersAreComplete(requiredParameters, details)
+
+        endpoint = self._baseUrl + self._endpointMap["ebills"]["create"]
+        response = requests.post(
+            endpoint,
+            headers=self.headers,
+            data=json.dumps(details))
+        return self._handleCreateResponse(response, details)
```

### Comparing `rave_python-1.2.9/rave_python/rave_zbmobile.py` & `rave_python-1.4.0/rave_python/rave_tzmobile.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,77 @@
 from rave_python.rave_payment import Payment
 from rave_python.rave_misc import generateTransactionReference
-import json, requests
+from rave_python.rave_exceptions import AccountChargeError
+import json
+import requests
+
+
+class TZSMobile(Payment):
 
-class ZBMobile(Payment):
-    
     def __init__(self, publicKey, secretKey, production, usingEnv):
-        super(ZBMobile, self).__init__(publicKey, secretKey, production, usingEnv)
+        super(TZSMobile, self).__init__(publicKey, secretKey, production, usingEnv)
+
+    
+    def _handleChargeResponse(self, response, txRef, request=None):
+        """ This handles account charge responses """
+        # This checks if we can parse the json successfully
+        res = self._preliminaryResponseChecks(
+            response, AccountChargeError, txRef=txRef)
 
+        response_json = res['json']
+        # change - added data before flwRef
+        response_data = response_json['data']
+        flw_ref = response_data['data']['flw_reference']
+        processor_message = response_data['response_message']
 
+        # If all preliminary checks are passed
+        data = {
+            'error': False,
+            'validationRequired': False,
+            'txRef': txRef,
+            'flwref': flw_ref,
+            'message': processor_message
+        }
+        return data
+
+    
     # Charge mobile money function
     def charge(self, accountDetails, hasFailed=False):
-        """ This is the ghMobile charge call.
+        """ This is the TZS Mobile Money charge.
              Parameters include:\n
             accountDetails (dict) -- These are the parameters passed to the function for processing\n
             hasFailed (boolean) -- This is a flag to determine if the attempt had previously failed due to a timeout\n
         """
-        feature_name = "Initiate-Zambia-mobile-money-charge"
+
         endpoint = self._baseUrl + self._endpointMap["account"]["charge"]
-        
+        feature_name = "TZS Mobile Money Payments"
+
         # It is faster to add boilerplate than to check if each one is present
-        accountDetails.update({"payment_type": "mobilemoneyzambia", "country":"NG", "is_mobile_money_ug":"1", "currency":"ZMW", "network": "MTN"})
-        
-        # If transaction reference is not set 
+        accountDetails.update({
+            "payment_type": "mobilemoneytanzania",
+            "country": "TZ",
+            "is_mobile_money_tz": True,
+            "currency": "TZS"
+            })
+
+        # If transaction reference is not set
         if not ("txRef" in accountDetails):
             accountDetails.update({"txRef": generateTransactionReference()})
-        
+
         # If order reference is not set
         if not ("orderRef" in accountDetails):
             accountDetails.update({"orderRef": generateTransactionReference()})
-        
+
         # Checking for required account components
-        requiredParameters = ["amount", "email", "phonenumber", "network", "IP", "redirect_url"]
-        return super(ZBMobile, self).charge(feature_name, accountDetails, requiredParameters, endpoint)
+        requiredParameters = ["amount", "email", "phonenumber"]
+        
+        return super(TZSMobile, self).charge(feature_name, accountDetails, requiredParameters, endpoint)
 
     def refund(self, flwRef, amount):
-        feature_name = "Zambia-mobile-money-charge-refund"
+        feature_name = "TZS Payments Refund"
         endpoint = self._baseUrl + self._endpointMap["refund"]
-        return super(ZBMobile, self).refund(feature_name, flwRef, amount)
+        return super(TZSMobile, self).refund(feature_name, flwRef, amount)
+
+    def verify(self, txRef):
+        feature_name = "Verify TZS Payment"
+        endpoint = self._baseUrl + self._endpointMap["verify"]
+        return super(TZSMobile, self).verify(feature_name, txRef)
```

### Comparing `rave_python-1.2.9/rave_python.egg-info/PKG-INFO` & `rave_python-1.4.0/rave_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,77 @@
 Metadata-Version: 2.1
 Name: rave-python
-Version: 1.2.9
-Summary: Official Rave Python Wrapper By Flutterwave
+Version: 1.4.0
+Summary: Python library for Flutterwave for Business (F4B) v2 APIs.
 Home-page: https://github.com/Flutterwave/rave-python
 Author: Flutterwave
 Author-email: developers@flutterwavego.com
 License: MIT
 Description: <p align="center">
-            <img title="Flutterwave" height="200" src="https://flutterwave.com/images/logo-colored.svg" width="50%"/>
+            <img title="Flutterwave" height="200" src="https://flutterwave.com/images/logo/full.svg" width="50%"/>
         </p>
         
-        # Rave Python Library.
+        # Flutterwave Python Library.
         ![Upload Python Package](https://github.com/Flutterwave/rave-python/workflows/Upload%20Python%20Package/badge.svg)
         ![PyPI](https://img.shields.io/pypi/v/rave_python)
         ![PyPI - Downloads](https://img.shields.io/pypi/dm/rave_python)
         ![PyPI - License](https://img.shields.io/pypi/l/rave_python)
         
         
         ## Introduction
-        This is a Python wrapper around the [API](https://flutterwavedevelopers.readme.io/v2.0/reference) for [Rave by Flutterwave](https://rave.flutterwave.com).
+        The Python library provides easy access to Flutterwave for Business (F4B) v2 APIs from Django, Flask, and other Python apps. It abstracts the complexity involved in direct integration and allows you to make quick calls to the APIs.
+        
+        Available features include:
+        
+        - Collections: Card, Account, Mobile money, Bank Transfers, USSD, Barter, NQR.
+        - Payouts and Beneficiaries.
+        - Recurring payments: Tokenization and Subscriptions.
+        - Split payments
+        - Card issuing
+        - Transactions dispute management: Refunds.
+        - Transaction reporting: Collections, Payouts, Settlements, and Refunds.
+        - Bill payments: Airtime, Data bundle, Cable, Power, Toll, E-bills, and Remitta.
+        - Identity verification: Resolve bank account, resolve BVN information.
+        
+        ## Table of Contents
+        1. [Requirements](#requirements)
+        2. [Installation](#installation)
+        3. [Initialization](#initialization)
+        4. [Usage](#usage)
+        5. [Testing](#testing)
+        6. [Debugging Errors](#debugging-errors)
+        7. [Support](#support)
+        8. [Contribution guidelines](#)
+        9. [License](#)
+        10. [Changelog](#)
+        
+        ## Requirements
+        1. Flutterwave for business [API Keys](https://developer.flutterwave.com/docs/integration-guides/authentication)
+        2. Supported Python versions: >=2.7, !=3.0.\*, !=3.1.\*, !=3.2.\*, !=3.3.\*, !=3.4.\*
         
-        #### Payment types implemented:
-        * Card Payments
-        * Bank Account Payments
-        * Ghana Mobile Money Payments
-        * Mpesa Payments
-        * Rwanda Mobile Money Payments
-        * Uganda Mobile Money Payments
-        * Zambia Mobile Money Payments
-        * Mobile Money Payments for Francophone countries
-        * Subaccounts
-        * Transfer
-        * Subscription (Recurring Payments)
-        * Bills payment
-        * Payment Plan
-        * USSD Payments (Still in Beta Mode)
-        
-        #### Other features include:
-        * Preauthorization charges
-        * Refunds
-        * Transaction Verification
-        * Transfer Recipients
-        * Virtual Cards
-        * Virtual Accounts
         
         ## Installation
-        To install, run
+        To install the library, run
         
         ```sh
         pip install rave_python
         ```
         
         Note: This is currently under active development
-        ## Import Package
+        
+        
+        ## Initialization
+        
+        ### Import Package
         The base class for this package is 'Rave'. To use this class, add:
         
         ```py
         from rave_python import Rave
         ```
         
-        ## Initialization
-        
         #### To instantiate in sandbox:
         To use Rave, instantiate the Rave class with your public key. We recommend that you store your secret key in an environment variable named, ```RAVE_SECRET_KEY```. Instantiating your rave object is therefore as simple as:
         
         ```py
         rave = Rave("YOUR_PUBLIC_KEY")
         ```
         
@@ -79,15 +86,17 @@
         #### To instantiate in production:
         To initialize in production, simply set the ```production``` flag to ```True```. It is highly discouraged but if you choose to not use environment variables, you can do so in the same way mentioned above.
         
         ```py
         rave = Rave("YOUR_PUBLIC_KEY", production=True)
         ```
         
-        # Rave Objects
+        
+        
+        # Usage
         This is the documentation for all of the components of rave_python
         
         ## ```rave.Card```
         This is used to facilitate card transactions.
         
         **Functions included:**
         
@@ -244,15 +253,15 @@
         This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
         
         Sample
         ```py
         {'flwRef': None, 'cardToken': u'flw-t1nf-5b0f12d565cd961f73c51370b1340f1f-m03k', 'chargedAmount': 100, 'amount': 100, 'transactionComplete': True, 'error': False, 'txRef': u'MC-1538095718251'}
         ```
         
-        #### Please note that after charging a card successfully on rave, if you wish to save the card for further charges, in your verify payment response you will find an object: "cardtoken": "flw-t0-f6f915f53a094671d98560272572993e-m03k".  This is the token you will use for card tokenization. Details are provided below.
+        > Please note that after charging a card successfully on rave, if you wish to save the card for further charges, in your verify payment response you will find an object: `"cardtoken": "flw-t0-f6f915f53a094671d98560272572993e-m03k"`.  This is the token you will use for card tokenization. Details are provided below.
         
         If your call could not be completed successfully, a ```TransactionVerificationError``` is raised.
         
         <br>
         
         ### ```.charge(payload_for_saved_card, chargeWithToken=True)```
         This is called to start a card transaction with a card that has been saved. The payload should be a dictionary containing card information. It should have the parameters:
@@ -399,40 +408,33 @@
         except RaveExceptions.TransactionVerificationError as e:
             print(e.err["errMsg"])
             print(e.err["txRef"])
         ```
         
         <br><br>
         ## ```rave.Account```
-        This is used to facilitate account transactions.
+        This is used to facilitate account transactions. Transactions initiated via this method are authorized by the user on their Banking platform.
         
         **Functions included:**
         
         * ```.charge```
-        
-        * ```.validate```
-        
         * ```.verify```
         
         <br>
         
         ### ```.charge(payload)```
-        This is called to start an account transaction. The payload should be a dictionary containing card information. It should have the parameters:
-        
-        * ```accountbank```, 
-        
-        * ```accountnumber```, 
-        
-        * ```amount```, 
+        This is called to start an account transaction. The payload should be a dictionary containing payment information. It should have the parameters:
         
+        * ```amount``` (The min amount for NGN account payments is N200. For GBP and EUR payments, the min amount is 1), 
+        * ```currency``` (This payment option supports NGN, GBP and EUR),  
         * ```email```, 
-        
-        * ```phonenumber```, 
-        
-        * ```IP```
+        * ```firstname```, 
+        * ```lastname```, 
+        * ```IP``` (optional)
+        * ```redirectUrl``` (optional)
         
         Optionally, you can add a custom transaction reference using the ```txRef``` parameter. Note that if you do not specify one, it would be automatically generated. We do provide a function for generating transaction references in the [Misc library](https://github.com/Flutterwave/rave-python/blob/master/rave_python/rave_misc.py).
         
         
         A sample call is:
         
         ```py
@@ -440,15 +442,22 @@
         ```
         
         #### Returns
         
         This call returns a dictionary. A sample response is:
         
         ```py
-         {'error': False, 'validationRequired': True, 'txRef': 'MC-1530899106006', 'flwRef': 'ACHG-1530899109682', 'authUrl': None}
+        # sample response for NGN account payments
+         {
+           "validationRequired":True,
+           "authUrl":"https://api.ravepay.co/flwv3-pug/getpaid/api/short-url/vHWOLuy89",
+           "flwRef":"XINH44931689941420152189",
+           "txRef":"MC-1689941418883",
+           "error":False
+        }
         ```
         
          This call raises an ```AccountChargeError``` if there was a problem processing your transaction. The ```AccountChargeError``` contains some information about your transaction. You can handle this as such:
         
         ```py
         try: 
             #Your charge call
@@ -461,77 +470,57 @@
         
         ```py
         {'error': True, 'txRef': 'MC-1530897824739', 'flwRef': None, 'errMsg': 'Sorry, that account number is invalid, please check and try again'}
         ```
         
         <br>
         
-        ### ```.validate(txRef)```
-        
-        After a successful charge, most times you will be asked to verify with OTP. To check if this is required, check the ```validationRequired``` key in the ```res``` of the charge call.
-        
-        In the case that an ```authUrl``` is returned from your charge call, you may skip the validation step and simply pass your authUrl to the end-user. 
-        
-        ```py
-        authUrl = res['authUrl']
-        ```
-        
-        To validate, you need to pass the ```flwRef``` from the ```res``` of the charge call as well as the OTP.
-        
-        A sample validate call is: 
-        
-        ```py
-        res2 = rave.Account.validate(res["flwRef"], "12345")
-        ```
-        
-        
-        #### Returns
-        
-        This call returns a dictionary containing the ```txRef```, ```flwRef``` among others if successful.
-        
-        This call raises a ```TransactionValidationError``` if the OTP is not correct or there was a problem processing your request. 
-        
-        To handle this, write:
-        
-        ```py
-        try:
-            # Your charge call
-        except RaveExceptions.TransactionValidationError as e:
-            print(e.err["errMsg"])
-            print(e.err["flwRef"])
-        ```
-        
-        A sample ``` e.err ``` contains:
-        
-        ```py
-        {'error': True, 'txRef': 'MC-1530899869968', 'flwRef': 'ACHG-1530899873118', 'errMsg': 'Pending OTP validation'}
-        ```
-        
-        
-        
-        <br>
-        
         ### ```.verify(txRef)```
         
-        You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned any of the calls (```charge``` or ```validate```). 
+        You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned any the ```charge```call. 
         
         A sample verify call is:
         
         ```py
         res = rave.Account.verify(data["txRef"])
         ```
         
         #### Returns
         
         This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
         
         Sample
         
         ```py
-        {'status': u'success', 'vbvcode': u'N/A', 'chargedamount': 500, 'vbvmessage': u'N/A', 'error': False, 'flwRef': u'ACHG-1538093023787', 'currency': u'NGN', 'amount': 500, 'transactionComplete': True, 'acctmessage': u'Approved Or Completed Successfully', 'chargecode': u'00', 'txRef': u'MC-1538093008498'}
+        {
+           "status":"success",
+           "vbvcode":"57",
+           "chargemessage":"Pending validation",
+           "chargedamount":200,
+           "vbvmessage":"transaction was abandoned",
+           "error":True,
+           "flwRef":"XINH44931689941420152189",
+           "currency":"NGN",
+           "amount":200,
+           "meta":[
+              {
+                 "getpaidTransactionId":984928641,
+                 "metavalue":"12383",
+                 "metaname":"test",
+                 "updatedAt":"2023-07-21T12:10:19.000Z",
+                 "deletedAt":"None",
+                 "id":2168360293,
+                 "createdAt":"2023-07-21T12:10:19.000Z"
+              }
+           ],
+           "transactionComplete":False,
+           "acctmessage":None,
+           "chargecode":"02",
+           "txRef":"MC-1689941418883"
+        }
         ```
         
         If your call could not be completed successfully or if a wrong ```txRef``` is passed, a ```TransactionVerificationError``` is raised. You can handle that as such
         ```py
         try: 
             #Your charge call
         except RaveExceptions.TransactionVerificationError as e:
@@ -564,22 +553,27 @@
         ### Complete account flow
         
         ```py
         from rave_python import Rave, RaveExceptions, Misc
         rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
         # account payload
         payload = {
-          "accountbank": "044",  # get the bank code from the bank list endpoint.
-          "accountnumber": "0690000031",
-          "currency": "NGN",
-          "country": "NG",
-          "amount": "100",
-          "email": "test@test.com",
-          "phonenumber": "0902620185",
-          "IP": "355426087298442",
+           "amount":2,
+           "PBFPubKey":"ENTER_YOUR_PUBLIC_KEY",
+           "currency":"GBP",
+           "email":"user@example.com",
+           "meta":[
+              {
+                 "metaname":"test",
+                 "metavalue":"12383"
+              }
+           ],
+           "ip":"123.0.1.3",
+           "firstname":"Flutterwave",
+           "lastname":"Tester"
         }
         
         try:
             res = rave.Account.charge(payload)
             if res["authUrl"]:
                 print(res["authUrl"])
         
@@ -606,21 +600,20 @@
         ## ```rave.GhMobile```
         This is used to facilitate Ghanaian mobile money transactions.
         
         **Functions included:**
         
         * ```.charge```
         
-        
         * ```.verify```
         
         <br>
         
         ### ```.charge(payload)```
-        This is called to start a Ghana mobile money transaction. The payload should be a dictionary containing account information. It should have the parameters:
+        This is called to start a Ghana mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
         
         * ```amount```,
         
         * ```email```, 
         
         * ```phonenumber```,
         
@@ -640,17 +633,29 @@
         ```
         
         #### Returns
         
         This call returns a dictionary. A sample response is:
         
         ```py
-        {'error': False, 'validationRequired': True, 'txRef': 'MC-1530910216380', 'flwRef': 'N/A'}
+        {
+            "status": "success",
+            "message": "Momo initiated",
+            "data": {
+                "code": "02",
+                "status": "pending",
+                "ts": 1591798138846,
+                "link": "https://ravemodal-dev.herokuapp.com/captcha/verify/123:49fa60c0db04f0017d717a0a662194cd"
+            }
+        }
         ```
         
+        
+        In order to complete the charge, kindly redirect users to the link returned as `data.link` from the charge response.
+        
          This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
         
         ```py
         try: 
             #Your charge call
         except RaveExceptions.TransactionChargeError as e:
             print(e.err["errMsg"])
@@ -873,15 +878,15 @@
         
         
         * ```.verify```
         
         <br>
         
         ### ```.charge(payload)```
-        This is called to start a Ugandan mobile money transaction. The payload should be a dictionary containing account information. It should have the parameters:
+        This is called to start a Ugandan mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
         
         * ```amount```,
         
         * ```email```, 
         
         * ```phonenumber```,
         
@@ -899,17 +904,29 @@
         ```
         
         #### Returns
         
         This call returns a dictionary. A sample response is:
         
         ```py
-        {'error': False, 'status': 'success', 'validationRequired': True, 'txRef': 'MC-1544013787279', 'flwRef': 'flwm3s4m0c1544013788481'}
+        {
+            "status": "success",
+            "message": "Momo initiated",
+            "data": {
+                "code": "02",
+                "status": "pending",
+                "ts": 1591798138846,
+                "link": "https://ravemodal-dev.herokuapp.com/captcha/verify/123:49fa60c0db04f0017d717a0a662194cd"
+            }
+        }
         ```
         
+        
+        In order to complete the charge, kindly redirect users to the link returned as `data.link` from the charge response.
+        
          This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
         
         ```py
         try: 
             #Your charge call
         except RaveExceptions.TransactionChargeError as e:
             print(e.err["errMsg"])
@@ -1003,15 +1020,15 @@
         
         
         * ```.verify```
         
         <br>
         
         ### ```.charge(payload)```
-        This is called to start a Zambian mobile money transaction. The payload should be a dictionary containing account information. It should have the parameters:
+        This is called to start a Zambian mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
         
         * ```amount```,
         
         * ```email```, 
         
         * ```phonenumber```,
         
@@ -1029,17 +1046,28 @@
         ```
         
         #### Returns
         
         This call returns a dictionary. A sample response is:
         
         ```py
-        {'error': False, 'status': 'success', 'validationRequired': True, 'txRef': 'MC-1544013787279', 'flwRef': 'flwm3s4m0c1544013788481'}
+        {
+            "status": "success",
+            "message": "Momo initiated",
+            "data": {
+                "code": "02",
+                "status": "pending",
+                "ts": 1591798138846,
+                "link": "https://ravemodal-dev.herokuapp.com/captcha/verify/123:49fa60c0db04f0017d717a0a662194cd"
+            }
+        }
         ```
         
+        In order to complete the charge, kindly redirect users to the link returned as `data.link` from the charge response.
+        
          This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
         
         ```py
         try: 
             #Your charge call
         except RaveExceptions.TransactionChargeError as e:
             print(e.err["errMsg"])
@@ -1134,15 +1162,15 @@
         
         
         * ```.verify```
         
         <br>
         
         ### ```.charge(payload)```
-        This is called to start a francophone mobile money transaction. The payload should be a dictionary containing account information. It should have the parameters:
+        This is called to start a francophone mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
         
         * ```amount```,
         
         * ```email```, 
         
         * ```phonenumber```,
         
@@ -1232,14 +1260,372 @@
         except RaveExceptions.TransactionVerificationError as e:
           print(e.err["errMsg"])
           print(e.err["txRef"])
         ```
         
         <br><br>
         
+        ## ```rave.TZSMobile```
+        This is used to collect Tanzanian mobile money collections.
+        
+        **Functions included:**
+        
+        * ```.charge```
+        
+        * ```.verify```
+        
+        <br>
+        
+        ### ```.charge(payload)```
+        This is called to start a Tanzanian mobile money transaction. The payload should be a dictionary containing payment information. It should have the parameters:
+        
+        * ```amount```,
+        
+        * ```email```, 
+        
+        * ```phonenumber```,
+        
+        * ```IP``` (optional),
+        
+        * ```redirect_url``` (optional)
+        
+        Optionally, you can add a custom transaction reference using the ```txRef``` parameter. Note that if you do not specify one, it would be automatically generated. We do provide a function for generating transaction references in the [Misc library](https://github.com/Flutterwave/rave-python/blob/master/rave_python/rave_misc.py).
+        
+        
+        A sample call is:
+        
+        ```py
+        res = rave.TZSMobile.charge(payload)
+        ```
+        
+        #### Returns
+        
+        This call returns a dictionary. A sample response is:
+        
+        ```py
+        {}
+        ```
+        
+        
+         This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
+        
+        ```py
+        try: 
+            #Your charge call
+        except RaveExceptions.TransactionChargeError as e:
+            print(e.err["errMsg"])
+            print(e.err["flwRef"])
+        
+        ```
+        
+        A sample ``` e.err ``` contains:
+        
+        ```py
+        {
+           "error":true,
+           "txRef":"MC-1530911537060",
+           "flwRef":None,
+           "errMsg":None
+        }
+        ```
+        
+        
+        <br>
+        
+        ### ```.verify(txRef)```
+        
+        You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned in the ```charge``` call. 
+        
+        A sample verify call is:
+        
+        ```py
+        res = rave.TZSMobile.verify(data["txRef"])
+        ```
+        
+        #### Returns
+        
+        This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
+        
+        If your call could not be completed successfully, a ```TransactionVerificationError``` is raised.
+        
+        
+        ### Complete Tanzania mobile money charge flow
+        
+        ```py
+        from rave_python import Rave, RaveExceptions, Misc
+        rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
+        
+        # mobile payload
+        payload = {
+          "amount": "50",
+          "email": "",
+          "phonenumber": "054709929220",
+          "redirect_url": "https://rave-webhook.herokuapp.com/receivepayment",
+          "IP":""
+        }
+        
+        try:
+          res = rave.TZSMobile.charge(payload)
+          res = rave.TZSMobile.verify(res["txRef"])
+          print(res)
+        
+        except RaveExceptions.TransactionChargeError as e:
+          print(e.err)
+          print(e.err["flwRef"])
+        
+        except RaveExceptions.TransactionVerificationError as e:
+          print(e.err["errMsg"])
+          print(e.err["txRef"])
+        ```
+        
+        <br><br>
+        
+        ## ```rave.BankTransfer```
+        This is used to create a virtual account for a Bank transfer payment.
+        
+        **Functions included:**
+        * ```.charge```
+        * ```.verify```
+        
+        <br>
+        
+        ### ```.charge(payload)```
+        This is called to initiate the Bank transfer payment. The payload should be a dictionary containing payment information. It should have the parameters:
+        
+        * ```amount```,
+        * ```email```,
+        * ```firstname```,
+        * ```lastname```,
+        * ```phonenumber``` (optional),
+        * ```IP``` (optional),
+        * ```redirect_url``` (optional)
+        
+        Optionally, you can add a custom transaction reference using the ```txRef``` parameter. Note that if you do not specify one, it would be automatically generated. We do provide a function for generating transaction references in the [Misc library](https://github.com/Flutterwave/rave-python/blob/master/rave_python/rave_misc.py).
+        
+        
+        A sample call is:
+        
+        ```py
+        res = rave.BankTransfer.charge(payload)
+        ```
+        
+        #### Returns
+        
+        This call returns a dictionary. A sample response is:
+        
+        ```py
+        {
+           "expiresIn":"2023-07-21 13:56:15",
+           "flwRef":"CTNT35701689940575038134",
+           "error":False,
+           "validationRequired":False,
+           "accountNumber":"8526418059",
+           "bankName":"Sterling Bank",
+           "transferNote":"Please make a bank transfer to Flutterwave Developers  FLW",
+           "txRef":"MC-1689940569118"
+        }
+        ```
+        
+        
+         This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
+        
+        ```py
+        try: 
+            #Your charge call
+        except RaveExceptions.TransactionChargeError as e:
+            print(e.err["errMsg"])
+            print(e.err["flwRef"])
+        
+        ```
+        
+        A sample ``` e.err ``` contains:
+        
+        ```py
+        {
+            "error":true,
+           "txRef":"MC-1689940569118",
+           "flwRef":None,
+           "errMsg":None
+        }
+        ```
+        
+        
+        <br>
+        
+        ### ```.verify(txRef)```
+        
+        You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned in the ```charge``` call. 
+        
+        A sample verify call is:
+        
+        ```py
+        res = rave.BankTransfer.verify(data["txRef"])
+        ```
+        
+        #### Returns
+        
+        This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
+        
+        If your call could not be completed successfully, a ```TransactionVerificationError``` is raised.
+        
+        
+        ### Complete Bank Transfer charge flow
+        
+        ```py
+        from rave_python import Rave, RaveExceptions, Misc
+        rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
+        
+        # mobile payload
+        payload = {
+          "amount": "50",
+          "email": "",
+          "phonenumber": "054709929220",
+          "redirect_url": "https://rave-webhook.herokuapp.com/receivepayment",
+          "IP":""
+        }
+        
+        try:
+          res = rave.BankTransfer.charge(payload)
+          res = rave.BankTransfer.verify(res["txRef"])
+          print(res)
+        
+        except RaveExceptions.TransactionChargeError as e:
+          print(e.err)
+          print(e.err["flwRef"])
+        
+        except RaveExceptions.TransactionVerificationError as e:
+          print(e.err["errMsg"])
+          print(e.err["txRef"])
+        ```
+        
+        <br><br>
+        
+        ===
+        ## ```rave.Enaira```
+        This is used to create Enaira wallet payments.
+        
+        **Functions included:**
+        * ```.charge```
+        * ```.verify```
+        
+        <br>
+        
+        ### ```.charge(payload)```
+        This is called to initiate the Enaira payment. The payload should be a dictionary containing payment information. It should have the parameters:
+        
+        * ```amount```,
+        * ```email```,
+        * ```firstname```,
+        * ```lastname```,
+        * ```ìs_token```,
+        * ```phonenumber``` (optional),
+        * ```IP``` (optional),
+        * ```redirect_url``` (optional)
+        
+        Optionally, you can add a custom transaction reference using the ```txRef``` parameter. Note that if you do not specify one, it would be automatically generated. We do provide a function for generating transaction references in the [Misc library](https://github.com/Flutterwave/rave-python/blob/master/rave_python/rave_misc.py).
+        
+        
+        A sample call is:
+        
+        ```py
+        res = rave.Enaira.charge(payload)
+        ```
+        
+        #### Returns
+        This call returns a dictionary. A sample response is:
+        
+        ```py
+        {
+           "txRef":"MC-1689947009435",
+           "error":False,
+           "validationRequired":True,
+           "image":"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAJQAAACUCAYAAAB1PADUAAAAAklEQVR4AewaftIAAAUZSURBVO3BQW4kwZEAQfdE///LvjzGqYBCJ7kaKczsB2tdcljrosNaFx3Wuuiw1kWHtS46rHXRYa2LDmtddFjrosNaFx3Wuuiw1kWHtS46rHXRYa2LPnxJ5S9VvKEyVUwqTyqeqDypeKIyVUwqf6niG4e1LjqsddFhrYs+XFZxk8oTlaniicpU8UTlJpVvVNykctNhrYsOa110WOuiD79M5Y2KNyomlaliUplU3qiYVKaKNyq+ofJGxW86rHXRYa2LDmtd9OF/TMUTlScqU8UTlScqU8W/7LDWRYe1LjqsddGHf5zKE5WpYlKZKiaVqeKJyhsV/00Oa110WOuiw1oXffhlFb+pYlJ5ojJVTCpTxTcqJpVJZap4o+I/yWGtiw5rXXRY66IPl6n8JZWpYlKZKiaVqWJSmSomlaliUpkqJpU3VP6THda66LDWRYe1LjLvuAYxO8DAAAAMklEQVR42mJ89x+CIQjIwMx2mlcDAAZLM2XBEGSJcs1PQwBAHQ6UAA2NhvTwAAAAAElFTkSuQmCC",
+           "validateInstructions":"Please scan the qr image in your eNaira app.",
+           "flwref":"AXOO81561689947011229191"
+        }
+        ```
+        
+        
+         This call raises a ```TransactionChargeError``` if there was a problem processing your transaction. The ```TransactionChargeError``` contains some information about your transaction. You can handle this as such:
+        
+        ```py
+        try: 
+            #Your charge call
+        except RaveExceptions.TransactionChargeError as e:
+            print(e.err["errMsg"])
+            print(e.err["flwRef"])
+        
+        ```
+        
+        A sample ``` e.err ``` contains:
+        
+        ```py
+        {
+            "error":true,
+           "txRef":"MC-1689940569118",
+           "flwRef":None,
+           "errMsg":None
+        }
+        ```
+        
+        
+        <br>
+        
+        ### ```.verify(txRef)```
+        
+        You can call this to check if your transaction was completed successfully. You have to pass the transaction reference generated at the point of charging. This is the ```txRef``` in the ```res``` parameter returned in the ```charge``` call. 
+        
+        A sample verify call is:
+        
+        ```py
+        res = rave.BankTransfer.verify(data["txRef"])
+        ```
+        
+        #### Returns
+        
+        This call returns a dict with ```txRef```, ```flwRef``` and ```transactionComplete``` which indicates whether the transaction was completed successfully. 
+        
+        If your call could not be completed successfully, a ```TransactionVerificationError``` is raised.
+        
+        
+        ### Complete Enaira charge flow
+        
+        ```py
+        from rave_python import Rave, RaveExceptions, Misc
+        rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
+        
+        # mobile payload
+        payload = {
+            "amount": 30,
+            "PBFPubKey": "ENTER_YOUR_PUBLIC_KEY",
+            "currency": "NGN",
+            "email": "user@example.com",
+            "meta": [{"metaname": "test", "metavalue": "12383"}],
+            "ip": "123.0.1.3",
+            "firstname": "Flutterwave",
+            "lastname": "Tester",
+            "is_token": False
+        }
+        
+        try:
+          res = rave.Enaira.charge(payload)
+          res = rave.Enaira.verify(res["txRef"])
+          print(res)
+        
+        except RaveExceptions.TransactionChargeError as e:
+          print(e.err)
+          print(e.err["flwRef"])
+        
+        except RaveExceptions.TransactionVerificationError as e:
+          print(e.err["errMsg"])
+          print(e.err["txRef"])
+        ```
+        
+        <br><br>
+        
         ## ```rave.Preauth```
         This is used to facilitate preauthorized card transactions. This inherits the Card class so any task you can do on Card, you can do with preauth.
         
         **Functions included:**
         
         * ```.charge```
         
@@ -1625,14 +2011,18 @@
         
         * ```.all```
         
         * ```.getFee```
         
         * ```.getBalance```
         
+        *```.retryTransfer```
+        
+        *```fetchRetries```
+        
         <br>
         
         ### ```.initiate(transferDetails)```
         
         This initiates a transfer to a customer's account. When a transfer is initiated, it comes with a status NEW this means the transfer has been queued for processing.
         
         **Please note that you must pass ```beneficiary_name``` as part of the initiate call. Else an error will be thrown.**
@@ -1821,16 +2211,53 @@
         This call returns a dictionary. A sample response is:
         
         ```py
         {'error': False, 'returnedData': {'status': 'success', 'message': 'WALLET-BALANCE', 'data': {'Id': 27122, 'ShortName': 'EUR', 'WalletNumber': '3855000502677', 'AvailableBalance': 0, 'LedgerBalance': 0}}}
         ```
         
         
+        ### ```.retryTransfer(transfer_id)```
+        
+        This allows you to retry a previously failed transfer attempt. You are expected to pass the id for the failed transfer into this call (ids can be gotten in data object from the initial transfer response)
+        
+        A sample fetch call is:
+        
+        ```py
+        res2 = rave.retryTransfer.Balance("169680")
+        ```
+        
+        #### Returns
+        
+        This call returns a dictionary. A sample response is:
+        
+        ```py
+        {'error': False, 'returnedData': {'status': 'success', 'message': 'Transfer retry attempt queued.', 'data': {'id': 169681, 'account_number': '0690000044', 'bank_code': '044', 'fullname': 'Mercedes Daniel', 'date_created': '2021-02-19T15:56:57.000Z', 'currency': 'NGN', 'amount': 500, 'fee': 10.75, 'status': 'NEW', 'reference': 'SampleTransfer4_PMCK_ST_FDU_1_RETRY_1', 'meta': None, 'narration': 'Test_Transfer_for_new_features', 'complete_message': '', 'requires_approval': 0, 'is_approved': 1, 'bank_name': 'ACCESS BANK NIGERIA'}}}
+        ```
+        
         <br>
         
+        ### ```.fetchRetries(transfer_id)```
+        
+        This allows you to get all retry attempts for all previously failed transfer attempts.
+        
+        A sample fetch call is:
+        
+        ```py
+        res2 = rave.fetchRetries.Balance("169680")
+        ```
+        
+        #### Returns
+        
+        This call returns a dictionary. A sample response is:
+        
+        ```py
+        {'error': False, 'returnedData': {'status': 'success', 'message': 'Transfer retry attempts retrieved.', 'data': [{'id': 169681, 'account_number': '0690000044', 'bank_code': '044', 'bank_name': 'ACCESS BANK NIGERIA', 'fullname': 'Mercedes Daniel', 'currency': 'NGN', 'debit_currency': None, 'amount': 500, 'fee': 10.75, 'status': 'FAILED', 'reference': 'SampleTransfer4_PMCK_ST_FDU_1_RETRY_1', 'narration': 'Test_Transfer_for_new_features', 'complete_message': 'DISBURSE FAILED: Transfer failed. Please contact support', 'meta': None, 'requires_approval': 0, 'is_approved': 1, 'date_created': '2021-02-19T15:56:57.000Z'}]}}
+        ```
+        
+        
         ### Complete transfer flow
         
         ```py
         from rave_python import Rave, RaveExceptions
         try:
             rave = Rave("ENTER_YOUR_PUBLIC_KEY", "ENTER_YOUR_SECRET_KEY", usingEnv = False)
         
@@ -2703,15 +3130,16 @@
             "Status": "success",
             "Message": "Withdrawal successful",
             "Reference": null
         }
         ```
         <br>
         
-        ## Run Tests
+        
+        ## Testing
         
         All of the SDK's tests are written with Python's ```unittest``` module. The tests currently test:
         ```rave.Account```
         ```rave.Card```
         ```rave.Transfer```
         ```rave.Preauth```
         ```rave.Subaccount```
@@ -2725,16 +3153,41 @@
         ```
         
         >**NOTE:** If the test fails for creating a subaccount, just change the ```account_number``` ```account_bank```  and ```businesss_email``` to something different
         
         >**NOTE:** The test may fail for account validation - ``` Pending OTP validation``` depending on whether the service is down or not
         <br>
         
+        
+        ## Debugging Errors
+        We understand that you may run into some errors while integrating our library. You can read more about our error messages [here](https://developer.flutterwave.com/docs/integration-guides/errors).
+        
+        For `authorization` and `validation` error responses, double-check your API keys and request. If you get a `server` error, kindly engage the team for support.
+        
+        
+        
         ## Support
-        For further assistance in using the SDK, you can contact the Developers on [Slack](https://join.slack.com/t/flutterwavedevelopers/shared_invite/enQtNTk3MjgxMjU3ODI5LWFkMjBkYTc0ZGJhM2Q5MTY3YjFkYzAyYmM1ZDZjZjUwMjE4YTc2NjQ1ZGM5ZWE4NDUxMzc4MmExYmI1Yjg5ZWU) and [Email](mailto:developers@flutterwavego.com). You can get more information about the amazing features here [here](https://developer.flutterwave.com/reference#introduction).
+        For additional assistance using this library, contact the developer experience (DX) team via [email](mailto:developers@flutterwavego.com) or on [slack](https://bit.ly/34Vkzcg). 
+        
+        You can also follow us [@FlutterwaveEng](https://twitter.com/FlutterwaveEng) and let us know what you think 😊.
+        
+        
+        ## Contribution guidelines
+        Read more about our community contribution guidelines [here](/CONTRIBUTING.md)
+        
+        
+        ## License
+        
+        By contributing to this library, you agree that your contributions will be licensed under its [MIT license](/LICENSE).
+        Copyright (c) Flutterwave Inc.
+        
+        ## Test section
+        Sample Description for teset file. 
+        
+        Final test 3 out of 10. Fingers crossed
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rave_python-1.2.9/rave_python.egg-info/SOURCES.txt` & `rave_python-1.4.0/rave_python.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 README.md
 setup.py
 rave_python/__init__.py
 rave_python/rave.py
 rave_python/rave_account.py
+rave_python/rave_banktransfer.py
 rave_python/rave_base.py
 rave_python/rave_bills.py
 rave_python/rave_card.py
 rave_python/rave_ebills.py
+rave_python/rave_enaira.py
 rave_python/rave_exceptions.py
 rave_python/rave_francophone.py
 rave_python/rave_ghmobile.py
 rave_python/rave_misc.py
 rave_python/rave_mpesa.py
 rave_python/rave_payment.py
 rave_python/rave_paymentplan.py
@@ -18,14 +20,15 @@
 rave_python/rave_recepient.py
 rave_python/rave_recipient.py
 rave_python/rave_rwmobile.py
 rave_python/rave_settlement.py
 rave_python/rave_subaccounts.py
 rave_python/rave_subscription.py
 rave_python/rave_transfer.py
+rave_python/rave_tzmobile.py
 rave_python/rave_ugmobile.py
 rave_python/rave_ussd.py
 rave_python/rave_verify.py
 rave_python/rave_virtualaccount.py
 rave_python/rave_virtualcard.py
 rave_python/rave_zbmobile.py
 rave_python.egg-info/PKG-INFO
```

### Comparing `rave_python-1.2.9/setup.py` & `rave_python-1.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rave_python",
-    version="1.2.9",
+    version="1.4.0",
     author="Flutterwave",
     author_email="developers@flutterwavego.com",
-    description="Official Rave Python Wrapper By Flutterwave",
+    description="Python library for Flutterwave for Business (F4B) v2 APIs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Flutterwave/rave-python",
     license="MIT",
     packages=setuptools.find_packages(),
     python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*",
     classifiers=(
@@ -22,12 +22,12 @@
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ),
-    install_requires = [
+    install_requires=[
         'pycryptodome',
         'requests'
     ]
-)
+)
```

