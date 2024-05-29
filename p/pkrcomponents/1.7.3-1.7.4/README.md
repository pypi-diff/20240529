# Comparing `tmp/pkrcomponents-1.7.3.tar.gz` & `tmp/pkrcomponents-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkrcomponents-1.7.3.tar", last modified: Mon May 27 23:04:50 2024, max compression
+gzip compressed data, was "pkrcomponents-1.7.4.tar", last modified: Wed May 29 11:11:12 2024, max compression
```

## Comparing `pkrcomponents-1.7.3.tar` & `pkrcomponents-1.7.4.tar`

### file list

```diff
@@ -1,50 +1,38 @@
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 23:04:49.991589 pkrcomponents-1.7.3/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 23:04:49.436228 pkrcomponents-1.7.3/.pytest_cache/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.7.3/.pytest_cache/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.7.3/LICENSE.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-1.7.3/MANIFEST.in
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-27 23:04:49.981583 pkrcomponents-1.7.3/PKG-INFO
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-1.7.3/README.md
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      267 2023-07-18 00:15:12.000000 pkrcomponents-1.7.3/README.rst
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1456 2024-05-27 23:02:47.000000 pkrcomponents-1.7.3/coverage.txt
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 23:04:49.730512 pkrcomponents-1.7.3/pkrcomponents/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.7.3/pkrcomponents/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.7.3/pkrcomponents/_common.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      612 2024-05-27 17:41:46.000000 pkrcomponents-1.7.3/pkrcomponents/action.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-1.7.3/pkrcomponents/bitcard.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.7.3/pkrcomponents/board.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      628 2024-05-27 15:52:21.000000 pkrcomponents-1.7.3/pkrcomponents/buy_in.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     5296 2024-05-15 11:58:01.000000 pkrcomponents-1.7.3/pkrcomponents/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3439 2024-05-27 17:30:11.000000 pkrcomponents-1.7.3/pkrcomponents/constants.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.7.3/pkrcomponents/evaluator.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13075 2024-05-27 18:44:25.000000 pkrcomponents-1.7.3/pkrcomponents/hand.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      790 2024-05-27 15:24:49.000000 pkrcomponents-1.7.3/pkrcomponents/level.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1382 2024-05-27 17:30:11.000000 pkrcomponents-1.7.3/pkrcomponents/listings.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.7.3/pkrcomponents/lookup_table.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 23:04:49.746139 pkrcomponents-1.7.3/pkrcomponents/models/
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 23:04:49.824922 pkrcomponents-1.7.3/pkrcomponents/models/actions/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      906 2023-11-10 18:09:18.000000 pkrcomponents-1.7.3/pkrcomponents/models/actions/move.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      251 2023-11-10 18:03:03.000000 pkrcomponents-1.7.3/pkrcomponents/models/actions/sequence.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      730 2023-11-10 19:18:13.000000 pkrcomponents-1.7.3/pkrcomponents/models/actions/street.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2181 2023-11-10 17:45:16.000000 pkrcomponents-1.7.3/pkrcomponents/models/amount.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 23:04:49.903450 pkrcomponents-1.7.3/pkrcomponents/models/cards/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      865 2024-04-16 09:33:15.000000 pkrcomponents-1.7.3/pkrcomponents/models/cards/card.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1526 2023-11-10 19:31:05.000000 pkrcomponents-1.7.3/pkrcomponents/models/cards/rank.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      911 2023-11-10 19:18:13.000000 pkrcomponents-1.7.3/pkrcomponents/models/cards/suit.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 23:04:49.919082 pkrcomponents-1.7.3/pkrcomponents/models/pots/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      958 2023-11-10 19:09:00.000000 pkrcomponents-1.7.3/pkrcomponents/models/pots/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2246 2024-05-27 16:04:03.000000 pkrcomponents-1.7.3/pkrcomponents/payout.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.7.3/pkrcomponents/players.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1039 2024-05-27 14:58:43.000000 pkrcomponents-1.7.3/pkrcomponents/pot.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    16733 2024-05-27 20:36:01.000000 pkrcomponents-1.7.3/pkrcomponents/table.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)    10491 2024-05-27 20:24:06.000000 pkrcomponents-1.7.3/pkrcomponents/table_player.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2717 2024-05-27 17:10:53.000000 pkrcomponents-1.7.3/pkrcomponents/tournament.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 23:04:49.950333 pkrcomponents-1.7.3/pkrcomponents/utils/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:06:12.000000 pkrcomponents-1.7.3/pkrcomponents/utils/__init__.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      301 2024-05-27 18:51:06.000000 pkrcomponents-1.7.3/pkrcomponents/utils/converters.py
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      371 2024-05-27 20:12:18.000000 pkrcomponents-1.7.3/pkrcomponents/utils/validators.py
-drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 23:04:49.981583 pkrcomponents-1.7.3/pkrcomponents.egg-info/
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      968 2024-05-27 23:04:48.000000 pkrcomponents-1.7.3/pkrcomponents.egg-info/SOURCES.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.7.3/requirements.txt
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-27 23:04:49.991589 pkrcomponents-1.7.3/setup.cfg
--rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1399 2024-05-27 22:58:49.000000 pkrcomponents-1.7.3/setup.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 11:11:12.488982 pkrcomponents-1.7.4/
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 11:11:11.715634 pkrcomponents-1.7.4/.pytest_cache/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      310 2024-04-16 09:27:16.000000 pkrcomponents-1.7.4/.pytest_cache/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1077 2023-11-10 16:45:14.000000 pkrcomponents-1.7.4/LICENSE.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      820 2024-05-24 19:24:47.000000 pkrcomponents-1.7.4/MANIFEST.in
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      951 2024-05-29 11:11:12.473321 pkrcomponents-1.7.4/PKG-INFO
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      224 2024-05-24 00:25:51.000000 pkrcomponents-1.7.4/README.md
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1512 2024-05-29 11:07:46.000000 pkrcomponents-1.7.4/coverage.txt
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 11:11:12.395083 pkrcomponents-1.7.4/pkrcomponents/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2023-07-18 00:15:12.000000 pkrcomponents-1.7.4/pkrcomponents/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     2954 2023-07-18 00:15:12.000000 pkrcomponents-1.7.4/pkrcomponents/_common.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      933 2024-05-27 23:40:01.000000 pkrcomponents-1.7.4/pkrcomponents/action.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     7569 2024-05-24 00:57:29.000000 pkrcomponents-1.7.4/pkrcomponents/bitcard.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3948 2024-05-15 15:52:00.000000 pkrcomponents-1.7.4/pkrcomponents/board.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1386 2024-05-29 10:10:09.000000 pkrcomponents-1.7.4/pkrcomponents/buy_in.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4409 2024-05-29 11:00:59.000000 pkrcomponents-1.7.4/pkrcomponents/card.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3439 2024-05-27 17:30:11.000000 pkrcomponents-1.7.4/pkrcomponents/constants.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1401 2024-05-29 11:06:38.000000 pkrcomponents-1.7.4/pkrcomponents/deck.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3103 2023-07-18 00:15:12.000000 pkrcomponents-1.7.4/pkrcomponents/evaluator.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    13075 2024-05-27 18:44:25.000000 pkrcomponents-1.7.4/pkrcomponents/hand.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1586 2024-05-29 09:57:04.000000 pkrcomponents-1.7.4/pkrcomponents/level.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1382 2024-05-27 17:30:11.000000 pkrcomponents-1.7.4/pkrcomponents/listings.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     9831 2023-07-18 00:15:12.000000 pkrcomponents-1.7.4/pkrcomponents/lookup_table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3998 2024-05-29 10:44:39.000000 pkrcomponents-1.7.4/pkrcomponents/payout.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     4434 2024-05-15 18:17:46.000000 pkrcomponents-1.7.4/pkrcomponents/players.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1429 2024-05-29 10:34:29.000000 pkrcomponents-1.7.4/pkrcomponents/pot.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    16774 2024-05-29 11:06:38.000000 pkrcomponents-1.7.4/pkrcomponents/table.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)    14901 2024-05-29 10:39:42.000000 pkrcomponents-1.7.4/pkrcomponents/table_player.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     3439 2024-05-29 09:25:32.000000 pkrcomponents-1.7.4/pkrcomponents/tournament.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 11:11:12.458308 pkrcomponents-1.7.4/pkrcomponents/utils/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-27 17:06:12.000000 pkrcomponents-1.7.4/pkrcomponents/utils/__init__.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      301 2024-05-27 18:51:06.000000 pkrcomponents-1.7.4/pkrcomponents/utils/converters.py
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      371 2024-05-27 20:12:18.000000 pkrcomponents-1.7.4/pkrcomponents/utils/validators.py
+drwxrwxrwx   0 manggy    (1000) manggy    (1000)        0 2024-05-29 11:11:12.473321 pkrcomponents-1.7.4/pkrcomponents.egg-info/
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      693 2024-05-29 11:11:09.000000 pkrcomponents-1.7.4/pkrcomponents.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)      315 2023-07-18 00:15:12.000000 pkrcomponents-1.7.4/requirements.txt
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)       38 2024-05-29 11:11:12.488982 pkrcomponents-1.7.4/setup.cfg
+-rwxrwxrwx   0 manggy    (1000) manggy    (1000)     1399 2024-05-27 22:58:49.000000 pkrcomponents-1.7.4/setup.py
```

### Comparing `pkrcomponents-1.7.3/LICENSE.txt` & `pkrcomponents-1.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.3/MANIFEST.in` & `pkrcomponents-1.7.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.3/PKG-INFO` & `pkrcomponents-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkrcomponents
-Version: 1.7.3
+Version: 1.7.4
 Summary: A Poker Package
 Home-page: https://github.com/manggy94/PokerComponents
 Author: Alexandre MANGWA
 Author-email: alex.mangwa@gmail.com
 License: MIT
 Keywords: poker pkrcomponents pkr
 Platform: UNKNOWN
