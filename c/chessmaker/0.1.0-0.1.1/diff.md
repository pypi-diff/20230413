# Comparing `tmp/chessmaker-0.1.0.tar.gz` & `tmp/chessmaker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chessmaker-0.1.0.tar", last modified: Wed Apr 12 23:50:50 2023, max compression
+gzip compressed data, was "chessmaker-0.1.1.tar", last modified: Thu Apr 13 00:01:25 2023, max compression
```

## Comparing `chessmaker-0.1.0.tar` & `chessmaker-0.1.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 23:50:50.652288 chessmaker-0.1.0/
--rw-rw-rw-   0        0        0    35184 2023-04-05 10:50:17.000000 chessmaker-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    42821 2023-04-12 23:50:50.651287 chessmaker-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1432 2023-04-12 23:32:13.000000 chessmaker-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 23:50:50.587287 chessmaker-0.1.0/chessmaker/
--rw-rw-rw-   0        0        0      159 2023-04-12 23:23:56.000000 chessmaker-0.1.0/chessmaker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 23:50:50.597287 chessmaker-0.1.0/chessmaker/chess/
--rw-rw-rw-   0        0        0      198 2023-04-12 23:20:16.000000 chessmaker-0.1.0/chessmaker/chess/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 23:50:50.608286 chessmaker-0.1.0/chessmaker/chess/base/
--rw-rw-rw-   0        0        0      686 2023-04-12 23:23:13.000000 chessmaker-0.1.0/chessmaker/chess/base/__init__.py
--rw-rw-rw-   0        0        0     6797 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/base/board.py
--rw-rw-rw-   0        0        0     1095 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/base/game.py
--rw-rw-rw-   0        0        0      275 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/base/move_option.py
--rw-rw-rw-   0        0        0     3472 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/base/piece.py
--rw-rw-rw-   0        0        0      583 2023-04-12 22:32:25.000000 chessmaker-0.1.0/chessmaker/chess/base/player.py
--rw-rw-rw-   0        0        0      241 2023-04-12 22:32:25.000000 chessmaker-0.1.0/chessmaker/chess/base/position.py
--rw-rw-rw-   0        0        0      708 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/base/rule.py
--rw-rw-rw-   0        0        0     2023 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/base/square.py
--rw-rw-rw-   0        0        0     4045 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/game_factory.py
-drwxrwxrwx   0        0        0        0 2023-04-12 23:50:50.622287 chessmaker-0.1.0/chessmaker/chess/pieces/
--rw-rw-rw-   0        0        0      607 2023-04-12 23:23:13.000000 chessmaker-0.1.0/chessmaker/chess/pieces/__init__.py
--rw-rw-rw-   0        0        0      659 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/pieces/bishop.py
--rw-rw-rw-   0        0        0     6570 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/pieces/king.py
--rw-rw-rw-   0        0        0      887 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/pieces/knight.py
-drwxrwxrwx   0        0        0        0 2023-04-12 23:50:50.630287 chessmaker-0.1.0/chessmaker/chess/pieces/knook/
--rw-rw-rw-   0        0        0      191 2023-04-12 23:23:13.000000 chessmaker-0.1.0/chessmaker/chess/pieces/knook/__init__.py
--rw-rw-rw-   0        0        0      975 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/pieces/knook/knook.py
--rw-rw-rw-   0        0        0       30 2023-04-12 22:32:25.000000 chessmaker-0.1.0/chessmaker/chess/pieces/knook/knookable.py
--rw-rw-rw-   0        0        0     1055 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/pieces/knook/knookable_knight.py
--rw-rw-rw-   0        0        0     1155 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/pieces/knook/knookable_rook.py
--rw-rw-rw-   0        0        0     1528 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/pieces/knook/merge_to_knook.py
--rw-rw-rw-   0        0        0     5542 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/pieces/pawn.py
--rw-rw-rw-   0        0        0     2458 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/pieces/piece_utils.py
--rw-rw-rw-   0        0        0      792 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/pieces/queen.py
--rw-rw-rw-   0        0        0     1064 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/pieces/rook.py
-drwxrwxrwx   0        0        0        0 2023-04-12 23:50:50.633287 chessmaker-0.1.0/chessmaker/chess/results/
--rw-rw-rw-   0        0        0       44 2023-04-12 23:20:15.000000 chessmaker-0.1.0/chessmaker/chess/results/__init__.py
--rw-rw-rw-   0        0        0     2428 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/results/simple_result.py
-drwxrwxrwx   0        0        0        0 2023-04-12 23:50:50.642287 chessmaker-0.1.0/chessmaker/chess/rules/
--rw-rw-rw-   0        0        0      254 2023-04-12 23:20:16.000000 chessmaker-0.1.0/chessmaker/chess/rules/__init__.py
--rw-rw-rw-   0        0        0     3501 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/rules/beta_decay.py
--rw-rw-rw-   0        0        0     1927 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/rules/force_en_passant.py
--rw-rw-rw-   0        0        0     3387 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/rules/il_vaticano.py
--rw-rw-rw-   0        0        0     2695 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/rules/knight_boosting.py
--rw-rw-rw-   0        0        0     1685 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/rules/omnipotent_f6_pawn.py
--rw-rw-rw-   0        0        0     2254 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/chess/rules/siberian_swipe.py
-drwxrwxrwx   0        0        0        0 2023-04-12 23:50:50.644287 chessmaker-0.1.0/chessmaker/clients/
--rw-rw-rw-   0        0        0       52 2023-04-12 23:20:16.000000 chessmaker-0.1.0/chessmaker/clients/__init__.py
--rw-rw-rw-   0        0        0    13708 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/clients/pywebio_ui.py
--rw-rw-rw-   0        0        0      278 2023-04-12 22:32:25.000000 chessmaker-0.1.0/chessmaker/cloneable.py
-drwxrwxrwx   0        0        0        0 2023-04-12 23:50:50.649288 chessmaker-0.1.0/chessmaker/events/
--rw-rw-rw-   0        0        0      132 2023-04-12 23:20:16.000000 chessmaker-0.1.0/chessmaker/events/__init__.py
--rw-rw-rw-   0        0        0      385 2023-04-12 22:32:25.000000 chessmaker-0.1.0/chessmaker/events/event.py
--rw-rw-rw-   0        0        0      147 2023-04-12 22:32:25.000000 chessmaker-0.1.0/chessmaker/events/event_priority.py
--rw-rw-rw-   0        0        0     3203 2023-04-12 22:57:13.000000 chessmaker-0.1.0/chessmaker/events/event_publisher.py
-drwxrwxrwx   0        0        0        0 2023-04-12 23:50:50.594287 chessmaker-0.1.0/chessmaker.egg-info/
--rw-rw-rw-   0        0        0    42821 2023-04-12 23:50:50.000000 chessmaker-0.1.0/chessmaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1697 2023-04-12 23:50:50.000000 chessmaker-0.1.0/chessmaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 23:50:50.000000 chessmaker-0.1.0/chessmaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-12 23:50:50.000000 chessmaker-0.1.0/chessmaker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-12 23:50:50.000000 chessmaker-0.1.0/chessmaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1255 2023-04-12 23:50:02.000000 chessmaker-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 23:50:50.652288 chessmaker-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.993213 chessmaker-0.1.1/
+-rw-rw-rw-   0        0        0    35184 2023-04-05 10:50:17.000000 chessmaker-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    42821 2023-04-13 00:01:25.993213 chessmaker-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1432 2023-04-12 23:32:13.000000 chessmaker-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.929214 chessmaker-0.1.1/chessmaker/
+-rw-rw-rw-   0        0        0      159 2023-04-12 23:23:56.000000 chessmaker-0.1.1/chessmaker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.940214 chessmaker-0.1.1/chessmaker/chess/
+-rw-rw-rw-   0        0        0      198 2023-04-12 23:20:16.000000 chessmaker-0.1.1/chessmaker/chess/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.952214 chessmaker-0.1.1/chessmaker/chess/base/
+-rw-rw-rw-   0        0        0      686 2023-04-12 23:23:13.000000 chessmaker-0.1.1/chessmaker/chess/base/__init__.py
+-rw-rw-rw-   0        0        0     6797 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/base/board.py
+-rw-rw-rw-   0        0        0     1095 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/base/game.py
+-rw-rw-rw-   0        0        0      275 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/base/move_option.py
+-rw-rw-rw-   0        0        0     3472 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/base/piece.py
+-rw-rw-rw-   0        0        0      583 2023-04-12 22:32:25.000000 chessmaker-0.1.1/chessmaker/chess/base/player.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 22:32:25.000000 chessmaker-0.1.1/chessmaker/chess/base/position.py
+-rw-rw-rw-   0        0        0      708 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/base/rule.py
+-rw-rw-rw-   0        0        0     2023 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/base/square.py
+-rw-rw-rw-   0        0        0     4045 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/game_factory.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.963214 chessmaker-0.1.1/chessmaker/chess/pieces/
+-rw-rw-rw-   0        0        0      607 2023-04-12 23:23:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/__init__.py
+-rw-rw-rw-   0        0        0      659 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/bishop.py
+-rw-rw-rw-   0        0        0     6570 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/king.py
+-rw-rw-rw-   0        0        0      887 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/knight.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.971215 chessmaker-0.1.1/chessmaker/chess/pieces/knook/
+-rw-rw-rw-   0        0        0      191 2023-04-12 23:23:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/knook/__init__.py
+-rw-rw-rw-   0        0        0      975 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/knook/knook.py
+-rw-rw-rw-   0        0        0       30 2023-04-12 22:32:25.000000 chessmaker-0.1.1/chessmaker/chess/pieces/knook/knookable.py
+-rw-rw-rw-   0        0        0     1055 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/knook/knookable_knight.py
+-rw-rw-rw-   0        0        0     1155 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/knook/knookable_rook.py
+-rw-rw-rw-   0        0        0     1528 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/knook/merge_to_knook.py
+-rw-rw-rw-   0        0        0     5542 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/pawn.py
+-rw-rw-rw-   0        0        0     2458 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/piece_utils.py
+-rw-rw-rw-   0        0        0      792 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/queen.py
+-rw-rw-rw-   0        0        0     1064 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/pieces/rook.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.974214 chessmaker-0.1.1/chessmaker/chess/results/
+-rw-rw-rw-   0        0        0       44 2023-04-12 23:20:15.000000 chessmaker-0.1.1/chessmaker/chess/results/__init__.py
+-rw-rw-rw-   0        0        0     2428 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/results/simple_result.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.983214 chessmaker-0.1.1/chessmaker/chess/rules/
+-rw-rw-rw-   0        0        0      254 2023-04-12 23:20:16.000000 chessmaker-0.1.1/chessmaker/chess/rules/__init__.py
+-rw-rw-rw-   0        0        0     3540 2023-04-13 00:00:02.000000 chessmaker-0.1.1/chessmaker/chess/rules/beta_decay.py
+-rw-rw-rw-   0        0        0     1927 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/rules/force_en_passant.py
+-rw-rw-rw-   0        0        0     3387 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/rules/il_vaticano.py
+-rw-rw-rw-   0        0        0     2695 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/rules/knight_boosting.py
+-rw-rw-rw-   0        0        0     1685 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/rules/omnipotent_f6_pawn.py
+-rw-rw-rw-   0        0        0     2254 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/chess/rules/siberian_swipe.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.986214 chessmaker-0.1.1/chessmaker/clients/
+-rw-rw-rw-   0        0        0       52 2023-04-12 23:20:16.000000 chessmaker-0.1.1/chessmaker/clients/__init__.py
+-rw-rw-rw-   0        0        0    13708 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/clients/pywebio_ui.py
+-rw-rw-rw-   0        0        0      278 2023-04-12 22:32:25.000000 chessmaker-0.1.1/chessmaker/cloneable.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.991214 chessmaker-0.1.1/chessmaker/events/
+-rw-rw-rw-   0        0        0      132 2023-04-12 23:20:16.000000 chessmaker-0.1.1/chessmaker/events/__init__.py
+-rw-rw-rw-   0        0        0      385 2023-04-12 22:32:25.000000 chessmaker-0.1.1/chessmaker/events/event.py
+-rw-rw-rw-   0        0        0      147 2023-04-12 22:32:25.000000 chessmaker-0.1.1/chessmaker/events/event_priority.py
+-rw-rw-rw-   0        0        0     3203 2023-04-12 22:57:13.000000 chessmaker-0.1.1/chessmaker/events/event_publisher.py
+drwxrwxrwx   0        0        0        0 2023-04-13 00:01:25.938214 chessmaker-0.1.1/chessmaker.egg-info/
+-rw-rw-rw-   0        0        0    42821 2023-04-13 00:01:25.000000 chessmaker-0.1.1/chessmaker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1697 2023-04-13 00:01:25.000000 chessmaker-0.1.1/chessmaker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 00:01:25.000000 chessmaker-0.1.1/chessmaker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-04-13 00:01:25.000000 chessmaker-0.1.1/chessmaker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-13 00:01:25.000000 chessmaker-0.1.1/chessmaker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1255 2023-04-13 00:00:59.000000 chessmaker-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 00:01:25.994214 chessmaker-0.1.1/setup.cfg
```

### Comparing `chessmaker-0.1.0/LICENSE` & `chessmaker-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/PKG-INFO` & `chessmaker-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chessmaker
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easily extendible chess implementation designed to support any custom rule or feature
 Author-email: WolfDWyc <yoavwolfdw@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `chessmaker-0.1.0/README.md` & `chessmaker-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/base/__init__.py` & `chessmaker-0.1.1/chessmaker/chess/base/__init__.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/base/board.py` & `chessmaker-0.1.1/chessmaker/chess/base/board.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/base/game.py` & `chessmaker-0.1.1/chessmaker/chess/base/game.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/base/piece.py` & `chessmaker-0.1.1/chessmaker/chess/base/piece.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/base/player.py` & `chessmaker-0.1.1/chessmaker/chess/base/player.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/base/rule.py` & `chessmaker-0.1.1/chessmaker/chess/base/rule.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/base/square.py` & `chessmaker-0.1.1/chessmaker/chess/base/square.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/game_factory.py` & `chessmaker-0.1.1/chessmaker/chess/game_factory.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/pieces/__init__.py` & `chessmaker-0.1.1/chessmaker/chess/pieces/__init__.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/pieces/bishop.py` & `chessmaker-0.1.1/chessmaker/chess/pieces/bishop.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/pieces/king.py` & `chessmaker-0.1.1/chessmaker/chess/pieces/king.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/pieces/knight.py` & `chessmaker-0.1.1/chessmaker/chess/pieces/knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/pieces/knook/knook.py` & `chessmaker-0.1.1/chessmaker/chess/pieces/knook/knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/pieces/knook/knookable_knight.py` & `chessmaker-0.1.1/chessmaker/chess/pieces/knook/knookable_knight.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/pieces/knook/knookable_rook.py` & `chessmaker-0.1.1/chessmaker/chess/pieces/knook/knookable_rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/pieces/knook/merge_to_knook.py` & `chessmaker-0.1.1/chessmaker/chess/pieces/knook/merge_to_knook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/pieces/pawn.py` & `chessmaker-0.1.1/chessmaker/chess/pieces/pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/pieces/piece_utils.py` & `chessmaker-0.1.1/chessmaker/chess/pieces/piece_utils.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/pieces/queen.py` & `chessmaker-0.1.1/chessmaker/chess/pieces/queen.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/pieces/rook.py` & `chessmaker-0.1.1/chessmaker/chess/pieces/rook.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/results/simple_result.py` & `chessmaker-0.1.1/chessmaker/chess/results/simple_result.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/rules/beta_decay.py` & `chessmaker-0.1.1/chessmaker/chess/rules/beta_decay.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from chessmaker.chess.base.piece import Piece, BeforeGetMoveOptionsEvent, BeforeMoveEvent, AfterMoveEvent
 from chessmaker.chess.base.player import Player
 from chessmaker.chess.base.rule import Rule
 from chessmaker.chess.pieces.piece_utils import iterate_until_blocked
 from chessmaker.chess.pieces.queen import Queen
 from chessmaker.events import EventPriority
 
+sign = lambda x: x and (1, -1)[x < 0]
 
 class BetaDecay(Rule):
     def __init__(self, decay_to_pieces: list[Callable[[Player], Piece]]):
         self.decay_to_pieces: list[Callable[[Player], Piece]] = decay_to_pieces
 
     def on_join_board(self, board: Board):
         for piece in board.get_pieces():
```

