# Comparing `tmp/chessmaker-0.4.0.tar.gz` & `tmp/chessmaker-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chessmaker-0.4.0.tar", max compression
+gzip compressed data, was "chessmaker-0.4.1.tar", max compression
```

## Comparing `chessmaker-0.4.0.tar` & `chessmaker-0.4.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      159 2023-04-12 23:23:56.894161 chessmaker-0.4.0/chessmaker/__init__.py
--rw-r--r--   0        0        0      240 2023-04-13 13:53:22.478241 chessmaker-0.4.0/chessmaker/chess/__init__.py
--rw-r--r--   0        0        0      690 2023-04-15 21:57:06.856292 chessmaker-0.4.0/chessmaker/chess/base/__init__.py
--rw-r--r--   0        0        0     6811 2023-04-22 18:15:44.473745 chessmaker-0.4.0/chessmaker/chess/base/board.py
--rw-r--r--   0        0        0     1091 2023-04-16 20:29:32.083728 chessmaker-0.4.0/chessmaker/chess/base/game.py
--rw-r--r--   0        0        0      275 2023-04-13 19:53:48.822414 chessmaker-0.4.0/chessmaker/chess/base/move_option.py
--rw-r--r--   0        0        0     3553 2023-04-18 19:28:26.768718 chessmaker-0.4.0/chessmaker/chess/base/piece.py
--rw-r--r--   0        0        0      583 2023-04-12 22:32:25.286163 chessmaker-0.4.0/chessmaker/chess/base/player.py
--rw-r--r--   0        0        0      241 2023-04-12 22:32:25.006418 chessmaker-0.4.0/chessmaker/chess/base/position.py
--rw-r--r--   0        0        0      708 2023-04-12 22:57:13.193723 chessmaker-0.4.0/chessmaker/chess/base/rule.py
--rw-r--r--   0        0        0     2304 2023-04-16 20:16:29.441811 chessmaker-0.4.0/chessmaker/chess/base/square.py
--rw-r--r--   0        0        0     5151 2023-04-22 18:15:44.474745 chessmaker-0.4.0/chessmaker/chess/game_factory.py
--rw-r--r--   0        0        0     2460 2023-04-15 15:01:42.502293 chessmaker-0.4.0/chessmaker/chess/piece_utils.py
--rw-r--r--   0        0        0      319 2023-04-13 13:47:46.308045 chessmaker-0.4.0/chessmaker/chess/pieces/__init__.py
--rw-r--r--   0        0        0      652 2023-04-13 13:46:31.618457 chessmaker-0.4.0/chessmaker/chess/pieces/bishop.py
--rw-r--r--   0        0        0     6790 2023-04-16 20:01:11.181718 chessmaker-0.4.0/chessmaker/chess/pieces/king.py
--rw-r--r--   0        0        0      880 2023-04-13 13:46:31.589457 chessmaker-0.4.0/chessmaker/chess/pieces/knight.py
--rw-r--r--   0        0        0      191 2023-04-12 23:23:13.134441 chessmaker-0.4.0/chessmaker/chess/pieces/knook/__init__.py
--rw-r--r--   0        0        0      968 2023-04-15 14:44:35.264730 chessmaker-0.4.0/chessmaker/chess/pieces/knook/knook.py
--rw-r--r--   0        0        0       30 2023-04-15 15:13:15.595692 chessmaker-0.4.0/chessmaker/chess/pieces/knook/knookable.py
--rw-r--r--   0        0        0     1184 2023-04-16 21:13:06.169907 chessmaker-0.4.0/chessmaker/chess/pieces/knook/knookable_knight.py
--rw-r--r--   0        0        0     1216 2023-04-15 21:58:00.111375 chessmaker-0.4.0/chessmaker/chess/pieces/knook/knookable_rook.py
--rw-r--r--   0        0        0     1615 2023-04-15 21:58:00.012862 chessmaker-0.4.0/chessmaker/chess/pieces/knook/merge_to_knook.py
--rw-r--r--   0        0        0     5506 2023-04-16 20:01:11.191719 chessmaker-0.4.0/chessmaker/chess/pieces/pawn.py
--rw-r--r--   0        0        0      785 2023-04-13 13:46:31.572457 chessmaker-0.4.0/chessmaker/chess/pieces/queen.py
--rw-r--r--   0        0        0     1057 2023-04-16 21:13:16.019354 chessmaker-0.4.0/chessmaker/chess/pieces/rook.py
--rw-r--r--   0        0        0      332 2023-04-14 13:45:12.352119 chessmaker-0.4.0/chessmaker/chess/results/__init__.py
--rw-r--r--   0        0        0      478 2023-04-14 12:39:03.945677 chessmaker-0.4.0/chessmaker/chess/results/capture_all_pieces_to_win.py
--rw-r--r--   0        0        0      584 2023-04-14 12:32:41.047541 chessmaker-0.4.0/chessmaker/chess/results/checkmate.py
--rw-r--r--   0        0        0      801 2023-04-16 21:29:32.511999 chessmaker-0.4.0/chessmaker/chess/results/double_check_to_win.py
--rw-r--r--   0        0        0     1134 2023-04-15 02:00:39.838687 chessmaker-0.4.0/chessmaker/chess/results/no_captures_or_pawn_moves.py
--rw-r--r--   0        0        0      923 2023-04-14 11:49:56.085457 chessmaker-0.4.0/chessmaker/chess/results/repetition.py
--rw-r--r--   0        0        0      326 2023-04-14 11:49:56.091457 chessmaker-0.4.0/chessmaker/chess/results/stalemate.py
--rw-r--r--   0        0        0      510 2023-04-15 00:31:09.011728 chessmaker-0.4.0/chessmaker/chess/results/standard_result.py
--rw-r--r--   0        0        0      345 2023-04-14 13:02:43.693404 chessmaker-0.4.0/chessmaker/chess/rules/__init__.py
--rw-r--r--   0        0        0     3533 2023-04-13 13:46:31.611456 chessmaker-0.4.0/chessmaker/chess/rules/beta_decay.py
--rw-r--r--   0        0        0     1876 2023-04-18 21:33:20.550001 chessmaker-0.4.0/chessmaker/chess/rules/forced_en_passant.py
--rw-r--r--   0        0        0     3670 2023-04-15 12:04:05.521043 chessmaker-0.4.0/chessmaker/chess/rules/il_vaticano.py
--rw-r--r--   0        0        0      979 2023-04-14 12:49:09.088586 chessmaker-0.4.0/chessmaker/chess/rules/king_cant_move_to_c2.py
--rw-r--r--   0        0        0     2695 2023-04-12 22:57:13.120723 chessmaker-0.4.0/chessmaker/chess/rules/knight_boosting.py
--rw-r--r--   0        0        0     2461 2023-04-14 13:33:54.257799 chessmaker-0.4.0/chessmaker/chess/rules/la_bastarda.py
--rw-r--r--   0        0        0     1871 2023-04-15 12:04:05.540043 chessmaker-0.4.0/chessmaker/chess/rules/omnipotent_f6_pawn.py
--rw-r--r--   0        0        0     1982 2023-04-14 01:23:32.960857 chessmaker-0.4.0/chessmaker/chess/rules/siberian_swipe.py
--rw-r--r--   0        0        0       64 2023-04-14 17:14:53.444902 chessmaker-0.4.0/chessmaker/clients/__init__.py
--rw-r--r--   0        0        0    17794 2023-04-22 18:15:44.475745 chessmaker-0.4.0/chessmaker/clients/pywebio_ui.py
--rw-r--r--   0        0        0      278 2023-04-12 22:32:25.207165 chessmaker-0.4.0/chessmaker/cloneable.py
--rw-r--r--   0        0        0      149 2023-04-15 21:57:06.796292 chessmaker-0.4.0/chessmaker/events/__init__.py
--rw-r--r--   0        0        0      395 2023-04-13 19:53:48.832414 chessmaker-0.4.0/chessmaker/events/event.py
--rw-r--r--   0        0        0      146 2023-04-14 13:26:17.602659 chessmaker-0.4.0/chessmaker/events/event_priority.py
--rw-r--r--   0        0        0     3834 2023-04-18 18:39:24.165304 chessmaker-0.4.0/chessmaker/events/event_publisher.py
--rw-r--r--   0        0        0    35184 2023-04-05 10:50:17.213863 chessmaker-0.4.0/LICENSE
--rw-r--r--   0        0        0     1098 2023-04-22 18:15:44.485745 chessmaker-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1862 2023-04-14 14:15:04.351108 chessmaker-0.4.0/README.md
--rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 chessmaker-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      159 2023-04-12 23:23:56.894161 chessmaker-0.4.1/chessmaker/__init__.py
+-rw-r--r--   0        0        0      240 2023-04-13 13:53:22.478241 chessmaker-0.4.1/chessmaker/chess/__init__.py
+-rw-r--r--   0        0        0      690 2023-04-15 21:57:06.856292 chessmaker-0.4.1/chessmaker/chess/base/__init__.py
+-rw-r--r--   0        0        0     6811 2023-04-22 18:15:44.473745 chessmaker-0.4.1/chessmaker/chess/base/board.py
+-rw-r--r--   0        0        0     1091 2023-04-16 20:29:32.083728 chessmaker-0.4.1/chessmaker/chess/base/game.py
+-rw-r--r--   0        0        0      275 2023-04-13 19:53:48.822414 chessmaker-0.4.1/chessmaker/chess/base/move_option.py
+-rw-r--r--   0        0        0     3553 2023-04-18 19:28:26.768718 chessmaker-0.4.1/chessmaker/chess/base/piece.py
+-rw-r--r--   0        0        0      583 2023-04-12 22:32:25.286163 chessmaker-0.4.1/chessmaker/chess/base/player.py
+-rw-r--r--   0        0        0      241 2023-04-12 22:32:25.006418 chessmaker-0.4.1/chessmaker/chess/base/position.py
+-rw-r--r--   0        0        0      708 2023-04-12 22:57:13.193723 chessmaker-0.4.1/chessmaker/chess/base/rule.py
+-rw-r--r--   0        0        0     2304 2023-04-16 20:16:29.441811 chessmaker-0.4.1/chessmaker/chess/base/square.py
+-rw-r--r--   0        0        0     5151 2023-04-22 18:15:44.474745 chessmaker-0.4.1/chessmaker/chess/game_factory.py
+-rw-r--r--   0        0        0     2460 2023-04-15 15:01:42.502293 chessmaker-0.4.1/chessmaker/chess/piece_utils.py
+-rw-r--r--   0        0        0      319 2023-04-13 13:47:46.308045 chessmaker-0.4.1/chessmaker/chess/pieces/__init__.py
+-rw-r--r--   0        0        0      652 2023-04-13 13:46:31.618457 chessmaker-0.4.1/chessmaker/chess/pieces/bishop.py
+-rw-r--r--   0        0        0     6790 2023-04-16 20:01:11.181718 chessmaker-0.4.1/chessmaker/chess/pieces/king.py
+-rw-r--r--   0        0        0      880 2023-04-13 13:46:31.589457 chessmaker-0.4.1/chessmaker/chess/pieces/knight.py
+-rw-r--r--   0        0        0      191 2023-04-12 23:23:13.134441 chessmaker-0.4.1/chessmaker/chess/pieces/knook/__init__.py
+-rw-r--r--   0        0        0      968 2023-04-15 14:44:35.264730 chessmaker-0.4.1/chessmaker/chess/pieces/knook/knook.py
+-rw-r--r--   0        0        0       30 2023-04-15 15:13:15.595692 chessmaker-0.4.1/chessmaker/chess/pieces/knook/knookable.py
+-rw-r--r--   0        0        0     1184 2023-04-16 21:13:06.169907 chessmaker-0.4.1/chessmaker/chess/pieces/knook/knookable_knight.py
+-rw-r--r--   0        0        0     1216 2023-04-15 21:58:00.111375 chessmaker-0.4.1/chessmaker/chess/pieces/knook/knookable_rook.py
+-rw-r--r--   0        0        0     1615 2023-04-15 21:58:00.012862 chessmaker-0.4.1/chessmaker/chess/pieces/knook/merge_to_knook.py
+-rw-r--r--   0        0        0     5506 2023-04-16 20:01:11.191719 chessmaker-0.4.1/chessmaker/chess/pieces/pawn.py
+-rw-r--r--   0        0        0      785 2023-04-13 13:46:31.572457 chessmaker-0.4.1/chessmaker/chess/pieces/queen.py
+-rw-r--r--   0        0        0     1057 2023-04-16 21:13:16.019354 chessmaker-0.4.1/chessmaker/chess/pieces/rook.py
+-rw-r--r--   0        0        0      332 2023-04-14 13:45:12.352119 chessmaker-0.4.1/chessmaker/chess/results/__init__.py
+-rw-r--r--   0        0        0      478 2023-04-14 12:39:03.945677 chessmaker-0.4.1/chessmaker/chess/results/capture_all_pieces_to_win.py
+-rw-r--r--   0        0        0      584 2023-04-14 12:32:41.047541 chessmaker-0.4.1/chessmaker/chess/results/checkmate.py
+-rw-r--r--   0        0        0      801 2023-04-16 21:29:32.511999 chessmaker-0.4.1/chessmaker/chess/results/double_check_to_win.py
+-rw-r--r--   0        0        0     1134 2023-04-15 02:00:39.838687 chessmaker-0.4.1/chessmaker/chess/results/no_captures_or_pawn_moves.py
+-rw-r--r--   0        0        0      923 2023-04-14 11:49:56.085457 chessmaker-0.4.1/chessmaker/chess/results/repetition.py
+-rw-r--r--   0        0        0      326 2023-04-14 11:49:56.091457 chessmaker-0.4.1/chessmaker/chess/results/stalemate.py
+-rw-r--r--   0        0        0      510 2023-04-15 00:31:09.011728 chessmaker-0.4.1/chessmaker/chess/results/standard_result.py
+-rw-r--r--   0        0        0      345 2023-04-14 13:02:43.693404 chessmaker-0.4.1/chessmaker/chess/rules/__init__.py
+-rw-r--r--   0        0        0     3533 2023-04-13 13:46:31.611456 chessmaker-0.4.1/chessmaker/chess/rules/beta_decay.py
+-rw-r--r--   0        0        0     1876 2023-04-18 21:33:20.550001 chessmaker-0.4.1/chessmaker/chess/rules/forced_en_passant.py
+-rw-r--r--   0        0        0     3670 2023-04-15 12:04:05.521043 chessmaker-0.4.1/chessmaker/chess/rules/il_vaticano.py
+-rw-r--r--   0        0        0      979 2023-04-14 12:49:09.088586 chessmaker-0.4.1/chessmaker/chess/rules/king_cant_move_to_c2.py
+-rw-r--r--   0        0        0     2695 2023-04-12 22:57:13.120723 chessmaker-0.4.1/chessmaker/chess/rules/knight_boosting.py
+-rw-r--r--   0        0        0     2461 2023-04-14 13:33:54.257799 chessmaker-0.4.1/chessmaker/chess/rules/la_bastarda.py
+-rw-r--r--   0        0        0     1871 2023-04-15 12:04:05.540043 chessmaker-0.4.1/chessmaker/chess/rules/omnipotent_f6_pawn.py
+-rw-r--r--   0        0        0     1982 2023-04-14 01:23:32.960857 chessmaker-0.4.1/chessmaker/chess/rules/siberian_swipe.py
+-rw-r--r--   0        0        0       64 2023-04-14 17:14:53.444902 chessmaker-0.4.1/chessmaker/clients/__init__.py
+-rw-r--r--   0        0        0    18171 2023-04-22 18:29:36.629482 chessmaker-0.4.1/chessmaker/clients/pywebio_ui.py
+-rw-r--r--   0        0        0      278 2023-04-12 22:32:25.207165 chessmaker-0.4.1/chessmaker/cloneable.py
+-rw-r--r--   0        0        0      149 2023-04-15 21:57:06.796292 chessmaker-0.4.1/chessmaker/events/__init__.py
+-rw-r--r--   0        0        0      395 2023-04-13 19:53:48.832414 chessmaker-0.4.1/chessmaker/events/event.py
+-rw-r--r--   0        0        0      146 2023-04-14 13:26:17.602659 chessmaker-0.4.1/chessmaker/events/event_priority.py
+-rw-r--r--   0        0        0     3834 2023-04-18 18:39:24.165304 chessmaker-0.4.1/chessmaker/events/event_publisher.py
+-rw-r--r--   0        0        0    35184 2023-04-05 10:50:17.213863 chessmaker-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1098 2023-04-22 18:29:36.624482 chessmaker-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1862 2023-04-14 14:15:04.351108 chessmaker-0.4.1/README.md
+-rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 chessmaker-0.4.1/PKG-INFO
```

### Comparing `chessmaker-0.4.0/chessmaker/chess/base/__init__.py` & `chessmaker-0.4.1/chessmaker/chess/base/__init__.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/base/board.py` & `chessmaker-0.4.1/chessmaker/chess/base/board.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/base/game.py` & `chessmaker-0.4.1/chessmaker/chess/base/game.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/base/piece.py` & `chessmaker-0.4.1/chessmaker/chess/base/piece.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/base/player.py` & `chessmaker-0.4.1/chessmaker/chess/base/player.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/base/rule.py` & `chessmaker-0.4.1/chessmaker/chess/base/rule.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/base/square.py` & `chessmaker-0.4.1/chessmaker/chess/base/square.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/game_factory.py` & `chessmaker-0.4.1/chessmaker/chess/game_factory.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/piece_utils.py` & `chessmaker-0.4.1/chessmaker/chess/piece_utils.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/pieces/bishop.py` & `chessmaker-0.4.1/chessmaker/chess/pieces/bishop.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/pieces/king.py` & `chessmaker-0.4.1/chessmaker/chess/pieces/king.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/pieces/knight.py` & `chessmaker-0.4.1/chessmaker/chess/pieces/knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/pieces/knook/knook.py` & `chessmaker-0.4.1/chessmaker/chess/pieces/knook/knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/pieces/knook/knookable_knight.py` & `chessmaker-0.4.1/chessmaker/chess/pieces/knook/knookable_knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/pieces/knook/knookable_rook.py` & `chessmaker-0.4.1/chessmaker/chess/pieces/knook/knookable_rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/pieces/knook/merge_to_knook.py` & `chessmaker-0.4.1/chessmaker/chess/pieces/knook/merge_to_knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/pieces/pawn.py` & `chessmaker-0.4.1/chessmaker/chess/pieces/pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/pieces/queen.py` & `chessmaker-0.4.1/chessmaker/chess/pieces/queen.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/pieces/rook.py` & `chessmaker-0.4.1/chessmaker/chess/pieces/rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/results/checkmate.py` & `chessmaker-0.4.1/chessmaker/chess/results/checkmate.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/results/double_check_to_win.py` & `chessmaker-0.4.1/chessmaker/chess/results/double_check_to_win.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/results/no_captures_or_pawn_moves.py` & `chessmaker-0.4.1/chessmaker/chess/results/no_captures_or_pawn_moves.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/results/repetition.py` & `chessmaker-0.4.1/chessmaker/chess/results/repetition.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/rules/beta_decay.py` & `chessmaker-0.4.1/chessmaker/chess/rules/beta_decay.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/rules/forced_en_passant.py` & `chessmaker-0.4.1/chessmaker/chess/rules/forced_en_passant.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/rules/il_vaticano.py` & `chessmaker-0.4.1/chessmaker/chess/rules/il_vaticano.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/rules/king_cant_move_to_c2.py` & `chessmaker-0.4.1/chessmaker/chess/rules/king_cant_move_to_c2.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/rules/knight_boosting.py` & `chessmaker-0.4.1/chessmaker/chess/rules/knight_boosting.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/rules/la_bastarda.py` & `chessmaker-0.4.1/chessmaker/chess/rules/la_bastarda.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/rules/omnipotent_f6_pawn.py` & `chessmaker-0.4.1/chessmaker/chess/rules/omnipotent_f6_pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/chess/rules/siberian_swipe.py` & `chessmaker-0.4.1/chessmaker/chess/rules/siberian_swipe.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/chessmaker/clients/pywebio_ui.py` & `chessmaker-0.4.1/chessmaker/clients/pywebio_ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 .markdown-body table th {padding:0;}
 .markdown-body p {margin:0;}
 .markdown-body table td {font-weight:bold; padding:0; line-height:80px; border: 0}
 .markdown-body table tr {border: 0}
 td>div {width:80px; height:80px}.btn-light {background-color:#d3d6da;}
 @media (max-width: 435px) {.btn{padding:0.375rem 0.5rem;}}
 @media (max-width: 355px) {.btn{padding:0.375rem 0.4rem;}}
-div[id='pywebio-scope-board'] .btn {width: 80px; height: 80px;}
+div[id="pywebio-scope-board"] .btn {width: 80px; height: 80px;}
 .pywebio {min-height:calc(100vh - 50px);}
 div[id$="-move-option"] button {color: #bdc6c8; display: inline-flex; align-item: flex-start;
  vertical-align: top; padding: 0px; line-height: 0.75; font-style: italic; font-size: 11px;
  white-space: nowrap;}
 """
 
 PIECE_URL_TEMPLATE = "https://www.chess.com/chess-themes/pieces/neo/150/{piece_color}{piece_type}.png"
@@ -316,52 +316,51 @@
     game = client_games[game_id].game
 
     session_data.game = game
     session_data.game_id = game_id
     session_data.own_game = False
 
     put_markdown("""# ChessMaker \n """).style("text-align:center")
-    put_button("Share Position", onclick=share_position)
+    put_button("Copy position URL", onclick=share_position)
     initialize_board()
     put_markdown(
         "[Docs](https://wolfdwyc.github.io/ChessMaker) - [Source](https://github.com/WolfDWyc/ChessMaker)\nMade by WolfDWyc").style(
         "text-align:center")
 
 
 def new_game(game_factory: Callable[..., Game], options: list[str], mode: str, piece_urls: dict[str, tuple[str, ...]]):
     game: Game = game_factory(**{option: True for option in options})
     game_id = str(uuid4())
 
     session_data.game = game
     session_data.game_id = game_id
 
     client_game = ClientGame(game, options, [ThreadBasedSession.get_current_session()], {}, piece_urls)
-    colors = ['w', 'b']
+    colors = ["w", "b"]
     for player in game.board.players:
         client_game.colors[player.name] = colors.pop(0)
 
     client_games[game_id] = client_game
-    if mode == 'Multiplayer (Public)':
+    if mode == "Multiplayer (Public)":
         public_games[game_id] = (time.time(), client_game)
 
     session_data.own_game = True
-    if mode != 'Singleplayer':
+    if mode != "Singleplayer":
         session_data.player = game.board.current_player
     else:
         session_data.player = ""
 
     game.board.subscribe(AfterMoveEvent, for_all_game_sessions(on_after_move), EventPriority.VERY_LOW + 1)
     game.board.subscribe(AfterTurnChangeEvent, for_all_game_sessions(on_after_turn_change))
     game.subscribe(AfterGameEndEvent, for_all_game_sessions(on_game_end))
 
     put_markdown("""# ChessMaker \n """).style("text-align:center")
-    buttons = [put_button("Share Position", onclick=share_position)]
-    if mode == 'Multiplayer (Private)':
+    buttons = [put_button("Copy position URL", onclick=share_position)]
+    if mode == "Multiplayer (Private)":
         buttons.append(put_button("Copy invite URL", onclick=invite))
-    # Put buttons on the same line
     put_scope("buttons", content=buttons).style("display: flex; justify-content: start; gap: 5px")
 
     initialize_board()
     put_markdown(
         "[Docs](https://wolfdwyc.github.io/ChessMaker)"
         " - [Source](https://github.com/WolfDWyc/ChessMaker)\nMade by WolfDWyc").style(
         "text-align:center"
@@ -399,49 +398,56 @@
                 join_game(get_query("game_id"))
             return
 
         if get_query("position_id"):
             if get_query("position_id") not in shared_positions:
                 popup("Error", put_error("Position not found"))
             else:
+                form_result = input_group("New Game", [
+                    radio("Mode", ["Singleplayer", "Multiplayer (Private)", "Multiplayer (Public)"], name="mode",
+                          value="Singleplayer"),
+                    actions("-", [
+                        {"label": "Create", "value": "create"},
+                    ], name="action"),
+                ])
                 shared_position = shared_positions[get_query("position_id")]
                 new_game(lambda **_: Game(shared_position.board, shared_position.get_result),
-                            shared_position.options, 'Singleplayer', piece_urls)
+                            shared_position.options, form_result["mode"], piece_urls)
             return
 
-
-        form_result = input_group('New Game', [
-            radio('Mode', ['Singleplayer', 'Multiplayer (Private)', 'Multiplayer (Public)'], name='mode',
-                  value='Singleplayer'),
+        form_result = input_group("New Game", [
+            radio("Mode", ["Singleplayer", "Multiplayer (Private)", "Multiplayer (Public)"], name="mode",
+                  value="Singleplayer"),
             checkbox(
-                'Options',
+                "Options",
                 options=supported_options,
-                name='options',
+                name="options",
                 help_text=f"See details at https://wolfdwyc.github.io/ChessMaker/packaged-variants/"
             ),
-            actions('Public Games', [
-                {'label': f"Join game: {', '.join(public_game.options) or 'standard'}", 'value': game_id}
+            actions("Public Games", [
+                {"label": f"Join game: {', '.join(public_game.options) or 'standard'}", "value": game_id}
                 for game_id, (_, public_game) in public_games.items()
-            ], name='public_games'),
-            actions('-', [
-                {'label': 'Create ', 'value': 'create'},
-            ], name='action'),
+            ], name="public_games"),
+            actions("-", [
+                {"label": "Create", "value": "create"},
+            ], name="action"),
         ])
 
-        if form_result['public_games'] is not None:
-            public_games.pop(form_result['public_games'])
-            join_game(form_result['public_games'])
+        if form_result["public_games"] is not None:
+            public_games.pop(form_result["public_games"])
+            join_game(form_result["public_games"])
             return
 
-        new_game(game_factory, form_result['options'], form_result['mode'], piece_urls)
+        new_game(game_factory, form_result["options"], form_result["mode"], piece_urls)
 
     start_server(main, port=port, remote_access=remote_access, debug=debug)
 
 
 if __name__ == "__main__":
     start_pywebio_chess_server(
         create_game,
         supported_options=["chess960", "knooks", "forced_en_passant", "knight_boosting", "omnipotent_f6_pawn",
                            "siberian_swipe", "il_vaticano", "beta_decay", "la_bastarda", "king_cant_move_to_c2",
                            "vertical_castling", "double_check_to_win", "capture_all_pieces_to_win"],
         piece_urls=PIECE_URLS | {"Knook": ["https://i.imgur.com/UiWcdEb.png", "https://i.imgur.com/g7xTVts.png"]}
+        , debug=True
     )
```

### Comparing `chessmaker-0.4.0/chessmaker/events/event_publisher.py` & `chessmaker-0.4.1/chessmaker/events/event_publisher.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/LICENSE` & `chessmaker-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/pyproject.toml` & `chessmaker-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chessmaker"
-version = "0.4.0"
+version = "0.4.1"
 description = "An easily extendible chess implementation designed to support any custom rule or feature"
 readme = "README.md"
 authors = ["WolfDWyc <yoavwolfdw@gmail.com>",]
 license = "AGPL-3.0-or-later"
 classifiers = [
 "License :: OSI Approved :: GNU Affero General Public License v3",
 "Programming Language :: Python",
```

### Comparing `chessmaker-0.4.0/README.md` & `chessmaker-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `chessmaker-0.4.0/PKG-INFO` & `chessmaker-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chessmaker
-Version: 0.4.0
+Version: 0.4.1
 Summary: An easily extendible chess implementation designed to support any custom rule or feature
 License: AGPL-3.0-or-later
 Keywords: chess
 Author: WolfDWyc
 Author-email: yoavwolfdw@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