```

### Comparing `pkrcomponents-1.7.3/coverage.txt` & `pkrcomponents-1.7.4/coverage.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 -------------------------------------------------------
 pkrcomponents/__init__.py               0      0   100%
 pkrcomponents/_common.py               48      0   100%
 pkrcomponents/action.py                11      0   100%
 pkrcomponents/bitcard.py               68      0   100%
 pkrcomponents/board.py                 81      0   100%
 pkrcomponents/buy_in.py                14      0   100%
-pkrcomponents/card.py                 112      1    99%
+pkrcomponents/card.py                  87      0   100%
 pkrcomponents/constants.py             71      0   100%
+pkrcomponents/deck.py                  26      1    96%
 pkrcomponents/evaluator.py             28      0   100%
 pkrcomponents/hand.py                 228      0   100%
 pkrcomponents/level.py                 17      0   100%
 pkrcomponents/listings.py              16      0   100%
 pkrcomponents/lookup_table.py         112      0   100%
-pkrcomponents/payout.py                39      0   100%
+pkrcomponents/payout.py                37      0   100%
 pkrcomponents/players.py               96      0   100%
 pkrcomponents/pot.py                   13      0   100%
 pkrcomponents/table.py                327      4    99%
-pkrcomponents/table_player.py         183      2    99%
+pkrcomponents/table_player.py         182      2    99%
 pkrcomponents/tournament.py            46      0   100%
 pkrcomponents/utils/__init__.py         0      0   100%
 pkrcomponents/utils/converters.py       6      1    83%
 pkrcomponents/utils/validators.py       7      0   100%
 -------------------------------------------------------
