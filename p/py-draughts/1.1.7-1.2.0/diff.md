# Comparing `tmp/py-draughts-1.1.7.tar.gz` & `tmp/py-draughts-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-1.1.7.tar", last modified: Fri Jul 21 08:39:35 2023, max compression
+gzip compressed data, was "py-draughts-1.2.0.tar", last modified: Fri Jul 21 13:22:15 2023, max compression
```

## Comparing `py-draughts-1.1.7.tar` & `py-draughts-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.355822 py-draughts-1.1.7/
--rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-1.1.7/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-16 08:41:45.000000 py-draughts-1.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     5136 2023-07-21 08:39:35.352821 py-draughts-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3716 2023-07-21 08:29:32.000000 py-draughts-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.241823 py-draughts-1.1.7/draughts/
--rw-rw-rw-   0        0        0     1585 2023-07-21 08:30:22.000000 py-draughts-1.1.7/draughts/__init__.py
--rw-rw-rw-   0        0        0     3666 2023-07-19 10:32:24.000000 py-draughts-1.1.7/draughts/american.py
--rw-rw-rw-   0        0        0    12403 2023-07-21 08:27:54.000000 py-draughts-1.1.7/draughts/base.py
--rw-rw-rw-   0        0        0     3857 2023-07-19 11:00:41.000000 py-draughts-1.1.7/draughts/engine.py
--rw-rw-rw-   0        0        0      671 2023-07-19 10:32:24.000000 py-draughts-1.1.7/draughts/models.py
--rw-rw-rw-   0        0        0     4179 2023-07-21 08:25:28.000000 py-draughts-1.1.7/draughts/move.py
--rw-rw-rw-   0        0        0     5595 2023-07-21 08:28:34.000000 py-draughts-1.1.7/draughts/server.py
--rw-rw-rw-   0        0        0     8462 2023-07-21 08:22:34.000000 py-draughts-1.1.7/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.145825 py-draughts-1.1.7/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.254821 py-draughts-1.1.7/draughts/static/css/
--rw-rw-rw-   0        0        0     3873 2023-07-13 16:31:38.000000 py-draughts-1.1.7/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.268823 py-draughts-1.1.7/draughts/static/js/
--rw-rw-rw-   0        0        0     6118 2023-07-19 10:32:24.000000 py-draughts-1.1.7/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.290826 py-draughts-1.1.7/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-13 13:19:03.000000 py-draughts-1.1.7/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2882 2023-07-16 09:39:24.000000 py-draughts-1.1.7/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-19 10:32:24.000000 py-draughts-1.1.7/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.330821 py-draughts-1.1.7/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     5136 2023-07-21 08:39:35.000000 py-draughts-1.1.7/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-07-21 08:39:35.000000 py-draughts-1.1.7/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 08:39:35.000000 py-draughts-1.1.7/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-21 08:39:35.000000 py-draughts-1.1.7/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 08:39:35.000000 py-draughts-1.1.7/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2023-07-19 10:32:24.000000 py-draughts-1.1.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 08:39:35.355822 py-draughts-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1908 2023-07-16 08:44:01.000000 py-draughts-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.345821 py-draughts-1.1.7/test/
--rw-rw-rw-   0        0        0     1104 2023-07-19 10:32:24.000000 py-draughts-1.1.7/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-13 17:33:45.000000 py-draughts-1.1.7/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.846282 py-draughts-1.2.0/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-16 08:41:45.000000 py-draughts-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5136 2023-07-21 13:22:15.844281 py-draughts-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3716 2023-07-21 08:29:32.000000 py-draughts-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.784279 py-draughts-1.2.0/draughts/
+-rw-rw-rw-   0        0        0     1585 2023-07-21 13:21:47.000000 py-draughts-1.2.0/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3763 2023-07-21 12:56:50.000000 py-draughts-1.2.0/draughts/american.py
+-rw-rw-rw-   0        0        0    13482 2023-07-21 13:12:47.000000 py-draughts-1.2.0/draughts/base.py
+-rw-rw-rw-   0        0        0     3857 2023-07-21 09:39:46.000000 py-draughts-1.2.0/draughts/engine.py
+-rw-rw-rw-   0        0        0      671 2023-07-19 10:32:24.000000 py-draughts-1.2.0/draughts/models.py
+-rw-rw-rw-   0        0        0     4179 2023-07-21 08:25:28.000000 py-draughts-1.2.0/draughts/move.py
+-rw-rw-rw-   0        0        0     5441 2023-07-21 12:58:57.000000 py-draughts-1.2.0/draughts/server.py
+-rw-rw-rw-   0        0        0     8403 2023-07-21 13:16:43.000000 py-draughts-1.2.0/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.719330 py-draughts-1.2.0/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.790277 py-draughts-1.2.0/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-13 16:31:38.000000 py-draughts-1.2.0/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.796276 py-draughts-1.2.0/draughts/static/js/
+-rw-rw-rw-   0        0        0     6118 2023-07-19 10:32:24.000000 py-draughts-1.2.0/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.805240 py-draughts-1.2.0/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-13 13:19:03.000000 py-draughts-1.2.0/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2882 2023-07-16 09:39:24.000000 py-draughts-1.2.0/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-19 10:32:24.000000 py-draughts-1.2.0/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.827274 py-draughts-1.2.0/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     5136 2023-07-21 13:22:15.000000 py-draughts-1.2.0/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2023-07-21 13:22:15.000000 py-draughts-1.2.0/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 13:22:15.000000 py-draughts-1.2.0/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-21 13:22:15.000000 py-draughts-1.2.0/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 13:22:15.000000 py-draughts-1.2.0/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-07-19 10:32:24.000000 py-draughts-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 13:22:15.846282 py-draughts-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1908 2023-07-16 08:44:01.000000 py-draughts-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.840269 py-draughts-1.2.0/test/
+-rw-rw-rw-   0        0        0     1104 2023-07-19 10:32:24.000000 py-draughts-1.2.0/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2510 2023-07-21 13:07:31.000000 py-draughts-1.2.0/test/test_board.py
+-rw-rw-rw-   0        0        0     1370 2023-07-21 13:21:26.000000 py-draughts-1.2.0/test/test_standard_board.py
```

### Comparing `py-draughts-1.1.7/LICENSE` & `py-draughts-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.7/PKG-INFO` & `py-draughts-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.1.7
+Version: 1.2.0
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
```

### Comparing `py-draughts-1.1.7/README.md` & `py-draughts-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.7/draughts/__init__.py` & `py-draughts-1.2.0/draughts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 A draughts library with advenced (customizable) WEB UI move generation and validation,
 PDN parsing and writing. Supports multiple variants of game.
 """
 
 from typing import Literal
 
-__version__ = "1.1.7"
+__version__ = "1.2.0"
 __author__ = "Michał Skibiński"
 
 
 def get_board(variant: Literal["standard", "american"], fen: str = None):
     """
     Board factory method.
     - ``standard`` - standard draughts board
