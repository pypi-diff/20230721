# Comparing `tmp/py-draughts-1.1.61.tar.gz` & `tmp/py-draughts-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-1.1.61.tar", last modified: Tue Jul 18 21:35:15 2023, max compression
+gzip compressed data, was "py-draughts-1.1.7.tar", last modified: Fri Jul 21 08:39:35 2023, max compression
```

## Comparing `py-draughts-1.1.61.tar` & `py-draughts-1.1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 21:35:15.549792 py-draughts-1.1.61/
--rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-1.1.61/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-16 09:45:04.000000 py-draughts-1.1.61/MANIFEST.in
--rw-rw-rw-   0        0        0     5203 2023-07-18 21:35:15.548792 py-draughts-1.1.61/PKG-INFO
--rw-rw-rw-   0        0        0     3779 2023-07-17 12:17:15.000000 py-draughts-1.1.61/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 21:35:15.528973 py-draughts-1.1.61/draughts/
--rw-rw-rw-   0        0        0     1586 2023-07-18 21:35:03.000000 py-draughts-1.1.61/draughts/__init__.py
--rw-rw-rw-   0        0        0     3666 2023-07-16 18:41:37.000000 py-draughts-1.1.61/draughts/american.py
--rw-rw-rw-   0        0        0    12412 2023-07-18 21:25:14.000000 py-draughts-1.1.61/draughts/base.py
--rw-rw-rw-   0        0        0     3663 2023-07-16 18:55:10.000000 py-draughts-1.1.61/draughts/engine.py
--rw-rw-rw-   0        0        0      671 2023-07-16 18:11:48.000000 py-draughts-1.1.61/draughts/models.py
--rw-rw-rw-   0        0        0     4147 2023-07-16 18:11:26.000000 py-draughts-1.1.61/draughts/move.py
--rw-rw-rw-   0        0        0     5607 2023-07-18 21:31:16.000000 py-draughts-1.1.61/draughts/server.py
--rw-rw-rw-   0        0        0     8454 2023-07-18 21:30:46.000000 py-draughts-1.1.61/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:35:15.501934 py-draughts-1.1.61/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-18 21:35:15.529974 py-draughts-1.1.61/draughts/static/css/
--rw-rw-rw-   0        0        0     3873 2023-07-16 09:45:04.000000 py-draughts-1.1.61/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-18 21:35:15.531972 py-draughts-1.1.61/draughts/static/js/
--rw-rw-rw-   0        0        0     6118 2023-07-16 09:50:41.000000 py-draughts-1.1.61/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-18 21:35:15.534974 py-draughts-1.1.61/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-1.1.61/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2882 2023-07-16 09:45:04.000000 py-draughts-1.1.61/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-16 10:59:23.000000 py-draughts-1.1.61/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:35:15.544973 py-draughts-1.1.61/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     5203 2023-07-18 21:35:15.000000 py-draughts-1.1.61/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-07-18 21:35:15.000000 py-draughts-1.1.61/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 21:35:15.000000 py-draughts-1.1.61/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-18 21:35:15.000000 py-draughts-1.1.61/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 21:35:15.000000 py-draughts-1.1.61/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2023-07-16 19:28:37.000000 py-draughts-1.1.61/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 21:35:15.549792 py-draughts-1.1.61/setup.cfg
--rw-rw-rw-   0        0        0     1911 2023-07-18 21:34:49.000000 py-draughts-1.1.61/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:35:15.547793 py-draughts-1.1.61/test/
--rw-rw-rw-   0        0        0     1104 2023-07-16 18:39:54.000000 py-draughts-1.1.61/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-16 09:45:04.000000 py-draughts-1.1.61/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.355822 py-draughts-1.1.7/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-16 08:41:45.000000 py-draughts-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5136 2023-07-21 08:39:35.352821 py-draughts-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3716 2023-07-21 08:29:32.000000 py-draughts-1.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.241823 py-draughts-1.1.7/draughts/
+-rw-rw-rw-   0        0        0     1585 2023-07-21 08:30:22.000000 py-draughts-1.1.7/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3666 2023-07-19 10:32:24.000000 py-draughts-1.1.7/draughts/american.py
+-rw-rw-rw-   0        0        0    12403 2023-07-21 08:27:54.000000 py-draughts-1.1.7/draughts/base.py
+-rw-rw-rw-   0        0        0     3857 2023-07-19 11:00:41.000000 py-draughts-1.1.7/draughts/engine.py
+-rw-rw-rw-   0        0        0      671 2023-07-19 10:32:24.000000 py-draughts-1.1.7/draughts/models.py
+-rw-rw-rw-   0        0        0     4179 2023-07-21 08:25:28.000000 py-draughts-1.1.7/draughts/move.py
+-rw-rw-rw-   0        0        0     5595 2023-07-21 08:28:34.000000 py-draughts-1.1.7/draughts/server.py
+-rw-rw-rw-   0        0        0     8462 2023-07-21 08:22:34.000000 py-draughts-1.1.7/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.145825 py-draughts-1.1.7/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.254821 py-draughts-1.1.7/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-13 16:31:38.000000 py-draughts-1.1.7/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.268823 py-draughts-1.1.7/draughts/static/js/
+-rw-rw-rw-   0        0        0     6118 2023-07-19 10:32:24.000000 py-draughts-1.1.7/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.290826 py-draughts-1.1.7/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-13 13:19:03.000000 py-draughts-1.1.7/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2882 2023-07-16 09:39:24.000000 py-draughts-1.1.7/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-19 10:32:24.000000 py-draughts-1.1.7/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.330821 py-draughts-1.1.7/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     5136 2023-07-21 08:39:35.000000 py-draughts-1.1.7/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-07-21 08:39:35.000000 py-draughts-1.1.7/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 08:39:35.000000 py-draughts-1.1.7/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-21 08:39:35.000000 py-draughts-1.1.7/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 08:39:35.000000 py-draughts-1.1.7/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-07-19 10:32:24.000000 py-draughts-1.1.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 08:39:35.355822 py-draughts-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1908 2023-07-16 08:44:01.000000 py-draughts-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 08:39:35.345821 py-draughts-1.1.7/test/
+-rw-rw-rw-   0        0        0     1104 2023-07-19 10:32:24.000000 py-draughts-1.1.7/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-13 17:33:45.000000 py-draughts-1.1.7/test/test_board.py
```

### Comparing `py-draughts-1.1.61/LICENSE` & `py-draughts-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.61/PKG-INFO` & `py-draughts-1.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.1.61
+Version: 1.1.7
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
-Home-page: https://github.com/michalskibinski109/py-draughts
+Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,14 @@
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
 [![Downloads](https://static.pepy.tech/badge/py-draughts)](https://pepy.tech/project/py-draughts)
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
-_inspired by [python-chess](https://pypi.org/project/chess/)_
 
 ## Installation
 
 ```bash
 pip install py-draughts
 ```
```

### Comparing `py-draughts-1.1.61/README.md` & `py-draughts-1.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
 [![Downloads](https://static.pepy.tech/badge/py-draughts)](https://pepy.tech/project/py-draughts)
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
-_inspired by [python-chess](https://pypi.org/project/chess/)_
 
 ## Installation
 
 ```bash
 pip install py-draughts
 ```
```

### Comparing `py-draughts-1.1.61/draughts/__init__.py` & `py-draughts-1.1.7/draughts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 A draughts library with advenced (customizable) WEB UI move generation and validation,
 PDN parsing and writing. Supports multiple variants of game.
 """
 
 from typing import Literal
 
-__version__ = "1.1.61"
+__version__ = "1.1.7"
 __author__ = "Michał Skibiński"
 
 
 def get_board(variant: Literal["standard", "american"], fen: str = None):
     """
     Board factory method.
     - ``standard`` - standard draughts board
```

### Comparing `py-draughts-1.1.61/draughts/american.py` & `py-draughts-1.1.7/draughts/american.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.61/draughts/base.py` & `py-draughts-1.1.7/draughts/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,23 +94,23 @@
         Initializes the board with a starting position.
         The starting position must be a numpy array of length n * n/2,
         where n is the size of the board.
 
         """
         super().__init__()
         self._pos = starting_position.copy()
+        self.turn = self.STARTING_COLOR
         size = int(np.sqrt(len(self.position) * 2))
         if size**2 != len(self.position) * 2:
             msg = f"Invalid board with shape {starting_position.shape} provided.\
                 Please use an array with lenght = (n * n/2). \
                 Where n is an size of the board."
             logger.error(msg)
             raise ValueError(msg)
         self.shape = (size, size)
-        self.turn = Color.WHITE
         self._moves_stack: list[Move] = []
         logger.info(f"Board initialized with shape {self.shape}.")
 
     # @abstractmethod
     @property
     def legal_moves(self) -> Generator[Move, None, None]:
         """
@@ -147,15 +147,17 @@
     @property
     def game_over(self) -> bool:
         """Returns ``True`` if the game is over."""
         # check if threefold repetition
 
         return self.is_draw or not bool(list(self.legal_moves))
 
-    def push(self, move: Move, is_finished: bool = True) -> None:
+    def push(
+        self, move: Move, is_finished: bool = True
+    ) -> None:  # TODO multiple captures != promotion
         """Pushes a move to the board.
         Automatically promotes a piece if it reaches the last row.
 
         If ``is_finished`` is set to ``True``, the turn is switched. This parameter is used only
         for generating legal moves.
         """
         src, tg = (
@@ -163,17 +165,19 @@
             move.square_list[-1],
         )
         self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
         # is promotion
         if (
             (tg // (self.shape[0] // 2)) == 0
             and self._pos[tg] == Figure.WHITE_MAN.value
+            and is_finished
         ) or (
             (tg // (self.shape[0] // 2)) == (self.shape[0] - 1)
             and self._pos[tg] == Figure.BLACK_MAN.value
+            and is_finished
         ):
             self._pos[tg] *= Figure.KING.value
             move.is_promotion = True
         if move.captured_list:
             self._pos[np.array([sq for sq in move.captured_list])] = Figure.EMPTY
         self._moves_stack.append(move)
         if is_finished:
@@ -245,15 +249,15 @@
     def from_fen(cls, fen: str) -> BaseBoard:
         """
         Creates a board from a FEN string by using regular expressions.
         """
         fen = fen.upper()
         re_turn = re.compile(r"[WB]:")
         re_premove = re.compile(r"(G[0-9]+|P[0-9]+)(,|)")
-        re_prefix = re.compile(r"[WB]:[WB]:[WB]:")
+        re_prefix = re.compile(r"[WB]:[WB]:[WB]")
         re_white = re.compile(r"W[0-9K,]+")
         re_black = re.compile(r"B[0-9K,]+")
         # remove premoves from fen
         # remove first 2 letters from prefix
         fen = re_premove.sub("", fen)
         prefix = re_prefix.search(fen)
         if prefix:
@@ -271,14 +275,15 @@
             raise ValueError(f"Invalid FEN: {fen}")
         try:
             cls.__populate_from_list(white.split(","), Color.WHITE)
             cls.__populate_from_list(black.split(","), Color.BLACK)
         except ValueError as e:
             logger.error(f"Invalid FEN: {fen} \n {e}")
         cls.turn = Color.WHITE if turn == "W" else Color.BLACK
+        cls.STARTING_COLOR = cls.turn
         return cls(starting_position=cls.STARTING_POSITION)
 
     @classmethod
     def __populate_from_list(cls, fen_list: list[str], color: Color) -> None:
         board_range = range(1, cls.STARTING_POSITION.shape[0] + 1)
         for sq in fen_list:
             if sq.isdigit() and int(sq) in board_range:
@@ -339,20 +344,16 @@
             yield sq
 
     def __getitem__(self, key: SquareT) -> Figure:
         return self.position[key]
 
 
 if __name__ == "__main__":
-    # board = BaseBoard(BaseBoard.STARTING_POSITION)
+    board = BaseBoard(BaseBoard.STARTING_POSITION)
     # print(board)
-    board = BaseBoard.from_fen("W:W:WG23:BP12,K19,K28")
-    print(board)
-    BaseBoard.from_fen("W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32")
-
 # print(board.info)
 #     m1 = Move([C3, B4])
 #     board.push(m1)
 
 #     m2 = Move([B6, A5])
 #     board.push(m2)
```

### Comparing `py-draughts-1.1.61/draughts/engine.py` & `py-draughts-1.1.7/draughts/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,25 +59,27 @@
     def __get_engine_move(self, board: Board) -> tuple:
         depth = self.depth
         legal_moves = list(board.legal_moves)
         legal_moves.sort(key=lambda move: board.is_capture(move), reverse=True)
         bar = tqdm(legal_moves)
         evals = []
         alpha, beta = -100, 100
+
         for move in legal_moves:
             board.push(move)
             evals.append(
                 self.__alpha_beta_puring(
                     board,
                     depth - 1,
                     alpha,
                     beta,
                 )
             )
             board.pop()
+
             bar.update(1)
             if board.turn == Color.WHITE:
                 alpha = max(alpha, evals[-1])
             else:
                 beta = min(beta, evals[-1])
         index = (
             evals.index(max(evals))
@@ -92,18 +94,24 @@
         if board.game_over:
             return -100 if board.turn == Color.WHITE else 100
         if depth == 0:
             self.inspected_nodes += 1
             return self.evaluate(board)
         legal_moves = list(board.legal_moves)
         legal_moves.sort(key=lambda move: board.is_capture(move), reverse=True)
+        tmp = board._pos.copy().sum()
+
         for move in legal_moves:
             board.push(move)
             evaluation = self.__alpha_beta_puring(board, depth - 1, alpha, beta)
             board.pop()
+            if board._pos.sum() != tmp:
+                logger.warning(str(board))
+                logger.error(f"{move}")
+                break
             if board.turn == Color.WHITE:
                 alpha = max(alpha, evaluation)
             else:
                 beta = min(beta, evaluation)
             if beta <= alpha:
                 break
         return alpha if board.turn == Color.WHITE else beta
```

### Comparing `py-draughts-1.1.61/draughts/models.py` & `py-draughts-1.1.7/draughts/models.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.61/draughts/move.py` & `py-draughts-1.1.7/draughts/move.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
             raise ValueError(
                 f"Cannot append moves {self} and {other}. Last square of first move should be equal to first square of second move."
             )
         return Move(
             self.square_list + other.square_list[1:],
             self.captured_list + other.captured_list,
             self.captured_entities + other.captured_entities,
+            self.is_promotion,
         )
 
     @classmethod
     def from_uci(cls, move: str, legal_moves: Generator) -> Move:
         """
 
         Converts string representation of move to ``Move`` object.
```

### Comparing `py-draughts-1.1.61/draughts/server.py` & `py-draughts-1.1.7/draughts/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,14 @@
         uvicorn.run(self.APP, **kwargs)
 
 
 if __name__ == "__main__":
     from draughts.engine import AlphaBetaEngine
     from draughts import get_board
 
-    engine = AlphaBetaEngine(depth=2)
-    # board = get_board(
-    #     "standard",
-    #     '[FEN "B:W18,26,28,29,32,33,38,39,41,45,46,47,48,49,50:B4,5,7,8,9,10,11,12,13,15,16,17,19,20"]',
-    # )
-    server = Server(get_best_move_method=engine.get_best_move)
+    engine = AlphaBetaEngine(depth=4)
+    board = get_board(
+        "standard",
+        '[FEN "W:B:W23,27,29,33,34,37,42,45,46,50:B5,8,9,10,12,13,14,15,16,17,20,36"]',
+    )
+    server = Server(board=board, get_best_move_method=engine.get_best_move)
     server.run()
```

### Comparing `py-draughts-1.1.61/draughts/standard.py` & `py-draughts-1.1.7/draughts/standard.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             ):
                 move = Move(
                     [square, direction[1]], [direction[0]], [self._pos[direction[0]]]
                 )
                 # moves.append(move)
                 self.push(move, False)
                 new_moves = [
-                    move + m for m in self._legal_moves_from(direction[1], True)
+                    move + m for m in self._get_man_legal_moves_from(direction[1], True)
                 ]
                 moves += [move] if len(new_moves) == 0 else new_moves
                 self.pop(False)
         return moves
 
     def _get_king_legal_moves_from(
         self, square: int, is_capture_mandatory: bool
```

### Comparing `py-draughts-1.1.61/draughts/static/css/style.css` & `py-draughts-1.1.7/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.61/draughts/static/js/script.js` & `py-draughts-1.1.7/draughts/static/js/script.js`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.61/draughts/templates/base.html` & `py-draughts-1.1.7/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.61/draughts/templates/index.html` & `py-draughts-1.1.7/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.61/draughts/utils.py` & `py-draughts-1.1.7/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.61/py_draughts.egg-info/PKG-INFO` & `py-draughts-1.1.7/py_draughts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.1.61
+Version: 1.1.7
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
-Home-page: https://github.com/michalskibinski109/py-draughts
+Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,14 @@
 [![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
 [![Downloads](https://static.pepy.tech/badge/py-draughts)](https://pepy.tech/project/py-draughts)
 
 Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
 Supports multiple variants of the game and allows playing against AI.
 
-_inspired by [python-chess](https://pypi.org/project/chess/)_
 
 ## Installation
 
 ```bash
 pip install py-draughts
 ```
```

### Comparing `py-draughts-1.1.61/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.1.7/py_draughts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.61/setup.py` & `py-draughts-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     long_description=long_description,
     # rst
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     package_data={"draughts": ["static/js/*", "static/css/*", "templates/*"]},
     license="GPL-3.0+",
     keywords=" draughts, checkers, AI mini-max, game, board",
-    url="https://github.com/michalskibinski109/py-draughts",
+    url="https://github.com/michalskibinski109/draughts",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `py-draughts-1.1.61/test/test_american_board.py` & `py-draughts-1.1.7/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.1.61/test/test_board.py` & `py-draughts-1.1.7/test/test_board.py`

 * *Files identical despite different names*