-TOTAL                                1523      8    99%
+TOTAL                                1521      8    99%
```

### Comparing `pkrcomponents-1.7.3/pkrcomponents/_common.py` & `pkrcomponents-1.7.4/pkrcomponents/_common.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.3/pkrcomponents/action.py` & `pkrcomponents-1.7.4/pkrcomponents/action.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,26 @@
 
 from pkrcomponents.constants import ActionMove
 from pkrcomponents.table_player import TablePlayer
 
 
 @define
 class Action:
-    """Class defining different possible actions and amounts a table_player can do"""
+    """
+    This class represents an action made by a player in a poker game
+
+    Attributes:
+        player(TablePlayer): The player making the action
+        move(ActionMove): The move made by the player
+        value(float): The value of the move made by the player
+
+    Methods:
+        __str__(): Returns a string representation of the action
+
+    """
 
     player = field(validator=[instance_of(TablePlayer)])
-    move = field(default=ActionMove.CALL, validator=[instance_of(ActionMove)])
-    value = field(default=0, validator=[ge(0), instance_of((float, int))])
+    move = field(default=ActionMove.CALL, validator=[instance_of(ActionMove)], converter=ActionMove)
+    value = field(default=0, validator=[ge(0), instance_of(float)], converter=float)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"{self.player.name} does a {self.move} for {self.value}"
```

### Comparing `pkrcomponents-1.7.3/pkrcomponents/bitcard.py` & `pkrcomponents-1.7.4/pkrcomponents/bitcard.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.3/pkrcomponents/board.py` & `pkrcomponents-1.7.4/pkrcomponents/board.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.3/pkrcomponents/card.py` & `pkrcomponents-1.7.4/pkrcomponents/card.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
+"""This module contains the Card class, which represents a playing card.
+It also contains the Rank and Suit classes, which are used to define the rank and suit of a card."""
 from itertools import product
 from functools import total_ordering
 
-import random
-
 from pkrcomponents._common import PokerEnum, _ReprMixin
 
-__all__ = ["Suit", "Rank", "Card", "FACE_RANKS", "BROADWAY_RANKS", "Deck"]
+__all__ = ["Suit", "Rank", "Card", "FACE_RANKS", "BROADWAY_RANKS"]
 
 
 class Suit(PokerEnum):
     """
-    Suit of a card
+    Suit of a card: Clubs, Diamonds, Hearts, Spades
     """
     CLUBS = "c", "clubs", "♣", "C"
     DIAMONDS = "d", "diamonds", "♦", "D"
     HEARTS = "h", "hearts", "♥", "H"
     SPADES = "s", "spades", "♠", "S"
-    # Can't make alias with redefined value property
-    # because of a bug in stdlib enum module (line 162)
-    # C = '♣', 'c', 'C', 'clubs'
 
 
 class Rank(PokerEnum):
     """
-    Rank of a card
+    Rank of a card in a deck, from 2 to Ace.
+
+    Methods:
+        difference: tells the numerical difference between two ranks
     """
     DEUCE = "2", 2
     THREE = "3", 3
     FOUR = "4", 4
     FIVE = "5", 5
     SIX = "6", 6
     SEVEN = "7", 7
@@ -36,16 +36,25 @@
     TEN = "T", 10
     JACK = ("J",)
     QUEEN = ("Q",)
     KING = ("K",)
     ACE = "A", 1
 
     @classmethod
-    def difference(cls, first, second):
-        """Tells the numerical difference between two ranks."""
+    def difference(cls, first, second) -> int:
+        """
+        Tells the numerical difference between two ranks.
+
+        Args:
+            first (Rank): the first rank
+            second (Rank): the second rank
+
+        Returns:
+            int: the difference between the two ranks
+        """
 
         # so we always get a Rank instance even if string were passed in
         first, second = cls(first), cls(second)
         rank_list = list(cls)
         a = rank_list.index(first)+2
         b = rank_list.index(second)+2
         if a == 14:
@@ -116,80 +125,29 @@
     def __str__(self):
         return f"{self.rank}{self.suit}"
 
     def __sub__(self, other):
         return self.rank - other.rank
 
     @property
-    def is_face(self):
+    def is_face(self) -> bool:
         """
         Indicates if the card is a face
         """
         return self.rank in FACE_RANKS
 
     @property
-    def is_broadway(self):
+    def is_broadway(self) -> bool:
         """
         Indicates if the card is a broadway
         """
         return self.rank in BROADWAY_RANKS
 
     @classmethod
     def make_random(cls):
         """Returns a random Card instance."""
         self = object.__new__(cls)
         self.rank = Rank.make_random()
         self.suit = Suit.make_random()
         return self
 
 
-class Deck:
-    """A deck of cards"""
-
-    def __init__(self):
-        self.cards = list(Card)
-
-    def __len__(self):
-        return self.cards.__len__()
-
-    def shuffle(self):
-        """
-        Randomly shuffles the deck
-        """
-        random.shuffle(self.cards)
-
-    def reset(self):
-        """Re-initializes the deck and shuffles it"""
-        self.cards = list(Card)
-        self.shuffle()
-
-    def draw(self, cd=None):
-        """
-        Returns a card from the deck
-        If the parameter card is given, it returns the card at stake and pops it from the deck
-        """
-        if not cd:
-            return self.cards.pop()
-        else:
-            cd = Card(cd)
-            idx = self.cards.index(cd)
-            return self.cards.pop(idx)
-
-    def replace(self, card):
-        """
-        Replaces a card in the deck
-        """
-        if card not in self.cards:
-            self.cards.append(card)
-
-    @property
-    def len(self):
-        """
-        Returns the number of cards currently in the deck
-        """
-        return self.__len__()
-
-    def to_json(self):
-        return {
-            "cards": [f"{card}" for card in self.cards],
-            "len": self.len
-        }
```

### Comparing `pkrcomponents-1.7.3/pkrcomponents/constants.py` & `pkrcomponents-1.7.4/pkrcomponents/constants.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.3/pkrcomponents/evaluator.py` & `pkrcomponents-1.7.4/pkrcomponents/evaluator.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.3/pkrcomponents/hand.py` & `pkrcomponents-1.7.4/pkrcomponents/hand.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.3/pkrcomponents/listings.py` & `pkrcomponents-1.7.4/pkrcomponents/listings.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.3/pkrcomponents/lookup_table.py` & `pkrcomponents-1.7.4/pkrcomponents/lookup_table.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.3/pkrcomponents/models/cards/suit.py` & `pkrcomponents-1.7.4/pkrcomponents/deck.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,56 @@
-from functools import cached_property
+"""This module contains the Deck class, which represents a deck of cards."""
+import random
+from pkrcomponents.card import Card
 
-SUIT_NAMES = ["CLUBS", "DIAMONDS", "HEARTS", "SPADES"]
-SUIT_SYMBOLS = ["♣", "♦", "♥", "♠"]
 
+class Deck:
+    """A deck of cards"""
 
-class Suit:
-    """
-    A model to describe poker cards suits
-    """
-    name: str
-    symbol: str
-    short_name: str
-    pk: int
+    def __init__(self):
+        self.cards = list(Card)
 
-    def __init__(self, name, symbol):
-        self.name = name
-        self.symbol = symbol
+    def __len__(self):
+        return self.cards.__len__()
 
-    def __str__(self):
-        return self.symbol
+    def shuffle(self):
+        """
+        Randomly shuffles the deck
+        """
+        random.shuffle(self.cards)
 
-    def __repr__(self):
-        return f"{self.__class__.__name__}('{self.name}')"
+    def reset(self):
+        """Re-initializes the deck and shuffles it"""
+        self.cards = list(Card)
+        self.shuffle()
 
-    def __lt__(self, other):
-        return self.pk < other.pk
+    def draw(self, card=None):
+        """
+        Returns a card from the deck
+        If the parameter card is given, it returns the card at stake and pops it from the deck
+        """
+        if not card:
+            return self.cards.pop()
+        else:
+            card = Card(card)
+            idx = self.cards.index(card)
+            return self.cards.pop(idx)
 
-    @cached_property
-    def short_name(self):
+    def replace(self, card):
         """
-        Returns the short name of the suit
+        Replaces a card in the deck
         """
-        return self.name[0].lower()
+        if card not in self.cards:
+            self.cards.append(card)
 
-    @cached_property
-    def pk(self):
+    @property
+    def len(self):
         """
-        Returns the primary key of the suit
+        Returns the number of cards currently in the deck
         """
