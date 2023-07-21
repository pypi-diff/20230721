# Comparing `tmp/py-draughts-1.2.0.tar.gz` & `tmp/py-draughts-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-1.2.0.tar", last modified: Fri Jul 21 13:22:15 2023, max compression
+gzip compressed data, was "py-draughts-1.2.1.tar", last modified: Fri Jul 21 15:01:08 2023, max compression
```

## Comparing `py-draughts-1.2.0.tar` & `py-draughts-1.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.846282 py-draughts-1.2.0/
--rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-1.2.0/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-16 08:41:45.000000 py-draughts-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5136 2023-07-21 13:22:15.844281 py-draughts-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3716 2023-07-21 08:29:32.000000 py-draughts-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.784279 py-draughts-1.2.0/draughts/
--rw-rw-rw-   0        0        0     1585 2023-07-21 13:21:47.000000 py-draughts-1.2.0/draughts/__init__.py
--rw-rw-rw-   0        0        0     3763 2023-07-21 12:56:50.000000 py-draughts-1.2.0/draughts/american.py
--rw-rw-rw-   0        0        0    13482 2023-07-21 13:12:47.000000 py-draughts-1.2.0/draughts/base.py
--rw-rw-rw-   0        0        0     3857 2023-07-21 09:39:46.000000 py-draughts-1.2.0/draughts/engine.py
--rw-rw-rw-   0        0        0      671 2023-07-19 10:32:24.000000 py-draughts-1.2.0/draughts/models.py
--rw-rw-rw-   0        0        0     4179 2023-07-21 08:25:28.000000 py-draughts-1.2.0/draughts/move.py
--rw-rw-rw-   0        0        0     5441 2023-07-21 12:58:57.000000 py-draughts-1.2.0/draughts/server.py
--rw-rw-rw-   0        0        0     8403 2023-07-21 13:16:43.000000 py-draughts-1.2.0/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.719330 py-draughts-1.2.0/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.790277 py-draughts-1.2.0/draughts/static/css/
--rw-rw-rw-   0        0        0     3873 2023-07-13 16:31:38.000000 py-draughts-1.2.0/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.796276 py-draughts-1.2.0/draughts/static/js/
--rw-rw-rw-   0        0        0     6118 2023-07-19 10:32:24.000000 py-draughts-1.2.0/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.805240 py-draughts-1.2.0/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-13 13:19:03.000000 py-draughts-1.2.0/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2882 2023-07-16 09:39:24.000000 py-draughts-1.2.0/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-19 10:32:24.000000 py-draughts-1.2.0/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.827274 py-draughts-1.2.0/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     5136 2023-07-21 13:22:15.000000 py-draughts-1.2.0/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      594 2023-07-21 13:22:15.000000 py-draughts-1.2.0/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 13:22:15.000000 py-draughts-1.2.0/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-21 13:22:15.000000 py-draughts-1.2.0/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 13:22:15.000000 py-draughts-1.2.0/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2023-07-19 10:32:24.000000 py-draughts-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 13:22:15.846282 py-draughts-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1908 2023-07-16 08:44:01.000000 py-draughts-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 13:22:15.840269 py-draughts-1.2.0/test/
--rw-rw-rw-   0        0        0     1104 2023-07-19 10:32:24.000000 py-draughts-1.2.0/test/test_american_board.py
--rw-rw-rw-   0        0        0     2510 2023-07-21 13:07:31.000000 py-draughts-1.2.0/test/test_board.py
--rw-rw-rw-   0        0        0     1370 2023-07-21 13:21:26.000000 py-draughts-1.2.0/test/test_standard_board.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:01:08.952460 py-draughts-1.2.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-16 09:45:04.000000 py-draughts-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5139 2023-07-21 15:01:08.951460 py-draughts-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3716 2023-07-21 15:00:24.000000 py-draughts-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 15:01:08.903446 py-draughts-1.2.1/draughts/
+-rw-rw-rw-   0        0        0     1585 2023-07-21 15:00:47.000000 py-draughts-1.2.1/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3740 2023-07-21 14:37:08.000000 py-draughts-1.2.1/draughts/american.py
+-rw-rw-rw-   0        0        0    13510 2023-07-21 14:37:08.000000 py-draughts-1.2.1/draughts/base.py
+-rw-rw-rw-   0        0        0     3695 2023-07-21 14:37:08.000000 py-draughts-1.2.1/draughts/engine.py
+-rw-rw-rw-   0        0        0      671 2023-07-16 18:11:48.000000 py-draughts-1.2.1/draughts/models.py
+-rw-rw-rw-   0        0        0     4179 2023-07-21 14:37:08.000000 py-draughts-1.2.1/draughts/move.py
+-rw-rw-rw-   0        0        0     5541 2023-07-21 15:00:27.000000 py-draughts-1.2.1/draughts/server.py
+-rw-rw-rw-   0        0        0     8403 2023-07-21 14:37:08.000000 py-draughts-1.2.1/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:01:08.865479 py-draughts-1.2.1/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-21 15:01:08.910417 py-draughts-1.2.1/draughts/static/css/
+-rw-rw-rw-   0        0        0     3873 2023-07-16 09:45:04.000000 py-draughts-1.2.1/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-21 15:01:08.912833 py-draughts-1.2.1/draughts/static/js/
+-rw-rw-rw-   0        0        0     6250 2023-07-21 14:37:08.000000 py-draughts-1.2.1/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-21 15:01:08.915835 py-draughts-1.2.1/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-1.2.1/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2882 2023-07-16 09:45:04.000000 py-draughts-1.2.1/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-16 10:59:23.000000 py-draughts-1.2.1/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:01:08.928362 py-draughts-1.2.1/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     5139 2023-07-21 15:01:08.000000 py-draughts-1.2.1/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2023-07-21 15:01:08.000000 py-draughts-1.2.1/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 15:01:08.000000 py-draughts-1.2.1/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-21 15:01:08.000000 py-draughts-1.2.1/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-21 15:01:08.000000 py-draughts-1.2.1/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-07-16 19:28:37.000000 py-draughts-1.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 15:01:08.952460 py-draughts-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1911 2023-07-18 21:34:49.000000 py-draughts-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 15:01:08.948951 py-draughts-1.2.1/test/
+-rw-rw-rw-   0        0        0     1104 2023-07-16 18:39:54.000000 py-draughts-1.2.1/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2510 2023-07-21 14:37:08.000000 py-draughts-1.2.1/test/test_board.py
+-rw-rw-rw-   0        0        0     1370 2023-07-21 14:37:08.000000 py-draughts-1.2.1/test/test_standard_board.py
```

### Comparing `py-draughts-1.2.0/LICENSE` & `py-draughts-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.0/PKG-INFO` & `py-draughts-1.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.2.0
+Version: 1.2.1
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
-Home-page: https://github.com/michalskibinski109/draughts
+Home-page: https://github.com/michalskibinski109/py-draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -146,15 +146,15 @@
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 ```
 
 _It is as simple as that!_
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/a7d67a8a-a325-437e-90b5-ba443d1b0874" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/11e4b7ea-4b47-4ab2-80b8-6d6cf1052869" width="800" />
 
 
 ## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 ## Bibliography
```

