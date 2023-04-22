# Comparing `tmp/chessmaker-0.3.2.tar.gz` & `tmp/chessmaker-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chessmaker-0.3.2.tar", max compression
+gzip compressed data, was "chessmaker-0.4.0.tar", max compression
```

## Comparing `chessmaker-0.3.2.tar` & `chessmaker-0.4.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      159 2023-04-12 23:23:56.894161 chessmaker-0.3.2/chessmaker/__init__.py
--rw-r--r--   0        0        0      240 2023-04-13 13:53:22.478241 chessmaker-0.3.2/chessmaker/chess/__init__.py
--rw-r--r--   0        0        0      690 2023-04-15 21:57:06.856292 chessmaker-0.3.2/chessmaker/chess/base/__init__.py
--rw-r--r--   0        0        0     6771 2023-04-22 18:14:52.245949 chessmaker-0.3.2/chessmaker/chess/base/board.py
--rw-r--r--   0        0        0     1091 2023-04-16 20:29:32.083728 chessmaker-0.3.2/chessmaker/chess/base/game.py
--rw-r--r--   0        0        0      275 2023-04-13 19:53:48.822414 chessmaker-0.3.2/chessmaker/chess/base/move_option.py
--rw-r--r--   0        0        0     3553 2023-04-18 19:28:26.768718 chessmaker-0.3.2/chessmaker/chess/base/piece.py
--rw-r--r--   0        0        0      583 2023-04-12 22:32:25.286163 chessmaker-0.3.2/chessmaker/chess/base/player.py
--rw-r--r--   0        0        0      241 2023-04-12 22:32:25.006418 chessmaker-0.3.2/chessmaker/chess/base/position.py
--rw-r--r--   0        0        0      708 2023-04-12 22:57:13.193723 chessmaker-0.3.2/chessmaker/chess/base/rule.py
--rw-r--r--   0        0        0     2304 2023-04-16 20:16:29.441811 chessmaker-0.3.2/chessmaker/chess/base/square.py
--rw-r--r--   0        0        0     5299 2023-04-22 18:14:52.246936 chessmaker-0.3.2/chessmaker/chess/game_factory.py
--rw-r--r--   0        0        0     2460 2023-04-15 15:01:42.502293 chessmaker-0.3.2/chessmaker/chess/piece_utils.py
--rw-r--r--   0        0        0      319 2023-04-13 13:47:46.308045 chessmaker-0.3.2/chessmaker/chess/pieces/__init__.py
--rw-r--r--   0        0        0      652 2023-04-13 13:46:31.618457 chessmaker-0.3.2/chessmaker/chess/pieces/bishop.py
--rw-r--r--   0        0        0     6790 2023-04-16 20:01:11.181718 chessmaker-0.3.2/chessmaker/chess/pieces/king.py
--rw-r--r--   0        0        0      880 2023-04-13 13:46:31.589457 chessmaker-0.3.2/chessmaker/chess/pieces/knight.py
--rw-r--r--   0        0        0      191 2023-04-12 23:23:13.134441 chessmaker-0.3.2/chessmaker/chess/pieces/knook/__init__.py
--rw-r--r--   0        0        0      968 2023-04-15 14:44:35.264730 chessmaker-0.3.2/chessmaker/chess/pieces/knook/knook.py
--rw-r--r--   0        0        0       30 2023-04-15 15:13:15.595692 chessmaker-0.3.2/chessmaker/chess/pieces/knook/knookable.py
--rw-r--r--   0        0        0     1184 2023-04-16 21:13:06.169907 chessmaker-0.3.2/chessmaker/chess/pieces/knook/knookable_knight.py
--rw-r--r--   0        0        0     1216 2023-04-15 21:58:00.111375 chessmaker-0.3.2/chessmaker/chess/pieces/knook/knookable_rook.py
--rw-r--r--   0        0        0     1615 2023-04-15 21:58:00.012862 chessmaker-0.3.2/chessmaker/chess/pieces/knook/merge_to_knook.py
--rw-r--r--   0        0        0     5506 2023-04-16 20:01:11.191719 chessmaker-0.3.2/chessmaker/chess/pieces/pawn.py
--rw-r--r--   0        0        0      785 2023-04-13 13:46:31.572457 chessmaker-0.3.2/chessmaker/chess/pieces/queen.py
--rw-r--r--   0        0        0     1057 2023-04-16 21:13:16.019354 chessmaker-0.3.2/chessmaker/chess/pieces/rook.py
--rw-r--r--   0        0        0      332 2023-04-14 13:45:12.352119 chessmaker-0.3.2/chessmaker/chess/results/__init__.py
--rw-r--r--   0        0        0      478 2023-04-14 12:39:03.945677 chessmaker-0.3.2/chessmaker/chess/results/capture_all_pieces_to_win.py
--rw-r--r--   0        0        0      584 2023-04-14 12:32:41.047541 chessmaker-0.3.2/chessmaker/chess/results/checkmate.py
--rw-r--r--   0        0        0      801 2023-04-16 21:29:32.511999 chessmaker-0.3.2/chessmaker/chess/results/double_check_to_win.py
--rw-r--r--   0        0        0     1134 2023-04-15 02:00:39.838687 chessmaker-0.3.2/chessmaker/chess/results/no_captures_or_pawn_moves.py
--rw-r--r--   0        0        0      923 2023-04-14 11:49:56.085457 chessmaker-0.3.2/chessmaker/chess/results/repetition.py
--rw-r--r--   0        0        0      326 2023-04-14 11:49:56.091457 chessmaker-0.3.2/chessmaker/chess/results/stalemate.py
--rw-r--r--   0        0        0      510 2023-04-15 00:31:09.011728 chessmaker-0.3.2/chessmaker/chess/results/standard_result.py
--rw-r--r--   0        0        0      345 2023-04-14 13:02:43.693404 chessmaker-0.3.2/chessmaker/chess/rules/__init__.py
--rw-r--r--   0        0        0     3533 2023-04-13 13:46:31.611456 chessmaker-0.3.2/chessmaker/chess/rules/beta_decay.py
--rw-r--r--   0        0        0     1876 2023-04-18 21:33:20.550001 chessmaker-0.3.2/chessmaker/chess/rules/forced_en_passant.py
--rw-r--r--   0        0        0     3670 2023-04-15 12:04:05.521043 chessmaker-0.3.2/chessmaker/chess/rules/il_vaticano.py
--rw-r--r--   0        0        0      979 2023-04-14 12:49:09.088586 chessmaker-0.3.2/chessmaker/chess/rules/king_cant_move_to_c2.py
--rw-r--r--   0        0        0     2695 2023-04-12 22:57:13.120723 chessmaker-0.3.2/chessmaker/chess/rules/knight_boosting.py
--rw-r--r--   0        0        0     2461 2023-04-14 13:33:54.257799 chessmaker-0.3.2/chessmaker/chess/rules/la_bastarda.py
--rw-r--r--   0        0        0     1871 2023-04-15 12:04:05.540043 chessmaker-0.3.2/chessmaker/chess/rules/omnipotent_f6_pawn.py
--rw-r--r--   0        0        0     1982 2023-04-14 01:23:32.960857 chessmaker-0.3.2/chessmaker/chess/rules/siberian_swipe.py
--rw-r--r--   0        0        0       64 2023-04-14 17:14:53.444902 chessmaker-0.3.2/chessmaker/clients/__init__.py
--rw-r--r--   0        0        0    16135 2023-04-22 18:14:52.247944 chessmaker-0.3.2/chessmaker/clients/pywebio_ui.py
--rw-r--r--   0        0        0      278 2023-04-12 22:32:25.207165 chessmaker-0.3.2/chessmaker/cloneable.py
--rw-r--r--   0        0        0      149 2023-04-15 21:57:06.796292 chessmaker-0.3.2/chessmaker/events/__init__.py
--rw-r--r--   0        0        0      395 2023-04-13 19:53:48.832414 chessmaker-0.3.2/chessmaker/events/event.py
--rw-r--r--   0        0        0      146 2023-04-14 13:26:17.602659 chessmaker-0.3.2/chessmaker/events/event_priority.py
--rw-r--r--   0        0        0     3834 2023-04-18 18:39:24.165304 chessmaker-0.3.2/chessmaker/events/event_publisher.py
--rw-r--r--   0        0        0    35184 2023-04-05 10:50:17.213863 chessmaker-0.3.2/LICENSE
--rw-r--r--   0        0        0     1098 2023-04-22 18:14:52.258935 chessmaker-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1862 2023-04-14 14:15:04.351108 chessmaker-0.3.2/README.md
--rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 chessmaker-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      159 2023-04-12 23:23:56.894161 chessmaker-0.4.0/chessmaker/__init__.py
+-rw-r--r--   0        0        0      240 2023-04-13 13:53:22.478241 chessmaker-0.4.0/chessmaker/chess/__init__.py
+-rw-r--r--   0        0        0      690 2023-04-15 21:57:06.856292 chessmaker-0.4.0/chessmaker/chess/base/__init__.py
+-rw-r--r--   0        0        0     6811 2023-04-22 18:15:44.473745 chessmaker-0.4.0/chessmaker/chess/base/board.py
+-rw-r--r--   0        0        0     1091 2023-04-16 20:29:32.083728 chessmaker-0.4.0/chessmaker/chess/base/game.py
+-rw-r--r--   0        0        0      275 2023-04-13 19:53:48.822414 chessmaker-0.4.0/chessmaker/chess/base/move_option.py
+-rw-r--r--   0        0        0     3553 2023-04-18 19:28:26.768718 chessmaker-0.4.0/chessmaker/chess/base/piece.py
+-rw-r--r--   0        0        0      583 2023-04-12 22:32:25.286163 chessmaker-0.4.0/chessmaker/chess/base/player.py
+-rw-r--r--   0        0        0      241 2023-04-12 22:32:25.006418 chessmaker-0.4.0/chessmaker/chess/base/position.py
+-rw-r--r--   0        0        0      708 2023-04-12 22:57:13.193723 chessmaker-0.4.0/chessmaker/chess/base/rule.py
+-rw-r--r--   0        0        0     2304 2023-04-16 20:16:29.441811 chessmaker-0.4.0/chessmaker/chess/base/square.py
+-rw-r--r--   0        0        0     5151 2023-04-22 18:15:44.474745 chessmaker-0.4.0/chessmaker/chess/game_factory.py
+-rw-r--r--   0        0        0     2460 2023-04-15 15:01:42.502293 chessmaker-0.4.0/chessmaker/chess/piece_utils.py
+-rw-r--r--   0        0        0      319 2023-04-13 13:47:46.308045 chessmaker-0.4.0/chessmaker/chess/pieces/__init__.py
+-rw-r--r--   0        0        0      652 2023-04-13 13:46:31.618457 chessmaker-0.4.0/chessmaker/chess/pieces/bishop.py
+-rw-r--r--   0        0        0     6790 2023-04-16 20:01:11.181718 chessmaker-0.4.0/chessmaker/chess/pieces/king.py
+-rw-r--r--   0        0        0      880 2023-04-13 13:46:31.589457 chessmaker-0.4.0/chessmaker/chess/pieces/knight.py
+-rw-r--r--   0        0        0      191 2023-04-12 23:23:13.134441 chessmaker-0.4.0/chessmaker/chess/pieces/knook/__init__.py
+-rw-r--r--   0        0        0      968 2023-04-15 14:44:35.264730 chessmaker-0.4.0/chessmaker/chess/pieces/knook/knook.py
+-rw-r--r--   0        0        0       30 2023-04-15 15:13:15.595692 chessmaker-0.4.0/chessmaker/chess/pieces/knook/knookable.py
+-rw-r--r--   0        0        0     1184 2023-04-16 21:13:06.169907 chessmaker-0.4.0/chessmaker/chess/pieces/knook/knookable_knight.py
+-rw-r--r--   0        0        0     1216 2023-04-15 21:58:00.111375 chessmaker-0.4.0/chessmaker/chess/pieces/knook/knookable_rook.py
+-rw-r--r--   0        0        0     1615 2023-04-15 21:58:00.012862 chessmaker-0.4.0/chessmaker/chess/pieces/knook/merge_to_knook.py
+-rw-r--r--   0        0        0     5506 2023-04-16 20:01:11.191719 chessmaker-0.4.0/chessmaker/chess/pieces/pawn.py
+-rw-r--r--   0        0        0      785 2023-04-13 13:46:31.572457 chessmaker-0.4.0/chessmaker/chess/pieces/queen.py
+-rw-r--r--   0        0        0     1057 2023-04-16 21:13:16.019354 chessmaker-0.4.0/chessmaker/chess/pieces/rook.py
+-rw-r--r--   0        0        0      332 2023-04-14 13:45:12.352119 chessmaker-0.4.0/chessmaker/chess/results/__init__.py
+-rw-r--r--   0        0        0      478 2023-04-14 12:39:03.945677 chessmaker-0.4.0/chessmaker/chess/results/capture_all_pieces_to_win.py
+-rw-r--r--   0        0        0      584 2023-04-14 12:32:41.047541 chessmaker-0.4.0/chessmaker/chess/results/checkmate.py
+-rw-r--r--   0        0        0      801 2023-04-16 21:29:32.511999 chessmaker-0.4.0/chessmaker/chess/results/double_check_to_win.py
+-rw-r--r--   0        0        0     1134 2023-04-15 02:00:39.838687 chessmaker-0.4.0/chessmaker/chess/results/no_captures_or_pawn_moves.py
+-rw-r--r--   0        0        0      923 2023-04-14 11:49:56.085457 chessmaker-0.4.0/chessmaker/chess/results/repetition.py
+-rw-r--r--   0        0        0      326 2023-04-14 11:49:56.091457 chessmaker-0.4.0/chessmaker/chess/results/stalemate.py
+-rw-r--r--   0        0        0      510 2023-04-15 00:31:09.011728 chessmaker-0.4.0/chessmaker/chess/results/standard_result.py
+-rw-r--r--   0        0        0      345 2023-04-14 13:02:43.693404 chessmaker-0.4.0/chessmaker/chess/rules/__init__.py
+-rw-r--r--   0        0        0     3533 2023-04-13 13:46:31.611456 chessmaker-0.4.0/chessmaker/chess/rules/beta_decay.py
+-rw-r--r--   0        0        0     1876 2023-04-18 21:33:20.550001 chessmaker-0.4.0/chessmaker/chess/rules/forced_en_passant.py
+-rw-r--r--   0        0        0     3670 2023-04-15 12:04:05.521043 chessmaker-0.4.0/chessmaker/chess/rules/il_vaticano.py
+-rw-r--r--   0        0        0      979 2023-04-14 12:49:09.088586 chessmaker-0.4.0/chessmaker/chess/rules/king_cant_move_to_c2.py
+-rw-r--r--   0        0        0     2695 2023-04-12 22:57:13.120723 chessmaker-0.4.0/chessmaker/chess/rules/knight_boosting.py
+-rw-r--r--   0        0        0     2461 2023-04-14 13:33:54.257799 chessmaker-0.4.0/chessmaker/chess/rules/la_bastarda.py
+-rw-r--r--   0        0        0     1871 2023-04-15 12:04:05.540043 chessmaker-0.4.0/chessmaker/chess/rules/omnipotent_f6_pawn.py
+-rw-r--r--   0        0        0     1982 2023-04-14 01:23:32.960857 chessmaker-0.4.0/chessmaker/chess/rules/siberian_swipe.py
+-rw-r--r--   0        0        0       64 2023-04-14 17:14:53.444902 chessmaker-0.4.0/chessmaker/clients/__init__.py
+-rw-r--r--   0        0        0    17794 2023-04-22 18:15:44.475745 chessmaker-0.4.0/chessmaker/clients/pywebio_ui.py
+-rw-r--r--   0        0        0      278 2023-04-12 22:32:25.207165 chessmaker-0.4.0/chessmaker/cloneable.py
+-rw-r--r--   0        0        0      149 2023-04-15 21:57:06.796292 chessmaker-0.4.0/chessmaker/events/__init__.py
+-rw-r--r--   0        0        0      395 2023-04-13 19:53:48.832414 chessmaker-0.4.0/chessmaker/events/event.py
+-rw-r--r--   0        0        0      146 2023-04-14 13:26:17.602659 chessmaker-0.4.0/chessmaker/events/event_priority.py
+-rw-r--r--   0        0        0     3834 2023-04-18 18:39:24.165304 chessmaker-0.4.0/chessmaker/events/event_publisher.py
+-rw-r--r--   0        0        0    35184 2023-04-05 10:50:17.213863 chessmaker-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1098 2023-04-22 18:15:44.485745 chessmaker-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1862 2023-04-14 14:15:04.351108 chessmaker-0.4.0/README.md
+-rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 chessmaker-0.4.0/PKG-INFO
```

### Comparing `chessmaker-0.3.2/chessmaker/chess/base/__init__.py` & `chessmaker-0.4.0/chessmaker/chess/base/__init__.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/base/board.py` & `chessmaker-0.4.0/chessmaker/chess/base/board.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,10 +168,10 @@
 
     def clone(self):
         turn_iterators = itertools.tee(self.turn_iterator, 2)
         self.turn_iterator = turn_iterators[0]
         return Board(
             [[square.clone() if square is not None else None for square in row] for row in self._squares],
             self.players,
-            turn_iterators[1],
+            itertools.chain([self.current_player], turn_iterators[1]),
             [rule.clone() for rule in self.rules]
         )