-        return SUIT_NAMES.index(self.name) + 1
+        return self.__len__()
+
+    def to_json(self):
+        return {
+            "cards": [f"{card}" for card in self.cards],
+            "len": self.len
+        }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pkrcomponents-1.7.3/pkrcomponents/players.py` & `pkrcomponents-1.7.4/pkrcomponents/players.py`

 * *Files identical despite different names*

### Comparing `pkrcomponents-1.7.3/pkrcomponents/pot.py` & `pkrcomponents-1.7.4/pkrcomponents/pot.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,21 +6,36 @@
 
 from attrs import define, field
 from attrs.validators import instance_of, ge
 
 
 @define
 class Pot:
-    """Class representing the pot of a table"""
-    value = field(default=0.0, validator=[ge(0), instance_of((float, int))])
-    highest_bet = field(default=0.0, validator=[ge(0), instance_of((float, int))])
+    """
+    This class represents the pot of a table
 
-    def add(self, amount):
-        """Add an amount to the pot"""
+    Attributes:
+        value (float): The value of the pot
+        highest_bet (float): The highest bet made by a player in the current round
+
+    Methods:
+        add(amount): Add an amount to the pot
+        reset(): Reset the pot
+    """
+    value = field(default=0.0, validator=[ge(0), instance_of(float, )], converter=float)
+    highest_bet = field(default=0.0, validator=[ge(0), instance_of(float)], converter=float)
+
+    def add(self, amount: float):
+        """
+        Add an amount to the pot
+
+        Args:
+            amount (float): The amount to add to the pot
+        """
         if amount < 0:
             raise ValueError("amount added to pot can only be positive")
         self.value += amount
 
-    def reset(self):
+    def reset(self) -> None:
         """Reset the pot"""
         self.value = 0
         self.highest_bet = 0
```

### Comparing `pkrcomponents-1.7.3/pkrcomponents/table.py` & `pkrcomponents-1.7.4/pkrcomponents/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from functools import cached_property
 from pkrcomponents.board import Board
-from pkrcomponents.card import Deck
+from pkrcomponents.deck import Deck
 from pkrcomponents.constants import Street
 from pkrcomponents.players import Players
 from pkrcomponents.pot import Pot
 from pkrcomponents.tournament import Level, Tournament
 from pkrcomponents.evaluator import Evaluator
 
 
@@ -82,53 +82,53 @@
 
     @property
     def is_empty(self) -> bool:
         """Returns True if the table is empty"""
         return self.players.len == 0
 
     @property
-    def pot(self):
+    def pot(self) -> Pot:
         """Returns the associated pot """
         return self._pot
 
     @property
     def tournament(self) -> Tournament or None:
         """Returns the associated tournament """
         return self._tournament
 
     @property
     def evaluator(self) -> Evaluator:
         """Returns the associated evaluator"""
         return self._evaluator
 
     @tournament.setter
-    def tournament(self, tournament):
+    def tournament(self, tournament: Tournament):
         """Setter for tournament property"""
         self._tournament = tournament
 
     @property
     def street(self) -> Street:
         """Returns table's current street"""
         return self._street
 
     @street.setter
-    def street(self, street):
+    def street(self, street: (str, Street)):
         """Setter for street property"""
         self._street = Street(street)
 
     @property
     def level(self) -> Level:
         """Returns current level"""
         if self._is_mtt:
             return self._tournament.level
         else:
             return self._level
 
     @level.setter
-    def level(self, level):
+    def level(self, level: Level):
         """Setter for level property"""
         self._level = level
 
     @property
     def playing_order(self) -> list[int]:
         """Returns the list of the indexes of players on the table, with order depending on current street"""
         if self._street == Street.PREFLOP:
```

### Comparing `pkrcomponents-1.7.3/pkrcomponents/table_player.py` & `pkrcomponents-1.7.4/pkrcomponents/table_player.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,22 +5,84 @@
 from pkrcomponents.hand import Combo
 from pkrcomponents.table import Table
 from pkrcomponents.utils.converters import convert_to_position
 
 
 @define
 class TablePlayer:
-    """Class Representing a player that sits to play poker on a table"""
+    """
+    This class represents a player on a poker table
+
+    Attributes:
+        name(str): The name of the player
+        seat(int): The seat number of the player
+        init_stack(float): The initial stack of the player at the beginning of the hand
+        stack(float): The current stack of the player
+        combo(Combo): The combo of the player
+        folded(bool): Whether the player has folded
+        hero(bool): Whether the player is the hero
+        position(Position): The position of the player
+        table(Table): The table the player is on
+        bounty(float): The bounty of the player
+        played(bool): Whether the player has played
+        is_hero(bool): Whether the player is the hero
+        current_bet(float): The current bet of the player
+        reward(int): The reward of the player
+        actions(dict): The actions of the player on each street
+
+    Methods:
+        stack_bb(): Returns the player's stack in big blinds
+        stack_to_pot_ratio(): Returns the player's stack to pot ratio
+        is_all_in(): Returns whether the player is all-in
+        m_factor(): Returns the player's M factor
+        m_factor_eff(): Returns the player's effective M factor
+        has_table(): Returns whether the player has a table
+        invested(): Returns the amount already invested by the player in the pot
+        to_call(): Returns the amount to call to continue on the table
+        to_call_bb(): Returns the amount to call to continue on the table in big blinds
+        is_current_player(): Returns whether the player is the current player
+        can_play(): Returns whether the player can still play in this hand
+        in_game(): Returns whether the player can still make actions in this hand
+        pot_odds(): Returns the pot odds
+        req_equity(): Returns the minimum required equity for an EV+ call
+        max_bet(value): Returns the real amount in a bet
+        max_reward(): Returns the maximum amount that can be won by the player
+        has_combo(): Returns whether the player has a known combo
+        hand_score(): Returns the player's current hand score on the table
+        rank_class(): Returns the player's current hand rank class on the table
+        class_str(): Returns the player's current hand rank class on the table
+        sit(table): Sits the player on a table
+        sit_out(): Removes the player from the table
+        reset_init_stack(): Resets the player's initial stack
+        distribute(combo): Distributes a combo to the player
+        shows(combo): The player shows a combo at showdown
+        delete_combo(): Deletes the player's combo
+        reset_street_status(): Resets street status
+        reset_hand_status(): Resets hand status
+        pay(value): Action of paying a value
+        do_bet(value): Action of betting a certain value
+        bet(value): Bet and step to next player
+        do_call(): Action of calling
+        call(): Call and step to next player
+        do_check(): Action of checking
+        check(): Check and step to next player
+        do_fold(): Action of folding
+        fold(): Fold and step to next player
+        post(value): Action of posting
+        win(amount): Gives the player a certain amount from the pot
+        preflop_bet_amounts(): Returns preflop bet amounts
+        postflop_bets(): Returns postflop bets
+
+    """
 
     name = field(default="Villain", validator=[instance_of(str), max_len(12), min_len(3)])
     seat = field(default=0, validator=[instance_of(int), ge(0), le(10)])
     init_stack = field(default=0, validator=[ge(0), instance_of(float)], converter=float)
     stack = field(default=Factory(lambda self: self.init_stack, takes_self=True),
                   validator=[ge(0), instance_of(float)], converter=float)
-
     combo = field(default=None, validator=optional(instance_of(Combo)), converter=Combo)
     folded = field(default=False, validator=instance_of(bool))
     hero = field(default=False, validator=instance_of(bool))
     position = field(default=None, validator=optional(instance_of(Position)), converter=convert_to_position)
     table = field(default=None, validator=optional(instance_of(Table)))
     bounty = field(default=0, validator=[ge(0), instance_of(float)], converter=float)
     played = field(default=False, validator=instance_of(bool))
@@ -31,16 +93,18 @@
         f"{Street('Preflop')}": [],
         f"{Street('Flop')}": [],
         f"{Street('Turn')}": [],
         f"{Street('River')}": []
     }, validator=instance_of(dict))
 
     @property
-    def stack_bb(self):
-        """Player's stack in big blinds"""
+    def stack_bb(self) -> float:
+        """
+        Player's stack in big blinds
+        """
         return self.stack / self.table.level.bb
 
     @property
     def stack_to_pot_ratio(self):
         """Player's stack to pot ratio"""
         return float("inf") if self.table.pot.value == 0 else self.stack / self.table.pot.value
 
@@ -56,35 +120,35 @@
 
     @property
     def m_factor_eff(self) -> float:
         """Player's effective M factor"""
         return round(self.m_factor * (self.table.players.len / 10), 2)
 
     @property
-    def has_table(self):
+    def has_table(self) -> bool:
         """Boolean indicating if player has a table"""
         return hasattr(self, "table")
 
     @property
-    def invested(self):
-        """Float indicating the amount already invested by a player in pot"""
+    def invested(self) -> float:
+        """The total amount already invested by a player in pot"""
         return self.init_stack - self.stack
 
     @property
-    def to_call(self):
-        """float indicating the amount to call to continue on the table"""
+    def to_call(self) -> float:
+        """The amount to call to continue on the table"""
         return min(self.table.pot.highest_bet - self.current_bet, self.stack)
 
     @property
     def to_call_bb(self):
-        """float indicating the amount to call to continue on the table in big blinds"""
+        """The amount to call to continue on the table in big blinds"""
         return self.to_call / self.table.level.bb
 
     @property
-    def is_current_player(self):
+    def is_current_player(self) -> bool:
         """Boolean indicating if the player is the current player"""
         if not self.can_play and self.table.current_player == self:
             self.table.advance_seat_playing()
             return False
         return self.table.current_player == self
 
     @property
@@ -103,48 +167,58 @@
         return float("inf") if self.to_call == 0 else float(self.table.pot.value / self.to_call)
 
     @property
     def req_equity(self):
         """Float indicating minimum required equity for an EV+ call"""
         return 1.0 / (1.0 + self.pot_odds)
 
-    def max_bet(self, value):
-        """Returns the real amount in a bet"""
+    def max_bet(self, value: float) -> float:
+        """
+        Returns the real amount in a bet
+
+        Args:
+            value (float): The amount to bet
+        """
         return min(self.stack, value)
 
     @property
-    def max_reward(self):
+    def max_reward(self) -> float:
         """Float indicating the maximum amount that can be won by the player"""
         return (not self.folded) * sum([min(self.invested, pl.invested) for pl in self.table.players])
 
     @property
     def has_combo(self) -> bool:
         """Boolean indicating if the player has a known combo"""
         return self.combo is not None
 
     @property
