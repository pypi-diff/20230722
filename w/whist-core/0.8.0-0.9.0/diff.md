# Comparing `tmp/whist_core-0.8.0.tar.gz` & `tmp/whist_core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whist_core-0.8.0.tar", max compression
+gzip compressed data, was "whist_core-0.9.0.tar", max compression
```

## Comparing `whist_core-0.8.0.tar` & `whist_core-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0     1067 2022-11-26 14:15:58.631801 whist_core-0.8.0/LICENSE
--rw-r--r--   0        0        0     1359 2022-11-26 14:15:58.631801 whist_core-0.8.0/README.md
--rw-r--r--   0        0        0      855 2022-11-26 14:15:58.635801 whist_core-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      232 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/__init__.py
--rw-r--r--   0        0        0       34 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/cards/__init__.py
--rw-r--r--   0        0        0     3889 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/cards/card.py
--rw-r--r--   0        0        0     7026 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/cards/card_container.py
--rw-r--r--   0        0        0       23 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/error/__init__.py
--rw-r--r--   0        0        0      182 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/error/matcher_error.py
--rw-r--r--   0        0        0      179 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/error/player_error.py
--rw-r--r--   0        0        0      734 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/error/table_error.py
--rw-r--r--   0        0        0       22 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/game/__init__.py
--rw-r--r--   0        0        0     1432 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/game/errors.py
--rw-r--r--   0        0        0     2371 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/game/game.py
--rw-r--r--   0        0        0     2510 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/game/hand.py
--rw-r--r--   0        0        0      888 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/game/legal_checker.py
--rw-r--r--   0        0        0     3585 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/game/play_order.py
--rw-r--r--   0        0        0      649 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/game/player_at_table.py
--rw-r--r--   0        0        0     1584 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/game/rubber.py
--rw-r--r--   0        0        0     2608 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/game/trick.py
--rw-r--r--   0        0        0      205 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/game/warnings.py
--rw-r--r--   0        0        0       41 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/scoring/__init__.py
--rw-r--r--   0        0        0     1734 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/scoring/elo.py
--rw-r--r--   0        0        0     1228 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/scoring/score.py
--rw-r--r--   0        0        0     1330 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/scoring/score_calculator.py
--rw-r--r--   0        0        0     2168 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/scoring/score_card.py
--rw-r--r--   0        0        0      910 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/scoring/team.py
--rw-r--r--   0        0        0       42 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/session/__init__.py
--rw-r--r--   0        0        0      951 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/session/distribution.py
--rw-r--r--   0        0        0     3628 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/session/matcher.py
--rw-r--r--   0        0        0      240 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/session/session.py
--rw-r--r--   0        0        0     5399 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/session/table.py
--rw-r--r--   0        0        0     5322 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/session/userlist.py
--rw-r--r--   0        0        0       37 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/user/__init__.py
--rw-r--r--   0        0        0     1669 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/user/player.py
--rw-r--r--   0        0        0      242 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/user/status.py
--rw-r--r--   0        0        0      156 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/user/user.py
--rw-r--r--   0        0        0      564 2022-11-26 14:15:58.635801 whist_core-0.8.0/whist_core/util.py
--rw-r--r--   0        0        0     2169 1970-01-01 00:00:00.000000 whist_core-0.8.0/setup.py
--rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 whist_core-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-21 22:47:28.479875 whist_core-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1359 2023-07-21 22:47:28.479875 whist_core-0.9.0/README.md
+-rw-r--r--   0        0        0      884 2023-07-21 22:47:28.479875 whist_core-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      232 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/__init__.py
+-rw-r--r--   0        0        0       34 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/cards/__init__.py
+-rw-r--r--   0        0        0     3720 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/cards/card.py
+-rw-r--r--   0        0        0     6837 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/cards/card_container.py
+-rw-r--r--   0        0        0       23 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/error/__init__.py
+-rw-r--r--   0        0        0      182 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/error/matcher_error.py
+-rw-r--r--   0        0        0      179 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/error/player_error.py
+-rw-r--r--   0        0        0      734 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/error/table_error.py
+-rw-r--r--   0        0        0       22 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/__init__.py
+-rw-r--r--   0        0        0     1432 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/errors.py
+-rw-r--r--   0        0        0     2187 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/game.py
+-rw-r--r--   0        0        0     3428 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/hand.py
+-rw-r--r--   0        0        0      888 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/legal_checker.py
+-rw-r--r--   0        0        0     3585 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/play_order.py
+-rw-r--r--   0        0        0      649 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/player_at_table.py
+-rw-r--r--   0        0        0     1397 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/rubber.py
+-rw-r--r--   0        0        0     2608 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/trick.py
+-rw-r--r--   0        0        0      205 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/game/warnings.py
+-rw-r--r--   0        0        0       41 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/scoring/__init__.py
+-rw-r--r--   0        0        0     1734 2023-07-21 22:47:28.479875 whist_core-0.9.0/whist_core/scoring/elo.py
+-rw-r--r--   0        0        0     1228 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/scoring/score.py
+-rw-r--r--   0        0        0     1330 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/scoring/score_calculator.py
+-rw-r--r--   0        0        0     2168 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/scoring/score_card.py
+-rw-r--r--   0        0        0      910 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/scoring/team.py
+-rw-r--r--   0        0        0       42 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/session/__init__.py
+-rw-r--r--   0        0        0      951 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/session/distribution.py
+-rw-r--r--   0        0        0     3534 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/session/matcher.py
+-rw-r--r--   0        0        0      240 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/session/session.py
+-rw-r--r--   0        0        0     6577 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/session/table.py
+-rw-r--r--   0        0        0     5322 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/session/userlist.py
+-rw-r--r--   0        0        0       37 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/user/__init__.py
+-rw-r--r--   0        0        0     1698 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/user/player.py
+-rw-r--r--   0        0        0      280 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/user/status.py
+-rw-r--r--   0        0        0      156 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/user/user.py
+-rw-r--r--   0        0        0      564 2023-07-21 22:47:28.483875 whist_core-0.9.0/whist_core/util.py
+-rw-r--r--   0        0        0     2206 1970-01-01 00:00:00.000000 whist_core-0.9.0/PKG-INFO
```

### Comparing `whist_core-0.8.0/LICENSE` & `whist_core-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/README.md` & `whist_core-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/pyproject.toml` & `whist_core-0.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "whist-core"
 # remember to also update the version in __init__.py!
