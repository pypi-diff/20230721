# Comparing `tmp/bridgeobjects-0.1.8.tar.gz` & `tmp/bridgeobjects-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bridgeobjects-0.1.8.tar", last modified: Mon Nov  8 15:02:09 2021, max compression
+gzip compressed data, was "bridgeobjects-0.1.9.tar", last modified: Mon Nov  8 15:08:33 2021, max compression
```

## Comparing `bridgeobjects-0.1.8.tar` & `bridgeobjects-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2021-11-08 15:02:09.616780 bridgeobjects-0.1.8/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     5857 2021-11-08 15:02:09.616780 bridgeobjects-0.1.8/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      874 2020-08-19 08:32:37.000000 bridgeobjects-0.1.8/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2021-11-08 15:02:09.613447 bridgeobjects-0.1.8/bridgeobjects/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1455 2021-08-23 12:09:33.000000 bridgeobjects-0.1.8/bridgeobjects/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2021-11-08 15:02:06.000000 bridgeobjects-0.1.8/bridgeobjects/_version.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1595 2021-05-13 09:54:15.000000 bridgeobjects-0.1.8/bridgeobjects/scratch.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2021-11-08 15:02:09.616780 bridgeobjects-0.1.8/bridgeobjects/source/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-05-05 11:34:45.000000 bridgeobjects-0.1.8/bridgeobjects/source/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4147 2021-11-08 14:50:46.000000 bridgeobjects-0.1.8/bridgeobjects/source/auction.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    11329 2021-08-23 13:07:25.000000 bridgeobjects-0.1.8/bridgeobjects/source/board.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     5637 2021-08-21 13:25:34.000000 bridgeobjects-0.1.8/bridgeobjects/source/call.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4496 2021-08-23 09:59:58.000000 bridgeobjects-0.1.8/bridgeobjects/source/card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     5098 2021-11-08 14:54:33.000000 bridgeobjects-0.1.8/bridgeobjects/source/constants.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7438 2021-11-08 14:58:21.000000 bridgeobjects-0.1.8/bridgeobjects/source/contract.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2842 2021-08-23 12:00:48.000000 bridgeobjects-0.1.8/bridgeobjects/source/denomination.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2795 2021-08-23 11:30:33.000000 bridgeobjects-0.1.8/bridgeobjects/source/event.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    32301 2021-11-08 15:00:57.000000 bridgeobjects-0.1.8/bridgeobjects/source/file_operations.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    33610 2021-10-07 17:15:22.000000 bridgeobjects-0.1.8/bridgeobjects/source/hand.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1804 2021-08-23 12:00:16.000000 bridgeobjects-0.1.8/bridgeobjects/source/suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4500 2021-10-10 11:15:38.000000 bridgeobjects-0.1.8/bridgeobjects/source/suit_base.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3889 2021-09-29 12:12:08.000000 bridgeobjects-0.1.8/bridgeobjects/source/trick.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2021-11-08 15:02:09.616780 bridgeobjects-0.1.8/bridgeobjects/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-05-05 11:34:45.000000 bridgeobjects-0.1.8/bridgeobjects/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2889 2021-05-13 07:24:57.000000 bridgeobjects-0.1.8/bridgeobjects/tests/test_auctions.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17219 2021-08-22 14:26:10.000000 bridgeobjects-0.1.8/bridgeobjects/tests/test_boards.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7627 2021-05-05 11:34:45.000000 bridgeobjects-0.1.8/bridgeobjects/tests/test_calls.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     5993 2021-05-13 09:04:06.000000 bridgeobjects-0.1.8/bridgeobjects/tests/test_cards.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3667 2021-05-05 11:34:45.000000 bridgeobjects-0.1.8/bridgeobjects/tests/test_contracts.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3984 2021-05-05 11:34:45.000000 bridgeobjects-0.1.8/bridgeobjects/tests/test_denominations.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2089 2021-08-23 08:48:16.000000 bridgeobjects-0.1.8/bridgeobjects/tests/test_events.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    31694 2021-08-23 13:47:08.000000 bridgeobjects-0.1.8/bridgeobjects/tests/test_hands.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7563 2021-08-23 13:57:47.000000 bridgeobjects-0.1.8/bridgeobjects/tests/test_pbn.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7560 2021-08-23 13:25:34.000000 bridgeobjects-0.1.8/bridgeobjects/tests/test_rbn.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3550 2021-05-05 11:34:45.000000 bridgeobjects-0.1.8/bridgeobjects/tests/test_suits.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1787 2021-08-21 15:11:56.000000 bridgeobjects-0.1.8/bridgeobjects/tests/test_trick.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2021-11-08 15:02:09.613447 bridgeobjects-0.1.8/bridgeobjects.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     5857 2021-11-08 15:02:09.000000 bridgeobjects-0.1.8/bridgeobjects.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1145 2021-11-08 15:02:09.000000 bridgeobjects-0.1.8/bridgeobjects.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2021-11-08 15:02:09.000000 bridgeobjects-0.1.8/bridgeobjects.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       14 2021-11-08 15:02:09.000000 bridgeobjects-0.1.8/bridgeobjects.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2021-11-08 15:02:09.616780 bridgeobjects-0.1.8/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1351 2021-07-03 11:07:25.000000 bridgeobjects-0.1.8/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2021-11-08 15:08:33.470423 bridgeobjects-0.1.9/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     5975 2021-11-08 15:08:33.470423 bridgeobjects-0.1.9/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      874 2020-08-19 08:32:37.000000 bridgeobjects-0.1.9/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2021-11-08 15:08:33.467090 bridgeobjects-0.1.9/bridgeobjects/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1455 2021-08-23 12:09:33.000000 bridgeobjects-0.1.9/bridgeobjects/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2021-11-08 15:07:41.000000 bridgeobjects-0.1.9/bridgeobjects/_version.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1595 2021-05-13 09:54:15.000000 bridgeobjects-0.1.9/bridgeobjects/scratch.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2021-11-08 15:08:33.470423 bridgeobjects-0.1.9/bridgeobjects/source/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-05-05 11:34:45.000000 bridgeobjects-0.1.9/bridgeobjects/source/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4147 2021-11-08 14:50:46.000000 bridgeobjects-0.1.9/bridgeobjects/source/auction.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    11493 2021-11-08 15:07:47.000000 bridgeobjects-0.1.9/bridgeobjects/source/board.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     5637 2021-08-21 13:25:34.000000 bridgeobjects-0.1.9/bridgeobjects/source/call.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4496 2021-08-23 09:59:58.000000 bridgeobjects-0.1.9/bridgeobjects/source/card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     5098 2021-11-08 14:54:33.000000 bridgeobjects-0.1.9/bridgeobjects/source/constants.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     7438 2021-11-08 14:58:21.000000 bridgeobjects-0.1.9/bridgeobjects/source/contract.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2842 2021-08-23 12:00:48.000000 bridgeobjects-0.1.9/bridgeobjects/source/denomination.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2795 2021-08-23 11:30:33.000000 bridgeobjects-0.1.9/bridgeobjects/source/event.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    32301 2021-11-08 15:00:57.000000 bridgeobjects-0.1.9/bridgeobjects/source/file_operations.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    33610 2021-10-07 17:15:22.000000 bridgeobjects-0.1.9/bridgeobjects/source/hand.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1804 2021-08-23 12:00:16.000000 bridgeobjects-0.1.9/bridgeobjects/source/suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4500 2021-10-10 11:15:38.000000 bridgeobjects-0.1.9/bridgeobjects/source/suit_base.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3889 2021-09-29 12:12:08.000000 bridgeobjects-0.1.9/bridgeobjects/source/trick.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2021-11-08 15:08:33.470423 bridgeobjects-0.1.9/bridgeobjects/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-05-05 11:34:45.000000 bridgeobjects-0.1.9/bridgeobjects/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2889 2021-05-13 07:24:57.000000 bridgeobjects-0.1.9/bridgeobjects/tests/test_auctions.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17219 2021-08-22 14:26:10.000000 bridgeobjects-0.1.9/bridgeobjects/tests/test_boards.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     7627 2021-05-05 11:34:45.000000 bridgeobjects-0.1.9/bridgeobjects/tests/test_calls.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     5993 2021-05-13 09:04:06.000000 bridgeobjects-0.1.9/bridgeobjects/tests/test_cards.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3667 2021-05-05 11:34:45.000000 bridgeobjects-0.1.9/bridgeobjects/tests/test_contracts.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3984 2021-05-05 11:34:45.000000 bridgeobjects-0.1.9/bridgeobjects/tests/test_denominations.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2089 2021-08-23 08:48:16.000000 bridgeobjects-0.1.9/bridgeobjects/tests/test_events.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    31694 2021-08-23 13:47:08.000000 bridgeobjects-0.1.9/bridgeobjects/tests/test_hands.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     7563 2021-08-23 13:57:47.000000 bridgeobjects-0.1.9/bridgeobjects/tests/test_pbn.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     7560 2021-08-23 13:25:34.000000 bridgeobjects-0.1.9/bridgeobjects/tests/test_rbn.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3550 2021-05-05 11:34:45.000000 bridgeobjects-0.1.9/bridgeobjects/tests/test_suits.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1787 2021-08-21 15:11:56.000000 bridgeobjects-0.1.9/bridgeobjects/tests/test_trick.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2021-11-08 15:08:33.467090 bridgeobjects-0.1.9/bridgeobjects.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     5975 2021-11-08 15:08:33.000000 bridgeobjects-0.1.9/bridgeobjects.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1145 2021-11-08 15:08:33.000000 bridgeobjects-0.1.9/bridgeobjects.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2021-11-08 15:08:33.000000 bridgeobjects-0.1.9/bridgeobjects.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       14 2021-11-08 15:08:33.000000 bridgeobjects-0.1.9/bridgeobjects.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2021-11-08 15:08:33.470423 bridgeobjects-0.1.9/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1351 2021-07-03 11:07:25.000000 bridgeobjects-0.1.9/setup.py
```

### Comparing `bridgeobjects-0.1.8/PKG-INFO` & `bridgeobjects-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgeobjects
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
             A collection of modules that allows the user to access objects used in bridge games,
             for example, a board or a contract.
         
 Home-page: https://psionman@bitbucket.org/psionman/bridgeobjects.git
 Author: jeff watkins
 Author-email: support@bidforgame.com