-    def hand_score(self):
+    def hand_score(self) -> int:
         """Returns player's current hand score on the table"""
         cards = (self.combo.first, self.combo.second)
         board = tuple(card for card in self.table.board[:self.table.board.len])
         score = self.table.evaluator.evaluate(cards=cards, board=board)
         return score
 
     @property
-    def rank_class(self):
+    def rank_class(self) -> int:
         """Returns player's current hand rank class on the table"""
         return self.table.evaluator.get_rank_class(self.hand_score)
 
     @property
-    def class_str(self):
+    def class_str(self) -> str:
         """Returns player's current hand rank class on the table"""
         return self.table.evaluator.score_to_string(self.hand_score)
 
-    def sit(self, table):
-        """Sits a player on a table"""
+    def sit(self, table: Table):
+        """
+        Sits a player on a table
+
+        Args:
+            table (Table): The table to sit the player on
+        """
         if table.players.len < table.max_players and table.players.seat_dict.get(self.seat) is None:
             self.table = table
             table.players.add_player(self)
             self.reset_street_status()
 
     def sit_out(self):
         """Removes player from the table"""
@@ -154,23 +228,33 @@
 
     def reset_init_stack(self):
         """Reset player's initial stack"""
         if self.stack == 0:
             self.table.remove_player(self)
         self.init_stack = self.stack
 
-    def distribute(self, combo):
-        """Distributes a combo to a player"""
+    def distribute(self, combo: (Combo, str)):
+        """
+        Distributes a combo to a player
+
+        Args:
+            combo (Combo, str): The combo to distribute
+        """
         combo = Combo(combo)
         self.table.deck.draw(combo.first)
         self.table.deck.draw(combo.second)
         self.combo = combo
 
     def shows(self, combo: (Combo, str)):
-        """The player shows a combo at showdown"""
+        """
+        The player shows a combo at showdown
+
+        Args:
+            combo (Combo, str): The combo to show
+        """
         self.combo = Combo(combo)
         if self.has_table:
             self.table.deck.draw(self.combo.first)
             self.table.deck.draw(self.combo.second)
 
     def delete_combo(self):
         """Deletes a player's combo"""
@@ -187,31 +271,46 @@
     def reset_hand_status(self):
         """Reset hand status"""
         self.reset_street_status()
         self.folded = False
         self.reset_init_stack()
         self.delete_combo()
 
-    def pay(self, value):
-        """Action of paying a value"""
+    def pay(self, value: float):
+        """
+        Action of paying a value
+
+        Args:
+            value (float): The amount to pay
+        """
         amount = self.max_bet(value)
         self.stack -= amount
         self.table.pot.add(amount)
 
-    def do_bet(self, value):
-        """Action of betting a certain value"""
+    def do_bet(self, value: float):
+        """
+        Action of betting a certain value
+
+        Args:
+            value (float): The amount to bet
+        """
         self.current_bet += self.max_bet(value)
         self.pay(value)
         if self.current_bet > self.table.pot.highest_bet:
             self.table.pot.highest_bet = self.current_bet
             self.table.cnt_bets += 1
         self.played = True
 