-version = "0.8.0"
+version = "0.9.0"
 description = "Whist rules implementation"
 authors = ["Whist-Team"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Whist-Team/Whist-Core"
 repository = "https://github.com/Whist-Team/Whist-Core"
 documentation = "https://whist-core.readthedocs.io"
@@ -15,20 +15,21 @@
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Whist-Team/Whist-Core/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = "^1.10"
+pydantic = ">=1.10,<3.0"
+deprecation = "^2.1.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2"
-pytest-cov = "^4.0"
-pytest-asyncio = "^0.20"
+pytest = "^7.4"
+pytest-cov = "^4.1"
+pytest-asyncio = "^0.21"
 flake8 = "^6.0"
-flake8-docstrings = "^1.6"
-pylint = "^2.15"
+flake8-docstrings = "^1.7"
+pylint = "^2.17"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `whist_core-0.8.0/whist_core/cards/card.py` & `whist_core-0.9.0/whist_core/cards/card.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,27 +95,20 @@
     J = ('jack', 'J')
     Q = ('queen', 'Q')
     K = ('king', 'K')
     A = ('ace', 'A')
 
 
 @total_ordering
-class Card(BaseModel):
+class Card(BaseModel, frozen=True):
     """A playing card"""
 
     suit: Suit
     rank: Rank
 
-    # pylint: disable=too-few-public-methods
-    class Config:
-        """
-        Configuration class for base model to make it immutable and hashable.
-        """
-        frozen = True
-
     @staticmethod
     def all_cards() -> Iterator['Card']:
         """
         Get iterator of all cards.
 
         :return: all cards
         """
@@ -142,15 +135,15 @@
         """
         return f'{self.rank} of {self.suit}'
 
     def dict(self, *args, **kwargs):
         """
         Returns the dictionary. See BaseModel for details.
         """
-        super_dict = super().dict(*args, **kwargs)
+        super_dict = super().model_dump(*args, **kwargs)
         return enforce_str_on_dict(super_dict, ('suit', 'rank'))
 
     def __lt__(self, other: Any) -> bool:
         """Checks if the other card is lower than this card."""
         if self.__class__ is other.__class__:
             return (self.suit, self.rank) < (other.suit, other.rank)
         return NotImplemented
```

### Comparing `whist_core-0.8.0/whist_core/cards/card_container.py` & `whist_core-0.9.0/whist_core/cards/card_container.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,28 +4,21 @@
 from typing import Iterator, Optional
 
 from pydantic import BaseModel, PrivateAttr
 
 from whist_core.cards.card import Card, Suit
 
 
-class CardContainer(BaseModel, abc.ABC):
+class CardContainer(BaseModel, abc.ABC, frozen=True):
     """
     Abstract Base Class for card containers. Duplicate cards are not allowed.
     """
 
     cards: tuple[Card, ...]
 
-    # pylint: disable=too-few-public-methods
-    class Config:
-        """
-        Configuration class for base model to make it immutable.
-        """
-        allow_mutation = False
-
     @classmethod
     def empty(cls) -> 'CardContainer':
         """
         Creates an empty card container.
 
         :return: empty ard container
         :rtype: correct subtype of CardContainer
@@ -164,36 +157,36 @@
         self._cards_set.add(card)
         self.__resync()
 
     def __resync(self) -> None:
         """
         de-duplicate and re-sort self.cards - i.e. synchronize with the set representation
         """
-        self.__config__.allow_mutation = True
+        self.model_config['frozen'] = False
         self.cards = tuple(sorted(self._cards_set))
-        self.__config__.allow_mutation = False
+        self.model_config['frozen'] = True
 
 
 class OrderedCardContainer(CardContainer):
     """
     Base Class ordered card containers
     """
 
     def _remove_impl(self, card: Card) -> None:
         card_list = list(self.cards)
         card_list.remove(card)
 
-        self.__config__.allow_mutation = True
+        self.model_config['frozen'] = False
         self.cards = tuple(card_list)
-        self.__config__.allow_mutation = False
+        self.model_config['frozen'] = True
 
     def _add_impl(self, card: Card) -> None:
-        self.__config__.allow_mutation = True
+        self.model_config['frozen'] = False
         self.cards = (*self.cards, card)
-        self.__config__.allow_mutation = False
+        self.model_config['frozen'] = True
 
     @property
     def first(self) -> Optional[Card]:
         """
         Returns the first card in the card container.
         :return: The first card played if it exists. Else None.
         """
```

### Comparing `whist_core-0.8.0/whist_core/error/table_error.py` & `whist_core-0.9.0/whist_core/error/table_error.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/whist_core/game/errors.py` & `whist_core-0.9.0/whist_core/game/errors.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/whist_core/game/game.py` & `whist_core-0.9.0/whist_core/game/game.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,31 +7,24 @@
 from whist_core.game.play_order import PlayOrder
 from whist_core.game.player_at_table import PlayerAtTable
 from whist_core.scoring.score_calculator import ScoreCalculator
 from whist_core.scoring.score_card import ScoreCard
 from whist_core.user.player import Player
 
 
-class Game(BaseModel):
+class Game(BaseModel, arbitrary_types_allowed=True):
     """
     One Game of whist.
     """
 
     play_order: PlayOrder
     win_score: int = 3
     score_card: ScoreCard = ScoreCard()
     hands: list[Hand] = []
 
-    # pylint: disable=too-few-public-methods
-    class Config:
-        """
-        Enables to have non models as field types and sets the encoder for play order.
-        """
-        arbitrary_types_allowed = True
-
     def next_hand(self) -> Hand:
         """
         Checks if the current hand is done and if so will return the next hand. If not it will
         return the current hand.
         :rtype: Hand
         """
         if self.current_hand is None:
```

### Comparing `whist_core-0.8.0/whist_core/game/hand.py` & `whist_core-0.9.0/whist_core/game/hand.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Hand of whist"""
-from typing import Optional
+from typing import Optional, Any, Dict
 
+import deprecation
 from pydantic import BaseModel
 
 from whist_core.cards.card import Card, Suit
-from whist_core.cards.card_container import UnorderedCardContainer
+from whist_core.cards.card_container import UnorderedCardContainer, OrderedCardContainer
 from whist_core.game.errors import HandDoneError
 from whist_core.game.play_order import PlayOrder
 from whist_core.game.player_at_table import PlayerAtTable
 from whist_core.game.trick import Trick
 from whist_core.game.warnings import TrickNotDoneWarning
 from whist_core.util import enforce_str_on_dict
 
@@ -46,15 +47,16 @@
         card: Optional[Card] = None
         while deck:
             player = play_order.get_next_player()
             card = deck.pop_random()
             player.hand.add(card)
         trump = card.suit
 
-        first_trick = Trick(play_order=list(play_order), trump=trump)
+        first_trick = Trick(play_order=list(play_order), stack=OrderedCardContainer.empty(),
+                            trump=trump)
         hand = Hand(tricks=[first_trick], trump=trump)
         return hand
 
     def next_trick(self, play_order: PlayOrder) -> Trick:
         """
         Starts the next trick.
         :return: the next trick
@@ -68,15 +70,27 @@
             next_trick_order = self._winner_plays_first_card(play_order)
         else:
             raise TrickNotDoneWarning()
         next_trick = Trick(play_order=list(next_trick_order), trump=self.trump)
         self.tricks.append(next_trick)
         return next_trick
 
+    @deprecation.deprecated("Use 'model_dump()' instead")
     def dict(self, *args, **kwargs):
         """Returns as dictionary."""
         super_dict = super().dict(*args, **kwargs)
         return enforce_str_on_dict(super_dict, ['trump'])
 
+    def model_dump(self, *, mode: str = 'python', include=None,
+                   exclude=None, by_alias: bool = False, exclude_unset: bool = False,
+                   exclude_defaults: bool = False, exclude_none: bool = False,
+                   round_trip: bool = False, warnings: bool = True) -> Dict[str, Any]:
+        """Returns as dictionary."""
+        model = super().model_dump(mode=mode, include=include, exclude=exclude, by_alias=by_alias,
+                                   exclude_unset=exclude_unset, exclude_defaults=exclude_defaults,
+                                   exclude_none=exclude_none, round_trip=round_trip,
+                                   warnings=warnings)
+        return enforce_str_on_dict(model, ['trump'])
+
     def _winner_plays_first_card(self, play_order: PlayOrder) -> PlayOrder:
         winner: PlayerAtTable = self.tricks[-1].winner
         return play_order.rotate(winner)
```

### Comparing `whist_core-0.8.0/whist_core/game/legal_checker.py` & `whist_core-0.9.0/whist_core/game/legal_checker.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/whist_core/game/play_order.py` & `whist_core-0.9.0/whist_core/game/play_order.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/whist_core/game/player_at_table.py` & `whist_core-0.9.0/whist_core/game/player_at_table.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/whist_core/game/trick.py` & `whist_core-0.9.0/whist_core/game/trick.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/whist_core/scoring/elo.py` & `whist_core-0.9.0/whist_core/scoring/elo.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/whist_core/scoring/score.py` & `whist_core-0.9.0/whist_core/scoring/score.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/whist_core/scoring/score_calculator.py` & `whist_core-0.9.0/whist_core/scoring/score_calculator.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/whist_core/scoring/score_card.py` & `whist_core-0.9.0/whist_core/scoring/score_card.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/whist_core/scoring/team.py` & `whist_core-0.9.0/whist_core/scoring/team.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/whist_core/session/distribution.py` & `whist_core-0.9.0/whist_core/session/distribution.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/whist_core/session/matcher.py` & `whist_core-0.9.0/whist_core/session/matcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from whist_core.session.distribution import Distribution, DistributionEntry
 from whist_core.session.userlist import UserList
 
 subclass_registry = {}
 
 
 # pylint: disable=too-few-public-methods
-class Matcher(abc.ABC, BaseModel):
+class Matcher(abc.ABC, BaseModel, extra='allow'):
     """
     Abstrakt class for player to teams matching.
     """
     teams: list[Distribution] = []
     number_teams: int
 
     def __init_subclass__(cls, **kwargs: Any) -> None:
@@ -27,20 +27,14 @@
         Initializes the subclass
         :param kwargs: field from above
         :return: None
         """
         super().__init_subclass__(**kwargs)
         subclass_registry[cls.__name__] = cls
 
-    class Config:
-        """
-        Configuration of matcher classes.
-        """
-        extra = "allow"
-
     @abc.abstractmethod
     def distribute(self, users: UserList) -> Distribution:
         """
         Distributes cards according to subclass implementation.
         :param users: the players to be distributed to teams
         :return: the list of teams with players distributed to them
         """
```

### Comparing `whist_core-0.8.0/whist_core/session/table.py` & `whist_core-0.9.0/whist_core/session/table.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """DAO of session."""
-from typing import Any
+from typing import Any, Union
 
-from pydantic import root_validator
+from pydantic import model_validator
+from typing_extensions import Literal
 
 from whist_core.error.table_error import TableFullError, TeamFullError, TableNotReadyError, \
     TableNotStartedError, TableSettingsError
 from whist_core.game.errors import RubberNotDoneError
 from whist_core.game.rubber import Rubber
 from whist_core.session.matcher import Matcher, subclass_registry
 from whist_core.session.session import Session
@@ -37,16 +38,41 @@
                 matcher_keys = sorted(subclass.__fields__.keys())
                 if item_matcher_keys == matcher_keys:
                     matcher = subclass(**matcher)
                     break
             data['matcher'] = matcher
         super().__init__(**data)
 
+    def model_dump(self, *, mode: Union[Literal['json', 'python'], str] = 'python', include=None,
+                   exclude=None, by_alias: bool = False, exclude_unset: bool = False,
+                   exclude_defaults: bool = False, exclude_none: bool = False,
+                   round_trip: bool = False, warnings: bool = True) -> dict[str, Any]:
+        """
+        Overrides model_dump to ensure matcher is correctly dumped.
+        :param mode:
+        :param include:
+        :param exclude:
+        :param by_alias:
+        :param exclude_unset:
+        :param exclude_defaults:
+        :param exclude_none:
+        :param round_trip:
+        :param warnings:
+        :return:
+        """
+        model = super().model_dump(mode=mode, include=include, exclude=exclude, by_alias=by_alias,
+                                   exclude_unset=exclude_unset, exclude_defaults=exclude_defaults,
+                                   exclude_none=exclude_none, round_trip=round_trip,
+                                   warnings=warnings)
+        model['matcher'] = self.matcher.model_dump()
+        return model
+
     # pylint: disable=no-self-argument
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def validate_min_is_lower_max_player(cls, values):
         """
         Checks if the min_player is less or equal than max_player.
         :param values:
         :return:
         """
         if values.get('min_player') > values.get('max_player'):
```

### Comparing `whist_core-0.8.0/whist_core/session/userlist.py` & `whist_core-0.9.0/whist_core/session/userlist.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/whist_core/user/player.py` & `whist_core-0.9.0/whist_core/user/player.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """DAO of user."""
 from typing import Optional
 
-from pydantic import validator
+from pydantic import field_validator
 
 from whist_core.error.player_error import NegativeRatingError
 from whist_core.user.user import User
 
 
 class Player(User):
     """
@@ -25,15 +25,16 @@
     def __eq__(self, other):
         """Checks if the other is the same player."""
         if not isinstance(other, Player):
             return False
         return other.username == self.username
 
     # Pydantic will convert this into a classmethod, cls is the correct parameter
-    @validator('rating')
+    @field_validator('rating')
+    @classmethod
     # noinspection ImproperFirstParameter
     def rating_must_not_be_negative(cls, value):  # pylint: disable=no-self-argument
         """
         Validates the rating. It must be zero or positive.
         """
         if value < 0:
             raise NegativeRatingError()
```

### Comparing `whist_core-0.8.0/whist_core/util.py` & `whist_core-0.9.0/whist_core/util.py`

 * *Files identical despite different names*

### Comparing `whist_core-0.8.0/PKG-INFO` & `whist_core-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: whist-core
-Version: 0.8.0
+Version: 0.9.0
 Summary: Whist rules implementation
 Home-page: https://github.com/Whist-Team/Whist-Core
 License: MIT
 Keywords: game,whist
 Author: Whist-Team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.10,<2.0)
+Requires-Dist: deprecation (>=2.1.0,<3.0.0)
+Requires-Dist: pydantic (>=1.10,<3.0)
 Project-URL: Bug Tracker, https://github.com/Whist-Team/Whist-Core/issues
 Project-URL: Documentation, https://whist-core.readthedocs.io
 Project-URL: Repository, https://github.com/Whist-Team/Whist-Core
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/pip/badge/?version=stable)](https://whist-core.readthedocs.io/en/latest/)
 [![codecov](https://codecov.io/gh/Whist-Team/Whist-Core/branch/main/graph/badge.svg)](https://codecov.io/gh/Whist-Team/Whist-Core)
```