```

### Comparing `chessmaker-0.3.2/chessmaker/chess/base/game.py` & `chessmaker-0.4.0/chessmaker/chess/base/game.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/base/piece.py` & `chessmaker-0.4.0/chessmaker/chess/base/piece.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/base/player.py` & `chessmaker-0.4.0/chessmaker/chess/base/player.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/base/rule.py` & `chessmaker-0.4.0/chessmaker/chess/base/rule.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/base/square.py` & `chessmaker-0.4.0/chessmaker/chess/base/square.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/game_factory.py` & `chessmaker-0.4.0/chessmaker/chess/game_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,28 +53,21 @@
     white = Player("white")
     black = Player("black")
     turn_iterator = cycle([white, black])
 
     def _empty_line(length: int) -> list[Square]:
         return [Square() for _ in range(length)]
 
-    def _up_pawn(player: Player):
-        return Pawn(player, Pawn.Direction.UP, promotions=[Bishop, _rook, Queen, _knight])
-
-    def _down_pawn(player: Player):
-        return Pawn(player, Pawn.Direction.DOWN, promotions=[Bishop, _rook, Queen, _knight])
-
     def _pawn(player: Player):
         if player == white:
-            return _up_pawn(player)
+            return Pawn(white, Pawn.Direction.UP, promotions=[Bishop, _rook, Queen, _knight])
         elif player == black:
-            return _down_pawn(player)
+            return Pawn(black, Pawn.Direction.DOWN, promotions=[Bishop, _rook, Queen, _knight])
 
     def _piece_row() -> list[Callable[[Player], Piece]]:
-
         pieces = [_rook, _knight, Bishop, Queen, _king, Bishop, _knight, _rook]
 
         if chess960:
             row = [None] * len(pieces)
             matched = False
             while not matched:
                 matched = True
```

### Comparing `chessmaker-0.3.2/chessmaker/chess/piece_utils.py` & `chessmaker-0.4.0/chessmaker/chess/piece_utils.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/pieces/bishop.py` & `chessmaker-0.4.0/chessmaker/chess/pieces/bishop.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/pieces/king.py` & `chessmaker-0.4.0/chessmaker/chess/pieces/king.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/pieces/knight.py` & `chessmaker-0.4.0/chessmaker/chess/pieces/knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/pieces/knook/knook.py` & `chessmaker-0.4.0/chessmaker/chess/pieces/knook/knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/pieces/knook/knookable_knight.py` & `chessmaker-0.4.0/chessmaker/chess/pieces/knook/knookable_knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/pieces/knook/knookable_rook.py` & `chessmaker-0.4.0/chessmaker/chess/pieces/knook/knookable_rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/pieces/knook/merge_to_knook.py` & `chessmaker-0.4.0/chessmaker/chess/pieces/knook/merge_to_knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/pieces/pawn.py` & `chessmaker-0.4.0/chessmaker/chess/pieces/pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/pieces/queen.py` & `chessmaker-0.4.0/chessmaker/chess/pieces/queen.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/pieces/rook.py` & `chessmaker-0.4.0/chessmaker/chess/pieces/rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/results/checkmate.py` & `chessmaker-0.4.0/chessmaker/chess/results/checkmate.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/results/double_check_to_win.py` & `chessmaker-0.4.0/chessmaker/chess/results/double_check_to_win.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/results/no_captures_or_pawn_moves.py` & `chessmaker-0.4.0/chessmaker/chess/results/no_captures_or_pawn_moves.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/results/repetition.py` & `chessmaker-0.4.0/chessmaker/chess/results/repetition.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/rules/beta_decay.py` & `chessmaker-0.4.0/chessmaker/chess/rules/beta_decay.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/rules/forced_en_passant.py` & `chessmaker-0.4.0/chessmaker/chess/rules/forced_en_passant.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/rules/il_vaticano.py` & `chessmaker-0.4.0/chessmaker/chess/rules/il_vaticano.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/rules/king_cant_move_to_c2.py` & `chessmaker-0.4.0/chessmaker/chess/rules/king_cant_move_to_c2.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/rules/knight_boosting.py` & `chessmaker-0.4.0/chessmaker/chess/rules/knight_boosting.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/rules/la_bastarda.py` & `chessmaker-0.4.0/chessmaker/chess/rules/la_bastarda.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/rules/omnipotent_f6_pawn.py` & `chessmaker-0.4.0/chessmaker/chess/rules/omnipotent_f6_pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/chess/rules/siberian_swipe.py` & `chessmaker-0.4.0/chessmaker/chess/rules/siberian_swipe.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/chessmaker/clients/pywebio_ui.py` & `chessmaker-0.4.0/chessmaker/clients/pywebio_ui.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from uuid import uuid4
 
 from pywebio import start_server, config
 from pywebio.input import input_group, actions, checkbox, radio
 from pywebio.io_ctrl import Output
 from pywebio.output import put_text, put_table, put_markdown, put_button, use_scope, clear, put_scope, popup, \
     close_popup, toast, put_error