```

### Comparing `py-draughts-1.1.7/draughts/american.py` & `py-draughts-1.2.0/draughts/american.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,23 +28,26 @@
      - Board size: 8x8
      - Short moves only
      - Only the king can capture backwards
      - Capture - choose any
     """
 
     GAME_TYPE = 23
+    STARTING_COLOR = Color.WHITE
     STARTING_POSITION = np.array([1] * 12 + [0] * 8 + [-1] * 12, dtype=np.int8)
     VARIANT_NAME = "American checkers"
     ROW_IDX = {val: val // 4 for val in range(len(STARTING_POSITION))}
     COL_IDX = {val: val % 8 for val in range(len(STARTING_POSITION))}
 
     size = int(np.sqrt(len(STARTING_POSITION) * 2))
 
-    def __init__(self, starting_position=STARTING_POSITION) -> None:
-        super().__init__(starting_position)
+    # def __init__(
+    #     self, starting_position=STARTING_POSITION, turn=STARTING_COLOR, *args, **kwargs
+    # ) -> None:
+    #     super().__init__(starting_position, turn, *args, **kwargs)
 
     @property
     def is_draw(self) -> bool:
         return self.is_threefold_repetition
 
     @property
     def legal_moves(self) -> Generator[Move, None, None]:
@@ -107,9 +110,8 @@
     board = Board()
     from draughts.server import Server
 
     Server(board).run()
     moves = ["24-20", "11-16", "20x11", "7x16"]
     for m in moves:
         board.push_uci(m)
-        print(board)
         print(list(board.legal_moves))
```

### Comparing `py-draughts-1.1.7/draughts/base.py` & `py-draughts-1.2.0/draughts/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from abc import ABC, abstractproperty
 from typing import Generator
 
 import numpy as np
 
 from draughts.models import FIGURE_REPR, Color, Figure, SquareT
 from draughts.move import Move
-from draughts.utils import logger
+from draughts.utils import (
+    logger,
+    get_king_pseudo_legal_moves,
+    get_man_pseudo_legal_moves,
+)
 
 # fmt: off
 SQUARES = [_, B8, D8, F8, H8,
         A7, C7, E7, G7,
         B6, D6, F6, H6,
         A5, C5, E5, G5,
         B4, D4, F4, H4,
@@ -33,26 +37,28 @@
     By specifying the starting position, the user can create a board of any size.
 
 
 
     To create new variants of draughts, inherit from this class and:
 
     - override the ``legal_moves`` property
-    - override the ``SQUARES`` list to match the new board size
+    - (optional) override the ``SQUARES`` list to match the new board size if you want to use UCI notation: ``[A1, B1, C1, ...]``
     - override the ``STARTING_POSITION`` to specify the starting position
-
+    - override the ``STARTING_COLOR`` to specify the starting color
     Constraints:
     - There are only two colors:
         - ``Color.WHITE``
         - ``Color.BLACK``
 
     - There are only two types of pieces:
         - ``PieceType.MAN``
         - ``PieceType.KING``
     - **Board should always be square.**
+    .. note::
+        For generating legal moves use
     """
 
     GAME_TYPE = -1
     """
     PDN game type. See `PDN specification <https://en.wikipedia.org/wiki/Portable_Draughts_Notation>`_.
     """
     VARIANT_NAME = "Abstract variant"