@@ -37,14 +37,21 @@
         ```bash
         pip install bridgeobjects
         ```
         
         
         ---------
         
+        Version 0.1.9 - 8 Nov 2021
+        
+        board.py not updated
+        
+        
+        ---------
+        
         Version 0.1.8 - 8 Nov 2021
         
         auction.play: add seat_calls
         
         board.py: add declarers_tricks and optimum_result_table
         
         constants.py: add DENOMINATION_NAMES, remove CARD_RANKS and consolidate into CARD_VALUES
```

### Comparing `bridgeobjects-0.1.8/README.md` & `bridgeobjects-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/__init__.py` & `bridgeobjects-0.1.9/bridgeobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/scratch.py` & `bridgeobjects-0.1.9/bridgeobjects/scratch.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/source/auction.py` & `bridgeobjects-0.1.9/bridgeobjects/source/auction.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/source/board.py` & `bridgeobjects-0.1.9/bridgeobjects/source/board.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .card import Card
 from .hand import Hand
 from .auction import Auction
 from .contract import Contract
 from .trick import Trick
 
-from .constants import SEATS, RANKS, SUITS, VULNERABLE, SUIT_NAMES, CARD_NAMES
+from .constants import SEATS, RANKS, SUITS, VULNERABLE, SUIT_NAMES, CARD_NAMES, DENOMINATION_NAMES
 
 __all__ = ['Board']
 
 
 class Board(object):
     """
     The board object for the bridgeobjects module.
@@ -55,14 +55,16 @@
         self._contract = Contract()
         self.auction = Auction()
         self.tricks: List[Trick] = []
         self.NS_tricks = 0
         self.EW_tricks = 0
         self.play_notes: Dict[str, str] = {}
         self.description = ""
+        self.result = ""
+        self.optimum_result_table = {seat: {denomination: 0 for denomination in DENOMINATION_NAMES} for seat in SEATS}
 
     def _set_hands(self, hands: List[Hand]) -> Tuple[Dict[object, Hand], Dict[int, Hand], Dict[str, Hand]]:
         """Return the hands as a dict."""
         # If hands is a list then 0 is the North hand and proceed clockwise.
         # If hands is a dict, then determine if the keys are numeric (position) or
         # alpha (SEATS) and proceed accordingly.
         hand_dict: Dict[object, Hand] = dict()
```

### Comparing `bridgeobjects-0.1.8/bridgeobjects/source/call.py` & `bridgeobjects-0.1.9/bridgeobjects/source/call.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/source/card.py` & `bridgeobjects-0.1.9/bridgeobjects/source/card.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/source/constants.py` & `bridgeobjects-0.1.9/bridgeobjects/source/constants.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/source/contract.py` & `bridgeobjects-0.1.9/bridgeobjects/source/contract.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/source/denomination.py` & `bridgeobjects-0.1.9/bridgeobjects/source/denomination.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/source/event.py` & `bridgeobjects-0.1.9/bridgeobjects/source/event.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/source/file_operations.py` & `bridgeobjects-0.1.9/bridgeobjects/source/file_operations.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/source/hand.py` & `bridgeobjects-0.1.9/bridgeobjects/source/hand.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/source/suit.py` & `bridgeobjects-0.1.9/bridgeobjects/source/suit.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/source/suit_base.py` & `bridgeobjects-0.1.9/bridgeobjects/source/suit_base.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/source/trick.py` & `bridgeobjects-0.1.9/bridgeobjects/source/trick.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/tests/test_auctions.py` & `bridgeobjects-0.1.9/bridgeobjects/tests/test_auctions.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/tests/test_boards.py` & `bridgeobjects-0.1.9/bridgeobjects/tests/test_boards.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/tests/test_calls.py` & `bridgeobjects-0.1.9/bridgeobjects/tests/test_calls.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/tests/test_cards.py` & `bridgeobjects-0.1.9/bridgeobjects/tests/test_cards.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/tests/test_contracts.py` & `bridgeobjects-0.1.9/bridgeobjects/tests/test_contracts.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/tests/test_denominations.py` & `bridgeobjects-0.1.9/bridgeobjects/tests/test_denominations.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/tests/test_events.py` & `bridgeobjects-0.1.9/bridgeobjects/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/tests/test_hands.py` & `bridgeobjects-0.1.9/bridgeobjects/tests/test_hands.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/tests/test_pbn.py` & `bridgeobjects-0.1.9/bridgeobjects/tests/test_pbn.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/tests/test_rbn.py` & `bridgeobjects-0.1.9/bridgeobjects/tests/test_rbn.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/tests/test_suits.py` & `bridgeobjects-0.1.9/bridgeobjects/tests/test_suits.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects/tests/test_trick.py` & `bridgeobjects-0.1.9/bridgeobjects/tests/test_trick.py`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/bridgeobjects.egg-info/PKG-INFO` & `bridgeobjects-0.1.9/bridgeobjects.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgeobjects
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
             A collection of modules that allows the user to access objects used in bridge games,
             for example, a board or a contract.
         
 Home-page: https://psionman@bitbucket.org/psionman/bridgeobjects.git
 Author: jeff watkins
 Author-email: support@bidforgame.com
@@ -37,14 +37,21 @@
         ```bash
         pip install bridgeobjects
         ```
         
         
         ---------
         
+        Version 0.1.9 - 8 Nov 2021
+        
+        board.py not updated
+        
+        
+        ---------
+        
         Version 0.1.8 - 8 Nov 2021
         
         auction.play: add seat_calls
         
         board.py: add declarers_tricks and optimum_result_table
         
         constants.py: add DENOMINATION_NAMES, remove CARD_RANKS and consolidate into CARD_VALUES
```

### Comparing `bridgeobjects-0.1.8/bridgeobjects.egg-info/SOURCES.txt` & `bridgeobjects-0.1.9/bridgeobjects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bridgeobjects-0.1.8/setup.py` & `bridgeobjects-0.1.9/setup.py`

 * *Files identical despite different names*