### Comparing `chessmaker-0.1.0/chessmaker/chess/rules/force_en_passant.py` & `chessmaker-0.1.1/chessmaker/chess/rules/force_en_passant.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/rules/il_vaticano.py` & `chessmaker-0.1.1/chessmaker/chess/rules/il_vaticano.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/rules/knight_boosting.py` & `chessmaker-0.1.1/chessmaker/chess/rules/knight_boosting.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/rules/omnipotent_f6_pawn.py` & `chessmaker-0.1.1/chessmaker/chess/rules/omnipotent_f6_pawn.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/chess/rules/siberian_swipe.py` & `chessmaker-0.1.1/chessmaker/chess/rules/siberian_swipe.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/clients/pywebio_ui.py` & `chessmaker-0.1.1/chessmaker/clients/pywebio_ui.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker/events/event_publisher.py` & `chessmaker-0.1.1/chessmaker/events/event_publisher.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/chessmaker.egg-info/PKG-INFO` & `chessmaker-0.1.1/chessmaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chessmaker
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easily extendible chess implementation designed to support any custom rule or feature
 Author-email: WolfDWyc <yoavwolfdw@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `chessmaker-0.1.0/chessmaker.egg-info/SOURCES.txt` & `chessmaker-0.1.1/chessmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.0/pyproject.toml` & `chessmaker-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["chessmaker", "chessmaker.*"]
 
 [project]
 name = "chessmaker"
-version = "0.1.0"
+version = "0.1.1"
 description = "An easily extendible chess implementation designed to support any custom rule or feature"
 readme = "README.md"
 authors = [{ name = "WolfDWyc", email="yoavwolfdw@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Programming Language :: Python",
```

