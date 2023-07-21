# Comparing `tmp/pgx-1.0.0.tar.gz` & `tmp/pgx-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-1.0.0.tar", last modified: Tue Jun 20 05:59:32 2023, max compression
+gzip compressed data, was "pgx-1.1.0.tar", last modified: Fri Jul 21 03:23:25 2023, max compression
```

## Comparing `pgx-1.0.0.tar` & `pgx-1.1.0.tar`

### file list

```diff
@@ -1,137 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:32.348621 pgx-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 05:59:20.000000 pgx-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17095 2023-06-20 05:59:32.348621 pgx-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-06-20 05:59:20.000000 pgx-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:32.320621 pgx-1.0.0/pgx/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:32.324621 pgx-1.0.0/pgx/_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_mahjong/_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_mahjong/_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_mahjong/_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_mahjong/_meld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_mahjong/_shanten.py
--rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_mahjong/_yaku.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:32.324621 pgx-1.0.0/pgx/_mahjong/cache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_mahjong/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:32.328621 pgx-1.0.0/pgx/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/api_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:32.328621 pgx-1.0.0/pgx/_src/assets/
--rw-r--r--   0 runner    (1001) docker     (123)  2657333 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/assets/between.npy
--rw-r--r--   0 runner    (1001) docker     (123)    91982 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/assets/can_move.npy
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/chess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:32.332621 pgx-1.0.0/pgx/_src/dwg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/animalshogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/gardner_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:32.332621 pgx-1.0.0/pgx/_src/dwg/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:32.336621 pgx-1.0.0/pgx/_src/dwg/images/chess/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/chess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/chess/bBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/chess/bKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/chess/bKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/chess/bPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/chess/bQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/chess/bRook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/chess/wBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/chess/wKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/chess/wKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/chess/wPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/chess/wQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/chess/wRook.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:32.340621 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/dwg/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/gardner_chess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/shogi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24056 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/_src/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)    39557 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    31606 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/connect_four.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:32.344621 pgx-1.0.0/pgx/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-20 05:59:20.000000 pgx-1.0.0/pgx/experimental/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-20 05:59:21.000000 pgx-1.0.0/pgx/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-20 05:59:21.000000 pgx-1.0.0/pgx/experimental/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-20 05:59:21.000000 pgx-1.0.0/pgx/experimental/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-06-20 05:59:21.000000 pgx-1.0.0/pgx/gardner_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-06-20 05:59:21.000000 pgx-1.0.0/pgx/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-20 05:59:21.000000 pgx-1.0.0/pgx/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-20 05:59:21.000000 pgx-1.0.0/pgx/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-20 05:59:21.000000 pgx-1.0.0/pgx/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-20 05:59:21.000000 pgx-1.0.0/pgx/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-06-20 05:59:21.000000 pgx-1.0.0/pgx/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-06-20 05:59:21.000000 pgx-1.0.0/pgx/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-06-20 05:59:21.000000 pgx-1.0.0/pgx/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-20 05:59:21.000000 pgx-1.0.0/pgx/tic_tac_toe.py
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-06-20 05:59:21.000000 pgx-1.0.0/pgx/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:32.324621 pgx-1.0.0/pgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17095 2023-06-20 05:59:32.000000 pgx-1.0.0/pgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-20 05:59:32.000000 pgx-1.0.0/pgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 05:59:32.000000 pgx-1.0.0/pgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 05:59:32.000000 pgx-1.0.0/pgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 05:59:32.000000 pgx-1.0.0/pgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-20 05:59:21.000000 pgx-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 05:59:32.348621 pgx-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-20 05:59:21.000000 pgx-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:32.348621 pgx-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    17919 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)    75314 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    46618 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)    41511 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_gardner_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)    39841 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    22440 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-20 05:59:21.000000 pgx-1.0.0/tests/test_tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:25.890104 pgx-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 03:23:06.000000 pgx-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15363 2023-07-21 03:23:25.886104 pgx-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-07-21 03:23:06.000000 pgx-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:25.854104 pgx-1.1.0/pgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-21 03:23:06.000000 pgx-1.1.0/pgx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:25.858104 pgx-1.1.0/pgx/_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:06.000000 pgx-1.1.0/pgx/_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-21 03:23:06.000000 pgx-1.1.0/pgx/_mahjong/_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-07-21 03:23:06.000000 pgx-1.1.0/pgx/_mahjong/_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-21 03:23:06.000000 pgx-1.1.0/pgx/_mahjong/_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-07-21 03:23:06.000000 pgx-1.1.0/pgx/_mahjong/_mahjong2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-21 03:23:06.000000 pgx-1.1.0/pgx/_mahjong/_meld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-21 03:23:06.000000 pgx-1.1.0/pgx/_mahjong/_shanten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-07-21 03:23:06.000000 pgx-1.1.0/pgx/_mahjong/_yaku.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:25.858104 pgx-1.1.0/pgx/_mahjong/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:06.000000 pgx-1.1.0/pgx/_mahjong/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:25.862104 pgx-1.1.0/pgx/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/api_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:25.866104 pgx-1.1.0/pgx/_src/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  2657333 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/assets/between.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    91982 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/assets/can_move.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/chess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:25.870104 pgx-1.1.0/pgx/_src/dwg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/animalshogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/gardner_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:25.870104 pgx-1.1.0/pgx/_src/dwg/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:25.874104 pgx-1.1.0/pgx/_src/dwg/images/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/chess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/chess/bBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/chess/bKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/chess/bKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/chess/bPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/chess/bQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/chess/bRook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/chess/wBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/chess/wKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/chess/wKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/chess/wPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/chess/wQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/chess/wRook.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:25.882104 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)   521809 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/mahjong_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/dwg/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/gardner_chess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/shogi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/_src/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39557 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/connect_four.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:25.882104 pgx-1.1.0/pgx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/experimental/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/experimental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/experimental/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/experimental/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/gardner_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/tic_tac_toe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-07-21 03:23:07.000000 pgx-1.1.0/pgx/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:25.854104 pgx-1.1.0/pgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15363 2023-07-21 03:23:25.000000 pgx-1.1.0/pgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-21 03:23:25.000000 pgx-1.1.0/pgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 03:23:25.000000 pgx-1.1.0/pgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 03:23:25.000000 pgx-1.1.0/pgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 03:23:25.000000 pgx-1.1.0/pgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-21 03:23:07.000000 pgx-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 03:23:25.890104 pgx-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-21 03:23:07.000000 pgx-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:25.886104 pgx-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17919 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75314 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47401 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41511 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_gardner_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39841 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22440 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-21 03:23:07.000000 pgx-1.1.0/tests/test_tic_tac_toe.py
```

### Comparing `pgx-1.0.0/LICENSE` & `pgx-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/PKG-INFO` & `pgx-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,1069 +1,932 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7067 780a  : 2.1.Name: pgx.
-00000020: 5665 7273 696f 6e3a 2031 2e30 2e30 0a53  Version: 1.0.0.S
-00000030: 756d 6d61 7279 3a20 4750 552f 5450 552d  ummary: GPU/TPU-
-00000040: 6163 6365 6c65 7261 7465 6420 7061 7261  accelerated para
-00000050: 6c6c 656c 2067 616d 6520 7369 6d75 6c61  llel game simula
-00000060: 746f 7273 2066 6f72 2072 6569 6e66 6f72  tors for reinfor
-00000070: 6365 6d65 6e74 206c 6561 726e 696e 6720  cement learning 
-00000080: 2852 4c29 0a48 6f6d 652d 7061 6765 3a20  (RL).Home-page: 
-00000090: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000000a0: 6f6d 2f73 6f74 6574 7375 6b2f 7067 780a  om/sotetsuk/pgx.
-000000b0: 4175 7468 6f72 3a20 536f 7465 7473 7520  Author: Sotetsu 
-000000c0: 4b4f 5941 4d41 4441 0a41 7574 686f 722d  KOYAMADA.Author-
-000000d0: 656d 6169 6c3a 2073 6f74 6574 7375 2e6b  email: sotetsu.k
-000000e0: 6f79 616d 6164 6140 676d 6169 6c2e 636f  oyamada@gmail.co
-000000f0: 6d0a 436c 6173 7369 6669 6572 3a20 5072  m.Classifier: Pr
-00000100: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000110: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000120: 332e 380a 436c 6173 7369 6669 6572 3a20  3.8.Classifier: 
-00000130: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000140: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000150: 3a20 332e 390a 436c 6173 7369 6669 6572  : 3.9.Classifier
-00000160: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000170: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000180: 203a 3a20 332e 3130 0a44 6573 6372 6970   :: 3.10.Descrip
-00000190: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-000001a0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-000001b0: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
-000001c0: 4943 454e 5345 0a0a 5b21 5b63 695d 2868  ICENSE..[![ci](h
-000001d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000001e0: 6d2f 736f 7465 7473 756b 2f70 6778 2f61  m/sotetsuk/pgx/a
-000001f0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
-00000200: 2f63 692e 796d 6c2f 6261 6467 652e 7376  /ci.yml/badge.sv
-00000210: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
-00000220: 7562 2e63 6f6d 2f73 6f74 6574 7375 6b2f  ub.com/sotetsuk/
-00000230: 7067 782f 6163 7469 6f6e 732f 776f 726b  pgx/actions/work
-00000240: 666c 6f77 732f 6369 2e79 6d6c 290a 0a3c  flows/ci.yml)..<
-00000250: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-00000260: 7222 3e0a 3c69 6d67 2073 7263 3d22 6874  r">.<img src="ht
-00000270: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00000280: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000290: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
-000002a0: 6e2f 646f 6373 2f61 7373 6574 732f 6c6f  n/docs/assets/lo
-000002b0: 676f 2e73 7667 2220 7769 6474 683d 2234  go.svg" width="4
-000002c0: 3025 223e 0a3c 2f64 6976 3e0a 0a41 2063  0%">.</div>..A c
-000002d0: 6f6c 6c65 6374 696f 6e20 6f66 2047 5055  ollection of GPU
-000002e0: 2f54 5055 2d61 6363 656c 6572 6174 6564  /TPU-accelerated
-000002f0: 2070 6172 616c 6c65 6c20 6761 6d65 2073   parallel game s
-00000300: 696d 756c 6174 6f72 7320 666f 7220 7265  imulators for re
-00000310: 696e 666f 7263 656d 656e 7420 6c65 6172  inforcement lear
-00000320: 6e69 6e67 2028 524c 290a 0a3c 6469 7620  ning (RL)..<div 
-00000330: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-00000340: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000350: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00000360: 636f 6e74 656e 742e 636f 6d2f 736f 7465  content.com/sote
-00000370: 7473 756b 2f70 6778 2f6d 6169 6e2f 646f  tsuk/pgx/main/do
-00000380: 6373 2f61 7373 6574 732f 676f 5f64 6172  cs/assets/go_dar
-00000390: 6b2e 6769 6623 6768 2d64 6172 6b2d 6d6f  k.gif#gh-dark-mo
-000003a0: 6465 2d6f 6e6c 7922 2077 6964 7468 3d22  de-only" width="
-000003b0: 3330 2522 3e3c 696d 6720 7372 633d 2268  30%"><img src="h
-000003c0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-000003d0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-000003e0: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-000003f0: 696e 2f64 6f63 732f 6173 7365 7473 2f67  in/docs/assets/g
-00000400: 6f5f 6461 726b 2e67 6966 2367 682d 6461  o_dark.gif#gh-da
-00000410: 726b 2d6d 6f64 652d 6f6e 6c79 2220 7769  rk-mode-only" wi
-00000420: 6474 683d 2233 3025 2220 7374 796c 653d  dth="30%" style=
-00000430: 2274 7261 6e73 666f 726d 3a72 6f74 6174  "transform:rotat
-00000440: 6528 3237 3064 6567 293b 223e 3c69 6d67  e(270deg);"><img
-00000450: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00000460: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000470: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
-00000480: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
-00000490: 7373 6574 732f 676f 5f64 6172 6b2e 6769  ssets/go_dark.gi
-000004a0: 6623 6768 2d64 6172 6b2d 6d6f 6465 2d6f  f#gh-dark-mode-o
-000004b0: 6e6c 7922 2077 6964 7468 3d22 3330 2522  nly" width="30%"
-000004c0: 2073 7479 6c65 3d22 7472 616e 7366 6f72   style="transfor
-000004d0: 6d3a 726f 7461 7465 2839 3064 6567 293b  m:rotate(90deg);
-000004e0: 223e 0a3c 696d 6720 7372 633d 2268 7474  ">.<img src="htt
-000004f0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00000500: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
-00000510: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
-00000520: 2f64 6f63 732f 6173 7365 7473 2f67 6f5f  /docs/assets/go_
-00000530: 6c69 6768 742e 6769 6623 6768 2d6c 6967  light.gif#gh-lig
-00000540: 6874 2d6d 6f64 652d 6f6e 6c79 2220 7769  ht-mode-only" wi
-00000550: 6474 683d 2233 3025 223e 3c69 6d67 2073  dth="30%"><img s
-00000560: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-00000570: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00000580: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
-00000590: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
-000005a0: 6574 732f 676f 5f6c 6967 6874 2e67 6966  ets/go_light.gif
-000005b0: 2367 682d 6c69 6768 742d 6d6f 6465 2d6f  #gh-light-mode-o
-000005c0: 6e6c 7922 2077 6964 7468 3d22 3330 2522  nly" width="30%"
-000005d0: 2073 7479 6c65 3d22 7472 616e 7366 6f72   style="transfor
-000005e0: 6d3a 726f 7461 7465 2832 3730 6465 6729  m:rotate(270deg)
-000005f0: 3b22 3e3c 696d 6720 7372 633d 2268 7474  ;"><img src="htt
-00000600: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00000610: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
-00000620: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
-00000630: 2f64 6f63 732f 6173 7365 7473 2f67 6f5f  /docs/assets/go_
-00000640: 6c69 6768 742e 6769 6623 6768 2d6c 6967  light.gif#gh-lig
-00000650: 6874 2d6d 6f64 652d 6f6e 6c79 2220 7769  ht-mode-only" wi
-00000660: 6474 683d 2233 3025 2220 7374 796c 653d  dth="30%" style=
-00000670: 2274 7261 6e73 666f 726d 3a72 6f74 6174  "transform:rotat
-00000680: 6528 3930 6465 6729 3b22 3e0a 3c2f 6469  e(90deg);">.</di
-00000690: 763e 0a0a f09f 8e89 202a 2a60 7631 2e30  v>...... **`v1.0
-000006a0: 2e30 602a 2a20 6973 2072 656c 6561 7365  .0`** is release
-000006b0: 6421 2028 3230 3233 2e36 2e32 3029 0a0a  d! (2023.6.20)..
-000006c0: 2323 2057 6879 2050 6778 3f0a 0a3c 212d  ## Why Pgx?..<!-
-000006d0: 2d2d 200a 7468 726f 7567 6870 7574 3a20  -- .throughput: 
-000006e0: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-000006f0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00000700: 6d2f 6472 6976 652f 3167 4957 4859 4c4b  m/drive/1gIWHYLK
-00000710: 4278 4532 584b 4468 416c 4559 4b56 6563  BxE2XKDhAlEYKVec
-00000720: 7a33 5747 3463 7a64 7a23 7363 726f 6c6c  z3WG4czdz#scroll
-00000730: 546f 3d56 3151 5a68 5258 6f47 4c38 4b0a  To=V1QZhRXoGL8K.
-00000740: 2d2d 2d3e 0a0a 5b42 7261 785d 2868 7474  --->..[Brax](htt
-00000750: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000760: 676f 6f67 6c65 2f62 7261 7829 2c20 6120  google/brax), a 
-00000770: 5b4a 4158 5d28 6874 7470 733a 2f2f 6769  [JAX](https://gi
-00000780: 7468 7562 2e63 6f6d 2f67 6f6f 676c 652f  thub.com/google/
-00000790: 6a61 7829 2d6e 6174 6976 6520 7068 7973  jax)-native phys
-000007a0: 6963 7320 656e 6769 6e65 2c20 7072 6f76  ics engine, prov
-000007b0: 6964 6573 2065 7874 7265 6d65 6c79 2068  ides extremely h
-000007c0: 6967 682d 7370 6565 6420 7061 7261 6c6c  igh-speed parall
-000007d0: 656c 2073 696d 756c 6174 696f 6e20 666f  el simulation fo
-000007e0: 7220 524c 2069 6e20 2a63 6f6e 7469 6e75  r RL in *continu
-000007f0: 6f75 732a 2073 7461 7465 2073 7061 6365  ous* state space
-00000800: 2e0a 5468 656e 2c20 7768 6174 2061 626f  ..Then, what abo
-00000810: 7574 2052 4c20 696e 202a 6469 7363 7265  ut RL in *discre
-00000820: 7465 2a20 7374 6174 6520 7370 6163 6573  te* state spaces
-00000830: 206c 696b 6520 4368 6573 732c 2053 686f   like Chess, Sho
-00000840: 6769 2c20 616e 6420 476f 3f20 2a2a 5067  gi, and Go? **Pg
-00000850: 782a 2a20 7072 6f76 6964 6573 2061 2077  x** provides a w
-00000860: 6964 6520 7661 7269 6574 7920 6f66 204a  ide variety of J
-00000870: 4158 2d6e 6174 6976 6520 6761 6d65 2073  AX-native game s
-00000880: 696d 756c 6174 6f72 7321 2048 6967 686c  imulators! Highl
-00000890: 6967 6874 6564 2066 6561 7475 7265 7320  ighted features 
-000008a0: 696e 636c 7564 653a 0a0a 2d20 e29a a120  include:..- ... 
-000008b0: 2a2a 5375 7065 7220 6661 7374 2a2a 2069  **Super fast** i
-000008c0: 6e20 7061 7261 6c6c 656c 2065 7865 6375  n parallel execu
-000008d0: 7469 6f6e 206f 6e20 6163 6365 6c65 7261  tion on accelera
-000008e0: 746f 7273 0a2d 20f0 9f8e b220 2a2a 5661  tors.- .... **Va
-000008f0: 7269 6f75 7320 6761 6d65 2073 7570 706f  rious game suppo
-00000900: 7274 2a2a 2069 6e63 6c75 6469 6e67 202a  rt** including *
-00000910: 2a42 6163 6b67 616d 6d6f 6e2a 2a2c 202a  *Backgammon**, *
-00000920: 2a43 6865 7373 2a2a 2c20 2a2a 5368 6f67  *Chess**, **Shog
-00000930: 692a 2a2c 2061 6e64 202a 2a47 6f2a 2a0a  i**, and **Go**.
-00000940: 2d20 f09f 96bc efb8 8f20 2a2a 4265 6175  - ....... **Beau
-00000950: 7469 6675 6c20 7669 7375 616c 697a 6174  tiful visualizat
-00000960: 696f 6e2a 2a20 696e 2053 5647 2066 6f72  ion** in SVG for
-00000970: 6d61 740a 0a0a 2323 2043 6f6c 6162 0a0a  mat...## Colab..
-00000980: 2d20 5b47 6574 7469 6e67 2073 7461 7274  - [Getting start
-00000990: 6564 5d28 6874 7470 733a 2f2f 636f 6c61  ed](https://cola
-000009a0: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
-000009b0: 652e 636f 6d2f 6769 7468 7562 2f73 6f74  e.com/github/sot
-000009c0: 6574 7375 6b2f 7067 782f 626c 6f62 2f6d  etsuk/pgx/blob/m
-000009d0: 6169 6e2f 636f 6c61 622f 7067 785f 6865  ain/colab/pgx_he
-000009e0: 6c6c 6f5f 776f 726c 642e 6970 796e 6229  llo_world.ipynb)
-000009f0: 0a2d 205b 5067 7820 6261 7365 6c69 6e65  .- [Pgx baseline
-00000a00: 206d 6f64 656c 735d 2868 7474 7073 3a2f   models](https:/
-00000a10: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
-00000a20: 676f 6f67 6c65 2e63 6f6d 2f67 6974 6875  google.com/githu
-00000a30: 622f 736f 7465 7473 756b 2f70 6778 2f62  b/sotetsuk/pgx/b
-00000a40: 6c6f 622f 6d61 696e 2f63 6f6c 6162 2f62  lob/main/colab/b
-00000a50: 6173 656c 696e 6573 2e69 7079 6e62 290a  aselines.ipynb).
-00000a60: 2d20 5b50 504f 2065 7861 6d70 6c65 5d28  - [PPO example](
-00000a70: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-00000a80: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00000a90: 6d2f 6769 7468 7562 2f73 6f74 6574 7375  m/github/sotetsu
-00000aa0: 6b2f 7067 782f 626c 6f62 2f6d 6169 6e2f  k/pgx/blob/main/
-00000ab0: 636f 6c61 622f 7070 6f2e 6970 796e 6229  colab/ppo.ipynb)
-00000ac0: 0a2d 205b 4578 706f 7274 2074 6f20 5065  .- [Export to Pe
-00000ad0: 7474 696e 675a 6f6f 2041 5049 5d28 6874  ttingZoo API](ht
-00000ae0: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
-00000af0: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
-00000b00: 6769 7468 7562 2f73 6f74 6574 7375 6b2f  github/sotetsuk/
-00000b10: 7067 782f 626c 6f62 2f6d 6169 6e2f 636f  pgx/blob/main/co
-00000b20: 6c61 622f 7067 7832 7065 7474 696e 677a  lab/pgx2pettingz
-00000b30: 6f6f 2e69 7079 6e62 290a 0a23 2320 496e  oo.ipynb)..## In
-00000b40: 7374 616c 6c61 7469 6f6e 0a0a 6060 6073  stallation..```s
-00000b50: 680a 7069 7020 696e 7374 616c 6c20 7067  h.pip install pg
-00000b60: 780a 6060 600a 0a4e 6f74 6520 7468 6174  x.```..Note that
-00000b70: 2074 6865 205b 4d69 6e41 7461 725d 2868   the [MinAtar](h
-00000b80: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000b90: 6d2f 6b65 6e6a 796f 756e 672f 4d69 6e41  m/kenjyoung/MinA
-00000ba0: 7461 7229 2073 7569 7465 2069 7320 7072  tar) suite is pr
-00000bb0: 6f76 6964 6564 2061 7320 6120 7365 7061  ovided as a sepa
-00000bc0: 7261 7465 2065 7874 656e 7369 6f6e 2066  rate extension f
-00000bd0: 6f72 2050 6778 2028 5b60 7067 782d 6d69  or Pgx ([`pgx-mi
-00000be0: 6e61 7461 7260 5d28 6874 7470 733a 2f2f  natar`](https://
-00000bf0: 6769 7468 7562 2e63 6f6d 2f73 6f74 6574  github.com/sotet
-00000c00: 7375 6b2f 7067 782d 6d69 6e61 7461 7229  suk/pgx-minatar)
-00000c10: 292e 2054 6865 7265 666f 7265 2c20 706c  ). Therefore, pl
-00000c20: 6561 7365 2072 756e 2074 6865 2066 6f6c  ease run the fol
-00000c30: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2061  lowing command a
-00000c40: 6464 6974 696f 6e61 6c79 2074 6f20 7573  dditionaly to us
-00000c50: 6520 7468 6520 4d69 6e41 7461 7220 7375  e the MinAtar su
-00000c60: 6974 6520 696e 2050 6778 3a0a 0a60 6060  ite in Pgx:..```
-00000c70: 7368 0a70 6970 2069 6e73 7461 6c6c 2070  sh.pip install p
-00000c80: 6778 2d6d 696e 6174 6172 0a60 6060 0a0a  gx-minatar.```..
-00000c90: 5067 7820 6973 2070 726f 7669 6465 6420  Pgx is provided 
-00000ca0: 756e 6465 7220 7468 6520 4170 6163 6865  under the Apache
-00000cb0: 2032 2e30 204c 6963 656e 7365 2c20 6275   2.0 License, bu
-00000cc0: 7420 7468 6520 6f72 6967 696e 616c 204d  t the original M
-00000cd0: 696e 4174 6172 2073 7569 7465 2066 6f6c  inAtar suite fol
-00000ce0: 6c6f 7773 2074 6865 2047 504c 2033 2e30  lows the GPL 3.0
-00000cf0: 204c 6963 656e 7365 2e20 5468 6572 6566   License. Theref
-00000d00: 6f72 652c 2070 6c65 6173 6520 6e6f 7465  ore, please note
-00000d10: 2074 6861 7420 7468 6520 7365 7061 7261   that the separa
-00000d20: 7465 6420 4d69 6e41 7461 7220 6578 7465  ted MinAtar exte
-00000d30: 6e73 696f 6e20 666f 7220 5067 7820 616c  nsion for Pgx al
-00000d40: 736f 2061 6468 6572 6573 2074 6f20 7468  so adheres to th
-00000d50: 6520 4750 4c20 332e 3020 4c69 6365 6e73  e GPL 3.0 Licens
-00000d60: 652e 0a0a 2323 2055 7361 6765 0a0a 0a4e  e...## Usage...N
-00000d70: 6f74 6520 7468 6174 2061 6c6c 2060 7374  ote that all `st
-00000d80: 6570 6020 6675 6e63 7469 6f6e 7320 696e  ep` functions in
-00000d90: 2050 6778 2065 6e76 6972 6f6e 6d65 6e74   Pgx environment
-00000da0: 7320 6172 6520 2a2a 4a41 582d 6e61 7469  s are **JAX-nati
-00000db0: 7665 2e2a 2a2c 2069 2e65 2e2c 2074 6865  ve.**, i.e., the
-00000dc0: 7920 6172 6520 616c 6c20 2a4a 4954 2d61  y are all *JIT-a
-00000dd0: 626c 652a 2e0a 0a3c 6120 6872 6566 3d22  ble*...<a href="
-00000de0: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-00000df0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00000e00: 6d2f 6769 7468 7562 2f73 6f74 6574 7375  m/github/sotetsu
-00000e10: 6b2f 7067 782f 626c 6f62 2f6d 6169 6e2f  k/pgx/blob/main/
-00000e20: 636f 6c61 622f 7067 785f 6865 6c6c 6f5f  colab/pgx_hello_
-00000e30: 776f 726c 642e 6970 796e 6222 3e3c 696d  world.ipynb"><im
-00000e40: 6720 7372 633d 2268 7474 7073 3a2f 2f63  g src="https://c
-00000e50: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
-00000e60: 6f67 6c65 2e63 6f6d 2f61 7373 6574 732f  ogle.com/assets/
-00000e70: 636f 6c61 622d 6261 6467 652e 7376 6722  colab-badge.svg"
-00000e80: 2061 6c74 3d22 4f70 656e 2049 6e20 436f   alt="Open In Co
-00000e90: 6c61 6222 2f3e 3c2f 613e 0a0a 6060 6070  lab"/></a>..```p
-00000ea0: 790a 696d 706f 7274 206a 6178 0a69 6d70  y.import jax.imp
-00000eb0: 6f72 7420 7067 780a 0a65 6e76 203d 2070  ort pgx..env = p
-00000ec0: 6778 2e6d 616b 6528 2267 6f5f 3139 7831  gx.make("go_19x1
-00000ed0: 3922 290a 696e 6974 203d 206a 6178 2e6a  9").init = jax.j
-00000ee0: 6974 286a 6178 2e76 6d61 7028 656e 762e  it(jax.vmap(env.
-00000ef0: 696e 6974 2929 2020 2320 7665 6374 6f72  init))  # vector
-00000f00: 697a 6520 616e 6420 4a49 542d 636f 6d70  ize and JIT-comp
-00000f10: 696c 650a 7374 6570 203d 206a 6178 2e6a  ile.step = jax.j
-00000f20: 6974 286a 6178 2e76 6d61 7028 656e 762e  it(jax.vmap(env.
-00000f30: 7374 6570 2929 0a0a 6261 7463 685f 7369  step))..batch_si
-00000f40: 7a65 203d 2031 3032 340a 6b65 7973 203d  ze = 1024.keys =
-00000f50: 206a 6178 2e72 616e 646f 6d2e 7370 6c69   jax.random.spli
-00000f60: 7428 6a61 782e 7261 6e64 6f6d 2e50 524e  t(jax.random.PRN
-00000f70: 474b 6579 2834 3229 2c20 6261 7463 685f  GKey(42), batch_
-00000f80: 7369 7a65 290a 7374 6174 6520 3d20 696e  size).state = in
-00000f90: 6974 286b 6579 7329 2020 2320 7665 6374  it(keys)  # vect
-00000fa0: 6f72 697a 6564 2073 7461 7465 730a 7768  orized states.wh
-00000fb0: 696c 6520 6e6f 7420 2873 7461 7465 2e74  ile not (state.t
-00000fc0: 6572 6d69 6e61 7465 6420 7c20 7374 6174  erminated | stat
-00000fd0: 652e 7472 756e 6361 7465 6429 2e61 6c6c  e.truncated).all
-00000fe0: 2829 3a0a 2020 2020 6163 7469 6f6e 203d  ():.    action =
-00000ff0: 206d 6f64 656c 2873 7461 7465 2e63 7572   model(state.cur
-00001000: 7265 6e74 5f70 6c61 7965 722c 2073 7461  rent_player, sta
-00001010: 7465 2e6f 6273 6572 7661 7469 6f6e 2c20  te.observation, 
-00001020: 7374 6174 652e 6c65 6761 6c5f 6163 7469  state.legal_acti
-00001030: 6f6e 5f6d 6173 6b29 0a20 2020 2073 7461  on_mask).    sta
-00001040: 7465 203d 2073 7465 7028 7374 6174 652c  te = step(state,
-00001050: 2061 6374 696f 6e29 2020 2320 7374 6174   action)  # stat
-00001060: 652e 7265 7761 7264 2028 322c 290a 6060  e.reward (2,).``
-00001070: 600a 0a50 6778 2069 7320 6120 6c69 6272  `..Pgx is a libr
-00001080: 6172 7920 7468 6174 2066 6f63 7573 6573  ary that focuses
-00001090: 206f 6e20 6661 7374 6572 2069 6d70 6c65   on faster imple
-000010a0: 6d65 6e74 6174 696f 6e73 2072 6174 6865  mentations rathe
-000010b0: 7220 7468 616e 206a 7573 7420 7468 6520  r than just the 
-000010c0: 4150 4920 6974 7365 6c66 2e20 0a48 6f77  API itself. .How
-000010d0: 6576 6572 2c20 7468 6520 4150 4920 6974  ever, the API it
-000010e0: 7365 6c66 2069 7320 616c 736f 2073 7566  self is also suf
-000010f0: 6669 6369 656e 746c 7920 6765 6e65 7261  ficiently genera
-00001100: 6c2e 2046 6f72 2065 7861 6d70 6c65 2c20  l. For example, 
-00001110: 616c 6c20 656e 7669 726f 6e6d 656e 7473  all environments
-00001120: 2069 6e20 5067 7820 6361 6e20 6265 2063   in Pgx can be c
-00001130: 6f6e 7665 7274 6564 2074 6f20 7468 6520  onverted to the 
-00001140: 4145 4320 4150 4920 6f66 205b 5065 7474  AEC API of [Pett
-00001150: 696e 675a 6f6f 5d28 6874 7470 733a 2f2f  ingZoo](https://
-00001160: 6769 7468 7562 2e63 6f6d 2f46 6172 616d  github.com/Faram
-00001170: 612d 466f 756e 6461 7469 6f6e 2f50 6574  a-Foundation/Pet
-00001180: 7469 6e67 5a6f 6f29 2c20 616e 6420 796f  tingZoo), and yo
-00001190: 7520 6361 6e20 7275 6e20 5067 7820 656e  u can run Pgx en
-000011a0: 7669 726f 6e6d 656e 7473 2074 6872 6f75  vironments throu
-000011b0: 6768 2074 6865 2050 6574 7469 6e67 5a6f  gh the PettingZo
-000011c0: 6f20 4150 492e 0a59 6f75 2063 616e 2073  o API..You can s
-000011d0: 6565 2074 6865 2064 656d 6f6e 7374 7261  ee the demonstra
-000011e0: 7469 6f6e 2069 6e20 476f 6f67 6c65 2043  tion in Google C
-000011f0: 6f6c 6162 3a0a 0a3c 6120 6872 6566 3d22  olab:..<a href="
-00001200: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-00001210: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00001220: 6d2f 6769 7468 7562 2f73 6f74 6574 7375  m/github/sotetsu
-00001230: 6b2f 7067 782f 626c 6f62 2f6d 6169 6e2f  k/pgx/blob/main/
-00001240: 636f 6c61 622f 7067 7832 7065 7474 696e  colab/pgx2pettin
-00001250: 677a 6f6f 2e69 7079 6e62 223e 3c69 6d67  gzoo.ipynb"><img
-00001260: 2073 7263 3d22 6874 7470 733a 2f2f 636f   src="https://co
-00001270: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00001280: 676c 652e 636f 6d2f 6173 7365 7473 2f63  gle.com/assets/c
-00001290: 6f6c 6162 2d62 6164 6765 2e73 7667 2220  olab-badge.svg" 
-000012a0: 616c 743d 224f 7065 6e20 496e 2043 6f6c  alt="Open In Col
-000012b0: 6162 222f 3e3c 2f61 3e0a 0a3c 212d 2d2d  ab"/></a>..<!---
-000012c0: 0a23 2323 204c 696d 6974 6174 696f 6e73  .### Limitations
-000012d0: 2028 666f 7220 7468 6520 7369 6d70 6c69   (for the simpli
-000012e0: 6369 7479 290a 2a20 446f 6573 202a 2a4e  city).* Does **N
-000012f0: 4f54 2a2a 2073 7570 706f 7274 2061 6765  OT** support age
-00001300: 6e74 2064 6561 7468 2061 6e64 2063 7265  nt death and cre
-00001310: 6174 696f 6e2c 2077 6869 6368 2064 796e  ation, which dyn
-00001320: 6d69 6361 6c6c 7920 6368 616e 6765 7320  mically changes 
-00001330: 7468 6520 6172 7261 7920 7369 7a65 2e20  the array size. 
-00001340: 4974 2064 6f65 7320 6e6f 7420 7765 6c6c  It does not well
-00001350: 2073 7569 7420 746f 2047 5055 2d61 6363   suit to GPU-acc
-00001360: 656c 6572 6174 6564 2063 6f6d 7075 7461  elerated computa
-00001370: 7469 6f6e 2e0a 2a20 446f 6573 202a 2a4e  tion..* Does **N
-00001380: 4f54 2a2a 2073 7570 706f 7274 2043 6861  OT** support Cha
-00001390: 6e63 6520 706c 6179 6572 2028 4e61 7475  nce player (Natu
-000013a0: 7265 2070 6c61 7965 7229 2077 6974 6820  re player) with 
-000013b0: 6163 7469 6f6e 2073 656c 6563 7469 6f6e  action selection
-000013c0: 2e0a 2a20 446f 6573 202a 2a4e 4f54 2a2a  ..* Does **NOT**
-000013d0: 2073 7570 706f 7274 204f 7065 6e41 4920   support OpenAI 
-000013e0: 4779 6d20 4150 492e 0a20 2020 202a 204f  Gym API..    * O
-000013f0: 7065 6e41 4920 4779 6d20 6973 2066 6f72  penAI Gym is for
-00001400: 2073 696e 676c 652d 6167 656e 7420 656e   single-agent en
-00001410: 7669 726f 6e6d 656e 742e 204d 6f73 7420  vironment. Most 
-00001420: 6f66 2050 6778 2065 6e76 6972 6f6e 6d65  of Pgx environme
-00001430: 6e74 7320 6172 6520 6d75 6c74 692d 706c  nts are multi-pl
-00001440: 6179 6572 2067 616d 6573 2e20 4a75 7374  ayer games. Just
-00001450: 2064 6566 696e 696e 6720 6f70 706f 6e65   defining oppone
-00001460: 6e74 7320 6973 206e 6f74 2065 6e6f 7567  nts is not enoug
-00001470: 6820 666f 7220 636f 6e76 6572 7469 6e67  h for converting
-00001480: 206d 756c 7469 2d61 6765 6e74 2065 6e76   multi-agent env
-00001490: 6972 6f6e 656d 6e74 7320 746f 204f 7065  ironemnts to Ope
-000014a0: 6e41 4920 4779 6d20 656e 7669 726f 6e6d  nAI Gym environm
-000014b0: 656e 742e 2045 2e67 2e2c 2069 6e20 7468  ent. E.g., in th
-000014c0: 6520 6761 6d65 206f 6620 676f 2c20 7468  e game of go, th
-000014d0: 6520 6e65 7874 2073 7461 7465 2073 2720  e next state s' 
-000014e0: 6973 2064 6566 696e 6564 2061 7320 7468  is defined as th
-000014f0: 6520 7374 6174 6520 6a75 7374 2061 6674  e state just aft
-00001500: 6572 2070 6c61 6369 6e67 2061 2073 746f  er placing a sto
-00001510: 6e65 2069 6e20 416c 6861 476f 2070 6170  ne in AlhaGo pap
-00001520: 6572 2e20 486f 7765 7665 722c 2073 2720  er. However, s' 
-00001530: 6265 636f 6d65 7320 7468 6520 7374 6174  becomes the stat
-00001540: 6520 6166 7465 7220 7468 6520 6f70 706f  e after the oppo
-00001550: 6e65 6e74 7327 2070 6c61 792e 2054 6869  nents' play. Thi
-00001560: 7320 6368 616e 6765 7320 7468 6520 6465  s changes the de
-00001570: 6669 6e69 7469 6f6e 206f 6620 5628 7327  finition of V(s'
-00001580: 292e 0a2a 2044 6f65 7320 2a2a 4e4f 542a  )..* Does **NOT*
-00001590: 2a20 7375 7070 6f72 7420 5065 7474 696e  * support Pettin
-000015a0: 675a 6f6f 2041 5049 2e0a 2020 2020 2a20  gZoo API..    * 
-000015b0: 5065 7474 696e 675a 6f6f 2069 7320 2a47  PettingZoo is *G
-000015c0: 796d 2066 6f72 206d 756c 7469 2d61 6765  ym for multi-age
-000015d0: 6e74 2052 4c2a 2e20 4173 2066 6172 2061  nt RL*. As far a
-000015e0: 7320 7765 206b 6e6f 772c 2050 6574 7469  s we know, Petti
-000015f0: 6e67 5a6f 6f20 646f 6573 206e 6f74 2073  ngZoo does not s
-00001600: 7570 706f 7274 2076 6563 746f 7269 7a65  upport vectorize
-00001610: 6420 656e 7669 726f 6e6d 656e 7473 2028  d environments (
-00001620: 6c69 6b65 2056 6563 746f 7245 6e76 2069  like VectorEnv i
-00001630: 6e20 4f70 656e 4149 2047 796d 292e 2041  n OpenAI Gym). A
-00001640: 7320 5067 7827 7320 6d61 696e 2066 6561  s Pgx's main fea
-00001650: 7475 7265 2069 7320 6869 6768 6c79 2076  ture is highly v
-00001660: 6563 746f 7269 7a65 6420 656e 7669 726f  ectorized enviro
-00001670: 6e6d 656e 7420 7669 6120 4750 552f 5450  nment via GPU/TP
-00001680: 5520 7375 7070 6f72 742c 2057 6520 646f  U support, We do
-00001690: 206e 6f74 2063 7572 7265 6e74 6c79 2073   not currently s
-000016a0: 7570 706f 7274 2050 6574 7469 6e67 5a6f  upport PettingZo
-000016b0: 6f20 4150 492e 200a 0a23 2323 2060 736b  o API. ..### `sk
-000016c0: 6970 5f63 6861 6e63 6560 0a2a 2057 6520  ip_chance`.* We 
-000016d0: 7072 6570 6172 6520 736b 6970 5f63 6861  prepare skip_cha
-000016e0: 6e63 653d 5472 7565 206f 7074 696f 6e20  nce=True option 
-000016f0: 666f 7220 736f 6d65 2065 6e76 6972 6f6e  for some environ
-00001700: 6d65 6e74 732e 2054 6869 7320 6d61 6b65  ments. This make
-00001710: 7320 6974 2070 6f73 7369 626c 6520 746f  s it possible to
-00001720: 2063 6f6e 7369 6465 7220 7661 6c75 6520   consider value 
-00001730: 6675 6e63 7469 6f6e 2066 6f72 2022 706f  function for "po
-00001740: 7374 2d64 6563 6973 696f 6e20 7374 6174  st-decision stat
-00001750: 6573 2220 2853 6565 2041 6c67 6f52 4c20  es" (See AlgoRL 
-00001760: 626f 6f6b 292e 2048 6f77 6576 6572 2c20  book). However, 
-00001770: 7765 2064 6f20 6e6f 7420 616c 6c6f 7720  we do not allow 
-00001780: 6368 616e 6365 2061 6765 6e74 2074 6f20  chance agent to 
-00001790: 6368 6f6f 7365 2061 6374 696f 6e20 6c69  choose action li
-000017a0: 6b65 204f 7065 6e53 7069 656c 2e20 5468  ke OpenSpiel. Th
-000017b0: 6973 2069 7320 6265 6361 7573 6520 7468  is is because th
-000017c0: 6520 6163 7469 6f6e 2073 7061 6365 206f  e action space o
-000017d0: 6620 6368 616e 6365 2061 6765 6e74 2061  f chance agent a
-000017e0: 6e64 2075 7375 616c 2061 6765 6e74 2061  nd usual agent a
-000017f0: 7265 2064 6966 6665 7265 6e74 2e20 5468  re different. Th
-00001800: 7573 2c20 7768 656e 2074 6865 2063 6861  us, when the cha
-00001810: 6e63 6520 706c 6179 6572 2069 7320 6368  nce player is ch
-00001820: 6f73 656e 2028 6063 7572 7265 6e74 5f70  osen (`current_p
-00001830: 6c61 7965 723d 2d31 6029 2c20 6061 6374  layer=-1`), `act
-00001840: 696f 6e3d 2d31 6020 6d75 7374 2062 6520  ion=-1` must be 
-00001850: 7265 7475 726e 6564 2074 6f20 7374 6570  returned to step
-00001860: 2066 756e 6374 696f 6e2e 2055 7365 2060   function. Use `
-00001870: 7368 7566 666c 6560 2074 6f20 6d61 6b65  shuffle` to make
-00001880: 2060 7374 6570 6020 7374 6f63 6861 7374   `step` stochast
-00001890: 6963 2e0a 0a23 2323 2074 7275 6e63 6174  ic...### truncat
-000018a0: 6174 696f 6e20 616e 6420 6175 746f 5f72  ation and auto_r
-000018b0: 6573 6574 0a2a 2073 7570 706f 7274 6564  eset.* supported
-000018c0: 2062 7920 606d 616b 6528 656e 765f 6964   by `make(env_id
-000018d0: 3d22 2e2e 2e22 2c20 6175 746f 5f72 6573  ="...", auto_res
-000018e0: 6574 3d54 7275 652c 206d 6178 5f65 7069  et=True, max_epi
-000018f0: 736f 6465 5f6c 656e 6774 683d 3634 2960  sode_length=64)`
-00001900: 0a2a 2060 6175 746f 5f72 6573 6574 6020  .* `auto_reset` 
-00001910: 7769 6c6c 2072 6570 6c61 6365 2074 6865  will replace the
-00001920: 2074 6572 6d69 6e61 6c20 7374 6174 6520   terminal state 
-00001930: 6279 2069 6e69 7469 616c 2073 7461 7465  by initial state
-00001940: 2028 6275 7420 6069 735f 7465 726d 696e   (but `is_termin
-00001950: 616c 3d54 7275 6560 2069 7320 7365 7429  al=True` is set)
-00001960: 0a2a 2060 6973 5f74 7275 6e63 6174 6564  .* `is_truncated
-00001970: 3d54 7275 6560 2069 7320 616c 736f 2073  =True` is also s
-00001980: 6574 2074 6f20 7374 6174 650a 2d2d 2d3e  et to state.--->
-00001990: 0a0a 2323 2053 7570 706f 7274 6564 2067  ..## Supported g
-000019a0: 616d 6573 0a0a 7c20 4261 636b 6761 6d6d  ames..| Backgamm
-000019b0: 6f6e 207c 2043 6865 7373 207c 2053 686f  on | Chess | Sho
-000019c0: 6769 207c 2047 6f20 7c0a 7c3a 2d2d 2d3a  gi | Go |.|:---:
-000019d0: 7c3a 2d2d 2d3a 7c3a 2d2d 2d3a 7c3a 2d2d  |:---:|:---:|:--
-000019e0: 2d3a 7c0a 7c3c 696d 6720 7372 633d 2268  -:|.|<img src="h
-000019f0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00001a00: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00001a10: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-00001a20: 696e 2f64 6f63 732f 6173 7365 7473 2f62  in/docs/assets/b
-00001a30: 6163 6b67 616d 6d6f 6e5f 6461 726b 2e67  ackgammon_dark.g
-00001a40: 6966 2367 682d 6461 726b 2d6d 6f64 652d  if#gh-dark-mode-
-00001a50: 6f6e 6c79 2220 7769 6474 683d 2231 3730  only" width="170
-00001a60: 7078 223e 3c69 6d67 2073 7263 3d22 6874  px"><img src="ht
-00001a70: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00001a80: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00001a90: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
-00001aa0: 6e2f 646f 6373 2f61 7373 6574 732f 6261  n/docs/assets/ba
-00001ab0: 636b 6761 6d6d 6f6e 5f6c 6967 6874 2e67  ckgammon_light.g
-00001ac0: 6966 2367 682d 6c69 6768 742d 6d6f 6465  if#gh-light-mode
-00001ad0: 2d6f 6e6c 7922 2077 6964 7468 3d22 3137  -only" width="17
-00001ae0: 3070 7822 3e7c 3c69 6d67 2073 7263 3d22  0px">|<img src="
-00001af0: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00001b00: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00001b10: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
-00001b20: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
-00001b30: 6368 6573 735f 6461 726b 2e67 6966 2367  chess_dark.gif#g
-00001b40: 682d 6461 726b 2d6d 6f64 652d 6f6e 6c79  h-dark-mode-only
-00001b50: 2220 7769 6474 683d 2231 3538 7078 223e  " width="158px">
-00001b60: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001b70: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00001b80: 636f 6e74 656e 742e 636f 6d2f 736f 7465  content.com/sote
-00001b90: 7473 756b 2f70 6778 2f6d 6169 6e2f 646f  tsuk/pgx/main/do
-00001ba0: 6373 2f61 7373 6574 732f 6368 6573 735f  cs/assets/chess_
-00001bb0: 6c69 6768 742e 6769 6623 6768 2d6c 6967  light.gif#gh-lig
-00001bc0: 6874 2d6d 6f64 652d 6f6e 6c79 2220 7769  ht-mode-only" wi
-00001bd0: 6474 683d 2231 3538 7078 223e 7c3c 696d  dth="158px">|<im
-00001be0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00001bf0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00001c00: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00001c10: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-00001c20: 6173 7365 7473 2f73 686f 6769 5f64 6172  assets/shogi_dar
-00001c30: 6b2e 6769 6623 6768 2d64 6172 6b2d 6d6f  k.gif#gh-dark-mo
-00001c40: 6465 2d6f 6e6c 7922 2077 6964 7468 3d22  de-only" width="
-00001c50: 3137 3070 7822 3e3c 696d 6720 7372 633d  170px"><img src=
-00001c60: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00001c70: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00001c80: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
-00001c90: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
-00001ca0: 2f73 686f 6769 5f6c 6967 6874 2e67 6966  /shogi_light.gif
-00001cb0: 2367 682d 6c69 6768 742d 6d6f 6465 2d6f  #gh-light-mode-o
-00001cc0: 6e6c 7922 2077 6964 7468 3d22 3137 3070  nly" width="170p
-00001cd0: 7822 3e7c 3c69 6d67 2073 7263 3d22 6874  x">|<img src="ht
-00001ce0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00001cf0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00001d00: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
-00001d10: 6e2f 646f 6373 2f61 7373 6574 732f 676f  n/docs/assets/go
-00001d20: 2d31 3978 3139 5f64 6172 6b2e 6769 6623  -19x19_dark.gif#
-00001d30: 6768 2d64 6172 6b2d 6d6f 6465 2d6f 6e6c  gh-dark-mode-onl
-00001d40: 7922 2077 6964 7468 3d22 3136 3070 7822  y" width="160px"
-00001d50: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00000000: 5b21 5b63 695d 2868 7474 7073 3a2f 2f67  [![ci](https://g
+00000010: 6974 6875 622e 636f 6d2f 736f 7465 7473  ithub.com/sotets
+00000020: 756b 2f70 6778 2f61 6374 696f 6e73 2f77  uk/pgx/actions/w
+00000030: 6f72 6b66 6c6f 7773 2f63 692e 796d 6c2f  orkflows/ci.yml/
+00000040: 6261 6467 652e 7376 6729 5d28 6874 7470  badge.svg)](http
+00000050: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000060: 6f74 6574 7375 6b2f 7067 782f 6163 7469  otetsuk/pgx/acti
+00000070: 6f6e 732f 776f 726b 666c 6f77 732f 6369  ons/workflows/ci
+00000080: 2e79 6d6c 290a 0a0a 3c64 6976 2061 6c69  .yml)...<div ali
+00000090: 676e 3d22 6365 6e74 6572 223e 0a3c 696d  gn="center">.<im
+000000a0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+000000b0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+000000c0: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
+000000d0: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
+000000e0: 6173 7365 7473 2f6c 6f67 6f2e 7376 6722  assets/logo.svg"
+000000f0: 2077 6964 7468 3d22 3430 2522 3e0a 3c2f   width="40%">.</
+00000100: 6469 763e 0a0a 4120 636f 6c6c 6563 7469  div>..A collecti
+00000110: 6f6e 206f 6620 4750 552f 5450 552d 6163  on of GPU/TPU-ac
+00000120: 6365 6c65 7261 7465 6420 7061 7261 6c6c  celerated parall
+00000130: 656c 2067 616d 6520 7369 6d75 6c61 746f  el game simulato
+00000140: 7273 2066 6f72 2072 6569 6e66 6f72 6365  rs for reinforce
+00000150: 6d65 6e74 206c 6561 726e 696e 6720 2852  ment learning (R
+00000160: 4c29 0a0a 3c64 6976 2061 6c69 676e 3d22  L)..<div align="
+00000170: 6365 6e74 6572 223e 0a3c 696d 6720 7372  center">.<img sr
+00000180: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00000190: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+000001a0: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
+000001b0: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
+000001c0: 7473 2f67 6f5f 6461 726b 2e67 6966 2367  ts/go_dark.gif#g
+000001d0: 682d 6461 726b 2d6d 6f64 652d 6f6e 6c79  h-dark-mode-only
+000001e0: 2220 7769 6474 683d 2233 3025 223e 3c69  " width="30%"><i
+000001f0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000200: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00000210: 6e74 656e 742e 636f 6d2f 736f 7465 7473  ntent.com/sotets
+00000220: 756b 2f70 6778 2f6d 6169 6e2f 646f 6373  uk/pgx/main/docs
+00000230: 2f61 7373 6574 732f 676f 5f64 6172 6b2e  /assets/go_dark.
+00000240: 6769 6623 6768 2d64 6172 6b2d 6d6f 6465  gif#gh-dark-mode
+00000250: 2d6f 6e6c 7922 2077 6964 7468 3d22 3330  -only" width="30
+00000260: 2522 2073 7479 6c65 3d22 7472 616e 7366  %" style="transf
+00000270: 6f72 6d3a 726f 7461 7465 2832 3730 6465  orm:rotate(270de
+00000280: 6729 3b22 3e3c 696d 6720 7372 633d 2268  g);"><img src="h
+00000290: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+000002a0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+000002b0: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
+000002c0: 696e 2f64 6f63 732f 6173 7365 7473 2f67  in/docs/assets/g
+000002d0: 6f5f 6461 726b 2e67 6966 2367 682d 6461  o_dark.gif#gh-da
+000002e0: 726b 2d6d 6f64 652d 6f6e 6c79 2220 7769  rk-mode-only" wi
+000002f0: 6474 683d 2233 3025 2220 7374 796c 653d  dth="30%" style=
+00000300: 2274 7261 6e73 666f 726d 3a72 6f74 6174  "transform:rotat
+00000310: 6528 3930 6465 6729 3b22 3e0a 3c69 6d67  e(90deg);">.<img
+00000320: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00000330: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00000340: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
+00000350: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
+00000360: 7373 6574 732f 676f 5f6c 6967 6874 2e67  ssets/go_light.g
+00000370: 6966 2367 682d 6c69 6768 742d 6d6f 6465  if#gh-light-mode
+00000380: 2d6f 6e6c 7922 2077 6964 7468 3d22 3330  -only" width="30
+00000390: 2522 3e3c 696d 6720 7372 633d 2268 7474  %"><img src="htt
+000003a0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+000003b0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
+000003c0: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
+000003d0: 2f64 6f63 732f 6173 7365 7473 2f67 6f5f  /docs/assets/go_
+000003e0: 6c69 6768 742e 6769 6623 6768 2d6c 6967  light.gif#gh-lig
+000003f0: 6874 2d6d 6f64 652d 6f6e 6c79 2220 7769  ht-mode-only" wi
+00000400: 6474 683d 2233 3025 2220 7374 796c 653d  dth="30%" style=
+00000410: 2274 7261 6e73 666f 726d 3a72 6f74 6174  "transform:rotat
+00000420: 6528 3237 3064 6567 293b 223e 3c69 6d67  e(270deg);"><img
+00000430: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00000440: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00000450: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
+00000460: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
+00000470: 7373 6574 732f 676f 5f6c 6967 6874 2e67  ssets/go_light.g
+00000480: 6966 2367 682d 6c69 6768 742d 6d6f 6465  if#gh-light-mode
+00000490: 2d6f 6e6c 7922 2077 6964 7468 3d22 3330  -only" width="30
+000004a0: 2522 2073 7479 6c65 3d22 7472 616e 7366  %" style="transf
+000004b0: 6f72 6d3a 726f 7461 7465 2839 3064 6567  orm:rotate(90deg
+000004c0: 293b 223e 0a3c 2f64 6976 3e0a 0af0 9f8e  );">.</div>.....
+000004d0: 8920 2a2a 6076 312e 302e 3060 2a2a 2069  . **`v1.0.0`** i
+000004e0: 7320 7265 6c65 6173 6564 2120 2832 3032  s released! (202
+000004f0: 332e 362e 3230 290a 0a23 2320 5768 7920  3.6.20)..## Why 
+00000500: 5067 783f 0a0a 3c21 2d2d 2d20 0a74 6872  Pgx?..<!--- .thr
+00000510: 6f75 6768 7075 743a 2068 7474 7073 3a2f  oughput: https:/
+00000520: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
+00000530: 676f 6f67 6c65 2e63 6f6d 2f64 7269 7665  google.com/drive
+00000540: 2f31 6749 5748 594c 4b42 7845 3258 4b44  /1gIWHYLKBxE2XKD
+00000550: 6841 6c45 594b 5665 637a 3357 4734 637a  hAlEYKVecz3WG4cz
+00000560: 647a 2373 6372 6f6c 6c54 6f3d 5631 515a  dz#scrollTo=V1QZ
+00000570: 6852 586f 474c 384b 0a2d 2d2d 3e0a 0a5b  hRXoGL8K.--->..[
+00000580: 4272 6178 5d28 6874 7470 733a 2f2f 6769  Brax](https://gi
+00000590: 7468 7562 2e63 6f6d 2f67 6f6f 676c 652f  thub.com/google/
+000005a0: 6272 6178 292c 2061 205b 4a41 585d 2868  brax), a [JAX](h
+000005b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000005c0: 6d2f 676f 6f67 6c65 2f6a 6178 292d 6e61  m/google/jax)-na
+000005d0: 7469 7665 2070 6879 7369 6373 2065 6e67  tive physics eng
+000005e0: 696e 652c 2070 726f 7669 6465 7320 6578  ine, provides ex
+000005f0: 7472 656d 656c 7920 6869 6768 2d73 7065  tremely high-spe
+00000600: 6564 2070 6172 616c 6c65 6c20 7369 6d75  ed parallel simu
+00000610: 6c61 7469 6f6e 2066 6f72 2052 4c20 696e  lation for RL in
+00000620: 202a 636f 6e74 696e 756f 7573 2a20 7374   *continuous* st
+00000630: 6174 6520 7370 6163 652e 0a54 6865 6e2c  ate space..Then,
+00000640: 2077 6861 7420 6162 6f75 7420 524c 2069   what about RL i
+00000650: 6e20 2a64 6973 6372 6574 652a 2073 7461  n *discrete* sta
+00000660: 7465 2073 7061 6365 7320 6c69 6b65 2043  te spaces like C
+00000670: 6865 7373 2c20 5368 6f67 692c 2061 6e64  hess, Shogi, and
+00000680: 2047 6f3f 202a 2a50 6778 2a2a 2070 726f   Go? **Pgx** pro
+00000690: 7669 6465 7320 6120 7769 6465 2076 6172  vides a wide var
+000006a0: 6965 7479 206f 6620 4a41 582d 6e61 7469  iety of JAX-nati
+000006b0: 7665 2067 616d 6520 7369 6d75 6c61 746f  ve game simulato
+000006c0: 7273 2120 4869 6768 6c69 6768 7465 6420  rs! Highlighted 
+000006d0: 6665 6174 7572 6573 2069 6e63 6c75 6465  features include
+000006e0: 3a0a 0a2d 20e2 9aa1 202a 2a53 7570 6572  :..- ... **Super
+000006f0: 2066 6173 742a 2a20 696e 2070 6172 616c   fast** in paral
+00000700: 6c65 6c20 6578 6563 7574 696f 6e20 6f6e  lel execution on
+00000710: 2061 6363 656c 6572 6174 6f72 730a 2d20   accelerators.- 
+00000720: f09f 8eb2 202a 2a56 6172 696f 7573 2067  .... **Various g
+00000730: 616d 6520 7375 7070 6f72 742a 2a20 696e  ame support** in
+00000740: 636c 7564 696e 6720 2a2a 4261 636b 6761  cluding **Backga
+00000750: 6d6d 6f6e 2a2a 2c20 2a2a 4368 6573 732a  mmon**, **Chess*
+00000760: 2a2c 202a 2a53 686f 6769 2a2a 2c20 616e  *, **Shogi**, an
+00000770: 6420 2a2a 476f 2a2a 0a2d 20f0 9f96 bcef  d **Go**.- .....
+00000780: b88f 202a 2a42 6561 7574 6966 756c 2076  .. **Beautiful v
+00000790: 6973 7561 6c69 7a61 7469 6f6e 2a2a 2069  isualization** i
+000007a0: 6e20 5356 4720 666f 726d 6174 0a0a 0a23  n SVG format...#
+000007b0: 2320 5175 6963 6b20 7374 6172 740a 0a2d  # Quick start..-
+000007c0: 205b 4765 7474 696e 6720 7374 6172 7465   [Getting starte
+000007d0: 645d 2868 7474 7073 3a2f 2f63 6f6c 6162  d](https://colab
+000007e0: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
+000007f0: 2e63 6f6d 2f67 6974 6875 622f 736f 7465  .com/github/sote
+00000800: 7473 756b 2f70 6778 2f62 6c6f 622f 6d61  tsuk/pgx/blob/ma
+00000810: 696e 2f63 6f6c 6162 2f70 6778 5f68 656c  in/colab/pgx_hel
+00000820: 6c6f 5f77 6f72 6c64 2e69 7079 6e62 290a  lo_world.ipynb).
+00000830: 2d20 5b50 6778 2062 6173 656c 696e 6520  - [Pgx baseline 
+00000840: 6d6f 6465 6c73 5d28 6874 7470 733a 2f2f  models](https://
+00000850: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+00000860: 6f6f 676c 652e 636f 6d2f 6769 7468 7562  oogle.com/github
+00000870: 2f73 6f74 6574 7375 6b2f 7067 782f 626c  /sotetsuk/pgx/bl
+00000880: 6f62 2f6d 6169 6e2f 636f 6c61 622f 6261  ob/main/colab/ba
+00000890: 7365 6c69 6e65 732e 6970 796e 6229 0a2d  selines.ipynb).-
+000008a0: 205b 5050 4f20 6578 616d 706c 655d 2868   [PPO example](h
+000008b0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
+000008c0: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
+000008d0: 2f67 6974 6875 622f 736f 7465 7473 756b  /github/sotetsuk
+000008e0: 2f70 6778 2f62 6c6f 622f 6d61 696e 2f63  /pgx/blob/main/c
+000008f0: 6f6c 6162 2f70 706f 2e69 7079 6e62 290a  olab/ppo.ipynb).
+00000900: 2d20 5b45 7870 6f72 7420 746f 2050 6574  - [Export to Pet
+00000910: 7469 6e67 5a6f 6f20 4150 495d 2868 7474  tingZoo API](htt
+00000920: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+00000930: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f67  rch.google.com/g
+00000940: 6974 6875 622f 736f 7465 7473 756b 2f70  ithub/sotetsuk/p
+00000950: 6778 2f62 6c6f 622f 6d61 696e 2f63 6f6c  gx/blob/main/col
+00000960: 6162 2f70 6778 3270 6574 7469 6e67 7a6f  ab/pgx2pettingzo
+00000970: 6f2e 6970 796e 6229 0a0a 2323 2055 7361  o.ipynb)..## Usa
+00000980: 6765 0a0a 5468 6520 666f 6c6c 6f77 696e  ge..The followin
+00000990: 6720 636f 6465 2073 6e69 7070 6574 2073  g code snippet s
+000009a0: 686f 7773 2061 2073 696d 706c 6520 6578  hows a simple ex
+000009b0: 616d 706c 6520 6f66 2075 7369 6e67 2050  ample of using P
+000009c0: 6778 2e0a 596f 7520 6361 6e20 7472 7920  gx..You can try 
+000009d0: 6974 206f 7574 2069 6e20 5b74 6869 7320  it out in [this 
+000009e0: 436f 6c61 625d 2868 7474 7073 3a2f 2f63  Colab](https://c
+000009f0: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00000a00: 6f67 6c65 2e63 6f6d 2f67 6974 6875 622f  ogle.com/github/
+00000a10: 736f 7465 7473 756b 2f70 6778 2f62 6c6f  sotetsuk/pgx/blo
+00000a20: 622f 6d61 696e 2f63 6f6c 6162 2f70 6778  b/main/colab/pgx
+00000a30: 5f68 656c 6c6f 5f77 6f72 6c64 2e69 7079  _hello_world.ipy
+00000a40: 6e62 292e 0a4e 6f74 6520 7468 6174 2061  nb)..Note that a
+00000a50: 6c6c 2060 7374 6570 6020 6675 6e63 7469  ll `step` functi
+00000a60: 6f6e 7320 696e 2050 6778 2065 6e76 6972  ons in Pgx envir
+00000a70: 6f6e 6d65 6e74 7320 6172 6520 2a2a 4a41  onments are **JA
+00000a80: 582d 6e61 7469 7665 2e2a 2a2c 2069 2e65  X-native.**, i.e
+00000a90: 2e2c 2074 6865 7920 6172 6520 616c 6c20  ., they are all 
+00000aa0: 2a4a 4954 2d61 626c 652a 2e0a 506c 6561  *JIT-able*..Plea
+00000ab0: 7365 2072 6566 6572 2074 6f20 7468 6520  se refer to the 
+00000ac0: 5b64 6f63 756d 656e 7461 7469 6f6e 5d28  [documentation](
+00000ad0: 6874 7470 733a 2f2f 736f 7465 7473 756b  https://sotetsuk
+00000ae0: 2e67 6974 6875 622e 696f 2f70 6778 2920  .github.io/pgx) 
+00000af0: 666f 7220 6d6f 7265 2064 6574 6169 6c73  for more details
+00000b00: 2e0a 0a60 6060 7079 0a69 6d70 6f72 7420  ...```py.import 
+00000b10: 6a61 780a 696d 706f 7274 2070 6778 0a0a  jax.import pgx..
+00000b20: 656e 7620 3d20 7067 782e 6d61 6b65 2822  env = pgx.make("
+00000b30: 676f 5f31 3978 3139 2229 0a69 6e69 7420  go_19x19").init 
+00000b40: 3d20 6a61 782e 6a69 7428 6a61 782e 766d  = jax.jit(jax.vm
+00000b50: 6170 2865 6e76 2e69 6e69 7429 290a 7374  ap(env.init)).st
+00000b60: 6570 203d 206a 6178 2e6a 6974 286a 6178  ep = jax.jit(jax
+00000b70: 2e76 6d61 7028 656e 762e 7374 6570 2929  .vmap(env.step))
+00000b80: 0a0a 6261 7463 685f 7369 7a65 203d 2031  ..batch_size = 1
+00000b90: 3032 340a 6b65 7973 203d 206a 6178 2e72  024.keys = jax.r
+00000ba0: 616e 646f 6d2e 7370 6c69 7428 6a61 782e  andom.split(jax.
+00000bb0: 7261 6e64 6f6d 2e50 524e 474b 6579 2834  random.PRNGKey(4
+00000bc0: 3229 2c20 6261 7463 685f 7369 7a65 290a  2), batch_size).
+00000bd0: 7374 6174 6520 3d20 696e 6974 286b 6579  state = init(key
+00000be0: 7329 2020 2320 7665 6374 6f72 697a 6564  s)  # vectorized
+00000bf0: 2073 7461 7465 730a 7768 696c 6520 6e6f   states.while no
+00000c00: 7420 2873 7461 7465 2e74 6572 6d69 6e61  t (state.termina
+00000c10: 7465 6420 7c20 7374 6174 652e 7472 756e  ted | state.trun
+00000c20: 6361 7465 6429 2e61 6c6c 2829 3a0a 2020  cated).all():.  
+00000c30: 2020 6163 7469 6f6e 203d 206d 6f64 656c    action = model
+00000c40: 2873 7461 7465 2e63 7572 7265 6e74 5f70  (state.current_p
+00000c50: 6c61 7965 722c 2073 7461 7465 2e6f 6273  layer, state.obs
+00000c60: 6572 7661 7469 6f6e 2c20 7374 6174 652e  ervation, state.
+00000c70: 6c65 6761 6c5f 6163 7469 6f6e 5f6d 6173  legal_action_mas
+00000c80: 6b29 0a20 2020 2073 7461 7465 203d 2073  k).    state = s
+00000c90: 7465 7028 7374 6174 652c 2061 6374 696f  tep(state, actio
+00000ca0: 6e29 2020 2320 7374 6174 652e 7265 7761  n)  # state.rewa
+00000cb0: 7264 2028 322c 290a 6060 600a 0a50 6778  rd (2,).```..Pgx
+00000cc0: 2069 7320 6120 6c69 6272 6172 7920 7468   is a library th
+00000cd0: 6174 2066 6f63 7573 6573 206f 6e20 6661  at focuses on fa
+00000ce0: 7374 6572 2069 6d70 6c65 6d65 6e74 6174  ster implementat
+00000cf0: 696f 6e73 2072 6174 6865 7220 7468 616e  ions rather than
+00000d00: 206a 7573 7420 7468 6520 4150 4920 6974   just the API it
+00000d10: 7365 6c66 2e20 0a48 6f77 6576 6572 2c20  self. .However, 
+00000d20: 7468 6520 4150 4920 6974 7365 6c66 2069  the API itself i
+00000d30: 7320 616c 736f 2073 7566 6669 6369 656e  s also sufficien
+00000d40: 746c 7920 6765 6e65 7261 6c2e 2046 6f72  tly general. For
+00000d50: 2065 7861 6d70 6c65 2c20 616c 6c20 656e   example, all en
+00000d60: 7669 726f 6e6d 656e 7473 2069 6e20 5067  vironments in Pg
+00000d70: 7820 6361 6e20 6265 2063 6f6e 7665 7274  x can be convert
+00000d80: 6564 2074 6f20 7468 6520 4145 4320 4150  ed to the AEC AP
+00000d90: 4920 6f66 205b 5065 7474 696e 675a 6f6f  I of [PettingZoo
+00000da0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000db0: 2e63 6f6d 2f46 6172 616d 612d 466f 756e  .com/Farama-Foun
+00000dc0: 6461 7469 6f6e 2f50 6574 7469 6e67 5a6f  dation/PettingZo
+00000dd0: 6f29 2c20 616e 6420 796f 7520 6361 6e20  o), and you can 
+00000de0: 7275 6e20 5067 7820 656e 7669 726f 6e6d  run Pgx environm
+00000df0: 656e 7473 2074 6872 6f75 6768 2074 6865  ents through the
+00000e00: 2050 6574 7469 6e67 5a6f 6f20 4150 492e   PettingZoo API.
+00000e10: 0a59 6f75 2063 616e 2073 6565 2074 6865  .You can see the
+00000e20: 2064 656d 6f6e 7374 7261 7469 6f6e 2069   demonstration i
+00000e30: 6e20 5b74 6869 7320 436f 6c61 625d 2868  n [this Colab](h
+00000e40: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
+00000e50: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
+00000e60: 2f67 6974 6875 622f 736f 7465 7473 756b  /github/sotetsuk
+00000e70: 2f70 6778 2f62 6c6f 622f 6d61 696e 2f63  /pgx/blob/main/c
+00000e80: 6f6c 6162 2f70 6778 3270 6574 7469 6e67  olab/pgx2petting
+00000e90: 7a6f 6f2e 6970 796e 6229 2e0a 0a0a 2323  zoo.ipynb)....##
+00000ea0: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a60   Installation..`
+00000eb0: 6060 7368 0a70 6970 2069 6e73 7461 6c6c  ``sh.pip install
+00000ec0: 2070 6778 0a60 6060 0a0a 4e6f 7465 2074   pgx.```..Note t
+00000ed0: 6861 7420 7468 6520 5b4d 696e 4174 6172  hat the [MinAtar
+00000ee0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000ef0: 2e63 6f6d 2f6b 656e 6a79 6f75 6e67 2f4d  .com/kenjyoung/M
+00000f00: 696e 4174 6172 2920 7375 6974 6520 6973  inAtar) suite is
+00000f10: 2070 726f 7669 6465 6420 6173 2061 2073   provided as a s
+00000f20: 6570 6172 6174 6520 6578 7465 6e73 696f  eparate extensio
+00000f30: 6e20 666f 7220 5067 7820 285b 6070 6778  n for Pgx ([`pgx
+00000f40: 2d6d 696e 6174 6172 605d 2868 7474 7073  -minatar`](https
+00000f50: 3a2f 2f67 6974 6875 622e 636f 6d2f 736f  ://github.com/so
+00000f60: 7465 7473 756b 2f70 6778 2d6d 696e 6174  tetsuk/pgx-minat
+00000f70: 6172 2929 2e20 5468 6572 6566 6f72 652c  ar)). Therefore,
+00000f80: 2070 6c65 6173 6520 7275 6e20 7468 6520   please run the 
+00000f90: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+00000fa0: 6420 6164 6469 7469 6f6e 616c 7920 746f  d additionaly to
+00000fb0: 2075 7365 2074 6865 204d 696e 4174 6172   use the MinAtar
+00000fc0: 2073 7569 7465 2069 6e20 5067 783a 0a0a   suite in Pgx:..
+00000fd0: 6060 6073 680a 7069 7020 696e 7374 616c  ```sh.pip instal
+00000fe0: 6c20 7067 782d 6d69 6e61 7461 720a 6060  l pgx-minatar.``
+00000ff0: 600a 0a50 6778 2069 7320 7072 6f76 6964  `..Pgx is provid
+00001000: 6564 2075 6e64 6572 2074 6865 2041 7061  ed under the Apa
+00001010: 6368 6520 322e 3020 4c69 6365 6e73 652c  che 2.0 License,
+00001020: 2062 7574 2074 6865 206f 7269 6769 6e61   but the origina
+00001030: 6c20 4d69 6e41 7461 7220 7375 6974 6520  l MinAtar suite 
+00001040: 666f 6c6c 6f77 7320 7468 6520 4750 4c20  follows the GPL 
+00001050: 332e 3020 4c69 6365 6e73 652e 2054 6865  3.0 License. The
+00001060: 7265 666f 7265 2c20 706c 6561 7365 206e  refore, please n
+00001070: 6f74 6520 7468 6174 2074 6865 2073 6570  ote that the sep
+00001080: 6172 6174 6564 204d 696e 4174 6172 2065  arated MinAtar e
+00001090: 7874 656e 7369 6f6e 2066 6f72 2050 6778  xtension for Pgx
+000010a0: 2061 6c73 6f20 6164 6865 7265 7320 746f   also adheres to
+000010b0: 2074 6865 2047 504c 2033 2e30 204c 6963   the GPL 3.0 Lic
+000010c0: 656e 7365 2e0a 0a23 2320 5375 7070 6f72  ense...## Suppor
+000010d0: 7465 6420 6761 6d65 730a 0a7c 2042 6163  ted games..| Bac
+000010e0: 6b67 616d 6d6f 6e20 7c20 4368 6573 7320  kgammon | Chess 
+000010f0: 7c20 5368 6f67 6920 7c20 476f 207c 0a7c  | Shogi | Go |.|
+00001100: 3a2d 2d2d 3a7c 3a2d 2d2d 3a7c 3a2d 2d2d  :---:|:---:|:---
+00001110: 3a7c 3a2d 2d2d 3a7c 0a7c 3c69 6d67 2073  :|:---:|.|<img s
+00001120: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00001130: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00001140: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00001150: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+00001160: 6574 732f 6261 636b 6761 6d6d 6f6e 5f64  ets/backgammon_d
+00001170: 6172 6b2e 6769 6623 6768 2d64 6172 6b2d  ark.gif#gh-dark-
+00001180: 6d6f 6465 2d6f 6e6c 7922 2077 6964 7468  mode-only" width
+00001190: 3d22 3137 3070 7822 3e3c 696d 6720 7372  ="170px"><img sr
+000011a0: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+000011b0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+000011c0: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
+000011d0: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
+000011e0: 7473 2f62 6163 6b67 616d 6d6f 6e5f 6c69  ts/backgammon_li
+000011f0: 6768 742e 6769 6623 6768 2d6c 6967 6874  ght.gif#gh-light
+00001200: 2d6d 6f64 652d 6f6e 6c79 2220 7769 6474  -mode-only" widt
+00001210: 683d 2231 3730 7078 223e 7c3c 696d 6720  h="170px">|<img 
+00001220: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00001230: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00001240: 6e74 2e63 6f6d 2f73 6f74 6574 7375 6b2f  nt.com/sotetsuk/
+00001250: 7067 782f 6d61 696e 2f64 6f63 732f 6173  pgx/main/docs/as
+00001260: 7365 7473 2f63 6865 7373 5f64 6172 6b2e  sets/chess_dark.
+00001270: 6769 6623 6768 2d64 6172 6b2d 6d6f 6465  gif#gh-dark-mode
+00001280: 2d6f 6e6c 7922 2077 6964 7468 3d22 3135  -only" width="15
+00001290: 3870 7822 3e3c 696d 6720 7372 633d 2268  8px"><img src="h
+000012a0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+000012b0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+000012c0: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
+000012d0: 696e 2f64 6f63 732f 6173 7365 7473 2f63  in/docs/assets/c
+000012e0: 6865 7373 5f6c 6967 6874 2e67 6966 2367  hess_light.gif#g
+000012f0: 682d 6c69 6768 742d 6d6f 6465 2d6f 6e6c  h-light-mode-onl
+00001300: 7922 2077 6964 7468 3d22 3135 3870 7822  y" width="158px"
+00001310: 3e7c 3c69 6d67 2073 7263 3d22 6874 7470  >|<img src="http
+00001320: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00001330: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00001340: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00001350: 646f 6373 2f61 7373 6574 732f 7368 6f67  docs/assets/shog
+00001360: 695f 6461 726b 2e67 6966 2367 682d 6461  i_dark.gif#gh-da
+00001370: 726b 2d6d 6f64 652d 6f6e 6c79 2220 7769  rk-mode-only" wi
+00001380: 6474 683d 2231 3730 7078 223e 3c69 6d67  dth="170px"><img
+00001390: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+000013a0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+000013b0: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
+000013c0: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
+000013d0: 7373 6574 732f 7368 6f67 695f 6c69 6768  ssets/shogi_ligh
+000013e0: 742e 6769 6623 6768 2d6c 6967 6874 2d6d  t.gif#gh-light-m
+000013f0: 6f64 652d 6f6e 6c79 2220 7769 6474 683d  ode-only" width=
+00001400: 2231 3730 7078 223e 7c3c 696d 6720 7372  "170px">|<img sr
+00001410: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00001420: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00001430: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
+00001440: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
+00001450: 7473 2f67 6f2d 3139 7831 395f 6461 726b  ts/go-19x19_dark
+00001460: 2e67 6966 2367 682d 6461 726b 2d6d 6f64  .gif#gh-dark-mod
+00001470: 652d 6f6e 6c79 2220 7769 6474 683d 2231  e-only" width="1
+00001480: 3630 7078 223e 3c69 6d67 2073 7263 3d22  60px"><img src="
+00001490: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+000014a0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+000014b0: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
+000014c0: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
+000014d0: 676f 2d31 3978 3139 5f6c 6967 6874 2e67  go-19x19_light.g
+000014e0: 6966 2367 682d 6c69 6768 742d 6d6f 6465  if#gh-light-mode
+000014f0: 2d6f 6e6c 7922 2077 6964 7468 3d22 3136  -only" width="16
+00001500: 3070 7822 3e7c 0a0a 0a55 7365 2060 7067  0px">|...Use `pg
+00001510: 782e 6176 6169 6c61 626c 655f 656e 7673  x.available_envs
+00001520: 2829 202d 3e20 5475 706c 655b 456e 7649  () -> Tuple[EnvI
+00001530: 645d 6020 746f 2073 6565 2074 6865 206c  d]` to see the l
+00001540: 6973 7420 6f66 2063 7572 7265 6e74 6c79  ist of currently
+00001550: 2061 7661 696c 6162 6c65 2067 616d 6573   available games
+00001560: 2e20 4769 7665 6e20 616e 2060 3c45 6e76  . Given an `<Env
+00001570: 4964 3e60 2c20 796f 7520 6361 6e20 6372  Id>`, you can cr
+00001580: 6561 7465 2074 6865 2065 6e76 6972 6f6e  eate the environ
+00001590: 6d65 6e74 2076 6961 0a0a 6060 6070 790a  ment via..```py.
+000015a0: 3e3e 3e20 656e 7620 3d20 7067 782e 6d61  >>> env = pgx.ma
+000015b0: 6b65 283c 456e 7649 643e 290a 6060 600a  ke(<EnvId>).```.
+000015c0: 0a7c 2047 616d 652f 456e 7649 6420 7c20  .| Game/EnvId | 
+000015d0: 5669 7375 616c 697a 6174 696f 6e20 7c20  Visualization | 
+000015e0: 5665 7273 696f 6e20 7c20 4669 7665 2d77  Version | Five-w
+000015f0: 6f72 6420 6465 7363 7269 7074 696f 6e20  ord description 
+00001600: 7c0a 7c3a 2d2d 2d3a 7c3a 2d2d 2d3a 7c3a  |.|:---:|:---:|:
+00001610: 2d2d 2d3a 7c3a 2d2d 2d3a 7c0a 7c3c 6120  ---:|:---:|.|<a 
+00001620: 6872 6566 3d22 6874 7470 733a 2f2f 656e  href="https://en
+00001630: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+00001640: 696b 692f 3230 3438 5f28 7669 6465 6f5f  iki/2048_(video_
+00001650: 6761 6d65 2922 3e32 3034 383c 2f61 3e20  game)">2048</a> 
+00001660: 3c62 723e 2060 2232 3034 3822 6020 7c3c  <br> `"2048"` |<
+00001670: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001680: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00001690: 6f6e 7465 6e74 2e63 6f6d 2f73 6f74 6574  ontent.com/sotet
+000016a0: 7375 6b2f 7067 782f 6d61 696e 2f64 6f63  suk/pgx/main/doc
+000016b0: 732f 6173 7365 7473 2f32 3034 385f 6461  s/assets/2048_da
+000016c0: 726b 2e67 6966 2220 7769 6474 683d 2236  rk.gif" width="6
+000016d0: 3070 7822 3e3c 696d 6720 7372 633d 2268  0px"><img src="h
+000016e0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+000016f0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00001700: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
+00001710: 696e 2f64 6f63 732f 6173 7365 7473 2f32  in/docs/assets/2
+00001720: 3034 385f 6c69 6768 742e 6769 6622 2077  048_light.gif" w
+00001730: 6964 7468 3d22 3630 7078 223e 7c20 6076  idth="60px">| `v
+00001740: 3060 207c 202a 4d65 7267 6520 7469 6c65  0` | *Merge tile
+00001750: 7320 746f 2063 7265 6174 6520 3230 3438  s to create 2048
+00001760: 2e2a 207c 0a7c 3c61 2068 7265 663d 2268  .* |.|<a href="h
+00001770: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+00001780: 6469 612e 6f72 672f 7769 6b69 2f44 2543  dia.org/wiki/D%C
+00001790: 3525 3844 6275 7473 755f 7368 2543 3525  5%8Dbutsu_sh%C5%
+000017a0: 3844 6769 223e 416e 696d 616c 2053 686f  8Dgi">Animal Sho
+000017b0: 6769 3c2f 613e 3c62 723e 6022 616e 696d  gi</a><br>`"anim
+000017c0: 616c 5f73 686f 6769 2260 207c 3c69 6d67  al_shogi"` |<img
+000017d0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+000017e0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+000017f0: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
+00001800: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
+00001810: 7373 6574 732f 616e 696d 616c 5f73 686f  ssets/animal_sho
+00001820: 6769 5f64 6172 6b2e 6769 6622 2077 6964  gi_dark.gif" wid
+00001830: 7468 3d22 3630 7078 223e 3c69 6d67 2073  th="60px"><img s
+00001840: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00001850: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00001860: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00001870: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+00001880: 6574 732f 616e 696d 616c 5f73 686f 6769  ets/animal_shogi
+00001890: 5f6c 6967 6874 2e67 6966 2220 7769 6474  _light.gif" widt
+000018a0: 683d 2236 3070 7822 3e7c 2020 6076 3060  h="60px">|  `v0`
+000018b0: 207c 202a 416e 696d 616c 2d74 6865 6d65   | *Animal-theme
+000018c0: 6420 6368 696c 642d 6672 6965 6e64 6c79  d child-friendly
+000018d0: 2073 686f 6769 2e2a 207c 0a7c 3c61 2068   shogi.* |.|<a h
+000018e0: 7265 663d 2268 7474 7073 3a2f 2f65 6e2e  ref="https://en.
+000018f0: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
+00001900: 6b69 2f42 6163 6b67 616d 6d6f 6e22 3e42  ki/Backgammon">B
+00001910: 6163 6b67 616d 6d6f 6e3c 2f61 3e3c 6272  ackgammon</a><br
+00001920: 3e60 2262 6163 6b67 616d 6d6f 6e22 6020  >`"backgammon"` 
+00001930: 7c3c 696d 6720 7372 633d 2268 7474 7073  |<img src="https
+00001940: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00001950: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
+00001960: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
+00001970: 6f63 732f 6173 7365 7473 2f62 6163 6b67  ocs/assets/backg
+00001980: 616d 6d6f 6e5f 6461 726b 2e67 6966 2220  ammon_dark.gif" 
+00001990: 7769 6474 683d 2236 3070 7822 3e3c 696d  width="60px"><im
+000019a0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+000019b0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+000019c0: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
+000019d0: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
+000019e0: 6173 7365 7473 2f62 6163 6b67 616d 6d6f  assets/backgammo
+000019f0: 6e5f 6c69 6768 742e 6769 6622 2077 6964  n_light.gif" wid
+00001a00: 7468 3d22 3630 7078 223e 7c20 6076 3060  th="60px">| `v0`
+00001a10: 207c 202a 4c75 636b 2061 6964 7320 6265   | *Luck aids be
+00001a20: 6172 696e 6720 6f66 6620 6368 6563 6b65  aring off checke
+00001a30: 7273 2e2a 207c 0a7c 3c61 2068 7265 663d  rs.* |.|<a href=
+00001a40: 2268 7474 7073 3a2f 2f65 6e2e 7769 6b69  "https://en.wiki
+00001a50: 7065 6469 612e 6f72 672f 7769 6b69 2f43  pedia.org/wiki/C
+00001a60: 6f6e 7472 6163 745f 6272 6964 6765 223e  ontract_bridge">
+00001a70: 4272 6964 6765 2062 6964 6469 6e67 3c2f  Bridge bidding</
+00001a80: 613e 3c62 723e 6022 6272 6964 6765 5f62  a><br>`"bridge_b
+00001a90: 6964 6469 6e67 2260 207c 3c69 6d67 2073  idding"` |<img s
+00001aa0: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00001ab0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00001ac0: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00001ad0: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+00001ae0: 6574 732f 6272 6964 6765 5f62 6964 6469  ets/bridge_biddi
+00001af0: 6e67 5f64 6172 6b2e 6769 6622 2077 6964  ng_dark.gif" wid
+00001b00: 7468 3d22 3630 7078 223e 3c69 6d67 2073  th="60px"><img s
+00001b10: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00001b20: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00001b30: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00001b40: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+00001b50: 6574 732f 6272 6964 6765 5f62 6964 6469  ets/bridge_biddi
+00001b60: 6e67 5f6c 6967 6874 2e67 6966 2220 7769  ng_light.gif" wi
+00001b70: 6474 683d 2236 3070 7822 3e7c 2060 7630  dth="60px">| `v0
+00001b80: 6020 7c20 2a50 6172 746e 6572 7320 6578  ` | *Partners ex
+00001b90: 6368 616e 6765 2069 6e66 6f72 6d61 7469  change informati
+00001ba0: 6f6e 2076 6961 2062 6964 732e 2a20 7c0a  on via bids.* |.
+00001bb0: 7c3c 6120 6872 6566 3d22 6874 7470 733a  |<a href="https:
+00001bc0: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+00001bd0: 7267 2f77 696b 692f 4368 6573 7322 3e43  rg/wiki/Chess">C
+00001be0: 6865 7373 3c2f 613e 3c62 723e 6022 6368  hess</a><br>`"ch
+00001bf0: 6573 7322 6020 7c3c 696d 6720 7372 633d  ess"` |<img src=
+00001c00: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00001c10: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00001c20: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
+00001c30: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
+00001c40: 2f63 6865 7373 5f64 6172 6b2e 6769 6622  /chess_dark.gif"
+00001c50: 2077 6964 7468 3d22 3630 7078 223e 3c69   width="60px"><i
+00001c60: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00001c70: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00001c80: 6e74 656e 742e 636f 6d2f 736f 7465 7473  ntent.com/sotets
+00001c90: 756b 2f70 6778 2f6d 6169 6e2f 646f 6373  uk/pgx/main/docs
+00001ca0: 2f61 7373 6574 732f 6368 6573 735f 6c69  /assets/chess_li
+00001cb0: 6768 742e 6769 6622 2077 6964 7468 3d22  ght.gif" width="
+00001cc0: 3630 7078 223e 7c20 6076 3160 207c 202a  60px">| `v1` | *
+00001cd0: 4368 6563 6b6d 6174 6520 6f70 706f 6e65  Checkmate oppone
+00001ce0: 6e74 2773 206b 696e 6720 746f 2077 696e  nt's king to win
+00001cf0: 2e2a 207c 0a7c 3c61 2068 7265 663d 2268  .* |.|<a href="h
+00001d00: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+00001d10: 6469 612e 6f72 672f 7769 6b69 2f43 6f6e  dia.org/wiki/Con
+00001d20: 6e65 6374 5f46 6f75 7222 3e43 6f6e 6e65  nect_Four">Conne
+00001d30: 6374 2046 6f75 723c 2f61 3e3c 6272 3e60  ct Four</a><br>`
+00001d40: 2263 6f6e 6e65 6374 5f66 6f75 7222 6020  "connect_four"` 
+00001d50: 7c3c 696d 6720 7372 633d 2268 7474 7073  |<img src="https
 00001d60: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
 00001d70: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
 00001d80: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
-00001d90: 6f63 732f 6173 7365 7473 2f67 6f2d 3139  ocs/assets/go-19
-00001da0: 7831 395f 6c69 6768 742e 6769 6623 6768  x19_light.gif#gh
-00001db0: 2d6c 6967 6874 2d6d 6f64 652d 6f6e 6c79  -light-mode-only
-00001dc0: 2220 7769 6474 683d 2231 3630 7078 223e  " width="160px">
-00001dd0: 7c0a 0a0a 5573 6520 6070 6778 2e61 7661  |...Use `pgx.ava
-00001de0: 696c 6162 6c65 5f65 6e76 7328 2920 2d3e  ilable_envs() ->
-00001df0: 2054 7570 6c65 5b45 6e76 4964 5d60 2074   Tuple[EnvId]` t
-00001e00: 6f20 7365 6520 7468 6520 6c69 7374 206f  o see the list o
-00001e10: 6620 6375 7272 656e 746c 7920 6176 6169  f currently avai
-00001e20: 6c61 626c 6520 6761 6d65 732e 2047 6976  lable games. Giv
-00001e30: 656e 2061 6e20 603c 456e 7649 643e 602c  en an `<EnvId>`,
-00001e40: 2079 6f75 2063 616e 2063 7265 6174 6520   you can create 
-00001e50: 7468 6520 656e 7669 726f 6e6d 656e 7420  the environment 
-00001e60: 7669 610a 0a60 6060 7079 0a3e 3e3e 2065  via..```py.>>> e
-00001e70: 6e76 203d 2070 6778 2e6d 616b 6528 3c45  nv = pgx.make(<E
-00001e80: 6e76 4964 3e29 0a60 6060 0a0a 7c20 4761  nvId>).```..| Ga
-00001e90: 6d65 2f45 6e76 4964 207c 2056 6973 7561  me/EnvId | Visua
-00001ea0: 6c69 7a61 7469 6f6e 207c 2056 6572 7369  lization | Versi
-00001eb0: 6f6e 207c 2046 6976 652d 776f 7264 2064  on | Five-word d
-00001ec0: 6573 6372 6970 7469 6f6e 207c 0a7c 3a2d  escription |.|:-
-00001ed0: 2d2d 3a7c 3a2d 2d2d 3a7c 3a2d 2d2d 3a7c  --:|:---:|:---:|
-00001ee0: 3a2d 2d2d 3a7c 0a7c 3c61 2068 7265 663d  :---:|.|<a href=
-00001ef0: 2268 7474 7073 3a2f 2f65 6e2e 7769 6b69  "https://en.wiki
-00001f00: 7065 6469 612e 6f72 672f 7769 6b69 2f32  pedia.org/wiki/2
-00001f10: 3034 385f 2876 6964 656f 5f67 616d 6529  048_(video_game)
-00001f20: 223e 3230 3438 3c2f 613e 203c 6272 3e20  ">2048</a> <br> 
-00001f30: 6022 3230 3438 2260 207c 3c69 6d67 2073  `"2048"` |<img s
-00001f40: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-00001f50: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00001f60: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
-00001f70: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
-00001f80: 6574 732f 3230 3438 5f64 6172 6b2e 6769  ets/2048_dark.gi
-00001f90: 6622 2077 6964 7468 3d22 3630 7078 223e  f" width="60px">
-00001fa0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001fb0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00001fc0: 636f 6e74 656e 742e 636f 6d2f 736f 7465  content.com/sote
-00001fd0: 7473 756b 2f70 6778 2f6d 6169 6e2f 646f  tsuk/pgx/main/do
-00001fe0: 6373 2f61 7373 6574 732f 3230 3438 5f6c  cs/assets/2048_l
-00001ff0: 6967 6874 2e67 6966 2220 7769 6474 683d  ight.gif" width=
-00002000: 2236 3070 7822 3e7c 2060 7630 6020 7c20  "60px">| `v0` | 
-00002010: 2a4d 6572 6765 2074 696c 6573 2074 6f20  *Merge tiles to 
-00002020: 6372 6561 7465 2032 3034 382e 2a20 7c0a  create 2048.* |.
-00002030: 7c3c 6120 6872 6566 3d22 6874 7470 733a  |<a href="https:
-00002040: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00002050: 7267 2f77 696b 692f 4425 4335 2538 4462  rg/wiki/D%C5%8Db
-00002060: 7574 7375 5f73 6825 4335 2538 4467 6922  utsu_sh%C5%8Dgi"
-00002070: 3e41 6e69 6d61 6c20 5368 6f67 693c 2f61  >Animal Shogi</a
-00002080: 3e3c 6272 3e60 2261 6e69 6d61 6c5f 7368  ><br>`"animal_sh
-00002090: 6f67 6922 6020 7c3c 696d 6720 7372 633d  ogi"` |<img src=
-000020a0: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-000020b0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-000020c0: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
-000020d0: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
-000020e0: 2f61 6e69 6d61 6c5f 7368 6f67 695f 6461  /animal_shogi_da
-000020f0: 726b 2e67 6966 2220 7769 6474 683d 2236  rk.gif" width="6
-00002100: 3070 7822 3e3c 696d 6720 7372 633d 2268  0px"><img src="h
-00002110: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00002120: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00002130: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-00002140: 696e 2f64 6f63 732f 6173 7365 7473 2f61  in/docs/assets/a
-00002150: 6e69 6d61 6c5f 7368 6f67 695f 6c69 6768  nimal_shogi_ligh
-00002160: 742e 6769 6622 2077 6964 7468 3d22 3630  t.gif" width="60
-00002170: 7078 223e 7c20 2060 7630 6020 7c20 2a41  px">|  `v0` | *A
-00002180: 6e69 6d61 6c2d 7468 656d 6564 2063 6869  nimal-themed chi
-00002190: 6c64 2d66 7269 656e 646c 7920 7368 6f67  ld-friendly shog
-000021a0: 692e 2a20 7c0a 7c3c 6120 6872 6566 3d22  i.* |.|<a href="
-000021b0: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-000021c0: 6564 6961 2e6f 7267 2f77 696b 692f 4261  edia.org/wiki/Ba
-000021d0: 636b 6761 6d6d 6f6e 223e 4261 636b 6761  ckgammon">Backga
-000021e0: 6d6d 6f6e 3c2f 613e 3c62 723e 6022 6261  mmon</a><br>`"ba
-000021f0: 636b 6761 6d6d 6f6e 2260 207c 3c69 6d67  ckgammon"` |<img
-00002200: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00002210: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00002220: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
-00002230: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
-00002240: 7373 6574 732f 6261 636b 6761 6d6d 6f6e  ssets/backgammon
-00002250: 5f64 6172 6b2e 6769 6622 2077 6964 7468  _dark.gif" width
-00002260: 3d22 3630 7078 223e 3c69 6d67 2073 7263  ="60px"><img src
-00002270: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00002280: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00002290: 636f 6d2f 736f 7465 7473 756b 2f70 6778  com/sotetsuk/pgx
-000022a0: 2f6d 6169 6e2f 646f 6373 2f61 7373 6574  /main/docs/asset
-000022b0: 732f 6261 636b 6761 6d6d 6f6e 5f6c 6967  s/backgammon_lig
-000022c0: 6874 2e67 6966 2220 7769 6474 683d 2236  ht.gif" width="6
-000022d0: 3070 7822 3e7c 2060 7630 6020 7c20 2a4c  0px">| `v0` | *L
-000022e0: 7563 6b20 6169 6473 2062 6561 7269 6e67  uck aids bearing
-000022f0: 206f 6666 2063 6865 636b 6572 732e 2a20   off checkers.* 
-00002300: 7c0a 7c3c 6120 6872 6566 3d22 6874 7470  |.|<a href="http
-00002310: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
-00002320: 2e6f 7267 2f77 696b 692f 436f 6e74 7261  .org/wiki/Contra
-00002330: 6374 5f62 7269 6467 6522 3e42 7269 6467  ct_bridge">Bridg
-00002340: 6520 6269 6464 696e 673c 2f61 3e3c 6272  e bidding</a><br
-00002350: 3e60 2262 7269 6467 655f 6269 6464 696e  >`"bridge_biddin
-00002360: 6722 6020 7c3c 696d 6720 7372 633d 2268  g"` |<img src="h
-00002370: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00002380: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00002390: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-000023a0: 696e 2f64 6f63 732f 6173 7365 7473 2f62  in/docs/assets/b
-000023b0: 7269 6467 655f 6269 6464 696e 675f 6461  ridge_bidding_da
-000023c0: 726b 2e67 6966 2220 7769 6474 683d 2236  rk.gif" width="6
-000023d0: 3070 7822 3e3c 696d 6720 7372 633d 2268  0px"><img src="h
-000023e0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-000023f0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00002400: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-00002410: 696e 2f64 6f63 732f 6173 7365 7473 2f62  in/docs/assets/b
-00002420: 7269 6467 655f 6269 6464 696e 675f 6c69  ridge_bidding_li
-00002430: 6768 742e 6769 6622 2077 6964 7468 3d22  ght.gif" width="
-00002440: 3630 7078 223e 7c20 6076 3060 207c 202a  60px">| `v0` | *
-00002450: 5061 7274 6e65 7273 2065 7863 6861 6e67  Partners exchang
-00002460: 6520 696e 666f 726d 6174 696f 6e20 7669  e information vi
-00002470: 6120 6269 6473 2e2a 207c 0a7c 3c61 2068  a bids.* |.|<a h
-00002480: 7265 663d 2268 7474 7073 3a2f 2f65 6e2e  ref="https://en.
-00002490: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
-000024a0: 6b69 2f43 6865 7373 223e 4368 6573 733c  ki/Chess">Chess<
-000024b0: 2f61 3e3c 6272 3e60 2263 6865 7373 2260  /a><br>`"chess"`
-000024c0: 207c 3c69 6d67 2073 7263 3d22 6874 7470   |<img src="http
-000024d0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-000024e0: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
-000024f0: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
-00002500: 646f 6373 2f61 7373 6574 732f 6368 6573  docs/assets/ches
-00002510: 735f 6461 726b 2e67 6966 2220 7769 6474  s_dark.gif" widt
-00002520: 683d 2236 3070 7822 3e3c 696d 6720 7372  h="60px"><img sr
-00002530: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
-00002540: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00002550: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
-00002560: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
-00002570: 7473 2f63 6865 7373 5f6c 6967 6874 2e67  ts/chess_light.g
-00002580: 6966 2220 7769 6474 683d 2236 3070 7822  if" width="60px"
-00002590: 3e7c 2060 7630 6020 7c20 2a43 6865 636b  >| `v0` | *Check
-000025a0: 6d61 7465 206f 7070 6f6e 656e 7427 7320  mate opponent's 
-000025b0: 6b69 6e67 2074 6f20 7769 6e2e 2a20 7c0a  king to win.* |.
-000025c0: 7c3c 6120 6872 6566 3d22 6874 7470 733a  |<a href="https:
-000025d0: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-000025e0: 7267 2f77 696b 692f 436f 6e6e 6563 745f  rg/wiki/Connect_
-000025f0: 466f 7572 223e 436f 6e6e 6563 7420 466f  Four">Connect Fo
-00002600: 7572 3c2f 613e 3c62 723e 6022 636f 6e6e  ur</a><br>`"conn
-00002610: 6563 745f 666f 7572 2260 207c 3c69 6d67  ect_four"` |<img
-00002620: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00002630: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00002640: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
-00002650: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
-00002660: 7373 6574 732f 636f 6e6e 6563 745f 666f  ssets/connect_fo
-00002670: 7572 5f64 6172 6b2e 6769 6622 2077 6964  ur_dark.gif" wid
-00002680: 7468 3d22 3630 7078 223e 3c69 6d67 2073  th="60px"><img s
-00002690: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-000026a0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-000026b0: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
-000026c0: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
-000026d0: 6574 732f 636f 6e6e 6563 745f 666f 7572  ets/connect_four
-000026e0: 5f6c 6967 6874 2e67 6966 2220 7769 6474  _light.gif" widt
-000026f0: 683d 2236 3070 7822 3e7c 2060 7630 6020  h="60px">| `v0` 
-00002700: 7c20 2a43 6f6e 6e65 6374 2064 6973 6373  | *Connect discs
-00002710: 2c20 7769 6e20 7769 7468 2066 6f75 722e  , win with four.
-00002720: 2a20 7c0a 7c3c 6120 6872 6566 3d22 6874  * |.|<a href="ht
-00002730: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
-00002740: 6961 2e6f 7267 2f77 696b 692f 4d69 6e69  ia.org/wiki/Mini
-00002750: 6368 6573 7322 3e47 6172 646e 6572 2043  chess">Gardner C
-00002760: 6865 7373 3c2f 613e 3c62 723e 6022 6761  hess</a><br>`"ga
-00002770: 7264 6e65 725f 6368 6573 7322 607c 3c69  rdner_chess"`|<i
-00002780: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00002790: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-000027a0: 6e74 656e 742e 636f 6d2f 736f 7465 7473  ntent.com/sotets
-000027b0: 756b 2f70 6778 2f6d 6169 6e2f 646f 6373  uk/pgx/main/docs
-000027c0: 2f61 7373 6574 732f 6761 7264 6e65 725f  /assets/gardner_
-000027d0: 6368 6573 735f 6461 726b 2e67 6966 2220  chess_dark.gif" 
-000027e0: 7769 6474 683d 2236 3070 7822 3e3c 696d  width="60px"><im
-000027f0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00002800: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00002810: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00002820: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-00002830: 6173 7365 7473 2f67 6172 646e 6572 5f63  assets/gardner_c
-00002840: 6865 7373 5f6c 6967 6874 2e67 6966 2220  hess_light.gif" 
-00002850: 7769 6474 683d 2236 3070 7822 3e7c 2060  width="60px">| `
-00002860: 7630 6020 7c20 2a35 7835 2063 6865 7373  v0` | *5x5 chess
-00002870: 2076 6172 6961 6e74 2c20 6578 636c 7564   variant, exclud
-00002880: 696e 6720 6361 7374 6c69 6e67 2e2a 207c  ing castling.* |
-00002890: 0a7c 3c61 2068 7265 663d 2268 7474 7073  .|<a href="https
-000028a0: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-000028b0: 6f72 672f 7769 6b69 2f47 6f5f 2867 616d  org/wiki/Go_(gam
-000028c0: 6529 223e 476f 3c2f 613e 3c62 723e 6022  e)">Go</a><br>`"
-000028d0: 676f 5f39 7839 2260 2060 2267 6f5f 3139  go_9x9"` `"go_19
-000028e0: 7831 3922 6020 7c3c 696d 6720 7372 633d  x19"` |<img src=
-000028f0: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00002900: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00002910: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
-00002920: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
-00002930: 2f67 6f2d 3139 7831 395f 6461 726b 2e67  /go-19x19_dark.g
-00002940: 6966 2220 7769 6474 683d 2236 3070 7822  if" width="60px"
-00002950: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00002960: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00002970: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
-00002980: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
-00002990: 6f63 732f 6173 7365 7473 2f67 6f2d 3139  ocs/assets/go-19
-000029a0: 7831 395f 6c69 6768 742e 6769 6622 2077  x19_light.gif" w
-000029b0: 6964 7468 3d22 3630 7078 223e 7c20 6076  idth="60px">| `v
-000029c0: 3060 207c 202a 5374 7261 7465 6769 6361  0` | *Strategica
-000029d0: 6c6c 7920 706c 6163 6520 7374 6f6e 6573  lly place stones
-000029e0: 2c20 636c 6169 6d20 7465 7272 6974 6f72  , claim territor
-000029f0: 792e 2a20 7c0a 7c3c 6120 6872 6566 3d22  y.* |.|<a href="
-00002a00: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00002a10: 6564 6961 2e6f 7267 2f77 696b 692f 4865  edia.org/wiki/He
-00002a20: 785f 2862 6f61 7264 5f67 616d 6529 223e  x_(board_game)">
-00002a30: 4865 783c 2f61 3e3c 6272 3e60 2268 6578  Hex</a><br>`"hex
-00002a40: 2260 207c 3c69 6d67 2073 7263 3d22 6874  "` |<img src="ht
-00002a50: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00002a60: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00002a70: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
-00002a80: 6e2f 646f 6373 2f61 7373 6574 732f 6865  n/docs/assets/he
-00002a90: 785f 6461 726b 2e67 6966 2220 7769 6474  x_dark.gif" widt
-00002aa0: 683d 2236 3070 7822 3e3c 696d 6720 7372  h="60px"><img sr
-00002ab0: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
-00002ac0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00002ad0: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
-00002ae0: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
-00002af0: 7473 2f68 6578 5f6c 6967 6874 2e67 6966  ts/hex_light.gif
-00002b00: 2220 7769 6474 683d 2236 3070 7822 3e7c  " width="60px">|
-00002b10: 2060 7630 6020 7c20 2a43 6f6e 6e65 6374   `v0` | *Connect
-00002b20: 206f 7070 6f73 6974 6520 7369 6465 732c   opposite sides,
-00002b30: 2062 6c6f 636b 206f 7070 6f6e 656e 742e   block opponent.
-00002b40: 2a20 7c0a 7c3c 6120 6872 6566 3d22 6874  * |.|<a href="ht
-00002b50: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
-00002b60: 6961 2e6f 7267 2f77 696b 692f 4b75 686e  ia.org/wiki/Kuhn
-00002b70: 5f70 6f6b 6572 223e 4b75 686e 2050 6f6b  _poker">Kuhn Pok
-00002b80: 6572 3c2f 613e 3c62 723e 6022 6b75 686e  er</a><br>`"kuhn
-00002b90: 5f70 6f6b 6572 2260 207c 3c69 6d67 2073  _poker"` |<img s
-00002ba0: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-00002bb0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00002bc0: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
-00002bd0: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
-00002be0: 6574 732f 6b75 686e 5f70 6f6b 6572 5f64  ets/kuhn_poker_d
-00002bf0: 6172 6b2e 6769 6622 2077 6964 7468 3d22  ark.gif" width="
-00002c00: 3630 7078 223e 3c69 6d67 2073 7263 3d22  60px"><img src="
-00002c10: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00002c20: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00002c30: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
-00002c40: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
-00002c50: 6b75 686e 5f70 6f6b 6572 5f6c 6967 6874  kuhn_poker_light
-00002c60: 2e67 6966 2220 7769 6474 683d 2236 3070  .gif" width="60p
-00002c70: 7822 3e7c 2060 7630 6020 7c20 2a54 6872  x">| `v0` | *Thr
-00002c80: 6565 2d63 6172 6420 6265 7474 696e 6720  ee-card betting 
-00002c90: 616e 6420 626c 7566 6669 6e67 2067 616d  and bluffing gam
-00002ca0: 652e 2a20 7c0a 7c3c 6120 6872 6566 3d22  e.* |.|<a href="
-00002cb0: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00002cc0: 672f 6162 732f 3132 3037 2e31 3431 3122  g/abs/1207.1411"
-00002cd0: 3e4c 6564 7563 2068 6f6c 6427 656d 3c2f  >Leduc hold'em</
-00002ce0: 613e 3c62 723e 6022 6c65 6475 635f 686f  a><br>`"leduc_ho
-00002cf0: 6c64 656d 2260 207c 3c69 6d67 2073 7263  ldem"` |<img src
-00002d00: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00002d10: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00002d20: 636f 6d2f 736f 7465 7473 756b 2f70 6778  com/sotetsuk/pgx
-00002d30: 2f6d 6169 6e2f 646f 6373 2f61 7373 6574  /main/docs/asset
-00002d40: 732f 6c65 6475 635f 686f 6c64 656d 5f64  s/leduc_holdem_d
-00002d50: 6172 6b2e 6769 6622 2077 6964 7468 3d22  ark.gif" width="
-00002d60: 3630 7078 223e 3c69 6d67 2073 7263 3d22  60px"><img src="
-00002d70: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00002d80: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00002d90: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
-00002da0: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
-00002db0: 6c65 6475 635f 686f 6c64 656d 5f6c 6967  leduc_holdem_lig
-00002dc0: 6874 2e67 6966 2220 7769 6474 683d 2236  ht.gif" width="6
-00002dd0: 3070 7822 3e7c 2060 7630 6020 7c20 2a54  0px">| `v0` | *T
-00002de0: 776f 2d73 7569 742c 206c 696d 6974 6564  wo-suit, limited
-00002df0: 2064 6563 6b20 706f 6b65 722e 2a20 7c0a   deck poker.* |.
-00002e00: 7c3c 6120 6872 6566 3d22 6874 7470 733a  |<a href="https:
-00002e10: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 656e  //github.com/ken
-00002e20: 6a79 6f75 6e67 2f4d 696e 4174 6172 223e  jyoung/MinAtar">
-00002e30: 4d69 6e41 7461 722f 4173 7465 7269 783c  MinAtar/Asterix<
-00002e40: 2f61 3e3c 6272 3e60 226d 696e 6174 6172  /a><br>`"minatar
-00002e50: 2d61 7374 6572 6978 2260 207c 3c69 6d67  -asterix"` |<img
-00002e60: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00002e70: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00002e80: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
-00002e90: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
-00002ea0: 7373 6574 732f 6d69 6e61 7461 722d 6173  ssets/minatar-as
-00002eb0: 7465 7269 782e 6769 6622 2077 6964 7468  terix.gif" width
-00002ec0: 3d22 3530 7078 223e 7c20 6076 3060 207c  ="50px">| `v0` |
-00002ed0: 202a 4176 6f69 6420 656e 656d 6965 732c   *Avoid enemies,
-00002ee0: 2063 6f6c 6c65 6374 2074 7265 6173 7572   collect treasur
-00002ef0: 652c 2073 7572 7669 7665 2e2a 207c 0a7c  e, survive.* |.|
-00002f00: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00002f10: 2f67 6974 6875 622e 636f 6d2f 6b65 6e6a  /github.com/kenj
-00002f20: 796f 756e 672f 4d69 6e41 7461 7222 3e4d  young/MinAtar">M
-00002f30: 696e 4174 6172 2f42 7265 616b 6f75 743c  inAtar/Breakout<
-00002f40: 2f61 3e3c 6272 3e60 226d 696e 6174 6172  /a><br>`"minatar
-00002f50: 2d62 7265 616b 6f75 7422 6020 7c3c 696d  -breakout"` |<im
-00002f60: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00002f70: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00002f80: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00002f90: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-00002fa0: 6173 7365 7473 2f6d 696e 6174 6172 2d62  assets/minatar-b
-00002fb0: 7265 616b 6f75 742e 6769 6622 2077 6964  reakout.gif" wid
-00002fc0: 7468 3d22 3530 7078 223e 7c20 6076 3060  th="50px">| `v0`
-00002fd0: 207c 202a 5061 6464 6c65 2c20 6261 6c6c   | *Paddle, ball
-00002fe0: 2c20 6272 6963 6b73 2c20 626f 756e 6365  , bricks, bounce
-00002ff0: 2c20 636c 6561 722e 2a20 7c0a 7c3c 6120  , clear.* |.|<a 
-00003000: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00003010: 7468 7562 2e63 6f6d 2f6b 656e 6a79 6f75  thub.com/kenjyou
-00003020: 6e67 2f4d 696e 4174 6172 223e 4d69 6e41  ng/MinAtar">MinA
-00003030: 7461 722f 4672 6565 7761 793c 2f61 3e3c  tar/Freeway</a><
-00003040: 6272 3e60 226d 696e 6174 6172 2d66 7265  br>`"minatar-fre
-00003050: 6577 6179 2260 207c 3c69 6d67 2073 7263  eway"` |<img src
-00003060: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00003070: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00003080: 636f 6d2f 736f 7465 7473 756b 2f70 6778  com/sotetsuk/pgx
-00003090: 2f6d 6169 6e2f 646f 6373 2f61 7373 6574  /main/docs/asset
-000030a0: 732f 6d69 6e61 7461 722d 6672 6565 7761  s/minatar-freewa
-000030b0: 792e 6769 6622 2077 6964 7468 3d22 3530  y.gif" width="50
-000030c0: 7078 223e 7c20 6076 3060 207c 202a 446f  px">| `v0` | *Do
-000030d0: 6467 696e 6720 6361 7273 2c20 636c 696d  dging cars, clim
-000030e0: 6269 6e67 2075 7020 6672 6565 7761 792e  bing up freeway.
-000030f0: 2a20 7c0a 7c3c 6120 6872 6566 3d22 6874  * |.|<a href="ht
-00003100: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003110: 2f6b 656e 6a79 6f75 6e67 2f4d 696e 4174  /kenjyoung/MinAt
-00003120: 6172 223e 4d69 6e41 7461 722f 5365 6171  ar">MinAtar/Seaq
-00003130: 7565 7374 3c2f 613e 3c62 723e 6022 6d69  uest</a><br>`"mi
-00003140: 6e61 7461 722d 7365 6171 7565 7374 2260  natar-seaquest"`
-00003150: 207c 3c69 6d67 2073 7263 3d22 6874 7470   |<img src="http
-00003160: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00003170: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
-00003180: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
-00003190: 646f 6373 2f61 7373 6574 732f 6d69 6e61  docs/assets/mina
-000031a0: 7461 722d 7365 6171 7565 7374 2e67 6966  tar-seaquest.gif
-000031b0: 2220 7769 6474 683d 2235 3070 7822 3e7c  " width="50px">|
-000031c0: 2060 7630 6020 7c20 2a55 6e64 6572 7761   `v0` | *Underwa
-000031d0: 7465 7220 7375 626d 6172 696e 6520 7265  ter submarine re
-000031e0: 7363 7565 2061 6e64 2063 6f6d 6261 742e  scue and combat.
-000031f0: 2a20 7c0a 7c3c 6120 6872 6566 3d22 6874  * |.|<a href="ht
-00003200: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003210: 2f6b 656e 6a79 6f75 6e67 2f4d 696e 4174  /kenjyoung/MinAt
-00003220: 6172 223e 4d69 6e41 7461 722f 5370 6163  ar">MinAtar/Spac
-00003230: 6549 6e76 6164 6572 733c 2f61 3e3c 6272  eInvaders</a><br
-00003240: 3e60 226d 696e 6174 6172 2d73 7061 6365  >`"minatar-space
-00003250: 5f69 6e76 6164 6572 7322 6020 7c3c 696d  _invaders"` |<im
-00003260: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00003270: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00003280: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00003290: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-000032a0: 6173 7365 7473 2f6d 696e 6174 6172 2d73  assets/minatar-s
-000032b0: 7061 6365 5f69 6e76 6164 6572 732e 6769  pace_invaders.gi
-000032c0: 6622 2077 6964 7468 3d22 3530 7078 223e  f" width="50px">
-000032d0: 7c20 6076 3060 207c 202a 416c 6965 6e20  | `v0` | *Alien 
-000032e0: 7368 6f6f 7465 7220 6761 6d65 2c20 646f  shooter game, do
-000032f0: 6467 6520 6275 6c6c 6574 732e 2a20 7c0a  dge bullets.* |.
-00003300: 7c3c 6120 6872 6566 3d22 6874 7470 733a  |<a href="https:
-00003310: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00003320: 7267 2f77 696b 692f 5265 7665 7273 6922  rg/wiki/Reversi"
-00003330: 3e4f 7468 656c 6c6f 3c2f 613e 3c62 723e  >Othello</a><br>
-00003340: 6022 6f74 6865 6c6c 6f22 6020 7c3c 696d  `"othello"` |<im
-00003350: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00003360: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00003370: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00003380: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-00003390: 6173 7365 7473 2f6f 7468 656c 6c6f 5f64  assets/othello_d
-000033a0: 6172 6b2e 6769 6622 2077 6964 7468 3d22  ark.gif" width="
-000033b0: 3630 7078 223e 3c69 6d67 2073 7263 3d22  60px"><img src="
-000033c0: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-000033d0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-000033e0: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
-000033f0: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
-00003400: 6f74 6865 6c6c 6f5f 6c69 6768 742e 6769  othello_light.gi
-00003410: 6622 2077 6964 7468 3d22 3630 7078 223e  f" width="60px">
-00003420: 7c20 6076 3060 207c 202a 466c 6970 2061  | `v0` | *Flip a
-00003430: 6e64 2063 6f6e 7175 6572 206f 7070 6f6e  nd conquer oppon
-00003440: 656e 7427 7320 7069 6563 6573 2e2a 207c  ent's pieces.* |
-00003450: 0a7c 3c61 2068 7265 663d 2268 7474 7073  .|<a href="https
-00003460: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-00003470: 6f72 672f 7769 6b69 2f53 686f 6769 223e  org/wiki/Shogi">
-00003480: 5368 6f67 693c 2f61 3e3c 6272 3e60 2273  Shogi</a><br>`"s
-00003490: 686f 6769 2260 207c 3c69 6d67 2073 7263  hogi"` |<img src
-000034a0: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-000034b0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-000034c0: 636f 6d2f 736f 7465 7473 756b 2f70 6778  com/sotetsuk/pgx
-000034d0: 2f6d 6169 6e2f 646f 6373 2f61 7373 6574  /main/docs/asset
-000034e0: 732f 7368 6f67 695f 6461 726b 2e67 6966  s/shogi_dark.gif
-000034f0: 2220 7769 6474 683d 2236 3070 7822 3e3c  " width="60px"><
-00003500: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00003510: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00003520: 6f6e 7465 6e74 2e63 6f6d 2f73 6f74 6574  ontent.com/sotet
-00003530: 7375 6b2f 7067 782f 6d61 696e 2f64 6f63  suk/pgx/main/doc
-00003540: 732f 6173 7365 7473 2f73 686f 6769 5f6c  s/assets/shogi_l
-00003550: 6967 6874 2e67 6966 2220 7769 6474 683d  ight.gif" width=
-00003560: 2236 3070 7822 3e20 7c20 6076 3060 207c  "60px"> | `v0` |
-00003570: 202a 4a61 7061 6e65 7365 2063 6865 7373   *Japanese chess
-00003580: 2077 6974 6820 6361 7074 7572 6564 2070   with captured p
-00003590: 6965 6365 732e 2a20 7c0a 7c3c 6120 6872  ieces.* |.|<a hr
-000035a0: 6566 3d22 6874 7470 733a 2f2f 7375 676f  ef="https://sugo
-000035b0: 726f 6b75 7961 2e6a 702f 702f 7375 7a75  rokuya.jp/p/suzu
-000035c0: 6d65 2d6a 6f6e 6722 3e53 7061 7272 6f77  me-jong">Sparrow
-000035d0: 204d 6168 6a6f 6e67 3c2f 613e 3c62 723e   Mahjong</a><br>
-000035e0: 6022 7370 6172 726f 775f 6d61 686a 6f6e  `"sparrow_mahjon
-000035f0: 6722 6020 7c3c 696d 6720 7372 633d 2268  g"` |<img src="h
-00003600: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00003610: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00003620: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-00003630: 696e 2f64 6f63 732f 6173 7365 7473 2f73  in/docs/assets/s
-00003640: 7061 7272 6f77 5f6d 6168 6a6f 6e67 5f64  parrow_mahjong_d
-00003650: 6172 6b2e 7376 6722 2077 6964 7468 3d22  ark.svg" width="
-00003660: 3630 7078 223e 3c69 6d67 2073 7263 3d22  60px"><img src="
-00003670: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00003680: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00003690: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
-000036a0: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
-000036b0: 7370 6172 726f 775f 6d61 686a 6f6e 675f  sparrow_mahjong_
-000036c0: 6c69 6768 742e 7376 6722 2077 6964 7468  light.svg" width
-000036d0: 3d22 3630 7078 223e 7c20 2060 7630 6020  ="60px">|  `v0` 
-000036e0: 7c20 2a41 2073 696d 706c 6966 6965 642c  | *A simplified,
-000036f0: 2063 6869 6c64 7265 6e2d 6672 6965 6e64   children-friend
-00003700: 6c79 204d 6168 6a6f 6e67 2e2a 207c 0a7c  ly Mahjong.* |.|
-00003710: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00003720: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-00003730: 672f 7769 6b69 2f54 6963 2d74 6163 2d74  g/wiki/Tic-tac-t
-00003740: 6f65 223e 5469 632d 7461 632d 746f 653c  oe">Tic-tac-toe<
-00003750: 2f61 3e3c 6272 3e60 2274 6963 5f74 6163  /a><br>`"tic_tac
-00003760: 5f74 6f65 2260 207c 3c69 6d67 2073 7263  _toe"` |<img src
-00003770: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00003780: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00003790: 636f 6d2f 736f 7465 7473 756b 2f70 6778  com/sotetsuk/pgx
-000037a0: 2f6d 6169 6e2f 646f 6373 2f61 7373 6574  /main/docs/asset
-000037b0: 732f 7469 635f 7461 635f 746f 655f 6461  s/tic_tac_toe_da
-000037c0: 726b 2e67 6966 2220 7769 6474 683d 2236  rk.gif" width="6
-000037d0: 3070 7822 3e3c 696d 6720 7372 633d 2268  0px"><img src="h
-000037e0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-000037f0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00003800: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-00003810: 696e 2f64 6f63 732f 6173 7365 7473 2f74  in/docs/assets/t
-00003820: 6963 5f74 6163 5f74 6f65 5f6c 6967 6874  ic_tac_toe_light
-00003830: 2e67 6966 2220 7769 6474 683d 2236 3070  .gif" width="60p
-00003840: 7822 3e7c 2060 7630 6020 7c20 2a54 6872  x">| `v0` | *Thr
-00003850: 6565 2069 6e20 6120 726f 7720 7769 6e73  ee in a row wins
-00003860: 2e2a 207c 0a0a 2d20 3c61 2068 7265 663d  .* |..- <a href=
-00003870: 2268 7474 7073 3a2f 2f65 6e2e 7769 6b69  "https://en.wiki
-00003880: 7065 6469 612e 6f72 672f 7769 6b69 2f4a  pedia.org/wiki/J
-00003890: 6170 616e 6573 655f 6d61 686a 6f6e 6722  apanese_mahjong"
-000038a0: 3e4d 6168 6a6f 6e67 3c2f 613e 2065 6e76  >Mahjong</a> env
-000038b0: 6972 6f6e 6d65 6e74 7320 6172 6520 756e  ironments are un
-000038c0: 6465 7220 6465 7665 6c6f 706d 656e 7420  der development 
-000038d0: f09f 9aa7 2049 6620 796f 7520 6861 7665  .... If you have
-000038e0: 2061 6e79 2072 6571 7565 7374 7320 666f   any requests fo
-000038f0: 7220 6e65 7720 656e 7669 726f 6e6d 656e  r new environmen
-00003900: 7473 2c20 706c 6561 7365 206c 6574 2075  ts, please let u
-00003910: 7320 6b6e 6f77 2062 7920 5b6f 7065 6e69  s know by [openi
-00003920: 6e67 2061 6e20 6973 7375 655d 2868 7474  ng an issue](htt
-00003930: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003940: 736f 7465 7473 756b 2f70 6778 2f69 7373  sotetsuk/pgx/iss
-00003950: 7565 732f 6e65 7729 0a2d 2046 6976 652d  ues/new).- Five-
-00003960: 776f 7264 2064 6573 6372 6970 7469 6f6e  word description
-00003970: 7320 7765 7265 2067 656e 6572 6174 6564  s were generated
-00003980: 2062 7920 5b43 6861 7447 5054 5d28 6874   by [ChatGPT](ht
-00003990: 7470 733a 2f2f 6368 6174 2e6f 7065 6e61  tps://chat.opena
-000039a0: 692e 636f 6d2f 2920 f09f a496 0a0a 2323  i.com/) ......##
-000039b0: 2320 5665 7273 696f 6e69 6e67 2070 6f6c  # Versioning pol
-000039c0: 6963 790a 0a45 6163 6820 656e 7669 726f  icy..Each enviro
-000039d0: 6e6d 656e 7420 6973 2076 6572 7369 6f6e  nment is version
-000039e0: 6564 2c20 616e 6420 7468 6520 7665 7273  ed, and the vers
-000039f0: 696f 6e20 6973 2069 6e63 7265 6d65 6e74  ion is increment
-00003a00: 6564 2077 6865 6e20 7468 6572 6520 6172  ed when there ar
-00003a10: 6520 6368 616e 6765 7320 7468 6174 2061  e changes that a
-00003a20: 6666 6563 7420 7468 6520 7065 7266 6f72  ffect the perfor
-00003a30: 6d61 6e63 6520 6f66 2061 6765 6e74 7320  mance of agents 
-00003a40: 6f72 2077 6865 6e20 7468 6572 6520 6172  or when there ar
-00003a50: 6520 6368 616e 6765 7320 7468 6174 2061  e changes that a
-00003a60: 7265 206e 6f74 2062 6163 6b77 6172 6420  re not backward 
-00003a70: 636f 6d70 6174 6962 6c65 2077 6974 6820  compatible with 
-00003a80: 7468 6520 4150 492e 0a49 6620 796f 7520  the API..If you 
-00003a90: 7761 6e74 2074 6f20 7075 7273 7565 2063  want to pursue c
-00003aa0: 6f6d 706c 6574 6520 7265 7072 6f64 7563  omplete reproduc
-00003ab0: 6962 696c 6974 792c 2077 6520 7265 636f  ibility, we reco
-00003ac0: 6d6d 656e 6420 7468 6174 2079 6f75 2063  mmend that you c
-00003ad0: 6865 636b 2074 6865 2076 6572 7369 6f6e  heck the version
-00003ae0: 206f 6620 5067 7820 616e 6420 6561 6368   of Pgx and each
-00003af0: 2065 6e76 6972 6f6e 6d65 6e74 2061 7320   environment as 
-00003b00: 666f 6c6c 6f77 733a 0a0a 6060 6070 790a  follows:..```py.
-00003b10: 3e3e 3e20 7067 782e 5f5f 7665 7273 696f  >>> pgx.__versio
-00003b20: 6e5f 5f0a 2731 2e30 2e30 270a 3e3e 3e20  n__.'1.0.0'.>>> 
-00003b30: 656e 762e 7665 7273 696f 6e0a 2776 3027  env.version.'v0'
-00003b40: 0a60 6060 0a0a 2323 2053 6565 2061 6c73  .```..## See als
-00003b50: 6f0a 0a50 6778 2069 7320 696e 7465 6e64  o..Pgx is intend
-00003b60: 6564 2074 6f20 636f 6d70 6c65 6d65 6e74  ed to complement
-00003b70: 2074 6865 7365 202a 2a4a 4158 2d6e 6174   these **JAX-nat
-00003b80: 6976 6520 656e 7669 726f 6e6d 656e 7473  ive environments
-00003b90: 2a2a 2077 6974 6820 2863 6c61 7373 6963  ** with (classic
-00003ba0: 2920 626f 6172 6420 6761 6d65 2073 7569  ) board game sui
-00003bb0: 7473 3a0a 0a2d 205b 526f 6265 7274 544c  ts:..- [RobertTL
-00003bc0: 616e 6765 2f67 796d 6e61 785d 2868 7474  ange/gymnax](htt
-00003bd0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003be0: 526f 6265 7274 544c 616e 6765 2f67 796d  RobertTLange/gym
-00003bf0: 6e61 7829 3a20 4a41 5820 696d 706c 656d  nax): JAX implem
-00003c00: 656e 7461 7469 6f6e 206f 6620 706f 7075  entation of popu
-00003c10: 6c61 7220 524c 2065 6e76 6972 6f6e 6d65  lar RL environme
-00003c20: 6e74 7320 285b 636c 6173 7369 6320 636f  nts ([classic co
-00003c30: 6e74 726f 6c5d 2868 7474 7073 3a2f 2f67  ntrol](https://g
-00003c40: 796d 6e61 7369 756d 2e66 6172 616d 612e  ymnasium.farama.
-00003c50: 6f72 672f 656e 7669 726f 6e6d 656e 7473  org/environments
-00003c60: 2f63 6c61 7373 6963 5f63 6f6e 7472 6f6c  /classic_control
-00003c70: 292c 205b 6273 7569 7465 5d28 6874 7470  ), [bsuite](http
-00003c80: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-00003c90: 6565 706d 696e 642f 6273 7569 7465 292c  eepmind/bsuite),
-00003ca0: 204d 696e 4174 6172 2c20 6574 6329 2061   MinAtar, etc) a
-00003cb0: 6e64 206d 6574 6120 524c 2074 6173 6b73  nd meta RL tasks
-00003cc0: 0a2d 205b 676f 6f67 6c65 2f62 7261 785d  .- [google/brax]
-00003cd0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003ce0: 636f 6d2f 676f 6f67 6c65 2f62 7261 7829  com/google/brax)
-00003cf0: 3a20 5269 6769 6462 6f64 7920 7068 7973  : Rigidbody phys
-00003d00: 6963 7320 7369 6d75 6c61 7469 6f6e 2069  ics simulation i
-00003d10: 6e20 4a41 5820 616e 6420 636f 6e74 696e  n JAX and contin
-00003d20: 756f 7573 2d73 7061 6365 2052 4c20 7461  uous-space RL ta
-00003d30: 736b 7320 2861 6e74 2c20 6665 7463 682c  sks (ant, fetch,
-00003d40: 2068 756d 616e 6f69 642c 2065 7463 290a   humanoid, etc).
-00003d50: 2d20 5b69 6e73 7461 6465 6570 6169 2f6a  - [instadeepai/j
-00003d60: 756d 616e 6a69 5d28 6874 7470 733a 2f2f  umanji](https://
-00003d70: 6769 7468 7562 2e63 6f6d 2f69 6e73 7461  github.com/insta
-00003d80: 6465 6570 6169 2f6a 756d 616e 6a69 293a  deepai/jumanji):
-00003d90: 2041 2073 7569 7465 206f 6620 6469 7665   A suite of dive
-00003da0: 7273 6520 616e 6420 6368 616c 6c65 6e67  rse and challeng
-00003db0: 696e 670a 2020 2020 524c 2065 6e76 6972  ing.    RL envir
-00003dc0: 6f6e 6d65 6e74 7320 696e 204a 4158 2028  onments in JAX (
-00003dd0: 6269 6e2d 7061 636b 696e 672c 2072 6f75  bin-packing, rou
-00003de0: 7469 6e67 2070 726f 626c 656d 732c 2065  ting problems, e
-00003df0: 7463 290a 0a43 6f6d 6269 6e69 6e67 2050  tc)..Combining P
-00003e00: 6778 2077 6974 6820 7468 6573 6520 2a2a  gx with these **
-00003e10: 4a41 582d 6e61 7469 7665 2061 6c67 6f72  JAX-native algor
-00003e20: 6974 686d 732f 696d 706c 656d 656e 7461  ithms/implementa
-00003e30: 7469 6f6e 732a 2a20 6d69 6768 7420 6265  tions** might be
-00003e40: 2061 6e20 696e 7465 7265 7374 696e 6720   an interesting 
-00003e50: 6469 7265 6374 696f 6e3a 0a0a 2d20 5b41  direction:..- [A
-00003e60: 6e61 6b69 6e20 6672 616d 6577 6f72 6b5d  nakin framework]
-00003e70: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
-00003e80: 7267 2f61 6273 2f32 3130 342e 3036 3237  rg/abs/2104.0627
-00003e90: 3229 3a20 4869 6768 6c79 2065 6666 6963  2): Highly effic
-00003ea0: 6965 6e74 2052 4c20 6672 616d 6577 6f72  ient RL framewor
-00003eb0: 6b20 7468 6174 2077 6f72 6b73 2077 6974  k that works wit
-00003ec0: 6820 4a41 582d 6e61 7469 7665 2065 6e76  h JAX-native env
-00003ed0: 6972 6f6e 6d65 6e74 7320 6f6e 2054 5055  ironments on TPU
-00003ee0: 730a 2d20 5b64 6565 706d 696e 642f 6d63  s.- [deepmind/mc
-00003ef0: 7478 5d28 6874 7470 733a 2f2f 6769 7468  tx](https://gith
-00003f00: 7562 2e63 6f6d 2f64 6565 706d 696e 642f  ub.com/deepmind/
-00003f10: 6d63 7478 293a 204a 4158 2d6e 6174 6976  mctx): JAX-nativ
-00003f20: 6520 4d43 5453 2069 6d70 6c65 6d65 6e74  e MCTS implement
-00003f30: 6174 696f 6e73 2c20 696e 636c 7564 696e  ations, includin
-00003f40: 6720 416c 7068 615a 6572 6f20 616e 6420  g AlphaZero and 
-00003f50: 4d75 5a65 726f 0a2d 205b 6465 6570 6d69  MuZero.- [deepmi
-00003f60: 6e64 2f72 6c61 785d 2868 7474 7073 3a2f  nd/rlax](https:/
-00003f70: 2f67 6974 6875 622e 636f 6d2f 6465 6570  /github.com/deep
-00003f80: 6d69 6e64 2f72 6c61 7829 3a20 4a41 582d  mind/rlax): JAX-
-00003f90: 6e61 7469 7665 2052 4c20 636f 6d70 6f6e  native RL compon
-00003fa0: 656e 7473 0a2d 205b 676f 6f67 6c65 2f65  ents.- [google/e
-00003fb0: 766f 6a61 785d 2868 7474 7073 3a2f 2f67  vojax](https://g
-00003fc0: 6974 6875 622e 636f 6d2f 676f 6f67 6c65  ithub.com/google
-00003fd0: 2f65 766f 6a61 7829 3a20 4861 7264 7761  /evojax): Hardwa
-00003fe0: 7265 2d41 6363 656c 6572 6174 6564 206e  re-Accelerated n
-00003ff0: 6575 726f 6576 6f6c 7574 696f 6e0a 2d20  euroevolution.- 
-00004000: 5b52 6f62 6572 7454 4c61 6e67 652f 6576  [RobertTLange/ev
-00004010: 6f73 6178 5d28 6874 7470 733a 2f2f 6769  osax](https://gi
-00004020: 7468 7562 2e63 6f6d 2f52 6f62 6572 7454  thub.com/RobertT
-00004030: 4c61 6e67 652f 6576 6f73 6178 293a 204a  Lange/evosax): J
-00004040: 4158 2d6e 6174 6976 6520 6576 6f6c 7574  AX-native evolut
-00004050: 696f 6e20 7374 7261 7465 6779 2028 4553  ion strategy (ES
-00004060: 2920 696d 706c 656d 656e 7461 7469 6f6e  ) implementation
-00004070: 730a 2d20 5b61 6461 7074 6976 652d 696e  s.- [adaptive-in
-00004080: 7465 6c6c 6967 656e 742d 726f 626f 7469  telligent-roboti
-00004090: 6373 2f51 4461 785d 2868 7474 7073 3a2f  cs/QDax](https:/
-000040a0: 2f67 6974 6875 622e 636f 6d2f 6164 6170  /github.com/adap
-000040b0: 7469 7665 2d69 6e74 656c 6c69 6765 6e74  tive-intelligent
-000040c0: 2d72 6f62 6f74 6963 732f 5144 6178 293a  -robotics/QDax):
-000040d0: 204a 4158 2d6e 6174 6976 6520 5175 616c   JAX-native Qual
-000040e0: 6974 792d 4469 7665 7273 6974 7920 2851  ity-Diversity (Q
-000040f0: 4429 2061 6c67 6f72 6974 686d 730a 2d20  D) algorithms.- 
-00004100: 5b6c 7563 6872 6973 3432 392f 7075 7265  [luchris429/pure
-00004110: 6a61 7872 6c5d 2868 7474 7073 3a2f 2f67  jaxrl](https://g
-00004120: 6974 6875 622e 636f 6d2f 6c75 6368 7269  ithub.com/luchri
-00004130: 7334 3239 2f70 7572 656a 6178 726c 293a  s429/purejaxrl):
-00004140: 204a 6178 2d6e 6174 6976 6520 524c 2069   Jax-native RL i
-00004150: 6d70 6c65 6d65 6e74 6174 696f 6e73 0a0a  mplementations..
-00004160: 2323 2043 6974 6174 696f 6e0a 0a60 6060  ## Citation..```
-00004170: 0a40 6172 7469 636c 657b 6b6f 7961 6d61  .@article{koyama
-00004180: 6461 3230 3233 7067 782c 0a20 2074 6974  da2023pgx,.  tit
-00004190: 6c65 3d7b 5067 783a 2048 6172 6477 6172  le={Pgx: Hardwar
-000041a0: 652d 6163 6365 6c65 7261 7465 6420 7061  e-accelerated pa
-000041b0: 7261 6c6c 656c 2067 616d 6520 7369 6d75  rallel game simu
-000041c0: 6c61 7469 6f6e 2066 6f72 2072 6569 6e66  lation for reinf
-000041d0: 6f72 6365 6d65 6e74 206c 6561 726e 696e  orcement learnin
-000041e0: 677d 2c0a 2020 6175 7468 6f72 3d7b 4b6f  g},.  author={Ko
-000041f0: 7961 6d61 6461 2c20 536f 7465 7473 7520  yamada, Sotetsu 
-00004200: 616e 6420 4f6b 616e 6f2c 2053 6869 6e72  and Okano, Shinr
-00004210: 6920 616e 6420 4e69 7368 696d 6f72 692c  i and Nishimori,
-00004220: 2053 6f69 6368 6972 6f20 616e 6420 4d75   Soichiro and Mu
-00004230: 7261 7461 2c20 5975 2061 6e64 2048 6162  rata, Yu and Hab
-00004240: 6172 612c 204b 6569 676f 2061 6e64 204b  ara, Keigo and K
-00004250: 6974 612c 2048 6172 756b 6120 616e 6420  ita, Haruka and 
-00004260: 4973 6869 692c 2053 6869 6e7d 2c0a 2020  Ishii, Shin},.  
-00004270: 6a6f 7572 6e61 6c3d 7b61 7258 6976 2070  journal={arXiv p
-00004280: 7265 7072 696e 7420 6172 5869 763a 3233  reprint arXiv:23
-00004290: 3033 2e31 3735 3033 7d2c 0a20 2079 6561  03.17503},.  yea
-000042a0: 723d 7b32 3032 337d 0a7d 0a60 6060 0a0a  r={2023}.}.```..
-000042b0: 2323 204c 4943 454e 5345 0a0a 4170 6163  ## LICENSE..Apac
-000042c0: 6865 2d32 2e30 0a                        he-2.0.
+00001d90: 6f63 732f 6173 7365 7473 2f63 6f6e 6e65  ocs/assets/conne
+00001da0: 6374 5f66 6f75 725f 6461 726b 2e67 6966  ct_four_dark.gif
+00001db0: 2220 7769 6474 683d 2236 3070 7822 3e3c  " width="60px"><
+00001dc0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001dd0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00001de0: 6f6e 7465 6e74 2e63 6f6d 2f73 6f74 6574  ontent.com/sotet
+00001df0: 7375 6b2f 7067 782f 6d61 696e 2f64 6f63  suk/pgx/main/doc
+00001e00: 732f 6173 7365 7473 2f63 6f6e 6e65 6374  s/assets/connect
+00001e10: 5f66 6f75 725f 6c69 6768 742e 6769 6622  _four_light.gif"
+00001e20: 2077 6964 7468 3d22 3630 7078 223e 7c20   width="60px">| 
+00001e30: 6076 3060 207c 202a 436f 6e6e 6563 7420  `v0` | *Connect 
+00001e40: 6469 7363 732c 2077 696e 2077 6974 6820  discs, win with 
+00001e50: 666f 7572 2e2a 207c 0a7c 3c61 2068 7265  four.* |.|<a hre
+00001e60: 663d 2268 7474 7073 3a2f 2f65 6e2e 7769  f="https://en.wi
+00001e70: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+00001e80: 2f4d 696e 6963 6865 7373 223e 4761 7264  /Minichess">Gard
+00001e90: 6e65 7220 4368 6573 733c 2f61 3e3c 6272  ner Chess</a><br
+00001ea0: 3e60 2267 6172 646e 6572 5f63 6865 7373  >`"gardner_chess
+00001eb0: 2260 7c3c 696d 6720 7372 633d 2268 7474  "`|<img src="htt
+00001ec0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00001ed0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
+00001ee0: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
+00001ef0: 2f64 6f63 732f 6173 7365 7473 2f67 6172  /docs/assets/gar
+00001f00: 646e 6572 5f63 6865 7373 5f64 6172 6b2e  dner_chess_dark.
+00001f10: 6769 6622 2077 6964 7468 3d22 3630 7078  gif" width="60px
+00001f20: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00001f30: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00001f40: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00001f50: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00001f60: 646f 6373 2f61 7373 6574 732f 6761 7264  docs/assets/gard
+00001f70: 6e65 725f 6368 6573 735f 6c69 6768 742e  ner_chess_light.
+00001f80: 6769 6622 2077 6964 7468 3d22 3630 7078  gif" width="60px
+00001f90: 223e 7c20 6076 3060 207c 202a 3578 3520  ">| `v0` | *5x5 
+00001fa0: 6368 6573 7320 7661 7269 616e 742c 2065  chess variant, e
+00001fb0: 7863 6c75 6469 6e67 2063 6173 746c 696e  xcluding castlin
+00001fc0: 672e 2a20 7c0a 7c3c 6120 6872 6566 3d22  g.* |.|<a href="
+00001fd0: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
+00001fe0: 6564 6961 2e6f 7267 2f77 696b 692f 476f  edia.org/wiki/Go
+00001ff0: 5f28 6761 6d65 2922 3e47 6f3c 2f61 3e3c  _(game)">Go</a><
+00002000: 6272 3e60 2267 6f5f 3978 3922 6020 6022  br>`"go_9x9"` `"
+00002010: 676f 5f31 3978 3139 2260 207c 3c69 6d67  go_19x19"` |<img
+00002020: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00002030: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00002040: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
+00002050: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
+00002060: 7373 6574 732f 676f 2d31 3978 3139 5f64  ssets/go-19x19_d
+00002070: 6172 6b2e 6769 6622 2077 6964 7468 3d22  ark.gif" width="
+00002080: 3630 7078 223e 3c69 6d67 2073 7263 3d22  60px"><img src="
+00002090: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+000020a0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+000020b0: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
+000020c0: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
+000020d0: 676f 2d31 3978 3139 5f6c 6967 6874 2e67  go-19x19_light.g
+000020e0: 6966 2220 7769 6474 683d 2236 3070 7822  if" width="60px"
+000020f0: 3e7c 2060 7630 6020 7c20 2a53 7472 6174  >| `v0` | *Strat
+00002100: 6567 6963 616c 6c79 2070 6c61 6365 2073  egically place s
+00002110: 746f 6e65 732c 2063 6c61 696d 2074 6572  tones, claim ter
+00002120: 7269 746f 7279 2e2a 207c 0a7c 3c61 2068  ritory.* |.|<a h
+00002130: 7265 663d 2268 7474 7073 3a2f 2f65 6e2e  ref="https://en.
+00002140: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
+00002150: 6b69 2f48 6578 5f28 626f 6172 645f 6761  ki/Hex_(board_ga
+00002160: 6d65 2922 3e48 6578 3c2f 613e 3c62 723e  me)">Hex</a><br>
+00002170: 6022 6865 7822 6020 7c3c 696d 6720 7372  `"hex"` |<img sr
+00002180: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00002190: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+000021a0: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
+000021b0: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
+000021c0: 7473 2f68 6578 5f64 6172 6b2e 6769 6622  ts/hex_dark.gif"
+000021d0: 2077 6964 7468 3d22 3630 7078 223e 3c69   width="60px"><i
+000021e0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000021f0: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00002200: 6e74 656e 742e 636f 6d2f 736f 7465 7473  ntent.com/sotets
+00002210: 756b 2f70 6778 2f6d 6169 6e2f 646f 6373  uk/pgx/main/docs
+00002220: 2f61 7373 6574 732f 6865 785f 6c69 6768  /assets/hex_ligh
+00002230: 742e 6769 6622 2077 6964 7468 3d22 3630  t.gif" width="60
+00002240: 7078 223e 7c20 6076 3060 207c 202a 436f  px">| `v0` | *Co
+00002250: 6e6e 6563 7420 6f70 706f 7369 7465 2073  nnect opposite s
+00002260: 6964 6573 2c20 626c 6f63 6b20 6f70 706f  ides, block oppo
+00002270: 6e65 6e74 2e2a 207c 0a7c 3c61 2068 7265  nent.* |.|<a hre
+00002280: 663d 2268 7474 7073 3a2f 2f65 6e2e 7769  f="https://en.wi
+00002290: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+000022a0: 2f4b 7568 6e5f 706f 6b65 7222 3e4b 7568  /Kuhn_poker">Kuh
+000022b0: 6e20 506f 6b65 723c 2f61 3e3c 6272 3e60  n Poker</a><br>`
+000022c0: 226b 7568 6e5f 706f 6b65 7222 6020 7c3c  "kuhn_poker"` |<
+000022d0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000022e0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+000022f0: 6f6e 7465 6e74 2e63 6f6d 2f73 6f74 6574  ontent.com/sotet
+00002300: 7375 6b2f 7067 782f 6d61 696e 2f64 6f63  suk/pgx/main/doc
+00002310: 732f 6173 7365 7473 2f6b 7568 6e5f 706f  s/assets/kuhn_po
+00002320: 6b65 725f 6461 726b 2e67 6966 2220 7769  ker_dark.gif" wi
+00002330: 6474 683d 2236 3070 7822 3e3c 696d 6720  dth="60px"><img 
+00002340: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00002350: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00002360: 6e74 2e63 6f6d 2f73 6f74 6574 7375 6b2f  nt.com/sotetsuk/
+00002370: 7067 782f 6d61 696e 2f64 6f63 732f 6173  pgx/main/docs/as
+00002380: 7365 7473 2f6b 7568 6e5f 706f 6b65 725f  sets/kuhn_poker_
+00002390: 6c69 6768 742e 6769 6622 2077 6964 7468  light.gif" width
+000023a0: 3d22 3630 7078 223e 7c20 6076 3060 207c  ="60px">| `v0` |
+000023b0: 202a 5468 7265 652d 6361 7264 2062 6574   *Three-card bet
+000023c0: 7469 6e67 2061 6e64 2062 6c75 6666 696e  ting and bluffin
+000023d0: 6720 6761 6d65 2e2a 207c 0a7c 3c61 2068  g game.* |.|<a h
+000023e0: 7265 663d 2268 7474 7073 3a2f 2f61 7278  ref="https://arx
+000023f0: 6976 2e6f 7267 2f61 6273 2f31 3230 372e  iv.org/abs/1207.
+00002400: 3134 3131 223e 4c65 6475 6320 686f 6c64  1411">Leduc hold
+00002410: 2765 6d3c 2f61 3e3c 6272 3e60 226c 6564  'em</a><br>`"led
+00002420: 7563 5f68 6f6c 6465 6d22 6020 7c3c 696d  uc_holdem"` |<im
+00002430: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+00002440: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00002450: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
+00002460: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
+00002470: 6173 7365 7473 2f6c 6564 7563 5f68 6f6c  assets/leduc_hol
+00002480: 6465 6d5f 6461 726b 2e67 6966 2220 7769  dem_dark.gif" wi
+00002490: 6474 683d 2236 3070 7822 3e3c 696d 6720  dth="60px"><img 
+000024a0: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+000024b0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000024c0: 6e74 2e63 6f6d 2f73 6f74 6574 7375 6b2f  nt.com/sotetsuk/
+000024d0: 7067 782f 6d61 696e 2f64 6f63 732f 6173  pgx/main/docs/as
+000024e0: 7365 7473 2f6c 6564 7563 5f68 6f6c 6465  sets/leduc_holde
+000024f0: 6d5f 6c69 6768 742e 6769 6622 2077 6964  m_light.gif" wid
+00002500: 7468 3d22 3630 7078 223e 7c20 6076 3060  th="60px">| `v0`
+00002510: 207c 202a 5477 6f2d 7375 6974 2c20 6c69   | *Two-suit, li
+00002520: 6d69 7465 6420 6465 636b 2070 6f6b 6572  mited deck poker
+00002530: 2e2a 207c 0a7c 3c61 2068 7265 663d 2268  .* |.|<a href="h
+00002540: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002550: 6d2f 6b65 6e6a 796f 756e 672f 4d69 6e41  m/kenjyoung/MinA
+00002560: 7461 7222 3e4d 696e 4174 6172 2f41 7374  tar">MinAtar/Ast
+00002570: 6572 6978 3c2f 613e 3c62 723e 6022 6d69  erix</a><br>`"mi
+00002580: 6e61 7461 722d 6173 7465 7269 7822 6020  natar-asterix"` 
+00002590: 7c3c 696d 6720 7372 633d 2268 7474 7073  |<img src="https
+000025a0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+000025b0: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
+000025c0: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
+000025d0: 6f63 732f 6173 7365 7473 2f6d 696e 6174  ocs/assets/minat
+000025e0: 6172 2d61 7374 6572 6978 2e67 6966 2220  ar-asterix.gif" 
+000025f0: 7769 6474 683d 2235 3070 7822 3e7c 2060  width="50px">| `
+00002600: 7630 6020 7c20 2a41 766f 6964 2065 6e65  v0` | *Avoid ene
+00002610: 6d69 6573 2c20 636f 6c6c 6563 7420 7472  mies, collect tr
+00002620: 6561 7375 7265 2c20 7375 7276 6976 652e  easure, survive.
+00002630: 2a20 7c0a 7c3c 6120 6872 6566 3d22 6874  * |.|<a href="ht
+00002640: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002650: 2f6b 656e 6a79 6f75 6e67 2f4d 696e 4174  /kenjyoung/MinAt
+00002660: 6172 223e 4d69 6e41 7461 722f 4272 6561  ar">MinAtar/Brea
+00002670: 6b6f 7574 3c2f 613e 3c62 723e 6022 6d69  kout</a><br>`"mi
+00002680: 6e61 7461 722d 6272 6561 6b6f 7574 2260  natar-breakout"`
+00002690: 207c 3c69 6d67 2073 7263 3d22 6874 7470   |<img src="http
+000026a0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+000026b0: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+000026c0: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+000026d0: 646f 6373 2f61 7373 6574 732f 6d69 6e61  docs/assets/mina
+000026e0: 7461 722d 6272 6561 6b6f 7574 2e67 6966  tar-breakout.gif
+000026f0: 2220 7769 6474 683d 2235 3070 7822 3e7c  " width="50px">|
+00002700: 2060 7630 6020 7c20 2a50 6164 646c 652c   `v0` | *Paddle,
+00002710: 2062 616c 6c2c 2062 7269 636b 732c 2062   ball, bricks, b
+00002720: 6f75 6e63 652c 2063 6c65 6172 2e2a 207c  ounce, clear.* |
+00002730: 0a7c 3c61 2068 7265 663d 2268 7474 7073  .|<a href="https
+00002740: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b65  ://github.com/ke
+00002750: 6e6a 796f 756e 672f 4d69 6e41 7461 7222  njyoung/MinAtar"
+00002760: 3e4d 696e 4174 6172 2f46 7265 6577 6179  >MinAtar/Freeway
+00002770: 3c2f 613e 3c62 723e 6022 6d69 6e61 7461  </a><br>`"minata
+00002780: 722d 6672 6565 7761 7922 6020 7c3c 696d  r-freeway"` |<im
+00002790: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+000027a0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+000027b0: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
+000027c0: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
+000027d0: 6173 7365 7473 2f6d 696e 6174 6172 2d66  assets/minatar-f
+000027e0: 7265 6577 6179 2e67 6966 2220 7769 6474  reeway.gif" widt
+000027f0: 683d 2235 3070 7822 3e7c 2060 7630 6020  h="50px">| `v0` 
+00002800: 7c20 2a44 6f64 6769 6e67 2063 6172 732c  | *Dodging cars,
+00002810: 2063 6c69 6d62 696e 6720 7570 2066 7265   climbing up fre
+00002820: 6577 6179 2e2a 207c 0a7c 3c61 2068 7265  eway.* |.|<a hre
+00002830: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00002840: 622e 636f 6d2f 6b65 6e6a 796f 756e 672f  b.com/kenjyoung/
+00002850: 4d69 6e41 7461 7222 3e4d 696e 4174 6172  MinAtar">MinAtar
+00002860: 2f53 6561 7175 6573 743c 2f61 3e3c 6272  /Seaquest</a><br
+00002870: 3e60 226d 696e 6174 6172 2d73 6561 7175  >`"minatar-seaqu
+00002880: 6573 7422 6020 7c3c 696d 6720 7372 633d  est"` |<img src=
+00002890: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+000028a0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+000028b0: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
+000028c0: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
+000028d0: 2f6d 696e 6174 6172 2d73 6561 7175 6573  /minatar-seaques
+000028e0: 742e 6769 6622 2077 6964 7468 3d22 3530  t.gif" width="50
+000028f0: 7078 223e 7c20 6076 3060 207c 202a 556e  px">| `v0` | *Un
+00002900: 6465 7277 6174 6572 2073 7562 6d61 7269  derwater submari
+00002910: 6e65 2072 6573 6375 6520 616e 6420 636f  ne rescue and co
+00002920: 6d62 6174 2e2a 207c 0a7c 3c61 2068 7265  mbat.* |.|<a hre
+00002930: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00002940: 622e 636f 6d2f 6b65 6e6a 796f 756e 672f  b.com/kenjyoung/
+00002950: 4d69 6e41 7461 7222 3e4d 696e 4174 6172  MinAtar">MinAtar
+00002960: 2f53 7061 6365 496e 7661 6465 7273 3c2f  /SpaceInvaders</
+00002970: 613e 3c62 723e 6022 6d69 6e61 7461 722d  a><br>`"minatar-
+00002980: 7370 6163 655f 696e 7661 6465 7273 2260  space_invaders"`
+00002990: 207c 3c69 6d67 2073 7263 3d22 6874 7470   |<img src="http
+000029a0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+000029b0: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+000029c0: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+000029d0: 646f 6373 2f61 7373 6574 732f 6d69 6e61  docs/assets/mina
+000029e0: 7461 722d 7370 6163 655f 696e 7661 6465  tar-space_invade
+000029f0: 7273 2e67 6966 2220 7769 6474 683d 2235  rs.gif" width="5
+00002a00: 3070 7822 3e7c 2060 7630 6020 7c20 2a41  0px">| `v0` | *A
+00002a10: 6c69 656e 2073 686f 6f74 6572 2067 616d  lien shooter gam
+00002a20: 652c 2064 6f64 6765 2062 756c 6c65 7473  e, dodge bullets
+00002a30: 2e2a 207c 0a7c 3c61 2068 7265 663d 2268  .* |.|<a href="h
+00002a40: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+00002a50: 6469 612e 6f72 672f 7769 6b69 2f52 6576  dia.org/wiki/Rev
+00002a60: 6572 7369 223e 4f74 6865 6c6c 6f3c 2f61  ersi">Othello</a
+00002a70: 3e3c 6272 3e60 226f 7468 656c 6c6f 2260  ><br>`"othello"`
+00002a80: 207c 3c69 6d67 2073 7263 3d22 6874 7470   |<img src="http
+00002a90: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00002aa0: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00002ab0: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00002ac0: 646f 6373 2f61 7373 6574 732f 6f74 6865  docs/assets/othe
+00002ad0: 6c6c 6f5f 6461 726b 2e67 6966 2220 7769  llo_dark.gif" wi
+00002ae0: 6474 683d 2236 3070 7822 3e3c 696d 6720  dth="60px"><img 
+00002af0: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00002b00: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00002b10: 6e74 2e63 6f6d 2f73 6f74 6574 7375 6b2f  nt.com/sotetsuk/
+00002b20: 7067 782f 6d61 696e 2f64 6f63 732f 6173  pgx/main/docs/as
+00002b30: 7365 7473 2f6f 7468 656c 6c6f 5f6c 6967  sets/othello_lig
+00002b40: 6874 2e67 6966 2220 7769 6474 683d 2236  ht.gif" width="6
+00002b50: 3070 7822 3e7c 2060 7630 6020 7c20 2a46  0px">| `v0` | *F
+00002b60: 6c69 7020 616e 6420 636f 6e71 7565 7220  lip and conquer 
+00002b70: 6f70 706f 6e65 6e74 2773 2070 6965 6365  opponent's piece
+00002b80: 732e 2a20 7c0a 7c3c 6120 6872 6566 3d22  s.* |.|<a href="
+00002b90: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
+00002ba0: 6564 6961 2e6f 7267 2f77 696b 692f 5368  edia.org/wiki/Sh
+00002bb0: 6f67 6922 3e53 686f 6769 3c2f 613e 3c62  ogi">Shogi</a><b
+00002bc0: 723e 6022 7368 6f67 6922 6020 7c3c 696d  r>`"shogi"` |<im
+00002bd0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+00002be0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00002bf0: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
+00002c00: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
+00002c10: 6173 7365 7473 2f73 686f 6769 5f64 6172  assets/shogi_dar
+00002c20: 6b2e 6769 6622 2077 6964 7468 3d22 3630  k.gif" width="60
+00002c30: 7078 223e 3c69 6d67 2073 7263 3d22 6874  px"><img src="ht
+00002c40: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00002c50: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00002c60: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
+00002c70: 6e2f 646f 6373 2f61 7373 6574 732f 7368  n/docs/assets/sh
+00002c80: 6f67 695f 6c69 6768 742e 6769 6622 2077  ogi_light.gif" w
+00002c90: 6964 7468 3d22 3630 7078 223e 207c 2060  idth="60px"> | `
+00002ca0: 7630 6020 7c20 2a4a 6170 616e 6573 6520  v0` | *Japanese 
+00002cb0: 6368 6573 7320 7769 7468 2063 6170 7475  chess with captu
+00002cc0: 7265 6420 7069 6563 6573 2e2a 207c 0a7c  red pieces.* |.|
+00002cd0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00002ce0: 2f73 7567 6f72 6f6b 7579 612e 6a70 2f70  /sugorokuya.jp/p
+00002cf0: 2f73 757a 756d 652d 6a6f 6e67 223e 5370  /suzume-jong">Sp
+00002d00: 6172 726f 7720 4d61 686a 6f6e 673c 2f61  arrow Mahjong</a
+00002d10: 3e3c 6272 3e60 2273 7061 7272 6f77 5f6d  ><br>`"sparrow_m
+00002d20: 6168 6a6f 6e67 2260 207c 3c69 6d67 2073  ahjong"` |<img s
+00002d30: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00002d40: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002d50: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00002d60: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+00002d70: 6574 732f 7370 6172 726f 775f 6d61 686a  ets/sparrow_mahj
+00002d80: 6f6e 675f 6461 726b 2e73 7667 2220 7769  ong_dark.svg" wi
+00002d90: 6474 683d 2236 3070 7822 3e3c 696d 6720  dth="60px"><img 
+00002da0: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00002db0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00002dc0: 6e74 2e63 6f6d 2f73 6f74 6574 7375 6b2f  nt.com/sotetsuk/
+00002dd0: 7067 782f 6d61 696e 2f64 6f63 732f 6173  pgx/main/docs/as
+00002de0: 7365 7473 2f73 7061 7272 6f77 5f6d 6168  sets/sparrow_mah
+00002df0: 6a6f 6e67 5f6c 6967 6874 2e73 7667 2220  jong_light.svg" 
+00002e00: 7769 6474 683d 2236 3070 7822 3e7c 2020  width="60px">|  
+00002e10: 6076 3060 207c 202a 4120 7369 6d70 6c69  `v0` | *A simpli
+00002e20: 6669 6564 2c20 6368 696c 6472 656e 2d66  fied, children-f
+00002e30: 7269 656e 646c 7920 4d61 686a 6f6e 672e  riendly Mahjong.
+00002e40: 2a20 7c0a 7c3c 6120 6872 6566 3d22 6874  * |.|<a href="ht
+00002e50: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+00002e60: 6961 2e6f 7267 2f77 696b 692f 5469 632d  ia.org/wiki/Tic-
+00002e70: 7461 632d 746f 6522 3e54 6963 2d74 6163  tac-toe">Tic-tac
+00002e80: 2d74 6f65 3c2f 613e 3c62 723e 6022 7469  -toe</a><br>`"ti
+00002e90: 635f 7461 635f 746f 6522 6020 7c3c 696d  c_tac_toe"` |<im
+00002ea0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+00002eb0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00002ec0: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
+00002ed0: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
+00002ee0: 6173 7365 7473 2f74 6963 5f74 6163 5f74  assets/tic_tac_t
+00002ef0: 6f65 5f64 6172 6b2e 6769 6622 2077 6964  oe_dark.gif" wid
+00002f00: 7468 3d22 3630 7078 223e 3c69 6d67 2073  th="60px"><img s
+00002f10: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00002f20: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002f30: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00002f40: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+00002f50: 6574 732f 7469 635f 7461 635f 746f 655f  ets/tic_tac_toe_
+00002f60: 6c69 6768 742e 6769 6622 2077 6964 7468  light.gif" width
+00002f70: 3d22 3630 7078 223e 7c20 6076 3060 207c  ="60px">| `v0` |
+00002f80: 202a 5468 7265 6520 696e 2061 2072 6f77   *Three in a row
+00002f90: 2077 696e 732e 2a20 7c0a 0a2d 203c 6120   wins.* |..- <a 
+00002fa0: 6872 6566 3d22 6874 7470 733a 2f2f 656e  href="https://en
+00002fb0: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+00002fc0: 696b 692f 4a61 7061 6e65 7365 5f6d 6168  iki/Japanese_mah
+00002fd0: 6a6f 6e67 223e 4d61 686a 6f6e 673c 2f61  jong">Mahjong</a
+00002fe0: 3e20 656e 7669 726f 6e6d 656e 7473 2061  > environments a
+00002ff0: 7265 2075 6e64 6572 2064 6576 656c 6f70  re under develop
+00003000: 6d65 6e74 20f0 9f9a a720 4966 2079 6f75  ment .... If you
+00003010: 2068 6176 6520 616e 7920 7265 7175 6573   have any reques
+00003020: 7473 2066 6f72 206e 6577 2065 6e76 6972  ts for new envir
+00003030: 6f6e 6d65 6e74 732c 2070 6c65 6173 6520  onments, please 
+00003040: 6c65 7420 7573 206b 6e6f 7720 6279 205b  let us know by [
+00003050: 6f70 656e 696e 6720 616e 2069 7373 7565  opening an issue
+00003060: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00003070: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
+00003080: 782f 6973 7375 6573 2f6e 6577 290a 2d20  x/issues/new).- 
+00003090: 4669 7665 2d77 6f72 6420 6465 7363 7269  Five-word descri
+000030a0: 7074 696f 6e73 2077 6572 6520 6765 6e65  ptions were gene
+000030b0: 7261 7465 6420 6279 205b 4368 6174 4750  rated by [ChatGP
+000030c0: 545d 2868 7474 7073 3a2f 2f63 6861 742e  T](https://chat.
+000030d0: 6f70 656e 6169 2e63 6f6d 2f29 20f0 9fa4  openai.com/) ...
+000030e0: 960a 0a23 2323 2056 6572 7369 6f6e 696e  ...### Versionin
+000030f0: 6720 706f 6c69 6379 0a0a 4561 6368 2065  g policy..Each e
+00003100: 6e76 6972 6f6e 6d65 6e74 2069 7320 7665  nvironment is ve
+00003110: 7273 696f 6e65 642c 2061 6e64 2074 6865  rsioned, and the
+00003120: 2076 6572 7369 6f6e 2069 7320 696e 6372   version is incr
+00003130: 656d 656e 7465 6420 7768 656e 2074 6865  emented when the
+00003140: 7265 2061 7265 2063 6861 6e67 6573 2074  re are changes t
+00003150: 6861 7420 6166 6665 6374 2074 6865 2070  hat affect the p
+00003160: 6572 666f 726d 616e 6365 206f 6620 6167  erformance of ag
+00003170: 656e 7473 206f 7220 7768 656e 2074 6865  ents or when the
+00003180: 7265 2061 7265 2063 6861 6e67 6573 2074  re are changes t
+00003190: 6861 7420 6172 6520 6e6f 7420 6261 636b  hat are not back
+000031a0: 7761 7264 2063 6f6d 7061 7469 626c 6520  ward compatible 
+000031b0: 7769 7468 2074 6865 2041 5049 2e0a 4966  with the API..If
+000031c0: 2079 6f75 2077 616e 7420 746f 2070 7572   you want to pur
+000031d0: 7375 6520 636f 6d70 6c65 7465 2072 6570  sue complete rep
+000031e0: 726f 6475 6369 6269 6c69 7479 2c20 7765  roducibility, we
+000031f0: 2072 6563 6f6d 6d65 6e64 2074 6861 7420   recommend that 
+00003200: 796f 7520 6368 6563 6b20 7468 6520 7665  you check the ve
+00003210: 7273 696f 6e20 6f66 2050 6778 2061 6e64  rsion of Pgx and
+00003220: 2065 6163 6820 656e 7669 726f 6e6d 656e   each environmen
+00003230: 7420 6173 2066 6f6c 6c6f 7773 3a0a 0a60  t as follows:..`
+00003240: 6060 7079 0a3e 3e3e 2070 6778 2e5f 5f76  ``py.>>> pgx.__v
+00003250: 6572 7369 6f6e 5f5f 0a27 312e 302e 3027  ersion__.'1.0.0'
+00003260: 0a3e 3e3e 2065 6e76 2e76 6572 7369 6f6e  .>>> env.version
+00003270: 0a27 7630 270a 6060 600a 0a23 2320 5365  .'v0'.```..## Se
+00003280: 6520 616c 736f 0a0a 5067 7820 6973 2069  e also..Pgx is i
+00003290: 6e74 656e 6465 6420 746f 2063 6f6d 706c  ntended to compl
+000032a0: 656d 656e 7420 7468 6573 6520 2a2a 4a41  ement these **JA
+000032b0: 582d 6e61 7469 7665 2065 6e76 6972 6f6e  X-native environ
+000032c0: 6d65 6e74 732a 2a20 7769 7468 2028 636c  ments** with (cl
+000032d0: 6173 7369 6329 2062 6f61 7264 2067 616d  assic) board gam
+000032e0: 6520 7375 6974 733a 0a0a 2d20 5b52 6f62  e suits:..- [Rob
+000032f0: 6572 7454 4c61 6e67 652f 6779 6d6e 6178  ertTLange/gymnax
+00003300: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00003310: 2e63 6f6d 2f52 6f62 6572 7454 4c61 6e67  .com/RobertTLang
+00003320: 652f 6779 6d6e 6178 293a 204a 4158 2069  e/gymnax): JAX i
+00003330: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
+00003340: 2070 6f70 756c 6172 2052 4c20 656e 7669   popular RL envi
+00003350: 726f 6e6d 656e 7473 2028 5b63 6c61 7373  ronments ([class
+00003360: 6963 2063 6f6e 7472 6f6c 5d28 6874 7470  ic control](http
+00003370: 733a 2f2f 6779 6d6e 6173 6975 6d2e 6661  s://gymnasium.fa
+00003380: 7261 6d61 2e6f 7267 2f65 6e76 6972 6f6e  rama.org/environ
+00003390: 6d65 6e74 732f 636c 6173 7369 635f 636f  ments/classic_co
+000033a0: 6e74 726f 6c29 2c20 5b62 7375 6974 655d  ntrol), [bsuite]
+000033b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000033c0: 636f 6d2f 6465 6570 6d69 6e64 2f62 7375  com/deepmind/bsu
+000033d0: 6974 6529 2c20 4d69 6e41 7461 722c 2065  ite), MinAtar, e
+000033e0: 7463 2920 616e 6420 6d65 7461 2052 4c20  tc) and meta RL 
+000033f0: 7461 736b 730a 2d20 5b67 6f6f 676c 652f  tasks.- [google/
+00003400: 6272 6178 5d28 6874 7470 733a 2f2f 6769  brax](https://gi
+00003410: 7468 7562 2e63 6f6d 2f67 6f6f 676c 652f  thub.com/google/
+00003420: 6272 6178 293a 2052 6967 6964 626f 6479  brax): Rigidbody
+00003430: 2070 6879 7369 6373 2073 696d 756c 6174   physics simulat
+00003440: 696f 6e20 696e 204a 4158 2061 6e64 2063  ion in JAX and c
+00003450: 6f6e 7469 6e75 6f75 732d 7370 6163 6520  ontinuous-space 
+00003460: 524c 2074 6173 6b73 2028 616e 742c 2066  RL tasks (ant, f
+00003470: 6574 6368 2c20 6875 6d61 6e6f 6964 2c20  etch, humanoid, 
+00003480: 6574 6329 0a2d 205b 696e 7374 6164 6565  etc).- [instadee
+00003490: 7061 692f 6a75 6d61 6e6a 695d 2868 7474  pai/jumanji](htt
+000034a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000034b0: 696e 7374 6164 6565 7061 692f 6a75 6d61  instadeepai/juma
+000034c0: 6e6a 6929 3a20 4120 7375 6974 6520 6f66  nji): A suite of
+000034d0: 2064 6976 6572 7365 2061 6e64 2063 6861   diverse and cha
+000034e0: 6c6c 656e 6769 6e67 0a20 2020 2052 4c20  llenging.    RL 
+000034f0: 656e 7669 726f 6e6d 656e 7473 2069 6e20  environments in 
+00003500: 4a41 5820 2862 696e 2d70 6163 6b69 6e67  JAX (bin-packing
+00003510: 2c20 726f 7574 696e 6720 7072 6f62 6c65  , routing proble
+00003520: 6d73 2c20 6574 6329 0a0a 436f 6d62 696e  ms, etc)..Combin
+00003530: 696e 6720 5067 7820 7769 7468 2074 6865  ing Pgx with the
+00003540: 7365 202a 2a4a 4158 2d6e 6174 6976 6520  se **JAX-native 
+00003550: 616c 676f 7269 7468 6d73 2f69 6d70 6c65  algorithms/imple
+00003560: 6d65 6e74 6174 696f 6e73 2a2a 206d 6967  mentations** mig
+00003570: 6874 2062 6520 616e 2069 6e74 6572 6573  ht be an interes
+00003580: 7469 6e67 2064 6972 6563 7469 6f6e 3a0a  ting direction:.
+00003590: 0a2d 205b 416e 616b 696e 2066 7261 6d65  .- [Anakin frame
+000035a0: 776f 726b 5d28 6874 7470 733a 2f2f 6172  work](https://ar
+000035b0: 7869 762e 6f72 672f 6162 732f 3231 3034  xiv.org/abs/2104
+000035c0: 2e30 3632 3732 293a 2048 6967 686c 7920  .06272): Highly 
+000035d0: 6566 6669 6369 656e 7420 524c 2066 7261  efficient RL fra
+000035e0: 6d65 776f 726b 2074 6861 7420 776f 726b  mework that work
+000035f0: 7320 7769 7468 204a 4158 2d6e 6174 6976  s with JAX-nativ
+00003600: 6520 656e 7669 726f 6e6d 656e 7473 206f  e environments o
+00003610: 6e20 5450 5573 0a2d 205b 6465 6570 6d69  n TPUs.- [deepmi
+00003620: 6e64 2f6d 6374 785d 2868 7474 7073 3a2f  nd/mctx](https:/
+00003630: 2f67 6974 6875 622e 636f 6d2f 6465 6570  /github.com/deep
+00003640: 6d69 6e64 2f6d 6374 7829 3a20 4a41 582d  mind/mctx): JAX-
+00003650: 6e61 7469 7665 204d 4354 5320 696d 706c  native MCTS impl
+00003660: 656d 656e 7461 7469 6f6e 732c 2069 6e63  ementations, inc
+00003670: 6c75 6469 6e67 2041 6c70 6861 5a65 726f  luding AlphaZero
+00003680: 2061 6e64 204d 755a 6572 6f0a 2d20 5b64   and MuZero.- [d
+00003690: 6565 706d 696e 642f 726c 6178 5d28 6874  eepmind/rlax](ht
+000036a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000036b0: 2f64 6565 706d 696e 642f 726c 6178 293a  /deepmind/rlax):
+000036c0: 204a 4158 2d6e 6174 6976 6520 524c 2063   JAX-native RL c
+000036d0: 6f6d 706f 6e65 6e74 730a 2d20 5b67 6f6f  omponents.- [goo
+000036e0: 676c 652f 6576 6f6a 6178 5d28 6874 7470  gle/evojax](http
+000036f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
+00003700: 6f6f 676c 652f 6576 6f6a 6178 293a 2048  oogle/evojax): H
+00003710: 6172 6477 6172 652d 4163 6365 6c65 7261  ardware-Accelera
+00003720: 7465 6420 6e65 7572 6f65 766f 6c75 7469  ted neuroevoluti
+00003730: 6f6e 0a2d 205b 526f 6265 7274 544c 616e  on.- [RobertTLan
+00003740: 6765 2f65 766f 7361 785d 2868 7474 7073  ge/evosax](https
+00003750: 3a2f 2f67 6974 6875 622e 636f 6d2f 526f  ://github.com/Ro
+00003760: 6265 7274 544c 616e 6765 2f65 766f 7361  bertTLange/evosa
+00003770: 7829 3a20 4a41 582d 6e61 7469 7665 2065  x): JAX-native e
+00003780: 766f 6c75 7469 6f6e 2073 7472 6174 6567  volution strateg
+00003790: 7920 2845 5329 2069 6d70 6c65 6d65 6e74  y (ES) implement
+000037a0: 6174 696f 6e73 0a2d 205b 6164 6170 7469  ations.- [adapti
+000037b0: 7665 2d69 6e74 656c 6c69 6765 6e74 2d72  ve-intelligent-r
+000037c0: 6f62 6f74 6963 732f 5144 6178 5d28 6874  obotics/QDax](ht
+000037d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000037e0: 2f61 6461 7074 6976 652d 696e 7465 6c6c  /adaptive-intell
+000037f0: 6967 656e 742d 726f 626f 7469 6373 2f51  igent-robotics/Q
+00003800: 4461 7829 3a20 4a41 582d 6e61 7469 7665  Dax): JAX-native
+00003810: 2051 7561 6c69 7479 2d44 6976 6572 7369   Quality-Diversi
+00003820: 7479 2028 5144 2920 616c 676f 7269 7468  ty (QD) algorith
+00003830: 6d73 0a2d 205b 6c75 6368 7269 7334 3239  ms.- [luchris429
+00003840: 2f70 7572 656a 6178 726c 5d28 6874 7470  /purejaxrl](http
+00003850: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
+00003860: 7563 6872 6973 3432 392f 7075 7265 6a61  uchris429/pureja
+00003870: 7872 6c29 3a20 4a61 782d 6e61 7469 7665  xrl): Jax-native
+00003880: 2052 4c20 696d 706c 656d 656e 7461 7469   RL implementati
+00003890: 6f6e 730a 0a23 2320 4369 7461 7469 6f6e  ons..## Citation
+000038a0: 0a0a 4966 2079 6f75 2075 7365 2050 6778  ..If you use Pgx
+000038b0: 2069 6e20 796f 7572 2077 6f72 6b2c 2070   in your work, p
+000038c0: 6c65 6173 6520 6369 7465 2074 6865 2066  lease cite the f
+000038d0: 6f6c 6c6f 7769 6e67 2070 6170 6572 3a0a  ollowing paper:.
+000038e0: 0a60 6060 0a40 6172 7469 636c 657b 6b6f  .```.@article{ko
+000038f0: 7961 6d61 6461 3230 3233 7067 782c 0a20  yamada2023pgx,. 
+00003900: 2074 6974 6c65 3d7b 5067 783a 2048 6172   title={Pgx: Har
+00003910: 6477 6172 652d 6163 6365 6c65 7261 7465  dware-accelerate
+00003920: 6420 5061 7261 6c6c 656c 2047 616d 6520  d Parallel Game 
+00003930: 5369 6d75 6c61 746f 7273 2066 6f72 2052  Simulators for R
+00003940: 6569 6e66 6f72 6365 6d65 6e74 204c 6561  einforcement Lea
+00003950: 726e 696e 677d 2c0a 2020 6175 7468 6f72  rning},.  author
+00003960: 3d7b 4b6f 7961 6d61 6461 2c20 536f 7465  ={Koyamada, Sote
+00003970: 7473 7520 616e 6420 4f6b 616e 6f2c 2053  tsu and Okano, S
+00003980: 6869 6e72 6920 616e 6420 4e69 7368 696d  hinri and Nishim
+00003990: 6f72 692c 2053 6f69 6368 6972 6f20 616e  ori, Soichiro an
+000039a0: 6420 4d75 7261 7461 2c20 5975 2061 6e64  d Murata, Yu and
+000039b0: 2048 6162 6172 612c 204b 6569 676f 2061   Habara, Keigo a
+000039c0: 6e64 204b 6974 612c 2048 6172 756b 6120  nd Kita, Haruka 
+000039d0: 616e 6420 4973 6869 692c 2053 6869 6e7d  and Ishii, Shin}
+000039e0: 2c0a 2020 6a6f 7572 6e61 6c3d 7b61 7258  ,.  journal={arX
+000039f0: 6976 2070 7265 7072 696e 7420 6172 5869  iv preprint arXi
+00003a00: 763a 3233 3033 2e31 3735 3033 7d2c 0a20  v:2303.17503},. 
+00003a10: 2079 6561 723d 7b32 3032 337d 0a7d 0a60   year={2023}.}.`
+00003a20: 6060 0a0a 2323 204c 4943 454e 5345 0a0a  ``..## LICENSE..
+00003a30: 4170 6163 6865 2d32 2e30 0a              Apache-2.0.
```

### Comparing `pgx-1.0.0/README.md` & `pgx-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,1040 +1,961 @@
-00000000: 5b21 5b63 695d 2868 7474 7073 3a2f 2f67  [![ci](https://g
-00000010: 6974 6875 622e 636f 6d2f 736f 7465 7473  ithub.com/sotets
-00000020: 756b 2f70 6778 2f61 6374 696f 6e73 2f77  uk/pgx/actions/w
-00000030: 6f72 6b66 6c6f 7773 2f63 692e 796d 6c2f  orkflows/ci.yml/
-00000040: 6261 6467 652e 7376 6729 5d28 6874 7470  badge.svg)](http
-00000050: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00000060: 6f74 6574 7375 6b2f 7067 782f 6163 7469  otetsuk/pgx/acti
-00000070: 6f6e 732f 776f 726b 666c 6f77 732f 6369  ons/workflows/ci
-00000080: 2e79 6d6c 290a 0a3c 6469 7620 616c 6967  .yml)..<div alig
-00000090: 6e3d 2263 656e 7465 7222 3e0a 3c69 6d67  n="center">.<img
-000000a0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-000000b0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-000000c0: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
-000000d0: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
-000000e0: 7373 6574 732f 6c6f 676f 2e73 7667 2220  ssets/logo.svg" 
-000000f0: 7769 6474 683d 2234 3025 223e 0a3c 2f64  width="40%">.</d
-00000100: 6976 3e0a 0a41 2063 6f6c 6c65 6374 696f  iv>..A collectio
-00000110: 6e20 6f66 2047 5055 2f54 5055 2d61 6363  n of GPU/TPU-acc
-00000120: 656c 6572 6174 6564 2070 6172 616c 6c65  elerated paralle
-00000130: 6c20 6761 6d65 2073 696d 756c 6174 6f72  l game simulator
-00000140: 7320 666f 7220 7265 696e 666f 7263 656d  s for reinforcem
-00000150: 656e 7420 6c65 6172 6e69 6e67 2028 524c  ent learning (RL
-00000160: 290a 0a3c 6469 7620 616c 6967 6e3d 2263  )..<div align="c
-00000170: 656e 7465 7222 3e0a 3c69 6d67 2073 7263  enter">.<img src
-00000180: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00000190: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-000001a0: 636f 6d2f 736f 7465 7473 756b 2f70 6778  com/sotetsuk/pgx
-000001b0: 2f6d 6169 6e2f 646f 6373 2f61 7373 6574  /main/docs/asset
-000001c0: 732f 676f 5f64 6172 6b2e 6769 6623 6768  s/go_dark.gif#gh
-000001d0: 2d64 6172 6b2d 6d6f 6465 2d6f 6e6c 7922  -dark-mode-only"
-000001e0: 2077 6964 7468 3d22 3330 2522 3e3c 696d   width="30%"><im
-000001f0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00000200: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000210: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00000220: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-00000230: 6173 7365 7473 2f67 6f5f 6461 726b 2e67  assets/go_dark.g
-00000240: 6966 2367 682d 6461 726b 2d6d 6f64 652d  if#gh-dark-mode-
-00000250: 6f6e 6c79 2220 7769 6474 683d 2233 3025  only" width="30%
-00000260: 2220 7374 796c 653d 2274 7261 6e73 666f  " style="transfo
-00000270: 726d 3a72 6f74 6174 6528 3237 3064 6567  rm:rotate(270deg
-00000280: 293b 223e 3c69 6d67 2073 7263 3d22 6874  );"><img src="ht
-00000290: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-000002a0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-000002b0: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
-000002c0: 6e2f 646f 6373 2f61 7373 6574 732f 676f  n/docs/assets/go
-000002d0: 5f64 6172 6b2e 6769 6623 6768 2d64 6172  _dark.gif#gh-dar
-000002e0: 6b2d 6d6f 6465 2d6f 6e6c 7922 2077 6964  k-mode-only" wid
-000002f0: 7468 3d22 3330 2522 2073 7479 6c65 3d22  th="30%" style="
-00000300: 7472 616e 7366 6f72 6d3a 726f 7461 7465  transform:rotate
-00000310: 2839 3064 6567 293b 223e 0a3c 696d 6720  (90deg);">.<img 
-00000320: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00000330: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000340: 6e74 2e63 6f6d 2f73 6f74 6574 7375 6b2f  nt.com/sotetsuk/
-00000350: 7067 782f 6d61 696e 2f64 6f63 732f 6173  pgx/main/docs/as
-00000360: 7365 7473 2f67 6f5f 6c69 6768 742e 6769  sets/go_light.gi
-00000370: 6623 6768 2d6c 6967 6874 2d6d 6f64 652d  f#gh-light-mode-
-00000380: 6f6e 6c79 2220 7769 6474 683d 2233 3025  only" width="30%
-00000390: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-000003a0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-000003b0: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
-000003c0: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
-000003d0: 646f 6373 2f61 7373 6574 732f 676f 5f6c  docs/assets/go_l
-000003e0: 6967 6874 2e67 6966 2367 682d 6c69 6768  ight.gif#gh-ligh
-000003f0: 742d 6d6f 6465 2d6f 6e6c 7922 2077 6964  t-mode-only" wid
-00000400: 7468 3d22 3330 2522 2073 7479 6c65 3d22  th="30%" style="
-00000410: 7472 616e 7366 6f72 6d3a 726f 7461 7465  transform:rotate
-00000420: 2832 3730 6465 6729 3b22 3e3c 696d 6720  (270deg);"><img 
-00000430: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00000440: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000450: 6e74 2e63 6f6d 2f73 6f74 6574 7375 6b2f  nt.com/sotetsuk/
-00000460: 7067 782f 6d61 696e 2f64 6f63 732f 6173  pgx/main/docs/as
-00000470: 7365 7473 2f67 6f5f 6c69 6768 742e 6769  sets/go_light.gi
-00000480: 6623 6768 2d6c 6967 6874 2d6d 6f64 652d  f#gh-light-mode-
-00000490: 6f6e 6c79 2220 7769 6474 683d 2233 3025  only" width="30%
-000004a0: 2220 7374 796c 653d 2274 7261 6e73 666f  " style="transfo
-000004b0: 726d 3a72 6f74 6174 6528 3930 6465 6729  rm:rotate(90deg)
-000004c0: 3b22 3e0a 3c2f 6469 763e 0a0a f09f 8e89  ;">.</div>......
-000004d0: 202a 2a60 7631 2e30 2e30 602a 2a20 6973   **`v1.0.0`** is
-000004e0: 2072 656c 6561 7365 6421 2028 3230 3233   released! (2023
-000004f0: 2e36 2e32 3029 0a0a 2323 2057 6879 2050  .6.20)..## Why P
-00000500: 6778 3f0a 0a3c 212d 2d2d 200a 7468 726f  gx?..<!--- .thro
-00000510: 7567 6870 7574 3a20 6874 7470 733a 2f2f  ughput: https://
-00000520: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
-00000530: 6f6f 676c 652e 636f 6d2f 6472 6976 652f  oogle.com/drive/
-00000540: 3167 4957 4859 4c4b 4278 4532 584b 4468  1gIWHYLKBxE2XKDh
-00000550: 416c 4559 4b56 6563 7a33 5747 3463 7a64  AlEYKVecz3WG4czd
-00000560: 7a23 7363 726f 6c6c 546f 3d56 3151 5a68  z#scrollTo=V1QZh
-00000570: 5258 6f47 4c38 4b0a 2d2d 2d3e 0a0a 5b42  RXoGL8K.--->..[B
-00000580: 7261 785d 2868 7474 7073 3a2f 2f67 6974  rax](https://git
-00000590: 6875 622e 636f 6d2f 676f 6f67 6c65 2f62  hub.com/google/b
-000005a0: 7261 7829 2c20 6120 5b4a 4158 5d28 6874  rax), a [JAX](ht
-000005b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000005c0: 2f67 6f6f 676c 652f 6a61 7829 2d6e 6174  /google/jax)-nat
-000005d0: 6976 6520 7068 7973 6963 7320 656e 6769  ive physics engi
-000005e0: 6e65 2c20 7072 6f76 6964 6573 2065 7874  ne, provides ext
-000005f0: 7265 6d65 6c79 2068 6967 682d 7370 6565  remely high-spee
-00000600: 6420 7061 7261 6c6c 656c 2073 696d 756c  d parallel simul
-00000610: 6174 696f 6e20 666f 7220 524c 2069 6e20  ation for RL in 
-00000620: 2a63 6f6e 7469 6e75 6f75 732a 2073 7461  *continuous* sta
-00000630: 7465 2073 7061 6365 2e0a 5468 656e 2c20  te space..Then, 
-00000640: 7768 6174 2061 626f 7574 2052 4c20 696e  what about RL in
-00000650: 202a 6469 7363 7265 7465 2a20 7374 6174   *discrete* stat
-00000660: 6520 7370 6163 6573 206c 696b 6520 4368  e spaces like Ch
-00000670: 6573 732c 2053 686f 6769 2c20 616e 6420  ess, Shogi, and 
-00000680: 476f 3f20 2a2a 5067 782a 2a20 7072 6f76  Go? **Pgx** prov
-00000690: 6964 6573 2061 2077 6964 6520 7661 7269  ides a wide vari
-000006a0: 6574 7920 6f66 204a 4158 2d6e 6174 6976  ety of JAX-nativ
-000006b0: 6520 6761 6d65 2073 696d 756c 6174 6f72  e game simulator
-000006c0: 7321 2048 6967 686c 6967 6874 6564 2066  s! Highlighted f
-000006d0: 6561 7475 7265 7320 696e 636c 7564 653a  eatures include:
-000006e0: 0a0a 2d20 e29a a120 2a2a 5375 7065 7220  ..- ... **Super 
-000006f0: 6661 7374 2a2a 2069 6e20 7061 7261 6c6c  fast** in parall
-00000700: 656c 2065 7865 6375 7469 6f6e 206f 6e20  el execution on 
-00000710: 6163 6365 6c65 7261 746f 7273 0a2d 20f0  accelerators.- .
-00000720: 9f8e b220 2a2a 5661 7269 6f75 7320 6761  ... **Various ga
-00000730: 6d65 2073 7570 706f 7274 2a2a 2069 6e63  me support** inc
-00000740: 6c75 6469 6e67 202a 2a42 6163 6b67 616d  luding **Backgam
-00000750: 6d6f 6e2a 2a2c 202a 2a43 6865 7373 2a2a  mon**, **Chess**
-00000760: 2c20 2a2a 5368 6f67 692a 2a2c 2061 6e64  , **Shogi**, and
-00000770: 202a 2a47 6f2a 2a0a 2d20 f09f 96bc efb8   **Go**.- ......
-00000780: 8f20 2a2a 4265 6175 7469 6675 6c20 7669  . **Beautiful vi
-00000790: 7375 616c 697a 6174 696f 6e2a 2a20 696e  sualization** in
-000007a0: 2053 5647 2066 6f72 6d61 740a 0a0a 2323   SVG format...##
-000007b0: 2043 6f6c 6162 0a0a 2d20 5b47 6574 7469   Colab..- [Getti
-000007c0: 6e67 2073 7461 7274 6564 5d28 6874 7470  ng started](http
-000007d0: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
-000007e0: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
-000007f0: 7468 7562 2f73 6f74 6574 7375 6b2f 7067  thub/sotetsuk/pg
-00000800: 782f 626c 6f62 2f6d 6169 6e2f 636f 6c61  x/blob/main/cola
-00000810: 622f 7067 785f 6865 6c6c 6f5f 776f 726c  b/pgx_hello_worl
-00000820: 642e 6970 796e 6229 0a2d 205b 5067 7820  d.ipynb).- [Pgx 
-00000830: 6261 7365 6c69 6e65 206d 6f64 656c 735d  baseline models]
-00000840: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
-00000850: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
-00000860: 6f6d 2f67 6974 6875 622f 736f 7465 7473  om/github/sotets
-00000870: 756b 2f70 6778 2f62 6c6f 622f 6d61 696e  uk/pgx/blob/main
-00000880: 2f63 6f6c 6162 2f62 6173 656c 696e 6573  /colab/baselines
-00000890: 2e69 7079 6e62 290a 2d20 5b50 504f 2065  .ipynb).- [PPO e
-000008a0: 7861 6d70 6c65 5d28 6874 7470 733a 2f2f  xample](https://
-000008b0: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
-000008c0: 6f6f 676c 652e 636f 6d2f 6769 7468 7562  oogle.com/github
-000008d0: 2f73 6f74 6574 7375 6b2f 7067 782f 626c  /sotetsuk/pgx/bl
-000008e0: 6f62 2f6d 6169 6e2f 636f 6c61 622f 7070  ob/main/colab/pp
-000008f0: 6f2e 6970 796e 6229 0a2d 205b 4578 706f  o.ipynb).- [Expo
-00000900: 7274 2074 6f20 5065 7474 696e 675a 6f6f  rt to PettingZoo
-00000910: 2041 5049 5d28 6874 7470 733a 2f2f 636f   API](https://co
-00000920: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00000930: 676c 652e 636f 6d2f 6769 7468 7562 2f73  gle.com/github/s
-00000940: 6f74 6574 7375 6b2f 7067 782f 626c 6f62  otetsuk/pgx/blob
-00000950: 2f6d 6169 6e2f 636f 6c61 622f 7067 7832  /main/colab/pgx2
-00000960: 7065 7474 696e 677a 6f6f 2e69 7079 6e62  pettingzoo.ipynb
-00000970: 290a 0a23 2320 496e 7374 616c 6c61 7469  )..## Installati
-00000980: 6f6e 0a0a 6060 6073 680a 7069 7020 696e  on..```sh.pip in
-00000990: 7374 616c 6c20 7067 780a 6060 600a 0a4e  stall pgx.```..N
-000009a0: 6f74 6520 7468 6174 2074 6865 205b 4d69  ote that the [Mi
-000009b0: 6e41 7461 725d 2868 7474 7073 3a2f 2f67  nAtar](https://g
-000009c0: 6974 6875 622e 636f 6d2f 6b65 6e6a 796f  ithub.com/kenjyo
-000009d0: 756e 672f 4d69 6e41 7461 7229 2073 7569  ung/MinAtar) sui
-000009e0: 7465 2069 7320 7072 6f76 6964 6564 2061  te is provided a
-000009f0: 7320 6120 7365 7061 7261 7465 2065 7874  s a separate ext
-00000a00: 656e 7369 6f6e 2066 6f72 2050 6778 2028  ension for Pgx (
-00000a10: 5b60 7067 782d 6d69 6e61 7461 7260 5d28  [`pgx-minatar`](
-00000a20: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000a30: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782d  om/sotetsuk/pgx-
-00000a40: 6d69 6e61 7461 7229 292e 2054 6865 7265  minatar)). There
-00000a50: 666f 7265 2c20 706c 6561 7365 2072 756e  fore, please run
-00000a60: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00000a70: 6f6d 6d61 6e64 2061 6464 6974 696f 6e61  ommand additiona
-00000a80: 6c79 2074 6f20 7573 6520 7468 6520 4d69  ly to use the Mi
-00000a90: 6e41 7461 7220 7375 6974 6520 696e 2050  nAtar suite in P
-00000aa0: 6778 3a0a 0a60 6060 7368 0a70 6970 2069  gx:..```sh.pip i
-00000ab0: 6e73 7461 6c6c 2070 6778 2d6d 696e 6174  nstall pgx-minat
-00000ac0: 6172 0a60 6060 0a0a 5067 7820 6973 2070  ar.```..Pgx is p
-00000ad0: 726f 7669 6465 6420 756e 6465 7220 7468  rovided under th
-00000ae0: 6520 4170 6163 6865 2032 2e30 204c 6963  e Apache 2.0 Lic
-00000af0: 656e 7365 2c20 6275 7420 7468 6520 6f72  ense, but the or
-00000b00: 6967 696e 616c 204d 696e 4174 6172 2073  iginal MinAtar s
-00000b10: 7569 7465 2066 6f6c 6c6f 7773 2074 6865  uite follows the
-00000b20: 2047 504c 2033 2e30 204c 6963 656e 7365   GPL 3.0 License
-00000b30: 2e20 5468 6572 6566 6f72 652c 2070 6c65  . Therefore, ple
-00000b40: 6173 6520 6e6f 7465 2074 6861 7420 7468  ase note that th
-00000b50: 6520 7365 7061 7261 7465 6420 4d69 6e41  e separated MinA
-00000b60: 7461 7220 6578 7465 6e73 696f 6e20 666f  tar extension fo
-00000b70: 7220 5067 7820 616c 736f 2061 6468 6572  r Pgx also adher
-00000b80: 6573 2074 6f20 7468 6520 4750 4c20 332e  es to the GPL 3.
-00000b90: 3020 4c69 6365 6e73 652e 0a0a 2323 2055  0 License...## U
-00000ba0: 7361 6765 0a0a 0a4e 6f74 6520 7468 6174  sage...Note that
-00000bb0: 2061 6c6c 2060 7374 6570 6020 6675 6e63   all `step` func
-00000bc0: 7469 6f6e 7320 696e 2050 6778 2065 6e76  tions in Pgx env
-00000bd0: 6972 6f6e 6d65 6e74 7320 6172 6520 2a2a  ironments are **
-00000be0: 4a41 582d 6e61 7469 7665 2e2a 2a2c 2069  JAX-native.**, i
-00000bf0: 2e65 2e2c 2074 6865 7920 6172 6520 616c  .e., they are al
-00000c00: 6c20 2a4a 4954 2d61 626c 652a 2e0a 0a3c  l *JIT-able*...<
-00000c10: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000c20: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
-00000c30: 6f6f 676c 652e 636f 6d2f 6769 7468 7562  oogle.com/github
-00000c40: 2f73 6f74 6574 7375 6b2f 7067 782f 626c  /sotetsuk/pgx/bl
-00000c50: 6f62 2f6d 6169 6e2f 636f 6c61 622f 7067  ob/main/colab/pg
-00000c60: 785f 6865 6c6c 6f5f 776f 726c 642e 6970  x_hello_world.ip
-00000c70: 796e 6222 3e3c 696d 6720 7372 633d 2268  ynb"><img src="h
-00000c80: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
-00000c90: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
-00000ca0: 2f61 7373 6574 732f 636f 6c61 622d 6261  /assets/colab-ba
-00000cb0: 6467 652e 7376 6722 2061 6c74 3d22 4f70  dge.svg" alt="Op
-00000cc0: 656e 2049 6e20 436f 6c61 6222 2f3e 3c2f  en In Colab"/></
-00000cd0: 613e 0a0a 6060 6070 790a 696d 706f 7274  a>..```py.import
-00000ce0: 206a 6178 0a69 6d70 6f72 7420 7067 780a   jax.import pgx.
-00000cf0: 0a65 6e76 203d 2070 6778 2e6d 616b 6528  .env = pgx.make(
-00000d00: 2267 6f5f 3139 7831 3922 290a 696e 6974  "go_19x19").init
-00000d10: 203d 206a 6178 2e6a 6974 286a 6178 2e76   = jax.jit(jax.v
-00000d20: 6d61 7028 656e 762e 696e 6974 2929 2020  map(env.init))  
-00000d30: 2320 7665 6374 6f72 697a 6520 616e 6420  # vectorize and 
-00000d40: 4a49 542d 636f 6d70 696c 650a 7374 6570  JIT-compile.step
-00000d50: 203d 206a 6178 2e6a 6974 286a 6178 2e76   = jax.jit(jax.v
-00000d60: 6d61 7028 656e 762e 7374 6570 2929 0a0a  map(env.step))..
-00000d70: 6261 7463 685f 7369 7a65 203d 2031 3032  batch_size = 102
-00000d80: 340a 6b65 7973 203d 206a 6178 2e72 616e  4.keys = jax.ran
-00000d90: 646f 6d2e 7370 6c69 7428 6a61 782e 7261  dom.split(jax.ra
-00000da0: 6e64 6f6d 2e50 524e 474b 6579 2834 3229  ndom.PRNGKey(42)
-00000db0: 2c20 6261 7463 685f 7369 7a65 290a 7374  , batch_size).st
-00000dc0: 6174 6520 3d20 696e 6974 286b 6579 7329  ate = init(keys)
-00000dd0: 2020 2320 7665 6374 6f72 697a 6564 2073    # vectorized s
-00000de0: 7461 7465 730a 7768 696c 6520 6e6f 7420  tates.while not 
-00000df0: 2873 7461 7465 2e74 6572 6d69 6e61 7465  (state.terminate
-00000e00: 6420 7c20 7374 6174 652e 7472 756e 6361  d | state.trunca
-00000e10: 7465 6429 2e61 6c6c 2829 3a0a 2020 2020  ted).all():.    
-00000e20: 6163 7469 6f6e 203d 206d 6f64 656c 2873  action = model(s
-00000e30: 7461 7465 2e63 7572 7265 6e74 5f70 6c61  tate.current_pla
-00000e40: 7965 722c 2073 7461 7465 2e6f 6273 6572  yer, state.obser
-00000e50: 7661 7469 6f6e 2c20 7374 6174 652e 6c65  vation, state.le
-00000e60: 6761 6c5f 6163 7469 6f6e 5f6d 6173 6b29  gal_action_mask)
-00000e70: 0a20 2020 2073 7461 7465 203d 2073 7465  .    state = ste
-00000e80: 7028 7374 6174 652c 2061 6374 696f 6e29  p(state, action)
-00000e90: 2020 2320 7374 6174 652e 7265 7761 7264    # state.reward
-00000ea0: 2028 322c 290a 6060 600a 0a50 6778 2069   (2,).```..Pgx i
-00000eb0: 7320 6120 6c69 6272 6172 7920 7468 6174  s a library that
-00000ec0: 2066 6f63 7573 6573 206f 6e20 6661 7374   focuses on fast
-00000ed0: 6572 2069 6d70 6c65 6d65 6e74 6174 696f  er implementatio
-00000ee0: 6e73 2072 6174 6865 7220 7468 616e 206a  ns rather than j
-00000ef0: 7573 7420 7468 6520 4150 4920 6974 7365  ust the API itse
-00000f00: 6c66 2e20 0a48 6f77 6576 6572 2c20 7468  lf. .However, th
-00000f10: 6520 4150 4920 6974 7365 6c66 2069 7320  e API itself is 
-00000f20: 616c 736f 2073 7566 6669 6369 656e 746c  also sufficientl
-00000f30: 7920 6765 6e65 7261 6c2e 2046 6f72 2065  y general. For e
-00000f40: 7861 6d70 6c65 2c20 616c 6c20 656e 7669  xample, all envi
-00000f50: 726f 6e6d 656e 7473 2069 6e20 5067 7820  ronments in Pgx 
-00000f60: 6361 6e20 6265 2063 6f6e 7665 7274 6564  can be converted
-00000f70: 2074 6f20 7468 6520 4145 4320 4150 4920   to the AEC API 
-00000f80: 6f66 205b 5065 7474 696e 675a 6f6f 5d28  of [PettingZoo](
-00000f90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000fa0: 6f6d 2f46 6172 616d 612d 466f 756e 6461  om/Farama-Founda
-00000fb0: 7469 6f6e 2f50 6574 7469 6e67 5a6f 6f29  tion/PettingZoo)
-00000fc0: 2c20 616e 6420 796f 7520 6361 6e20 7275  , and you can ru
-00000fd0: 6e20 5067 7820 656e 7669 726f 6e6d 656e  n Pgx environmen
-00000fe0: 7473 2074 6872 6f75 6768 2074 6865 2050  ts through the P
-00000ff0: 6574 7469 6e67 5a6f 6f20 4150 492e 0a59  ettingZoo API..Y
-00001000: 6f75 2063 616e 2073 6565 2074 6865 2064  ou can see the d
-00001010: 656d 6f6e 7374 7261 7469 6f6e 2069 6e20  emonstration in 
-00001020: 476f 6f67 6c65 2043 6f6c 6162 3a0a 0a3c  Google Colab:..<
-00001030: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001040: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
-00001050: 6f6f 676c 652e 636f 6d2f 6769 7468 7562  oogle.com/github
-00001060: 2f73 6f74 6574 7375 6b2f 7067 782f 626c  /sotetsuk/pgx/bl
-00001070: 6f62 2f6d 6169 6e2f 636f 6c61 622f 7067  ob/main/colab/pg
-00001080: 7832 7065 7474 696e 677a 6f6f 2e69 7079  x2pettingzoo.ipy
-00001090: 6e62 223e 3c69 6d67 2073 7263 3d22 6874  nb"><img src="ht
-000010a0: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
-000010b0: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
-000010c0: 6173 7365 7473 2f63 6f6c 6162 2d62 6164  assets/colab-bad
-000010d0: 6765 2e73 7667 2220 616c 743d 224f 7065  ge.svg" alt="Ope
-000010e0: 6e20 496e 2043 6f6c 6162 222f 3e3c 2f61  n In Colab"/></a
-000010f0: 3e0a 0a3c 212d 2d2d 0a23 2323 204c 696d  >..<!---.### Lim
-00001100: 6974 6174 696f 6e73 2028 666f 7220 7468  itations (for th
-00001110: 6520 7369 6d70 6c69 6369 7479 290a 2a20  e simplicity).* 
-00001120: 446f 6573 202a 2a4e 4f54 2a2a 2073 7570  Does **NOT** sup
-00001130: 706f 7274 2061 6765 6e74 2064 6561 7468  port agent death
-00001140: 2061 6e64 2063 7265 6174 696f 6e2c 2077   and creation, w
-00001150: 6869 6368 2064 796e 6d69 6361 6c6c 7920  hich dynmically 
-00001160: 6368 616e 6765 7320 7468 6520 6172 7261  changes the arra
-00001170: 7920 7369 7a65 2e20 4974 2064 6f65 7320  y size. It does 
-00001180: 6e6f 7420 7765 6c6c 2073 7569 7420 746f  not well suit to
-00001190: 2047 5055 2d61 6363 656c 6572 6174 6564   GPU-accelerated
-000011a0: 2063 6f6d 7075 7461 7469 6f6e 2e0a 2a20   computation..* 
-000011b0: 446f 6573 202a 2a4e 4f54 2a2a 2073 7570  Does **NOT** sup
-000011c0: 706f 7274 2043 6861 6e63 6520 706c 6179  port Chance play
-000011d0: 6572 2028 4e61 7475 7265 2070 6c61 7965  er (Nature playe
-000011e0: 7229 2077 6974 6820 6163 7469 6f6e 2073  r) with action s
-000011f0: 656c 6563 7469 6f6e 2e0a 2a20 446f 6573  election..* Does
-00001200: 202a 2a4e 4f54 2a2a 2073 7570 706f 7274   **NOT** support
-00001210: 204f 7065 6e41 4920 4779 6d20 4150 492e   OpenAI Gym API.
-00001220: 0a20 2020 202a 204f 7065 6e41 4920 4779  .    * OpenAI Gy
-00001230: 6d20 6973 2066 6f72 2073 696e 676c 652d  m is for single-
-00001240: 6167 656e 7420 656e 7669 726f 6e6d 656e  agent environmen
-00001250: 742e 204d 6f73 7420 6f66 2050 6778 2065  t. Most of Pgx e
-00001260: 6e76 6972 6f6e 6d65 6e74 7320 6172 6520  nvironments are 
-00001270: 6d75 6c74 692d 706c 6179 6572 2067 616d  multi-player gam
-00001280: 6573 2e20 4a75 7374 2064 6566 696e 696e  es. Just definin
-00001290: 6720 6f70 706f 6e65 6e74 7320 6973 206e  g opponents is n
-000012a0: 6f74 2065 6e6f 7567 6820 666f 7220 636f  ot enough for co
-000012b0: 6e76 6572 7469 6e67 206d 756c 7469 2d61  nverting multi-a
-000012c0: 6765 6e74 2065 6e76 6972 6f6e 656d 6e74  gent environemnt
-000012d0: 7320 746f 204f 7065 6e41 4920 4779 6d20  s to OpenAI Gym 
-000012e0: 656e 7669 726f 6e6d 656e 742e 2045 2e67  environment. E.g
-000012f0: 2e2c 2069 6e20 7468 6520 6761 6d65 206f  ., in the game o
-00001300: 6620 676f 2c20 7468 6520 6e65 7874 2073  f go, the next s
-00001310: 7461 7465 2073 2720 6973 2064 6566 696e  tate s' is defin
-00001320: 6564 2061 7320 7468 6520 7374 6174 6520  ed as the state 
-00001330: 6a75 7374 2061 6674 6572 2070 6c61 6369  just after placi
-00001340: 6e67 2061 2073 746f 6e65 2069 6e20 416c  ng a stone in Al
-00001350: 6861 476f 2070 6170 6572 2e20 486f 7765  haGo paper. Howe
-00001360: 7665 722c 2073 2720 6265 636f 6d65 7320  ver, s' becomes 
-00001370: 7468 6520 7374 6174 6520 6166 7465 7220  the state after 
-00001380: 7468 6520 6f70 706f 6e65 6e74 7327 2070  the opponents' p
-00001390: 6c61 792e 2054 6869 7320 6368 616e 6765  lay. This change
-000013a0: 7320 7468 6520 6465 6669 6e69 7469 6f6e  s the definition
-000013b0: 206f 6620 5628 7327 292e 0a2a 2044 6f65   of V(s')..* Doe
-000013c0: 7320 2a2a 4e4f 542a 2a20 7375 7070 6f72  s **NOT** suppor
-000013d0: 7420 5065 7474 696e 675a 6f6f 2041 5049  t PettingZoo API
-000013e0: 2e0a 2020 2020 2a20 5065 7474 696e 675a  ..    * PettingZ
-000013f0: 6f6f 2069 7320 2a47 796d 2066 6f72 206d  oo is *Gym for m
-00001400: 756c 7469 2d61 6765 6e74 2052 4c2a 2e20  ulti-agent RL*. 
-00001410: 4173 2066 6172 2061 7320 7765 206b 6e6f  As far as we kno
-00001420: 772c 2050 6574 7469 6e67 5a6f 6f20 646f  w, PettingZoo do
-00001430: 6573 206e 6f74 2073 7570 706f 7274 2076  es not support v
-00001440: 6563 746f 7269 7a65 6420 656e 7669 726f  ectorized enviro
-00001450: 6e6d 656e 7473 2028 6c69 6b65 2056 6563  nments (like Vec
-00001460: 746f 7245 6e76 2069 6e20 4f70 656e 4149  torEnv in OpenAI
-00001470: 2047 796d 292e 2041 7320 5067 7827 7320   Gym). As Pgx's 
-00001480: 6d61 696e 2066 6561 7475 7265 2069 7320  main feature is 
-00001490: 6869 6768 6c79 2076 6563 746f 7269 7a65  highly vectorize
-000014a0: 6420 656e 7669 726f 6e6d 656e 7420 7669  d environment vi
-000014b0: 6120 4750 552f 5450 5520 7375 7070 6f72  a GPU/TPU suppor
-000014c0: 742c 2057 6520 646f 206e 6f74 2063 7572  t, We do not cur
-000014d0: 7265 6e74 6c79 2073 7570 706f 7274 2050  rently support P
-000014e0: 6574 7469 6e67 5a6f 6f20 4150 492e 200a  ettingZoo API. .
-000014f0: 0a23 2323 2060 736b 6970 5f63 6861 6e63  .### `skip_chanc
-00001500: 6560 0a2a 2057 6520 7072 6570 6172 6520  e`.* We prepare 
-00001510: 736b 6970 5f63 6861 6e63 653d 5472 7565  skip_chance=True
-00001520: 206f 7074 696f 6e20 666f 7220 736f 6d65   option for some
-00001530: 2065 6e76 6972 6f6e 6d65 6e74 732e 2054   environments. T
-00001540: 6869 7320 6d61 6b65 7320 6974 2070 6f73  his makes it pos
-00001550: 7369 626c 6520 746f 2063 6f6e 7369 6465  sible to conside
-00001560: 7220 7661 6c75 6520 6675 6e63 7469 6f6e  r value function
-00001570: 2066 6f72 2022 706f 7374 2d64 6563 6973   for "post-decis
-00001580: 696f 6e20 7374 6174 6573 2220 2853 6565  ion states" (See
-00001590: 2041 6c67 6f52 4c20 626f 6f6b 292e 2048   AlgoRL book). H
-000015a0: 6f77 6576 6572 2c20 7765 2064 6f20 6e6f  owever, we do no
-000015b0: 7420 616c 6c6f 7720 6368 616e 6365 2061  t allow chance a
-000015c0: 6765 6e74 2074 6f20 6368 6f6f 7365 2061  gent to choose a
-000015d0: 6374 696f 6e20 6c69 6b65 204f 7065 6e53  ction like OpenS
-000015e0: 7069 656c 2e20 5468 6973 2069 7320 6265  piel. This is be
-000015f0: 6361 7573 6520 7468 6520 6163 7469 6f6e  cause the action
-00001600: 2073 7061 6365 206f 6620 6368 616e 6365   space of chance
-00001610: 2061 6765 6e74 2061 6e64 2075 7375 616c   agent and usual
-00001620: 2061 6765 6e74 2061 7265 2064 6966 6665   agent are diffe
-00001630: 7265 6e74 2e20 5468 7573 2c20 7768 656e  rent. Thus, when
-00001640: 2074 6865 2063 6861 6e63 6520 706c 6179   the chance play
-00001650: 6572 2069 7320 6368 6f73 656e 2028 6063  er is chosen (`c
-00001660: 7572 7265 6e74 5f70 6c61 7965 723d 2d31  urrent_player=-1
-00001670: 6029 2c20 6061 6374 696f 6e3d 2d31 6020  `), `action=-1` 
-00001680: 6d75 7374 2062 6520 7265 7475 726e 6564  must be returned
-00001690: 2074 6f20 7374 6570 2066 756e 6374 696f   to step functio
-000016a0: 6e2e 2055 7365 2060 7368 7566 666c 6560  n. Use `shuffle`
-000016b0: 2074 6f20 6d61 6b65 2060 7374 6570 6020   to make `step` 
-000016c0: 7374 6f63 6861 7374 6963 2e0a 0a23 2323  stochastic...###
-000016d0: 2074 7275 6e63 6174 6174 696f 6e20 616e   truncatation an
-000016e0: 6420 6175 746f 5f72 6573 6574 0a2a 2073  d auto_reset.* s
-000016f0: 7570 706f 7274 6564 2062 7920 606d 616b  upported by `mak
-00001700: 6528 656e 765f 6964 3d22 2e2e 2e22 2c20  e(env_id="...", 
-00001710: 6175 746f 5f72 6573 6574 3d54 7275 652c  auto_reset=True,
-00001720: 206d 6178 5f65 7069 736f 6465 5f6c 656e   max_episode_len
-00001730: 6774 683d 3634 2960 0a2a 2060 6175 746f  gth=64)`.* `auto
-00001740: 5f72 6573 6574 6020 7769 6c6c 2072 6570  _reset` will rep
-00001750: 6c61 6365 2074 6865 2074 6572 6d69 6e61  lace the termina
-00001760: 6c20 7374 6174 6520 6279 2069 6e69 7469  l state by initi
-00001770: 616c 2073 7461 7465 2028 6275 7420 6069  al state (but `i
-00001780: 735f 7465 726d 696e 616c 3d54 7275 6560  s_terminal=True`
-00001790: 2069 7320 7365 7429 0a2a 2060 6973 5f74   is set).* `is_t
-000017a0: 7275 6e63 6174 6564 3d54 7275 6560 2069  runcated=True` i
-000017b0: 7320 616c 736f 2073 6574 2074 6f20 7374  s also set to st
-000017c0: 6174 650a 2d2d 2d3e 0a0a 2323 2053 7570  ate.--->..## Sup
-000017d0: 706f 7274 6564 2067 616d 6573 0a0a 7c20  ported games..| 
-000017e0: 4261 636b 6761 6d6d 6f6e 207c 2043 6865  Backgammon | Che
-000017f0: 7373 207c 2053 686f 6769 207c 2047 6f20  ss | Shogi | Go 
-00001800: 7c0a 7c3a 2d2d 2d3a 7c3a 2d2d 2d3a 7c3a  |.|:---:|:---:|:
-00001810: 2d2d 2d3a 7c3a 2d2d 2d3a 7c0a 7c3c 696d  ---:|:---:|.|<im
-00001820: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00001830: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00001840: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00001850: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-00001860: 6173 7365 7473 2f62 6163 6b67 616d 6d6f  assets/backgammo
-00001870: 6e5f 6461 726b 2e67 6966 2367 682d 6461  n_dark.gif#gh-da
-00001880: 726b 2d6d 6f64 652d 6f6e 6c79 2220 7769  rk-mode-only" wi
-00001890: 6474 683d 2231 3730 7078 223e 3c69 6d67  dth="170px"><img
-000018a0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-000018b0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-000018c0: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
-000018d0: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
-000018e0: 7373 6574 732f 6261 636b 6761 6d6d 6f6e  ssets/backgammon
-000018f0: 5f6c 6967 6874 2e67 6966 2367 682d 6c69  _light.gif#gh-li
-00001900: 6768 742d 6d6f 6465 2d6f 6e6c 7922 2077  ght-mode-only" w
-00001910: 6964 7468 3d22 3137 3070 7822 3e7c 3c69  idth="170px">|<i
-00001920: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00001930: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00001940: 6e74 656e 742e 636f 6d2f 736f 7465 7473  ntent.com/sotets
-00001950: 756b 2f70 6778 2f6d 6169 6e2f 646f 6373  uk/pgx/main/docs
-00001960: 2f61 7373 6574 732f 6368 6573 735f 6461  /assets/chess_da
-00001970: 726b 2e67 6966 2367 682d 6461 726b 2d6d  rk.gif#gh-dark-m
-00001980: 6f64 652d 6f6e 6c79 2220 7769 6474 683d  ode-only" width=
-00001990: 2231 3538 7078 223e 3c69 6d67 2073 7263  "158px"><img src
-000019a0: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-000019b0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-000019c0: 636f 6d2f 736f 7465 7473 756b 2f70 6778  com/sotetsuk/pgx
-000019d0: 2f6d 6169 6e2f 646f 6373 2f61 7373 6574  /main/docs/asset
-000019e0: 732f 6368 6573 735f 6c69 6768 742e 6769  s/chess_light.gi
-000019f0: 6623 6768 2d6c 6967 6874 2d6d 6f64 652d  f#gh-light-mode-
-00001a00: 6f6e 6c79 2220 7769 6474 683d 2231 3538  only" width="158
-00001a10: 7078 223e 7c3c 696d 6720 7372 633d 2268  px">|<img src="h
-00001a20: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00001a30: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00001a40: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-00001a50: 696e 2f64 6f63 732f 6173 7365 7473 2f73  in/docs/assets/s
-00001a60: 686f 6769 5f64 6172 6b2e 6769 6623 6768  hogi_dark.gif#gh
-00001a70: 2d64 6172 6b2d 6d6f 6465 2d6f 6e6c 7922  -dark-mode-only"
-00001a80: 2077 6964 7468 3d22 3137 3070 7822 3e3c   width="170px"><
-00001a90: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00001aa0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00001ab0: 6f6e 7465 6e74 2e63 6f6d 2f73 6f74 6574  ontent.com/sotet
-00001ac0: 7375 6b2f 7067 782f 6d61 696e 2f64 6f63  suk/pgx/main/doc
-00001ad0: 732f 6173 7365 7473 2f73 686f 6769 5f6c  s/assets/shogi_l
-00001ae0: 6967 6874 2e67 6966 2367 682d 6c69 6768  ight.gif#gh-ligh
-00001af0: 742d 6d6f 6465 2d6f 6e6c 7922 2077 6964  t-mode-only" wid
-00001b00: 7468 3d22 3137 3070 7822 3e7c 3c69 6d67  th="170px">|<img
-00001b10: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00001b20: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00001b30: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
-00001b40: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
-00001b50: 7373 6574 732f 676f 2d31 3978 3139 5f64  ssets/go-19x19_d
-00001b60: 6172 6b2e 6769 6623 6768 2d64 6172 6b2d  ark.gif#gh-dark-
-00001b70: 6d6f 6465 2d6f 6e6c 7922 2077 6964 7468  mode-only" width
-00001b80: 3d22 3136 3070 7822 3e3c 696d 6720 7372  ="160px"><img sr
-00001b90: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
-00001ba0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00001bb0: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
-00001bc0: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
-00001bd0: 7473 2f67 6f2d 3139 7831 395f 6c69 6768  ts/go-19x19_ligh
-00001be0: 742e 6769 6623 6768 2d6c 6967 6874 2d6d  t.gif#gh-light-m
-00001bf0: 6f64 652d 6f6e 6c79 2220 7769 6474 683d  ode-only" width=
-00001c00: 2231 3630 7078 223e 7c0a 0a0a 5573 6520  "160px">|...Use 
-00001c10: 6070 6778 2e61 7661 696c 6162 6c65 5f65  `pgx.available_e
-00001c20: 6e76 7328 2920 2d3e 2054 7570 6c65 5b45  nvs() -> Tuple[E
-00001c30: 6e76 4964 5d60 2074 6f20 7365 6520 7468  nvId]` to see th
-00001c40: 6520 6c69 7374 206f 6620 6375 7272 656e  e list of curren
-00001c50: 746c 7920 6176 6169 6c61 626c 6520 6761  tly available ga
-00001c60: 6d65 732e 2047 6976 656e 2061 6e20 603c  mes. Given an `<
-00001c70: 456e 7649 643e 602c 2079 6f75 2063 616e  EnvId>`, you can
-00001c80: 2063 7265 6174 6520 7468 6520 656e 7669   create the envi
-00001c90: 726f 6e6d 656e 7420 7669 610a 0a60 6060  ronment via..```
-00001ca0: 7079 0a3e 3e3e 2065 6e76 203d 2070 6778  py.>>> env = pgx
-00001cb0: 2e6d 616b 6528 3c45 6e76 4964 3e29 0a60  .make(<EnvId>).`
-00001cc0: 6060 0a0a 7c20 4761 6d65 2f45 6e76 4964  ``..| Game/EnvId
-00001cd0: 207c 2056 6973 7561 6c69 7a61 7469 6f6e   | Visualization
-00001ce0: 207c 2056 6572 7369 6f6e 207c 2046 6976   | Version | Fiv
-00001cf0: 652d 776f 7264 2064 6573 6372 6970 7469  e-word descripti
-00001d00: 6f6e 207c 0a7c 3a2d 2d2d 3a7c 3a2d 2d2d  on |.|:---:|:---
-00001d10: 3a7c 3a2d 2d2d 3a7c 3a2d 2d2d 3a7c 0a7c  :|:---:|:---:|.|
-00001d20: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001d30: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-00001d40: 672f 7769 6b69 2f32 3034 385f 2876 6964  g/wiki/2048_(vid
-00001d50: 656f 5f67 616d 6529 223e 3230 3438 3c2f  eo_game)">2048</
-00001d60: 613e 203c 6272 3e20 6022 3230 3438 2260  a> <br> `"2048"`
-00001d70: 207c 3c69 6d67 2073 7263 3d22 6874 7470   |<img src="http
-00001d80: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00001d90: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
-00001da0: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
-00001db0: 646f 6373 2f61 7373 6574 732f 3230 3438  docs/assets/2048
-00001dc0: 5f64 6172 6b2e 6769 6622 2077 6964 7468  _dark.gif" width
-00001dd0: 3d22 3630 7078 223e 3c69 6d67 2073 7263  ="60px"><img src
-00001de0: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00001df0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00001e00: 636f 6d2f 736f 7465 7473 756b 2f70 6778  com/sotetsuk/pgx
-00001e10: 2f6d 6169 6e2f 646f 6373 2f61 7373 6574  /main/docs/asset
-00001e20: 732f 3230 3438 5f6c 6967 6874 2e67 6966  s/2048_light.gif
-00001e30: 2220 7769 6474 683d 2236 3070 7822 3e7c  " width="60px">|
-00001e40: 2060 7630 6020 7c20 2a4d 6572 6765 2074   `v0` | *Merge t
-00001e50: 696c 6573 2074 6f20 6372 6561 7465 2032  iles to create 2
-00001e60: 3034 382e 2a20 7c0a 7c3c 6120 6872 6566  048.* |.|<a href
-00001e70: 3d22 6874 7470 733a 2f2f 656e 2e77 696b  ="https://en.wik
-00001e80: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-00001e90: 4425 4335 2538 4462 7574 7375 5f73 6825  D%C5%8Dbutsu_sh%
-00001ea0: 4335 2538 4467 6922 3e41 6e69 6d61 6c20  C5%8Dgi">Animal 
-00001eb0: 5368 6f67 693c 2f61 3e3c 6272 3e60 2261  Shogi</a><br>`"a
-00001ec0: 6e69 6d61 6c5f 7368 6f67 6922 6020 7c3c  nimal_shogi"` |<
-00001ed0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00001ee0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00001ef0: 6f6e 7465 6e74 2e63 6f6d 2f73 6f74 6574  ontent.com/sotet
-00001f00: 7375 6b2f 7067 782f 6d61 696e 2f64 6f63  suk/pgx/main/doc
-00001f10: 732f 6173 7365 7473 2f61 6e69 6d61 6c5f  s/assets/animal_
-00001f20: 7368 6f67 695f 6461 726b 2e67 6966 2220  shogi_dark.gif" 
-00001f30: 7769 6474 683d 2236 3070 7822 3e3c 696d  width="60px"><im
-00001f40: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00001f50: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00001f60: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00001f70: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-00001f80: 6173 7365 7473 2f61 6e69 6d61 6c5f 7368  assets/animal_sh
-00001f90: 6f67 695f 6c69 6768 742e 6769 6622 2077  ogi_light.gif" w
-00001fa0: 6964 7468 3d22 3630 7078 223e 7c20 2060  idth="60px">|  `
-00001fb0: 7630 6020 7c20 2a41 6e69 6d61 6c2d 7468  v0` | *Animal-th
-00001fc0: 656d 6564 2063 6869 6c64 2d66 7269 656e  emed child-frien
-00001fd0: 646c 7920 7368 6f67 692e 2a20 7c0a 7c3c  dly shogi.* |.|<
-00001fe0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001ff0: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
-00002000: 2f77 696b 692f 4261 636b 6761 6d6d 6f6e  /wiki/Backgammon
-00002010: 223e 4261 636b 6761 6d6d 6f6e 3c2f 613e  ">Backgammon</a>
-00002020: 3c62 723e 6022 6261 636b 6761 6d6d 6f6e  <br>`"backgammon
-00002030: 2260 207c 3c69 6d67 2073 7263 3d22 6874  "` |<img src="ht
-00002040: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00002050: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00002060: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
-00002070: 6e2f 646f 6373 2f61 7373 6574 732f 6261  n/docs/assets/ba
-00002080: 636b 6761 6d6d 6f6e 5f64 6172 6b2e 6769  ckgammon_dark.gi
-00002090: 6622 2077 6964 7468 3d22 3630 7078 223e  f" width="60px">
-000020a0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000020b0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-000020c0: 636f 6e74 656e 742e 636f 6d2f 736f 7465  content.com/sote
-000020d0: 7473 756b 2f70 6778 2f6d 6169 6e2f 646f  tsuk/pgx/main/do
-000020e0: 6373 2f61 7373 6574 732f 6261 636b 6761  cs/assets/backga
-000020f0: 6d6d 6f6e 5f6c 6967 6874 2e67 6966 2220  mmon_light.gif" 
-00002100: 7769 6474 683d 2236 3070 7822 3e7c 2060  width="60px">| `
-00002110: 7630 6020 7c20 2a4c 7563 6b20 6169 6473  v0` | *Luck aids
-00002120: 2062 6561 7269 6e67 206f 6666 2063 6865   bearing off che
-00002130: 636b 6572 732e 2a20 7c0a 7c3c 6120 6872  ckers.* |.|<a hr
-00002140: 6566 3d22 6874 7470 733a 2f2f 656e 2e77  ef="https://en.w
-00002150: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
-00002160: 692f 436f 6e74 7261 6374 5f62 7269 6467  i/Contract_bridg
-00002170: 6522 3e42 7269 6467 6520 6269 6464 696e  e">Bridge biddin
-00002180: 673c 2f61 3e3c 6272 3e60 2262 7269 6467  g</a><br>`"bridg
-00002190: 655f 6269 6464 696e 6722 6020 7c3c 696d  e_bidding"` |<im
-000021a0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-000021b0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-000021c0: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-000021d0: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-000021e0: 6173 7365 7473 2f62 7269 6467 655f 6269  assets/bridge_bi
-000021f0: 6464 696e 675f 6461 726b 2e67 6966 2220  dding_dark.gif" 
-00002200: 7769 6474 683d 2236 3070 7822 3e3c 696d  width="60px"><im
-00002210: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00002220: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00002230: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00002240: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-00002250: 6173 7365 7473 2f62 7269 6467 655f 6269  assets/bridge_bi
-00002260: 6464 696e 675f 6c69 6768 742e 6769 6622  dding_light.gif"
-00002270: 2077 6964 7468 3d22 3630 7078 223e 7c20   width="60px">| 
-00002280: 6076 3060 207c 202a 5061 7274 6e65 7273  `v0` | *Partners
-00002290: 2065 7863 6861 6e67 6520 696e 666f 726d   exchange inform
-000022a0: 6174 696f 6e20 7669 6120 6269 6473 2e2a  ation via bids.*
-000022b0: 207c 0a7c 3c61 2068 7265 663d 2268 7474   |.|<a href="htt
-000022c0: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
-000022d0: 612e 6f72 672f 7769 6b69 2f43 6865 7373  a.org/wiki/Chess
-000022e0: 223e 4368 6573 733c 2f61 3e3c 6272 3e60  ">Chess</a><br>`
-000022f0: 2263 6865 7373 2260 207c 3c69 6d67 2073  "chess"` |<img s
-00002300: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-00002310: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00002320: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
-00002330: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
-00002340: 6574 732f 6368 6573 735f 6461 726b 2e67  ets/chess_dark.g
-00002350: 6966 2220 7769 6474 683d 2236 3070 7822  if" width="60px"
-00002360: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00002370: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00002380: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
-00002390: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
-000023a0: 6f63 732f 6173 7365 7473 2f63 6865 7373  ocs/assets/chess
-000023b0: 5f6c 6967 6874 2e67 6966 2220 7769 6474  _light.gif" widt
-000023c0: 683d 2236 3070 7822 3e7c 2060 7630 6020  h="60px">| `v0` 
-000023d0: 7c20 2a43 6865 636b 6d61 7465 206f 7070  | *Checkmate opp
-000023e0: 6f6e 656e 7427 7320 6b69 6e67 2074 6f20  onent's king to 
-000023f0: 7769 6e2e 2a20 7c0a 7c3c 6120 6872 6566  win.* |.|<a href
-00002400: 3d22 6874 7470 733a 2f2f 656e 2e77 696b  ="https://en.wik
-00002410: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-00002420: 436f 6e6e 6563 745f 466f 7572 223e 436f  Connect_Four">Co
-00002430: 6e6e 6563 7420 466f 7572 3c2f 613e 3c62  nnect Four</a><b
-00002440: 723e 6022 636f 6e6e 6563 745f 666f 7572  r>`"connect_four
-00002450: 2260 207c 3c69 6d67 2073 7263 3d22 6874  "` |<img src="ht
-00002460: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00002470: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00002480: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
-00002490: 6e2f 646f 6373 2f61 7373 6574 732f 636f  n/docs/assets/co
-000024a0: 6e6e 6563 745f 666f 7572 5f64 6172 6b2e  nnect_four_dark.
-000024b0: 6769 6622 2077 6964 7468 3d22 3630 7078  gif" width="60px
-000024c0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-000024d0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-000024e0: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
-000024f0: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
-00002500: 646f 6373 2f61 7373 6574 732f 636f 6e6e  docs/assets/conn
-00002510: 6563 745f 666f 7572 5f6c 6967 6874 2e67  ect_four_light.g
-00002520: 6966 2220 7769 6474 683d 2236 3070 7822  if" width="60px"
-00002530: 3e7c 2060 7630 6020 7c20 2a43 6f6e 6e65  >| `v0` | *Conne
-00002540: 6374 2064 6973 6373 2c20 7769 6e20 7769  ct discs, win wi
-00002550: 7468 2066 6f75 722e 2a20 7c0a 7c3c 6120  th four.* |.|<a 
-00002560: 6872 6566 3d22 6874 7470 733a 2f2f 656e  href="https://en
-00002570: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
-00002580: 696b 692f 4d69 6e69 6368 6573 7322 3e47  iki/Minichess">G
-00002590: 6172 646e 6572 2043 6865 7373 3c2f 613e  ardner Chess</a>
-000025a0: 3c62 723e 6022 6761 7264 6e65 725f 6368  <br>`"gardner_ch
-000025b0: 6573 7322 607c 3c69 6d67 2073 7263 3d22  ess"`|<img src="
-000025c0: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-000025d0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-000025e0: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
-000025f0: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
-00002600: 6761 7264 6e65 725f 6368 6573 735f 6461  gardner_chess_da
-00002610: 726b 2e67 6966 2220 7769 6474 683d 2236  rk.gif" width="6
-00002620: 3070 7822 3e3c 696d 6720 7372 633d 2268  0px"><img src="h
-00002630: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00002640: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00002650: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-00002660: 696e 2f64 6f63 732f 6173 7365 7473 2f67  in/docs/assets/g
-00002670: 6172 646e 6572 5f63 6865 7373 5f6c 6967  ardner_chess_lig
-00002680: 6874 2e67 6966 2220 7769 6474 683d 2236  ht.gif" width="6
-00002690: 3070 7822 3e7c 2060 7630 6020 7c20 2a35  0px">| `v0` | *5
-000026a0: 7835 2063 6865 7373 2076 6172 6961 6e74  x5 chess variant
-000026b0: 2c20 6578 636c 7564 696e 6720 6361 7374  , excluding cast
-000026c0: 6c69 6e67 2e2a 207c 0a7c 3c61 2068 7265  ling.* |.|<a hre
-000026d0: 663d 2268 7474 7073 3a2f 2f65 6e2e 7769  f="https://en.wi
-000026e0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
-000026f0: 2f47 6f5f 2867 616d 6529 223e 476f 3c2f  /Go_(game)">Go</
-00002700: 613e 3c62 723e 6022 676f 5f39 7839 2260  a><br>`"go_9x9"`
-00002710: 2060 2267 6f5f 3139 7831 3922 6020 7c3c   `"go_19x19"` |<
-00002720: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00002730: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00002740: 6f6e 7465 6e74 2e63 6f6d 2f73 6f74 6574  ontent.com/sotet
-00002750: 7375 6b2f 7067 782f 6d61 696e 2f64 6f63  suk/pgx/main/doc
-00002760: 732f 6173 7365 7473 2f67 6f2d 3139 7831  s/assets/go-19x1
-00002770: 395f 6461 726b 2e67 6966 2220 7769 6474  9_dark.gif" widt
-00002780: 683d 2236 3070 7822 3e3c 696d 6720 7372  h="60px"><img sr
-00002790: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
-000027a0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-000027b0: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
-000027c0: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
-000027d0: 7473 2f67 6f2d 3139 7831 395f 6c69 6768  ts/go-19x19_ligh
-000027e0: 742e 6769 6622 2077 6964 7468 3d22 3630  t.gif" width="60
-000027f0: 7078 223e 7c20 6076 3060 207c 202a 5374  px">| `v0` | *St
-00002800: 7261 7465 6769 6361 6c6c 7920 706c 6163  rategically plac
-00002810: 6520 7374 6f6e 6573 2c20 636c 6169 6d20  e stones, claim 
-00002820: 7465 7272 6974 6f72 792e 2a20 7c0a 7c3c  territory.* |.|<
-00002830: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00002840: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
-00002850: 2f77 696b 692f 4865 785f 2862 6f61 7264  /wiki/Hex_(board
-00002860: 5f67 616d 6529 223e 4865 783c 2f61 3e3c  _game)">Hex</a><
-00002870: 6272 3e60 2268 6578 2260 207c 3c69 6d67  br>`"hex"` |<img
-00002880: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00002890: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-000028a0: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
-000028b0: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
-000028c0: 7373 6574 732f 6865 785f 6461 726b 2e67  ssets/hex_dark.g
-000028d0: 6966 2220 7769 6474 683d 2236 3070 7822  if" width="60px"
-000028e0: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-000028f0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00002900: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
-00002910: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
-00002920: 6f63 732f 6173 7365 7473 2f68 6578 5f6c  ocs/assets/hex_l
-00002930: 6967 6874 2e67 6966 2220 7769 6474 683d  ight.gif" width=
-00002940: 2236 3070 7822 3e7c 2060 7630 6020 7c20  "60px">| `v0` | 
-00002950: 2a43 6f6e 6e65 6374 206f 7070 6f73 6974  *Connect opposit
-00002960: 6520 7369 6465 732c 2062 6c6f 636b 206f  e sides, block o
-00002970: 7070 6f6e 656e 742e 2a20 7c0a 7c3c 6120  pponent.* |.|<a 
-00002980: 6872 6566 3d22 6874 7470 733a 2f2f 656e  href="https://en
-00002990: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
-000029a0: 696b 692f 4b75 686e 5f70 6f6b 6572 223e  iki/Kuhn_poker">
-000029b0: 4b75 686e 2050 6f6b 6572 3c2f 613e 3c62  Kuhn Poker</a><b
-000029c0: 723e 6022 6b75 686e 5f70 6f6b 6572 2260  r>`"kuhn_poker"`
-000029d0: 207c 3c69 6d67 2073 7263 3d22 6874 7470   |<img src="http
-000029e0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-000029f0: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
-00002a00: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
-00002a10: 646f 6373 2f61 7373 6574 732f 6b75 686e  docs/assets/kuhn
-00002a20: 5f70 6f6b 6572 5f64 6172 6b2e 6769 6622  _poker_dark.gif"
-00002a30: 2077 6964 7468 3d22 3630 7078 223e 3c69   width="60px"><i
-00002a40: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00002a50: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00002a60: 6e74 656e 742e 636f 6d2f 736f 7465 7473  ntent.com/sotets
-00002a70: 756b 2f70 6778 2f6d 6169 6e2f 646f 6373  uk/pgx/main/docs
-00002a80: 2f61 7373 6574 732f 6b75 686e 5f70 6f6b  /assets/kuhn_pok
-00002a90: 6572 5f6c 6967 6874 2e67 6966 2220 7769  er_light.gif" wi
-00002aa0: 6474 683d 2236 3070 7822 3e7c 2060 7630  dth="60px">| `v0
-00002ab0: 6020 7c20 2a54 6872 6565 2d63 6172 6420  ` | *Three-card 
-00002ac0: 6265 7474 696e 6720 616e 6420 626c 7566  betting and bluf
-00002ad0: 6669 6e67 2067 616d 652e 2a20 7c0a 7c3c  fing game.* |.|<
-00002ae0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00002af0: 6172 7869 762e 6f72 672f 6162 732f 3132  arxiv.org/abs/12
-00002b00: 3037 2e31 3431 3122 3e4c 6564 7563 2068  07.1411">Leduc h
-00002b10: 6f6c 6427 656d 3c2f 613e 3c62 723e 6022  old'em</a><br>`"
-00002b20: 6c65 6475 635f 686f 6c64 656d 2260 207c  leduc_holdem"` |
-00002b30: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00002b40: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00002b50: 636f 6e74 656e 742e 636f 6d2f 736f 7465  content.com/sote
-00002b60: 7473 756b 2f70 6778 2f6d 6169 6e2f 646f  tsuk/pgx/main/do
-00002b70: 6373 2f61 7373 6574 732f 6c65 6475 635f  cs/assets/leduc_
-00002b80: 686f 6c64 656d 5f64 6172 6b2e 6769 6622  holdem_dark.gif"
-00002b90: 2077 6964 7468 3d22 3630 7078 223e 3c69   width="60px"><i
-00002ba0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00002bb0: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00002bc0: 6e74 656e 742e 636f 6d2f 736f 7465 7473  ntent.com/sotets
-00002bd0: 756b 2f70 6778 2f6d 6169 6e2f 646f 6373  uk/pgx/main/docs
-00002be0: 2f61 7373 6574 732f 6c65 6475 635f 686f  /assets/leduc_ho
-00002bf0: 6c64 656d 5f6c 6967 6874 2e67 6966 2220  ldem_light.gif" 
-00002c00: 7769 6474 683d 2236 3070 7822 3e7c 2060  width="60px">| `
-00002c10: 7630 6020 7c20 2a54 776f 2d73 7569 742c  v0` | *Two-suit,
-00002c20: 206c 696d 6974 6564 2064 6563 6b20 706f   limited deck po
-00002c30: 6b65 722e 2a20 7c0a 7c3c 6120 6872 6566  ker.* |.|<a href
-00002c40: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00002c50: 2e63 6f6d 2f6b 656e 6a79 6f75 6e67 2f4d  .com/kenjyoung/M
-00002c60: 696e 4174 6172 223e 4d69 6e41 7461 722f  inAtar">MinAtar/
-00002c70: 4173 7465 7269 783c 2f61 3e3c 6272 3e60  Asterix</a><br>`
-00002c80: 226d 696e 6174 6172 2d61 7374 6572 6978  "minatar-asterix
-00002c90: 2260 207c 3c69 6d67 2073 7263 3d22 6874  "` |<img src="ht
-00002ca0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00002cb0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00002cc0: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
-00002cd0: 6e2f 646f 6373 2f61 7373 6574 732f 6d69  n/docs/assets/mi
-00002ce0: 6e61 7461 722d 6173 7465 7269 782e 6769  natar-asterix.gi
-00002cf0: 6622 2077 6964 7468 3d22 3530 7078 223e  f" width="50px">
-00002d00: 7c20 6076 3060 207c 202a 4176 6f69 6420  | `v0` | *Avoid 
-00002d10: 656e 656d 6965 732c 2063 6f6c 6c65 6374  enemies, collect
-00002d20: 2074 7265 6173 7572 652c 2073 7572 7669   treasure, survi
-00002d30: 7665 2e2a 207c 0a7c 3c61 2068 7265 663d  ve.* |.|<a href=
-00002d40: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00002d50: 636f 6d2f 6b65 6e6a 796f 756e 672f 4d69  com/kenjyoung/Mi
-00002d60: 6e41 7461 7222 3e4d 696e 4174 6172 2f42  nAtar">MinAtar/B
-00002d70: 7265 616b 6f75 743c 2f61 3e3c 6272 3e60  reakout</a><br>`
-00002d80: 226d 696e 6174 6172 2d62 7265 616b 6f75  "minatar-breakou
-00002d90: 7422 6020 7c3c 696d 6720 7372 633d 2268  t"` |<img src="h
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7067 780a  : 2.1.Name: pgx.
+00000020: 5665 7273 696f 6e3a 2031 2e31 2e30 0a53  Version: 1.1.0.S
+00000030: 756d 6d61 7279 3a20 4750 552f 5450 552d  ummary: GPU/TPU-
+00000040: 6163 6365 6c65 7261 7465 6420 7061 7261  accelerated para
+00000050: 6c6c 656c 2067 616d 6520 7369 6d75 6c61  llel game simula
+00000060: 746f 7273 2066 6f72 2072 6569 6e66 6f72  tors for reinfor
+00000070: 6365 6d65 6e74 206c 6561 726e 696e 6720  cement learning 
+00000080: 2852 4c29 0a48 6f6d 652d 7061 6765 3a20  (RL).Home-page: 
+00000090: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000000a0: 6f6d 2f73 6f74 6574 7375 6b2f 7067 780a  om/sotetsuk/pgx.
+000000b0: 4175 7468 6f72 3a20 536f 7465 7473 7520  Author: Sotetsu 
+000000c0: 4b4f 5941 4d41 4441 0a41 7574 686f 722d  KOYAMADA.Author-
+000000d0: 656d 6169 6c3a 2073 6f74 6574 7375 2e6b  email: sotetsu.k
+000000e0: 6f79 616d 6164 6140 676d 6169 6c2e 636f  oyamada@gmail.co
+000000f0: 6d0a 436c 6173 7369 6669 6572 3a20 5072  m.Classifier: Pr
+00000100: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000110: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000120: 332e 380a 436c 6173 7369 6669 6572 3a20  3.8.Classifier: 
+00000130: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000140: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000150: 3a20 332e 390a 436c 6173 7369 6669 6572  : 3.9.Classifier
+00000160: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000170: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000180: 203a 3a20 332e 3130 0a44 6573 6372 6970   :: 3.10.Descrip
+00000190: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+000001a0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+000001b0: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
+000001c0: 4943 454e 5345 0a0a 5b21 5b63 695d 2868  ICENSE..[![ci](h
+000001d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001e0: 6d2f 736f 7465 7473 756b 2f70 6778 2f61  m/sotetsuk/pgx/a
+000001f0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000200: 2f63 692e 796d 6c2f 6261 6467 652e 7376  /ci.yml/badge.sv
+00000210: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
+00000220: 7562 2e63 6f6d 2f73 6f74 6574 7375 6b2f  ub.com/sotetsuk/
+00000230: 7067 782f 6163 7469 6f6e 732f 776f 726b  pgx/actions/work
+00000240: 666c 6f77 732f 6369 2e79 6d6c 290a 0a0a  flows/ci.yml)...
+00000250: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000260: 6572 223e 0a3c 696d 6720 7372 633d 2268  er">.<img src="h
+00000270: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000280: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000290: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
+000002a0: 696e 2f64 6f63 732f 6173 7365 7473 2f6c  in/docs/assets/l
+000002b0: 6f67 6f2e 7376 6722 2077 6964 7468 3d22  ogo.svg" width="
+000002c0: 3430 2522 3e0a 3c2f 6469 763e 0a0a 4120  40%">.</div>..A 
+000002d0: 636f 6c6c 6563 7469 6f6e 206f 6620 4750  collection of GP
+000002e0: 552f 5450 552d 6163 6365 6c65 7261 7465  U/TPU-accelerate
+000002f0: 6420 7061 7261 6c6c 656c 2067 616d 6520  d parallel game 
+00000300: 7369 6d75 6c61 746f 7273 2066 6f72 2072  simulators for r
+00000310: 6569 6e66 6f72 6365 6d65 6e74 206c 6561  einforcement lea
+00000320: 726e 696e 6720 2852 4c29 0a0a 3c64 6976  rning (RL)..<div
+00000330: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000340: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
+00000350: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000360: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
+00000370: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
+00000380: 6f63 732f 6173 7365 7473 2f67 6f5f 6461  ocs/assets/go_da
+00000390: 726b 2e67 6966 2367 682d 6461 726b 2d6d  rk.gif#gh-dark-m
+000003a0: 6f64 652d 6f6e 6c79 2220 7769 6474 683d  ode-only" width=
+000003b0: 2233 3025 223e 3c69 6d67 2073 7263 3d22  "30%"><img src="
+000003c0: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+000003d0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+000003e0: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
+000003f0: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
+00000400: 676f 5f64 6172 6b2e 6769 6623 6768 2d64  go_dark.gif#gh-d
+00000410: 6172 6b2d 6d6f 6465 2d6f 6e6c 7922 2077  ark-mode-only" w
+00000420: 6964 7468 3d22 3330 2522 2073 7479 6c65  idth="30%" style
+00000430: 3d22 7472 616e 7366 6f72 6d3a 726f 7461  ="transform:rota
+00000440: 7465 2832 3730 6465 6729 3b22 3e3c 696d  te(270deg);"><im
+00000450: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+00000460: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00000470: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
+00000480: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
+00000490: 6173 7365 7473 2f67 6f5f 6461 726b 2e67  assets/go_dark.g
+000004a0: 6966 2367 682d 6461 726b 2d6d 6f64 652d  if#gh-dark-mode-
+000004b0: 6f6e 6c79 2220 7769 6474 683d 2233 3025  only" width="30%
+000004c0: 2220 7374 796c 653d 2274 7261 6e73 666f  " style="transfo
+000004d0: 726d 3a72 6f74 6174 6528 3930 6465 6729  rm:rotate(90deg)
+000004e0: 3b22 3e0a 3c69 6d67 2073 7263 3d22 6874  ;">.<img src="ht
+000004f0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000500: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000510: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
+00000520: 6e2f 646f 6373 2f61 7373 6574 732f 676f  n/docs/assets/go
+00000530: 5f6c 6967 6874 2e67 6966 2367 682d 6c69  _light.gif#gh-li
+00000540: 6768 742d 6d6f 6465 2d6f 6e6c 7922 2077  ght-mode-only" w
+00000550: 6964 7468 3d22 3330 2522 3e3c 696d 6720  idth="30%"><img 
+00000560: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00000570: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000580: 6e74 2e63 6f6d 2f73 6f74 6574 7375 6b2f  nt.com/sotetsuk/
+00000590: 7067 782f 6d61 696e 2f64 6f63 732f 6173  pgx/main/docs/as
+000005a0: 7365 7473 2f67 6f5f 6c69 6768 742e 6769  sets/go_light.gi
+000005b0: 6623 6768 2d6c 6967 6874 2d6d 6f64 652d  f#gh-light-mode-
+000005c0: 6f6e 6c79 2220 7769 6474 683d 2233 3025  only" width="30%
+000005d0: 2220 7374 796c 653d 2274 7261 6e73 666f  " style="transfo
+000005e0: 726d 3a72 6f74 6174 6528 3237 3064 6567  rm:rotate(270deg
+000005f0: 293b 223e 3c69 6d67 2073 7263 3d22 6874  );"><img src="ht
+00000600: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000610: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000620: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
+00000630: 6e2f 646f 6373 2f61 7373 6574 732f 676f  n/docs/assets/go
+00000640: 5f6c 6967 6874 2e67 6966 2367 682d 6c69  _light.gif#gh-li
+00000650: 6768 742d 6d6f 6465 2d6f 6e6c 7922 2077  ght-mode-only" w
+00000660: 6964 7468 3d22 3330 2522 2073 7479 6c65  idth="30%" style
+00000670: 3d22 7472 616e 7366 6f72 6d3a 726f 7461  ="transform:rota
+00000680: 7465 2839 3064 6567 293b 223e 0a3c 2f64  te(90deg);">.</d
+00000690: 6976 3e0a 0af0 9f8e 8920 2a2a 6076 312e  iv>...... **`v1.
+000006a0: 302e 3060 2a2a 2069 7320 7265 6c65 6173  0.0`** is releas
+000006b0: 6564 2120 2832 3032 332e 362e 3230 290a  ed! (2023.6.20).
+000006c0: 0a23 2320 5768 7920 5067 783f 0a0a 3c21  .## Why Pgx?..<!
+000006d0: 2d2d 2d20 0a74 6872 6f75 6768 7075 743a  --- .throughput:
+000006e0: 2068 7474 7073 3a2f 2f63 6f6c 6162 2e72   https://colab.r
+000006f0: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+00000700: 6f6d 2f64 7269 7665 2f31 6749 5748 594c  om/drive/1gIWHYL
+00000710: 4b42 7845 3258 4b44 6841 6c45 594b 5665  KBxE2XKDhAlEYKVe
+00000720: 637a 3357 4734 637a 647a 2373 6372 6f6c  cz3WG4czdz#scrol
+00000730: 6c54 6f3d 5631 515a 6852 586f 474c 384b  lTo=V1QZhRXoGL8K
+00000740: 0a2d 2d2d 3e0a 0a5b 4272 6178 5d28 6874  .--->..[Brax](ht
+00000750: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000760: 2f67 6f6f 676c 652f 6272 6178 292c 2061  /google/brax), a
+00000770: 205b 4a41 585d 2868 7474 7073 3a2f 2f67   [JAX](https://g
+00000780: 6974 6875 622e 636f 6d2f 676f 6f67 6c65  ithub.com/google
+00000790: 2f6a 6178 292d 6e61 7469 7665 2070 6879  /jax)-native phy
+000007a0: 7369 6373 2065 6e67 696e 652c 2070 726f  sics engine, pro
+000007b0: 7669 6465 7320 6578 7472 656d 656c 7920  vides extremely 
+000007c0: 6869 6768 2d73 7065 6564 2070 6172 616c  high-speed paral
+000007d0: 6c65 6c20 7369 6d75 6c61 7469 6f6e 2066  lel simulation f
+000007e0: 6f72 2052 4c20 696e 202a 636f 6e74 696e  or RL in *contin
+000007f0: 756f 7573 2a20 7374 6174 6520 7370 6163  uous* state spac
+00000800: 652e 0a54 6865 6e2c 2077 6861 7420 6162  e..Then, what ab
+00000810: 6f75 7420 524c 2069 6e20 2a64 6973 6372  out RL in *discr
+00000820: 6574 652a 2073 7461 7465 2073 7061 6365  ete* state space
+00000830: 7320 6c69 6b65 2043 6865 7373 2c20 5368  s like Chess, Sh
+00000840: 6f67 692c 2061 6e64 2047 6f3f 202a 2a50  ogi, and Go? **P
+00000850: 6778 2a2a 2070 726f 7669 6465 7320 6120  gx** provides a 
+00000860: 7769 6465 2076 6172 6965 7479 206f 6620  wide variety of 
+00000870: 4a41 582d 6e61 7469 7665 2067 616d 6520  JAX-native game 
+00000880: 7369 6d75 6c61 746f 7273 2120 4869 6768  simulators! High
+00000890: 6c69 6768 7465 6420 6665 6174 7572 6573  lighted features
+000008a0: 2069 6e63 6c75 6465 3a0a 0a2d 20e2 9aa1   include:..- ...
+000008b0: 202a 2a53 7570 6572 2066 6173 742a 2a20   **Super fast** 
+000008c0: 696e 2070 6172 616c 6c65 6c20 6578 6563  in parallel exec
+000008d0: 7574 696f 6e20 6f6e 2061 6363 656c 6572  ution on acceler
+000008e0: 6174 6f72 730a 2d20 f09f 8eb2 202a 2a56  ators.- .... **V
+000008f0: 6172 696f 7573 2067 616d 6520 7375 7070  arious game supp
+00000900: 6f72 742a 2a20 696e 636c 7564 696e 6720  ort** including 
+00000910: 2a2a 4261 636b 6761 6d6d 6f6e 2a2a 2c20  **Backgammon**, 
+00000920: 2a2a 4368 6573 732a 2a2c 202a 2a53 686f  **Chess**, **Sho
+00000930: 6769 2a2a 2c20 616e 6420 2a2a 476f 2a2a  gi**, and **Go**
+00000940: 0a2d 20f0 9f96 bcef b88f 202a 2a42 6561  .- ....... **Bea
+00000950: 7574 6966 756c 2076 6973 7561 6c69 7a61  utiful visualiza
+00000960: 7469 6f6e 2a2a 2069 6e20 5356 4720 666f  tion** in SVG fo
+00000970: 726d 6174 0a0a 0a23 2320 5175 6963 6b20  rmat...## Quick 
+00000980: 7374 6172 740a 0a2d 205b 4765 7474 696e  start..- [Gettin
+00000990: 6720 7374 6172 7465 645d 2868 7474 7073  g started](https
+000009a0: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
+000009b0: 682e 676f 6f67 6c65 2e63 6f6d 2f67 6974  h.google.com/git
+000009c0: 6875 622f 736f 7465 7473 756b 2f70 6778  hub/sotetsuk/pgx
+000009d0: 2f62 6c6f 622f 6d61 696e 2f63 6f6c 6162  /blob/main/colab
+000009e0: 2f70 6778 5f68 656c 6c6f 5f77 6f72 6c64  /pgx_hello_world
+000009f0: 2e69 7079 6e62 290a 2d20 5b50 6778 2062  .ipynb).- [Pgx b
+00000a00: 6173 656c 696e 6520 6d6f 6465 6c73 5d28  aseline models](
+00000a10: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
+00000a20: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
+00000a30: 6d2f 6769 7468 7562 2f73 6f74 6574 7375  m/github/sotetsu
+00000a40: 6b2f 7067 782f 626c 6f62 2f6d 6169 6e2f  k/pgx/blob/main/
+00000a50: 636f 6c61 622f 6261 7365 6c69 6e65 732e  colab/baselines.
+00000a60: 6970 796e 6229 0a2d 205b 5050 4f20 6578  ipynb).- [PPO ex
+00000a70: 616d 706c 655d 2868 7474 7073 3a2f 2f63  ample](https://c
+00000a80: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00000a90: 6f67 6c65 2e63 6f6d 2f67 6974 6875 622f  ogle.com/github/
+00000aa0: 736f 7465 7473 756b 2f70 6778 2f62 6c6f  sotetsuk/pgx/blo
+00000ab0: 622f 6d61 696e 2f63 6f6c 6162 2f70 706f  b/main/colab/ppo
+00000ac0: 2e69 7079 6e62 290a 2d20 5b45 7870 6f72  .ipynb).- [Expor
+00000ad0: 7420 746f 2050 6574 7469 6e67 5a6f 6f20  t to PettingZoo 
+00000ae0: 4150 495d 2868 7474 7073 3a2f 2f63 6f6c  API](https://col
+00000af0: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
+00000b00: 6c65 2e63 6f6d 2f67 6974 6875 622f 736f  le.com/github/so
+00000b10: 7465 7473 756b 2f70 6778 2f62 6c6f 622f  tetsuk/pgx/blob/
+00000b20: 6d61 696e 2f63 6f6c 6162 2f70 6778 3270  main/colab/pgx2p
+00000b30: 6574 7469 6e67 7a6f 6f2e 6970 796e 6229  ettingzoo.ipynb)
+00000b40: 0a0a 2323 2055 7361 6765 0a0a 5468 6520  ..## Usage..The 
+00000b50: 666f 6c6c 6f77 696e 6720 636f 6465 2073  following code s
+00000b60: 6e69 7070 6574 2073 686f 7773 2061 2073  nippet shows a s
+00000b70: 696d 706c 6520 6578 616d 706c 6520 6f66  imple example of
+00000b80: 2075 7369 6e67 2050 6778 2e0a 596f 7520   using Pgx..You 
+00000b90: 6361 6e20 7472 7920 6974 206f 7574 2069  can try it out i
+00000ba0: 6e20 5b74 6869 7320 436f 6c61 625d 2868  n [this Colab](h
+00000bb0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
+00000bc0: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
+00000bd0: 2f67 6974 6875 622f 736f 7465 7473 756b  /github/sotetsuk
+00000be0: 2f70 6778 2f62 6c6f 622f 6d61 696e 2f63  /pgx/blob/main/c
+00000bf0: 6f6c 6162 2f70 6778 5f68 656c 6c6f 5f77  olab/pgx_hello_w
+00000c00: 6f72 6c64 2e69 7079 6e62 292e 0a4e 6f74  orld.ipynb)..Not
+00000c10: 6520 7468 6174 2061 6c6c 2060 7374 6570  e that all `step
+00000c20: 6020 6675 6e63 7469 6f6e 7320 696e 2050  ` functions in P
+00000c30: 6778 2065 6e76 6972 6f6e 6d65 6e74 7320  gx environments 
+00000c40: 6172 6520 2a2a 4a41 582d 6e61 7469 7665  are **JAX-native
+00000c50: 2e2a 2a2c 2069 2e65 2e2c 2074 6865 7920  .**, i.e., they 
+00000c60: 6172 6520 616c 6c20 2a4a 4954 2d61 626c  are all *JIT-abl
+00000c70: 652a 2e0a 506c 6561 7365 2072 6566 6572  e*..Please refer
+00000c80: 2074 6f20 7468 6520 5b64 6f63 756d 656e   to the [documen
+00000c90: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+00000ca0: 736f 7465 7473 756b 2e67 6974 6875 622e  sotetsuk.github.
+00000cb0: 696f 2f70 6778 2920 666f 7220 6d6f 7265  io/pgx) for more
+00000cc0: 2064 6574 6169 6c73 2e0a 0a60 6060 7079   details...```py
+00000cd0: 0a69 6d70 6f72 7420 6a61 780a 696d 706f  .import jax.impo
+00000ce0: 7274 2070 6778 0a0a 656e 7620 3d20 7067  rt pgx..env = pg
+00000cf0: 782e 6d61 6b65 2822 676f 5f31 3978 3139  x.make("go_19x19
+00000d00: 2229 0a69 6e69 7420 3d20 6a61 782e 6a69  ").init = jax.ji
+00000d10: 7428 6a61 782e 766d 6170 2865 6e76 2e69  t(jax.vmap(env.i
+00000d20: 6e69 7429 290a 7374 6570 203d 206a 6178  nit)).step = jax
+00000d30: 2e6a 6974 286a 6178 2e76 6d61 7028 656e  .jit(jax.vmap(en
+00000d40: 762e 7374 6570 2929 0a0a 6261 7463 685f  v.step))..batch_
+00000d50: 7369 7a65 203d 2031 3032 340a 6b65 7973  size = 1024.keys
+00000d60: 203d 206a 6178 2e72 616e 646f 6d2e 7370   = jax.random.sp
+00000d70: 6c69 7428 6a61 782e 7261 6e64 6f6d 2e50  lit(jax.random.P
+00000d80: 524e 474b 6579 2834 3229 2c20 6261 7463  RNGKey(42), batc
+00000d90: 685f 7369 7a65 290a 7374 6174 6520 3d20  h_size).state = 
+00000da0: 696e 6974 286b 6579 7329 2020 2320 7665  init(keys)  # ve
+00000db0: 6374 6f72 697a 6564 2073 7461 7465 730a  ctorized states.
+00000dc0: 7768 696c 6520 6e6f 7420 2873 7461 7465  while not (state
+00000dd0: 2e74 6572 6d69 6e61 7465 6420 7c20 7374  .terminated | st
+00000de0: 6174 652e 7472 756e 6361 7465 6429 2e61  ate.truncated).a
+00000df0: 6c6c 2829 3a0a 2020 2020 6163 7469 6f6e  ll():.    action
+00000e00: 203d 206d 6f64 656c 2873 7461 7465 2e63   = model(state.c
+00000e10: 7572 7265 6e74 5f70 6c61 7965 722c 2073  urrent_player, s
+00000e20: 7461 7465 2e6f 6273 6572 7661 7469 6f6e  tate.observation
+00000e30: 2c20 7374 6174 652e 6c65 6761 6c5f 6163  , state.legal_ac
+00000e40: 7469 6f6e 5f6d 6173 6b29 0a20 2020 2073  tion_mask).    s
+00000e50: 7461 7465 203d 2073 7465 7028 7374 6174  tate = step(stat
+00000e60: 652c 2061 6374 696f 6e29 2020 2320 7374  e, action)  # st
+00000e70: 6174 652e 7265 7761 7264 2028 322c 290a  ate.reward (2,).
+00000e80: 6060 600a 0a50 6778 2069 7320 6120 6c69  ```..Pgx is a li
+00000e90: 6272 6172 7920 7468 6174 2066 6f63 7573  brary that focus
+00000ea0: 6573 206f 6e20 6661 7374 6572 2069 6d70  es on faster imp
+00000eb0: 6c65 6d65 6e74 6174 696f 6e73 2072 6174  lementations rat
+00000ec0: 6865 7220 7468 616e 206a 7573 7420 7468  her than just th
+00000ed0: 6520 4150 4920 6974 7365 6c66 2e20 0a48  e API itself. .H
+00000ee0: 6f77 6576 6572 2c20 7468 6520 4150 4920  owever, the API 
+00000ef0: 6974 7365 6c66 2069 7320 616c 736f 2073  itself is also s
+00000f00: 7566 6669 6369 656e 746c 7920 6765 6e65  ufficiently gene
+00000f10: 7261 6c2e 2046 6f72 2065 7861 6d70 6c65  ral. For example
+00000f20: 2c20 616c 6c20 656e 7669 726f 6e6d 656e  , all environmen
+00000f30: 7473 2069 6e20 5067 7820 6361 6e20 6265  ts in Pgx can be
+00000f40: 2063 6f6e 7665 7274 6564 2074 6f20 7468   converted to th
+00000f50: 6520 4145 4320 4150 4920 6f66 205b 5065  e AEC API of [Pe
+00000f60: 7474 696e 675a 6f6f 5d28 6874 7470 733a  ttingZoo](https:
+00000f70: 2f2f 6769 7468 7562 2e63 6f6d 2f46 6172  //github.com/Far
+00000f80: 616d 612d 466f 756e 6461 7469 6f6e 2f50  ama-Foundation/P
+00000f90: 6574 7469 6e67 5a6f 6f29 2c20 616e 6420  ettingZoo), and 
+00000fa0: 796f 7520 6361 6e20 7275 6e20 5067 7820  you can run Pgx 
+00000fb0: 656e 7669 726f 6e6d 656e 7473 2074 6872  environments thr
+00000fc0: 6f75 6768 2074 6865 2050 6574 7469 6e67  ough the Petting
+00000fd0: 5a6f 6f20 4150 492e 0a59 6f75 2063 616e  Zoo API..You can
+00000fe0: 2073 6565 2074 6865 2064 656d 6f6e 7374   see the demonst
+00000ff0: 7261 7469 6f6e 2069 6e20 5b74 6869 7320  ration in [this 
+00001000: 436f 6c61 625d 2868 7474 7073 3a2f 2f63  Colab](https://c
+00001010: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00001020: 6f67 6c65 2e63 6f6d 2f67 6974 6875 622f  ogle.com/github/
+00001030: 736f 7465 7473 756b 2f70 6778 2f62 6c6f  sotetsuk/pgx/blo
+00001040: 622f 6d61 696e 2f63 6f6c 6162 2f70 6778  b/main/colab/pgx
+00001050: 3270 6574 7469 6e67 7a6f 6f2e 6970 796e  2pettingzoo.ipyn
+00001060: 6229 2e0a 0a0a 2323 2049 6e73 7461 6c6c  b)....## Install
+00001070: 6174 696f 6e0a 0a60 6060 7368 0a70 6970  ation..```sh.pip
+00001080: 2069 6e73 7461 6c6c 2070 6778 0a60 6060   install pgx.```
+00001090: 0a0a 4e6f 7465 2074 6861 7420 7468 6520  ..Note that the 
+000010a0: 5b4d 696e 4174 6172 5d28 6874 7470 733a  [MinAtar](https:
+000010b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 656e  //github.com/ken
+000010c0: 6a79 6f75 6e67 2f4d 696e 4174 6172 2920  jyoung/MinAtar) 
+000010d0: 7375 6974 6520 6973 2070 726f 7669 6465  suite is provide
+000010e0: 6420 6173 2061 2073 6570 6172 6174 6520  d as a separate 
+000010f0: 6578 7465 6e73 696f 6e20 666f 7220 5067  extension for Pg
+00001100: 7820 285b 6070 6778 2d6d 696e 6174 6172  x ([`pgx-minatar
+00001110: 605d 2868 7474 7073 3a2f 2f67 6974 6875  `](https://githu
+00001120: 622e 636f 6d2f 736f 7465 7473 756b 2f70  b.com/sotetsuk/p
+00001130: 6778 2d6d 696e 6174 6172 2929 2e20 5468  gx-minatar)). Th
+00001140: 6572 6566 6f72 652c 2070 6c65 6173 6520  erefore, please 
+00001150: 7275 6e20 7468 6520 666f 6c6c 6f77 696e  run the followin
+00001160: 6720 636f 6d6d 616e 6420 6164 6469 7469  g command additi
+00001170: 6f6e 616c 7920 746f 2075 7365 2074 6865  onaly to use the
+00001180: 204d 696e 4174 6172 2073 7569 7465 2069   MinAtar suite i
+00001190: 6e20 5067 783a 0a0a 6060 6073 680a 7069  n Pgx:..```sh.pi
+000011a0: 7020 696e 7374 616c 6c20 7067 782d 6d69  p install pgx-mi
+000011b0: 6e61 7461 720a 6060 600a 0a50 6778 2069  natar.```..Pgx i
+000011c0: 7320 7072 6f76 6964 6564 2075 6e64 6572  s provided under
+000011d0: 2074 6865 2041 7061 6368 6520 322e 3020   the Apache 2.0 
+000011e0: 4c69 6365 6e73 652c 2062 7574 2074 6865  License, but the
+000011f0: 206f 7269 6769 6e61 6c20 4d69 6e41 7461   original MinAta
+00001200: 7220 7375 6974 6520 666f 6c6c 6f77 7320  r suite follows 
+00001210: 7468 6520 4750 4c20 332e 3020 4c69 6365  the GPL 3.0 Lice
+00001220: 6e73 652e 2054 6865 7265 666f 7265 2c20  nse. Therefore, 
+00001230: 706c 6561 7365 206e 6f74 6520 7468 6174  please note that
+00001240: 2074 6865 2073 6570 6172 6174 6564 204d   the separated M
+00001250: 696e 4174 6172 2065 7874 656e 7369 6f6e  inAtar extension
+00001260: 2066 6f72 2050 6778 2061 6c73 6f20 6164   for Pgx also ad
+00001270: 6865 7265 7320 746f 2074 6865 2047 504c  heres to the GPL
+00001280: 2033 2e30 204c 6963 656e 7365 2e0a 0a23   3.0 License...#
+00001290: 2320 5375 7070 6f72 7465 6420 6761 6d65  # Supported game
+000012a0: 730a 0a7c 2042 6163 6b67 616d 6d6f 6e20  s..| Backgammon 
+000012b0: 7c20 4368 6573 7320 7c20 5368 6f67 6920  | Chess | Shogi 
+000012c0: 7c20 476f 207c 0a7c 3a2d 2d2d 3a7c 3a2d  | Go |.|:---:|:-
+000012d0: 2d2d 3a7c 3a2d 2d2d 3a7c 3a2d 2d2d 3a7c  --:|:---:|:---:|
+000012e0: 0a7c 3c69 6d67 2073 7263 3d22 6874 7470  .|<img src="http
+000012f0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00001300: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00001310: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00001320: 646f 6373 2f61 7373 6574 732f 6261 636b  docs/assets/back
+00001330: 6761 6d6d 6f6e 5f64 6172 6b2e 6769 6623  gammon_dark.gif#
+00001340: 6768 2d64 6172 6b2d 6d6f 6465 2d6f 6e6c  gh-dark-mode-onl
+00001350: 7922 2077 6964 7468 3d22 3137 3070 7822  y" width="170px"
+00001360: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00001370: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00001380: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
+00001390: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
+000013a0: 6f63 732f 6173 7365 7473 2f62 6163 6b67  ocs/assets/backg
+000013b0: 616d 6d6f 6e5f 6c69 6768 742e 6769 6623  ammon_light.gif#
+000013c0: 6768 2d6c 6967 6874 2d6d 6f64 652d 6f6e  gh-light-mode-on
+000013d0: 6c79 2220 7769 6474 683d 2231 3730 7078  ly" width="170px
+000013e0: 223e 7c3c 696d 6720 7372 633d 2268 7474  ">|<img src="htt
+000013f0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00001400: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
+00001410: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
+00001420: 2f64 6f63 732f 6173 7365 7473 2f63 6865  /docs/assets/che
+00001430: 7373 5f64 6172 6b2e 6769 6623 6768 2d64  ss_dark.gif#gh-d
+00001440: 6172 6b2d 6d6f 6465 2d6f 6e6c 7922 2077  ark-mode-only" w
+00001450: 6964 7468 3d22 3135 3870 7822 3e3c 696d  idth="158px"><im
+00001460: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+00001470: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00001480: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
+00001490: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
+000014a0: 6173 7365 7473 2f63 6865 7373 5f6c 6967  assets/chess_lig
+000014b0: 6874 2e67 6966 2367 682d 6c69 6768 742d  ht.gif#gh-light-
+000014c0: 6d6f 6465 2d6f 6e6c 7922 2077 6964 7468  mode-only" width
+000014d0: 3d22 3135 3870 7822 3e7c 3c69 6d67 2073  ="158px">|<img s
+000014e0: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+000014f0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00001500: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00001510: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+00001520: 6574 732f 7368 6f67 695f 6461 726b 2e67  ets/shogi_dark.g
+00001530: 6966 2367 682d 6461 726b 2d6d 6f64 652d  if#gh-dark-mode-
+00001540: 6f6e 6c79 2220 7769 6474 683d 2231 3730  only" width="170
+00001550: 7078 223e 3c69 6d67 2073 7263 3d22 6874  px"><img src="ht
+00001560: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00001570: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00001580: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
+00001590: 6e2f 646f 6373 2f61 7373 6574 732f 7368  n/docs/assets/sh
+000015a0: 6f67 695f 6c69 6768 742e 6769 6623 6768  ogi_light.gif#gh
+000015b0: 2d6c 6967 6874 2d6d 6f64 652d 6f6e 6c79  -light-mode-only
+000015c0: 2220 7769 6474 683d 2231 3730 7078 223e  " width="170px">
+000015d0: 7c3c 696d 6720 7372 633d 2268 7474 7073  |<img src="https
+000015e0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+000015f0: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
+00001600: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
+00001610: 6f63 732f 6173 7365 7473 2f67 6f2d 3139  ocs/assets/go-19
+00001620: 7831 395f 6461 726b 2e67 6966 2367 682d  x19_dark.gif#gh-
+00001630: 6461 726b 2d6d 6f64 652d 6f6e 6c79 2220  dark-mode-only" 
+00001640: 7769 6474 683d 2231 3630 7078 223e 3c69  width="160px"><i
+00001650: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00001660: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00001670: 6e74 656e 742e 636f 6d2f 736f 7465 7473  ntent.com/sotets
+00001680: 756b 2f70 6778 2f6d 6169 6e2f 646f 6373  uk/pgx/main/docs
+00001690: 2f61 7373 6574 732f 676f 2d31 3978 3139  /assets/go-19x19
+000016a0: 5f6c 6967 6874 2e67 6966 2367 682d 6c69  _light.gif#gh-li
+000016b0: 6768 742d 6d6f 6465 2d6f 6e6c 7922 2077  ght-mode-only" w
+000016c0: 6964 7468 3d22 3136 3070 7822 3e7c 0a0a  idth="160px">|..
+000016d0: 0a55 7365 2060 7067 782e 6176 6169 6c61  .Use `pgx.availa
+000016e0: 626c 655f 656e 7673 2829 202d 3e20 5475  ble_envs() -> Tu
+000016f0: 706c 655b 456e 7649 645d 6020 746f 2073  ple[EnvId]` to s
+00001700: 6565 2074 6865 206c 6973 7420 6f66 2063  ee the list of c
+00001710: 7572 7265 6e74 6c79 2061 7661 696c 6162  urrently availab
+00001720: 6c65 2067 616d 6573 2e20 4769 7665 6e20  le games. Given 
+00001730: 616e 2060 3c45 6e76 4964 3e60 2c20 796f  an `<EnvId>`, yo
+00001740: 7520 6361 6e20 6372 6561 7465 2074 6865  u can create the
+00001750: 2065 6e76 6972 6f6e 6d65 6e74 2076 6961   environment via
+00001760: 0a0a 6060 6070 790a 3e3e 3e20 656e 7620  ..```py.>>> env 
+00001770: 3d20 7067 782e 6d61 6b65 283c 456e 7649  = pgx.make(<EnvI
+00001780: 643e 290a 6060 600a 0a7c 2047 616d 652f  d>).```..| Game/
+00001790: 456e 7649 6420 7c20 5669 7375 616c 697a  EnvId | Visualiz
+000017a0: 6174 696f 6e20 7c20 5665 7273 696f 6e20  ation | Version 
+000017b0: 7c20 4669 7665 2d77 6f72 6420 6465 7363  | Five-word desc
+000017c0: 7269 7074 696f 6e20 7c0a 7c3a 2d2d 2d3a  ription |.|:---:
+000017d0: 7c3a 2d2d 2d3a 7c3a 2d2d 2d3a 7c3a 2d2d  |:---:|:---:|:--
+000017e0: 2d3a 7c0a 7c3c 6120 6872 6566 3d22 6874  -:|.|<a href="ht
+000017f0: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+00001800: 6961 2e6f 7267 2f77 696b 692f 3230 3438  ia.org/wiki/2048
+00001810: 5f28 7669 6465 6f5f 6761 6d65 2922 3e32  _(video_game)">2
+00001820: 3034 383c 2f61 3e20 3c62 723e 2060 2232  048</a> <br> `"2
+00001830: 3034 3822 6020 7c3c 696d 6720 7372 633d  048"` |<img src=
+00001840: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00001850: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00001860: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
+00001870: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
+00001880: 2f32 3034 385f 6461 726b 2e67 6966 2220  /2048_dark.gif" 
+00001890: 7769 6474 683d 2236 3070 7822 3e3c 696d  width="60px"><im
+000018a0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+000018b0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+000018c0: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
+000018d0: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
+000018e0: 6173 7365 7473 2f32 3034 385f 6c69 6768  assets/2048_ligh
+000018f0: 742e 6769 6622 2077 6964 7468 3d22 3630  t.gif" width="60
+00001900: 7078 223e 7c20 6076 3060 207c 202a 4d65  px">| `v0` | *Me
+00001910: 7267 6520 7469 6c65 7320 746f 2063 7265  rge tiles to cre
+00001920: 6174 6520 3230 3438 2e2a 207c 0a7c 3c61  ate 2048.* |.|<a
+00001930: 2068 7265 663d 2268 7474 7073 3a2f 2f65   href="https://e
+00001940: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+00001950: 7769 6b69 2f44 2543 3525 3844 6275 7473  wiki/D%C5%8Dbuts
+00001960: 755f 7368 2543 3525 3844 6769 223e 416e  u_sh%C5%8Dgi">An
+00001970: 696d 616c 2053 686f 6769 3c2f 613e 3c62  imal Shogi</a><b
+00001980: 723e 6022 616e 696d 616c 5f73 686f 6769  r>`"animal_shogi
+00001990: 2260 207c 3c69 6d67 2073 7263 3d22 6874  "` |<img src="ht
+000019a0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+000019b0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+000019c0: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
+000019d0: 6e2f 646f 6373 2f61 7373 6574 732f 616e  n/docs/assets/an
+000019e0: 696d 616c 5f73 686f 6769 5f64 6172 6b2e  imal_shogi_dark.
+000019f0: 6769 6622 2077 6964 7468 3d22 3630 7078  gif" width="60px
+00001a00: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00001a10: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00001a20: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00001a30: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00001a40: 646f 6373 2f61 7373 6574 732f 616e 696d  docs/assets/anim
+00001a50: 616c 5f73 686f 6769 5f6c 6967 6874 2e67  al_shogi_light.g
+00001a60: 6966 2220 7769 6474 683d 2236 3070 7822  if" width="60px"
+00001a70: 3e7c 2020 6076 3060 207c 202a 416e 696d  >|  `v0` | *Anim
+00001a80: 616c 2d74 6865 6d65 6420 6368 696c 642d  al-themed child-
+00001a90: 6672 6965 6e64 6c79 2073 686f 6769 2e2a  friendly shogi.*
+00001aa0: 207c 0a7c 3c61 2068 7265 663d 2268 7474   |.|<a href="htt
+00001ab0: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
+00001ac0: 612e 6f72 672f 7769 6b69 2f42 6163 6b67  a.org/wiki/Backg
+00001ad0: 616d 6d6f 6e22 3e42 6163 6b67 616d 6d6f  ammon">Backgammo
+00001ae0: 6e3c 2f61 3e3c 6272 3e60 2262 6163 6b67  n</a><br>`"backg
+00001af0: 616d 6d6f 6e22 6020 7c3c 696d 6720 7372  ammon"` |<img sr
+00001b00: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00001b10: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00001b20: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
+00001b30: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
+00001b40: 7473 2f62 6163 6b67 616d 6d6f 6e5f 6461  ts/backgammon_da
+00001b50: 726b 2e67 6966 2220 7769 6474 683d 2236  rk.gif" width="6
+00001b60: 3070 7822 3e3c 696d 6720 7372 633d 2268  0px"><img src="h
+00001b70: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00001b80: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00001b90: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
+00001ba0: 696e 2f64 6f63 732f 6173 7365 7473 2f62  in/docs/assets/b
+00001bb0: 6163 6b67 616d 6d6f 6e5f 6c69 6768 742e  ackgammon_light.
+00001bc0: 6769 6622 2077 6964 7468 3d22 3630 7078  gif" width="60px
+00001bd0: 223e 7c20 6076 3060 207c 202a 4c75 636b  ">| `v0` | *Luck
+00001be0: 2061 6964 7320 6265 6172 696e 6720 6f66   aids bearing of
+00001bf0: 6620 6368 6563 6b65 7273 2e2a 207c 0a7c  f checkers.* |.|
+00001c00: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001c10: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
+00001c20: 672f 7769 6b69 2f43 6f6e 7472 6163 745f  g/wiki/Contract_
+00001c30: 6272 6964 6765 223e 4272 6964 6765 2062  bridge">Bridge b
+00001c40: 6964 6469 6e67 3c2f 613e 3c62 723e 6022  idding</a><br>`"
+00001c50: 6272 6964 6765 5f62 6964 6469 6e67 2260  bridge_bidding"`
+00001c60: 207c 3c69 6d67 2073 7263 3d22 6874 7470   |<img src="http
+00001c70: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00001c80: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00001c90: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00001ca0: 646f 6373 2f61 7373 6574 732f 6272 6964  docs/assets/brid
+00001cb0: 6765 5f62 6964 6469 6e67 5f64 6172 6b2e  ge_bidding_dark.
+00001cc0: 6769 6622 2077 6964 7468 3d22 3630 7078  gif" width="60px
+00001cd0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00001ce0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00001cf0: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00001d00: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00001d10: 646f 6373 2f61 7373 6574 732f 6272 6964  docs/assets/brid
+00001d20: 6765 5f62 6964 6469 6e67 5f6c 6967 6874  ge_bidding_light
+00001d30: 2e67 6966 2220 7769 6474 683d 2236 3070  .gif" width="60p
+00001d40: 7822 3e7c 2060 7630 6020 7c20 2a50 6172  x">| `v0` | *Par
+00001d50: 746e 6572 7320 6578 6368 616e 6765 2069  tners exchange i
+00001d60: 6e66 6f72 6d61 7469 6f6e 2076 6961 2062  nformation via b
+00001d70: 6964 732e 2a20 7c0a 7c3c 6120 6872 6566  ids.* |.|<a href
+00001d80: 3d22 6874 7470 733a 2f2f 656e 2e77 696b  ="https://en.wik
+00001d90: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+00001da0: 4368 6573 7322 3e43 6865 7373 3c2f 613e  Chess">Chess</a>
+00001db0: 3c62 723e 6022 6368 6573 7322 6020 7c3c  <br>`"chess"` |<
+00001dc0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001dd0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00001de0: 6f6e 7465 6e74 2e63 6f6d 2f73 6f74 6574  ontent.com/sotet
+00001df0: 7375 6b2f 7067 782f 6d61 696e 2f64 6f63  suk/pgx/main/doc
+00001e00: 732f 6173 7365 7473 2f63 6865 7373 5f64  s/assets/chess_d
+00001e10: 6172 6b2e 6769 6622 2077 6964 7468 3d22  ark.gif" width="
+00001e20: 3630 7078 223e 3c69 6d67 2073 7263 3d22  60px"><img src="
+00001e30: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+00001e40: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+00001e50: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
+00001e60: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
+00001e70: 6368 6573 735f 6c69 6768 742e 6769 6622  chess_light.gif"
+00001e80: 2077 6964 7468 3d22 3630 7078 223e 7c20   width="60px">| 
+00001e90: 6076 3160 207c 202a 4368 6563 6b6d 6174  `v1` | *Checkmat
+00001ea0: 6520 6f70 706f 6e65 6e74 2773 206b 696e  e opponent's kin
+00001eb0: 6720 746f 2077 696e 2e2a 207c 0a7c 3c61  g to win.* |.|<a
+00001ec0: 2068 7265 663d 2268 7474 7073 3a2f 2f65   href="https://e
+00001ed0: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+00001ee0: 7769 6b69 2f43 6f6e 6e65 6374 5f46 6f75  wiki/Connect_Fou
+00001ef0: 7222 3e43 6f6e 6e65 6374 2046 6f75 723c  r">Connect Four<
+00001f00: 2f61 3e3c 6272 3e60 2263 6f6e 6e65 6374  /a><br>`"connect
+00001f10: 5f66 6f75 7222 6020 7c3c 696d 6720 7372  _four"` |<img sr
+00001f20: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00001f30: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00001f40: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
+00001f50: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
+00001f60: 7473 2f63 6f6e 6e65 6374 5f66 6f75 725f  ts/connect_four_
+00001f70: 6461 726b 2e67 6966 2220 7769 6474 683d  dark.gif" width=
+00001f80: 2236 3070 7822 3e3c 696d 6720 7372 633d  "60px"><img src=
+00001f90: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00001fa0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00001fb0: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
+00001fc0: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
+00001fd0: 2f63 6f6e 6e65 6374 5f66 6f75 725f 6c69  /connect_four_li
+00001fe0: 6768 742e 6769 6622 2077 6964 7468 3d22  ght.gif" width="
+00001ff0: 3630 7078 223e 7c20 6076 3060 207c 202a  60px">| `v0` | *
+00002000: 436f 6e6e 6563 7420 6469 7363 732c 2077  Connect discs, w
+00002010: 696e 2077 6974 6820 666f 7572 2e2a 207c  in with four.* |
+00002020: 0a7c 3c61 2068 7265 663d 2268 7474 7073  .|<a href="https
+00002030: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+00002040: 6f72 672f 7769 6b69 2f4d 696e 6963 6865  org/wiki/Miniche
+00002050: 7373 223e 4761 7264 6e65 7220 4368 6573  ss">Gardner Ches
+00002060: 733c 2f61 3e3c 6272 3e60 2267 6172 646e  s</a><br>`"gardn
+00002070: 6572 5f63 6865 7373 2260 7c3c 696d 6720  er_chess"`|<img 
+00002080: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00002090: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000020a0: 6e74 2e63 6f6d 2f73 6f74 6574 7375 6b2f  nt.com/sotetsuk/
+000020b0: 7067 782f 6d61 696e 2f64 6f63 732f 6173  pgx/main/docs/as
+000020c0: 7365 7473 2f67 6172 646e 6572 5f63 6865  sets/gardner_che
+000020d0: 7373 5f64 6172 6b2e 6769 6622 2077 6964  ss_dark.gif" wid
+000020e0: 7468 3d22 3630 7078 223e 3c69 6d67 2073  th="60px"><img s
+000020f0: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00002100: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002110: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00002120: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+00002130: 6574 732f 6761 7264 6e65 725f 6368 6573  ets/gardner_ches
+00002140: 735f 6c69 6768 742e 6769 6622 2077 6964  s_light.gif" wid
+00002150: 7468 3d22 3630 7078 223e 7c20 6076 3060  th="60px">| `v0`
+00002160: 207c 202a 3578 3520 6368 6573 7320 7661   | *5x5 chess va
+00002170: 7269 616e 742c 2065 7863 6c75 6469 6e67  riant, excluding
+00002180: 2063 6173 746c 696e 672e 2a20 7c0a 7c3c   castling.* |.|<
+00002190: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000021a0: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
+000021b0: 2f77 696b 692f 476f 5f28 6761 6d65 2922  /wiki/Go_(game)"
+000021c0: 3e47 6f3c 2f61 3e3c 6272 3e60 2267 6f5f  >Go</a><br>`"go_
+000021d0: 3978 3922 6020 6022 676f 5f31 3978 3139  9x9"` `"go_19x19
+000021e0: 2260 207c 3c69 6d67 2073 7263 3d22 6874  "` |<img src="ht
+000021f0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00002200: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00002210: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
+00002220: 6e2f 646f 6373 2f61 7373 6574 732f 676f  n/docs/assets/go
+00002230: 2d31 3978 3139 5f64 6172 6b2e 6769 6622  -19x19_dark.gif"
+00002240: 2077 6964 7468 3d22 3630 7078 223e 3c69   width="60px"><i
+00002250: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00002260: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00002270: 6e74 656e 742e 636f 6d2f 736f 7465 7473  ntent.com/sotets
+00002280: 756b 2f70 6778 2f6d 6169 6e2f 646f 6373  uk/pgx/main/docs
+00002290: 2f61 7373 6574 732f 676f 2d31 3978 3139  /assets/go-19x19
+000022a0: 5f6c 6967 6874 2e67 6966 2220 7769 6474  _light.gif" widt
+000022b0: 683d 2236 3070 7822 3e7c 2060 7630 6020  h="60px">| `v0` 
+000022c0: 7c20 2a53 7472 6174 6567 6963 616c 6c79  | *Strategically
+000022d0: 2070 6c61 6365 2073 746f 6e65 732c 2063   place stones, c
+000022e0: 6c61 696d 2074 6572 7269 746f 7279 2e2a  laim territory.*
+000022f0: 207c 0a7c 3c61 2068 7265 663d 2268 7474   |.|<a href="htt
+00002300: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
+00002310: 612e 6f72 672f 7769 6b69 2f48 6578 5f28  a.org/wiki/Hex_(
+00002320: 626f 6172 645f 6761 6d65 2922 3e48 6578  board_game)">Hex
+00002330: 3c2f 613e 3c62 723e 6022 6865 7822 6020  </a><br>`"hex"` 
+00002340: 7c3c 696d 6720 7372 633d 2268 7474 7073  |<img src="https
+00002350: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00002360: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
+00002370: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
+00002380: 6f63 732f 6173 7365 7473 2f68 6578 5f64  ocs/assets/hex_d
+00002390: 6172 6b2e 6769 6622 2077 6964 7468 3d22  ark.gif" width="
+000023a0: 3630 7078 223e 3c69 6d67 2073 7263 3d22  60px"><img src="
+000023b0: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+000023c0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+000023d0: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
+000023e0: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
+000023f0: 6865 785f 6c69 6768 742e 6769 6622 2077  hex_light.gif" w
+00002400: 6964 7468 3d22 3630 7078 223e 7c20 6076  idth="60px">| `v
+00002410: 3060 207c 202a 436f 6e6e 6563 7420 6f70  0` | *Connect op
+00002420: 706f 7369 7465 2073 6964 6573 2c20 626c  posite sides, bl
+00002430: 6f63 6b20 6f70 706f 6e65 6e74 2e2a 207c  ock opponent.* |
+00002440: 0a7c 3c61 2068 7265 663d 2268 7474 7073  .|<a href="https
+00002450: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+00002460: 6f72 672f 7769 6b69 2f4b 7568 6e5f 706f  org/wiki/Kuhn_po
+00002470: 6b65 7222 3e4b 7568 6e20 506f 6b65 723c  ker">Kuhn Poker<
+00002480: 2f61 3e3c 6272 3e60 226b 7568 6e5f 706f  /a><br>`"kuhn_po
+00002490: 6b65 7222 6020 7c3c 696d 6720 7372 633d  ker"` |<img src=
+000024a0: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+000024b0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+000024c0: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
+000024d0: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
+000024e0: 2f6b 7568 6e5f 706f 6b65 725f 6461 726b  /kuhn_poker_dark
+000024f0: 2e67 6966 2220 7769 6474 683d 2236 3070  .gif" width="60p
+00002500: 7822 3e3c 696d 6720 7372 633d 2268 7474  x"><img src="htt
+00002510: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00002520: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
+00002530: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
+00002540: 2f64 6f63 732f 6173 7365 7473 2f6b 7568  /docs/assets/kuh
+00002550: 6e5f 706f 6b65 725f 6c69 6768 742e 6769  n_poker_light.gi
+00002560: 6622 2077 6964 7468 3d22 3630 7078 223e  f" width="60px">
+00002570: 7c20 6076 3060 207c 202a 5468 7265 652d  | `v0` | *Three-
+00002580: 6361 7264 2062 6574 7469 6e67 2061 6e64  card betting and
+00002590: 2062 6c75 6666 696e 6720 6761 6d65 2e2a   bluffing game.*
+000025a0: 207c 0a7c 3c61 2068 7265 663d 2268 7474   |.|<a href="htt
+000025b0: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+000025c0: 6273 2f31 3230 372e 3134 3131 223e 4c65  bs/1207.1411">Le
+000025d0: 6475 6320 686f 6c64 2765 6d3c 2f61 3e3c  duc hold'em</a><
+000025e0: 6272 3e60 226c 6564 7563 5f68 6f6c 6465  br>`"leduc_holde
+000025f0: 6d22 6020 7c3c 696d 6720 7372 633d 2268  m"` |<img src="h
+00002600: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00002610: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00002620: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
+00002630: 696e 2f64 6f63 732f 6173 7365 7473 2f6c  in/docs/assets/l
+00002640: 6564 7563 5f68 6f6c 6465 6d5f 6461 726b  educ_holdem_dark
+00002650: 2e67 6966 2220 7769 6474 683d 2236 3070  .gif" width="60p
+00002660: 7822 3e3c 696d 6720 7372 633d 2268 7474  x"><img src="htt
+00002670: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00002680: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
+00002690: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
+000026a0: 2f64 6f63 732f 6173 7365 7473 2f6c 6564  /docs/assets/led
+000026b0: 7563 5f68 6f6c 6465 6d5f 6c69 6768 742e  uc_holdem_light.
+000026c0: 6769 6622 2077 6964 7468 3d22 3630 7078  gif" width="60px
+000026d0: 223e 7c20 6076 3060 207c 202a 5477 6f2d  ">| `v0` | *Two-
+000026e0: 7375 6974 2c20 6c69 6d69 7465 6420 6465  suit, limited de
+000026f0: 636b 2070 6f6b 6572 2e2a 207c 0a7c 3c61  ck poker.* |.|<a
+00002700: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00002710: 6974 6875 622e 636f 6d2f 6b65 6e6a 796f  ithub.com/kenjyo
+00002720: 756e 672f 4d69 6e41 7461 7222 3e4d 696e  ung/MinAtar">Min
+00002730: 4174 6172 2f41 7374 6572 6978 3c2f 613e  Atar/Asterix</a>
+00002740: 3c62 723e 6022 6d69 6e61 7461 722d 6173  <br>`"minatar-as
+00002750: 7465 7269 7822 6020 7c3c 696d 6720 7372  terix"` |<img sr
+00002760: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00002770: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00002780: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
+00002790: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
+000027a0: 7473 2f6d 696e 6174 6172 2d61 7374 6572  ts/minatar-aster
+000027b0: 6978 2e67 6966 2220 7769 6474 683d 2235  ix.gif" width="5
+000027c0: 3070 7822 3e7c 2060 7630 6020 7c20 2a41  0px">| `v0` | *A
+000027d0: 766f 6964 2065 6e65 6d69 6573 2c20 636f  void enemies, co
+000027e0: 6c6c 6563 7420 7472 6561 7375 7265 2c20  llect treasure, 
+000027f0: 7375 7276 6976 652e 2a20 7c0a 7c3c 6120  survive.* |.|<a 
+00002800: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00002810: 7468 7562 2e63 6f6d 2f6b 656e 6a79 6f75  thub.com/kenjyou
+00002820: 6e67 2f4d 696e 4174 6172 223e 4d69 6e41  ng/MinAtar">MinA
+00002830: 7461 722f 4272 6561 6b6f 7574 3c2f 613e  tar/Breakout</a>
+00002840: 3c62 723e 6022 6d69 6e61 7461 722d 6272  <br>`"minatar-br
+00002850: 6561 6b6f 7574 2260 207c 3c69 6d67 2073  eakout"` |<img s
+00002860: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00002870: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002880: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00002890: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+000028a0: 6574 732f 6d69 6e61 7461 722d 6272 6561  ets/minatar-brea
+000028b0: 6b6f 7574 2e67 6966 2220 7769 6474 683d  kout.gif" width=
+000028c0: 2235 3070 7822 3e7c 2060 7630 6020 7c20  "50px">| `v0` | 
+000028d0: 2a50 6164 646c 652c 2062 616c 6c2c 2062  *Paddle, ball, b
+000028e0: 7269 636b 732c 2062 6f75 6e63 652c 2063  ricks, bounce, c
+000028f0: 6c65 6172 2e2a 207c 0a7c 3c61 2068 7265  lear.* |.|<a hre
+00002900: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00002910: 622e 636f 6d2f 6b65 6e6a 796f 756e 672f  b.com/kenjyoung/
+00002920: 4d69 6e41 7461 7222 3e4d 696e 4174 6172  MinAtar">MinAtar
+00002930: 2f46 7265 6577 6179 3c2f 613e 3c62 723e  /Freeway</a><br>
+00002940: 6022 6d69 6e61 7461 722d 6672 6565 7761  `"minatar-freewa
+00002950: 7922 6020 7c3c 696d 6720 7372 633d 2268  y"` |<img src="h
+00002960: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00002970: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00002980: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
+00002990: 696e 2f64 6f63 732f 6173 7365 7473 2f6d  in/docs/assets/m
+000029a0: 696e 6174 6172 2d66 7265 6577 6179 2e67  inatar-freeway.g
+000029b0: 6966 2220 7769 6474 683d 2235 3070 7822  if" width="50px"
+000029c0: 3e7c 2060 7630 6020 7c20 2a44 6f64 6769  >| `v0` | *Dodgi
+000029d0: 6e67 2063 6172 732c 2063 6c69 6d62 696e  ng cars, climbin
+000029e0: 6720 7570 2066 7265 6577 6179 2e2a 207c  g up freeway.* |
+000029f0: 0a7c 3c61 2068 7265 663d 2268 7474 7073  .|<a href="https
+00002a00: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b65  ://github.com/ke
+00002a10: 6e6a 796f 756e 672f 4d69 6e41 7461 7222  njyoung/MinAtar"
+00002a20: 3e4d 696e 4174 6172 2f53 6561 7175 6573  >MinAtar/Seaques
+00002a30: 743c 2f61 3e3c 6272 3e60 226d 696e 6174  t</a><br>`"minat
+00002a40: 6172 2d73 6561 7175 6573 7422 6020 7c3c  ar-seaquest"` |<
+00002a50: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00002a60: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00002a70: 6f6e 7465 6e74 2e63 6f6d 2f73 6f74 6574  ontent.com/sotet
+00002a80: 7375 6b2f 7067 782f 6d61 696e 2f64 6f63  suk/pgx/main/doc
+00002a90: 732f 6173 7365 7473 2f6d 696e 6174 6172  s/assets/minatar
+00002aa0: 2d73 6561 7175 6573 742e 6769 6622 2077  -seaquest.gif" w
+00002ab0: 6964 7468 3d22 3530 7078 223e 7c20 6076  idth="50px">| `v
+00002ac0: 3060 207c 202a 556e 6465 7277 6174 6572  0` | *Underwater
+00002ad0: 2073 7562 6d61 7269 6e65 2072 6573 6375   submarine rescu
+00002ae0: 6520 616e 6420 636f 6d62 6174 2e2a 207c  e and combat.* |
+00002af0: 0a7c 3c61 2068 7265 663d 2268 7474 7073  .|<a href="https
+00002b00: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b65  ://github.com/ke
+00002b10: 6e6a 796f 756e 672f 4d69 6e41 7461 7222  njyoung/MinAtar"
+00002b20: 3e4d 696e 4174 6172 2f53 7061 6365 496e  >MinAtar/SpaceIn
+00002b30: 7661 6465 7273 3c2f 613e 3c62 723e 6022  vaders</a><br>`"
+00002b40: 6d69 6e61 7461 722d 7370 6163 655f 696e  minatar-space_in
+00002b50: 7661 6465 7273 2260 207c 3c69 6d67 2073  vaders"` |<img s
+00002b60: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00002b70: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002b80: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00002b90: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+00002ba0: 6574 732f 6d69 6e61 7461 722d 7370 6163  ets/minatar-spac
+00002bb0: 655f 696e 7661 6465 7273 2e67 6966 2220  e_invaders.gif" 
+00002bc0: 7769 6474 683d 2235 3070 7822 3e7c 2060  width="50px">| `
+00002bd0: 7630 6020 7c20 2a41 6c69 656e 2073 686f  v0` | *Alien sho
+00002be0: 6f74 6572 2067 616d 652c 2064 6f64 6765  oter game, dodge
+00002bf0: 2062 756c 6c65 7473 2e2a 207c 0a7c 3c61   bullets.* |.|<a
+00002c00: 2068 7265 663d 2268 7474 7073 3a2f 2f65   href="https://e
+00002c10: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+00002c20: 7769 6b69 2f52 6576 6572 7369 223e 4f74  wiki/Reversi">Ot
+00002c30: 6865 6c6c 6f3c 2f61 3e3c 6272 3e60 226f  hello</a><br>`"o
+00002c40: 7468 656c 6c6f 2260 207c 3c69 6d67 2073  thello"` |<img s
+00002c50: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00002c60: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002c70: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00002c80: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+00002c90: 6574 732f 6f74 6865 6c6c 6f5f 6461 726b  ets/othello_dark
+00002ca0: 2e67 6966 2220 7769 6474 683d 2236 3070  .gif" width="60p
+00002cb0: 7822 3e3c 696d 6720 7372 633d 2268 7474  x"><img src="htt
+00002cc0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00002cd0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
+00002ce0: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
+00002cf0: 2f64 6f63 732f 6173 7365 7473 2f6f 7468  /docs/assets/oth
+00002d00: 656c 6c6f 5f6c 6967 6874 2e67 6966 2220  ello_light.gif" 
+00002d10: 7769 6474 683d 2236 3070 7822 3e7c 2060  width="60px">| `
+00002d20: 7630 6020 7c20 2a46 6c69 7020 616e 6420  v0` | *Flip and 
+00002d30: 636f 6e71 7565 7220 6f70 706f 6e65 6e74  conquer opponent
+00002d40: 2773 2070 6965 6365 732e 2a20 7c0a 7c3c  's pieces.* |.|<
+00002d50: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00002d60: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
+00002d70: 2f77 696b 692f 5368 6f67 6922 3e53 686f  /wiki/Shogi">Sho
+00002d80: 6769 3c2f 613e 3c62 723e 6022 7368 6f67  gi</a><br>`"shog
+00002d90: 6922 6020 7c3c 696d 6720 7372 633d 2268  i"` |<img src="h
 00002da0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
 00002db0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
 00002dc0: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-00002dd0: 696e 2f64 6f63 732f 6173 7365 7473 2f6d  in/docs/assets/m
-00002de0: 696e 6174 6172 2d62 7265 616b 6f75 742e  inatar-breakout.
-00002df0: 6769 6622 2077 6964 7468 3d22 3530 7078  gif" width="50px
-00002e00: 223e 7c20 6076 3060 207c 202a 5061 6464  ">| `v0` | *Padd
-00002e10: 6c65 2c20 6261 6c6c 2c20 6272 6963 6b73  le, ball, bricks
-00002e20: 2c20 626f 756e 6365 2c20 636c 6561 722e  , bounce, clear.
-00002e30: 2a20 7c0a 7c3c 6120 6872 6566 3d22 6874  * |.|<a href="ht
-00002e40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002e50: 2f6b 656e 6a79 6f75 6e67 2f4d 696e 4174  /kenjyoung/MinAt
-00002e60: 6172 223e 4d69 6e41 7461 722f 4672 6565  ar">MinAtar/Free
-00002e70: 7761 793c 2f61 3e3c 6272 3e60 226d 696e  way</a><br>`"min
-00002e80: 6174 6172 2d66 7265 6577 6179 2260 207c  atar-freeway"` |
-00002e90: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00002ea0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00002eb0: 636f 6e74 656e 742e 636f 6d2f 736f 7465  content.com/sote
-00002ec0: 7473 756b 2f70 6778 2f6d 6169 6e2f 646f  tsuk/pgx/main/do
-00002ed0: 6373 2f61 7373 6574 732f 6d69 6e61 7461  cs/assets/minata
-00002ee0: 722d 6672 6565 7761 792e 6769 6622 2077  r-freeway.gif" w
-00002ef0: 6964 7468 3d22 3530 7078 223e 7c20 6076  idth="50px">| `v
-00002f00: 3060 207c 202a 446f 6467 696e 6720 6361  0` | *Dodging ca
-00002f10: 7273 2c20 636c 696d 6269 6e67 2075 7020  rs, climbing up 
-00002f20: 6672 6565 7761 792e 2a20 7c0a 7c3c 6120  freeway.* |.|<a 
-00002f30: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00002f40: 7468 7562 2e63 6f6d 2f6b 656e 6a79 6f75  thub.com/kenjyou
-00002f50: 6e67 2f4d 696e 4174 6172 223e 4d69 6e41  ng/MinAtar">MinA
-00002f60: 7461 722f 5365 6171 7565 7374 3c2f 613e  tar/Seaquest</a>
-00002f70: 3c62 723e 6022 6d69 6e61 7461 722d 7365  <br>`"minatar-se
-00002f80: 6171 7565 7374 2260 207c 3c69 6d67 2073  aquest"` |<img s
-00002f90: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-00002fa0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00002fb0: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
-00002fc0: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
-00002fd0: 6574 732f 6d69 6e61 7461 722d 7365 6171  ets/minatar-seaq
-00002fe0: 7565 7374 2e67 6966 2220 7769 6474 683d  uest.gif" width=
-00002ff0: 2235 3070 7822 3e7c 2060 7630 6020 7c20  "50px">| `v0` | 
-00003000: 2a55 6e64 6572 7761 7465 7220 7375 626d  *Underwater subm
-00003010: 6172 696e 6520 7265 7363 7565 2061 6e64  arine rescue and
-00003020: 2063 6f6d 6261 742e 2a20 7c0a 7c3c 6120   combat.* |.|<a 
-00003030: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00003040: 7468 7562 2e63 6f6d 2f6b 656e 6a79 6f75  thub.com/kenjyou
-00003050: 6e67 2f4d 696e 4174 6172 223e 4d69 6e41  ng/MinAtar">MinA
-00003060: 7461 722f 5370 6163 6549 6e76 6164 6572  tar/SpaceInvader
-00003070: 733c 2f61 3e3c 6272 3e60 226d 696e 6174  s</a><br>`"minat
-00003080: 6172 2d73 7061 6365 5f69 6e76 6164 6572  ar-space_invader
-00003090: 7322 6020 7c3c 696d 6720 7372 633d 2268  s"` |<img src="h
-000030a0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-000030b0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-000030c0: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-000030d0: 696e 2f64 6f63 732f 6173 7365 7473 2f6d  in/docs/assets/m
-000030e0: 696e 6174 6172 2d73 7061 6365 5f69 6e76  inatar-space_inv
-000030f0: 6164 6572 732e 6769 6622 2077 6964 7468  aders.gif" width
-00003100: 3d22 3530 7078 223e 7c20 6076 3060 207c  ="50px">| `v0` |
-00003110: 202a 416c 6965 6e20 7368 6f6f 7465 7220   *Alien shooter 
-00003120: 6761 6d65 2c20 646f 6467 6520 6275 6c6c  game, dodge bull
-00003130: 6574 732e 2a20 7c0a 7c3c 6120 6872 6566  ets.* |.|<a href
-00003140: 3d22 6874 7470 733a 2f2f 656e 2e77 696b  ="https://en.wik
-00003150: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-00003160: 5265 7665 7273 6922 3e4f 7468 656c 6c6f  Reversi">Othello
-00003170: 3c2f 613e 3c62 723e 6022 6f74 6865 6c6c  </a><br>`"othell
-00003180: 6f22 6020 7c3c 696d 6720 7372 633d 2268  o"` |<img src="h
-00003190: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-000031a0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-000031b0: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-000031c0: 696e 2f64 6f63 732f 6173 7365 7473 2f6f  in/docs/assets/o
-000031d0: 7468 656c 6c6f 5f64 6172 6b2e 6769 6622  thello_dark.gif"
-000031e0: 2077 6964 7468 3d22 3630 7078 223e 3c69   width="60px"><i
-000031f0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00003200: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00003210: 6e74 656e 742e 636f 6d2f 736f 7465 7473  ntent.com/sotets
-00003220: 756b 2f70 6778 2f6d 6169 6e2f 646f 6373  uk/pgx/main/docs
-00003230: 2f61 7373 6574 732f 6f74 6865 6c6c 6f5f  /assets/othello_
-00003240: 6c69 6768 742e 6769 6622 2077 6964 7468  light.gif" width
-00003250: 3d22 3630 7078 223e 7c20 6076 3060 207c  ="60px">| `v0` |
-00003260: 202a 466c 6970 2061 6e64 2063 6f6e 7175   *Flip and conqu
-00003270: 6572 206f 7070 6f6e 656e 7427 7320 7069  er opponent's pi
-00003280: 6563 6573 2e2a 207c 0a7c 3c61 2068 7265  eces.* |.|<a hre
-00003290: 663d 2268 7474 7073 3a2f 2f65 6e2e 7769  f="https://en.wi
-000032a0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
-000032b0: 2f53 686f 6769 223e 5368 6f67 693c 2f61  /Shogi">Shogi</a
-000032c0: 3e3c 6272 3e60 2273 686f 6769 2260 207c  ><br>`"shogi"` |
-000032d0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000032e0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-000032f0: 636f 6e74 656e 742e 636f 6d2f 736f 7465  content.com/sote
-00003300: 7473 756b 2f70 6778 2f6d 6169 6e2f 646f  tsuk/pgx/main/do
-00003310: 6373 2f61 7373 6574 732f 7368 6f67 695f  cs/assets/shogi_
-00003320: 6461 726b 2e67 6966 2220 7769 6474 683d  dark.gif" width=
-00003330: 2236 3070 7822 3e3c 696d 6720 7372 633d  "60px"><img src=
-00003340: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00003350: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00003360: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
-00003370: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
-00003380: 2f73 686f 6769 5f6c 6967 6874 2e67 6966  /shogi_light.gif
-00003390: 2220 7769 6474 683d 2236 3070 7822 3e20  " width="60px"> 
-000033a0: 7c20 6076 3060 207c 202a 4a61 7061 6e65  | `v0` | *Japane
-000033b0: 7365 2063 6865 7373 2077 6974 6820 6361  se chess with ca
-000033c0: 7074 7572 6564 2070 6965 6365 732e 2a20  ptured pieces.* 
-000033d0: 7c0a 7c3c 6120 6872 6566 3d22 6874 7470  |.|<a href="http
-000033e0: 733a 2f2f 7375 676f 726f 6b75 7961 2e6a  s://sugorokuya.j
-000033f0: 702f 702f 7375 7a75 6d65 2d6a 6f6e 6722  p/p/suzume-jong"
-00003400: 3e53 7061 7272 6f77 204d 6168 6a6f 6e67  >Sparrow Mahjong
-00003410: 3c2f 613e 3c62 723e 6022 7370 6172 726f  </a><br>`"sparro
-00003420: 775f 6d61 686a 6f6e 6722 6020 7c3c 696d  w_mahjong"` |<im
-00003430: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00003440: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00003450: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00003460: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-00003470: 6173 7365 7473 2f73 7061 7272 6f77 5f6d  assets/sparrow_m
-00003480: 6168 6a6f 6e67 5f64 6172 6b2e 7376 6722  ahjong_dark.svg"
-00003490: 2077 6964 7468 3d22 3630 7078 223e 3c69   width="60px"><i
-000034a0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000034b0: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-000034c0: 6e74 656e 742e 636f 6d2f 736f 7465 7473  ntent.com/sotets
-000034d0: 756b 2f70 6778 2f6d 6169 6e2f 646f 6373  uk/pgx/main/docs
-000034e0: 2f61 7373 6574 732f 7370 6172 726f 775f  /assets/sparrow_
-000034f0: 6d61 686a 6f6e 675f 6c69 6768 742e 7376  mahjong_light.sv
-00003500: 6722 2077 6964 7468 3d22 3630 7078 223e  g" width="60px">
-00003510: 7c20 2060 7630 6020 7c20 2a41 2073 696d  |  `v0` | *A sim
-00003520: 706c 6966 6965 642c 2063 6869 6c64 7265  plified, childre
-00003530: 6e2d 6672 6965 6e64 6c79 204d 6168 6a6f  n-friendly Mahjo
-00003540: 6e67 2e2a 207c 0a7c 3c61 2068 7265 663d  ng.* |.|<a href=
-00003550: 2268 7474 7073 3a2f 2f65 6e2e 7769 6b69  "https://en.wiki
-00003560: 7065 6469 612e 6f72 672f 7769 6b69 2f54  pedia.org/wiki/T
-00003570: 6963 2d74 6163 2d74 6f65 223e 5469 632d  ic-tac-toe">Tic-
-00003580: 7461 632d 746f 653c 2f61 3e3c 6272 3e60  tac-toe</a><br>`
-00003590: 2274 6963 5f74 6163 5f74 6f65 2260 207c  "tic_tac_toe"` |
-000035a0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000035b0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-000035c0: 636f 6e74 656e 742e 636f 6d2f 736f 7465  content.com/sote
-000035d0: 7473 756b 2f70 6778 2f6d 6169 6e2f 646f  tsuk/pgx/main/do
-000035e0: 6373 2f61 7373 6574 732f 7469 635f 7461  cs/assets/tic_ta
-000035f0: 635f 746f 655f 6461 726b 2e67 6966 2220  c_toe_dark.gif" 
-00003600: 7769 6474 683d 2236 3070 7822 3e3c 696d  width="60px"><im
-00003610: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00003620: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00003630: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00003640: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-00003650: 6173 7365 7473 2f74 6963 5f74 6163 5f74  assets/tic_tac_t
-00003660: 6f65 5f6c 6967 6874 2e67 6966 2220 7769  oe_light.gif" wi
-00003670: 6474 683d 2236 3070 7822 3e7c 2060 7630  dth="60px">| `v0
-00003680: 6020 7c20 2a54 6872 6565 2069 6e20 6120  ` | *Three in a 
-00003690: 726f 7720 7769 6e73 2e2a 207c 0a0a 2d20  row wins.* |..- 
-000036a0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000036b0: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-000036c0: 672f 7769 6b69 2f4a 6170 616e 6573 655f  g/wiki/Japanese_
-000036d0: 6d61 686a 6f6e 6722 3e4d 6168 6a6f 6e67  mahjong">Mahjong
-000036e0: 3c2f 613e 2065 6e76 6972 6f6e 6d65 6e74  </a> environment
-000036f0: 7320 6172 6520 756e 6465 7220 6465 7665  s are under deve
-00003700: 6c6f 706d 656e 7420 f09f 9aa7 2049 6620  lopment .... If 
-00003710: 796f 7520 6861 7665 2061 6e79 2072 6571  you have any req
-00003720: 7565 7374 7320 666f 7220 6e65 7720 656e  uests for new en
-00003730: 7669 726f 6e6d 656e 7473 2c20 706c 6561  vironments, plea
-00003740: 7365 206c 6574 2075 7320 6b6e 6f77 2062  se let us know b
-00003750: 7920 5b6f 7065 6e69 6e67 2061 6e20 6973  y [opening an is
-00003760: 7375 655d 2868 7474 7073 3a2f 2f67 6974  sue](https://git
-00003770: 6875 622e 636f 6d2f 736f 7465 7473 756b  hub.com/sotetsuk
-00003780: 2f70 6778 2f69 7373 7565 732f 6e65 7729  /pgx/issues/new)
-00003790: 0a2d 2046 6976 652d 776f 7264 2064 6573  .- Five-word des
-000037a0: 6372 6970 7469 6f6e 7320 7765 7265 2067  criptions were g
-000037b0: 656e 6572 6174 6564 2062 7920 5b43 6861  enerated by [Cha
-000037c0: 7447 5054 5d28 6874 7470 733a 2f2f 6368  tGPT](https://ch
-000037d0: 6174 2e6f 7065 6e61 692e 636f 6d2f 2920  at.openai.com/) 
-000037e0: f09f a496 0a0a 2323 2320 5665 7273 696f  ......### Versio
-000037f0: 6e69 6e67 2070 6f6c 6963 790a 0a45 6163  ning policy..Eac
-00003800: 6820 656e 7669 726f 6e6d 656e 7420 6973  h environment is
-00003810: 2076 6572 7369 6f6e 6564 2c20 616e 6420   versioned, and 
-00003820: 7468 6520 7665 7273 696f 6e20 6973 2069  the version is i
-00003830: 6e63 7265 6d65 6e74 6564 2077 6865 6e20  ncremented when 
-00003840: 7468 6572 6520 6172 6520 6368 616e 6765  there are change
-00003850: 7320 7468 6174 2061 6666 6563 7420 7468  s that affect th
-00003860: 6520 7065 7266 6f72 6d61 6e63 6520 6f66  e performance of
-00003870: 2061 6765 6e74 7320 6f72 2077 6865 6e20   agents or when 
-00003880: 7468 6572 6520 6172 6520 6368 616e 6765  there are change
-00003890: 7320 7468 6174 2061 7265 206e 6f74 2062  s that are not b
-000038a0: 6163 6b77 6172 6420 636f 6d70 6174 6962  ackward compatib
-000038b0: 6c65 2077 6974 6820 7468 6520 4150 492e  le with the API.
-000038c0: 0a49 6620 796f 7520 7761 6e74 2074 6f20  .If you want to 
-000038d0: 7075 7273 7565 2063 6f6d 706c 6574 6520  pursue complete 
-000038e0: 7265 7072 6f64 7563 6962 696c 6974 792c  reproducibility,
-000038f0: 2077 6520 7265 636f 6d6d 656e 6420 7468   we recommend th
-00003900: 6174 2079 6f75 2063 6865 636b 2074 6865  at you check the
-00003910: 2076 6572 7369 6f6e 206f 6620 5067 7820   version of Pgx 
-00003920: 616e 6420 6561 6368 2065 6e76 6972 6f6e  and each environ
-00003930: 6d65 6e74 2061 7320 666f 6c6c 6f77 733a  ment as follows:
-00003940: 0a0a 6060 6070 790a 3e3e 3e20 7067 782e  ..```py.>>> pgx.
-00003950: 5f5f 7665 7273 696f 6e5f 5f0a 2731 2e30  __version__.'1.0
-00003960: 2e30 270a 3e3e 3e20 656e 762e 7665 7273  .0'.>>> env.vers
-00003970: 696f 6e0a 2776 3027 0a60 6060 0a0a 2323  ion.'v0'.```..##
-00003980: 2053 6565 2061 6c73 6f0a 0a50 6778 2069   See also..Pgx i
-00003990: 7320 696e 7465 6e64 6564 2074 6f20 636f  s intended to co
-000039a0: 6d70 6c65 6d65 6e74 2074 6865 7365 202a  mplement these *
-000039b0: 2a4a 4158 2d6e 6174 6976 6520 656e 7669  *JAX-native envi
-000039c0: 726f 6e6d 656e 7473 2a2a 2077 6974 6820  ronments** with 
-000039d0: 2863 6c61 7373 6963 2920 626f 6172 6420  (classic) board 
-000039e0: 6761 6d65 2073 7569 7473 3a0a 0a2d 205b  game suits:..- [
-000039f0: 526f 6265 7274 544c 616e 6765 2f67 796d  RobertTLange/gym
-00003a00: 6e61 785d 2868 7474 7073 3a2f 2f67 6974  nax](https://git
-00003a10: 6875 622e 636f 6d2f 526f 6265 7274 544c  hub.com/RobertTL
-00003a20: 616e 6765 2f67 796d 6e61 7829 3a20 4a41  ange/gymnax): JA
-00003a30: 5820 696d 706c 656d 656e 7461 7469 6f6e  X implementation
-00003a40: 206f 6620 706f 7075 6c61 7220 524c 2065   of popular RL e
-00003a50: 6e76 6972 6f6e 6d65 6e74 7320 285b 636c  nvironments ([cl
-00003a60: 6173 7369 6320 636f 6e74 726f 6c5d 2868  assic control](h
-00003a70: 7474 7073 3a2f 2f67 796d 6e61 7369 756d  ttps://gymnasium
-00003a80: 2e66 6172 616d 612e 6f72 672f 656e 7669  .farama.org/envi
-00003a90: 726f 6e6d 656e 7473 2f63 6c61 7373 6963  ronments/classic
-00003aa0: 5f63 6f6e 7472 6f6c 292c 205b 6273 7569  _control), [bsui
-00003ab0: 7465 5d28 6874 7470 733a 2f2f 6769 7468  te](https://gith
-00003ac0: 7562 2e63 6f6d 2f64 6565 706d 696e 642f  ub.com/deepmind/
-00003ad0: 6273 7569 7465 292c 204d 696e 4174 6172  bsuite), MinAtar
-00003ae0: 2c20 6574 6329 2061 6e64 206d 6574 6120  , etc) and meta 
-00003af0: 524c 2074 6173 6b73 0a2d 205b 676f 6f67  RL tasks.- [goog
-00003b00: 6c65 2f62 7261 785d 2868 7474 7073 3a2f  le/brax](https:/
-00003b10: 2f67 6974 6875 622e 636f 6d2f 676f 6f67  /github.com/goog
-00003b20: 6c65 2f62 7261 7829 3a20 5269 6769 6462  le/brax): Rigidb
-00003b30: 6f64 7920 7068 7973 6963 7320 7369 6d75  ody physics simu
-00003b40: 6c61 7469 6f6e 2069 6e20 4a41 5820 616e  lation in JAX an
-00003b50: 6420 636f 6e74 696e 756f 7573 2d73 7061  d continuous-spa
-00003b60: 6365 2052 4c20 7461 736b 7320 2861 6e74  ce RL tasks (ant
-00003b70: 2c20 6665 7463 682c 2068 756d 616e 6f69  , fetch, humanoi
-00003b80: 642c 2065 7463 290a 2d20 5b69 6e73 7461  d, etc).- [insta
-00003b90: 6465 6570 6169 2f6a 756d 616e 6a69 5d28  deepai/jumanji](
-00003ba0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00003bb0: 6f6d 2f69 6e73 7461 6465 6570 6169 2f6a  om/instadeepai/j
-00003bc0: 756d 616e 6a69 293a 2041 2073 7569 7465  umanji): A suite
-00003bd0: 206f 6620 6469 7665 7273 6520 616e 6420   of diverse and 
-00003be0: 6368 616c 6c65 6e67 696e 670a 2020 2020  challenging.    
-00003bf0: 524c 2065 6e76 6972 6f6e 6d65 6e74 7320  RL environments 
-00003c00: 696e 204a 4158 2028 6269 6e2d 7061 636b  in JAX (bin-pack
-00003c10: 696e 672c 2072 6f75 7469 6e67 2070 726f  ing, routing pro
-00003c20: 626c 656d 732c 2065 7463 290a 0a43 6f6d  blems, etc)..Com
-00003c30: 6269 6e69 6e67 2050 6778 2077 6974 6820  bining Pgx with 
-00003c40: 7468 6573 6520 2a2a 4a41 582d 6e61 7469  these **JAX-nati
-00003c50: 7665 2061 6c67 6f72 6974 686d 732f 696d  ve algorithms/im
-00003c60: 706c 656d 656e 7461 7469 6f6e 732a 2a20  plementations** 
-00003c70: 6d69 6768 7420 6265 2061 6e20 696e 7465  might be an inte
-00003c80: 7265 7374 696e 6720 6469 7265 6374 696f  resting directio
-00003c90: 6e3a 0a0a 2d20 5b41 6e61 6b69 6e20 6672  n:..- [Anakin fr
-00003ca0: 616d 6577 6f72 6b5d 2868 7474 7073 3a2f  amework](https:/
-00003cb0: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
-00003cc0: 3130 342e 3036 3237 3229 3a20 4869 6768  104.06272): High
-00003cd0: 6c79 2065 6666 6963 6965 6e74 2052 4c20  ly efficient RL 
-00003ce0: 6672 616d 6577 6f72 6b20 7468 6174 2077  framework that w
-00003cf0: 6f72 6b73 2077 6974 6820 4a41 582d 6e61  orks with JAX-na
-00003d00: 7469 7665 2065 6e76 6972 6f6e 6d65 6e74  tive environment
-00003d10: 7320 6f6e 2054 5055 730a 2d20 5b64 6565  s on TPUs.- [dee
-00003d20: 706d 696e 642f 6d63 7478 5d28 6874 7470  pmind/mctx](http
-00003d30: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-00003d40: 6565 706d 696e 642f 6d63 7478 293a 204a  eepmind/mctx): J
-00003d50: 4158 2d6e 6174 6976 6520 4d43 5453 2069  AX-native MCTS i
-00003d60: 6d70 6c65 6d65 6e74 6174 696f 6e73 2c20  mplementations, 
-00003d70: 696e 636c 7564 696e 6720 416c 7068 615a  including AlphaZ
-00003d80: 6572 6f20 616e 6420 4d75 5a65 726f 0a2d  ero and MuZero.-
-00003d90: 205b 6465 6570 6d69 6e64 2f72 6c61 785d   [deepmind/rlax]
-00003da0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003db0: 636f 6d2f 6465 6570 6d69 6e64 2f72 6c61  com/deepmind/rla
-00003dc0: 7829 3a20 4a41 582d 6e61 7469 7665 2052  x): JAX-native R
-00003dd0: 4c20 636f 6d70 6f6e 656e 7473 0a2d 205b  L components.- [
-00003de0: 676f 6f67 6c65 2f65 766f 6a61 785d 2868  google/evojax](h
-00003df0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003e00: 6d2f 676f 6f67 6c65 2f65 766f 6a61 7829  m/google/evojax)
-00003e10: 3a20 4861 7264 7761 7265 2d41 6363 656c  : Hardware-Accel
-00003e20: 6572 6174 6564 206e 6575 726f 6576 6f6c  erated neuroevol
-00003e30: 7574 696f 6e0a 2d20 5b52 6f62 6572 7454  ution.- [RobertT
-00003e40: 4c61 6e67 652f 6576 6f73 6178 5d28 6874  Lange/evosax](ht
-00003e50: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003e60: 2f52 6f62 6572 7454 4c61 6e67 652f 6576  /RobertTLange/ev
-00003e70: 6f73 6178 293a 204a 4158 2d6e 6174 6976  osax): JAX-nativ
-00003e80: 6520 6576 6f6c 7574 696f 6e20 7374 7261  e evolution stra
-00003e90: 7465 6779 2028 4553 2920 696d 706c 656d  tegy (ES) implem
-00003ea0: 656e 7461 7469 6f6e 730a 2d20 5b61 6461  entations.- [ada
-00003eb0: 7074 6976 652d 696e 7465 6c6c 6967 656e  ptive-intelligen
-00003ec0: 742d 726f 626f 7469 6373 2f51 4461 785d  t-robotics/QDax]
-00003ed0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003ee0: 636f 6d2f 6164 6170 7469 7665 2d69 6e74  com/adaptive-int
-00003ef0: 656c 6c69 6765 6e74 2d72 6f62 6f74 6963  elligent-robotic
-00003f00: 732f 5144 6178 293a 204a 4158 2d6e 6174  s/QDax): JAX-nat
-00003f10: 6976 6520 5175 616c 6974 792d 4469 7665  ive Quality-Dive
-00003f20: 7273 6974 7920 2851 4429 2061 6c67 6f72  rsity (QD) algor
-00003f30: 6974 686d 730a 2d20 5b6c 7563 6872 6973  ithms.- [luchris
-00003f40: 3432 392f 7075 7265 6a61 7872 6c5d 2868  429/purejaxrl](h
-00003f50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003f60: 6d2f 6c75 6368 7269 7334 3239 2f70 7572  m/luchris429/pur
-00003f70: 656a 6178 726c 293a 204a 6178 2d6e 6174  ejaxrl): Jax-nat
-00003f80: 6976 6520 524c 2069 6d70 6c65 6d65 6e74  ive RL implement
-00003f90: 6174 696f 6e73 0a0a 2323 2043 6974 6174  ations..## Citat
-00003fa0: 696f 6e0a 0a60 6060 0a40 6172 7469 636c  ion..```.@articl
-00003fb0: 657b 6b6f 7961 6d61 6461 3230 3233 7067  e{koyamada2023pg
-00003fc0: 782c 0a20 2074 6974 6c65 3d7b 5067 783a  x,.  title={Pgx:
-00003fd0: 2048 6172 6477 6172 652d 6163 6365 6c65   Hardware-accele
-00003fe0: 7261 7465 6420 7061 7261 6c6c 656c 2067  rated parallel g
-00003ff0: 616d 6520 7369 6d75 6c61 7469 6f6e 2066  ame simulation f
-00004000: 6f72 2072 6569 6e66 6f72 6365 6d65 6e74  or reinforcement
-00004010: 206c 6561 726e 696e 677d 2c0a 2020 6175   learning},.  au
-00004020: 7468 6f72 3d7b 4b6f 7961 6d61 6461 2c20  thor={Koyamada, 
-00004030: 536f 7465 7473 7520 616e 6420 4f6b 616e  Sotetsu and Okan
-00004040: 6f2c 2053 6869 6e72 6920 616e 6420 4e69  o, Shinri and Ni
-00004050: 7368 696d 6f72 692c 2053 6f69 6368 6972  shimori, Soichir
-00004060: 6f20 616e 6420 4d75 7261 7461 2c20 5975  o and Murata, Yu
-00004070: 2061 6e64 2048 6162 6172 612c 204b 6569   and Habara, Kei
-00004080: 676f 2061 6e64 204b 6974 612c 2048 6172  go and Kita, Har
-00004090: 756b 6120 616e 6420 4973 6869 692c 2053  uka and Ishii, S
-000040a0: 6869 6e7d 2c0a 2020 6a6f 7572 6e61 6c3d  hin},.  journal=
-000040b0: 7b61 7258 6976 2070 7265 7072 696e 7420  {arXiv preprint 
-000040c0: 6172 5869 763a 3233 3033 2e31 3735 3033  arXiv:2303.17503
-000040d0: 7d2c 0a20 2079 6561 723d 7b32 3032 337d  },.  year={2023}
-000040e0: 0a7d 0a60 6060 0a0a 2323 204c 4943 454e  .}.```..## LICEN
-000040f0: 5345 0a0a 4170 6163 6865 2d32 2e30 0a    SE..Apache-2.0.
+00002dd0: 696e 2f64 6f63 732f 6173 7365 7473 2f73  in/docs/assets/s
+00002de0: 686f 6769 5f64 6172 6b2e 6769 6622 2077  hogi_dark.gif" w
+00002df0: 6964 7468 3d22 3630 7078 223e 3c69 6d67  idth="60px"><img
+00002e00: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00002e10: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00002e20: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
+00002e30: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
+00002e40: 7373 6574 732f 7368 6f67 695f 6c69 6768  ssets/shogi_ligh
+00002e50: 742e 6769 6622 2077 6964 7468 3d22 3630  t.gif" width="60
+00002e60: 7078 223e 207c 2060 7630 6020 7c20 2a4a  px"> | `v0` | *J
+00002e70: 6170 616e 6573 6520 6368 6573 7320 7769  apanese chess wi
+00002e80: 7468 2063 6170 7475 7265 6420 7069 6563  th captured piec
+00002e90: 6573 2e2a 207c 0a7c 3c61 2068 7265 663d  es.* |.|<a href=
+00002ea0: 2268 7474 7073 3a2f 2f73 7567 6f72 6f6b  "https://sugorok
+00002eb0: 7579 612e 6a70 2f70 2f73 757a 756d 652d  uya.jp/p/suzume-
+00002ec0: 6a6f 6e67 223e 5370 6172 726f 7720 4d61  jong">Sparrow Ma
+00002ed0: 686a 6f6e 673c 2f61 3e3c 6272 3e60 2273  hjong</a><br>`"s
+00002ee0: 7061 7272 6f77 5f6d 6168 6a6f 6e67 2260  parrow_mahjong"`
+00002ef0: 207c 3c69 6d67 2073 7263 3d22 6874 7470   |<img src="http
+00002f00: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00002f10: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00002f20: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00002f30: 646f 6373 2f61 7373 6574 732f 7370 6172  docs/assets/spar
+00002f40: 726f 775f 6d61 686a 6f6e 675f 6461 726b  row_mahjong_dark
+00002f50: 2e73 7667 2220 7769 6474 683d 2236 3070  .svg" width="60p
+00002f60: 7822 3e3c 696d 6720 7372 633d 2268 7474  x"><img src="htt
+00002f70: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00002f80: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
+00002f90: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
+00002fa0: 2f64 6f63 732f 6173 7365 7473 2f73 7061  /docs/assets/spa
+00002fb0: 7272 6f77 5f6d 6168 6a6f 6e67 5f6c 6967  rrow_mahjong_lig
+00002fc0: 6874 2e73 7667 2220 7769 6474 683d 2236  ht.svg" width="6
+00002fd0: 3070 7822 3e7c 2020 6076 3060 207c 202a  0px">|  `v0` | *
+00002fe0: 4120 7369 6d70 6c69 6669 6564 2c20 6368  A simplified, ch
+00002ff0: 696c 6472 656e 2d66 7269 656e 646c 7920  ildren-friendly 
+00003000: 4d61 686a 6f6e 672e 2a20 7c0a 7c3c 6120  Mahjong.* |.|<a 
+00003010: 6872 6566 3d22 6874 7470 733a 2f2f 656e  href="https://en
+00003020: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+00003030: 696b 692f 5469 632d 7461 632d 746f 6522  iki/Tic-tac-toe"
+00003040: 3e54 6963 2d74 6163 2d74 6f65 3c2f 613e  >Tic-tac-toe</a>
+00003050: 3c62 723e 6022 7469 635f 7461 635f 746f  <br>`"tic_tac_to
+00003060: 6522 6020 7c3c 696d 6720 7372 633d 2268  e"` |<img src="h
+00003070: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00003080: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00003090: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
+000030a0: 696e 2f64 6f63 732f 6173 7365 7473 2f74  in/docs/assets/t
+000030b0: 6963 5f74 6163 5f74 6f65 5f64 6172 6b2e  ic_tac_toe_dark.
+000030c0: 6769 6622 2077 6964 7468 3d22 3630 7078  gif" width="60px
+000030d0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+000030e0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+000030f0: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00003100: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00003110: 646f 6373 2f61 7373 6574 732f 7469 635f  docs/assets/tic_
+00003120: 7461 635f 746f 655f 6c69 6768 742e 6769  tac_toe_light.gi
+00003130: 6622 2077 6964 7468 3d22 3630 7078 223e  f" width="60px">
+00003140: 7c20 6076 3060 207c 202a 5468 7265 6520  | `v0` | *Three 
+00003150: 696e 2061 2072 6f77 2077 696e 732e 2a20  in a row wins.* 
+00003160: 7c0a 0a2d 203c 6120 6872 6566 3d22 6874  |..- <a href="ht
+00003170: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+00003180: 6961 2e6f 7267 2f77 696b 692f 4a61 7061  ia.org/wiki/Japa
+00003190: 6e65 7365 5f6d 6168 6a6f 6e67 223e 4d61  nese_mahjong">Ma
+000031a0: 686a 6f6e 673c 2f61 3e20 656e 7669 726f  hjong</a> enviro
+000031b0: 6e6d 656e 7473 2061 7265 2075 6e64 6572  nments are under
+000031c0: 2064 6576 656c 6f70 6d65 6e74 20f0 9f9a   development ...
+000031d0: a720 4966 2079 6f75 2068 6176 6520 616e  . If you have an
+000031e0: 7920 7265 7175 6573 7473 2066 6f72 206e  y requests for n
+000031f0: 6577 2065 6e76 6972 6f6e 6d65 6e74 732c  ew environments,
+00003200: 2070 6c65 6173 6520 6c65 7420 7573 206b   please let us k
+00003210: 6e6f 7720 6279 205b 6f70 656e 696e 6720  now by [opening 
+00003220: 616e 2069 7373 7565 5d28 6874 7470 733a  an issue](https:
+00003230: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6f74  //github.com/sot
+00003240: 6574 7375 6b2f 7067 782f 6973 7375 6573  etsuk/pgx/issues
+00003250: 2f6e 6577 290a 2d20 4669 7665 2d77 6f72  /new).- Five-wor
+00003260: 6420 6465 7363 7269 7074 696f 6e73 2077  d descriptions w
+00003270: 6572 6520 6765 6e65 7261 7465 6420 6279  ere generated by
+00003280: 205b 4368 6174 4750 545d 2868 7474 7073   [ChatGPT](https
+00003290: 3a2f 2f63 6861 742e 6f70 656e 6169 2e63  ://chat.openai.c
+000032a0: 6f6d 2f29 20f0 9fa4 960a 0a23 2323 2056  om/) ......### V
+000032b0: 6572 7369 6f6e 696e 6720 706f 6c69 6379  ersioning policy
+000032c0: 0a0a 4561 6368 2065 6e76 6972 6f6e 6d65  ..Each environme
+000032d0: 6e74 2069 7320 7665 7273 696f 6e65 642c  nt is versioned,
+000032e0: 2061 6e64 2074 6865 2076 6572 7369 6f6e   and the version
+000032f0: 2069 7320 696e 6372 656d 656e 7465 6420   is incremented 
+00003300: 7768 656e 2074 6865 7265 2061 7265 2063  when there are c
+00003310: 6861 6e67 6573 2074 6861 7420 6166 6665  hanges that affe
+00003320: 6374 2074 6865 2070 6572 666f 726d 616e  ct the performan
+00003330: 6365 206f 6620 6167 656e 7473 206f 7220  ce of agents or 
+00003340: 7768 656e 2074 6865 7265 2061 7265 2063  when there are c
+00003350: 6861 6e67 6573 2074 6861 7420 6172 6520  hanges that are 
+00003360: 6e6f 7420 6261 636b 7761 7264 2063 6f6d  not backward com
+00003370: 7061 7469 626c 6520 7769 7468 2074 6865  patible with the
+00003380: 2041 5049 2e0a 4966 2079 6f75 2077 616e   API..If you wan
+00003390: 7420 746f 2070 7572 7375 6520 636f 6d70  t to pursue comp
+000033a0: 6c65 7465 2072 6570 726f 6475 6369 6269  lete reproducibi
+000033b0: 6c69 7479 2c20 7765 2072 6563 6f6d 6d65  lity, we recomme
+000033c0: 6e64 2074 6861 7420 796f 7520 6368 6563  nd that you chec
+000033d0: 6b20 7468 6520 7665 7273 696f 6e20 6f66  k the version of
+000033e0: 2050 6778 2061 6e64 2065 6163 6820 656e   Pgx and each en
+000033f0: 7669 726f 6e6d 656e 7420 6173 2066 6f6c  vironment as fol
+00003400: 6c6f 7773 3a0a 0a60 6060 7079 0a3e 3e3e  lows:..```py.>>>
+00003410: 2070 6778 2e5f 5f76 6572 7369 6f6e 5f5f   pgx.__version__
+00003420: 0a27 312e 302e 3027 0a3e 3e3e 2065 6e76  .'1.0.0'.>>> env
+00003430: 2e76 6572 7369 6f6e 0a27 7630 270a 6060  .version.'v0'.``
+00003440: 600a 0a23 2320 5365 6520 616c 736f 0a0a  `..## See also..
+00003450: 5067 7820 6973 2069 6e74 656e 6465 6420  Pgx is intended 
+00003460: 746f 2063 6f6d 706c 656d 656e 7420 7468  to complement th
+00003470: 6573 6520 2a2a 4a41 582d 6e61 7469 7665  ese **JAX-native
+00003480: 2065 6e76 6972 6f6e 6d65 6e74 732a 2a20   environments** 
+00003490: 7769 7468 2028 636c 6173 7369 6329 2062  with (classic) b
+000034a0: 6f61 7264 2067 616d 6520 7375 6974 733a  oard game suits:
+000034b0: 0a0a 2d20 5b52 6f62 6572 7454 4c61 6e67  ..- [RobertTLang
+000034c0: 652f 6779 6d6e 6178 5d28 6874 7470 733a  e/gymnax](https:
+000034d0: 2f2f 6769 7468 7562 2e63 6f6d 2f52 6f62  //github.com/Rob
+000034e0: 6572 7454 4c61 6e67 652f 6779 6d6e 6178  ertTLange/gymnax
+000034f0: 293a 204a 4158 2069 6d70 6c65 6d65 6e74  ): JAX implement
+00003500: 6174 696f 6e20 6f66 2070 6f70 756c 6172  ation of popular
+00003510: 2052 4c20 656e 7669 726f 6e6d 656e 7473   RL environments
+00003520: 2028 5b63 6c61 7373 6963 2063 6f6e 7472   ([classic contr
+00003530: 6f6c 5d28 6874 7470 733a 2f2f 6779 6d6e  ol](https://gymn
+00003540: 6173 6975 6d2e 6661 7261 6d61 2e6f 7267  asium.farama.org
+00003550: 2f65 6e76 6972 6f6e 6d65 6e74 732f 636c  /environments/cl
+00003560: 6173 7369 635f 636f 6e74 726f 6c29 2c20  assic_control), 
+00003570: 5b62 7375 6974 655d 2868 7474 7073 3a2f  [bsuite](https:/
+00003580: 2f67 6974 6875 622e 636f 6d2f 6465 6570  /github.com/deep
+00003590: 6d69 6e64 2f62 7375 6974 6529 2c20 4d69  mind/bsuite), Mi
+000035a0: 6e41 7461 722c 2065 7463 2920 616e 6420  nAtar, etc) and 
+000035b0: 6d65 7461 2052 4c20 7461 736b 730a 2d20  meta RL tasks.- 
+000035c0: 5b67 6f6f 676c 652f 6272 6178 5d28 6874  [google/brax](ht
+000035d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000035e0: 2f67 6f6f 676c 652f 6272 6178 293a 2052  /google/brax): R
+000035f0: 6967 6964 626f 6479 2070 6879 7369 6373  igidbody physics
+00003600: 2073 696d 756c 6174 696f 6e20 696e 204a   simulation in J
+00003610: 4158 2061 6e64 2063 6f6e 7469 6e75 6f75  AX and continuou
+00003620: 732d 7370 6163 6520 524c 2074 6173 6b73  s-space RL tasks
+00003630: 2028 616e 742c 2066 6574 6368 2c20 6875   (ant, fetch, hu
+00003640: 6d61 6e6f 6964 2c20 6574 6329 0a2d 205b  manoid, etc).- [
+00003650: 696e 7374 6164 6565 7061 692f 6a75 6d61  instadeepai/juma
+00003660: 6e6a 695d 2868 7474 7073 3a2f 2f67 6974  nji](https://git
+00003670: 6875 622e 636f 6d2f 696e 7374 6164 6565  hub.com/instadee
+00003680: 7061 692f 6a75 6d61 6e6a 6929 3a20 4120  pai/jumanji): A 
+00003690: 7375 6974 6520 6f66 2064 6976 6572 7365  suite of diverse
+000036a0: 2061 6e64 2063 6861 6c6c 656e 6769 6e67   and challenging
+000036b0: 0a20 2020 2052 4c20 656e 7669 726f 6e6d  .    RL environm
+000036c0: 656e 7473 2069 6e20 4a41 5820 2862 696e  ents in JAX (bin
+000036d0: 2d70 6163 6b69 6e67 2c20 726f 7574 696e  -packing, routin
+000036e0: 6720 7072 6f62 6c65 6d73 2c20 6574 6329  g problems, etc)
+000036f0: 0a0a 436f 6d62 696e 696e 6720 5067 7820  ..Combining Pgx 
+00003700: 7769 7468 2074 6865 7365 202a 2a4a 4158  with these **JAX
+00003710: 2d6e 6174 6976 6520 616c 676f 7269 7468  -native algorith
+00003720: 6d73 2f69 6d70 6c65 6d65 6e74 6174 696f  ms/implementatio
+00003730: 6e73 2a2a 206d 6967 6874 2062 6520 616e  ns** might be an
+00003740: 2069 6e74 6572 6573 7469 6e67 2064 6972   interesting dir
+00003750: 6563 7469 6f6e 3a0a 0a2d 205b 416e 616b  ection:..- [Anak
+00003760: 696e 2066 7261 6d65 776f 726b 5d28 6874  in framework](ht
+00003770: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
+00003780: 6162 732f 3231 3034 2e30 3632 3732 293a  abs/2104.06272):
+00003790: 2048 6967 686c 7920 6566 6669 6369 656e   Highly efficien
+000037a0: 7420 524c 2066 7261 6d65 776f 726b 2074  t RL framework t
+000037b0: 6861 7420 776f 726b 7320 7769 7468 204a  hat works with J
+000037c0: 4158 2d6e 6174 6976 6520 656e 7669 726f  AX-native enviro
+000037d0: 6e6d 656e 7473 206f 6e20 5450 5573 0a2d  nments on TPUs.-
+000037e0: 205b 6465 6570 6d69 6e64 2f6d 6374 785d   [deepmind/mctx]
+000037f0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00003800: 636f 6d2f 6465 6570 6d69 6e64 2f6d 6374  com/deepmind/mct
+00003810: 7829 3a20 4a41 582d 6e61 7469 7665 204d  x): JAX-native M
+00003820: 4354 5320 696d 706c 656d 656e 7461 7469  CTS implementati
+00003830: 6f6e 732c 2069 6e63 6c75 6469 6e67 2041  ons, including A
+00003840: 6c70 6861 5a65 726f 2061 6e64 204d 755a  lphaZero and MuZ
+00003850: 6572 6f0a 2d20 5b64 6565 706d 696e 642f  ero.- [deepmind/
+00003860: 726c 6178 5d28 6874 7470 733a 2f2f 6769  rlax](https://gi
+00003870: 7468 7562 2e63 6f6d 2f64 6565 706d 696e  thub.com/deepmin
+00003880: 642f 726c 6178 293a 204a 4158 2d6e 6174  d/rlax): JAX-nat
+00003890: 6976 6520 524c 2063 6f6d 706f 6e65 6e74  ive RL component
+000038a0: 730a 2d20 5b67 6f6f 676c 652f 6576 6f6a  s.- [google/evoj
+000038b0: 6178 5d28 6874 7470 733a 2f2f 6769 7468  ax](https://gith
+000038c0: 7562 2e63 6f6d 2f67 6f6f 676c 652f 6576  ub.com/google/ev
+000038d0: 6f6a 6178 293a 2048 6172 6477 6172 652d  ojax): Hardware-
+000038e0: 4163 6365 6c65 7261 7465 6420 6e65 7572  Accelerated neur
+000038f0: 6f65 766f 6c75 7469 6f6e 0a2d 205b 526f  oevolution.- [Ro
+00003900: 6265 7274 544c 616e 6765 2f65 766f 7361  bertTLange/evosa
+00003910: 785d 2868 7474 7073 3a2f 2f67 6974 6875  x](https://githu
+00003920: 622e 636f 6d2f 526f 6265 7274 544c 616e  b.com/RobertTLan
+00003930: 6765 2f65 766f 7361 7829 3a20 4a41 582d  ge/evosax): JAX-
+00003940: 6e61 7469 7665 2065 766f 6c75 7469 6f6e  native evolution
+00003950: 2073 7472 6174 6567 7920 2845 5329 2069   strategy (ES) i
+00003960: 6d70 6c65 6d65 6e74 6174 696f 6e73 0a2d  mplementations.-
+00003970: 205b 6164 6170 7469 7665 2d69 6e74 656c   [adaptive-intel
+00003980: 6c69 6765 6e74 2d72 6f62 6f74 6963 732f  ligent-robotics/
+00003990: 5144 6178 5d28 6874 7470 733a 2f2f 6769  QDax](https://gi
+000039a0: 7468 7562 2e63 6f6d 2f61 6461 7074 6976  thub.com/adaptiv
+000039b0: 652d 696e 7465 6c6c 6967 656e 742d 726f  e-intelligent-ro
+000039c0: 626f 7469 6373 2f51 4461 7829 3a20 4a41  botics/QDax): JA
+000039d0: 582d 6e61 7469 7665 2051 7561 6c69 7479  X-native Quality
+000039e0: 2d44 6976 6572 7369 7479 2028 5144 2920  -Diversity (QD) 
+000039f0: 616c 676f 7269 7468 6d73 0a2d 205b 6c75  algorithms.- [lu
+00003a00: 6368 7269 7334 3239 2f70 7572 656a 6178  chris429/purejax
+00003a10: 726c 5d28 6874 7470 733a 2f2f 6769 7468  rl](https://gith
+00003a20: 7562 2e63 6f6d 2f6c 7563 6872 6973 3432  ub.com/luchris42
+00003a30: 392f 7075 7265 6a61 7872 6c29 3a20 4a61  9/purejaxrl): Ja
+00003a40: 782d 6e61 7469 7665 2052 4c20 696d 706c  x-native RL impl
+00003a50: 656d 656e 7461 7469 6f6e 730a 0a23 2320  ementations..## 
+00003a60: 4369 7461 7469 6f6e 0a0a 4966 2079 6f75  Citation..If you
+00003a70: 2075 7365 2050 6778 2069 6e20 796f 7572   use Pgx in your
+00003a80: 2077 6f72 6b2c 2070 6c65 6173 6520 6369   work, please ci
+00003a90: 7465 2074 6865 2066 6f6c 6c6f 7769 6e67  te the following
+00003aa0: 2070 6170 6572 3a0a 0a60 6060 0a40 6172   paper:..```.@ar
+00003ab0: 7469 636c 657b 6b6f 7961 6d61 6461 3230  ticle{koyamada20
+00003ac0: 3233 7067 782c 0a20 2074 6974 6c65 3d7b  23pgx,.  title={
+00003ad0: 5067 783a 2048 6172 6477 6172 652d 6163  Pgx: Hardware-ac
+00003ae0: 6365 6c65 7261 7465 6420 5061 7261 6c6c  celerated Parall
+00003af0: 656c 2047 616d 6520 5369 6d75 6c61 746f  el Game Simulato
+00003b00: 7273 2066 6f72 2052 6569 6e66 6f72 6365  rs for Reinforce
+00003b10: 6d65 6e74 204c 6561 726e 696e 677d 2c0a  ment Learning},.
+00003b20: 2020 6175 7468 6f72 3d7b 4b6f 7961 6d61    author={Koyama
+00003b30: 6461 2c20 536f 7465 7473 7520 616e 6420  da, Sotetsu and 
+00003b40: 4f6b 616e 6f2c 2053 6869 6e72 6920 616e  Okano, Shinri an
+00003b50: 6420 4e69 7368 696d 6f72 692c 2053 6f69  d Nishimori, Soi
+00003b60: 6368 6972 6f20 616e 6420 4d75 7261 7461  chiro and Murata
+00003b70: 2c20 5975 2061 6e64 2048 6162 6172 612c  , Yu and Habara,
+00003b80: 204b 6569 676f 2061 6e64 204b 6974 612c   Keigo and Kita,
+00003b90: 2048 6172 756b 6120 616e 6420 4973 6869   Haruka and Ishi
+00003ba0: 692c 2053 6869 6e7d 2c0a 2020 6a6f 7572  i, Shin},.  jour
+00003bb0: 6e61 6c3d 7b61 7258 6976 2070 7265 7072  nal={arXiv prepr
+00003bc0: 696e 7420 6172 5869 763a 3233 3033 2e31  int arXiv:2303.1
+00003bd0: 3735 3033 7d2c 0a20 2079 6561 723d 7b32  7503},.  year={2
+00003be0: 3032 337d 0a7d 0a60 6060 0a0a 2323 204c  023}.}.```..## L
+00003bf0: 4943 454e 5345 0a0a 4170 6163 6865 2d32  ICENSE..Apache-2
+00003c00: 2e30 0a                                  .0.
```

### Comparing `pgx-1.0.0/pgx/__init__.py` & `pgx-1.1.0/pgx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pgx._src.visualizer import (
     save_svg,
     save_svg_animation,
     set_visualization_config,
 )
 from pgx.v1 import Env, EnvId, State, available_envs, make
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 __all__ = [
     # v1 api components
     "State",
     "Env",
     "EnvId",
     "make",
```

### Comparing `pgx-1.0.0/pgx/_mahjong/_hand.py` & `pgx-1.1.0/pgx/_mahjong/_hand.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_mahjong/_shanten.py` & `pgx-1.1.0/pgx/_mahjong/_shanten.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_mahjong/_yaku.py` & `pgx-1.1.0/pgx/_mahjong/_yaku.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/api_test.py` & `pgx-1.1.0/pgx/_src/api_test.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/assets/between.npy` & `pgx-1.1.0/pgx/_src/assets/between.npy`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/assets/can_move.npy` & `pgx-1.1.0/pgx/_src/assets/can_move.npy`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/baseline.py` & `pgx-1.1.0/pgx/_src/baseline.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/chess_utils.py` & `pgx-1.1.0/pgx/_src/chess_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/animalshogi.py` & `pgx-1.1.0/pgx/_src/dwg/animalshogi.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/backgammon.py` & `pgx-1.1.0/pgx/_src/dwg/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/bridge_bidding.py` & `pgx-1.1.0/pgx/_src/dwg/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/chess.py` & `pgx-1.1.0/pgx/_src/dwg/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/connect_four.py` & `pgx-1.1.0/pgx/_src/dwg/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/gardner_chess.py` & `pgx-1.1.0/pgx/_src/dwg/gardner_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/go.py` & `pgx-1.1.0/pgx/_src/dwg/go.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/hex.py` & `pgx-1.1.0/pgx/_src/dwg/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/chess/LICENSE` & `pgx-1.1.0/pgx/_src/dwg/images/chess/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/chess/bBishop.svg` & `pgx-1.1.0/pgx/_src/dwg/images/chess/bBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/chess/bKing.svg` & `pgx-1.1.0/pgx/_src/dwg/images/chess/bKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/chess/bKnight.svg` & `pgx-1.1.0/pgx/_src/dwg/images/chess/bKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/chess/bPawn.svg` & `pgx-1.1.0/pgx/_src/dwg/images/chess/bPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/chess/bQueen.svg` & `pgx-1.1.0/pgx/_src/dwg/images/chess/bQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/chess/bRook.svg` & `pgx-1.1.0/pgx/_src/dwg/images/chess/bRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/chess/wBishop.svg` & `pgx-1.1.0/pgx/_src/dwg/images/chess/wBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/chess/wKing.svg` & `pgx-1.1.0/pgx/_src/dwg/images/chess/wKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/chess/wKnight.svg` & `pgx-1.1.0/pgx/_src/dwg/images/chess/wKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/chess/wPawn.svg` & `pgx-1.1.0/pgx/_src/dwg/images/chess/wPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/chess/wQueen.svg` & `pgx-1.1.0/pgx/_src/dwg/images/chess/wQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/chess/wRook.svg` & `pgx-1.1.0/pgx/_src/dwg/images/chess/wRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/1p.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/1p.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/2p.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/2p.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/3p.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/3p.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/4p.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/4p.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/5p.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/5p.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/6p.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/6p.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/7p.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/7p.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/8p.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/8p.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/9p.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/9p.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/b.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/b.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/gd.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/gd.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/oya.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/oya.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/images/sparrow_mahjong/rd.svg` & `pgx-1.1.0/pgx/_src/dwg/images/sparrow_mahjong/rd.svg`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/kuhn_poker.py` & `pgx-1.1.0/pgx/_src/dwg/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/leduc_holdem.py` & `pgx-1.1.0/pgx/_src/dwg/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/othello.py` & `pgx-1.1.0/pgx/_src/dwg/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/play2048.py` & `pgx-1.1.0/pgx/_src/dwg/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/shogi.py` & `pgx-1.1.0/pgx/_src/dwg/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/sparrow_mahjong.py` & `pgx-1.1.0/pgx/_src/dwg/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/dwg/tictactoe.py` & `pgx-1.1.0/pgx/_src/dwg/tictactoe.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/gardner_chess_utils.py` & `pgx-1.1.0/pgx/_src/gardner_chess_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/shogi_utils.py` & `pgx-1.1.0/pgx/_src/shogi_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/struct.py` & `pgx-1.1.0/pgx/_src/struct.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/_src/visualizer.py` & `pgx-1.1.0/pgx/_src/visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,14 +504,44 @@
                     "black",
                     "",
                     "",
                     "white",
                     "black",
                     "",
                 )
+        elif _state.env_id == "mahjong":
+            from pgx._src.dwg.mahjong import _make_mahjong_dwg
+
+            self.config["GRID_SIZE"] = 10
+            self.config["BOARD_WIDTH"] = 70
+            self.config["BOARD_HEIGHT"] = 70
+            self._make_dwg_group = _make_mahjong_dwg  # type:ignore
+            if (
+                self.config["COLOR_THEME"] is None
+                and self.config["COLOR_THEME"] == "dark"
+            ) or self.config["COLOR_THEME"] == "dark":
+                self.config["COLOR_SET"] = ColorSet(
+                    "black",
+                    "darkgray",
+                    "white",
+                    "white",
+                    "#1e1e1e",
+                    "silver",
+                    "",
+                )
+            else:
+                self.config["COLOR_SET"] = ColorSet(
+                    "black",
+                    "white",
+                    "black",
+                    "black",
+                    "white",
+                    "black",
+                    "",
+                )
         elif _state.env_id == "othello":
             from pgx._src.dwg.othello import _make_othello_dwg
 
             self.config["GRID_SIZE"] = 30
             self.config["BOARD_WIDTH"] = 8
             self.config["BOARD_HEIGHT"] = 8
             self._make_dwg_group = _make_othello_dwg  # type:ignore
```

### Comparing `pgx-1.0.0/pgx/animal_shogi.py` & `pgx-1.1.0/pgx/animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/backgammon.py` & `pgx-1.1.0/pgx/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/bridge_bidding.py` & `pgx-1.1.0/pgx/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/chess.py` & `pgx-1.1.0/pgx/chess.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 # 7  6 14 22 30 38 46 54 62
 # 6  5 13 21 29 37 45 53 61
 # 5  4 12 20 28 36 44 52 60
 # 4  3 11 19 27 35 43 51 59
 # 3  2 10 18 26 34 42 50 58
 # 2  1  9 17 25 33 41 49 57
 # 1  0  8 16 24 32 40 48 56
-#    a  b  c  d  e  f  g  f
+#    a  b  c  d  e  f  g  h
 # board index (flipped black view)
 # 8  0  8 16 24 32 40 48 56
 # 7  1  9 17 25 33 41 49 57
 # 6  2 10 18 26 34 42 50 58
 # 5  3 11 19 27 35 43 51 59
 # 4  4 12 20 28 36 44 52 60
 # 3  5 13 21 29 37 45 53 61
@@ -220,15 +220,15 @@
 
     @property
     def id(self) -> v1.EnvId:
         return "chess"
 
     @property
     def version(self) -> str:
-        return "v0"
+        return "v1"
 
     @property
     def num_players(self) -> int:
         return 2
 
 
 def _step(state: State, action: jnp.ndarray):
@@ -351,23 +351,35 @@
     # 可能かどうかの判断はここでは行わない。castlingがlegalでない場合はフィルタされている前提
     # left
     state = state.replace(  # type: ignore
         _board=jax.lax.cond(
             (piece == KING) & (a.from_ == 32) & (a.to == 16),
             lambda: state._board.at[0].set(EMPTY).at[24].set(ROOK),
             lambda: state._board,
-        )
+        ),
+        # update rook position
+        _possible_piece_positions=jax.lax.cond(
+            (piece == KING) & (a.from_ == 32) & (a.to == 16),
+            lambda: state._possible_piece_positions.at[0, 0].set(24),
+            lambda: state._possible_piece_positions,
+        ),
     )
     # right
     state = state.replace(  # type: ignore
         _board=jax.lax.cond(
             (piece == KING) & (a.from_ == 32) & (a.to == 48),
             lambda: state._board.at[56].set(EMPTY).at[40].set(ROOK),
             lambda: state._board,
-        )
+        ),
+        # update rook position
+        _possible_piece_positions=jax.lax.cond(
+            (piece == KING) & (a.from_ == 32) & (a.to == 48),
+            lambda: state._possible_piece_positions.at[0, 14].set(40),
+            lambda: state._possible_piece_positions,
+        ),
     )
     # update my can_castle_xxx_side
     state = state.replace(  # type: ignore
         _can_castle_queen_side=state._can_castle_queen_side.at[0].set(
             jax.lax.select(
                 (a.from_ == 32) | (a.from_ == 0),
                 FALSE,
```

### Comparing `pgx-1.0.0/pgx/connect_four.py` & `pgx-1.1.0/pgx/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/experimental/bridge_bidding.py` & `pgx-1.1.0/pgx/experimental/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/experimental/visualize.py` & `pgx-1.1.0/pgx/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/experimental/wrappers.py` & `pgx-1.1.0/pgx/experimental/wrappers.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/gardner_chess.py` & `pgx-1.1.0/pgx/gardner_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/go.py` & `pgx-1.1.0/pgx/go.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/hex.py` & `pgx-1.1.0/pgx/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/kuhn_poker.py` & `pgx-1.1.0/pgx/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/leduc_holdem.py` & `pgx-1.1.0/pgx/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/othello.py` & `pgx-1.1.0/pgx/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/play2048.py` & `pgx-1.1.0/pgx/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/shogi.py` & `pgx-1.1.0/pgx/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/sparrow_mahjong.py` & `pgx-1.1.0/pgx/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/tic_tac_toe.py` & `pgx-1.1.0/pgx/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx/v1.py` & `pgx-1.1.0/pgx/v1.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/pgx.egg-info/PKG-INFO` & `pgx-1.1.0/pgx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7067 780a  : 2.1.Name: pgx.
-00000020: 5665 7273 696f 6e3a 2031 2e30 2e30 0a53  Version: 1.0.0.S
+00000020: 5665 7273 696f 6e3a 2031 2e31 2e30 0a53  Version: 1.1.0.S
 00000030: 756d 6d61 7279 3a20 4750 552f 5450 552d  ummary: GPU/TPU-
 00000040: 6163 6365 6c65 7261 7465 6420 7061 7261  accelerated para
 00000050: 6c6c 656c 2067 616d 6520 7369 6d75 6c61  llel game simula
 00000060: 746f 7273 2066 6f72 2072 6569 6e66 6f72  tors for reinfor
 00000070: 6365 6d65 6e74 206c 6561 726e 696e 6720  cement learning 
 00000080: 2852 4c29 0a48 6f6d 652d 7061 6765 3a20  (RL).Home-page: 
 00000090: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
@@ -30,1040 +30,932 @@
 000001d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 000001e0: 6d2f 736f 7465 7473 756b 2f70 6778 2f61  m/sotetsuk/pgx/a
 000001f0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
 00000200: 2f63 692e 796d 6c2f 6261 6467 652e 7376  /ci.yml/badge.sv
 00000210: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
 00000220: 7562 2e63 6f6d 2f73 6f74 6574 7375 6b2f  ub.com/sotetsuk/
 00000230: 7067 782f 6163 7469 6f6e 732f 776f 726b  pgx/actions/work
-00000240: 666c 6f77 732f 6369 2e79 6d6c 290a 0a3c  flows/ci.yml)..<
-00000250: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
-00000260: 7222 3e0a 3c69 6d67 2073 7263 3d22 6874  r">.<img src="ht
-00000270: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00000280: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000290: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
-000002a0: 6e2f 646f 6373 2f61 7373 6574 732f 6c6f  n/docs/assets/lo
-000002b0: 676f 2e73 7667 2220 7769 6474 683d 2234  go.svg" width="4
-000002c0: 3025 223e 0a3c 2f64 6976 3e0a 0a41 2063  0%">.</div>..A c
-000002d0: 6f6c 6c65 6374 696f 6e20 6f66 2047 5055  ollection of GPU
-000002e0: 2f54 5055 2d61 6363 656c 6572 6174 6564  /TPU-accelerated
-000002f0: 2070 6172 616c 6c65 6c20 6761 6d65 2073   parallel game s
-00000300: 696d 756c 6174 6f72 7320 666f 7220 7265  imulators for re
-00000310: 696e 666f 7263 656d 656e 7420 6c65 6172  inforcement lear
-00000320: 6e69 6e67 2028 524c 290a 0a3c 6469 7620  ning (RL)..<div 
-00000330: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-00000340: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000350: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00000360: 636f 6e74 656e 742e 636f 6d2f 736f 7465  content.com/sote
-00000370: 7473 756b 2f70 6778 2f6d 6169 6e2f 646f  tsuk/pgx/main/do
-00000380: 6373 2f61 7373 6574 732f 676f 5f64 6172  cs/assets/go_dar
-00000390: 6b2e 6769 6623 6768 2d64 6172 6b2d 6d6f  k.gif#gh-dark-mo
-000003a0: 6465 2d6f 6e6c 7922 2077 6964 7468 3d22  de-only" width="
-000003b0: 3330 2522 3e3c 696d 6720 7372 633d 2268  30%"><img src="h
-000003c0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-000003d0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-000003e0: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-000003f0: 696e 2f64 6f63 732f 6173 7365 7473 2f67  in/docs/assets/g
-00000400: 6f5f 6461 726b 2e67 6966 2367 682d 6461  o_dark.gif#gh-da
-00000410: 726b 2d6d 6f64 652d 6f6e 6c79 2220 7769  rk-mode-only" wi
-00000420: 6474 683d 2233 3025 2220 7374 796c 653d  dth="30%" style=
-00000430: 2274 7261 6e73 666f 726d 3a72 6f74 6174  "transform:rotat
-00000440: 6528 3237 3064 6567 293b 223e 3c69 6d67  e(270deg);"><img
-00000450: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00000460: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000470: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
-00000480: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
-00000490: 7373 6574 732f 676f 5f64 6172 6b2e 6769  ssets/go_dark.gi
-000004a0: 6623 6768 2d64 6172 6b2d 6d6f 6465 2d6f  f#gh-dark-mode-o
-000004b0: 6e6c 7922 2077 6964 7468 3d22 3330 2522  nly" width="30%"
-000004c0: 2073 7479 6c65 3d22 7472 616e 7366 6f72   style="transfor
-000004d0: 6d3a 726f 7461 7465 2839 3064 6567 293b  m:rotate(90deg);
-000004e0: 223e 0a3c 696d 6720 7372 633d 2268 7474  ">.<img src="htt
-000004f0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00000500: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
-00000510: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
-00000520: 2f64 6f63 732f 6173 7365 7473 2f67 6f5f  /docs/assets/go_
-00000530: 6c69 6768 742e 6769 6623 6768 2d6c 6967  light.gif#gh-lig
-00000540: 6874 2d6d 6f64 652d 6f6e 6c79 2220 7769  ht-mode-only" wi
-00000550: 6474 683d 2233 3025 223e 3c69 6d67 2073  dth="30%"><img s
-00000560: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-00000570: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00000580: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
-00000590: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
-000005a0: 6574 732f 676f 5f6c 6967 6874 2e67 6966  ets/go_light.gif
-000005b0: 2367 682d 6c69 6768 742d 6d6f 6465 2d6f  #gh-light-mode-o
-000005c0: 6e6c 7922 2077 6964 7468 3d22 3330 2522  nly" width="30%"
-000005d0: 2073 7479 6c65 3d22 7472 616e 7366 6f72   style="transfor
-000005e0: 6d3a 726f 7461 7465 2832 3730 6465 6729  m:rotate(270deg)
-000005f0: 3b22 3e3c 696d 6720 7372 633d 2268 7474  ;"><img src="htt
-00000600: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00000610: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
-00000620: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
-00000630: 2f64 6f63 732f 6173 7365 7473 2f67 6f5f  /docs/assets/go_
-00000640: 6c69 6768 742e 6769 6623 6768 2d6c 6967  light.gif#gh-lig
-00000650: 6874 2d6d 6f64 652d 6f6e 6c79 2220 7769  ht-mode-only" wi
-00000660: 6474 683d 2233 3025 2220 7374 796c 653d  dth="30%" style=
-00000670: 2274 7261 6e73 666f 726d 3a72 6f74 6174  "transform:rotat
-00000680: 6528 3930 6465 6729 3b22 3e0a 3c2f 6469  e(90deg);">.</di
-00000690: 763e 0a0a f09f 8e89 202a 2a60 7631 2e30  v>...... **`v1.0
-000006a0: 2e30 602a 2a20 6973 2072 656c 6561 7365  .0`** is release
-000006b0: 6421 2028 3230 3233 2e36 2e32 3029 0a0a  d! (2023.6.20)..
-000006c0: 2323 2057 6879 2050 6778 3f0a 0a3c 212d  ## Why Pgx?..<!-
-000006d0: 2d2d 200a 7468 726f 7567 6870 7574 3a20  -- .throughput: 
-000006e0: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-000006f0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00000700: 6d2f 6472 6976 652f 3167 4957 4859 4c4b  m/drive/1gIWHYLK
-00000710: 4278 4532 584b 4468 416c 4559 4b56 6563  BxE2XKDhAlEYKVec
-00000720: 7a33 5747 3463 7a64 7a23 7363 726f 6c6c  z3WG4czdz#scroll
-00000730: 546f 3d56 3151 5a68 5258 6f47 4c38 4b0a  To=V1QZhRXoGL8K.
-00000740: 2d2d 2d3e 0a0a 5b42 7261 785d 2868 7474  --->..[Brax](htt
-00000750: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000760: 676f 6f67 6c65 2f62 7261 7829 2c20 6120  google/brax), a 
-00000770: 5b4a 4158 5d28 6874 7470 733a 2f2f 6769  [JAX](https://gi
-00000780: 7468 7562 2e63 6f6d 2f67 6f6f 676c 652f  thub.com/google/
-00000790: 6a61 7829 2d6e 6174 6976 6520 7068 7973  jax)-native phys
-000007a0: 6963 7320 656e 6769 6e65 2c20 7072 6f76  ics engine, prov
-000007b0: 6964 6573 2065 7874 7265 6d65 6c79 2068  ides extremely h
-000007c0: 6967 682d 7370 6565 6420 7061 7261 6c6c  igh-speed parall
-000007d0: 656c 2073 696d 756c 6174 696f 6e20 666f  el simulation fo
-000007e0: 7220 524c 2069 6e20 2a63 6f6e 7469 6e75  r RL in *continu
-000007f0: 6f75 732a 2073 7461 7465 2073 7061 6365  ous* state space
-00000800: 2e0a 5468 656e 2c20 7768 6174 2061 626f  ..Then, what abo
-00000810: 7574 2052 4c20 696e 202a 6469 7363 7265  ut RL in *discre
-00000820: 7465 2a20 7374 6174 6520 7370 6163 6573  te* state spaces
-00000830: 206c 696b 6520 4368 6573 732c 2053 686f   like Chess, Sho
-00000840: 6769 2c20 616e 6420 476f 3f20 2a2a 5067  gi, and Go? **Pg
-00000850: 782a 2a20 7072 6f76 6964 6573 2061 2077  x** provides a w
-00000860: 6964 6520 7661 7269 6574 7920 6f66 204a  ide variety of J
-00000870: 4158 2d6e 6174 6976 6520 6761 6d65 2073  AX-native game s
-00000880: 696d 756c 6174 6f72 7321 2048 6967 686c  imulators! Highl
-00000890: 6967 6874 6564 2066 6561 7475 7265 7320  ighted features 
-000008a0: 696e 636c 7564 653a 0a0a 2d20 e29a a120  include:..- ... 
-000008b0: 2a2a 5375 7065 7220 6661 7374 2a2a 2069  **Super fast** i
-000008c0: 6e20 7061 7261 6c6c 656c 2065 7865 6375  n parallel execu
-000008d0: 7469 6f6e 206f 6e20 6163 6365 6c65 7261  tion on accelera
-000008e0: 746f 7273 0a2d 20f0 9f8e b220 2a2a 5661  tors.- .... **Va
-000008f0: 7269 6f75 7320 6761 6d65 2073 7570 706f  rious game suppo
-00000900: 7274 2a2a 2069 6e63 6c75 6469 6e67 202a  rt** including *
-00000910: 2a42 6163 6b67 616d 6d6f 6e2a 2a2c 202a  *Backgammon**, *
-00000920: 2a43 6865 7373 2a2a 2c20 2a2a 5368 6f67  *Chess**, **Shog
-00000930: 692a 2a2c 2061 6e64 202a 2a47 6f2a 2a0a  i**, and **Go**.
-00000940: 2d20 f09f 96bc efb8 8f20 2a2a 4265 6175  - ....... **Beau
-00000950: 7469 6675 6c20 7669 7375 616c 697a 6174  tiful visualizat
-00000960: 696f 6e2a 2a20 696e 2053 5647 2066 6f72  ion** in SVG for
-00000970: 6d61 740a 0a0a 2323 2043 6f6c 6162 0a0a  mat...## Colab..
-00000980: 2d20 5b47 6574 7469 6e67 2073 7461 7274  - [Getting start
-00000990: 6564 5d28 6874 7470 733a 2f2f 636f 6c61  ed](https://cola
-000009a0: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
-000009b0: 652e 636f 6d2f 6769 7468 7562 2f73 6f74  e.com/github/sot
-000009c0: 6574 7375 6b2f 7067 782f 626c 6f62 2f6d  etsuk/pgx/blob/m
-000009d0: 6169 6e2f 636f 6c61 622f 7067 785f 6865  ain/colab/pgx_he
-000009e0: 6c6c 6f5f 776f 726c 642e 6970 796e 6229  llo_world.ipynb)
-000009f0: 0a2d 205b 5067 7820 6261 7365 6c69 6e65  .- [Pgx baseline
-00000a00: 206d 6f64 656c 735d 2868 7474 7073 3a2f   models](https:/
-00000a10: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
-00000a20: 676f 6f67 6c65 2e63 6f6d 2f67 6974 6875  google.com/githu
-00000a30: 622f 736f 7465 7473 756b 2f70 6778 2f62  b/sotetsuk/pgx/b
-00000a40: 6c6f 622f 6d61 696e 2f63 6f6c 6162 2f62  lob/main/colab/b
-00000a50: 6173 656c 696e 6573 2e69 7079 6e62 290a  aselines.ipynb).
-00000a60: 2d20 5b50 504f 2065 7861 6d70 6c65 5d28  - [PPO example](
-00000a70: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-00000a80: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00000a90: 6d2f 6769 7468 7562 2f73 6f74 6574 7375  m/github/sotetsu
-00000aa0: 6b2f 7067 782f 626c 6f62 2f6d 6169 6e2f  k/pgx/blob/main/
-00000ab0: 636f 6c61 622f 7070 6f2e 6970 796e 6229  colab/ppo.ipynb)
-00000ac0: 0a2d 205b 4578 706f 7274 2074 6f20 5065  .- [Export to Pe
-00000ad0: 7474 696e 675a 6f6f 2041 5049 5d28 6874  ttingZoo API](ht
-00000ae0: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
-00000af0: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
-00000b00: 6769 7468 7562 2f73 6f74 6574 7375 6b2f  github/sotetsuk/
-00000b10: 7067 782f 626c 6f62 2f6d 6169 6e2f 636f  pgx/blob/main/co
-00000b20: 6c61 622f 7067 7832 7065 7474 696e 677a  lab/pgx2pettingz
-00000b30: 6f6f 2e69 7079 6e62 290a 0a23 2320 496e  oo.ipynb)..## In
-00000b40: 7374 616c 6c61 7469 6f6e 0a0a 6060 6073  stallation..```s
-00000b50: 680a 7069 7020 696e 7374 616c 6c20 7067  h.pip install pg
-00000b60: 780a 6060 600a 0a4e 6f74 6520 7468 6174  x.```..Note that
-00000b70: 2074 6865 205b 4d69 6e41 7461 725d 2868   the [MinAtar](h
-00000b80: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000b90: 6d2f 6b65 6e6a 796f 756e 672f 4d69 6e41  m/kenjyoung/MinA
-00000ba0: 7461 7229 2073 7569 7465 2069 7320 7072  tar) suite is pr
-00000bb0: 6f76 6964 6564 2061 7320 6120 7365 7061  ovided as a sepa
-00000bc0: 7261 7465 2065 7874 656e 7369 6f6e 2066  rate extension f
-00000bd0: 6f72 2050 6778 2028 5b60 7067 782d 6d69  or Pgx ([`pgx-mi
-00000be0: 6e61 7461 7260 5d28 6874 7470 733a 2f2f  natar`](https://
-00000bf0: 6769 7468 7562 2e63 6f6d 2f73 6f74 6574  github.com/sotet
-00000c00: 7375 6b2f 7067 782d 6d69 6e61 7461 7229  suk/pgx-minatar)
-00000c10: 292e 2054 6865 7265 666f 7265 2c20 706c  ). Therefore, pl
-00000c20: 6561 7365 2072 756e 2074 6865 2066 6f6c  ease run the fol
-00000c30: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2061  lowing command a
-00000c40: 6464 6974 696f 6e61 6c79 2074 6f20 7573  dditionaly to us
-00000c50: 6520 7468 6520 4d69 6e41 7461 7220 7375  e the MinAtar su
-00000c60: 6974 6520 696e 2050 6778 3a0a 0a60 6060  ite in Pgx:..```
-00000c70: 7368 0a70 6970 2069 6e73 7461 6c6c 2070  sh.pip install p
-00000c80: 6778 2d6d 696e 6174 6172 0a60 6060 0a0a  gx-minatar.```..
-00000c90: 5067 7820 6973 2070 726f 7669 6465 6420  Pgx is provided 
-00000ca0: 756e 6465 7220 7468 6520 4170 6163 6865  under the Apache
-00000cb0: 2032 2e30 204c 6963 656e 7365 2c20 6275   2.0 License, bu
-00000cc0: 7420 7468 6520 6f72 6967 696e 616c 204d  t the original M
-00000cd0: 696e 4174 6172 2073 7569 7465 2066 6f6c  inAtar suite fol
-00000ce0: 6c6f 7773 2074 6865 2047 504c 2033 2e30  lows the GPL 3.0
-00000cf0: 204c 6963 656e 7365 2e20 5468 6572 6566   License. Theref
-00000d00: 6f72 652c 2070 6c65 6173 6520 6e6f 7465  ore, please note
-00000d10: 2074 6861 7420 7468 6520 7365 7061 7261   that the separa
-00000d20: 7465 6420 4d69 6e41 7461 7220 6578 7465  ted MinAtar exte
-00000d30: 6e73 696f 6e20 666f 7220 5067 7820 616c  nsion for Pgx al
-00000d40: 736f 2061 6468 6572 6573 2074 6f20 7468  so adheres to th
-00000d50: 6520 4750 4c20 332e 3020 4c69 6365 6e73  e GPL 3.0 Licens
-00000d60: 652e 0a0a 2323 2055 7361 6765 0a0a 0a4e  e...## Usage...N
-00000d70: 6f74 6520 7468 6174 2061 6c6c 2060 7374  ote that all `st
-00000d80: 6570 6020 6675 6e63 7469 6f6e 7320 696e  ep` functions in
-00000d90: 2050 6778 2065 6e76 6972 6f6e 6d65 6e74   Pgx environment
-00000da0: 7320 6172 6520 2a2a 4a41 582d 6e61 7469  s are **JAX-nati
-00000db0: 7665 2e2a 2a2c 2069 2e65 2e2c 2074 6865  ve.**, i.e., the
-00000dc0: 7920 6172 6520 616c 6c20 2a4a 4954 2d61  y are all *JIT-a
-00000dd0: 626c 652a 2e0a 0a3c 6120 6872 6566 3d22  ble*...<a href="
-00000de0: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-00000df0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00000e00: 6d2f 6769 7468 7562 2f73 6f74 6574 7375  m/github/sotetsu
-00000e10: 6b2f 7067 782f 626c 6f62 2f6d 6169 6e2f  k/pgx/blob/main/
-00000e20: 636f 6c61 622f 7067 785f 6865 6c6c 6f5f  colab/pgx_hello_
-00000e30: 776f 726c 642e 6970 796e 6222 3e3c 696d  world.ipynb"><im
-00000e40: 6720 7372 633d 2268 7474 7073 3a2f 2f63  g src="https://c
-00000e50: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
-00000e60: 6f67 6c65 2e63 6f6d 2f61 7373 6574 732f  ogle.com/assets/
-00000e70: 636f 6c61 622d 6261 6467 652e 7376 6722  colab-badge.svg"
-00000e80: 2061 6c74 3d22 4f70 656e 2049 6e20 436f   alt="Open In Co
-00000e90: 6c61 6222 2f3e 3c2f 613e 0a0a 6060 6070  lab"/></a>..```p
-00000ea0: 790a 696d 706f 7274 206a 6178 0a69 6d70  y.import jax.imp
-00000eb0: 6f72 7420 7067 780a 0a65 6e76 203d 2070  ort pgx..env = p
-00000ec0: 6778 2e6d 616b 6528 2267 6f5f 3139 7831  gx.make("go_19x1
-00000ed0: 3922 290a 696e 6974 203d 206a 6178 2e6a  9").init = jax.j
-00000ee0: 6974 286a 6178 2e76 6d61 7028 656e 762e  it(jax.vmap(env.
-00000ef0: 696e 6974 2929 2020 2320 7665 6374 6f72  init))  # vector
-00000f00: 697a 6520 616e 6420 4a49 542d 636f 6d70  ize and JIT-comp
-00000f10: 696c 650a 7374 6570 203d 206a 6178 2e6a  ile.step = jax.j
-00000f20: 6974 286a 6178 2e76 6d61 7028 656e 762e  it(jax.vmap(env.
-00000f30: 7374 6570 2929 0a0a 6261 7463 685f 7369  step))..batch_si
-00000f40: 7a65 203d 2031 3032 340a 6b65 7973 203d  ze = 1024.keys =
-00000f50: 206a 6178 2e72 616e 646f 6d2e 7370 6c69   jax.random.spli
-00000f60: 7428 6a61 782e 7261 6e64 6f6d 2e50 524e  t(jax.random.PRN
-00000f70: 474b 6579 2834 3229 2c20 6261 7463 685f  GKey(42), batch_
-00000f80: 7369 7a65 290a 7374 6174 6520 3d20 696e  size).state = in
-00000f90: 6974 286b 6579 7329 2020 2320 7665 6374  it(keys)  # vect
-00000fa0: 6f72 697a 6564 2073 7461 7465 730a 7768  orized states.wh
-00000fb0: 696c 6520 6e6f 7420 2873 7461 7465 2e74  ile not (state.t
-00000fc0: 6572 6d69 6e61 7465 6420 7c20 7374 6174  erminated | stat
-00000fd0: 652e 7472 756e 6361 7465 6429 2e61 6c6c  e.truncated).all
-00000fe0: 2829 3a0a 2020 2020 6163 7469 6f6e 203d  ():.    action =
-00000ff0: 206d 6f64 656c 2873 7461 7465 2e63 7572   model(state.cur
-00001000: 7265 6e74 5f70 6c61 7965 722c 2073 7461  rent_player, sta
-00001010: 7465 2e6f 6273 6572 7661 7469 6f6e 2c20  te.observation, 
-00001020: 7374 6174 652e 6c65 6761 6c5f 6163 7469  state.legal_acti
-00001030: 6f6e 5f6d 6173 6b29 0a20 2020 2073 7461  on_mask).    sta
-00001040: 7465 203d 2073 7465 7028 7374 6174 652c  te = step(state,
-00001050: 2061 6374 696f 6e29 2020 2320 7374 6174   action)  # stat
-00001060: 652e 7265 7761 7264 2028 322c 290a 6060  e.reward (2,).``
-00001070: 600a 0a50 6778 2069 7320 6120 6c69 6272  `..Pgx is a libr
-00001080: 6172 7920 7468 6174 2066 6f63 7573 6573  ary that focuses
-00001090: 206f 6e20 6661 7374 6572 2069 6d70 6c65   on faster imple
-000010a0: 6d65 6e74 6174 696f 6e73 2072 6174 6865  mentations rathe
-000010b0: 7220 7468 616e 206a 7573 7420 7468 6520  r than just the 
-000010c0: 4150 4920 6974 7365 6c66 2e20 0a48 6f77  API itself. .How
-000010d0: 6576 6572 2c20 7468 6520 4150 4920 6974  ever, the API it
-000010e0: 7365 6c66 2069 7320 616c 736f 2073 7566  self is also suf
-000010f0: 6669 6369 656e 746c 7920 6765 6e65 7261  ficiently genera
-00001100: 6c2e 2046 6f72 2065 7861 6d70 6c65 2c20  l. For example, 
-00001110: 616c 6c20 656e 7669 726f 6e6d 656e 7473  all environments
-00001120: 2069 6e20 5067 7820 6361 6e20 6265 2063   in Pgx can be c
-00001130: 6f6e 7665 7274 6564 2074 6f20 7468 6520  onverted to the 
-00001140: 4145 4320 4150 4920 6f66 205b 5065 7474  AEC API of [Pett
-00001150: 696e 675a 6f6f 5d28 6874 7470 733a 2f2f  ingZoo](https://
-00001160: 6769 7468 7562 2e63 6f6d 2f46 6172 616d  github.com/Faram
-00001170: 612d 466f 756e 6461 7469 6f6e 2f50 6574  a-Foundation/Pet
-00001180: 7469 6e67 5a6f 6f29 2c20 616e 6420 796f  tingZoo), and yo
-00001190: 7520 6361 6e20 7275 6e20 5067 7820 656e  u can run Pgx en
-000011a0: 7669 726f 6e6d 656e 7473 2074 6872 6f75  vironments throu
-000011b0: 6768 2074 6865 2050 6574 7469 6e67 5a6f  gh the PettingZo
-000011c0: 6f20 4150 492e 0a59 6f75 2063 616e 2073  o API..You can s
-000011d0: 6565 2074 6865 2064 656d 6f6e 7374 7261  ee the demonstra
-000011e0: 7469 6f6e 2069 6e20 476f 6f67 6c65 2043  tion in Google C
-000011f0: 6f6c 6162 3a0a 0a3c 6120 6872 6566 3d22  olab:..<a href="
-00001200: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-00001210: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00001220: 6d2f 6769 7468 7562 2f73 6f74 6574 7375  m/github/sotetsu
-00001230: 6b2f 7067 782f 626c 6f62 2f6d 6169 6e2f  k/pgx/blob/main/
-00001240: 636f 6c61 622f 7067 7832 7065 7474 696e  colab/pgx2pettin
-00001250: 677a 6f6f 2e69 7079 6e62 223e 3c69 6d67  gzoo.ipynb"><img
-00001260: 2073 7263 3d22 6874 7470 733a 2f2f 636f   src="https://co
-00001270: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00001280: 676c 652e 636f 6d2f 6173 7365 7473 2f63  gle.com/assets/c
-00001290: 6f6c 6162 2d62 6164 6765 2e73 7667 2220  olab-badge.svg" 
-000012a0: 616c 743d 224f 7065 6e20 496e 2043 6f6c  alt="Open In Col
-000012b0: 6162 222f 3e3c 2f61 3e0a 0a3c 212d 2d2d  ab"/></a>..<!---
-000012c0: 0a23 2323 204c 696d 6974 6174 696f 6e73  .### Limitations
-000012d0: 2028 666f 7220 7468 6520 7369 6d70 6c69   (for the simpli
-000012e0: 6369 7479 290a 2a20 446f 6573 202a 2a4e  city).* Does **N
-000012f0: 4f54 2a2a 2073 7570 706f 7274 2061 6765  OT** support age
-00001300: 6e74 2064 6561 7468 2061 6e64 2063 7265  nt death and cre
-00001310: 6174 696f 6e2c 2077 6869 6368 2064 796e  ation, which dyn
-00001320: 6d69 6361 6c6c 7920 6368 616e 6765 7320  mically changes 
-00001330: 7468 6520 6172 7261 7920 7369 7a65 2e20  the array size. 
-00001340: 4974 2064 6f65 7320 6e6f 7420 7765 6c6c  It does not well
-00001350: 2073 7569 7420 746f 2047 5055 2d61 6363   suit to GPU-acc
-00001360: 656c 6572 6174 6564 2063 6f6d 7075 7461  elerated computa
-00001370: 7469 6f6e 2e0a 2a20 446f 6573 202a 2a4e  tion..* Does **N
-00001380: 4f54 2a2a 2073 7570 706f 7274 2043 6861  OT** support Cha
-00001390: 6e63 6520 706c 6179 6572 2028 4e61 7475  nce player (Natu
-000013a0: 7265 2070 6c61 7965 7229 2077 6974 6820  re player) with 
-000013b0: 6163 7469 6f6e 2073 656c 6563 7469 6f6e  action selection
-000013c0: 2e0a 2a20 446f 6573 202a 2a4e 4f54 2a2a  ..* Does **NOT**
-000013d0: 2073 7570 706f 7274 204f 7065 6e41 4920   support OpenAI 
-000013e0: 4779 6d20 4150 492e 0a20 2020 202a 204f  Gym API..    * O
-000013f0: 7065 6e41 4920 4779 6d20 6973 2066 6f72  penAI Gym is for
-00001400: 2073 696e 676c 652d 6167 656e 7420 656e   single-agent en
-00001410: 7669 726f 6e6d 656e 742e 204d 6f73 7420  vironment. Most 
-00001420: 6f66 2050 6778 2065 6e76 6972 6f6e 6d65  of Pgx environme
-00001430: 6e74 7320 6172 6520 6d75 6c74 692d 706c  nts are multi-pl
-00001440: 6179 6572 2067 616d 6573 2e20 4a75 7374  ayer games. Just
-00001450: 2064 6566 696e 696e 6720 6f70 706f 6e65   defining oppone
-00001460: 6e74 7320 6973 206e 6f74 2065 6e6f 7567  nts is not enoug
-00001470: 6820 666f 7220 636f 6e76 6572 7469 6e67  h for converting
-00001480: 206d 756c 7469 2d61 6765 6e74 2065 6e76   multi-agent env
-00001490: 6972 6f6e 656d 6e74 7320 746f 204f 7065  ironemnts to Ope
-000014a0: 6e41 4920 4779 6d20 656e 7669 726f 6e6d  nAI Gym environm
-000014b0: 656e 742e 2045 2e67 2e2c 2069 6e20 7468  ent. E.g., in th
-000014c0: 6520 6761 6d65 206f 6620 676f 2c20 7468  e game of go, th
-000014d0: 6520 6e65 7874 2073 7461 7465 2073 2720  e next state s' 
-000014e0: 6973 2064 6566 696e 6564 2061 7320 7468  is defined as th
-000014f0: 6520 7374 6174 6520 6a75 7374 2061 6674  e state just aft
-00001500: 6572 2070 6c61 6369 6e67 2061 2073 746f  er placing a sto
-00001510: 6e65 2069 6e20 416c 6861 476f 2070 6170  ne in AlhaGo pap
-00001520: 6572 2e20 486f 7765 7665 722c 2073 2720  er. However, s' 
-00001530: 6265 636f 6d65 7320 7468 6520 7374 6174  becomes the stat
-00001540: 6520 6166 7465 7220 7468 6520 6f70 706f  e after the oppo
-00001550: 6e65 6e74 7327 2070 6c61 792e 2054 6869  nents' play. Thi
-00001560: 7320 6368 616e 6765 7320 7468 6520 6465  s changes the de
-00001570: 6669 6e69 7469 6f6e 206f 6620 5628 7327  finition of V(s'
-00001580: 292e 0a2a 2044 6f65 7320 2a2a 4e4f 542a  )..* Does **NOT*
-00001590: 2a20 7375 7070 6f72 7420 5065 7474 696e  * support Pettin
-000015a0: 675a 6f6f 2041 5049 2e0a 2020 2020 2a20  gZoo API..    * 
-000015b0: 5065 7474 696e 675a 6f6f 2069 7320 2a47  PettingZoo is *G
-000015c0: 796d 2066 6f72 206d 756c 7469 2d61 6765  ym for multi-age
-000015d0: 6e74 2052 4c2a 2e20 4173 2066 6172 2061  nt RL*. As far a
-000015e0: 7320 7765 206b 6e6f 772c 2050 6574 7469  s we know, Petti
-000015f0: 6e67 5a6f 6f20 646f 6573 206e 6f74 2073  ngZoo does not s
-00001600: 7570 706f 7274 2076 6563 746f 7269 7a65  upport vectorize
-00001610: 6420 656e 7669 726f 6e6d 656e 7473 2028  d environments (
-00001620: 6c69 6b65 2056 6563 746f 7245 6e76 2069  like VectorEnv i
-00001630: 6e20 4f70 656e 4149 2047 796d 292e 2041  n OpenAI Gym). A
-00001640: 7320 5067 7827 7320 6d61 696e 2066 6561  s Pgx's main fea
-00001650: 7475 7265 2069 7320 6869 6768 6c79 2076  ture is highly v
-00001660: 6563 746f 7269 7a65 6420 656e 7669 726f  ectorized enviro
-00001670: 6e6d 656e 7420 7669 6120 4750 552f 5450  nment via GPU/TP
-00001680: 5520 7375 7070 6f72 742c 2057 6520 646f  U support, We do
-00001690: 206e 6f74 2063 7572 7265 6e74 6c79 2073   not currently s
-000016a0: 7570 706f 7274 2050 6574 7469 6e67 5a6f  upport PettingZo
-000016b0: 6f20 4150 492e 200a 0a23 2323 2060 736b  o API. ..### `sk
-000016c0: 6970 5f63 6861 6e63 6560 0a2a 2057 6520  ip_chance`.* We 
-000016d0: 7072 6570 6172 6520 736b 6970 5f63 6861  prepare skip_cha
-000016e0: 6e63 653d 5472 7565 206f 7074 696f 6e20  nce=True option 
-000016f0: 666f 7220 736f 6d65 2065 6e76 6972 6f6e  for some environ
-00001700: 6d65 6e74 732e 2054 6869 7320 6d61 6b65  ments. This make
-00001710: 7320 6974 2070 6f73 7369 626c 6520 746f  s it possible to
-00001720: 2063 6f6e 7369 6465 7220 7661 6c75 6520   consider value 
-00001730: 6675 6e63 7469 6f6e 2066 6f72 2022 706f  function for "po
-00001740: 7374 2d64 6563 6973 696f 6e20 7374 6174  st-decision stat
-00001750: 6573 2220 2853 6565 2041 6c67 6f52 4c20  es" (See AlgoRL 
-00001760: 626f 6f6b 292e 2048 6f77 6576 6572 2c20  book). However, 
-00001770: 7765 2064 6f20 6e6f 7420 616c 6c6f 7720  we do not allow 
-00001780: 6368 616e 6365 2061 6765 6e74 2074 6f20  chance agent to 
-00001790: 6368 6f6f 7365 2061 6374 696f 6e20 6c69  choose action li
-000017a0: 6b65 204f 7065 6e53 7069 656c 2e20 5468  ke OpenSpiel. Th
-000017b0: 6973 2069 7320 6265 6361 7573 6520 7468  is is because th
-000017c0: 6520 6163 7469 6f6e 2073 7061 6365 206f  e action space o
-000017d0: 6620 6368 616e 6365 2061 6765 6e74 2061  f chance agent a
-000017e0: 6e64 2075 7375 616c 2061 6765 6e74 2061  nd usual agent a
-000017f0: 7265 2064 6966 6665 7265 6e74 2e20 5468  re different. Th
-00001800: 7573 2c20 7768 656e 2074 6865 2063 6861  us, when the cha
-00001810: 6e63 6520 706c 6179 6572 2069 7320 6368  nce player is ch
-00001820: 6f73 656e 2028 6063 7572 7265 6e74 5f70  osen (`current_p
-00001830: 6c61 7965 723d 2d31 6029 2c20 6061 6374  layer=-1`), `act
-00001840: 696f 6e3d 2d31 6020 6d75 7374 2062 6520  ion=-1` must be 
-00001850: 7265 7475 726e 6564 2074 6f20 7374 6570  returned to step
-00001860: 2066 756e 6374 696f 6e2e 2055 7365 2060   function. Use `
-00001870: 7368 7566 666c 6560 2074 6f20 6d61 6b65  shuffle` to make
-00001880: 2060 7374 6570 6020 7374 6f63 6861 7374   `step` stochast
-00001890: 6963 2e0a 0a23 2323 2074 7275 6e63 6174  ic...### truncat
-000018a0: 6174 696f 6e20 616e 6420 6175 746f 5f72  ation and auto_r
-000018b0: 6573 6574 0a2a 2073 7570 706f 7274 6564  eset.* supported
-000018c0: 2062 7920 606d 616b 6528 656e 765f 6964   by `make(env_id
-000018d0: 3d22 2e2e 2e22 2c20 6175 746f 5f72 6573  ="...", auto_res
-000018e0: 6574 3d54 7275 652c 206d 6178 5f65 7069  et=True, max_epi
-000018f0: 736f 6465 5f6c 656e 6774 683d 3634 2960  sode_length=64)`
-00001900: 0a2a 2060 6175 746f 5f72 6573 6574 6020  .* `auto_reset` 
-00001910: 7769 6c6c 2072 6570 6c61 6365 2074 6865  will replace the
-00001920: 2074 6572 6d69 6e61 6c20 7374 6174 6520   terminal state 
-00001930: 6279 2069 6e69 7469 616c 2073 7461 7465  by initial state
-00001940: 2028 6275 7420 6069 735f 7465 726d 696e   (but `is_termin
-00001950: 616c 3d54 7275 6560 2069 7320 7365 7429  al=True` is set)
-00001960: 0a2a 2060 6973 5f74 7275 6e63 6174 6564  .* `is_truncated
-00001970: 3d54 7275 6560 2069 7320 616c 736f 2073  =True` is also s
-00001980: 6574 2074 6f20 7374 6174 650a 2d2d 2d3e  et to state.--->
-00001990: 0a0a 2323 2053 7570 706f 7274 6564 2067  ..## Supported g
-000019a0: 616d 6573 0a0a 7c20 4261 636b 6761 6d6d  ames..| Backgamm
-000019b0: 6f6e 207c 2043 6865 7373 207c 2053 686f  on | Chess | Sho
-000019c0: 6769 207c 2047 6f20 7c0a 7c3a 2d2d 2d3a  gi | Go |.|:---:
-000019d0: 7c3a 2d2d 2d3a 7c3a 2d2d 2d3a 7c3a 2d2d  |:---:|:---:|:--
-000019e0: 2d3a 7c0a 7c3c 696d 6720 7372 633d 2268  -:|.|<img src="h
-000019f0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00001a00: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00001a10: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-00001a20: 696e 2f64 6f63 732f 6173 7365 7473 2f62  in/docs/assets/b
-00001a30: 6163 6b67 616d 6d6f 6e5f 6461 726b 2e67  ackgammon_dark.g
-00001a40: 6966 2367 682d 6461 726b 2d6d 6f64 652d  if#gh-dark-mode-
-00001a50: 6f6e 6c79 2220 7769 6474 683d 2231 3730  only" width="170
-00001a60: 7078 223e 3c69 6d67 2073 7263 3d22 6874  px"><img src="ht
-00001a70: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00001a80: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00001a90: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
-00001aa0: 6e2f 646f 6373 2f61 7373 6574 732f 6261  n/docs/assets/ba
-00001ab0: 636b 6761 6d6d 6f6e 5f6c 6967 6874 2e67  ckgammon_light.g
-00001ac0: 6966 2367 682d 6c69 6768 742d 6d6f 6465  if#gh-light-mode
-00001ad0: 2d6f 6e6c 7922 2077 6964 7468 3d22 3137  -only" width="17
-00001ae0: 3070 7822 3e7c 3c69 6d67 2073 7263 3d22  0px">|<img src="
-00001af0: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00001b00: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00001b10: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
-00001b20: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
-00001b30: 6368 6573 735f 6461 726b 2e67 6966 2367  chess_dark.gif#g
-00001b40: 682d 6461 726b 2d6d 6f64 652d 6f6e 6c79  h-dark-mode-only
-00001b50: 2220 7769 6474 683d 2231 3538 7078 223e  " width="158px">
-00001b60: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001b70: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00001b80: 636f 6e74 656e 742e 636f 6d2f 736f 7465  content.com/sote
-00001b90: 7473 756b 2f70 6778 2f6d 6169 6e2f 646f  tsuk/pgx/main/do
-00001ba0: 6373 2f61 7373 6574 732f 6368 6573 735f  cs/assets/chess_
-00001bb0: 6c69 6768 742e 6769 6623 6768 2d6c 6967  light.gif#gh-lig
-00001bc0: 6874 2d6d 6f64 652d 6f6e 6c79 2220 7769  ht-mode-only" wi
-00001bd0: 6474 683d 2231 3538 7078 223e 7c3c 696d  dth="158px">|<im
-00001be0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00001bf0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00001c00: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00001c10: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-00001c20: 6173 7365 7473 2f73 686f 6769 5f64 6172  assets/shogi_dar
-00001c30: 6b2e 6769 6623 6768 2d64 6172 6b2d 6d6f  k.gif#gh-dark-mo
-00001c40: 6465 2d6f 6e6c 7922 2077 6964 7468 3d22  de-only" width="
-00001c50: 3137 3070 7822 3e3c 696d 6720 7372 633d  170px"><img src=
-00001c60: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00001c70: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00001c80: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
-00001c90: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
-00001ca0: 2f73 686f 6769 5f6c 6967 6874 2e67 6966  /shogi_light.gif
-00001cb0: 2367 682d 6c69 6768 742d 6d6f 6465 2d6f  #gh-light-mode-o
-00001cc0: 6e6c 7922 2077 6964 7468 3d22 3137 3070  nly" width="170p
-00001cd0: 7822 3e7c 3c69 6d67 2073 7263 3d22 6874  x">|<img src="ht
-00001ce0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00001cf0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00001d00: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
-00001d10: 6e2f 646f 6373 2f61 7373 6574 732f 676f  n/docs/assets/go
-00001d20: 2d31 3978 3139 5f64 6172 6b2e 6769 6623  -19x19_dark.gif#
-00001d30: 6768 2d64 6172 6b2d 6d6f 6465 2d6f 6e6c  gh-dark-mode-onl
-00001d40: 7922 2077 6964 7468 3d22 3136 3070 7822  y" width="160px"
-00001d50: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00001d60: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00001d70: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
-00001d80: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
-00001d90: 6f63 732f 6173 7365 7473 2f67 6f2d 3139  ocs/assets/go-19
-00001da0: 7831 395f 6c69 6768 742e 6769 6623 6768  x19_light.gif#gh
-00001db0: 2d6c 6967 6874 2d6d 6f64 652d 6f6e 6c79  -light-mode-only
-00001dc0: 2220 7769 6474 683d 2231 3630 7078 223e  " width="160px">
-00001dd0: 7c0a 0a0a 5573 6520 6070 6778 2e61 7661  |...Use `pgx.ava
-00001de0: 696c 6162 6c65 5f65 6e76 7328 2920 2d3e  ilable_envs() ->
-00001df0: 2054 7570 6c65 5b45 6e76 4964 5d60 2074   Tuple[EnvId]` t
-00001e00: 6f20 7365 6520 7468 6520 6c69 7374 206f  o see the list o
-00001e10: 6620 6375 7272 656e 746c 7920 6176 6169  f currently avai
-00001e20: 6c61 626c 6520 6761 6d65 732e 2047 6976  lable games. Giv
-00001e30: 656e 2061 6e20 603c 456e 7649 643e 602c  en an `<EnvId>`,
-00001e40: 2079 6f75 2063 616e 2063 7265 6174 6520   you can create 
-00001e50: 7468 6520 656e 7669 726f 6e6d 656e 7420  the environment 
-00001e60: 7669 610a 0a60 6060 7079 0a3e 3e3e 2065  via..```py.>>> e
-00001e70: 6e76 203d 2070 6778 2e6d 616b 6528 3c45  nv = pgx.make(<E
-00001e80: 6e76 4964 3e29 0a60 6060 0a0a 7c20 4761  nvId>).```..| Ga
-00001e90: 6d65 2f45 6e76 4964 207c 2056 6973 7561  me/EnvId | Visua
-00001ea0: 6c69 7a61 7469 6f6e 207c 2056 6572 7369  lization | Versi
-00001eb0: 6f6e 207c 2046 6976 652d 776f 7264 2064  on | Five-word d
-00001ec0: 6573 6372 6970 7469 6f6e 207c 0a7c 3a2d  escription |.|:-
-00001ed0: 2d2d 3a7c 3a2d 2d2d 3a7c 3a2d 2d2d 3a7c  --:|:---:|:---:|
-00001ee0: 3a2d 2d2d 3a7c 0a7c 3c61 2068 7265 663d  :---:|.|<a href=
-00001ef0: 2268 7474 7073 3a2f 2f65 6e2e 7769 6b69  "https://en.wiki
-00001f00: 7065 6469 612e 6f72 672f 7769 6b69 2f32  pedia.org/wiki/2
-00001f10: 3034 385f 2876 6964 656f 5f67 616d 6529  048_(video_game)
-00001f20: 223e 3230 3438 3c2f 613e 203c 6272 3e20  ">2048</a> <br> 
-00001f30: 6022 3230 3438 2260 207c 3c69 6d67 2073  `"2048"` |<img s
-00001f40: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-00001f50: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00001f60: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
-00001f70: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
-00001f80: 6574 732f 3230 3438 5f64 6172 6b2e 6769  ets/2048_dark.gi
-00001f90: 6622 2077 6964 7468 3d22 3630 7078 223e  f" width="60px">
-00001fa0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001fb0: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00001fc0: 636f 6e74 656e 742e 636f 6d2f 736f 7465  content.com/sote
-00001fd0: 7473 756b 2f70 6778 2f6d 6169 6e2f 646f  tsuk/pgx/main/do
-00001fe0: 6373 2f61 7373 6574 732f 3230 3438 5f6c  cs/assets/2048_l
-00001ff0: 6967 6874 2e67 6966 2220 7769 6474 683d  ight.gif" width=
-00002000: 2236 3070 7822 3e7c 2060 7630 6020 7c20  "60px">| `v0` | 
-00002010: 2a4d 6572 6765 2074 696c 6573 2074 6f20  *Merge tiles to 
-00002020: 6372 6561 7465 2032 3034 382e 2a20 7c0a  create 2048.* |.
-00002030: 7c3c 6120 6872 6566 3d22 6874 7470 733a  |<a href="https:
-00002040: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00002050: 7267 2f77 696b 692f 4425 4335 2538 4462  rg/wiki/D%C5%8Db
-00002060: 7574 7375 5f73 6825 4335 2538 4467 6922  utsu_sh%C5%8Dgi"
-00002070: 3e41 6e69 6d61 6c20 5368 6f67 693c 2f61  >Animal Shogi</a
-00002080: 3e3c 6272 3e60 2261 6e69 6d61 6c5f 7368  ><br>`"animal_sh
-00002090: 6f67 6922 6020 7c3c 696d 6720 7372 633d  ogi"` |<img src=
-000020a0: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-000020b0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-000020c0: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
-000020d0: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
-000020e0: 2f61 6e69 6d61 6c5f 7368 6f67 695f 6461  /animal_shogi_da
-000020f0: 726b 2e67 6966 2220 7769 6474 683d 2236  rk.gif" width="6
-00002100: 3070 7822 3e3c 696d 6720 7372 633d 2268  0px"><img src="h
-00002110: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00002120: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00002130: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-00002140: 696e 2f64 6f63 732f 6173 7365 7473 2f61  in/docs/assets/a
-00002150: 6e69 6d61 6c5f 7368 6f67 695f 6c69 6768  nimal_shogi_ligh
-00002160: 742e 6769 6622 2077 6964 7468 3d22 3630  t.gif" width="60
-00002170: 7078 223e 7c20 2060 7630 6020 7c20 2a41  px">|  `v0` | *A
-00002180: 6e69 6d61 6c2d 7468 656d 6564 2063 6869  nimal-themed chi
-00002190: 6c64 2d66 7269 656e 646c 7920 7368 6f67  ld-friendly shog
-000021a0: 692e 2a20 7c0a 7c3c 6120 6872 6566 3d22  i.* |.|<a href="
-000021b0: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-000021c0: 6564 6961 2e6f 7267 2f77 696b 692f 4261  edia.org/wiki/Ba
-000021d0: 636b 6761 6d6d 6f6e 223e 4261 636b 6761  ckgammon">Backga
-000021e0: 6d6d 6f6e 3c2f 613e 3c62 723e 6022 6261  mmon</a><br>`"ba
-000021f0: 636b 6761 6d6d 6f6e 2260 207c 3c69 6d67  ckgammon"` |<img
-00002200: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00002210: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00002220: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
-00002230: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
-00002240: 7373 6574 732f 6261 636b 6761 6d6d 6f6e  ssets/backgammon
-00002250: 5f64 6172 6b2e 6769 6622 2077 6964 7468  _dark.gif" width
-00002260: 3d22 3630 7078 223e 3c69 6d67 2073 7263  ="60px"><img src
-00002270: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00002280: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00002290: 636f 6d2f 736f 7465 7473 756b 2f70 6778  com/sotetsuk/pgx
-000022a0: 2f6d 6169 6e2f 646f 6373 2f61 7373 6574  /main/docs/asset
-000022b0: 732f 6261 636b 6761 6d6d 6f6e 5f6c 6967  s/backgammon_lig
-000022c0: 6874 2e67 6966 2220 7769 6474 683d 2236  ht.gif" width="6
-000022d0: 3070 7822 3e7c 2060 7630 6020 7c20 2a4c  0px">| `v0` | *L
-000022e0: 7563 6b20 6169 6473 2062 6561 7269 6e67  uck aids bearing
-000022f0: 206f 6666 2063 6865 636b 6572 732e 2a20   off checkers.* 
-00002300: 7c0a 7c3c 6120 6872 6566 3d22 6874 7470  |.|<a href="http
-00002310: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
-00002320: 2e6f 7267 2f77 696b 692f 436f 6e74 7261  .org/wiki/Contra
-00002330: 6374 5f62 7269 6467 6522 3e42 7269 6467  ct_bridge">Bridg
-00002340: 6520 6269 6464 696e 673c 2f61 3e3c 6272  e bidding</a><br
-00002350: 3e60 2262 7269 6467 655f 6269 6464 696e  >`"bridge_biddin
-00002360: 6722 6020 7c3c 696d 6720 7372 633d 2268  g"` |<img src="h
-00002370: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00002380: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00002390: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-000023a0: 696e 2f64 6f63 732f 6173 7365 7473 2f62  in/docs/assets/b
-000023b0: 7269 6467 655f 6269 6464 696e 675f 6461  ridge_bidding_da
-000023c0: 726b 2e67 6966 2220 7769 6474 683d 2236  rk.gif" width="6
-000023d0: 3070 7822 3e3c 696d 6720 7372 633d 2268  0px"><img src="h
-000023e0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-000023f0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00002400: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-00002410: 696e 2f64 6f63 732f 6173 7365 7473 2f62  in/docs/assets/b
-00002420: 7269 6467 655f 6269 6464 696e 675f 6c69  ridge_bidding_li
-00002430: 6768 742e 6769 6622 2077 6964 7468 3d22  ght.gif" width="
-00002440: 3630 7078 223e 7c20 6076 3060 207c 202a  60px">| `v0` | *
-00002450: 5061 7274 6e65 7273 2065 7863 6861 6e67  Partners exchang
-00002460: 6520 696e 666f 726d 6174 696f 6e20 7669  e information vi
-00002470: 6120 6269 6473 2e2a 207c 0a7c 3c61 2068  a bids.* |.|<a h
-00002480: 7265 663d 2268 7474 7073 3a2f 2f65 6e2e  ref="https://en.
-00002490: 7769 6b69 7065 6469 612e 6f72 672f 7769  wikipedia.org/wi
-000024a0: 6b69 2f43 6865 7373 223e 4368 6573 733c  ki/Chess">Chess<
-000024b0: 2f61 3e3c 6272 3e60 2263 6865 7373 2260  /a><br>`"chess"`
-000024c0: 207c 3c69 6d67 2073 7263 3d22 6874 7470   |<img src="http
-000024d0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-000024e0: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
-000024f0: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
-00002500: 646f 6373 2f61 7373 6574 732f 6368 6573  docs/assets/ches
-00002510: 735f 6461 726b 2e67 6966 2220 7769 6474  s_dark.gif" widt
-00002520: 683d 2236 3070 7822 3e3c 696d 6720 7372  h="60px"><img sr
-00002530: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
-00002540: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00002550: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
-00002560: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
-00002570: 7473 2f63 6865 7373 5f6c 6967 6874 2e67  ts/chess_light.g
-00002580: 6966 2220 7769 6474 683d 2236 3070 7822  if" width="60px"
-00002590: 3e7c 2060 7630 6020 7c20 2a43 6865 636b  >| `v0` | *Check
-000025a0: 6d61 7465 206f 7070 6f6e 656e 7427 7320  mate opponent's 
-000025b0: 6b69 6e67 2074 6f20 7769 6e2e 2a20 7c0a  king to win.* |.
-000025c0: 7c3c 6120 6872 6566 3d22 6874 7470 733a  |<a href="https:
-000025d0: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-000025e0: 7267 2f77 696b 692f 436f 6e6e 6563 745f  rg/wiki/Connect_
-000025f0: 466f 7572 223e 436f 6e6e 6563 7420 466f  Four">Connect Fo
-00002600: 7572 3c2f 613e 3c62 723e 6022 636f 6e6e  ur</a><br>`"conn
-00002610: 6563 745f 666f 7572 2260 207c 3c69 6d67  ect_four"` |<img
-00002620: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00002630: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00002640: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
-00002650: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
-00002660: 7373 6574 732f 636f 6e6e 6563 745f 666f  ssets/connect_fo
-00002670: 7572 5f64 6172 6b2e 6769 6622 2077 6964  ur_dark.gif" wid
-00002680: 7468 3d22 3630 7078 223e 3c69 6d67 2073  th="60px"><img s
-00002690: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-000026a0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-000026b0: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
-000026c0: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
-000026d0: 6574 732f 636f 6e6e 6563 745f 666f 7572  ets/connect_four
-000026e0: 5f6c 6967 6874 2e67 6966 2220 7769 6474  _light.gif" widt
-000026f0: 683d 2236 3070 7822 3e7c 2060 7630 6020  h="60px">| `v0` 
-00002700: 7c20 2a43 6f6e 6e65 6374 2064 6973 6373  | *Connect discs
-00002710: 2c20 7769 6e20 7769 7468 2066 6f75 722e  , win with four.
-00002720: 2a20 7c0a 7c3c 6120 6872 6566 3d22 6874  * |.|<a href="ht
-00002730: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
-00002740: 6961 2e6f 7267 2f77 696b 692f 4d69 6e69  ia.org/wiki/Mini
-00002750: 6368 6573 7322 3e47 6172 646e 6572 2043  chess">Gardner C
-00002760: 6865 7373 3c2f 613e 3c62 723e 6022 6761  hess</a><br>`"ga
-00002770: 7264 6e65 725f 6368 6573 7322 607c 3c69  rdner_chess"`|<i
-00002780: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00002790: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-000027a0: 6e74 656e 742e 636f 6d2f 736f 7465 7473  ntent.com/sotets
-000027b0: 756b 2f70 6778 2f6d 6169 6e2f 646f 6373  uk/pgx/main/docs
-000027c0: 2f61 7373 6574 732f 6761 7264 6e65 725f  /assets/gardner_
-000027d0: 6368 6573 735f 6461 726b 2e67 6966 2220  chess_dark.gif" 
-000027e0: 7769 6474 683d 2236 3070 7822 3e3c 696d  width="60px"><im
-000027f0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00002800: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00002810: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00002820: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-00002830: 6173 7365 7473 2f67 6172 646e 6572 5f63  assets/gardner_c
-00002840: 6865 7373 5f6c 6967 6874 2e67 6966 2220  hess_light.gif" 
-00002850: 7769 6474 683d 2236 3070 7822 3e7c 2060  width="60px">| `
-00002860: 7630 6020 7c20 2a35 7835 2063 6865 7373  v0` | *5x5 chess
-00002870: 2076 6172 6961 6e74 2c20 6578 636c 7564   variant, exclud
-00002880: 696e 6720 6361 7374 6c69 6e67 2e2a 207c  ing castling.* |
-00002890: 0a7c 3c61 2068 7265 663d 2268 7474 7073  .|<a href="https
-000028a0: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-000028b0: 6f72 672f 7769 6b69 2f47 6f5f 2867 616d  org/wiki/Go_(gam
-000028c0: 6529 223e 476f 3c2f 613e 3c62 723e 6022  e)">Go</a><br>`"
-000028d0: 676f 5f39 7839 2260 2060 2267 6f5f 3139  go_9x9"` `"go_19
-000028e0: 7831 3922 6020 7c3c 696d 6720 7372 633d  x19"` |<img src=
-000028f0: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00002900: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00002910: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
-00002920: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
-00002930: 2f67 6f2d 3139 7831 395f 6461 726b 2e67  /go-19x19_dark.g
-00002940: 6966 2220 7769 6474 683d 2236 3070 7822  if" width="60px"
-00002950: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00002960: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
-00002970: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
-00002980: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
-00002990: 6f63 732f 6173 7365 7473 2f67 6f2d 3139  ocs/assets/go-19
-000029a0: 7831 395f 6c69 6768 742e 6769 6622 2077  x19_light.gif" w
-000029b0: 6964 7468 3d22 3630 7078 223e 7c20 6076  idth="60px">| `v
-000029c0: 3060 207c 202a 5374 7261 7465 6769 6361  0` | *Strategica
-000029d0: 6c6c 7920 706c 6163 6520 7374 6f6e 6573  lly place stones
-000029e0: 2c20 636c 6169 6d20 7465 7272 6974 6f72  , claim territor
-000029f0: 792e 2a20 7c0a 7c3c 6120 6872 6566 3d22  y.* |.|<a href="
-00002a00: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00002a10: 6564 6961 2e6f 7267 2f77 696b 692f 4865  edia.org/wiki/He
-00002a20: 785f 2862 6f61 7264 5f67 616d 6529 223e  x_(board_game)">
-00002a30: 4865 783c 2f61 3e3c 6272 3e60 2268 6578  Hex</a><br>`"hex
-00002a40: 2260 207c 3c69 6d67 2073 7263 3d22 6874  "` |<img src="ht
-00002a50: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00002a60: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00002a70: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
-00002a80: 6e2f 646f 6373 2f61 7373 6574 732f 6865  n/docs/assets/he
-00002a90: 785f 6461 726b 2e67 6966 2220 7769 6474  x_dark.gif" widt
-00002aa0: 683d 2236 3070 7822 3e3c 696d 6720 7372  h="60px"><img sr
-00002ab0: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
-00002ac0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00002ad0: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
-00002ae0: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
-00002af0: 7473 2f68 6578 5f6c 6967 6874 2e67 6966  ts/hex_light.gif
-00002b00: 2220 7769 6474 683d 2236 3070 7822 3e7c  " width="60px">|
-00002b10: 2060 7630 6020 7c20 2a43 6f6e 6e65 6374   `v0` | *Connect
-00002b20: 206f 7070 6f73 6974 6520 7369 6465 732c   opposite sides,
-00002b30: 2062 6c6f 636b 206f 7070 6f6e 656e 742e   block opponent.
-00002b40: 2a20 7c0a 7c3c 6120 6872 6566 3d22 6874  * |.|<a href="ht
-00002b50: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
-00002b60: 6961 2e6f 7267 2f77 696b 692f 4b75 686e  ia.org/wiki/Kuhn
-00002b70: 5f70 6f6b 6572 223e 4b75 686e 2050 6f6b  _poker">Kuhn Pok
-00002b80: 6572 3c2f 613e 3c62 723e 6022 6b75 686e  er</a><br>`"kuhn
-00002b90: 5f70 6f6b 6572 2260 207c 3c69 6d67 2073  _poker"` |<img s
-00002ba0: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
-00002bb0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00002bc0: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
-00002bd0: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
-00002be0: 6574 732f 6b75 686e 5f70 6f6b 6572 5f64  ets/kuhn_poker_d
-00002bf0: 6172 6b2e 6769 6622 2077 6964 7468 3d22  ark.gif" width="
-00002c00: 3630 7078 223e 3c69 6d67 2073 7263 3d22  60px"><img src="
-00002c10: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00002c20: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00002c30: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
-00002c40: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
-00002c50: 6b75 686e 5f70 6f6b 6572 5f6c 6967 6874  kuhn_poker_light
-00002c60: 2e67 6966 2220 7769 6474 683d 2236 3070  .gif" width="60p
-00002c70: 7822 3e7c 2060 7630 6020 7c20 2a54 6872  x">| `v0` | *Thr
-00002c80: 6565 2d63 6172 6420 6265 7474 696e 6720  ee-card betting 
-00002c90: 616e 6420 626c 7566 6669 6e67 2067 616d  and bluffing gam
-00002ca0: 652e 2a20 7c0a 7c3c 6120 6872 6566 3d22  e.* |.|<a href="
-00002cb0: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00002cc0: 672f 6162 732f 3132 3037 2e31 3431 3122  g/abs/1207.1411"
-00002cd0: 3e4c 6564 7563 2068 6f6c 6427 656d 3c2f  >Leduc hold'em</
-00002ce0: 613e 3c62 723e 6022 6c65 6475 635f 686f  a><br>`"leduc_ho
-00002cf0: 6c64 656d 2260 207c 3c69 6d67 2073 7263  ldem"` |<img src
-00002d00: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00002d10: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00002d20: 636f 6d2f 736f 7465 7473 756b 2f70 6778  com/sotetsuk/pgx
-00002d30: 2f6d 6169 6e2f 646f 6373 2f61 7373 6574  /main/docs/asset
-00002d40: 732f 6c65 6475 635f 686f 6c64 656d 5f64  s/leduc_holdem_d
-00002d50: 6172 6b2e 6769 6622 2077 6964 7468 3d22  ark.gif" width="
-00002d60: 3630 7078 223e 3c69 6d67 2073 7263 3d22  60px"><img src="
-00002d70: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00002d80: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00002d90: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
-00002da0: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
-00002db0: 6c65 6475 635f 686f 6c64 656d 5f6c 6967  leduc_holdem_lig
-00002dc0: 6874 2e67 6966 2220 7769 6474 683d 2236  ht.gif" width="6
-00002dd0: 3070 7822 3e7c 2060 7630 6020 7c20 2a54  0px">| `v0` | *T
-00002de0: 776f 2d73 7569 742c 206c 696d 6974 6564  wo-suit, limited
-00002df0: 2064 6563 6b20 706f 6b65 722e 2a20 7c0a   deck poker.* |.
-00002e00: 7c3c 6120 6872 6566 3d22 6874 7470 733a  |<a href="https:
-00002e10: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 656e  //github.com/ken
-00002e20: 6a79 6f75 6e67 2f4d 696e 4174 6172 223e  jyoung/MinAtar">
-00002e30: 4d69 6e41 7461 722f 4173 7465 7269 783c  MinAtar/Asterix<
-00002e40: 2f61 3e3c 6272 3e60 226d 696e 6174 6172  /a><br>`"minatar
-00002e50: 2d61 7374 6572 6978 2260 207c 3c69 6d67  -asterix"` |<img
-00002e60: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-00002e70: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00002e80: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
-00002e90: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
-00002ea0: 7373 6574 732f 6d69 6e61 7461 722d 6173  ssets/minatar-as
-00002eb0: 7465 7269 782e 6769 6622 2077 6964 7468  terix.gif" width
-00002ec0: 3d22 3530 7078 223e 7c20 6076 3060 207c  ="50px">| `v0` |
-00002ed0: 202a 4176 6f69 6420 656e 656d 6965 732c   *Avoid enemies,
-00002ee0: 2063 6f6c 6c65 6374 2074 7265 6173 7572   collect treasur
-00002ef0: 652c 2073 7572 7669 7665 2e2a 207c 0a7c  e, survive.* |.|
-00002f00: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00002f10: 2f67 6974 6875 622e 636f 6d2f 6b65 6e6a  /github.com/kenj
-00002f20: 796f 756e 672f 4d69 6e41 7461 7222 3e4d  young/MinAtar">M
-00002f30: 696e 4174 6172 2f42 7265 616b 6f75 743c  inAtar/Breakout<
-00002f40: 2f61 3e3c 6272 3e60 226d 696e 6174 6172  /a><br>`"minatar
-00002f50: 2d62 7265 616b 6f75 7422 6020 7c3c 696d  -breakout"` |<im
-00002f60: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00002f70: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00002f80: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00002f90: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-00002fa0: 6173 7365 7473 2f6d 696e 6174 6172 2d62  assets/minatar-b
-00002fb0: 7265 616b 6f75 742e 6769 6622 2077 6964  reakout.gif" wid
-00002fc0: 7468 3d22 3530 7078 223e 7c20 6076 3060  th="50px">| `v0`
-00002fd0: 207c 202a 5061 6464 6c65 2c20 6261 6c6c   | *Paddle, ball
-00002fe0: 2c20 6272 6963 6b73 2c20 626f 756e 6365  , bricks, bounce
-00002ff0: 2c20 636c 6561 722e 2a20 7c0a 7c3c 6120  , clear.* |.|<a 
-00003000: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00003010: 7468 7562 2e63 6f6d 2f6b 656e 6a79 6f75  thub.com/kenjyou
-00003020: 6e67 2f4d 696e 4174 6172 223e 4d69 6e41  ng/MinAtar">MinA
-00003030: 7461 722f 4672 6565 7761 793c 2f61 3e3c  tar/Freeway</a><
-00003040: 6272 3e60 226d 696e 6174 6172 2d66 7265  br>`"minatar-fre
-00003050: 6577 6179 2260 207c 3c69 6d67 2073 7263  eway"` |<img src
-00003060: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00003070: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00003080: 636f 6d2f 736f 7465 7473 756b 2f70 6778  com/sotetsuk/pgx
-00003090: 2f6d 6169 6e2f 646f 6373 2f61 7373 6574  /main/docs/asset
-000030a0: 732f 6d69 6e61 7461 722d 6672 6565 7761  s/minatar-freewa
-000030b0: 792e 6769 6622 2077 6964 7468 3d22 3530  y.gif" width="50
-000030c0: 7078 223e 7c20 6076 3060 207c 202a 446f  px">| `v0` | *Do
-000030d0: 6467 696e 6720 6361 7273 2c20 636c 696d  dging cars, clim
-000030e0: 6269 6e67 2075 7020 6672 6565 7761 792e  bing up freeway.
-000030f0: 2a20 7c0a 7c3c 6120 6872 6566 3d22 6874  * |.|<a href="ht
-00003100: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003110: 2f6b 656e 6a79 6f75 6e67 2f4d 696e 4174  /kenjyoung/MinAt
-00003120: 6172 223e 4d69 6e41 7461 722f 5365 6171  ar">MinAtar/Seaq
-00003130: 7565 7374 3c2f 613e 3c62 723e 6022 6d69  uest</a><br>`"mi
-00003140: 6e61 7461 722d 7365 6171 7565 7374 2260  natar-seaquest"`
-00003150: 207c 3c69 6d67 2073 7263 3d22 6874 7470   |<img src="http
-00003160: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
-00003170: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
-00003180: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
-00003190: 646f 6373 2f61 7373 6574 732f 6d69 6e61  docs/assets/mina
-000031a0: 7461 722d 7365 6171 7565 7374 2e67 6966  tar-seaquest.gif
-000031b0: 2220 7769 6474 683d 2235 3070 7822 3e7c  " width="50px">|
-000031c0: 2060 7630 6020 7c20 2a55 6e64 6572 7761   `v0` | *Underwa
-000031d0: 7465 7220 7375 626d 6172 696e 6520 7265  ter submarine re
-000031e0: 7363 7565 2061 6e64 2063 6f6d 6261 742e  scue and combat.
-000031f0: 2a20 7c0a 7c3c 6120 6872 6566 3d22 6874  * |.|<a href="ht
-00003200: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003210: 2f6b 656e 6a79 6f75 6e67 2f4d 696e 4174  /kenjyoung/MinAt
-00003220: 6172 223e 4d69 6e41 7461 722f 5370 6163  ar">MinAtar/Spac
-00003230: 6549 6e76 6164 6572 733c 2f61 3e3c 6272  eInvaders</a><br
-00003240: 3e60 226d 696e 6174 6172 2d73 7061 6365  >`"minatar-space
-00003250: 5f69 6e76 6164 6572 7322 6020 7c3c 696d  _invaders"` |<im
-00003260: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00003270: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00003280: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00003290: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-000032a0: 6173 7365 7473 2f6d 696e 6174 6172 2d73  assets/minatar-s
-000032b0: 7061 6365 5f69 6e76 6164 6572 732e 6769  pace_invaders.gi
-000032c0: 6622 2077 6964 7468 3d22 3530 7078 223e  f" width="50px">
-000032d0: 7c20 6076 3060 207c 202a 416c 6965 6e20  | `v0` | *Alien 
-000032e0: 7368 6f6f 7465 7220 6761 6d65 2c20 646f  shooter game, do
-000032f0: 6467 6520 6275 6c6c 6574 732e 2a20 7c0a  dge bullets.* |.
-00003300: 7c3c 6120 6872 6566 3d22 6874 7470 733a  |<a href="https:
-00003310: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00003320: 7267 2f77 696b 692f 5265 7665 7273 6922  rg/wiki/Reversi"
-00003330: 3e4f 7468 656c 6c6f 3c2f 613e 3c62 723e  >Othello</a><br>
-00003340: 6022 6f74 6865 6c6c 6f22 6020 7c3c 696d  `"othello"` |<im
-00003350: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00003360: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00003370: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
-00003380: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
-00003390: 6173 7365 7473 2f6f 7468 656c 6c6f 5f64  assets/othello_d
-000033a0: 6172 6b2e 6769 6622 2077 6964 7468 3d22  ark.gif" width="
-000033b0: 3630 7078 223e 3c69 6d67 2073 7263 3d22  60px"><img src="
-000033c0: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-000033d0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-000033e0: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
-000033f0: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
-00003400: 6f74 6865 6c6c 6f5f 6c69 6768 742e 6769  othello_light.gi
-00003410: 6622 2077 6964 7468 3d22 3630 7078 223e  f" width="60px">
-00003420: 7c20 6076 3060 207c 202a 466c 6970 2061  | `v0` | *Flip a
-00003430: 6e64 2063 6f6e 7175 6572 206f 7070 6f6e  nd conquer oppon
-00003440: 656e 7427 7320 7069 6563 6573 2e2a 207c  ent's pieces.* |
-00003450: 0a7c 3c61 2068 7265 663d 2268 7474 7073  .|<a href="https
-00003460: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-00003470: 6f72 672f 7769 6b69 2f53 686f 6769 223e  org/wiki/Shogi">
-00003480: 5368 6f67 693c 2f61 3e3c 6272 3e60 2273  Shogi</a><br>`"s
-00003490: 686f 6769 2260 207c 3c69 6d67 2073 7263  hogi"` |<img src
-000034a0: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-000034b0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-000034c0: 636f 6d2f 736f 7465 7473 756b 2f70 6778  com/sotetsuk/pgx
-000034d0: 2f6d 6169 6e2f 646f 6373 2f61 7373 6574  /main/docs/asset
-000034e0: 732f 7368 6f67 695f 6461 726b 2e67 6966  s/shogi_dark.gif
-000034f0: 2220 7769 6474 683d 2236 3070 7822 3e3c  " width="60px"><
-00003500: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00003510: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00003520: 6f6e 7465 6e74 2e63 6f6d 2f73 6f74 6574  ontent.com/sotet
-00003530: 7375 6b2f 7067 782f 6d61 696e 2f64 6f63  suk/pgx/main/doc
-00003540: 732f 6173 7365 7473 2f73 686f 6769 5f6c  s/assets/shogi_l
-00003550: 6967 6874 2e67 6966 2220 7769 6474 683d  ight.gif" width=
-00003560: 2236 3070 7822 3e20 7c20 6076 3060 207c  "60px"> | `v0` |
-00003570: 202a 4a61 7061 6e65 7365 2063 6865 7373   *Japanese chess
-00003580: 2077 6974 6820 6361 7074 7572 6564 2070   with captured p
-00003590: 6965 6365 732e 2a20 7c0a 7c3c 6120 6872  ieces.* |.|<a hr
-000035a0: 6566 3d22 6874 7470 733a 2f2f 7375 676f  ef="https://sugo
-000035b0: 726f 6b75 7961 2e6a 702f 702f 7375 7a75  rokuya.jp/p/suzu
-000035c0: 6d65 2d6a 6f6e 6722 3e53 7061 7272 6f77  me-jong">Sparrow
-000035d0: 204d 6168 6a6f 6e67 3c2f 613e 3c62 723e   Mahjong</a><br>
-000035e0: 6022 7370 6172 726f 775f 6d61 686a 6f6e  `"sparrow_mahjon
-000035f0: 6722 6020 7c3c 696d 6720 7372 633d 2268  g"` |<img src="h
-00003600: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00003610: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00003620: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-00003630: 696e 2f64 6f63 732f 6173 7365 7473 2f73  in/docs/assets/s
-00003640: 7061 7272 6f77 5f6d 6168 6a6f 6e67 5f64  parrow_mahjong_d
-00003650: 6172 6b2e 7376 6722 2077 6964 7468 3d22  ark.svg" width="
-00003660: 3630 7078 223e 3c69 6d67 2073 7263 3d22  60px"><img src="
-00003670: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-00003680: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-00003690: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
-000036a0: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
-000036b0: 7370 6172 726f 775f 6d61 686a 6f6e 675f  sparrow_mahjong_
-000036c0: 6c69 6768 742e 7376 6722 2077 6964 7468  light.svg" width
-000036d0: 3d22 3630 7078 223e 7c20 2060 7630 6020  ="60px">|  `v0` 
-000036e0: 7c20 2a41 2073 696d 706c 6966 6965 642c  | *A simplified,
-000036f0: 2063 6869 6c64 7265 6e2d 6672 6965 6e64   children-friend
-00003700: 6c79 204d 6168 6a6f 6e67 2e2a 207c 0a7c  ly Mahjong.* |.|
-00003710: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00003720: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-00003730: 672f 7769 6b69 2f54 6963 2d74 6163 2d74  g/wiki/Tic-tac-t
-00003740: 6f65 223e 5469 632d 7461 632d 746f 653c  oe">Tic-tac-toe<
-00003750: 2f61 3e3c 6272 3e60 2274 6963 5f74 6163  /a><br>`"tic_tac
-00003760: 5f74 6f65 2260 207c 3c69 6d67 2073 7263  _toe"` |<img src
-00003770: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00003780: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00003790: 636f 6d2f 736f 7465 7473 756b 2f70 6778  com/sotetsuk/pgx
-000037a0: 2f6d 6169 6e2f 646f 6373 2f61 7373 6574  /main/docs/asset
-000037b0: 732f 7469 635f 7461 635f 746f 655f 6461  s/tic_tac_toe_da
-000037c0: 726b 2e67 6966 2220 7769 6474 683d 2236  rk.gif" width="6
-000037d0: 3070 7822 3e3c 696d 6720 7372 633d 2268  0px"><img src="h
-000037e0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-000037f0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00003800: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
-00003810: 696e 2f64 6f63 732f 6173 7365 7473 2f74  in/docs/assets/t
-00003820: 6963 5f74 6163 5f74 6f65 5f6c 6967 6874  ic_tac_toe_light
-00003830: 2e67 6966 2220 7769 6474 683d 2236 3070  .gif" width="60p
-00003840: 7822 3e7c 2060 7630 6020 7c20 2a54 6872  x">| `v0` | *Thr
-00003850: 6565 2069 6e20 6120 726f 7720 7769 6e73  ee in a row wins
-00003860: 2e2a 207c 0a0a 2d20 3c61 2068 7265 663d  .* |..- <a href=
-00003870: 2268 7474 7073 3a2f 2f65 6e2e 7769 6b69  "https://en.wiki
-00003880: 7065 6469 612e 6f72 672f 7769 6b69 2f4a  pedia.org/wiki/J
-00003890: 6170 616e 6573 655f 6d61 686a 6f6e 6722  apanese_mahjong"
-000038a0: 3e4d 6168 6a6f 6e67 3c2f 613e 2065 6e76  >Mahjong</a> env
-000038b0: 6972 6f6e 6d65 6e74 7320 6172 6520 756e  ironments are un
-000038c0: 6465 7220 6465 7665 6c6f 706d 656e 7420  der development 
-000038d0: f09f 9aa7 2049 6620 796f 7520 6861 7665  .... If you have
-000038e0: 2061 6e79 2072 6571 7565 7374 7320 666f   any requests fo
-000038f0: 7220 6e65 7720 656e 7669 726f 6e6d 656e  r new environmen
-00003900: 7473 2c20 706c 6561 7365 206c 6574 2075  ts, please let u
-00003910: 7320 6b6e 6f77 2062 7920 5b6f 7065 6e69  s know by [openi
-00003920: 6e67 2061 6e20 6973 7375 655d 2868 7474  ng an issue](htt
-00003930: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003940: 736f 7465 7473 756b 2f70 6778 2f69 7373  sotetsuk/pgx/iss
-00003950: 7565 732f 6e65 7729 0a2d 2046 6976 652d  ues/new).- Five-
-00003960: 776f 7264 2064 6573 6372 6970 7469 6f6e  word description
-00003970: 7320 7765 7265 2067 656e 6572 6174 6564  s were generated
-00003980: 2062 7920 5b43 6861 7447 5054 5d28 6874   by [ChatGPT](ht
-00003990: 7470 733a 2f2f 6368 6174 2e6f 7065 6e61  tps://chat.opena
-000039a0: 692e 636f 6d2f 2920 f09f a496 0a0a 2323  i.com/) ......##
-000039b0: 2320 5665 7273 696f 6e69 6e67 2070 6f6c  # Versioning pol
-000039c0: 6963 790a 0a45 6163 6820 656e 7669 726f  icy..Each enviro
-000039d0: 6e6d 656e 7420 6973 2076 6572 7369 6f6e  nment is version
-000039e0: 6564 2c20 616e 6420 7468 6520 7665 7273  ed, and the vers
-000039f0: 696f 6e20 6973 2069 6e63 7265 6d65 6e74  ion is increment
-00003a00: 6564 2077 6865 6e20 7468 6572 6520 6172  ed when there ar
-00003a10: 6520 6368 616e 6765 7320 7468 6174 2061  e changes that a
-00003a20: 6666 6563 7420 7468 6520 7065 7266 6f72  ffect the perfor
-00003a30: 6d61 6e63 6520 6f66 2061 6765 6e74 7320  mance of agents 
-00003a40: 6f72 2077 6865 6e20 7468 6572 6520 6172  or when there ar
-00003a50: 6520 6368 616e 6765 7320 7468 6174 2061  e changes that a
-00003a60: 7265 206e 6f74 2062 6163 6b77 6172 6420  re not backward 
-00003a70: 636f 6d70 6174 6962 6c65 2077 6974 6820  compatible with 
-00003a80: 7468 6520 4150 492e 0a49 6620 796f 7520  the API..If you 
-00003a90: 7761 6e74 2074 6f20 7075 7273 7565 2063  want to pursue c
-00003aa0: 6f6d 706c 6574 6520 7265 7072 6f64 7563  omplete reproduc
-00003ab0: 6962 696c 6974 792c 2077 6520 7265 636f  ibility, we reco
-00003ac0: 6d6d 656e 6420 7468 6174 2079 6f75 2063  mmend that you c
-00003ad0: 6865 636b 2074 6865 2076 6572 7369 6f6e  heck the version
-00003ae0: 206f 6620 5067 7820 616e 6420 6561 6368   of Pgx and each
-00003af0: 2065 6e76 6972 6f6e 6d65 6e74 2061 7320   environment as 
-00003b00: 666f 6c6c 6f77 733a 0a0a 6060 6070 790a  follows:..```py.
-00003b10: 3e3e 3e20 7067 782e 5f5f 7665 7273 696f  >>> pgx.__versio
-00003b20: 6e5f 5f0a 2731 2e30 2e30 270a 3e3e 3e20  n__.'1.0.0'.>>> 
-00003b30: 656e 762e 7665 7273 696f 6e0a 2776 3027  env.version.'v0'
-00003b40: 0a60 6060 0a0a 2323 2053 6565 2061 6c73  .```..## See als
-00003b50: 6f0a 0a50 6778 2069 7320 696e 7465 6e64  o..Pgx is intend
-00003b60: 6564 2074 6f20 636f 6d70 6c65 6d65 6e74  ed to complement
-00003b70: 2074 6865 7365 202a 2a4a 4158 2d6e 6174   these **JAX-nat
-00003b80: 6976 6520 656e 7669 726f 6e6d 656e 7473  ive environments
-00003b90: 2a2a 2077 6974 6820 2863 6c61 7373 6963  ** with (classic
-00003ba0: 2920 626f 6172 6420 6761 6d65 2073 7569  ) board game sui
-00003bb0: 7473 3a0a 0a2d 205b 526f 6265 7274 544c  ts:..- [RobertTL
-00003bc0: 616e 6765 2f67 796d 6e61 785d 2868 7474  ange/gymnax](htt
-00003bd0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003be0: 526f 6265 7274 544c 616e 6765 2f67 796d  RobertTLange/gym
-00003bf0: 6e61 7829 3a20 4a41 5820 696d 706c 656d  nax): JAX implem
-00003c00: 656e 7461 7469 6f6e 206f 6620 706f 7075  entation of popu
-00003c10: 6c61 7220 524c 2065 6e76 6972 6f6e 6d65  lar RL environme
-00003c20: 6e74 7320 285b 636c 6173 7369 6320 636f  nts ([classic co
-00003c30: 6e74 726f 6c5d 2868 7474 7073 3a2f 2f67  ntrol](https://g
-00003c40: 796d 6e61 7369 756d 2e66 6172 616d 612e  ymnasium.farama.
-00003c50: 6f72 672f 656e 7669 726f 6e6d 656e 7473  org/environments
-00003c60: 2f63 6c61 7373 6963 5f63 6f6e 7472 6f6c  /classic_control
-00003c70: 292c 205b 6273 7569 7465 5d28 6874 7470  ), [bsuite](http
-00003c80: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-00003c90: 6565 706d 696e 642f 6273 7569 7465 292c  eepmind/bsuite),
-00003ca0: 204d 696e 4174 6172 2c20 6574 6329 2061   MinAtar, etc) a
-00003cb0: 6e64 206d 6574 6120 524c 2074 6173 6b73  nd meta RL tasks
-00003cc0: 0a2d 205b 676f 6f67 6c65 2f62 7261 785d  .- [google/brax]
-00003cd0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003ce0: 636f 6d2f 676f 6f67 6c65 2f62 7261 7829  com/google/brax)
-00003cf0: 3a20 5269 6769 6462 6f64 7920 7068 7973  : Rigidbody phys
-00003d00: 6963 7320 7369 6d75 6c61 7469 6f6e 2069  ics simulation i
-00003d10: 6e20 4a41 5820 616e 6420 636f 6e74 696e  n JAX and contin
-00003d20: 756f 7573 2d73 7061 6365 2052 4c20 7461  uous-space RL ta
-00003d30: 736b 7320 2861 6e74 2c20 6665 7463 682c  sks (ant, fetch,
-00003d40: 2068 756d 616e 6f69 642c 2065 7463 290a   humanoid, etc).
-00003d50: 2d20 5b69 6e73 7461 6465 6570 6169 2f6a  - [instadeepai/j
-00003d60: 756d 616e 6a69 5d28 6874 7470 733a 2f2f  umanji](https://
-00003d70: 6769 7468 7562 2e63 6f6d 2f69 6e73 7461  github.com/insta
-00003d80: 6465 6570 6169 2f6a 756d 616e 6a69 293a  deepai/jumanji):
-00003d90: 2041 2073 7569 7465 206f 6620 6469 7665   A suite of dive
-00003da0: 7273 6520 616e 6420 6368 616c 6c65 6e67  rse and challeng
-00003db0: 696e 670a 2020 2020 524c 2065 6e76 6972  ing.    RL envir
-00003dc0: 6f6e 6d65 6e74 7320 696e 204a 4158 2028  onments in JAX (
-00003dd0: 6269 6e2d 7061 636b 696e 672c 2072 6f75  bin-packing, rou
-00003de0: 7469 6e67 2070 726f 626c 656d 732c 2065  ting problems, e
-00003df0: 7463 290a 0a43 6f6d 6269 6e69 6e67 2050  tc)..Combining P
-00003e00: 6778 2077 6974 6820 7468 6573 6520 2a2a  gx with these **
-00003e10: 4a41 582d 6e61 7469 7665 2061 6c67 6f72  JAX-native algor
-00003e20: 6974 686d 732f 696d 706c 656d 656e 7461  ithms/implementa
-00003e30: 7469 6f6e 732a 2a20 6d69 6768 7420 6265  tions** might be
-00003e40: 2061 6e20 696e 7465 7265 7374 696e 6720   an interesting 
-00003e50: 6469 7265 6374 696f 6e3a 0a0a 2d20 5b41  direction:..- [A
-00003e60: 6e61 6b69 6e20 6672 616d 6577 6f72 6b5d  nakin framework]
-00003e70: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
-00003e80: 7267 2f61 6273 2f32 3130 342e 3036 3237  rg/abs/2104.0627
-00003e90: 3229 3a20 4869 6768 6c79 2065 6666 6963  2): Highly effic
-00003ea0: 6965 6e74 2052 4c20 6672 616d 6577 6f72  ient RL framewor
-00003eb0: 6b20 7468 6174 2077 6f72 6b73 2077 6974  k that works wit
-00003ec0: 6820 4a41 582d 6e61 7469 7665 2065 6e76  h JAX-native env
-00003ed0: 6972 6f6e 6d65 6e74 7320 6f6e 2054 5055  ironments on TPU
-00003ee0: 730a 2d20 5b64 6565 706d 696e 642f 6d63  s.- [deepmind/mc
-00003ef0: 7478 5d28 6874 7470 733a 2f2f 6769 7468  tx](https://gith
-00003f00: 7562 2e63 6f6d 2f64 6565 706d 696e 642f  ub.com/deepmind/
-00003f10: 6d63 7478 293a 204a 4158 2d6e 6174 6976  mctx): JAX-nativ
-00003f20: 6520 4d43 5453 2069 6d70 6c65 6d65 6e74  e MCTS implement
-00003f30: 6174 696f 6e73 2c20 696e 636c 7564 696e  ations, includin
-00003f40: 6720 416c 7068 615a 6572 6f20 616e 6420  g AlphaZero and 
-00003f50: 4d75 5a65 726f 0a2d 205b 6465 6570 6d69  MuZero.- [deepmi
-00003f60: 6e64 2f72 6c61 785d 2868 7474 7073 3a2f  nd/rlax](https:/
-00003f70: 2f67 6974 6875 622e 636f 6d2f 6465 6570  /github.com/deep
-00003f80: 6d69 6e64 2f72 6c61 7829 3a20 4a41 582d  mind/rlax): JAX-
-00003f90: 6e61 7469 7665 2052 4c20 636f 6d70 6f6e  native RL compon
-00003fa0: 656e 7473 0a2d 205b 676f 6f67 6c65 2f65  ents.- [google/e
-00003fb0: 766f 6a61 785d 2868 7474 7073 3a2f 2f67  vojax](https://g
-00003fc0: 6974 6875 622e 636f 6d2f 676f 6f67 6c65  ithub.com/google
-00003fd0: 2f65 766f 6a61 7829 3a20 4861 7264 7761  /evojax): Hardwa
-00003fe0: 7265 2d41 6363 656c 6572 6174 6564 206e  re-Accelerated n
-00003ff0: 6575 726f 6576 6f6c 7574 696f 6e0a 2d20  euroevolution.- 
-00004000: 5b52 6f62 6572 7454 4c61 6e67 652f 6576  [RobertTLange/ev
-00004010: 6f73 6178 5d28 6874 7470 733a 2f2f 6769  osax](https://gi
-00004020: 7468 7562 2e63 6f6d 2f52 6f62 6572 7454  thub.com/RobertT
-00004030: 4c61 6e67 652f 6576 6f73 6178 293a 204a  Lange/evosax): J
-00004040: 4158 2d6e 6174 6976 6520 6576 6f6c 7574  AX-native evolut
-00004050: 696f 6e20 7374 7261 7465 6779 2028 4553  ion strategy (ES
-00004060: 2920 696d 706c 656d 656e 7461 7469 6f6e  ) implementation
-00004070: 730a 2d20 5b61 6461 7074 6976 652d 696e  s.- [adaptive-in
-00004080: 7465 6c6c 6967 656e 742d 726f 626f 7469  telligent-roboti
-00004090: 6373 2f51 4461 785d 2868 7474 7073 3a2f  cs/QDax](https:/
-000040a0: 2f67 6974 6875 622e 636f 6d2f 6164 6170  /github.com/adap
-000040b0: 7469 7665 2d69 6e74 656c 6c69 6765 6e74  tive-intelligent
-000040c0: 2d72 6f62 6f74 6963 732f 5144 6178 293a  -robotics/QDax):
-000040d0: 204a 4158 2d6e 6174 6976 6520 5175 616c   JAX-native Qual
-000040e0: 6974 792d 4469 7665 7273 6974 7920 2851  ity-Diversity (Q
-000040f0: 4429 2061 6c67 6f72 6974 686d 730a 2d20  D) algorithms.- 
-00004100: 5b6c 7563 6872 6973 3432 392f 7075 7265  [luchris429/pure
-00004110: 6a61 7872 6c5d 2868 7474 7073 3a2f 2f67  jaxrl](https://g
-00004120: 6974 6875 622e 636f 6d2f 6c75 6368 7269  ithub.com/luchri
-00004130: 7334 3239 2f70 7572 656a 6178 726c 293a  s429/purejaxrl):
-00004140: 204a 6178 2d6e 6174 6976 6520 524c 2069   Jax-native RL i
-00004150: 6d70 6c65 6d65 6e74 6174 696f 6e73 0a0a  mplementations..
-00004160: 2323 2043 6974 6174 696f 6e0a 0a60 6060  ## Citation..```
-00004170: 0a40 6172 7469 636c 657b 6b6f 7961 6d61  .@article{koyama
-00004180: 6461 3230 3233 7067 782c 0a20 2074 6974  da2023pgx,.  tit
-00004190: 6c65 3d7b 5067 783a 2048 6172 6477 6172  le={Pgx: Hardwar
-000041a0: 652d 6163 6365 6c65 7261 7465 6420 7061  e-accelerated pa
-000041b0: 7261 6c6c 656c 2067 616d 6520 7369 6d75  rallel game simu
-000041c0: 6c61 7469 6f6e 2066 6f72 2072 6569 6e66  lation for reinf
-000041d0: 6f72 6365 6d65 6e74 206c 6561 726e 696e  orcement learnin
-000041e0: 677d 2c0a 2020 6175 7468 6f72 3d7b 4b6f  g},.  author={Ko
-000041f0: 7961 6d61 6461 2c20 536f 7465 7473 7520  yamada, Sotetsu 
-00004200: 616e 6420 4f6b 616e 6f2c 2053 6869 6e72  and Okano, Shinr
-00004210: 6920 616e 6420 4e69 7368 696d 6f72 692c  i and Nishimori,
-00004220: 2053 6f69 6368 6972 6f20 616e 6420 4d75   Soichiro and Mu
-00004230: 7261 7461 2c20 5975 2061 6e64 2048 6162  rata, Yu and Hab
-00004240: 6172 612c 204b 6569 676f 2061 6e64 204b  ara, Keigo and K
-00004250: 6974 612c 2048 6172 756b 6120 616e 6420  ita, Haruka and 
-00004260: 4973 6869 692c 2053 6869 6e7d 2c0a 2020  Ishii, Shin},.  
-00004270: 6a6f 7572 6e61 6c3d 7b61 7258 6976 2070  journal={arXiv p
-00004280: 7265 7072 696e 7420 6172 5869 763a 3233  reprint arXiv:23
-00004290: 3033 2e31 3735 3033 7d2c 0a20 2079 6561  03.17503},.  yea
-000042a0: 723d 7b32 3032 337d 0a7d 0a60 6060 0a0a  r={2023}.}.```..
-000042b0: 2323 204c 4943 454e 5345 0a0a 4170 6163  ## LICENSE..Apac
-000042c0: 6865 2d32 2e30 0a                        he-2.0.
+00000240: 666c 6f77 732f 6369 2e79 6d6c 290a 0a0a  flows/ci.yml)...
+00000250: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000260: 6572 223e 0a3c 696d 6720 7372 633d 2268  er">.<img src="h
+00000270: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000280: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000290: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
+000002a0: 696e 2f64 6f63 732f 6173 7365 7473 2f6c  in/docs/assets/l
+000002b0: 6f67 6f2e 7376 6722 2077 6964 7468 3d22  ogo.svg" width="
+000002c0: 3430 2522 3e0a 3c2f 6469 763e 0a0a 4120  40%">.</div>..A 
+000002d0: 636f 6c6c 6563 7469 6f6e 206f 6620 4750  collection of GP
+000002e0: 552f 5450 552d 6163 6365 6c65 7261 7465  U/TPU-accelerate
+000002f0: 6420 7061 7261 6c6c 656c 2067 616d 6520  d parallel game 
+00000300: 7369 6d75 6c61 746f 7273 2066 6f72 2072  simulators for r
+00000310: 6569 6e66 6f72 6365 6d65 6e74 206c 6561  einforcement lea
+00000320: 726e 696e 6720 2852 4c29 0a0a 3c64 6976  rning (RL)..<div
+00000330: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000340: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
+00000350: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000360: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
+00000370: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
+00000380: 6f63 732f 6173 7365 7473 2f67 6f5f 6461  ocs/assets/go_da
+00000390: 726b 2e67 6966 2367 682d 6461 726b 2d6d  rk.gif#gh-dark-m
+000003a0: 6f64 652d 6f6e 6c79 2220 7769 6474 683d  ode-only" width=
+000003b0: 2233 3025 223e 3c69 6d67 2073 7263 3d22  "30%"><img src="
+000003c0: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+000003d0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+000003e0: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
+000003f0: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
+00000400: 676f 5f64 6172 6b2e 6769 6623 6768 2d64  go_dark.gif#gh-d
+00000410: 6172 6b2d 6d6f 6465 2d6f 6e6c 7922 2077  ark-mode-only" w
+00000420: 6964 7468 3d22 3330 2522 2073 7479 6c65  idth="30%" style
+00000430: 3d22 7472 616e 7366 6f72 6d3a 726f 7461  ="transform:rota
+00000440: 7465 2832 3730 6465 6729 3b22 3e3c 696d  te(270deg);"><im
+00000450: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+00000460: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00000470: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
+00000480: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
+00000490: 6173 7365 7473 2f67 6f5f 6461 726b 2e67  assets/go_dark.g
+000004a0: 6966 2367 682d 6461 726b 2d6d 6f64 652d  if#gh-dark-mode-
+000004b0: 6f6e 6c79 2220 7769 6474 683d 2233 3025  only" width="30%
+000004c0: 2220 7374 796c 653d 2274 7261 6e73 666f  " style="transfo
+000004d0: 726d 3a72 6f74 6174 6528 3930 6465 6729  rm:rotate(90deg)
+000004e0: 3b22 3e0a 3c69 6d67 2073 7263 3d22 6874  ;">.<img src="ht
+000004f0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000500: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000510: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
+00000520: 6e2f 646f 6373 2f61 7373 6574 732f 676f  n/docs/assets/go
+00000530: 5f6c 6967 6874 2e67 6966 2367 682d 6c69  _light.gif#gh-li
+00000540: 6768 742d 6d6f 6465 2d6f 6e6c 7922 2077  ght-mode-only" w
+00000550: 6964 7468 3d22 3330 2522 3e3c 696d 6720  idth="30%"><img 
+00000560: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00000570: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000580: 6e74 2e63 6f6d 2f73 6f74 6574 7375 6b2f  nt.com/sotetsuk/
+00000590: 7067 782f 6d61 696e 2f64 6f63 732f 6173  pgx/main/docs/as
+000005a0: 7365 7473 2f67 6f5f 6c69 6768 742e 6769  sets/go_light.gi
+000005b0: 6623 6768 2d6c 6967 6874 2d6d 6f64 652d  f#gh-light-mode-
+000005c0: 6f6e 6c79 2220 7769 6474 683d 2233 3025  only" width="30%
+000005d0: 2220 7374 796c 653d 2274 7261 6e73 666f  " style="transfo
+000005e0: 726d 3a72 6f74 6174 6528 3237 3064 6567  rm:rotate(270deg
+000005f0: 293b 223e 3c69 6d67 2073 7263 3d22 6874  );"><img src="ht
+00000600: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00000610: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00000620: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
+00000630: 6e2f 646f 6373 2f61 7373 6574 732f 676f  n/docs/assets/go
+00000640: 5f6c 6967 6874 2e67 6966 2367 682d 6c69  _light.gif#gh-li
+00000650: 6768 742d 6d6f 6465 2d6f 6e6c 7922 2077  ght-mode-only" w
+00000660: 6964 7468 3d22 3330 2522 2073 7479 6c65  idth="30%" style
+00000670: 3d22 7472 616e 7366 6f72 6d3a 726f 7461  ="transform:rota
+00000680: 7465 2839 3064 6567 293b 223e 0a3c 2f64  te(90deg);">.</d
+00000690: 6976 3e0a 0af0 9f8e 8920 2a2a 6076 312e  iv>...... **`v1.
+000006a0: 302e 3060 2a2a 2069 7320 7265 6c65 6173  0.0`** is releas
+000006b0: 6564 2120 2832 3032 332e 362e 3230 290a  ed! (2023.6.20).
+000006c0: 0a23 2320 5768 7920 5067 783f 0a0a 3c21  .## Why Pgx?..<!
+000006d0: 2d2d 2d20 0a74 6872 6f75 6768 7075 743a  --- .throughput:
+000006e0: 2068 7474 7073 3a2f 2f63 6f6c 6162 2e72   https://colab.r
+000006f0: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+00000700: 6f6d 2f64 7269 7665 2f31 6749 5748 594c  om/drive/1gIWHYL
+00000710: 4b42 7845 3258 4b44 6841 6c45 594b 5665  KBxE2XKDhAlEYKVe
+00000720: 637a 3357 4734 637a 647a 2373 6372 6f6c  cz3WG4czdz#scrol
+00000730: 6c54 6f3d 5631 515a 6852 586f 474c 384b  lTo=V1QZhRXoGL8K
+00000740: 0a2d 2d2d 3e0a 0a5b 4272 6178 5d28 6874  .--->..[Brax](ht
+00000750: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000760: 2f67 6f6f 676c 652f 6272 6178 292c 2061  /google/brax), a
+00000770: 205b 4a41 585d 2868 7474 7073 3a2f 2f67   [JAX](https://g
+00000780: 6974 6875 622e 636f 6d2f 676f 6f67 6c65  ithub.com/google
+00000790: 2f6a 6178 292d 6e61 7469 7665 2070 6879  /jax)-native phy
+000007a0: 7369 6373 2065 6e67 696e 652c 2070 726f  sics engine, pro
+000007b0: 7669 6465 7320 6578 7472 656d 656c 7920  vides extremely 
+000007c0: 6869 6768 2d73 7065 6564 2070 6172 616c  high-speed paral
+000007d0: 6c65 6c20 7369 6d75 6c61 7469 6f6e 2066  lel simulation f
+000007e0: 6f72 2052 4c20 696e 202a 636f 6e74 696e  or RL in *contin
+000007f0: 756f 7573 2a20 7374 6174 6520 7370 6163  uous* state spac
+00000800: 652e 0a54 6865 6e2c 2077 6861 7420 6162  e..Then, what ab
+00000810: 6f75 7420 524c 2069 6e20 2a64 6973 6372  out RL in *discr
+00000820: 6574 652a 2073 7461 7465 2073 7061 6365  ete* state space
+00000830: 7320 6c69 6b65 2043 6865 7373 2c20 5368  s like Chess, Sh
+00000840: 6f67 692c 2061 6e64 2047 6f3f 202a 2a50  ogi, and Go? **P
+00000850: 6778 2a2a 2070 726f 7669 6465 7320 6120  gx** provides a 
+00000860: 7769 6465 2076 6172 6965 7479 206f 6620  wide variety of 
+00000870: 4a41 582d 6e61 7469 7665 2067 616d 6520  JAX-native game 
+00000880: 7369 6d75 6c61 746f 7273 2120 4869 6768  simulators! High
+00000890: 6c69 6768 7465 6420 6665 6174 7572 6573  lighted features
+000008a0: 2069 6e63 6c75 6465 3a0a 0a2d 20e2 9aa1   include:..- ...
+000008b0: 202a 2a53 7570 6572 2066 6173 742a 2a20   **Super fast** 
+000008c0: 696e 2070 6172 616c 6c65 6c20 6578 6563  in parallel exec
+000008d0: 7574 696f 6e20 6f6e 2061 6363 656c 6572  ution on acceler
+000008e0: 6174 6f72 730a 2d20 f09f 8eb2 202a 2a56  ators.- .... **V
+000008f0: 6172 696f 7573 2067 616d 6520 7375 7070  arious game supp
+00000900: 6f72 742a 2a20 696e 636c 7564 696e 6720  ort** including 
+00000910: 2a2a 4261 636b 6761 6d6d 6f6e 2a2a 2c20  **Backgammon**, 
+00000920: 2a2a 4368 6573 732a 2a2c 202a 2a53 686f  **Chess**, **Sho
+00000930: 6769 2a2a 2c20 616e 6420 2a2a 476f 2a2a  gi**, and **Go**
+00000940: 0a2d 20f0 9f96 bcef b88f 202a 2a42 6561  .- ....... **Bea
+00000950: 7574 6966 756c 2076 6973 7561 6c69 7a61  utiful visualiza
+00000960: 7469 6f6e 2a2a 2069 6e20 5356 4720 666f  tion** in SVG fo
+00000970: 726d 6174 0a0a 0a23 2320 5175 6963 6b20  rmat...## Quick 
+00000980: 7374 6172 740a 0a2d 205b 4765 7474 696e  start..- [Gettin
+00000990: 6720 7374 6172 7465 645d 2868 7474 7073  g started](https
+000009a0: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
+000009b0: 682e 676f 6f67 6c65 2e63 6f6d 2f67 6974  h.google.com/git
+000009c0: 6875 622f 736f 7465 7473 756b 2f70 6778  hub/sotetsuk/pgx
+000009d0: 2f62 6c6f 622f 6d61 696e 2f63 6f6c 6162  /blob/main/colab
+000009e0: 2f70 6778 5f68 656c 6c6f 5f77 6f72 6c64  /pgx_hello_world
+000009f0: 2e69 7079 6e62 290a 2d20 5b50 6778 2062  .ipynb).- [Pgx b
+00000a00: 6173 656c 696e 6520 6d6f 6465 6c73 5d28  aseline models](
+00000a10: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
+00000a20: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
+00000a30: 6d2f 6769 7468 7562 2f73 6f74 6574 7375  m/github/sotetsu
+00000a40: 6b2f 7067 782f 626c 6f62 2f6d 6169 6e2f  k/pgx/blob/main/
+00000a50: 636f 6c61 622f 6261 7365 6c69 6e65 732e  colab/baselines.
+00000a60: 6970 796e 6229 0a2d 205b 5050 4f20 6578  ipynb).- [PPO ex
+00000a70: 616d 706c 655d 2868 7474 7073 3a2f 2f63  ample](https://c
+00000a80: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00000a90: 6f67 6c65 2e63 6f6d 2f67 6974 6875 622f  ogle.com/github/
+00000aa0: 736f 7465 7473 756b 2f70 6778 2f62 6c6f  sotetsuk/pgx/blo
+00000ab0: 622f 6d61 696e 2f63 6f6c 6162 2f70 706f  b/main/colab/ppo
+00000ac0: 2e69 7079 6e62 290a 2d20 5b45 7870 6f72  .ipynb).- [Expor
+00000ad0: 7420 746f 2050 6574 7469 6e67 5a6f 6f20  t to PettingZoo 
+00000ae0: 4150 495d 2868 7474 7073 3a2f 2f63 6f6c  API](https://col
+00000af0: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
+00000b00: 6c65 2e63 6f6d 2f67 6974 6875 622f 736f  le.com/github/so
+00000b10: 7465 7473 756b 2f70 6778 2f62 6c6f 622f  tetsuk/pgx/blob/
+00000b20: 6d61 696e 2f63 6f6c 6162 2f70 6778 3270  main/colab/pgx2p
+00000b30: 6574 7469 6e67 7a6f 6f2e 6970 796e 6229  ettingzoo.ipynb)
+00000b40: 0a0a 2323 2055 7361 6765 0a0a 5468 6520  ..## Usage..The 
+00000b50: 666f 6c6c 6f77 696e 6720 636f 6465 2073  following code s
+00000b60: 6e69 7070 6574 2073 686f 7773 2061 2073  nippet shows a s
+00000b70: 696d 706c 6520 6578 616d 706c 6520 6f66  imple example of
+00000b80: 2075 7369 6e67 2050 6778 2e0a 596f 7520   using Pgx..You 
+00000b90: 6361 6e20 7472 7920 6974 206f 7574 2069  can try it out i
+00000ba0: 6e20 5b74 6869 7320 436f 6c61 625d 2868  n [this Colab](h
+00000bb0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
+00000bc0: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
+00000bd0: 2f67 6974 6875 622f 736f 7465 7473 756b  /github/sotetsuk
+00000be0: 2f70 6778 2f62 6c6f 622f 6d61 696e 2f63  /pgx/blob/main/c
+00000bf0: 6f6c 6162 2f70 6778 5f68 656c 6c6f 5f77  olab/pgx_hello_w
+00000c00: 6f72 6c64 2e69 7079 6e62 292e 0a4e 6f74  orld.ipynb)..Not
+00000c10: 6520 7468 6174 2061 6c6c 2060 7374 6570  e that all `step
+00000c20: 6020 6675 6e63 7469 6f6e 7320 696e 2050  ` functions in P
+00000c30: 6778 2065 6e76 6972 6f6e 6d65 6e74 7320  gx environments 
+00000c40: 6172 6520 2a2a 4a41 582d 6e61 7469 7665  are **JAX-native
+00000c50: 2e2a 2a2c 2069 2e65 2e2c 2074 6865 7920  .**, i.e., they 
+00000c60: 6172 6520 616c 6c20 2a4a 4954 2d61 626c  are all *JIT-abl
+00000c70: 652a 2e0a 506c 6561 7365 2072 6566 6572  e*..Please refer
+00000c80: 2074 6f20 7468 6520 5b64 6f63 756d 656e   to the [documen
+00000c90: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+00000ca0: 736f 7465 7473 756b 2e67 6974 6875 622e  sotetsuk.github.
+00000cb0: 696f 2f70 6778 2920 666f 7220 6d6f 7265  io/pgx) for more
+00000cc0: 2064 6574 6169 6c73 2e0a 0a60 6060 7079   details...```py
+00000cd0: 0a69 6d70 6f72 7420 6a61 780a 696d 706f  .import jax.impo
+00000ce0: 7274 2070 6778 0a0a 656e 7620 3d20 7067  rt pgx..env = pg
+00000cf0: 782e 6d61 6b65 2822 676f 5f31 3978 3139  x.make("go_19x19
+00000d00: 2229 0a69 6e69 7420 3d20 6a61 782e 6a69  ").init = jax.ji
+00000d10: 7428 6a61 782e 766d 6170 2865 6e76 2e69  t(jax.vmap(env.i
+00000d20: 6e69 7429 290a 7374 6570 203d 206a 6178  nit)).step = jax
+00000d30: 2e6a 6974 286a 6178 2e76 6d61 7028 656e  .jit(jax.vmap(en
+00000d40: 762e 7374 6570 2929 0a0a 6261 7463 685f  v.step))..batch_
+00000d50: 7369 7a65 203d 2031 3032 340a 6b65 7973  size = 1024.keys
+00000d60: 203d 206a 6178 2e72 616e 646f 6d2e 7370   = jax.random.sp
+00000d70: 6c69 7428 6a61 782e 7261 6e64 6f6d 2e50  lit(jax.random.P
+00000d80: 524e 474b 6579 2834 3229 2c20 6261 7463  RNGKey(42), batc
+00000d90: 685f 7369 7a65 290a 7374 6174 6520 3d20  h_size).state = 
+00000da0: 696e 6974 286b 6579 7329 2020 2320 7665  init(keys)  # ve
+00000db0: 6374 6f72 697a 6564 2073 7461 7465 730a  ctorized states.
+00000dc0: 7768 696c 6520 6e6f 7420 2873 7461 7465  while not (state
+00000dd0: 2e74 6572 6d69 6e61 7465 6420 7c20 7374  .terminated | st
+00000de0: 6174 652e 7472 756e 6361 7465 6429 2e61  ate.truncated).a
+00000df0: 6c6c 2829 3a0a 2020 2020 6163 7469 6f6e  ll():.    action
+00000e00: 203d 206d 6f64 656c 2873 7461 7465 2e63   = model(state.c
+00000e10: 7572 7265 6e74 5f70 6c61 7965 722c 2073  urrent_player, s
+00000e20: 7461 7465 2e6f 6273 6572 7661 7469 6f6e  tate.observation
+00000e30: 2c20 7374 6174 652e 6c65 6761 6c5f 6163  , state.legal_ac
+00000e40: 7469 6f6e 5f6d 6173 6b29 0a20 2020 2073  tion_mask).    s
+00000e50: 7461 7465 203d 2073 7465 7028 7374 6174  tate = step(stat
+00000e60: 652c 2061 6374 696f 6e29 2020 2320 7374  e, action)  # st
+00000e70: 6174 652e 7265 7761 7264 2028 322c 290a  ate.reward (2,).
+00000e80: 6060 600a 0a50 6778 2069 7320 6120 6c69  ```..Pgx is a li
+00000e90: 6272 6172 7920 7468 6174 2066 6f63 7573  brary that focus
+00000ea0: 6573 206f 6e20 6661 7374 6572 2069 6d70  es on faster imp
+00000eb0: 6c65 6d65 6e74 6174 696f 6e73 2072 6174  lementations rat
+00000ec0: 6865 7220 7468 616e 206a 7573 7420 7468  her than just th
+00000ed0: 6520 4150 4920 6974 7365 6c66 2e20 0a48  e API itself. .H
+00000ee0: 6f77 6576 6572 2c20 7468 6520 4150 4920  owever, the API 
+00000ef0: 6974 7365 6c66 2069 7320 616c 736f 2073  itself is also s
+00000f00: 7566 6669 6369 656e 746c 7920 6765 6e65  ufficiently gene
+00000f10: 7261 6c2e 2046 6f72 2065 7861 6d70 6c65  ral. For example
+00000f20: 2c20 616c 6c20 656e 7669 726f 6e6d 656e  , all environmen
+00000f30: 7473 2069 6e20 5067 7820 6361 6e20 6265  ts in Pgx can be
+00000f40: 2063 6f6e 7665 7274 6564 2074 6f20 7468   converted to th
+00000f50: 6520 4145 4320 4150 4920 6f66 205b 5065  e AEC API of [Pe
+00000f60: 7474 696e 675a 6f6f 5d28 6874 7470 733a  ttingZoo](https:
+00000f70: 2f2f 6769 7468 7562 2e63 6f6d 2f46 6172  //github.com/Far
+00000f80: 616d 612d 466f 756e 6461 7469 6f6e 2f50  ama-Foundation/P
+00000f90: 6574 7469 6e67 5a6f 6f29 2c20 616e 6420  ettingZoo), and 
+00000fa0: 796f 7520 6361 6e20 7275 6e20 5067 7820  you can run Pgx 
+00000fb0: 656e 7669 726f 6e6d 656e 7473 2074 6872  environments thr
+00000fc0: 6f75 6768 2074 6865 2050 6574 7469 6e67  ough the Petting
+00000fd0: 5a6f 6f20 4150 492e 0a59 6f75 2063 616e  Zoo API..You can
+00000fe0: 2073 6565 2074 6865 2064 656d 6f6e 7374   see the demonst
+00000ff0: 7261 7469 6f6e 2069 6e20 5b74 6869 7320  ration in [this 
+00001000: 436f 6c61 625d 2868 7474 7073 3a2f 2f63  Colab](https://c
+00001010: 6f6c 6162 2e72 6573 6561 7263 682e 676f  olab.research.go
+00001020: 6f67 6c65 2e63 6f6d 2f67 6974 6875 622f  ogle.com/github/
+00001030: 736f 7465 7473 756b 2f70 6778 2f62 6c6f  sotetsuk/pgx/blo
+00001040: 622f 6d61 696e 2f63 6f6c 6162 2f70 6778  b/main/colab/pgx
+00001050: 3270 6574 7469 6e67 7a6f 6f2e 6970 796e  2pettingzoo.ipyn
+00001060: 6229 2e0a 0a0a 2323 2049 6e73 7461 6c6c  b)....## Install
+00001070: 6174 696f 6e0a 0a60 6060 7368 0a70 6970  ation..```sh.pip
+00001080: 2069 6e73 7461 6c6c 2070 6778 0a60 6060   install pgx.```
+00001090: 0a0a 4e6f 7465 2074 6861 7420 7468 6520  ..Note that the 
+000010a0: 5b4d 696e 4174 6172 5d28 6874 7470 733a  [MinAtar](https:
+000010b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 656e  //github.com/ken
+000010c0: 6a79 6f75 6e67 2f4d 696e 4174 6172 2920  jyoung/MinAtar) 
+000010d0: 7375 6974 6520 6973 2070 726f 7669 6465  suite is provide
+000010e0: 6420 6173 2061 2073 6570 6172 6174 6520  d as a separate 
+000010f0: 6578 7465 6e73 696f 6e20 666f 7220 5067  extension for Pg
+00001100: 7820 285b 6070 6778 2d6d 696e 6174 6172  x ([`pgx-minatar
+00001110: 605d 2868 7474 7073 3a2f 2f67 6974 6875  `](https://githu
+00001120: 622e 636f 6d2f 736f 7465 7473 756b 2f70  b.com/sotetsuk/p
+00001130: 6778 2d6d 696e 6174 6172 2929 2e20 5468  gx-minatar)). Th
+00001140: 6572 6566 6f72 652c 2070 6c65 6173 6520  erefore, please 
+00001150: 7275 6e20 7468 6520 666f 6c6c 6f77 696e  run the followin
+00001160: 6720 636f 6d6d 616e 6420 6164 6469 7469  g command additi
+00001170: 6f6e 616c 7920 746f 2075 7365 2074 6865  onaly to use the
+00001180: 204d 696e 4174 6172 2073 7569 7465 2069   MinAtar suite i
+00001190: 6e20 5067 783a 0a0a 6060 6073 680a 7069  n Pgx:..```sh.pi
+000011a0: 7020 696e 7374 616c 6c20 7067 782d 6d69  p install pgx-mi
+000011b0: 6e61 7461 720a 6060 600a 0a50 6778 2069  natar.```..Pgx i
+000011c0: 7320 7072 6f76 6964 6564 2075 6e64 6572  s provided under
+000011d0: 2074 6865 2041 7061 6368 6520 322e 3020   the Apache 2.0 
+000011e0: 4c69 6365 6e73 652c 2062 7574 2074 6865  License, but the
+000011f0: 206f 7269 6769 6e61 6c20 4d69 6e41 7461   original MinAta
+00001200: 7220 7375 6974 6520 666f 6c6c 6f77 7320  r suite follows 
+00001210: 7468 6520 4750 4c20 332e 3020 4c69 6365  the GPL 3.0 Lice
+00001220: 6e73 652e 2054 6865 7265 666f 7265 2c20  nse. Therefore, 
+00001230: 706c 6561 7365 206e 6f74 6520 7468 6174  please note that
+00001240: 2074 6865 2073 6570 6172 6174 6564 204d   the separated M
+00001250: 696e 4174 6172 2065 7874 656e 7369 6f6e  inAtar extension
+00001260: 2066 6f72 2050 6778 2061 6c73 6f20 6164   for Pgx also ad
+00001270: 6865 7265 7320 746f 2074 6865 2047 504c  heres to the GPL
+00001280: 2033 2e30 204c 6963 656e 7365 2e0a 0a23   3.0 License...#
+00001290: 2320 5375 7070 6f72 7465 6420 6761 6d65  # Supported game
+000012a0: 730a 0a7c 2042 6163 6b67 616d 6d6f 6e20  s..| Backgammon 
+000012b0: 7c20 4368 6573 7320 7c20 5368 6f67 6920  | Chess | Shogi 
+000012c0: 7c20 476f 207c 0a7c 3a2d 2d2d 3a7c 3a2d  | Go |.|:---:|:-
+000012d0: 2d2d 3a7c 3a2d 2d2d 3a7c 3a2d 2d2d 3a7c  --:|:---:|:---:|
+000012e0: 0a7c 3c69 6d67 2073 7263 3d22 6874 7470  .|<img src="http
+000012f0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00001300: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00001310: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00001320: 646f 6373 2f61 7373 6574 732f 6261 636b  docs/assets/back
+00001330: 6761 6d6d 6f6e 5f64 6172 6b2e 6769 6623  gammon_dark.gif#
+00001340: 6768 2d64 6172 6b2d 6d6f 6465 2d6f 6e6c  gh-dark-mode-onl
+00001350: 7922 2077 6964 7468 3d22 3137 3070 7822  y" width="170px"
+00001360: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00001370: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00001380: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
+00001390: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
+000013a0: 6f63 732f 6173 7365 7473 2f62 6163 6b67  ocs/assets/backg
+000013b0: 616d 6d6f 6e5f 6c69 6768 742e 6769 6623  ammon_light.gif#
+000013c0: 6768 2d6c 6967 6874 2d6d 6f64 652d 6f6e  gh-light-mode-on
+000013d0: 6c79 2220 7769 6474 683d 2231 3730 7078  ly" width="170px
+000013e0: 223e 7c3c 696d 6720 7372 633d 2268 7474  ">|<img src="htt
+000013f0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00001400: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
+00001410: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
+00001420: 2f64 6f63 732f 6173 7365 7473 2f63 6865  /docs/assets/che
+00001430: 7373 5f64 6172 6b2e 6769 6623 6768 2d64  ss_dark.gif#gh-d
+00001440: 6172 6b2d 6d6f 6465 2d6f 6e6c 7922 2077  ark-mode-only" w
+00001450: 6964 7468 3d22 3135 3870 7822 3e3c 696d  idth="158px"><im
+00001460: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+00001470: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00001480: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
+00001490: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
+000014a0: 6173 7365 7473 2f63 6865 7373 5f6c 6967  assets/chess_lig
+000014b0: 6874 2e67 6966 2367 682d 6c69 6768 742d  ht.gif#gh-light-
+000014c0: 6d6f 6465 2d6f 6e6c 7922 2077 6964 7468  mode-only" width
+000014d0: 3d22 3135 3870 7822 3e7c 3c69 6d67 2073  ="158px">|<img s
+000014e0: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+000014f0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00001500: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00001510: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+00001520: 6574 732f 7368 6f67 695f 6461 726b 2e67  ets/shogi_dark.g
+00001530: 6966 2367 682d 6461 726b 2d6d 6f64 652d  if#gh-dark-mode-
+00001540: 6f6e 6c79 2220 7769 6474 683d 2231 3730  only" width="170
+00001550: 7078 223e 3c69 6d67 2073 7263 3d22 6874  px"><img src="ht
+00001560: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00001570: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00001580: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
+00001590: 6e2f 646f 6373 2f61 7373 6574 732f 7368  n/docs/assets/sh
+000015a0: 6f67 695f 6c69 6768 742e 6769 6623 6768  ogi_light.gif#gh
+000015b0: 2d6c 6967 6874 2d6d 6f64 652d 6f6e 6c79  -light-mode-only
+000015c0: 2220 7769 6474 683d 2231 3730 7078 223e  " width="170px">
+000015d0: 7c3c 696d 6720 7372 633d 2268 7474 7073  |<img src="https
+000015e0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+000015f0: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
+00001600: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
+00001610: 6f63 732f 6173 7365 7473 2f67 6f2d 3139  ocs/assets/go-19
+00001620: 7831 395f 6461 726b 2e67 6966 2367 682d  x19_dark.gif#gh-
+00001630: 6461 726b 2d6d 6f64 652d 6f6e 6c79 2220  dark-mode-only" 
+00001640: 7769 6474 683d 2231 3630 7078 223e 3c69  width="160px"><i
+00001650: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00001660: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00001670: 6e74 656e 742e 636f 6d2f 736f 7465 7473  ntent.com/sotets
+00001680: 756b 2f70 6778 2f6d 6169 6e2f 646f 6373  uk/pgx/main/docs
+00001690: 2f61 7373 6574 732f 676f 2d31 3978 3139  /assets/go-19x19
+000016a0: 5f6c 6967 6874 2e67 6966 2367 682d 6c69  _light.gif#gh-li
+000016b0: 6768 742d 6d6f 6465 2d6f 6e6c 7922 2077  ght-mode-only" w
+000016c0: 6964 7468 3d22 3136 3070 7822 3e7c 0a0a  idth="160px">|..
+000016d0: 0a55 7365 2060 7067 782e 6176 6169 6c61  .Use `pgx.availa
+000016e0: 626c 655f 656e 7673 2829 202d 3e20 5475  ble_envs() -> Tu
+000016f0: 706c 655b 456e 7649 645d 6020 746f 2073  ple[EnvId]` to s
+00001700: 6565 2074 6865 206c 6973 7420 6f66 2063  ee the list of c
+00001710: 7572 7265 6e74 6c79 2061 7661 696c 6162  urrently availab
+00001720: 6c65 2067 616d 6573 2e20 4769 7665 6e20  le games. Given 
+00001730: 616e 2060 3c45 6e76 4964 3e60 2c20 796f  an `<EnvId>`, yo
+00001740: 7520 6361 6e20 6372 6561 7465 2074 6865  u can create the
+00001750: 2065 6e76 6972 6f6e 6d65 6e74 2076 6961   environment via
+00001760: 0a0a 6060 6070 790a 3e3e 3e20 656e 7620  ..```py.>>> env 
+00001770: 3d20 7067 782e 6d61 6b65 283c 456e 7649  = pgx.make(<EnvI
+00001780: 643e 290a 6060 600a 0a7c 2047 616d 652f  d>).```..| Game/
+00001790: 456e 7649 6420 7c20 5669 7375 616c 697a  EnvId | Visualiz
+000017a0: 6174 696f 6e20 7c20 5665 7273 696f 6e20  ation | Version 
+000017b0: 7c20 4669 7665 2d77 6f72 6420 6465 7363  | Five-word desc
+000017c0: 7269 7074 696f 6e20 7c0a 7c3a 2d2d 2d3a  ription |.|:---:
+000017d0: 7c3a 2d2d 2d3a 7c3a 2d2d 2d3a 7c3a 2d2d  |:---:|:---:|:--
+000017e0: 2d3a 7c0a 7c3c 6120 6872 6566 3d22 6874  -:|.|<a href="ht
+000017f0: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+00001800: 6961 2e6f 7267 2f77 696b 692f 3230 3438  ia.org/wiki/2048
+00001810: 5f28 7669 6465 6f5f 6761 6d65 2922 3e32  _(video_game)">2
+00001820: 3034 383c 2f61 3e20 3c62 723e 2060 2232  048</a> <br> `"2
+00001830: 3034 3822 6020 7c3c 696d 6720 7372 633d  048"` |<img src=
+00001840: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00001850: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00001860: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
+00001870: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
+00001880: 2f32 3034 385f 6461 726b 2e67 6966 2220  /2048_dark.gif" 
+00001890: 7769 6474 683d 2236 3070 7822 3e3c 696d  width="60px"><im
+000018a0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+000018b0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+000018c0: 7465 6e74 2e63 6f6d 2f73 6f74 6574 7375  tent.com/sotetsu
+000018d0: 6b2f 7067 782f 6d61 696e 2f64 6f63 732f  k/pgx/main/docs/
+000018e0: 6173 7365 7473 2f32 3034 385f 6c69 6768  assets/2048_ligh
+000018f0: 742e 6769 6622 2077 6964 7468 3d22 3630  t.gif" width="60
+00001900: 7078 223e 7c20 6076 3060 207c 202a 4d65  px">| `v0` | *Me
+00001910: 7267 6520 7469 6c65 7320 746f 2063 7265  rge tiles to cre
+00001920: 6174 6520 3230 3438 2e2a 207c 0a7c 3c61  ate 2048.* |.|<a
+00001930: 2068 7265 663d 2268 7474 7073 3a2f 2f65   href="https://e
+00001940: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+00001950: 7769 6b69 2f44 2543 3525 3844 6275 7473  wiki/D%C5%8Dbuts
+00001960: 755f 7368 2543 3525 3844 6769 223e 416e  u_sh%C5%8Dgi">An
+00001970: 696d 616c 2053 686f 6769 3c2f 613e 3c62  imal Shogi</a><b
+00001980: 723e 6022 616e 696d 616c 5f73 686f 6769  r>`"animal_shogi
+00001990: 2260 207c 3c69 6d67 2073 7263 3d22 6874  "` |<img src="ht
+000019a0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+000019b0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+000019c0: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
+000019d0: 6e2f 646f 6373 2f61 7373 6574 732f 616e  n/docs/assets/an
+000019e0: 696d 616c 5f73 686f 6769 5f64 6172 6b2e  imal_shogi_dark.
+000019f0: 6769 6622 2077 6964 7468 3d22 3630 7078  gif" width="60px
+00001a00: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00001a10: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00001a20: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00001a30: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00001a40: 646f 6373 2f61 7373 6574 732f 616e 696d  docs/assets/anim
+00001a50: 616c 5f73 686f 6769 5f6c 6967 6874 2e67  al_shogi_light.g
+00001a60: 6966 2220 7769 6474 683d 2236 3070 7822  if" width="60px"
+00001a70: 3e7c 2020 6076 3060 207c 202a 416e 696d  >|  `v0` | *Anim
+00001a80: 616c 2d74 6865 6d65 6420 6368 696c 642d  al-themed child-
+00001a90: 6672 6965 6e64 6c79 2073 686f 6769 2e2a  friendly shogi.*
+00001aa0: 207c 0a7c 3c61 2068 7265 663d 2268 7474   |.|<a href="htt
+00001ab0: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
+00001ac0: 612e 6f72 672f 7769 6b69 2f42 6163 6b67  a.org/wiki/Backg
+00001ad0: 616d 6d6f 6e22 3e42 6163 6b67 616d 6d6f  ammon">Backgammo
+00001ae0: 6e3c 2f61 3e3c 6272 3e60 2262 6163 6b67  n</a><br>`"backg
+00001af0: 616d 6d6f 6e22 6020 7c3c 696d 6720 7372  ammon"` |<img sr
+00001b00: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00001b10: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00001b20: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
+00001b30: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
+00001b40: 7473 2f62 6163 6b67 616d 6d6f 6e5f 6461  ts/backgammon_da
+00001b50: 726b 2e67 6966 2220 7769 6474 683d 2236  rk.gif" width="6
+00001b60: 3070 7822 3e3c 696d 6720 7372 633d 2268  0px"><img src="h
+00001b70: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00001b80: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00001b90: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
+00001ba0: 696e 2f64 6f63 732f 6173 7365 7473 2f62  in/docs/assets/b
+00001bb0: 6163 6b67 616d 6d6f 6e5f 6c69 6768 742e  ackgammon_light.
+00001bc0: 6769 6622 2077 6964 7468 3d22 3630 7078  gif" width="60px
+00001bd0: 223e 7c20 6076 3060 207c 202a 4c75 636b  ">| `v0` | *Luck
+00001be0: 2061 6964 7320 6265 6172 696e 6720 6f66   aids bearing of
+00001bf0: 6620 6368 6563 6b65 7273 2e2a 207c 0a7c  f checkers.* |.|
+00001c00: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001c10: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
+00001c20: 672f 7769 6b69 2f43 6f6e 7472 6163 745f  g/wiki/Contract_
+00001c30: 6272 6964 6765 223e 4272 6964 6765 2062  bridge">Bridge b
+00001c40: 6964 6469 6e67 3c2f 613e 3c62 723e 6022  idding</a><br>`"
+00001c50: 6272 6964 6765 5f62 6964 6469 6e67 2260  bridge_bidding"`
+00001c60: 207c 3c69 6d67 2073 7263 3d22 6874 7470   |<img src="http
+00001c70: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00001c80: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00001c90: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00001ca0: 646f 6373 2f61 7373 6574 732f 6272 6964  docs/assets/brid
+00001cb0: 6765 5f62 6964 6469 6e67 5f64 6172 6b2e  ge_bidding_dark.
+00001cc0: 6769 6622 2077 6964 7468 3d22 3630 7078  gif" width="60px
+00001cd0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00001ce0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00001cf0: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00001d00: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00001d10: 646f 6373 2f61 7373 6574 732f 6272 6964  docs/assets/brid
+00001d20: 6765 5f62 6964 6469 6e67 5f6c 6967 6874  ge_bidding_light
+00001d30: 2e67 6966 2220 7769 6474 683d 2236 3070  .gif" width="60p
+00001d40: 7822 3e7c 2060 7630 6020 7c20 2a50 6172  x">| `v0` | *Par
+00001d50: 746e 6572 7320 6578 6368 616e 6765 2069  tners exchange i
+00001d60: 6e66 6f72 6d61 7469 6f6e 2076 6961 2062  nformation via b
+00001d70: 6964 732e 2a20 7c0a 7c3c 6120 6872 6566  ids.* |.|<a href
+00001d80: 3d22 6874 7470 733a 2f2f 656e 2e77 696b  ="https://en.wik
+00001d90: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+00001da0: 4368 6573 7322 3e43 6865 7373 3c2f 613e  Chess">Chess</a>
+00001db0: 3c62 723e 6022 6368 6573 7322 6020 7c3c  <br>`"chess"` |<
+00001dc0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001dd0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00001de0: 6f6e 7465 6e74 2e63 6f6d 2f73 6f74 6574  ontent.com/sotet
+00001df0: 7375 6b2f 7067 782f 6d61 696e 2f64 6f63  suk/pgx/main/doc
+00001e00: 732f 6173 7365 7473 2f63 6865 7373 5f64  s/assets/chess_d
+00001e10: 6172 6b2e 6769 6622 2077 6964 7468 3d22  ark.gif" width="
+00001e20: 3630 7078 223e 3c69 6d67 2073 7263 3d22  60px"><img src="
+00001e30: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+00001e40: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+00001e50: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
+00001e60: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
+00001e70: 6368 6573 735f 6c69 6768 742e 6769 6622  chess_light.gif"
+00001e80: 2077 6964 7468 3d22 3630 7078 223e 7c20   width="60px">| 
+00001e90: 6076 3160 207c 202a 4368 6563 6b6d 6174  `v1` | *Checkmat
+00001ea0: 6520 6f70 706f 6e65 6e74 2773 206b 696e  e opponent's kin
+00001eb0: 6720 746f 2077 696e 2e2a 207c 0a7c 3c61  g to win.* |.|<a
+00001ec0: 2068 7265 663d 2268 7474 7073 3a2f 2f65   href="https://e
+00001ed0: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+00001ee0: 7769 6b69 2f43 6f6e 6e65 6374 5f46 6f75  wiki/Connect_Fou
+00001ef0: 7222 3e43 6f6e 6e65 6374 2046 6f75 723c  r">Connect Four<
+00001f00: 2f61 3e3c 6272 3e60 2263 6f6e 6e65 6374  /a><br>`"connect
+00001f10: 5f66 6f75 7222 6020 7c3c 696d 6720 7372  _four"` |<img sr
+00001f20: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00001f30: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00001f40: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
+00001f50: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
+00001f60: 7473 2f63 6f6e 6e65 6374 5f66 6f75 725f  ts/connect_four_
+00001f70: 6461 726b 2e67 6966 2220 7769 6474 683d  dark.gif" width=
+00001f80: 2236 3070 7822 3e3c 696d 6720 7372 633d  "60px"><img src=
+00001f90: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00001fa0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00001fb0: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
+00001fc0: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
+00001fd0: 2f63 6f6e 6e65 6374 5f66 6f75 725f 6c69  /connect_four_li
+00001fe0: 6768 742e 6769 6622 2077 6964 7468 3d22  ght.gif" width="
+00001ff0: 3630 7078 223e 7c20 6076 3060 207c 202a  60px">| `v0` | *
+00002000: 436f 6e6e 6563 7420 6469 7363 732c 2077  Connect discs, w
+00002010: 696e 2077 6974 6820 666f 7572 2e2a 207c  in with four.* |
+00002020: 0a7c 3c61 2068 7265 663d 2268 7474 7073  .|<a href="https
+00002030: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+00002040: 6f72 672f 7769 6b69 2f4d 696e 6963 6865  org/wiki/Miniche
+00002050: 7373 223e 4761 7264 6e65 7220 4368 6573  ss">Gardner Ches
+00002060: 733c 2f61 3e3c 6272 3e60 2267 6172 646e  s</a><br>`"gardn
+00002070: 6572 5f63 6865 7373 2260 7c3c 696d 6720  er_chess"`|<img 
+00002080: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
+00002090: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000020a0: 6e74 2e63 6f6d 2f73 6f74 6574 7375 6b2f  nt.com/sotetsuk/
+000020b0: 7067 782f 6d61 696e 2f64 6f63 732f 6173  pgx/main/docs/as
+000020c0: 7365 7473 2f67 6172 646e 6572 5f63 6865  sets/gardner_che
+000020d0: 7373 5f64 6172 6b2e 6769 6622 2077 6964  ss_dark.gif" wid
+000020e0: 7468 3d22 3630 7078 223e 3c69 6d67 2073  th="60px"><img s
+000020f0: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00002100: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002110: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00002120: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+00002130: 6574 732f 6761 7264 6e65 725f 6368 6573  ets/gardner_ches
+00002140: 735f 6c69 6768 742e 6769 6622 2077 6964  s_light.gif" wid
+00002150: 7468 3d22 3630 7078 223e 7c20 6076 3060  th="60px">| `v0`
+00002160: 207c 202a 3578 3520 6368 6573 7320 7661   | *5x5 chess va
+00002170: 7269 616e 742c 2065 7863 6c75 6469 6e67  riant, excluding
+00002180: 2063 6173 746c 696e 672e 2a20 7c0a 7c3c   castling.* |.|<
+00002190: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000021a0: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
+000021b0: 2f77 696b 692f 476f 5f28 6761 6d65 2922  /wiki/Go_(game)"
+000021c0: 3e47 6f3c 2f61 3e3c 6272 3e60 2267 6f5f  >Go</a><br>`"go_
+000021d0: 3978 3922 6020 6022 676f 5f31 3978 3139  9x9"` `"go_19x19
+000021e0: 2260 207c 3c69 6d67 2073 7263 3d22 6874  "` |<img src="ht
+000021f0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+00002200: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+00002210: 736f 7465 7473 756b 2f70 6778 2f6d 6169  sotetsuk/pgx/mai
+00002220: 6e2f 646f 6373 2f61 7373 6574 732f 676f  n/docs/assets/go
+00002230: 2d31 3978 3139 5f64 6172 6b2e 6769 6622  -19x19_dark.gif"
+00002240: 2077 6964 7468 3d22 3630 7078 223e 3c69   width="60px"><i
+00002250: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00002260: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+00002270: 6e74 656e 742e 636f 6d2f 736f 7465 7473  ntent.com/sotets
+00002280: 756b 2f70 6778 2f6d 6169 6e2f 646f 6373  uk/pgx/main/docs
+00002290: 2f61 7373 6574 732f 676f 2d31 3978 3139  /assets/go-19x19
+000022a0: 5f6c 6967 6874 2e67 6966 2220 7769 6474  _light.gif" widt
+000022b0: 683d 2236 3070 7822 3e7c 2060 7630 6020  h="60px">| `v0` 
+000022c0: 7c20 2a53 7472 6174 6567 6963 616c 6c79  | *Strategically
+000022d0: 2070 6c61 6365 2073 746f 6e65 732c 2063   place stones, c
+000022e0: 6c61 696d 2074 6572 7269 746f 7279 2e2a  laim territory.*
+000022f0: 207c 0a7c 3c61 2068 7265 663d 2268 7474   |.|<a href="htt
+00002300: 7073 3a2f 2f65 6e2e 7769 6b69 7065 6469  ps://en.wikipedi
+00002310: 612e 6f72 672f 7769 6b69 2f48 6578 5f28  a.org/wiki/Hex_(
+00002320: 626f 6172 645f 6761 6d65 2922 3e48 6578  board_game)">Hex
+00002330: 3c2f 613e 3c62 723e 6022 6865 7822 6020  </a><br>`"hex"` 
+00002340: 7c3c 696d 6720 7372 633d 2268 7474 7073  |<img src="https
+00002350: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00002360: 7263 6f6e 7465 6e74 2e63 6f6d 2f73 6f74  rcontent.com/sot
+00002370: 6574 7375 6b2f 7067 782f 6d61 696e 2f64  etsuk/pgx/main/d
+00002380: 6f63 732f 6173 7365 7473 2f68 6578 5f64  ocs/assets/hex_d
+00002390: 6172 6b2e 6769 6622 2077 6964 7468 3d22  ark.gif" width="
+000023a0: 3630 7078 223e 3c69 6d67 2073 7263 3d22  60px"><img src="
+000023b0: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+000023c0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+000023d0: 6d2f 736f 7465 7473 756b 2f70 6778 2f6d  m/sotetsuk/pgx/m
+000023e0: 6169 6e2f 646f 6373 2f61 7373 6574 732f  ain/docs/assets/
+000023f0: 6865 785f 6c69 6768 742e 6769 6622 2077  hex_light.gif" w
+00002400: 6964 7468 3d22 3630 7078 223e 7c20 6076  idth="60px">| `v
+00002410: 3060 207c 202a 436f 6e6e 6563 7420 6f70  0` | *Connect op
+00002420: 706f 7369 7465 2073 6964 6573 2c20 626c  posite sides, bl
+00002430: 6f63 6b20 6f70 706f 6e65 6e74 2e2a 207c  ock opponent.* |
+00002440: 0a7c 3c61 2068 7265 663d 2268 7474 7073  .|<a href="https
+00002450: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+00002460: 6f72 672f 7769 6b69 2f4b 7568 6e5f 706f  org/wiki/Kuhn_po
+00002470: 6b65 7222 3e4b 7568 6e20 506f 6b65 723c  ker">Kuhn Poker<
+00002480: 2f61 3e3c 6272 3e60 226b 7568 6e5f 706f  /a><br>`"kuhn_po
+00002490: 6b65 7222 6020 7c3c 696d 6720 7372 633d  ker"` |<img src=
+000024a0: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+000024b0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+000024c0: 6f6d 2f73 6f74 6574 7375 6b2f 7067 782f  om/sotetsuk/pgx/
+000024d0: 6d61 696e 2f64 6f63 732f 6173 7365 7473  main/docs/assets
+000024e0: 2f6b 7568 6e5f 706f 6b65 725f 6461 726b  /kuhn_poker_dark
+000024f0: 2e67 6966 2220 7769 6474 683d 2236 3070  .gif" width="60p
+00002500: 7822 3e3c 696d 6720 7372 633d 2268 7474  x"><img src="htt
+00002510: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00002520: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
+00002530: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
+00002540: 2f64 6f63 732f 6173 7365 7473 2f6b 7568  /docs/assets/kuh
+00002550: 6e5f 706f 6b65 725f 6c69 6768 742e 6769  n_poker_light.gi
+00002560: 6622 2077 6964 7468 3d22 3630 7078 223e  f" width="60px">
+00002570: 7c20 6076 3060 207c 202a 5468 7265 652d  | `v0` | *Three-
+00002580: 6361 7264 2062 6574 7469 6e67 2061 6e64  card betting and
+00002590: 2062 6c75 6666 696e 6720 6761 6d65 2e2a   bluffing game.*
+000025a0: 207c 0a7c 3c61 2068 7265 663d 2268 7474   |.|<a href="htt
+000025b0: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+000025c0: 6273 2f31 3230 372e 3134 3131 223e 4c65  bs/1207.1411">Le
+000025d0: 6475 6320 686f 6c64 2765 6d3c 2f61 3e3c  duc hold'em</a><
+000025e0: 6272 3e60 226c 6564 7563 5f68 6f6c 6465  br>`"leduc_holde
+000025f0: 6d22 6020 7c3c 696d 6720 7372 633d 2268  m"` |<img src="h
+00002600: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00002610: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00002620: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
+00002630: 696e 2f64 6f63 732f 6173 7365 7473 2f6c  in/docs/assets/l
+00002640: 6564 7563 5f68 6f6c 6465 6d5f 6461 726b  educ_holdem_dark
+00002650: 2e67 6966 2220 7769 6474 683d 2236 3070  .gif" width="60p
+00002660: 7822 3e3c 696d 6720 7372 633d 2268 7474  x"><img src="htt
+00002670: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00002680: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
+00002690: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
+000026a0: 2f64 6f63 732f 6173 7365 7473 2f6c 6564  /docs/assets/led
+000026b0: 7563 5f68 6f6c 6465 6d5f 6c69 6768 742e  uc_holdem_light.
+000026c0: 6769 6622 2077 6964 7468 3d22 3630 7078  gif" width="60px
+000026d0: 223e 7c20 6076 3060 207c 202a 5477 6f2d  ">| `v0` | *Two-
+000026e0: 7375 6974 2c20 6c69 6d69 7465 6420 6465  suit, limited de
+000026f0: 636b 2070 6f6b 6572 2e2a 207c 0a7c 3c61  ck poker.* |.|<a
+00002700: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00002710: 6974 6875 622e 636f 6d2f 6b65 6e6a 796f  ithub.com/kenjyo
+00002720: 756e 672f 4d69 6e41 7461 7222 3e4d 696e  ung/MinAtar">Min
+00002730: 4174 6172 2f41 7374 6572 6978 3c2f 613e  Atar/Asterix</a>
+00002740: 3c62 723e 6022 6d69 6e61 7461 722d 6173  <br>`"minatar-as
+00002750: 7465 7269 7822 6020 7c3c 696d 6720 7372  terix"` |<img sr
+00002760: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00002770: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00002780: 2e63 6f6d 2f73 6f74 6574 7375 6b2f 7067  .com/sotetsuk/pg
+00002790: 782f 6d61 696e 2f64 6f63 732f 6173 7365  x/main/docs/asse
+000027a0: 7473 2f6d 696e 6174 6172 2d61 7374 6572  ts/minatar-aster
+000027b0: 6978 2e67 6966 2220 7769 6474 683d 2235  ix.gif" width="5
+000027c0: 3070 7822 3e7c 2060 7630 6020 7c20 2a41  0px">| `v0` | *A
+000027d0: 766f 6964 2065 6e65 6d69 6573 2c20 636f  void enemies, co
+000027e0: 6c6c 6563 7420 7472 6561 7375 7265 2c20  llect treasure, 
+000027f0: 7375 7276 6976 652e 2a20 7c0a 7c3c 6120  survive.* |.|<a 
+00002800: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00002810: 7468 7562 2e63 6f6d 2f6b 656e 6a79 6f75  thub.com/kenjyou
+00002820: 6e67 2f4d 696e 4174 6172 223e 4d69 6e41  ng/MinAtar">MinA
+00002830: 7461 722f 4272 6561 6b6f 7574 3c2f 613e  tar/Breakout</a>
+00002840: 3c62 723e 6022 6d69 6e61 7461 722d 6272  <br>`"minatar-br
+00002850: 6561 6b6f 7574 2260 207c 3c69 6d67 2073  eakout"` |<img s
+00002860: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00002870: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002880: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00002890: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+000028a0: 6574 732f 6d69 6e61 7461 722d 6272 6561  ets/minatar-brea
+000028b0: 6b6f 7574 2e67 6966 2220 7769 6474 683d  kout.gif" width=
+000028c0: 2235 3070 7822 3e7c 2060 7630 6020 7c20  "50px">| `v0` | 
+000028d0: 2a50 6164 646c 652c 2062 616c 6c2c 2062  *Paddle, ball, b
+000028e0: 7269 636b 732c 2062 6f75 6e63 652c 2063  ricks, bounce, c
+000028f0: 6c65 6172 2e2a 207c 0a7c 3c61 2068 7265  lear.* |.|<a hre
+00002900: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00002910: 622e 636f 6d2f 6b65 6e6a 796f 756e 672f  b.com/kenjyoung/
+00002920: 4d69 6e41 7461 7222 3e4d 696e 4174 6172  MinAtar">MinAtar
+00002930: 2f46 7265 6577 6179 3c2f 613e 3c62 723e  /Freeway</a><br>
+00002940: 6022 6d69 6e61 7461 722d 6672 6565 7761  `"minatar-freewa
+00002950: 7922 6020 7c3c 696d 6720 7372 633d 2268  y"` |<img src="h
+00002960: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00002970: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00002980: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
+00002990: 696e 2f64 6f63 732f 6173 7365 7473 2f6d  in/docs/assets/m
+000029a0: 696e 6174 6172 2d66 7265 6577 6179 2e67  inatar-freeway.g
+000029b0: 6966 2220 7769 6474 683d 2235 3070 7822  if" width="50px"
+000029c0: 3e7c 2060 7630 6020 7c20 2a44 6f64 6769  >| `v0` | *Dodgi
+000029d0: 6e67 2063 6172 732c 2063 6c69 6d62 696e  ng cars, climbin
+000029e0: 6720 7570 2066 7265 6577 6179 2e2a 207c  g up freeway.* |
+000029f0: 0a7c 3c61 2068 7265 663d 2268 7474 7073  .|<a href="https
+00002a00: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b65  ://github.com/ke
+00002a10: 6e6a 796f 756e 672f 4d69 6e41 7461 7222  njyoung/MinAtar"
+00002a20: 3e4d 696e 4174 6172 2f53 6561 7175 6573  >MinAtar/Seaques
+00002a30: 743c 2f61 3e3c 6272 3e60 226d 696e 6174  t</a><br>`"minat
+00002a40: 6172 2d73 6561 7175 6573 7422 6020 7c3c  ar-seaquest"` |<
+00002a50: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00002a60: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00002a70: 6f6e 7465 6e74 2e63 6f6d 2f73 6f74 6574  ontent.com/sotet
+00002a80: 7375 6b2f 7067 782f 6d61 696e 2f64 6f63  suk/pgx/main/doc
+00002a90: 732f 6173 7365 7473 2f6d 696e 6174 6172  s/assets/minatar
+00002aa0: 2d73 6561 7175 6573 742e 6769 6622 2077  -seaquest.gif" w
+00002ab0: 6964 7468 3d22 3530 7078 223e 7c20 6076  idth="50px">| `v
+00002ac0: 3060 207c 202a 556e 6465 7277 6174 6572  0` | *Underwater
+00002ad0: 2073 7562 6d61 7269 6e65 2072 6573 6375   submarine rescu
+00002ae0: 6520 616e 6420 636f 6d62 6174 2e2a 207c  e and combat.* |
+00002af0: 0a7c 3c61 2068 7265 663d 2268 7474 7073  .|<a href="https
+00002b00: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b65  ://github.com/ke
+00002b10: 6e6a 796f 756e 672f 4d69 6e41 7461 7222  njyoung/MinAtar"
+00002b20: 3e4d 696e 4174 6172 2f53 7061 6365 496e  >MinAtar/SpaceIn
+00002b30: 7661 6465 7273 3c2f 613e 3c62 723e 6022  vaders</a><br>`"
+00002b40: 6d69 6e61 7461 722d 7370 6163 655f 696e  minatar-space_in
+00002b50: 7661 6465 7273 2260 207c 3c69 6d67 2073  vaders"` |<img s
+00002b60: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00002b70: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002b80: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00002b90: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+00002ba0: 6574 732f 6d69 6e61 7461 722d 7370 6163  ets/minatar-spac
+00002bb0: 655f 696e 7661 6465 7273 2e67 6966 2220  e_invaders.gif" 
+00002bc0: 7769 6474 683d 2235 3070 7822 3e7c 2060  width="50px">| `
+00002bd0: 7630 6020 7c20 2a41 6c69 656e 2073 686f  v0` | *Alien sho
+00002be0: 6f74 6572 2067 616d 652c 2064 6f64 6765  oter game, dodge
+00002bf0: 2062 756c 6c65 7473 2e2a 207c 0a7c 3c61   bullets.* |.|<a
+00002c00: 2068 7265 663d 2268 7474 7073 3a2f 2f65   href="https://e
+00002c10: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+00002c20: 7769 6b69 2f52 6576 6572 7369 223e 4f74  wiki/Reversi">Ot
+00002c30: 6865 6c6c 6f3c 2f61 3e3c 6272 3e60 226f  hello</a><br>`"o
+00002c40: 7468 656c 6c6f 2260 207c 3c69 6d67 2073  thello"` |<img s
+00002c50: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00002c60: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002c70: 742e 636f 6d2f 736f 7465 7473 756b 2f70  t.com/sotetsuk/p
+00002c80: 6778 2f6d 6169 6e2f 646f 6373 2f61 7373  gx/main/docs/ass
+00002c90: 6574 732f 6f74 6865 6c6c 6f5f 6461 726b  ets/othello_dark
+00002ca0: 2e67 6966 2220 7769 6474 683d 2236 3070  .gif" width="60p
+00002cb0: 7822 3e3c 696d 6720 7372 633d 2268 7474  x"><img src="htt
+00002cc0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00002cd0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
+00002ce0: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
+00002cf0: 2f64 6f63 732f 6173 7365 7473 2f6f 7468  /docs/assets/oth
+00002d00: 656c 6c6f 5f6c 6967 6874 2e67 6966 2220  ello_light.gif" 
+00002d10: 7769 6474 683d 2236 3070 7822 3e7c 2060  width="60px">| `
+00002d20: 7630 6020 7c20 2a46 6c69 7020 616e 6420  v0` | *Flip and 
+00002d30: 636f 6e71 7565 7220 6f70 706f 6e65 6e74  conquer opponent
+00002d40: 2773 2070 6965 6365 732e 2a20 7c0a 7c3c  's pieces.* |.|<
+00002d50: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00002d60: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
+00002d70: 2f77 696b 692f 5368 6f67 6922 3e53 686f  /wiki/Shogi">Sho
+00002d80: 6769 3c2f 613e 3c62 723e 6022 7368 6f67  gi</a><br>`"shog
+00002d90: 6922 6020 7c3c 696d 6720 7372 633d 2268  i"` |<img src="h
+00002da0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00002db0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00002dc0: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
+00002dd0: 696e 2f64 6f63 732f 6173 7365 7473 2f73  in/docs/assets/s
+00002de0: 686f 6769 5f64 6172 6b2e 6769 6622 2077  hogi_dark.gif" w
+00002df0: 6964 7468 3d22 3630 7078 223e 3c69 6d67  idth="60px"><img
+00002e00: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00002e10: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00002e20: 656e 742e 636f 6d2f 736f 7465 7473 756b  ent.com/sotetsuk
+00002e30: 2f70 6778 2f6d 6169 6e2f 646f 6373 2f61  /pgx/main/docs/a
+00002e40: 7373 6574 732f 7368 6f67 695f 6c69 6768  ssets/shogi_ligh
+00002e50: 742e 6769 6622 2077 6964 7468 3d22 3630  t.gif" width="60
+00002e60: 7078 223e 207c 2060 7630 6020 7c20 2a4a  px"> | `v0` | *J
+00002e70: 6170 616e 6573 6520 6368 6573 7320 7769  apanese chess wi
+00002e80: 7468 2063 6170 7475 7265 6420 7069 6563  th captured piec
+00002e90: 6573 2e2a 207c 0a7c 3c61 2068 7265 663d  es.* |.|<a href=
+00002ea0: 2268 7474 7073 3a2f 2f73 7567 6f72 6f6b  "https://sugorok
+00002eb0: 7579 612e 6a70 2f70 2f73 757a 756d 652d  uya.jp/p/suzume-
+00002ec0: 6a6f 6e67 223e 5370 6172 726f 7720 4d61  jong">Sparrow Ma
+00002ed0: 686a 6f6e 673c 2f61 3e3c 6272 3e60 2273  hjong</a><br>`"s
+00002ee0: 7061 7272 6f77 5f6d 6168 6a6f 6e67 2260  parrow_mahjong"`
+00002ef0: 207c 3c69 6d67 2073 7263 3d22 6874 7470   |<img src="http
+00002f00: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00002f10: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00002f20: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00002f30: 646f 6373 2f61 7373 6574 732f 7370 6172  docs/assets/spar
+00002f40: 726f 775f 6d61 686a 6f6e 675f 6461 726b  row_mahjong_dark
+00002f50: 2e73 7667 2220 7769 6474 683d 2236 3070  .svg" width="60p
+00002f60: 7822 3e3c 696d 6720 7372 633d 2268 7474  x"><img src="htt
+00002f70: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00002f80: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
+00002f90: 6f74 6574 7375 6b2f 7067 782f 6d61 696e  otetsuk/pgx/main
+00002fa0: 2f64 6f63 732f 6173 7365 7473 2f73 7061  /docs/assets/spa
+00002fb0: 7272 6f77 5f6d 6168 6a6f 6e67 5f6c 6967  rrow_mahjong_lig
+00002fc0: 6874 2e73 7667 2220 7769 6474 683d 2236  ht.svg" width="6
+00002fd0: 3070 7822 3e7c 2020 6076 3060 207c 202a  0px">|  `v0` | *
+00002fe0: 4120 7369 6d70 6c69 6669 6564 2c20 6368  A simplified, ch
+00002ff0: 696c 6472 656e 2d66 7269 656e 646c 7920  ildren-friendly 
+00003000: 4d61 686a 6f6e 672e 2a20 7c0a 7c3c 6120  Mahjong.* |.|<a 
+00003010: 6872 6566 3d22 6874 7470 733a 2f2f 656e  href="https://en
+00003020: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+00003030: 696b 692f 5469 632d 7461 632d 746f 6522  iki/Tic-tac-toe"
+00003040: 3e54 6963 2d74 6163 2d74 6f65 3c2f 613e  >Tic-tac-toe</a>
+00003050: 3c62 723e 6022 7469 635f 7461 635f 746f  <br>`"tic_tac_to
+00003060: 6522 6020 7c3c 696d 6720 7372 633d 2268  e"` |<img src="h
+00003070: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00003080: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00003090: 2f73 6f74 6574 7375 6b2f 7067 782f 6d61  /sotetsuk/pgx/ma
+000030a0: 696e 2f64 6f63 732f 6173 7365 7473 2f74  in/docs/assets/t
+000030b0: 6963 5f74 6163 5f74 6f65 5f64 6172 6b2e  ic_tac_toe_dark.
+000030c0: 6769 6622 2077 6964 7468 3d22 3630 7078  gif" width="60px
+000030d0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+000030e0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+000030f0: 6572 636f 6e74 656e 742e 636f 6d2f 736f  ercontent.com/so
+00003100: 7465 7473 756b 2f70 6778 2f6d 6169 6e2f  tetsuk/pgx/main/
+00003110: 646f 6373 2f61 7373 6574 732f 7469 635f  docs/assets/tic_
+00003120: 7461 635f 746f 655f 6c69 6768 742e 6769  tac_toe_light.gi
+00003130: 6622 2077 6964 7468 3d22 3630 7078 223e  f" width="60px">
+00003140: 7c20 6076 3060 207c 202a 5468 7265 6520  | `v0` | *Three 
+00003150: 696e 2061 2072 6f77 2077 696e 732e 2a20  in a row wins.* 
+00003160: 7c0a 0a2d 203c 6120 6872 6566 3d22 6874  |..- <a href="ht
+00003170: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+00003180: 6961 2e6f 7267 2f77 696b 692f 4a61 7061  ia.org/wiki/Japa
+00003190: 6e65 7365 5f6d 6168 6a6f 6e67 223e 4d61  nese_mahjong">Ma
+000031a0: 686a 6f6e 673c 2f61 3e20 656e 7669 726f  hjong</a> enviro
+000031b0: 6e6d 656e 7473 2061 7265 2075 6e64 6572  nments are under
+000031c0: 2064 6576 656c 6f70 6d65 6e74 20f0 9f9a   development ...
+000031d0: a720 4966 2079 6f75 2068 6176 6520 616e  . If you have an
+000031e0: 7920 7265 7175 6573 7473 2066 6f72 206e  y requests for n
+000031f0: 6577 2065 6e76 6972 6f6e 6d65 6e74 732c  ew environments,
+00003200: 2070 6c65 6173 6520 6c65 7420 7573 206b   please let us k
+00003210: 6e6f 7720 6279 205b 6f70 656e 696e 6720  now by [opening 
+00003220: 616e 2069 7373 7565 5d28 6874 7470 733a  an issue](https:
+00003230: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6f74  //github.com/sot
+00003240: 6574 7375 6b2f 7067 782f 6973 7375 6573  etsuk/pgx/issues
+00003250: 2f6e 6577 290a 2d20 4669 7665 2d77 6f72  /new).- Five-wor
+00003260: 6420 6465 7363 7269 7074 696f 6e73 2077  d descriptions w
+00003270: 6572 6520 6765 6e65 7261 7465 6420 6279  ere generated by
+00003280: 205b 4368 6174 4750 545d 2868 7474 7073   [ChatGPT](https
+00003290: 3a2f 2f63 6861 742e 6f70 656e 6169 2e63  ://chat.openai.c
+000032a0: 6f6d 2f29 20f0 9fa4 960a 0a23 2323 2056  om/) ......### V
+000032b0: 6572 7369 6f6e 696e 6720 706f 6c69 6379  ersioning policy
+000032c0: 0a0a 4561 6368 2065 6e76 6972 6f6e 6d65  ..Each environme
+000032d0: 6e74 2069 7320 7665 7273 696f 6e65 642c  nt is versioned,
+000032e0: 2061 6e64 2074 6865 2076 6572 7369 6f6e   and the version
+000032f0: 2069 7320 696e 6372 656d 656e 7465 6420   is incremented 
+00003300: 7768 656e 2074 6865 7265 2061 7265 2063  when there are c
+00003310: 6861 6e67 6573 2074 6861 7420 6166 6665  hanges that affe
+00003320: 6374 2074 6865 2070 6572 666f 726d 616e  ct the performan
+00003330: 6365 206f 6620 6167 656e 7473 206f 7220  ce of agents or 
+00003340: 7768 656e 2074 6865 7265 2061 7265 2063  when there are c
+00003350: 6861 6e67 6573 2074 6861 7420 6172 6520  hanges that are 
+00003360: 6e6f 7420 6261 636b 7761 7264 2063 6f6d  not backward com
+00003370: 7061 7469 626c 6520 7769 7468 2074 6865  patible with the
+00003380: 2041 5049 2e0a 4966 2079 6f75 2077 616e   API..If you wan
+00003390: 7420 746f 2070 7572 7375 6520 636f 6d70  t to pursue comp
+000033a0: 6c65 7465 2072 6570 726f 6475 6369 6269  lete reproducibi
+000033b0: 6c69 7479 2c20 7765 2072 6563 6f6d 6d65  lity, we recomme
+000033c0: 6e64 2074 6861 7420 796f 7520 6368 6563  nd that you chec
+000033d0: 6b20 7468 6520 7665 7273 696f 6e20 6f66  k the version of
+000033e0: 2050 6778 2061 6e64 2065 6163 6820 656e   Pgx and each en
+000033f0: 7669 726f 6e6d 656e 7420 6173 2066 6f6c  vironment as fol
+00003400: 6c6f 7773 3a0a 0a60 6060 7079 0a3e 3e3e  lows:..```py.>>>
+00003410: 2070 6778 2e5f 5f76 6572 7369 6f6e 5f5f   pgx.__version__
+00003420: 0a27 312e 302e 3027 0a3e 3e3e 2065 6e76  .'1.0.0'.>>> env
+00003430: 2e76 6572 7369 6f6e 0a27 7630 270a 6060  .version.'v0'.``
+00003440: 600a 0a23 2320 5365 6520 616c 736f 0a0a  `..## See also..
+00003450: 5067 7820 6973 2069 6e74 656e 6465 6420  Pgx is intended 
+00003460: 746f 2063 6f6d 706c 656d 656e 7420 7468  to complement th
+00003470: 6573 6520 2a2a 4a41 582d 6e61 7469 7665  ese **JAX-native
+00003480: 2065 6e76 6972 6f6e 6d65 6e74 732a 2a20   environments** 
+00003490: 7769 7468 2028 636c 6173 7369 6329 2062  with (classic) b
+000034a0: 6f61 7264 2067 616d 6520 7375 6974 733a  oard game suits:
+000034b0: 0a0a 2d20 5b52 6f62 6572 7454 4c61 6e67  ..- [RobertTLang
+000034c0: 652f 6779 6d6e 6178 5d28 6874 7470 733a  e/gymnax](https:
+000034d0: 2f2f 6769 7468 7562 2e63 6f6d 2f52 6f62  //github.com/Rob
+000034e0: 6572 7454 4c61 6e67 652f 6779 6d6e 6178  ertTLange/gymnax
+000034f0: 293a 204a 4158 2069 6d70 6c65 6d65 6e74  ): JAX implement
+00003500: 6174 696f 6e20 6f66 2070 6f70 756c 6172  ation of popular
+00003510: 2052 4c20 656e 7669 726f 6e6d 656e 7473   RL environments
+00003520: 2028 5b63 6c61 7373 6963 2063 6f6e 7472   ([classic contr
+00003530: 6f6c 5d28 6874 7470 733a 2f2f 6779 6d6e  ol](https://gymn
+00003540: 6173 6975 6d2e 6661 7261 6d61 2e6f 7267  asium.farama.org
+00003550: 2f65 6e76 6972 6f6e 6d65 6e74 732f 636c  /environments/cl
+00003560: 6173 7369 635f 636f 6e74 726f 6c29 2c20  assic_control), 
+00003570: 5b62 7375 6974 655d 2868 7474 7073 3a2f  [bsuite](https:/
+00003580: 2f67 6974 6875 622e 636f 6d2f 6465 6570  /github.com/deep
+00003590: 6d69 6e64 2f62 7375 6974 6529 2c20 4d69  mind/bsuite), Mi
+000035a0: 6e41 7461 722c 2065 7463 2920 616e 6420  nAtar, etc) and 
+000035b0: 6d65 7461 2052 4c20 7461 736b 730a 2d20  meta RL tasks.- 
+000035c0: 5b67 6f6f 676c 652f 6272 6178 5d28 6874  [google/brax](ht
+000035d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000035e0: 2f67 6f6f 676c 652f 6272 6178 293a 2052  /google/brax): R
+000035f0: 6967 6964 626f 6479 2070 6879 7369 6373  igidbody physics
+00003600: 2073 696d 756c 6174 696f 6e20 696e 204a   simulation in J
+00003610: 4158 2061 6e64 2063 6f6e 7469 6e75 6f75  AX and continuou
+00003620: 732d 7370 6163 6520 524c 2074 6173 6b73  s-space RL tasks
+00003630: 2028 616e 742c 2066 6574 6368 2c20 6875   (ant, fetch, hu
+00003640: 6d61 6e6f 6964 2c20 6574 6329 0a2d 205b  manoid, etc).- [
+00003650: 696e 7374 6164 6565 7061 692f 6a75 6d61  instadeepai/juma
+00003660: 6e6a 695d 2868 7474 7073 3a2f 2f67 6974  nji](https://git
+00003670: 6875 622e 636f 6d2f 696e 7374 6164 6565  hub.com/instadee
+00003680: 7061 692f 6a75 6d61 6e6a 6929 3a20 4120  pai/jumanji): A 
+00003690: 7375 6974 6520 6f66 2064 6976 6572 7365  suite of diverse
+000036a0: 2061 6e64 2063 6861 6c6c 656e 6769 6e67   and challenging
+000036b0: 0a20 2020 2052 4c20 656e 7669 726f 6e6d  .    RL environm
+000036c0: 656e 7473 2069 6e20 4a41 5820 2862 696e  ents in JAX (bin
+000036d0: 2d70 6163 6b69 6e67 2c20 726f 7574 696e  -packing, routin
+000036e0: 6720 7072 6f62 6c65 6d73 2c20 6574 6329  g problems, etc)
+000036f0: 0a0a 436f 6d62 696e 696e 6720 5067 7820  ..Combining Pgx 
+00003700: 7769 7468 2074 6865 7365 202a 2a4a 4158  with these **JAX
+00003710: 2d6e 6174 6976 6520 616c 676f 7269 7468  -native algorith
+00003720: 6d73 2f69 6d70 6c65 6d65 6e74 6174 696f  ms/implementatio
+00003730: 6e73 2a2a 206d 6967 6874 2062 6520 616e  ns** might be an
+00003740: 2069 6e74 6572 6573 7469 6e67 2064 6972   interesting dir
+00003750: 6563 7469 6f6e 3a0a 0a2d 205b 416e 616b  ection:..- [Anak
+00003760: 696e 2066 7261 6d65 776f 726b 5d28 6874  in framework](ht
+00003770: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
+00003780: 6162 732f 3231 3034 2e30 3632 3732 293a  abs/2104.06272):
+00003790: 2048 6967 686c 7920 6566 6669 6369 656e   Highly efficien
+000037a0: 7420 524c 2066 7261 6d65 776f 726b 2074  t RL framework t
+000037b0: 6861 7420 776f 726b 7320 7769 7468 204a  hat works with J
+000037c0: 4158 2d6e 6174 6976 6520 656e 7669 726f  AX-native enviro
+000037d0: 6e6d 656e 7473 206f 6e20 5450 5573 0a2d  nments on TPUs.-
+000037e0: 205b 6465 6570 6d69 6e64 2f6d 6374 785d   [deepmind/mctx]
+000037f0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00003800: 636f 6d2f 6465 6570 6d69 6e64 2f6d 6374  com/deepmind/mct
+00003810: 7829 3a20 4a41 582d 6e61 7469 7665 204d  x): JAX-native M
+00003820: 4354 5320 696d 706c 656d 656e 7461 7469  CTS implementati
+00003830: 6f6e 732c 2069 6e63 6c75 6469 6e67 2041  ons, including A
+00003840: 6c70 6861 5a65 726f 2061 6e64 204d 755a  lphaZero and MuZ
+00003850: 6572 6f0a 2d20 5b64 6565 706d 696e 642f  ero.- [deepmind/
+00003860: 726c 6178 5d28 6874 7470 733a 2f2f 6769  rlax](https://gi
+00003870: 7468 7562 2e63 6f6d 2f64 6565 706d 696e  thub.com/deepmin
+00003880: 642f 726c 6178 293a 204a 4158 2d6e 6174  d/rlax): JAX-nat
+00003890: 6976 6520 524c 2063 6f6d 706f 6e65 6e74  ive RL component
+000038a0: 730a 2d20 5b67 6f6f 676c 652f 6576 6f6a  s.- [google/evoj
+000038b0: 6178 5d28 6874 7470 733a 2f2f 6769 7468  ax](https://gith
+000038c0: 7562 2e63 6f6d 2f67 6f6f 676c 652f 6576  ub.com/google/ev
+000038d0: 6f6a 6178 293a 2048 6172 6477 6172 652d  ojax): Hardware-
+000038e0: 4163 6365 6c65 7261 7465 6420 6e65 7572  Accelerated neur
+000038f0: 6f65 766f 6c75 7469 6f6e 0a2d 205b 526f  oevolution.- [Ro
+00003900: 6265 7274 544c 616e 6765 2f65 766f 7361  bertTLange/evosa
+00003910: 785d 2868 7474 7073 3a2f 2f67 6974 6875  x](https://githu
+00003920: 622e 636f 6d2f 526f 6265 7274 544c 616e  b.com/RobertTLan
+00003930: 6765 2f65 766f 7361 7829 3a20 4a41 582d  ge/evosax): JAX-
+00003940: 6e61 7469 7665 2065 766f 6c75 7469 6f6e  native evolution
+00003950: 2073 7472 6174 6567 7920 2845 5329 2069   strategy (ES) i
+00003960: 6d70 6c65 6d65 6e74 6174 696f 6e73 0a2d  mplementations.-
+00003970: 205b 6164 6170 7469 7665 2d69 6e74 656c   [adaptive-intel
+00003980: 6c69 6765 6e74 2d72 6f62 6f74 6963 732f  ligent-robotics/
+00003990: 5144 6178 5d28 6874 7470 733a 2f2f 6769  QDax](https://gi
+000039a0: 7468 7562 2e63 6f6d 2f61 6461 7074 6976  thub.com/adaptiv
+000039b0: 652d 696e 7465 6c6c 6967 656e 742d 726f  e-intelligent-ro
+000039c0: 626f 7469 6373 2f51 4461 7829 3a20 4a41  botics/QDax): JA
+000039d0: 582d 6e61 7469 7665 2051 7561 6c69 7479  X-native Quality
+000039e0: 2d44 6976 6572 7369 7479 2028 5144 2920  -Diversity (QD) 
+000039f0: 616c 676f 7269 7468 6d73 0a2d 205b 6c75  algorithms.- [lu
+00003a00: 6368 7269 7334 3239 2f70 7572 656a 6178  chris429/purejax
+00003a10: 726c 5d28 6874 7470 733a 2f2f 6769 7468  rl](https://gith
+00003a20: 7562 2e63 6f6d 2f6c 7563 6872 6973 3432  ub.com/luchris42
+00003a30: 392f 7075 7265 6a61 7872 6c29 3a20 4a61  9/purejaxrl): Ja
+00003a40: 782d 6e61 7469 7665 2052 4c20 696d 706c  x-native RL impl
+00003a50: 656d 656e 7461 7469 6f6e 730a 0a23 2320  ementations..## 
+00003a60: 4369 7461 7469 6f6e 0a0a 4966 2079 6f75  Citation..If you
+00003a70: 2075 7365 2050 6778 2069 6e20 796f 7572   use Pgx in your
+00003a80: 2077 6f72 6b2c 2070 6c65 6173 6520 6369   work, please ci
+00003a90: 7465 2074 6865 2066 6f6c 6c6f 7769 6e67  te the following
+00003aa0: 2070 6170 6572 3a0a 0a60 6060 0a40 6172   paper:..```.@ar
+00003ab0: 7469 636c 657b 6b6f 7961 6d61 6461 3230  ticle{koyamada20
+00003ac0: 3233 7067 782c 0a20 2074 6974 6c65 3d7b  23pgx,.  title={
+00003ad0: 5067 783a 2048 6172 6477 6172 652d 6163  Pgx: Hardware-ac
+00003ae0: 6365 6c65 7261 7465 6420 5061 7261 6c6c  celerated Parall
+00003af0: 656c 2047 616d 6520 5369 6d75 6c61 746f  el Game Simulato
+00003b00: 7273 2066 6f72 2052 6569 6e66 6f72 6365  rs for Reinforce
+00003b10: 6d65 6e74 204c 6561 726e 696e 677d 2c0a  ment Learning},.
+00003b20: 2020 6175 7468 6f72 3d7b 4b6f 7961 6d61    author={Koyama
+00003b30: 6461 2c20 536f 7465 7473 7520 616e 6420  da, Sotetsu and 
+00003b40: 4f6b 616e 6f2c 2053 6869 6e72 6920 616e  Okano, Shinri an
+00003b50: 6420 4e69 7368 696d 6f72 692c 2053 6f69  d Nishimori, Soi
+00003b60: 6368 6972 6f20 616e 6420 4d75 7261 7461  chiro and Murata
+00003b70: 2c20 5975 2061 6e64 2048 6162 6172 612c  , Yu and Habara,
+00003b80: 204b 6569 676f 2061 6e64 204b 6974 612c   Keigo and Kita,
+00003b90: 2048 6172 756b 6120 616e 6420 4973 6869   Haruka and Ishi
+00003ba0: 692c 2053 6869 6e7d 2c0a 2020 6a6f 7572  i, Shin},.  jour
+00003bb0: 6e61 6c3d 7b61 7258 6976 2070 7265 7072  nal={arXiv prepr
+00003bc0: 696e 7420 6172 5869 763a 3233 3033 2e31  int arXiv:2303.1
+00003bd0: 3735 3033 7d2c 0a20 2079 6561 723d 7b32  7503},.  year={2
+00003be0: 3032 337d 0a7d 0a60 6060 0a0a 2323 204c  023}.}.```..## L
+00003bf0: 4943 454e 5345 0a0a 4170 6163 6865 2d32  ICENSE..Apache-2
+00003c00: 2e30 0a                                  .0.
```

### Comparing `pgx-1.0.0/pgx.egg-info/SOURCES.txt` & `pgx-1.1.0/pgx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 pgx.egg-info/dependency_links.txt
 pgx.egg-info/requires.txt
 pgx.egg-info/top_level.txt
 pgx/_mahjong/__init__.py
 pgx/_mahjong/_action.py
 pgx/_mahjong/_hand.py
 pgx/_mahjong/_mahjong.py
+pgx/_mahjong/_mahjong2.py
 pgx/_mahjong/_meld.py
 pgx/_mahjong/_shanten.py
 pgx/_mahjong/_yaku.py
 pgx/_mahjong/cache/__init__.py
 pgx/_src/__init__.py
 pgx/_src/api_test.py
 pgx/_src/baseline.py
@@ -50,14 +51,16 @@
 pgx/_src/dwg/chess.py
 pgx/_src/dwg/connect_four.py
 pgx/_src/dwg/gardner_chess.py
 pgx/_src/dwg/go.py
 pgx/_src/dwg/hex.py
 pgx/_src/dwg/kuhn_poker.py
 pgx/_src/dwg/leduc_holdem.py
+pgx/_src/dwg/mahjong.py
+pgx/_src/dwg/mahjong_tile.py
 pgx/_src/dwg/othello.py
 pgx/_src/dwg/play2048.py
 pgx/_src/dwg/shogi.py
 pgx/_src/dwg/sparrow_mahjong.py
 pgx/_src/dwg/tictactoe.py
 pgx/_src/dwg/images/__init__.py
 pgx/_src/dwg/images/chess/LICENSE
```

### Comparing `pgx-1.0.0/pyproject.toml` & `pgx-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/setup.py` & `pgx-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_animal_shogi.py` & `pgx-1.1.0/tests/test_animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_backgammon.py` & `pgx-1.1.0/tests/test_backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_baseline.py` & `pgx-1.1.0/tests/test_baseline.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_bridge_bidding.py` & `pgx-1.1.0/tests/test_bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_chess.py` & `pgx-1.1.0/tests/test_chess.py`

 * *Files 0% similar despite different names*

```diff
@@ -711,14 +711,24 @@
     # wrong en passant by pinned pawn
     state = State._from_fen("rn6/1b6/8/p1Br1k1p/PPp1pPpP/NRp3P1/2B4R/2K5 b - f3 0 54")
     print(state._en_passant)
     state.save_svg("tests/assets/chess/buggy_samples_011.svg")
     expected_legal_actions = [16, 17, 263, 652, 654, 656, 701, 714, 715, 1517, 1984, 1985, 1986, 1987, 1988, 1989, 1990, 2000, 2001, 3154, 3182, 3197, 3853]
     assert state.legal_action_mask.sum() == len(expected_legal_actions), f"\nactual:{jnp.nonzero(state.legal_action_mask)[0]}\nexpected\n{expected_legal_actions}"
 
+    # wrong rook position when castling
+    state = State._from_fen("r1b1k2r/2q2pp1/p1pbpn1p/2p5/2P2P2/1PNP4/P5PP/R1BQNR1K b kq - 0 15")
+    state.save_svg("tests/assets/chess/buggy_samples_012.svg")
+    state = step(state, jnp.int32(2367))
+    state.save_svg("tests/assets/chess/buggy_samples_013.svg")
+    state = step(state, jnp.int32(1796))
+    state.save_svg("tests/assets/chess/buggy_samples_014.svg")
+    expected_legal_actions = [16, 30, 162, 1212, 1225, 1269, 1270, 1271, 1272, 1284, 1297, 1298, 1299, 1942, 1943, 1956, 2498, 2948, 2949, 3131, 3132, 3133, 3134, 3135, 3136, 3138, 3534, 3548, 3593, 3594, 4250]
+    assert state.legal_action_mask.sum() == len(expected_legal_actions), f"\nactual:{jnp.nonzero(state.legal_action_mask)[0]}\nexpected\n{expected_legal_actions}"
+
 
 def test_observe():
     state = init(jax.random.PRNGKey(0))
     assert state.observation.shape == (8, 8, 119)
 
     # my pawn
     expected = jnp.float32(
```

### Comparing `pgx-1.0.0/tests/test_connect_four.py` & `pgx-1.1.0/tests/test_connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_gardner_chess.py` & `pgx-1.1.0/tests/test_gardner_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_go.py` & `pgx-1.1.0/tests/test_go.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_hex.py` & `pgx-1.1.0/tests/test_hex.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_kuhn_poker.py` & `pgx-1.1.0/tests/test_kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_leduc_holdem.py` & `pgx-1.1.0/tests/test_leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_othello.py` & `pgx-1.1.0/tests/test_othello.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_play2048.py` & `pgx-1.1.0/tests/test_play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_shogi.py` & `pgx-1.1.0/tests/test_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_sparrow_mahjong.py` & `pgx-1.1.0/tests/test_sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-1.0.0/tests/test_tic_tac_toe.py` & `pgx-1.1.0/tests/test_tic_tac_toe.py`

 * *Files identical despite different names*

