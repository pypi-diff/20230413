# Comparing `tmp/chessmaker-0.1.1.tar.gz` & `tmp/chessmaker-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chessmaker-0.1.1.tar", last modified: Thu Apr 13 00:01:25 2023, max compression
+gzip compressed data, was "chessmaker-0.1.2.tar", last modified: Thu Apr 13 00:44:40 2023, max compression
```

## Comparing `chessmaker-0.1.1.tar` & `chessmaker-0.1.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.993213 chessmaker-0.1.1/
--rw-rw-rw-   0        0        0    35184 2023-04-05 10:50:17.000000 chessmaker-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    42821 2023-04-13 00:01:25.993213 chessmaker-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1432 2023-04-12 23:32:13.000000 chessmaker-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.929214 chessmaker-0.1.1/chessmaker/
--rw-rw-rw-   0        0        0      159 2023-04-12 23:23:56.000000 chessmaker-0.1.1/chessmaker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.940214 chessmaker-0.1.1/chessmaker/chess/
--rw-rw-rw-   0        0        0      198 2023-04-12 23:20:16.000000 chessmaker-0.1.1/chessmaker/chess/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.952214 chessmaker-0.1.1/chessmaker/chess/base/
--rw-rw-rw-   0        0        0      686 2023-04-12 23:23:13.000000 chessmaker-0.1.1/chessmaker/chess/base/__init__.py
--rw-rw-rw-   0        0        0     6797 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/base/board.py
--rw-rw-rw-   0        0        0     1095 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/base/game.py
--rw-rw-rw-   0        0        0      275 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/base/move_option.py
--rw-rw-rw-   0        0        0     3472 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/base/piece.py
--rw-rw-rw-   0        0        0      583 2023-04-12 22:32:25.000000 chessmaker-0.1.1/chessmaker/chess/base/player.py
--rw-rw-rw-   0        0        0      241 2023-04-12 22:32:25.000000 chessmaker-0.1.1/chessmaker/chess/base/position.py
--rw-rw-rw-   0        0        0      708 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/base/rule.py
--rw-rw-rw-   0        0        0     2023 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/base/square.py
--rw-rw-rw-   0        0        0     4045 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/game_factory.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.963214 chessmaker-0.1.1/chessmaker/chess/pieces/
--rw-rw-rw-   0        0        0      607 2023-04-12 23:23:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/__init__.py
--rw-rw-rw-   0        0        0      659 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/bishop.py
--rw-rw-rw-   0        0        0     6570 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/king.py
--rw-rw-rw-   0        0        0      887 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/knight.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.971215 chessmaker-0.1.1/chessmaker/chess/pieces/knook/
--rw-rw-rw-   0        0        0      191 2023-04-12 23:23:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/knook/__init__.py
--rw-rw-rw-   0        0        0      975 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/knook/knook.py
--rw-rw-rw-   0        0        0       30 2023-04-12 22:32:25.000000 chessmaker-0.1.1/chessmaker/chess/pieces/knook/knookable.py
--rw-rw-rw-   0        0        0     1055 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/knook/knookable_knight.py
--rw-rw-rw-   0        0        0     1155 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/knook/knookable_rook.py
--rw-rw-rw-   0        0        0     1528 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/knook/merge_to_knook.py
--rw-rw-rw-   0        0        0     5542 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/pawn.py
--rw-rw-rw-   0        0        0     2458 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/piece_utils.py
--rw-rw-rw-   0        0        0      792 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/queen.py
--rw-rw-rw-   0        0        0     1064 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/rook.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.974214 chessmaker-0.1.1/chessmaker/chess/results/
--rw-rw-rw-   0        0        0       44 2023-04-12 23:20:15.000000 chessmaker-0.1.1/chessmaker/chess/results/__init__.py
--rw-rw-rw-   0        0        0     2428 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/results/simple_result.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.983214 chessmaker-0.1.1/chessmaker/chess/rules/
--rw-rw-rw-   0        0        0      254 2023-04-12 23:20:16.000000 chessmaker-0.1.1/chessmaker/chess/rules/__init__.py
--rw-rw-rw-   0        0        0     3540 2023-04-13 00:00:02.000000 chessmaker-0.1.1/chessmaker/chess/rules/beta_decay.py
--rw-rw-rw-   0        0        0     1927 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/rules/force_en_passant.py
--rw-rw-rw-   0        0        0     3387 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/rules/il_vaticano.py
--rw-rw-rw-   0        0        0     2695 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/rules/knight_boosting.py
--rw-rw-rw-   0        0        0     1685 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/rules/omnipotent_f6_pawn.py
--rw-rw-rw-   0        0        0     2254 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/rules/siberian_swipe.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.986214 chessmaker-0.1.1/chessmaker/clients/
--rw-rw-rw-   0        0        0       52 2023-04-12 23:20:16.000000 chessmaker-0.1.1/chessmaker/clients/__init__.py
--rw-rw-rw-   0        0        0    13708 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/clients/pywebio_ui.py
--rw-rw-rw-   0        0        0      278 2023-04-12 22:32:25.000000 chessmaker-0.1.1/chessmaker/cloneable.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.991214 chessmaker-0.1.1/chessmaker/events/
--rw-rw-rw-   0        0        0      132 2023-04-12 23:20:16.000000 chessmaker-0.1.1/chessmaker/events/__init__.py
--rw-rw-rw-   0        0        0      385 2023-04-12 22:32:25.000000 chessmaker-0.1.1/chessmaker/events/event.py
--rw-rw-rw-   0        0        0      147 2023-04-12 22:32:25.000000 chessmaker-0.1.1/chessmaker/events/event_priority.py
--rw-rw-rw-   0        0        0     3203 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/events/event_publisher.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.938214 chessmaker-0.1.1/chessmaker.egg-info/
--rw-rw-rw-   0        0        0    42821 2023-04-13 00:01:25.000000 chessmaker-0.1.1/chessmaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1697 2023-04-13 00:01:25.000000 chessmaker-0.1.1/chessmaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 00:01:25.000000 chessmaker-0.1.1/chessmaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-13 00:01:25.000000 chessmaker-0.1.1/chessmaker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-13 00:01:25.000000 chessmaker-0.1.1/chessmaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1255 2023-04-13 00:00:59.000000 chessmaker-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 00:01:25.994214 chessmaker-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.208286 chessmaker-0.1.2/
+-rw-rw-rw-   0        0        0    35184 2023-04-05 10:50:17.000000 chessmaker-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0    43007 2023-04-13 00:44:40.207286 chessmaker-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-04-13 00:44:26.000000 chessmaker-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.144287 chessmaker-0.1.2/chessmaker/
+-rw-rw-rw-   0        0        0      159 2023-04-12 23:23:56.000000 chessmaker-0.1.2/chessmaker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.156288 chessmaker-0.1.2/chessmaker/chess/
+-rw-rw-rw-   0        0        0      198 2023-04-12 23:20:16.000000 chessmaker-0.1.2/chessmaker/chess/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.167287 chessmaker-0.1.2/chessmaker/chess/base/
+-rw-rw-rw-   0        0        0      686 2023-04-12 23:23:13.000000 chessmaker-0.1.2/chessmaker/chess/base/__init__.py
+-rw-rw-rw-   0        0        0     6797 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/base/board.py
+-rw-rw-rw-   0        0        0     1095 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/base/game.py
+-rw-rw-rw-   0        0        0      275 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/base/move_option.py
+-rw-rw-rw-   0        0        0     3472 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/base/piece.py
+-rw-rw-rw-   0        0        0      583 2023-04-12 22:32:25.000000 chessmaker-0.1.2/chessmaker/chess/base/player.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 22:32:25.000000 chessmaker-0.1.2/chessmaker/chess/base/position.py
+-rw-rw-rw-   0        0        0      708 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/base/rule.py
+-rw-rw-rw-   0        0        0     2023 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/base/square.py
+-rw-rw-rw-   0        0        0     4049 2023-04-13 00:44:26.000000 chessmaker-0.1.2/chessmaker/chess/game_factory.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.178287 chessmaker-0.1.2/chessmaker/chess/pieces/
+-rw-rw-rw-   0        0        0      607 2023-04-12 23:23:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/__init__.py
+-rw-rw-rw-   0        0        0      659 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/bishop.py
+-rw-rw-rw-   0        0        0     6570 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/king.py
+-rw-rw-rw-   0        0        0      887 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/knight.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.185287 chessmaker-0.1.2/chessmaker/chess/pieces/knook/
+-rw-rw-rw-   0        0        0      191 2023-04-12 23:23:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/knook/__init__.py
+-rw-rw-rw-   0        0        0      975 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/knook/knook.py
+-rw-rw-rw-   0        0        0       30 2023-04-12 22:32:25.000000 chessmaker-0.1.2/chessmaker/chess/pieces/knook/knookable.py
+-rw-rw-rw-   0        0        0     1055 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/knook/knookable_knight.py
+-rw-rw-rw-   0        0        0     1155 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/knook/knookable_rook.py
+-rw-rw-rw-   0        0        0     1528 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/knook/merge_to_knook.py
+-rw-rw-rw-   0        0        0     5542 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/pawn.py
+-rw-rw-rw-   0        0        0     2458 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/piece_utils.py
+-rw-rw-rw-   0        0        0      792 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/queen.py
+-rw-rw-rw-   0        0        0     1064 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/rook.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.188286 chessmaker-0.1.2/chessmaker/chess/results/
+-rw-rw-rw-   0        0        0       44 2023-04-12 23:20:15.000000 chessmaker-0.1.2/chessmaker/chess/results/__init__.py
+-rw-rw-rw-   0        0        0     2428 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/results/simple_result.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.197287 chessmaker-0.1.2/chessmaker/chess/rules/
+-rw-rw-rw-   0        0        0      256 2023-04-13 00:44:26.000000 chessmaker-0.1.2/chessmaker/chess/rules/__init__.py
+-rw-rw-rw-   0        0        0     3540 2023-04-13 00:00:02.000000 chessmaker-0.1.2/chessmaker/chess/rules/beta_decay.py
+-rw-rw-rw-   0        0        0     1929 2023-04-13 00:44:26.000000 chessmaker-0.1.2/chessmaker/chess/rules/forced_en_passant.py
+-rw-rw-rw-   0        0        0     3387 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/rules/il_vaticano.py
+-rw-rw-rw-   0        0        0     2695 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/rules/knight_boosting.py
+-rw-rw-rw-   0        0        0     1685 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/rules/omnipotent_f6_pawn.py
+-rw-rw-rw-   0        0        0     2254 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/rules/siberian_swipe.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.199286 chessmaker-0.1.2/chessmaker/clients/
+-rw-rw-rw-   0        0        0       52 2023-04-12 23:20:16.000000 chessmaker-0.1.2/chessmaker/clients/__init__.py
+-rw-rw-rw-   0        0        0    13709 2023-04-13 00:44:26.000000 chessmaker-0.1.2/chessmaker/clients/pywebio_ui.py
+-rw-rw-rw-   0        0        0      278 2023-04-12 22:32:25.000000 chessmaker-0.1.2/chessmaker/cloneable.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.205286 chessmaker-0.1.2/chessmaker/events/
+-rw-rw-rw-   0        0        0      132 2023-04-12 23:20:16.000000 chessmaker-0.1.2/chessmaker/events/__init__.py
+-rw-rw-rw-   0        0        0      385 2023-04-12 22:32:25.000000 chessmaker-0.1.2/chessmaker/events/event.py
+-rw-rw-rw-   0        0        0      147 2023-04-12 22:32:25.000000 chessmaker-0.1.2/chessmaker/events/event_priority.py
+-rw-rw-rw-   0        0        0     3203 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/events/event_publisher.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.152287 chessmaker-0.1.2/chessmaker.egg-info/
+-rw-rw-rw-   0        0        0    43007 2023-04-13 00:44:40.000000 chessmaker-0.1.2/chessmaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1698 2023-04-13 00:44:40.000000 chessmaker-0.1.2/chessmaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 00:44:40.000000 chessmaker-0.1.2/chessmaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-04-13 00:44:40.000000 chessmaker-0.1.2/chessmaker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-13 00:44:40.000000 chessmaker-0.1.2/chessmaker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1253 2023-04-13 00:40:55.000000 chessmaker-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 00:44:40.208286 chessmaker-0.1.2/setup.cfg
```

### Comparing `chessmaker-0.1.1/LICENSE` & `chessmaker-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/PKG-INFO` & `chessmaker-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chessmaker
-Version: 0.1.1
+Version: 0.1.2
 Summary: An easily extendible chess implementation designed to support any custom rule or feature
 Author-email: WolfDWyc <yoavwolfdw@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,30 +682,34 @@
 License-File: LICENSE
 
 # ChessMaker
 
 An easily extendible chess implementation designed
 to support any custom rule or feature.
 