### Comparing `py-draughts-1.2.0/README.md` & `py-draughts-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 ```
 
 _It is as simple as that!_
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/a7d67a8a-a325-437e-90b5-ba443d1b0874" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/11e4b7ea-4b47-4ab2-80b8-6d6cf1052869" width="800" />
 
 
 ## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 ## Bibliography
```

### Comparing `py-draughts-1.2.0/draughts/__init__.py` & `py-draughts-1.2.1/draughts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """
 A draughts library with advenced (customizable) WEB UI move generation and validation,
 PDN parsing and writing. Supports multiple variants of game.
 """
 
 from typing import Literal
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 __author__ = "Michał Skibiński"
 
 
 def get_board(variant: Literal["standard", "american"], fen: str = None):
     """
     Board factory method.
     - ``standard`` - standard draughts board
```

### Comparing `py-draughts-1.2.0/draughts/american.py` & `py-draughts-1.2.1/draughts/american.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,13 @@
                 moves += [move + m for m in self._legal_moves_from(capture_sq, True)]
                 self.pop(False)
 
         return moves
 
 
 if __name__ == "__main__":
-    board = Board()
-    from draughts.server import Server
+    from draughts.standard import Board as StandardBoard
 
-    Server(board).run()
-    moves = ["24-20", "11-16", "20x11", "7x16"]
-    for m in moves:
-        board.push_uci(m)
-        print(list(board.legal_moves))
+    board = BaseBoard(BaseBoard.STARTING_POSITION, Color.WHITE)
+    print(board.GAME_TYPE)
+    board = Board()
+    print(board.GAME_TYPE)
```

### Comparing `py-draughts-1.2.0/draughts/base.py` & `py-draughts-1.2.1/draughts/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,25 +123,25 @@
             starting_position
             if starting_position is not None
             else self.STARTING_POSITION
         )
         self.turn = turn if turn is not None else self.STARTING_COLOR
         size = int(np.sqrt(len(self.position) * 2))
         if size**2 != len(self.position) * 2:
-            msg = f"Invalid board with shape {starting_position.shape} provided.\
+            msg = f"Invalid board with shape {self._pos.shape} provided.\
                 Please use an array with lenght = (n * n/2). \
                 Where n is an size of the board."
             logger.error(msg)
             raise ValueError(msg)
         self.shape = (size, size)
         self._moves_stack: list[Move] = []
         logger.info(f"Board initialized with shape {self.shape}.")
 
     # @abstractmethod
-    @property
+    @abstractproperty
     def legal_moves(self) -> Generator[Move, None, None]:
         """
         Return list legal moves for the current position.
         *For every concrete variant of draughts this method should be overriden.*
 
         .. warning::
             Depending of implementation method can return generator or list.