-from pywebio.session import local as session_data, ThreadBasedSession, eval_js
+from pywebio.session import local as session_data, ThreadBasedSession, run_js
 from pywebio_battery import get_query
 
 from chessmaker.chess.base.board import Board
 from chessmaker.chess.base.game import Game, AfterTurnChangeEvent, AfterGameEndEvent
 from chessmaker.chess.base.move_option import MoveOption
 from chessmaker.chess.base.piece import Piece, AfterMoveEvent
 from chessmaker.chess.base.player import Player
@@ -47,34 +47,43 @@
     PIECE_URLS[piece] = (
         PIECE_URL_TEMPLATE.format(piece_color="w", piece_type=piece_type),
         PIECE_URL_TEMPLATE.format(piece_color="b", piece_type=piece_type),
     )
 
 
 @dataclass
-class MultiplayerGame:
+class ClientGame:
     game: Game
     options: list[str]
     sessions: List[ThreadBasedSession] = field(default_factory=list)
     colors: dict[str, str] = field(default_factory=dict)
     piece_urls: dict[str, tuple[str, ...]] = field(default_factory=lambda: PIECE_URLS)
 
 
-public_games: dict[str, tuple[float, MultiplayerGame]] = {}
-multiplayer_games: dict[str, MultiplayerGame] = {}
+@dataclass
+class SharedPosition:
+    board: Board
+    get_result: Callable[[Board], str | None]
+    options: list[str]
+    piece_urls: dict[str, tuple[str, ...]] = field(default_factory=lambda: PIECE_URLS)
+
+
+public_games: dict[str, tuple[float, ClientGame]] = {}
+client_games: dict[str, ClientGame] = {}
+shared_positions: dict[str, SharedPosition] = {}
 
 PS = ParamSpec("PS")
 RT = TypeVar("RT")
 
 
 def for_all_game_sessions(func: Callable[PS, RT]) -> Callable[PS, RT]:
     game_id = session_data.game_id
 
     def wrapper(*args, **kwargs):