@@ -69,40 +75,60 @@
     """
 
     STARTING_COLOR = Color.WHITE
     """
     Starting color. ``Color.WHITE`` or ``Color.BLACK``.
     """
 
-    PSEUDO_LEGAL_KING_MOVES = None
+    PSEUDO_LEGAL_MAN_MOVES = ...
     """
     Dictionary of pseudo-legal moves for king pieces. Generated only on module import.
     This dictionary contains all possible moves for king piece (as if there were no other pieces on the board).
     
     **Structure:**
-    
     ``[(right-up moves), (left-up moves), (right-down moves), (left-down moves)]``
-    
     """
-    PSEUDO_LEGAL_MAN_MOVES = None
+    PSEUDO_LEGAL_KING_MOVES = ...
     """ 
     Same as ``PSEUDO_LEGAL_KING_MOVES`` but contains only first 2 squares of the move.
     (one for move and one for capture)
     """
 
-    def __init__(self, starting_position: np.ndarray) -> None:
+    def __init_subclass__(cls, **kwargs):
+        parent_class = cls.__bases__[0]
+        parent_class_vars = vars(parent_class)
+        child_class_vars = vars(cls)
+        for var_name, var_value in child_class_vars.items():
+            if var_name in parent_class_vars and not var_name.startswith("_"):
+                setattr(parent_class, var_name, var_value)
+        cls.PSEUDO_LEGAL_KING_MOVES = get_king_pseudo_legal_moves(
+            len(cls.STARTING_POSITION)
+        )
+        cls.PSEUDO_LEGAL_MAN_MOVES = get_man_pseudo_legal_moves(
+            len(cls.STARTING_POSITION)
+        )
+
+    def __init__(
+        self,
+        starting_position: np.ndarray = None,
+        turn: Color = None,
+    ) -> None:
         """
         Initializes the board with a starting position.
         The starting position must be a numpy array of length n * n/2,
         where n is the size of the board.
 
         """
         super().__init__()
-        self._pos = starting_position.copy()
-        self.turn = self.STARTING_COLOR
+        self._pos = (
+            starting_position
+            if starting_position is not None
+            else self.STARTING_POSITION
+        )
+        self.turn = turn if turn is not None else self.STARTING_COLOR
         size = int(np.sqrt(len(self.position) * 2))
         if size**2 != len(self.position) * 2:
             msg = f"Invalid board with shape {starting_position.shape} provided.\
                 Please use an array with lenght = (n * n/2). \
                 Where n is an size of the board."
             logger.error(msg)
             raise ValueError(msg)
@@ -246,14 +272,15 @@
         return "".join(fen_components)
 
     @classmethod
     def from_fen(cls, fen: str) -> BaseBoard:
         """
         Creates a board from a FEN string by using regular expressions.
         """
+        logger.debug(f"Initializing board from FEN: {fen}")
         fen = fen.upper()
         re_turn = re.compile(r"[WB]:")
         re_premove = re.compile(r"(G[0-9]+|P[0-9]+)(,|)")
         re_prefix = re.compile(r"[WB]:[WB]:[WB]")
         re_white = re.compile(r"W[0-9K,]+")
         re_black = re.compile(r"B[0-9K,]+")
         # remove premoves from fen
@@ -274,17 +301,16 @@
         if len(turn) != 1 or (len(white) == 0 and len(black) == 0):
             raise ValueError(f"Invalid FEN: {fen}")
         try:
             cls.__populate_from_list(white.split(","), Color.WHITE)
             cls.__populate_from_list(black.split(","), Color.BLACK)
         except ValueError as e:
             logger.error(f"Invalid FEN: {fen} \n {e}")
-        cls.turn = Color.WHITE if turn == "W" else Color.BLACK
-        cls.STARTING_COLOR = cls.turn
-        return cls(starting_position=cls.STARTING_POSITION)
+        turn = Color.WHITE if turn == "W" else Color.BLACK
+        return cls(cls.STARTING_POSITION, turn)
 
     @classmethod
     def __populate_from_list(cls, fen_list: list[str], color: Color) -> None:
         board_range = range(1, cls.STARTING_POSITION.shape[0] + 1)
         for sq in fen_list:
             if sq.isdigit() and int(sq) in board_range:
                 cls.STARTING_POSITION[int(sq) - 1] = color.value
@@ -344,15 +370,15 @@
             yield sq
 
     def __getitem__(self, key: SquareT) -> Figure:
         return self.position[key]
 
 
 if __name__ == "__main__":
-    board = BaseBoard(BaseBoard.STARTING_POSITION)
+    board = BaseBoard(BaseBoard.STARTING_POSITION, Color.WHITE)
     # print(board)
 # print(board.info)
 #     m1 = Move([C3, B4])
 #     board.push(m1)
 
 #     m2 = Move([B6, A5])
 #     board.push(m2)
```

### Comparing `py-draughts-1.1.7/draughts/engine.py` & `py-draughts-1.2.0/draughts/engine.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.7/draughts/models.py` & `py-draughts-1.2.0/draughts/models.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.7/draughts/move.py` & `py-draughts-1.2.0/draughts/move.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.7/draughts/server.py` & `py-draughts-1.2.0/draughts/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,10 @@
         uvicorn.run(self.APP, **kwargs)
 
 
 if __name__ == "__main__":
     from draughts.engine import AlphaBetaEngine
     from draughts import get_board
 
-    engine = AlphaBetaEngine(depth=4)
-    board = get_board(
-        "standard",
-        '[FEN "W:B:W23,27,29,33,34,37,42,45,46,50:B5,8,9,10,12,13,14,15,16,17,20,36"]',
-    )
-    server = Server(board=board, get_best_move_method=engine.get_best_move)
+    engine = AlphaBetaEngine(depth=6)
+    server = Server(get_best_move_method=engine.get_best_move)
     server.run()
```

### Comparing `py-draughts-1.1.7/draughts/standard.py` & `py-draughts-1.2.0/draughts/standard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
+import types
+from typing import Any
 
 import numpy as np
 
 from draughts.base import BaseBoard
-from draughts.models import Figure
+from draughts.models import Color, Figure
 from draughts.move import Move
 from draughts.utils import (
     get_king_pseudo_legal_moves,
     get_man_pseudo_legal_moves,
     logger,
 )
 
@@ -51,21 +53,23 @@
       or less including at least one king (one king, two kings, or one king and a man),
       the game is drawn after both players made 5 moves.
 
     """
 
     GAME_TYPE = 20
     STARTING_POSITION = np.array([1] * 15 + [0] * 20 + [-1] * 15, dtype=np.int8)