@@ -371,14 +371,15 @@
 
     def __getitem__(self, key: SquareT) -> Figure:
         return self.position[key]
 
 
 if __name__ == "__main__":
     board = BaseBoard(BaseBoard.STARTING_POSITION, Color.WHITE)
+    print(board.GAME_TYPE)
     # print(board)
 # print(board.info)
 #     m1 = Move([C3, B4])
 #     board.push(m1)
 
 #     m2 = Move([B6, A5])
 #     board.push(m2)
```

### Comparing `py-draughts-1.2.0/draughts/engine.py` & `py-draughts-1.2.1/draughts/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         if with_evaluation:
             return move, evaluation
         return move
 
     def __get_engine_move(self, board: Board) -> tuple:
         depth = self.depth
         legal_moves = list(board.legal_moves)
-        legal_moves.sort(key=lambda move: board.is_capture(move), reverse=True)
         bar = tqdm(legal_moves)
         evals = []
         alpha, beta = -100, 100
 
         for move in legal_moves:
             board.push(move)
             evals.append(
@@ -93,15 +92,14 @@
     ) -> float:
         if board.game_over:
             return -100 if board.turn == Color.WHITE else 100
         if depth == 0:
             self.inspected_nodes += 1
             return self.evaluate(board)
         legal_moves = list(board.legal_moves)
-        legal_moves.sort(key=lambda move: board.is_capture(move), reverse=True)
         tmp = board._pos.copy().sum()
 
         for move in legal_moves:
             board.push(move)
             evaluation = self.__alpha_beta_puring(board, depth - 1, alpha, beta)
             board.pop()
             if board._pos.sum() != tmp:
```

### Comparing `py-draughts-1.2.0/draughts/models.py` & `py-draughts-1.2.1/draughts/models.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.0/draughts/move.py` & `py-draughts-1.2.1/draughts/move.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.0/draughts/server.py` & `py-draughts-1.2.1/draughts/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,19 +82,20 @@
         }
 
     @property
     def position_json(self) -> PositionResponse:
         history = []  # (numver, white, black)
         stack = self.board._moves_stack
         for idx in range(len(stack)):
-            src, tg = stack[idx].square_list[0] + 1, stack[idx].square_list[-1]
+            src, tg = stack[idx].square_list[0] + 1, stack[idx].square_list[-1] + 1
+            separator = "-" if len(stack[idx].captured_list) == 0 else "x"
             if idx % 2 == 0:
-                history.append([(idx // 2) + 1, f"{src}-{tg}"])
+                history.append([(idx // 2) + 1, f"{src}{separator}{tg}"])
             else:
-                history[-1].append(f"{src}-{tg}")
+                history[-1].append(f"{src}{separator}{tg}")
         turn = "white" if self.board.turn == Color.WHITE else "black"
         return PositionResponse(
             position=self.board.friendly_form.tolist(),
             history=history,
             turn=turn,
         )
 
@@ -142,10 +143,10 @@
         uvicorn.run(self.APP, **kwargs)
 
 
 if __name__ == "__main__":
     from draughts.engine import AlphaBetaEngine
     from draughts import get_board
 
-    engine = AlphaBetaEngine(depth=6)
+    engine = AlphaBetaEngine(depth=2)
     server = Server(get_best_move_method=engine.get_best_move)
     server.run()
```

### Comparing `py-draughts-1.2.0/draughts/standard.py` & `py-draughts-1.2.1/draughts/standard.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     - When one player has only a king left, and the other player two pieces
       or less including at least one king (one king, two kings, or one king and a man),
       the game is drawn after both players made 5 moves.
 
     """
 
     GAME_TYPE = 20
-    STARTING_POSITION = np.array([1] * 15 + [0] * 20 + [-1] * 15, dtype=np.int8)
+    STARTING_POSITION = np.array([1] * 20 + [0] * 10 + [-1] * 20, dtype=np.int8)
     STARTING_COLOR = Color.WHITE
 
     ROW_IDX = {val: val // 5 for val in range(len(STARTING_POSITION))}
     COL_IDX = {val: val % 10 for val in range(len(STARTING_POSITION))}
 
     # def __init__(
     #     self, starting_position=STARTING_POSITION, turn=STARTING_COLOR, *args, **kwargs
```

### Comparing `py-draughts-1.2.0/draughts/static/css/style.css` & `py-draughts-1.2.1/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.0/draughts/static/js/script.js` & `py-draughts-1.2.1/draughts/static/js/script.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -76,18 +76,22 @@
         })
     );
 
 const makeBestMove = () => {
     $.ajax({
         url: "best_move",
         type: "GET",
+        beforeSend: function() {
+            $("#makeMove").prop("disabled", true);
+        },
         success: (data) => {
             boardArray = data["position"];
             historyData = data["history"];
             turn = data["turn"];
+            $("#makeMove").prop("disabled", false);
             upadateBoard();
         },
     });
 };
 
 const pop = () => {
     $.ajax({
```

### Comparing `py-draughts-1.2.0/draughts/templates/base.html` & `py-draughts-1.2.1/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.0/draughts/templates/index.html` & `py-draughts-1.2.1/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.0/draughts/utils.py` & `py-draughts-1.2.1/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.0/py_draughts.egg-info/PKG-INFO` & `py-draughts-1.2.1/py_draughts.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 1.2.0
+Version: 1.2.1
 Summary: A draughts library with advenced (customizable) WEB UI move generation and validation, PDN parsing and writing. Supports multiple variants of game.
-Home-page: https://github.com/michalskibinski109/draughts
+Home-page: https://github.com/michalskibinski109/py-draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/py-draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -146,15 +146,15 @@
 INFO:     Waiting for application startup.
 INFO:     Application startup complete.
 INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
 ```
 
 _It is as simple as that!_
 
-<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/a7d67a8a-a325-437e-90b5-ba443d1b0874" width="800" />
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/11e4b7ea-4b47-4ab2-80b8-6d6cf1052869" width="800" />
 
 
 ## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 ## Bibliography
```

### Comparing `py-draughts-1.2.0/py_draughts.egg-info/SOURCES.txt` & `py-draughts-1.2.1/py_draughts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.0/setup.py` & `py-draughts-1.2.1/setup.py`

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
-    url="https://github.com/michalskibinski109/draughts",
+    url="https://github.com/michalskibinski109/py-draughts",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `py-draughts-1.2.0/test/test_american_board.py` & `py-draughts-1.2.1/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.0/test/test_board.py` & `py-draughts-1.2.1/test/test_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-1.2.0/test/test_standard_board.py` & `py-draughts-1.2.1/test/test_standard_board.py`

 * *Files identical despite different names*