-        game = multiplayer_games[game_id]
+        game = client_games[game_id]
         for session in game.sessions:
             func_id = str(uuid4())
 
             def inner(_):
                 func(*args, **kwargs)
 
             session.callbacks[func_id] = (inner, False)
@@ -92,17 +101,17 @@
             with use_scope(str(position), clear=True):
                 put_scope(str(uuid4()), square_content(board[position]))
         session_data.shown_move_options = None
         session_data.clicked_position = None
 
 
 def get_piece_url(piece: Piece):
-    multiplayer_game = multiplayer_games[session_data.game_id]
-    player_index = list(multiplayer_game.colors.keys()).index(piece.player.name)
-    return multiplayer_game.piece_urls[piece.name][player_index]
+    client_game = client_games[session_data.game_id]
+    player_index = list(client_game.colors.keys()).index(piece.player.name)
+    return client_game.piece_urls[piece.name][player_index]
 
 
 def move_piece(piece: Piece, move_option: MoveOption):
     if session_data.clicked_position is None:
         return
     session_data.clicked_position = None
     piece.move(move_option)
@@ -176,15 +185,15 @@
     current_player: Player = board.current_player
     if current_player != board[position].piece.player:
         return
 
     if session_data.player != "":
         if session_data.player != current_player:
             return