-    PSEUDO_LEGAL_KING_MOVES = get_king_pseudo_legal_moves(len(STARTING_POSITION))
-    PSEUDO_LEGAL_MAN_MOVES = get_man_pseudo_legal_moves(len(STARTING_POSITION))
+    STARTING_COLOR = Color.WHITE
+
     ROW_IDX = {val: val // 5 for val in range(len(STARTING_POSITION))}
     COL_IDX = {val: val % 10 for val in range(len(STARTING_POSITION))}
 
-    def __init__(self, starting_position=STARTING_POSITION) -> None:
-        super().__init__(starting_position)
+    # def __init__(
+    #     self, starting_position=STARTING_POSITION, turn=STARTING_COLOR, *args, **kwargs
+    # ) -> None:
+    #     super().__init__(starting_position, turn, *args, **kwargs)
 
     @property
     def is_draw(self) -> bool:
         return (
             self.is_threefold_repetition
             or self.is_5_moves_rule
             or self.is_16_moves_rule
@@ -116,17 +120,15 @@
         for square in squares_list.flatten():
             moves = self._legal_moves_from(square, is_capture_mandatory)
             # if not is_capture_mandatory and any( # TODO this should optimize the search
             #     [len(move.square_list) > 0 for move in moves]
             # ):
             #     is_capture_mandatory = True
             all_moves.extend(moves)
-        if any([len(move) > 1 for move in all_moves]):
-            all_moves = [move for move in all_moves if len(move) > 1]
-        return all_moves
+        return [mv for mv in all_moves if len(mv) == max(len(m) for m in all_moves)]
 
     def _get_man_legal_moves_from(
         self, square: int, is_capture_mandatory: bool
     ) -> list:
         moves = []
         # white can move only on even directions
         for idx, direction in enumerate(self.PSEUDO_LEGAL_MAN_MOVES[square]):
@@ -203,10 +205,10 @@
             moves = [move for move in moves if len(move.captured_list) > 0]
         return moves
 
 
 if __name__ == "__main__":
     board = Board()
 
-    b = Board.from_fen("B:B:WG8,18,24,28,34,37,42,44,49:B2,10,12,15,25,26")
-    print(b)
-    Board.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
+    # b = Board.from_fen("B:B:WG8,18,24,28,34,37,42,44,49:B2,10,12,15,25,26")
+    # print(b)
+    # Board.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
```

### Comparing `py-draughts-1.1.7/draughts/static/css/style.css` & `py-draughts-1.2.0/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.7/draughts/static/js/script.js` & `py-draughts-1.2.0/draughts/static/js/script.js`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.7/draughts/templates/base.html` & `py-draughts-1.2.0/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.7/draughts/templates/index.html` & `py-draughts-1.2.0/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.7/draughts/utils.py` & `py-draughts-1.2.0/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.7/py_draughts.egg-info/PKG-INFO` & `py-draughts-1.2.0/py_draughts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.1.7
+Version: 1.2.0
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
```

### Comparing `py-draughts-1.1.7/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.2.0/py_draughts.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 draughts/templates/index.html
 py_draughts.egg-info/PKG-INFO
 py_draughts.egg-info/SOURCES.txt
 py_draughts.egg-info/dependency_links.txt
 py_draughts.egg-info/requires.txt
 py_draughts.egg-info/top_level.txt
 test/test_american_board.py
-test/test_board.py
+test/test_board.py
+test/test_standard_board.py
```

### Comparing `py-draughts-1.1.7/setup.py` & `py-draughts-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.7/test/test_american_board.py` & `py-draughts-1.2.0/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.7/test/test_board.py` & `py-draughts-1.2.0/test/test_board.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 import numpy as np
 import pytest
 
-import draughts.base as checkers
+import draughts.american as checkers
 from draughts.base import BaseBoard, Color, Figure, Move
+from draughts import get_board
+from draughts.american import Board
 
 
 class TestBoard:
     @pytest.fixture(autouse=True)
     def setup(self):
-        self.board = BaseBoard(BaseBoard.STARTING_POSITION)
+        self.board = get_board("american")
         yield
         del self.board
 
     def test_init(self):
         assert self.board.turn == Color.WHITE
-        assert np.array_equal(self.board.position, BaseBoard.STARTING_POSITION)
+        assert np.array_equal(self.board.position, Board.STARTING_POSITION)
 
-    def test_move(self):
-        m = Move([checkers.A3, checkers.B4])
-        self.board.push(m)
-        assert self.board.turn == Color.BLACK
-        assert self.board[checkers.A3] == Figure.EMPTY
-        assert self.board[checkers.B4] == Figure.WHITE_MAN
-        m = Move([checkers.F6, checkers.G5])
-        self.board.push(m)
-        assert self.board.turn == Color.WHITE
-        assert self.board[checkers.F6] == Figure.EMPTY
-        assert self.board[checkers.G5] == Figure.BLACK_MAN
-
-    def test_capture(self):
-        m1 = Move([checkers.C3, checkers.B4])
-        self.board.push(m1)
-
-        m2 = Move([checkers.B6, checkers.A5])
-        self.board.push(m2)
-
-        m3 = Move([checkers.G3, checkers.H4])
-        self.board.push(m3)
-
-        m4 = Move([checkers.A5, checkers.C3], captured_list=[checkers.B4])
-        self.board.push(m4)
-
-        assert self.board[checkers.B4] == Figure.EMPTY
-        assert self.board[checkers.C3] == Figure.BLACK_MAN
-
-        m5 = Move([checkers.B2, checkers.D4], captured_list=[checkers.C3])
-        self.board.push(m5)
-        assert self.board[checkers.B2] == Figure.EMPTY
-        assert self.board[checkers.C3] == Figure.EMPTY
-        assert self.board[checkers.D4] == Figure.WHITE_MAN
-
-    def test_pop(self):
-        m = Move([checkers.A3, checkers.B4])
-        self.board.push(m)
-        assert self.board.turn == Color.BLACK
-        assert self.board[checkers.A3] == Figure.EMPTY
-        assert self.board[checkers.B4] == Figure.WHITE_MAN
-        m = Move([checkers.F6, checkers.G5])
-        self.board.push(m)
-        self.board.pop()
-        assert self.board.turn == Color.BLACK
-        assert self.board[checkers.F6] == Figure.BLACK_MAN
-        assert self.board[checkers.G5] == Figure.EMPTY
-        assert self.board[checkers.A3] == Figure.EMPTY
-        assert self.board[checkers.B4] == Figure.WHITE_MAN
+    # def test_move(self):
+    #     m = Move([checkers.A3, checkers.B4])
+    #     self.board.push(m)
+    #     assert self.board.turn == Color.BLACK
+    #     assert self.board[checkers.A3] == Figure.EMPTY
+    #     assert self.board[checkers.B4] == Figure.WHITE_MAN
+    #     m = Move([checkers.F6, checkers.G5])
+    #     self.board.push(m)
+    #     assert self.board.turn == Color.WHITE
+    #     assert self.board[checkers.F6] == Figure.EMPTY
+    #     assert self.board[checkers.G5] == Figure.BLACK_MAN
+
+    # def test_capture(self):
+    #     m1 = Move([checkers.C3, checkers.B4])
+    #     self.board.push(m1)
+
+    #     m2 = Move([checkers.B6, checkers.A5])
+    #     self.board.push(m2)
+
+    #     m3 = Move([checkers.G3, checkers.H4])
+    #     self.board.push(m3)
+
+    #     m4 = Move([checkers.A5, checkers.C3], captured_list=[checkers.B4])
+    #     self.board.push(m4)
+
+    #     assert self.board[checkers.B4] == Figure.EMPTY
+    #     assert self.board[checkers.C3] == Figure.BLACK_MAN
+
+    #     m5 = Move([checkers.B2, checkers.D4], captured_list=[checkers.C3])
+    #     self.board.push(m5)
+    #     assert self.board[checkers.B2] == Figure.EMPTY
+    #     assert self.board[checkers.C3] == Figure.EMPTY
+    #     assert self.board[checkers.D4] == Figure.WHITE_MAN
+
+    # def test_pop(self):
+    #     m = Move([checkers.A3, checkers.B4])
+    #     self.board.push(m)
+    #     assert self.board.turn == Color.BLACK
+    #     assert self.board[checkers.A3] == Figure.EMPTY
+    #     assert self.board[checkers.B4] == Figure.WHITE_MAN
+    #     m = Move([checkers.F6, checkers.G5])
+    #     self.board.push(m)
+    #     self.board.pop()
+    #     assert self.board.turn == Color.BLACK
+    #     assert self.board[checkers.F6] == Figure.BLACK_MAN
+    #     assert self.board[checkers.G5] == Figure.EMPTY
+    #     assert self.board[checkers.A3] == Figure.EMPTY
+    #     assert self.board[checkers.B4] == Figure.WHITE_MAN
```