+**Documentation**: [https://wolfdwyc.github.io/ChessMaker](https://wolfdwyc.github.io/ChessMaker)
+
+**Source Code**: [https://github.com/WolfDWyc/ChessMaker](https://wolfdwyc.github.io/ChessMaker)
+
 ---
 
 ## What is ChessMaker?
 
 ChessMaker is a Python (3.11+) chess implementation that can be extended to support any custom rule or feature.
 It allows you to build almost any variant you can think of easily and quickly.
 
 ChessMaker isn't tied to any GUI, but comes with a thin, [pywebio](https://pywebio.readthedocs.io/en/latest/), multiplayer web interface.
 
-It was inspired by [r/AnarchyChess](https://www.reddit.com/r/AnarchyChess/) - and the pacakged optional rules are almost all inspired by that subreddit.
+It was inspired by [r/AnarchyChess](https://www.reddit.com/r/AnarchyChess/) - and the packaged optional rules are almost all inspired by that subreddit.
 
-The packaged optional rules are:
+These rules are:
 
 * Chess960
 * Knooks
-* Force En Passant
+* Forced En Passant
 * Knight Boosting
 * Siberian Swipe
 * Il Vaticano
 * Beta Decay
 * Omnipotent F6 Pawn
 
 ## What ChessMaker isn't
```

### Comparing `chessmaker-0.1.1/README.md` & `chessmaker-0.1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # ChessMaker
 
 An easily extendible chess implementation designed
 to support any custom rule or feature.
 
+**Documentation**: [https://wolfdwyc.github.io/ChessMaker](https://wolfdwyc.github.io/ChessMaker)
+
+**Source Code**: [https://github.com/WolfDWyc/ChessMaker](https://wolfdwyc.github.io/ChessMaker)
+
 ---
 
 ## What is ChessMaker?
 
 ChessMaker is a Python (3.11+) chess implementation that can be extended to support any custom rule or feature.
 It allows you to build almost any variant you can think of easily and quickly.
 
 ChessMaker isn't tied to any GUI, but comes with a thin, [pywebio](https://pywebio.readthedocs.io/en/latest/), multiplayer web interface.
 
-It was inspired by [r/AnarchyChess](https://www.reddit.com/r/AnarchyChess/) - and the pacakged optional rules are almost all inspired by that subreddit.
+It was inspired by [r/AnarchyChess](https://www.reddit.com/r/AnarchyChess/) - and the packaged optional rules are almost all inspired by that subreddit.
 
-The packaged optional rules are:
+These rules are:
 
 * Chess960
 * Knooks
-* Force En Passant
+* Forced En Passant
 * Knight Boosting
 * Siberian Swipe
 * Il Vaticano
 * Beta Decay
 * Omnipotent F6 Pawn
 
 ## What ChessMaker isn't
```

### Comparing `chessmaker-0.1.1/chessmaker/chess/base/__init__.py` & `chessmaker-0.1.2/chessmaker/chess/base/__init__.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/base/board.py` & `chessmaker-0.1.2/chessmaker/chess/base/board.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/base/game.py` & `chessmaker-0.1.2/chessmaker/chess/base/game.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/base/piece.py` & `chessmaker-0.1.2/chessmaker/chess/base/piece.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/base/player.py` & `chessmaker-0.1.2/chessmaker/chess/base/player.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/base/rule.py` & `chessmaker-0.1.2/chessmaker/chess/base/rule.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/base/square.py` & `chessmaker-0.1.2/chessmaker/chess/base/square.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/game_factory.py` & `chessmaker-0.1.2/chessmaker/chess/game_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 from chessmaker.chess.pieces.knight import Knight
 from chessmaker.chess.pieces.knook.knookable_knight import KnookableKnight
 from chessmaker.chess.pieces.knook.knookable_rook import KnookableRook
 from chessmaker.chess.pieces.pawn import Pawn
 from chessmaker.chess.pieces.queen import Queen
 from chessmaker.chess.pieces.rook import Rook
 from chessmaker.chess.results.simple_result import GetSimpleResult
-from chessmaker.chess.rules import ForceEnPassant, KnightBoosting, OmnipotentF6Pawn, SiberianSwipe, IlVaticano, BetaDecay
+from chessmaker.chess.rules import ForcedEnPassant, KnightBoosting, OmnipotentF6Pawn, SiberianSwipe, IlVaticano, BetaDecay
 
 class A:
     pass
 
 def create_game(
         chess960: bool = False,
         knooks: bool = False,
-        force_en_passant: bool = False,
+        forced_en_passant: bool = False,
         knight_boosting: bool = False,
         omnipotent_f6_pawn: bool = False,
         siberian_swipe: bool = False,
         il_vaticano: bool = False,
         beta_decay: bool = False,
 ):
     _knight = Knight
@@ -76,15 +76,15 @@
 
         return row
 
     piece_row = _piece_row()
 
     rules = []
     for enabled, rule in [
-        (force_en_passant, ForceEnPassant()),
+        (forced_en_passant, ForcedEnPassant()),
         (knight_boosting, KnightBoosting()),
         (siberian_swipe, SiberianSwipe()),
         (il_vaticano, IlVaticano()),
         (omnipotent_f6_pawn, OmnipotentF6Pawn({white: lambda: _up_pawn(white).piece, black: lambda: _down_pawn(black).piece})),
         (beta_decay, BetaDecay([_rook, Bishop,
             lambda player: _up_pawn(player).piece if player == white else _down_pawn(player).piece,
         ])),
```

### Comparing `chessmaker-0.1.1/chessmaker/chess/pieces/__init__.py` & `chessmaker-0.1.2/chessmaker/chess/pieces/__init__.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/pieces/bishop.py` & `chessmaker-0.1.2/chessmaker/chess/pieces/bishop.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/pieces/king.py` & `chessmaker-0.1.2/chessmaker/chess/pieces/king.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/pieces/knight.py` & `chessmaker-0.1.2/chessmaker/chess/pieces/knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/pieces/knook/knook.py` & `chessmaker-0.1.2/chessmaker/chess/pieces/knook/knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/pieces/knook/knookable_knight.py` & `chessmaker-0.1.2/chessmaker/chess/pieces/knook/knookable_knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/pieces/knook/knookable_rook.py` & `chessmaker-0.1.2/chessmaker/chess/pieces/knook/knookable_rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/pieces/knook/merge_to_knook.py` & `chessmaker-0.1.2/chessmaker/chess/pieces/knook/merge_to_knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/pieces/pawn.py` & `chessmaker-0.1.2/chessmaker/chess/pieces/pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/pieces/piece_utils.py` & `chessmaker-0.1.2/chessmaker/chess/pieces/piece_utils.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/pieces/queen.py` & `chessmaker-0.1.2/chessmaker/chess/pieces/queen.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/pieces/rook.py` & `chessmaker-0.1.2/chessmaker/chess/pieces/rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/results/simple_result.py` & `chessmaker-0.1.2/chessmaker/chess/results/simple_result.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/rules/beta_decay.py` & `chessmaker-0.1.2/chessmaker/chess/rules/beta_decay.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/rules/force_en_passant.py` & `chessmaker-0.1.2/chessmaker/chess/rules/forced_en_passant.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from chessmaker.chess.base.piece import BeforeGetMoveOptionsEvent
 from chessmaker.chess.base.player import Player
 from chessmaker.chess.base.rule import Rule
 from chessmaker.chess.pieces.pawn import Pawn
 from chessmaker.events import EventPriority
 
 
-class ForceEnPassant(Rule):
+class ForcedEnPassant(Rule):
     def __init__(self, can_en_passant: dict[Player, bool] = None):
         if can_en_passant is None:
             can_en_passant = defaultdict(lambda: False)
         self.can_en_passant: dict[Player, bool] = can_en_passant
 
     def on_join_board(self, board: Board):
         board.subscribe(BeforeGetMoveOptionsEvent, self.on_before_get_move_options, EventPriority.LOW)
@@ -36,11 +36,11 @@
         move_options = []
         for move_option in event_move_options:
             if move_option.extra.get("en_passant"):
                 move_options.append(move_option)
         event.set_move_options(move_options)
 
     def clone(self):
-        return ForceEnPassant(can_en_passant=self.can_en_passant.copy())
+        return ForcedEnPassant(can_en_passant=self.can_en_passant.copy())
```

### Comparing `chessmaker-0.1.1/chessmaker/chess/rules/il_vaticano.py` & `chessmaker-0.1.2/chessmaker/chess/rules/il_vaticano.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/rules/knight_boosting.py` & `chessmaker-0.1.2/chessmaker/chess/rules/knight_boosting.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/rules/omnipotent_f6_pawn.py` & `chessmaker-0.1.2/chessmaker/chess/rules/omnipotent_f6_pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/chess/rules/siberian_swipe.py` & `chessmaker-0.1.2/chessmaker/chess/rules/siberian_swipe.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker/clients/pywebio_ui.py` & `chessmaker-0.1.2/chessmaker/clients/pywebio_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,9 +348,9 @@
 
         new_game(game_factory, form_result['options'], form_result['mode'])
 
     start_server(main, port=port, remote_access=remote_access, debug=debug)
 
 
 if __name__ == "__main__":
-    start_pywebio_chess_server(create_game, ["chess960", "knooks", "force_en_passant", "knight_boosting", "omnipotent_f6_pawn",
+    start_pywebio_chess_server(create_game, ["chess960", "knooks", "forced_en_passant", "knight_boosting", "omnipotent_f6_pawn",
                               "siberian_swipe", "il_vaticano", "beta_decay"], debug=True)
```

### Comparing `chessmaker-0.1.1/chessmaker/events/event_publisher.py` & `chessmaker-0.1.2/chessmaker/events/event_publisher.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.1/chessmaker.egg-info/PKG-INFO` & `chessmaker-0.1.2/chessmaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chessmaker
-Version: 0.1.1
+Version: 0.1.2
 Summary: An easily extendible chess implementation designed to support any custom rule or feature
 Author-email: WolfDWyc <yoavwolfdw@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,30 +682,34 @@
 License-File: LICENSE
 
 # ChessMaker
 
 An easily extendible chess implementation designed
 to support any custom rule or feature.
 
+**Documentation**: [https://wolfdwyc.github.io/ChessMaker](https://wolfdwyc.github.io/ChessMaker)
+
+**Source Code**: [https://github.com/WolfDWyc/ChessMaker](https://wolfdwyc.github.io/ChessMaker)
+
 ---
 
 ## What is ChessMaker?
 
 ChessMaker is a Python (3.11+) chess implementation that can be extended to support any custom rule or feature.
 It allows you to build almost any variant you can think of easily and quickly.
 
 ChessMaker isn't tied to any GUI, but comes with a thin, [pywebio](https://pywebio.readthedocs.io/en/latest/), multiplayer web interface.
 
-It was inspired by [r/AnarchyChess](https://www.reddit.com/r/AnarchyChess/) - and the pacakged optional rules are almost all inspired by that subreddit.
+It was inspired by [r/AnarchyChess](https://www.reddit.com/r/AnarchyChess/) - and the packaged optional rules are almost all inspired by that subreddit.
 
-The packaged optional rules are:
+These rules are:
 
 * Chess960
 * Knooks
-* Force En Passant
+* Forced En Passant
 * Knight Boosting
 * Siberian Swipe
 * Il Vaticano
 * Beta Decay
 * Omnipotent F6 Pawn
 
 ## What ChessMaker isn't
```

### Comparing `chessmaker-0.1.1/chessmaker.egg-info/SOURCES.txt` & `chessmaker-0.1.2/chessmaker.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 chessmaker/chess/pieces/knook/knookable_knight.py
 chessmaker/chess/pieces/knook/knookable_rook.py
 chessmaker/chess/pieces/knook/merge_to_knook.py
 chessmaker/chess/results/__init__.py
 chessmaker/chess/results/simple_result.py
 chessmaker/chess/rules/__init__.py
 chessmaker/chess/rules/beta_decay.py
-chessmaker/chess/rules/force_en_passant.py
+chessmaker/chess/rules/forced_en_passant.py
 chessmaker/chess/rules/il_vaticano.py
 chessmaker/chess/rules/knight_boosting.py
 chessmaker/chess/rules/omnipotent_f6_pawn.py
 chessmaker/chess/rules/siberian_swipe.py
 chessmaker/clients/__init__.py
 chessmaker/clients/pywebio_ui.py
 chessmaker/events/__init__.py
```

### Comparing `chessmaker-0.1.1/pyproject.toml` & `chessmaker-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["chessmaker", "chessmaker.*"]
 
 [project]
 name = "chessmaker"
-version = "0.1.1"
+version = "0.1.2"
 description = "An easily extendible chess implementation designed to support any custom rule or feature"
 readme = "README.md"
 authors = [{ name = "WolfDWyc", email="yoavwolfdw@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Programming Language :: Python",
@@ -32,11 +32,10 @@
 
 [project.optional-dependencies]
 dev = [
     "mkdocs-material==9.1.6",
     "pydoc-markdown==4.5.1",
 ]
 
-
 [project.urls]
 Homepage = "https://github.com/WolfDWyc/ChessMaker"
```