-        if len(multiplayer_games[session_data.game_id].sessions) < 2:
+        if len(client_games[session_data.game_id].sessions) < 2:
             toast("Waiting for another player to join...", position="top", duration=3)
             return
 
     show_move_options(position)
 
 
 @use_scope("board")
@@ -241,17 +250,37 @@
         session_data.player = event.player
 
 
 def on_game_end(event: AfterGameEndEvent):
     popup("Game Over", event.result)
 
 
+def share_position():
+    board = session_data.game.board.clone()
+    get_result = session_data.game._get_result
+    options = client_games[session_data.game_id].options
+    piece_urls = client_games[session_data.game_id].piece_urls
+
+    position_id = str(uuid4())
+    shared_positions[position_id] = SharedPosition(board, get_result, options, piece_urls)
+
+    run_js("navigator.clipboard.writeText(window.location.href.split('?')[0] + '?position_id=' + position_id);",
+           position_id=position_id)
+    toast("Position URL copied to clipboard")
+
+
+def invite():
+    game_id = session_data.game_id
+    run_js("navigator.clipboard.writeText(window.location.href.split('?')[0] + '?game_id=' + game_id);", game_id=game_id)
+    toast("Invite URL copied to clipboard")
+
+
 def initialize_board():
     board: Board = session_data.game.board