-    def bet(self, value):
-        """Bet and step to next player"""
+    def bet(self, value: float):
+        """
+        Bet and step to next player
+
+        Args:
+            value (float): The amount to bet
+        """
         if value >= self.table.min_bet:
             self.table.min_bet = 2*value - self.table.pot.highest_bet
             self.do_bet(value)
         elif self.table.min_bet > self.stack:
             self.bet(self.table.min_bet)
         else:
             raise ValueError(f"You cannot bet {value} if the minimum bet is {self.table.min_bet} "
@@ -245,34 +344,49 @@
         self.played = True
 
     def fold(self):
         """Fold and step to next player"""
         self.do_fold()
         self.table.advance_seat_playing()
 
-    def post(self, value):
-        """Action of posting"""
+    def post(self, value: float):
+        """
+        Action of posting
+
+        Args:
+            value (float): The amount to post
+        """
         self.pay(value)
         if value > self.table.pot.highest_bet:
             self.table.pot.highest_bet = value
 
-    def win(self, amount):
-        """gives player a certain amount from the pot"""
+    def win(self, amount: float) -> None:
+        """
+        Gives player a certain amount from the pot
+
+        Args:
+            amount (float): The amount to win
+        """
         self.table.pot.value -= amount
         self.stack += amount
 
     @property
-    def preflop_bet_amounts(self):
-        bet_amounts = [round(self.table.min_bet * factor) for factor in self.table.preflop_bet_factors]
-        bet_amounts = [amt for amt in bet_amounts if amt < self.stack]
+    def preflop_bet_amounts(self) -> list:
+        """Returns preflop bet amounts for the player"""
+        bet_amounts = [round(self.table.min_bet * factor)
+                       for factor in self.table.preflop_bet_factors
+                       if round(self.table.min_bet * factor) < self.stack]
         bet_amounts.append(self.stack)
         return bet_amounts
 
     @property
-    def postflop_bets(self):
+    def postflop_bets(self) -> list:
+        """
+        Returns postflop bets for the player
+        """
         postflop_bets = [
             {"text": factor.get("text"), "value": round(self.table.pot.value * factor.get("value"))}
             for factor in self.table.postflop_bet_factors
         ]
         postflop_bets = [bet for bet in postflop_bets
                          if self.table.min_bet < bet.get("value") < self.stack]
         postflop_bets.append({"text": "All-in", "value": self.stack})
```

### Comparing `pkrcomponents-1.7.3/pkrcomponents/tournament.py` & `pkrcomponents-1.7.4/pkrcomponents/tournament.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,42 @@
 from pkrcomponents.payout import Payouts
 from pkrcomponents.buy_in import BuyIn
 from pkrcomponents.utils.validators import validate_players_remaining
 
 
 @define
 class Tournament:
-    """Class for played tournaments"""
+    """
+    This class represents a poker tournament
+
+    Attributes:
+        id(str): The id of the tournament
+        name(str): The name of the tournament
+        buy_in(BuyIn): The buy-in of the tournament
+        is_ko(bool): Whether the tournament is a knockout tournament
+        money_type(MoneyType): The type of money used in the tournament
+        level(Level): The current level of the tournament
+        payouts(Payouts): The payouts of the tournament
+        total_players(int): The total number of players in the tournament
+        players_remaining(int): The number of players remaining in the tournament
+        starting_stack(float): The starting stack for each player in the tournament
+    """
     id = field(default='0000', validator=[instance_of(str)])
     name = field(default='Kill The Fish', validator=[instance_of(str)])
-    buyin = field(default=Factory(BuyIn), validator=[instance_of(BuyIn)])
+    buy_in = field(default=Factory(BuyIn), validator=[instance_of(BuyIn)])
     is_ko = field(default=True, validator=[instance_of(bool)])
-    money_type = field(default=MoneyType.REAL, validator=[instance_of(MoneyType)])
+    money_type = field(default=MoneyType.REAL, validator=[instance_of(MoneyType)], converter=MoneyType)
     level = field(default=Factory(Level), validator=[instance_of(Level)])
     payouts = field(default=Factory(Payouts), validator=[instance_of(Payouts)])
     total_players = field(default=2, validator=[gt(1), instance_of(int)])
     players_remaining = field(default=2, validator=validate_players_remaining)
-    starting_stack = field(default=20000.0, validator=[gt(0), instance_of((float, int))])
+    starting_stack = field(default=20000.0, validator=[gt(0), instance_of(float)], converter=float)
 
     def __str__(self):
-        return f"Name: {self.name}\nId: {self.id}\nBuy-in: {self.buyin}\nMoney: {self.money_type}"
+        return f"Name: {self.name}\nId: {self.id}\nBuy-in: {self.buy_in}\nMoney: {self.money_type}"
 
     @property
     def total_chips(self):
         return self.total_players * self.starting_stack
 
     @property
     def average_stack(self):
@@ -60,11 +74,11 @@
         return min(round(self.total_chips / average_stack), self.total_players)
 
     def to_json(self):
         return {
             "level": self.level.to_json(),
             "id": self.id,
             "name": self.name,
-            "buy_in": self.buyin.to_json(),
+            "buy_in": self.buy_in.to_json(),
             "is_ko": self.is_ko,
             "money_type": self.money_type
         }
```

### Comparing `pkrcomponents-1.7.3/pkrcomponents.egg-info/SOURCES.txt` & `pkrcomponents-1.7.4/pkrcomponents.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,30 @@
 LICENSE.txt
 MANIFEST.in
 README.md
-README.rst
 coverage.txt
 requirements.txt
 setup.py
 .pytest_cache/README.md
 pkrcomponents/__init__.py
 pkrcomponents/_common.py
 pkrcomponents/action.py
 pkrcomponents/bitcard.py
 pkrcomponents/board.py
 pkrcomponents/buy_in.py
 pkrcomponents/card.py
 pkrcomponents/constants.py
+pkrcomponents/deck.py
 pkrcomponents/evaluator.py
 pkrcomponents/hand.py
 pkrcomponents/level.py
 pkrcomponents/listings.py
 pkrcomponents/lookup_table.py
 pkrcomponents/payout.py
 pkrcomponents/players.py
 pkrcomponents/pot.py
 pkrcomponents/table.py
 pkrcomponents/table_player.py
 pkrcomponents/tournament.py
-pkrcomponents/models/amount.py
-pkrcomponents/models/actions/move.py
-pkrcomponents/models/actions/sequence.py
-pkrcomponents/models/actions/street.py
-pkrcomponents/models/cards/card.py
-pkrcomponents/models/cards/rank.py
-pkrcomponents/models/cards/suit.py
-pkrcomponents/models/pots/pot.py
 pkrcomponents/utils/__init__.py
 pkrcomponents/utils/converters.py
 pkrcomponents/utils/validators.py
```

### Comparing `pkrcomponents-1.7.3/setup.py` & `pkrcomponents-1.7.4/setup.py`

 * *Files identical despite different names*