-    options = multiplayer_games[session_data.game_id].options
+    options = client_games[session_data.game_id].options
     if options:
         put_text(f"Options: {', '.join(options)}")
 
     with use_scope("board"):
         grid: list[list[Output | None]] = [[None for _ in range(board.size[0])] for _ in range(board.size[1])]
 
         for y in range(board.size[1]):
@@ -279,61 +308,68 @@
 
         put_table(grid).style("text-align: center")
 
     session_data.last_board_pieces = get_board_strings(board)
 
 
 def join_game(game_id: str):
-    multiplayer_games[game_id].sessions.append(ThreadBasedSession.get_current_session())
-    game = multiplayer_games[game_id].game
+    client_games[game_id].sessions.append(ThreadBasedSession.get_current_session())
+    game = client_games[game_id].game
 
     session_data.game = game
     session_data.game_id = game_id
     session_data.own_game = False
 
     put_markdown("""# ChessMaker \n """).style("text-align:center")
+    put_button("Share Position", onclick=share_position)
     initialize_board()
     put_markdown(
         "[Docs](https://wolfdwyc.github.io/ChessMaker) - [Source](https://github.com/WolfDWyc/ChessMaker)\nMade by WolfDWyc").style(
         "text-align:center")
 
 
 def new_game(game_factory: Callable[..., Game], options: list[str], mode: str, piece_urls: dict[str, tuple[str, ...]]):
     game: Game = game_factory(**{option: True for option in options})
     game_id = str(uuid4())
 
     session_data.game = game
     session_data.game_id = game_id
 
-    multiplayer_game = MultiplayerGame(game, options, [ThreadBasedSession.get_current_session()], {}, piece_urls)
+    client_game = ClientGame(game, options, [ThreadBasedSession.get_current_session()], {}, piece_urls)
     colors = ['w', 'b']
     for player in game.board.players:
-        multiplayer_game.colors[player.name] = colors.pop(0)
+        client_game.colors[player.name] = colors.pop(0)
 
-    multiplayer_games[game_id] = multiplayer_game
+    client_games[game_id] = client_game
     if mode == 'Multiplayer (Public)':
-        public_games[game_id] = (time.time(), multiplayer_game)
+        public_games[game_id] = (time.time(), client_game)
 
     session_data.own_game = True
     if mode != 'Singleplayer':
         session_data.player = game.board.current_player
     else:
         session_data.player = ""
 
     game.board.subscribe(AfterMoveEvent, for_all_game_sessions(on_after_move), EventPriority.VERY_LOW + 1)
     game.board.subscribe(AfterTurnChangeEvent, for_all_game_sessions(on_after_turn_change))
     game.subscribe(AfterGameEndEvent, for_all_game_sessions(on_game_end))
 
     put_markdown("""# ChessMaker \n """).style("text-align:center")
+    buttons = [put_button("Share Position", onclick=share_position)]
     if mode == 'Multiplayer (Private)':
-        put_text("Invite URL: " + eval_js("window.location.href.split('?')[0]") + "?game_id=" + session_data.game_id)
+        buttons.append(put_button("Copy invite URL", onclick=invite))
+    # Put buttons on the same line
+    put_scope("buttons", content=buttons).style("display: flex; justify-content: start; gap: 5px")
+
     initialize_board()
     put_markdown(
-        "[Docs](https://wolfdwyc.github.io/ChessMaker) - [Source](https://github.com/WolfDWyc/ChessMaker)\nMade by WolfDWyc").style(
-        "text-align:center")
+        "[Docs](https://wolfdwyc.github.io/ChessMaker)"
+        " - [Source](https://github.com/WolfDWyc/ChessMaker)\nMade by WolfDWyc").style(
+        "text-align:center"
+    )
 
 
 def start_pywebio_chess_server(
         game_factory: Callable[..., Game],
         supported_options: List[str] = None,
         piece_urls: dict[str, tuple[str, ...]] = PIECE_URLS,
         remote_access: bool = False,
@@ -353,20 +389,30 @@
         for game_id, (time_created, game) in public_games.items():
             if time.time() - time_created > 5 * 60:
                 games_to_remove.append(game_id)
         for game_id in games_to_remove:
             public_games.pop(game_id)
 
         if get_query("game_id"):
-            if get_query("game_id") not in multiplayer_games:
+            if get_query("game_id") not in client_games:
                 popup("Error", put_error("Game not found"))
             else:
                 join_game(get_query("game_id"))
             return
 
+        if get_query("position_id"):
+            if get_query("position_id") not in shared_positions:
+                popup("Error", put_error("Position not found"))
+            else:
+                shared_position = shared_positions[get_query("position_id")]
+                new_game(lambda **_: Game(shared_position.board, shared_position.get_result),
+                            shared_position.options, 'Singleplayer', piece_urls)
+            return
+
+
         form_result = input_group('New Game', [
             radio('Mode', ['Singleplayer', 'Multiplayer (Private)', 'Multiplayer (Public)'], name='mode',
                   value='Singleplayer'),
             checkbox(
                 'Options',
                 options=supported_options,
                 name='options',
```

### Comparing `chessmaker-0.3.2/chessmaker/events/event_publisher.py` & `chessmaker-0.4.0/chessmaker/events/event_publisher.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/LICENSE` & `chessmaker-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/pyproject.toml` & `chessmaker-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chessmaker"
-version = "0.3.2"
+version = "0.4.0"
 description = "An easily extendible chess implementation designed to support any custom rule or feature"
 readme = "README.md"
 authors = ["WolfDWyc <yoavwolfdw@gmail.com>",]
 license = "AGPL-3.0-or-later"
 classifiers = [
 "License :: OSI Approved :: GNU Affero General Public License v3",
 "Programming Language :: Python",
```

### Comparing `chessmaker-0.3.2/README.md` & `chessmaker-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `chessmaker-0.3.2/PKG-INFO` & `chessmaker-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chessmaker
-Version: 0.3.2
+Version: 0.4.0
 Summary: An easily extendible chess implementation designed to support any custom rule or feature
 License: AGPL-3.0-or-later
 Keywords: chess
 Author: WolfDWyc
 Author-email: yoavwolfdw@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

