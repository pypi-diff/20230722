# Comparing `tmp/pied_poker-1.0.8.tar.gz` & `tmp/pied_poker-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pied_poker-1.0.8.tar", last modified: Tue Jan 10 08:19:11 2023, max compression
+gzip compressed data, was "pied_poker-1.0.9.tar", last modified: Wed Jan 11 01:43:23 2023, max compression
```

## Comparing `pied_poker-1.0.8.tar` & `pied_poker-1.0.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-10 08:19:11.283031 pied_poker-1.0.8/
--rw-r--r--   0 ellek      (501) staff       (20)      737 2023-01-10 08:19:11.282644 pied_poker-1.0.8/PKG-INFO
--rw-r--r--   0 ellek      (501) staff       (20)      166 2022-03-21 04:52:37.000000 pied_poker-1.0.8/README.md
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-10 08:19:11.250585 pied_poker-1.0.8/pied_poker/
--rw-r--r--   0 ellek      (501) staff       (20)     2332 2023-01-10 06:49:49.000000 pied_poker-1.0.8/pied_poker/__init__.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-10 08:19:11.254856 pied_poker-1.0.8/pied_poker/card/
--rw-r--r--   0 ellek      (501) staff       (20)      164 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/card/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     1673 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/card/card.py
--rw-r--r--   0 ellek      (501) staff       (20)      379 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/card/comparable.py
--rw-r--r--   0 ellek      (501) staff       (20)     2075 2023-01-09 01:24:35.000000 pied_poker-1.0.8/pied_poker/card/rank.py
--rw-r--r--   0 ellek      (501) staff       (20)      824 2023-01-08 20:45:48.000000 pied_poker-1.0.8/pied_poker/card/suit.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-10 08:19:11.255703 pied_poker-1.0.8/pied_poker/deck/
--rw-r--r--   0 ellek      (501) staff       (20)       38 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/deck/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     1976 2023-01-08 08:59:27.000000 pied_poker-1.0.8/pied_poker/deck/deck.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-10 08:19:11.261793 pied_poker-1.0.8/pied_poker/hand/
--rw-r--r--   0 ellek      (501) staff       (20)      589 2023-01-10 06:49:35.000000 pied_poker-1.0.8/pied_poker/hand/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     7980 2023-01-10 08:09:33.000000 pied_poker-1.0.8/pied_poker/hand/base_hand.py
--rw-r--r--   0 ellek      (501) staff       (20)     2953 2023-01-10 08:00:34.000000 pied_poker-1.0.8/pied_poker/hand/flush.py
--rw-r--r--   0 ellek      (501) staff       (20)     2567 2023-01-10 07:31:28.000000 pied_poker-1.0.8/pied_poker/hand/four_of_a_kind.py
--rw-r--r--   0 ellek      (501) staff       (20)     3284 2023-01-10 07:31:33.000000 pied_poker-1.0.8/pied_poker/hand/full_house.py
--rw-r--r--   0 ellek      (501) staff       (20)     2641 2023-01-10 07:31:38.000000 pied_poker-1.0.8/pied_poker/hand/high_card.py
--rw-r--r--   0 ellek      (501) staff       (20)     2913 2023-01-10 07:31:44.000000 pied_poker-1.0.8/pied_poker/hand/one_pair.py
--rw-r--r--   0 ellek      (501) staff       (20)     3318 2023-01-10 06:50:18.000000 pied_poker-1.0.8/pied_poker/hand/poker_hand.py
--rw-r--r--   0 ellek      (501) staff       (20)     1953 2023-01-10 08:17:04.000000 pied_poker-1.0.8/pied_poker/hand/royal_flush.py
--rw-r--r--   0 ellek      (501) staff       (20)     2099 2023-01-10 07:31:59.000000 pied_poker-1.0.8/pied_poker/hand/straight.py
--rw-r--r--   0 ellek      (501) staff       (20)     2012 2023-01-10 08:11:25.000000 pied_poker-1.0.8/pied_poker/hand/straight_flush.py
--rw-r--r--   0 ellek      (501) staff       (20)     2853 2023-01-10 07:32:10.000000 pied_poker-1.0.8/pied_poker/hand/three_of_a_kind.py
--rw-r--r--   0 ellek      (501) staff       (20)     3493 2023-01-10 07:32:15.000000 pied_poker-1.0.8/pied_poker/hand/two_pair.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-10 08:19:11.262669 pied_poker-1.0.8/pied_poker/player/
--rw-r--r--   0 ellek      (501) staff       (20)       44 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/player/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)      845 2023-01-10 05:38:07.000000 pied_poker-1.0.8/pied_poker/player/player.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-10 08:19:11.265636 pied_poker-1.0.8/pied_poker/poker_round/
--rw-r--r--   0 ellek      (501) staff       (20)      297 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/poker_round/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     3735 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/poker_round/poker_round.py
--rw-r--r--   0 ellek      (501) staff       (20)     1757 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/poker_round/poker_round_result.py
--rw-r--r--   0 ellek      (501) staff       (20)     6794 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/poker_round/poker_round_simulation_result.py
--rw-r--r--   0 ellek      (501) staff       (20)     3771 2023-01-01 00:18:26.000000 pied_poker-1.0.8/pied_poker/poker_round/poker_round_simulator.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-10 08:19:11.267258 pied_poker-1.0.8/pied_poker/probability/
--rw-r--r--   0 ellek      (501) staff       (20)      886 2023-01-01 00:48:00.000000 pied_poker-1.0.8/pied_poker/probability/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     1053 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/probability/base_poker_event.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-10 08:19:11.274797 pied_poker-1.0.8/pied_poker/probability/events/
--rw-r--r--   0 ellek      (501) staff       (20)      980 2023-01-01 00:47:51.000000 pied_poker-1.0.8/pied_poker/probability/events/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)      861 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/probability/events/community_cards_include.py
--rw-r--r--   0 ellek      (501) staff       (20)      770 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/probability/events/no_tie.py
--rw-r--r--   0 ellek      (501) staff       (20)     1211 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/probability/events/player_has_card_ranks.py
--rw-r--r--   0 ellek      (501) staff       (20)     1211 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/probability/events/player_has_card_suits.py
--rw-r--r--   0 ellek      (501) staff       (20)     1181 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/probability/events/player_has_cards.py
--rw-r--r--   0 ellek      (501) staff       (20)     1611 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/probability/events/player_has_hand.py
--rw-r--r--   0 ellek      (501) staff       (20)     1224 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/probability/events/player_has_hand_or_higher.py
--rw-r--r--   0 ellek      (501) staff       (20)     2218 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/probability/events/player_has_pocket_pair.py
--rw-r--r--   0 ellek      (501) staff       (20)     1520 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/probability/events/player_has_suited_cards.py
--rw-r--r--   0 ellek      (501) staff       (20)      792 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/probability/events/player_loses.py
--rw-r--r--   0 ellek      (501) staff       (20)     1275 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/probability/events/player_wins.py
--rw-r--r--   0 ellek      (501) staff       (20)      959 2023-01-01 00:52:22.000000 pied_poker-1.0.8/pied_poker/probability/events/player_wins_with_tie.py
--rw-r--r--   0 ellek      (501) staff       (20)      767 2023-01-01 00:43:13.000000 pied_poker-1.0.8/pied_poker/probability/events/tie.py
--rw-r--r--   0 ellek      (501) staff       (20)      871 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/probability/probability_value.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-10 08:19:11.275649 pied_poker-1.0.8/pied_poker/visualization/
--rw-r--r--   0 ellek      (501) staff       (20)      415 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/visualization/__init__.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-10 08:19:11.280480 pied_poker-1.0.8/pied_poker/visualization/heatmap/
--rw-r--r--   0 ellek      (501) staff       (20)      336 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/visualization/heatmap/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     1989 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/visualization/heatmap/categorical_heat_map.py
--rw-r--r--   0 ellek      (501) staff       (20)      691 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/visualization/heatmap/heatmap_dimension.py
--rw-r--r--   0 ellek      (501) staff       (20)      365 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/visualization/heatmap/heatmap_dimension_value.py
--rw-r--r--   0 ellek      (501) staff       (20)     1588 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/visualization/heatmap/heatmap_generator.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-10 08:19:11.282003 pied_poker-1.0.8/pied_poker/visualization/heatmap_samples/
--rw-r--r--   0 ellek      (501) staff       (20)      212 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/visualization/heatmap_samples/__init__.py
--rw-r--r--   0 ellek      (501) staff       (20)     1661 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/visualization/heatmap_samples/all_suited_starting_hands.py
--rw-r--r--   0 ellek      (501) staff       (20)     1538 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/visualization/heatmap_samples/pocket_pair_vs_num_players.py
--rw-r--r--   0 ellek      (501) staff       (20)     1960 2022-03-21 04:52:37.000000 pied_poker-1.0.8/pied_poker/visualization/pocket_pair_map.py
-drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-10 08:19:11.252696 pied_poker-1.0.8/pied_poker.egg-info/
--rw-r--r--   0 ellek      (501) staff       (20)      737 2023-01-10 08:19:11.000000 pied_poker-1.0.8/pied_poker.egg-info/PKG-INFO
--rw-r--r--   0 ellek      (501) staff       (20)     2430 2023-01-10 08:19:11.000000 pied_poker-1.0.8/pied_poker.egg-info/SOURCES.txt
--rw-r--r--   0 ellek      (501) staff       (20)        1 2023-01-10 08:19:11.000000 pied_poker-1.0.8/pied_poker.egg-info/dependency_links.txt
--rw-r--r--   0 ellek      (501) staff       (20)       33 2023-01-10 08:19:11.000000 pied_poker-1.0.8/pied_poker.egg-info/requires.txt
--rw-r--r--   0 ellek      (501) staff       (20)       11 2023-01-10 08:19:11.000000 pied_poker-1.0.8/pied_poker.egg-info/top_level.txt
--rw-r--r--   0 ellek      (501) staff       (20)       38 2023-01-10 08:19:11.283178 pied_poker-1.0.8/setup.cfg
--rw-r--r--   0 ellek      (501) staff       (20)     1359 2023-01-10 08:18:58.000000 pied_poker-1.0.8/setup.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-11 01:43:23.804989 pied_poker-1.0.9/
+-rw-r--r--   0 ellek      (501) staff       (20)      737 2023-01-11 01:43:23.804582 pied_poker-1.0.9/PKG-INFO
+-rw-r--r--   0 ellek      (501) staff       (20)      166 2022-03-21 04:52:37.000000 pied_poker-1.0.9/README.md
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-11 01:43:23.770685 pied_poker-1.0.9/pied_poker/
+-rw-r--r--   0 ellek      (501) staff       (20)     2332 2023-01-10 06:49:49.000000 pied_poker-1.0.9/pied_poker/__init__.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-11 01:43:23.775195 pied_poker-1.0.9/pied_poker/card/
+-rw-r--r--   0 ellek      (501) staff       (20)      164 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/card/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1673 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/card/card.py
+-rw-r--r--   0 ellek      (501) staff       (20)      379 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/card/comparable.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2075 2023-01-09 01:24:35.000000 pied_poker-1.0.9/pied_poker/card/rank.py
+-rw-r--r--   0 ellek      (501) staff       (20)      824 2023-01-08 20:45:48.000000 pied_poker-1.0.9/pied_poker/card/suit.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-11 01:43:23.776189 pied_poker-1.0.9/pied_poker/deck/
+-rw-r--r--   0 ellek      (501) staff       (20)       38 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/deck/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1976 2023-01-08 08:59:27.000000 pied_poker-1.0.9/pied_poker/deck/deck.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-11 01:43:23.784323 pied_poker-1.0.9/pied_poker/hand/
+-rw-r--r--   0 ellek      (501) staff       (20)      589 2023-01-10 06:49:35.000000 pied_poker-1.0.9/pied_poker/hand/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     7980 2023-01-10 08:27:16.000000 pied_poker-1.0.9/pied_poker/hand/base_hand.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2953 2023-01-10 08:00:34.000000 pied_poker-1.0.9/pied_poker/hand/flush.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2567 2023-01-10 07:31:28.000000 pied_poker-1.0.9/pied_poker/hand/four_of_a_kind.py
+-rw-r--r--   0 ellek      (501) staff       (20)     3284 2023-01-10 07:31:33.000000 pied_poker-1.0.9/pied_poker/hand/full_house.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2641 2023-01-10 07:31:38.000000 pied_poker-1.0.9/pied_poker/hand/high_card.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2913 2023-01-10 07:31:44.000000 pied_poker-1.0.9/pied_poker/hand/one_pair.py
+-rw-r--r--   0 ellek      (501) staff       (20)     3318 2023-01-10 06:50:18.000000 pied_poker-1.0.9/pied_poker/hand/poker_hand.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1953 2023-01-10 08:17:04.000000 pied_poker-1.0.9/pied_poker/hand/royal_flush.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2099 2023-01-10 07:31:59.000000 pied_poker-1.0.9/pied_poker/hand/straight.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2012 2023-01-10 08:11:25.000000 pied_poker-1.0.9/pied_poker/hand/straight_flush.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2853 2023-01-10 07:32:10.000000 pied_poker-1.0.9/pied_poker/hand/three_of_a_kind.py
+-rw-r--r--   0 ellek      (501) staff       (20)     3493 2023-01-10 07:32:15.000000 pied_poker-1.0.9/pied_poker/hand/two_pair.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-11 01:43:23.785487 pied_poker-1.0.9/pied_poker/player/
+-rw-r--r--   0 ellek      (501) staff       (20)       44 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/player/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)      845 2023-01-10 05:38:07.000000 pied_poker-1.0.9/pied_poker/player/player.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-11 01:43:23.788193 pied_poker-1.0.9/pied_poker/poker_round/
+-rw-r--r--   0 ellek      (501) staff       (20)      297 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/poker_round/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     3735 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/poker_round/poker_round.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1757 2023-01-11 01:24:11.000000 pied_poker-1.0.9/pied_poker/poker_round/poker_round_result.py
+-rw-r--r--   0 ellek      (501) staff       (20)     6794 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/poker_round/poker_round_simulation_result.py
+-rw-r--r--   0 ellek      (501) staff       (20)     4887 2023-01-11 01:42:09.000000 pied_poker-1.0.9/pied_poker/poker_round/poker_round_simulator.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-11 01:43:23.789789 pied_poker-1.0.9/pied_poker/probability/
+-rw-r--r--   0 ellek      (501) staff       (20)      886 2023-01-01 00:48:00.000000 pied_poker-1.0.9/pied_poker/probability/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1053 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/probability/base_poker_event.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-11 01:43:23.796614 pied_poker-1.0.9/pied_poker/probability/events/
+-rw-r--r--   0 ellek      (501) staff       (20)      980 2023-01-01 00:47:51.000000 pied_poker-1.0.9/pied_poker/probability/events/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)      861 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/probability/events/community_cards_include.py
+-rw-r--r--   0 ellek      (501) staff       (20)      770 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/probability/events/no_tie.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1211 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/probability/events/player_has_card_ranks.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1211 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/probability/events/player_has_card_suits.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1181 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/probability/events/player_has_cards.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1611 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/probability/events/player_has_hand.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1224 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/probability/events/player_has_hand_or_higher.py
+-rw-r--r--   0 ellek      (501) staff       (20)     2218 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/probability/events/player_has_pocket_pair.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1520 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/probability/events/player_has_suited_cards.py
+-rw-r--r--   0 ellek      (501) staff       (20)      792 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/probability/events/player_loses.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1275 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/probability/events/player_wins.py
+-rw-r--r--   0 ellek      (501) staff       (20)      959 2023-01-01 00:52:22.000000 pied_poker-1.0.9/pied_poker/probability/events/player_wins_with_tie.py
+-rw-r--r--   0 ellek      (501) staff       (20)      767 2023-01-01 00:43:13.000000 pied_poker-1.0.9/pied_poker/probability/events/tie.py
+-rw-r--r--   0 ellek      (501) staff       (20)      871 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/probability/probability_value.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-11 01:43:23.798366 pied_poker-1.0.9/pied_poker/visualization/
+-rw-r--r--   0 ellek      (501) staff       (20)      415 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/visualization/__init__.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-11 01:43:23.801918 pied_poker-1.0.9/pied_poker/visualization/heatmap/
+-rw-r--r--   0 ellek      (501) staff       (20)      336 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/visualization/heatmap/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1989 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/visualization/heatmap/categorical_heat_map.py
+-rw-r--r--   0 ellek      (501) staff       (20)      691 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/visualization/heatmap/heatmap_dimension.py
+-rw-r--r--   0 ellek      (501) staff       (20)      365 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/visualization/heatmap/heatmap_dimension_value.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1588 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/visualization/heatmap/heatmap_generator.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-11 01:43:23.803741 pied_poker-1.0.9/pied_poker/visualization/heatmap_samples/
+-rw-r--r--   0 ellek      (501) staff       (20)      212 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/visualization/heatmap_samples/__init__.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1661 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/visualization/heatmap_samples/all_suited_starting_hands.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1538 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/visualization/heatmap_samples/pocket_pair_vs_num_players.py
+-rw-r--r--   0 ellek      (501) staff       (20)     1960 2022-03-21 04:52:37.000000 pied_poker-1.0.9/pied_poker/visualization/pocket_pair_map.py
+drwxr-xr-x   0 ellek      (501) staff       (20)        0 2023-01-11 01:43:23.772567 pied_poker-1.0.9/pied_poker.egg-info/
+-rw-r--r--   0 ellek      (501) staff       (20)      737 2023-01-11 01:43:23.000000 pied_poker-1.0.9/pied_poker.egg-info/PKG-INFO
+-rw-r--r--   0 ellek      (501) staff       (20)     2430 2023-01-11 01:43:23.000000 pied_poker-1.0.9/pied_poker.egg-info/SOURCES.txt
+-rw-r--r--   0 ellek      (501) staff       (20)        1 2023-01-11 01:43:23.000000 pied_poker-1.0.9/pied_poker.egg-info/dependency_links.txt
+-rw-r--r--   0 ellek      (501) staff       (20)       33 2023-01-11 01:43:23.000000 pied_poker-1.0.9/pied_poker.egg-info/requires.txt
+-rw-r--r--   0 ellek      (501) staff       (20)       11 2023-01-11 01:43:23.000000 pied_poker-1.0.9/pied_poker.egg-info/top_level.txt
+-rw-r--r--   0 ellek      (501) staff       (20)       38 2023-01-11 01:43:23.805137 pied_poker-1.0.9/setup.cfg
+-rw-r--r--   0 ellek      (501) staff       (20)     1359 2023-01-11 01:42:49.000000 pied_poker-1.0.9/setup.py
```

### Comparing `pied_poker-1.0.8/PKG-INFO` & `pied_poker-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pied_poker
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python package to run flexible and fast poker simulations using a monte carlo style simulator.
 Home-page: https://github.com/elleklinton/PiedPoker
 Author: Ellek Linton
 Author-email: ellek@elleklinton.com
 License: GNU LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pied_poker-1.0.8/pied_poker/__init__.py` & `pied_poker-1.0.9/pied_poker/__init__.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/card/card.py` & `pied_poker-1.0.9/pied_poker/card/card.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/card/rank.py` & `pied_poker-1.0.9/pied_poker/card/rank.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/card/suit.py` & `pied_poker-1.0.9/pied_poker/card/suit.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/deck/deck.py` & `pied_poker-1.0.9/pied_poker/deck/deck.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/hand/__init__.py` & `pied_poker-1.0.9/pied_poker/hand/__init__.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/hand/base_hand.py` & `pied_poker-1.0.9/pied_poker/hand/base_hand.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/hand/flush.py` & `pied_poker-1.0.9/pied_poker/hand/flush.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/hand/four_of_a_kind.py` & `pied_poker-1.0.9/pied_poker/hand/four_of_a_kind.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/hand/full_house.py` & `pied_poker-1.0.9/pied_poker/hand/full_house.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/hand/high_card.py` & `pied_poker-1.0.9/pied_poker/hand/high_card.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/hand/one_pair.py` & `pied_poker-1.0.9/pied_poker/hand/one_pair.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/hand/poker_hand.py` & `pied_poker-1.0.9/pied_poker/hand/poker_hand.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/hand/royal_flush.py` & `pied_poker-1.0.9/pied_poker/hand/royal_flush.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/hand/straight.py` & `pied_poker-1.0.9/pied_poker/hand/straight.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/hand/straight_flush.py` & `pied_poker-1.0.9/pied_poker/hand/straight_flush.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/hand/three_of_a_kind.py` & `pied_poker-1.0.9/pied_poker/hand/three_of_a_kind.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/hand/two_pair.py` & `pied_poker-1.0.9/pied_poker/hand/two_pair.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/player/player.py` & `pied_poker-1.0.9/pied_poker/player/player.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/poker_round/poker_round.py` & `pied_poker-1.0.9/pied_poker/poker_round/poker_round.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/poker_round/poker_round_result.py` & `pied_poker-1.0.9/pied_poker/poker_round/poker_round_result.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/poker_round/poker_round_simulation_result.py` & `pied_poker-1.0.9/pied_poker/poker_round/poker_round_simulation_result.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/poker_round/poker_round_simulator.py` & `pied_poker-1.0.9/pied_poker/poker_round/poker_round_simulator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import sys
-from typing import List
+from typing import List, Callable
 from joblib import Parallel, delayed
 from tqdm import tqdm
 from copy import deepcopy
 
 import pied_poker.card.card as card
 import pied_poker.player.player as player
 import pied_poker.poker_round.poker_round_simulation_result as simulation_probability
@@ -34,42 +34,63 @@
         for i in range(total_players - len(players)):
             i = i + 1 + len(players)
             players.append(player.Player(f'player_{i}', []))
 
         self.round = round.PokerRound(community_cards, players, other_drawn_cards)
         self.players = self.round.players
 
-    def simulate(self, n: int = 1000, n_jobs: int = -1, status_bar: bool = True) \
-            -> simulation_probability.PokerRoundSimulationResult:
+    def simulate(self, n: int = 1000,
+                 n_jobs: int = -1,
+                 status_bar: bool = True,
+                 callback: Callable[[float], None] = lambda x: None,
+                 callback_frequency: float = 1.0) -> simulation_probability.PokerRoundSimulationResult:
         """
         Runs a simulation of n poker games, and returns a SimulationProbability object, which is be used to compute
         probabilities based on the simulations run. This function is parallelized and configurable via function
         parameters.
 
         :param status_bar: Whether to display status bar
         :type status_bar: bool
         :param n: Number of simulations to run
         :type n: int
         :param n_jobs: Number of jobs used during process parallelization. To disable parallelization, set n_jobs to 1.
         To use all available CPUs, set n_jobs to -1. Do NOT use parallelization when running through an interactive
         console.
         :type n_jobs: int
+        :param callback: Called on progress intervals. Only called when n_jobs is 1 (no parallelization)
+        :type: Callable[[float], None]
+        :param callback_frequency: The frequency at which the callback is called, in percent. I.e. to call the callback
+        every 1 percent of progress, set callback_frequency to 0.01. To call the callback every 0.05 percents of progress, set
+        callback_frequency to 5.
+        :type: float
         :return: SimulationProbability object, used to compute probabilities based on the simulations run.
         :rtype: SimulationProbability
         """
         simulations: List[round_result.PokerRoundResult]
 
         interactive_console = bool(getattr(sys, 'ps1', sys.flags.interactive))
         # If we are in interactive console, prevent threading because it breaks there
 
         if n_jobs == 1 or interactive_console:  # Don't want to parallelize
             if n_jobs != 1 and interactive_console:
                 print(f'Warning: Threading was requested (n_jobs={n_jobs}), but disabling threading because interactive'
                       f' console was detected.')
 
+                simulations = []
+                rounds_per_callback = n * callback_frequency
+                rounds_since_last_callback = rounds_per_callback - 1
+                for i in range(n) if not status_bar else tqdm(range(n)):
+                    simulations.append(self.round.simulate())
+                    rounds_since_last_callback += 1
+                    if rounds_since_last_callback == rounds_per_callback:
+                        callback(i / n)
+                        rounds_since_last_callback = 0
+
+
+
             if not status_bar:
                 simulations = [self.round.simulate() for i in range(n)]
             else:
                 simulations = [self.round.simulate() for i in tqdm(range(n))]
         else:
             if not status_bar:
                 simulations = Parallel(n_jobs=n_jobs)(delayed(self.round.simulate)() for i in range(n))
```

### Comparing `pied_poker-1.0.8/pied_poker/probability/__init__.py` & `pied_poker-1.0.9/pied_poker/probability/__init__.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/base_poker_event.py` & `pied_poker-1.0.9/pied_poker/probability/base_poker_event.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/events/__init__.py` & `pied_poker-1.0.9/pied_poker/probability/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/events/community_cards_include.py` & `pied_poker-1.0.9/pied_poker/probability/events/community_cards_include.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/events/no_tie.py` & `pied_poker-1.0.9/pied_poker/probability/events/no_tie.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/events/player_has_card_ranks.py` & `pied_poker-1.0.9/pied_poker/probability/events/player_has_card_ranks.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/events/player_has_card_suits.py` & `pied_poker-1.0.9/pied_poker/probability/events/player_has_card_suits.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/events/player_has_cards.py` & `pied_poker-1.0.9/pied_poker/probability/events/player_has_cards.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/events/player_has_hand.py` & `pied_poker-1.0.9/pied_poker/probability/events/player_has_hand.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/events/player_has_hand_or_higher.py` & `pied_poker-1.0.9/pied_poker/probability/events/player_has_hand_or_higher.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/events/player_has_pocket_pair.py` & `pied_poker-1.0.9/pied_poker/probability/events/player_has_pocket_pair.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/events/player_has_suited_cards.py` & `pied_poker-1.0.9/pied_poker/probability/events/player_has_suited_cards.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/events/player_loses.py` & `pied_poker-1.0.9/pied_poker/probability/events/player_loses.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/events/player_wins.py` & `pied_poker-1.0.9/pied_poker/probability/events/player_wins.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/events/player_wins_with_tie.py` & `pied_poker-1.0.9/pied_poker/probability/events/player_wins_with_tie.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/events/tie.py` & `pied_poker-1.0.9/pied_poker/probability/events/tie.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/probability/probability_value.py` & `pied_poker-1.0.9/pied_poker/probability/probability_value.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/visualization/heatmap/categorical_heat_map.py` & `pied_poker-1.0.9/pied_poker/visualization/heatmap/categorical_heat_map.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/visualization/heatmap/heatmap_dimension.py` & `pied_poker-1.0.9/pied_poker/visualization/heatmap/heatmap_dimension.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/visualization/heatmap/heatmap_generator.py` & `pied_poker-1.0.9/pied_poker/visualization/heatmap/heatmap_generator.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/visualization/heatmap_samples/all_suited_starting_hands.py` & `pied_poker-1.0.9/pied_poker/visualization/heatmap_samples/all_suited_starting_hands.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/visualization/heatmap_samples/pocket_pair_vs_num_players.py` & `pied_poker-1.0.9/pied_poker/visualization/heatmap_samples/pocket_pair_vs_num_players.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker/visualization/pocket_pair_map.py` & `pied_poker-1.0.9/pied_poker/visualization/pocket_pair_map.py`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/pied_poker.egg-info/PKG-INFO` & `pied_poker-1.0.9/pied_poker.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pied-poker
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python package to run flexible and fast poker simulations using a monte carlo style simulator.
 Home-page: https://github.com/elleklinton/PiedPoker
 Author: Ellek Linton
 Author-email: ellek@elleklinton.com
 License: GNU LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pied_poker-1.0.8/pied_poker.egg-info/SOURCES.txt` & `pied_poker-1.0.9/pied_poker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pied_poker-1.0.8/setup.py` & `pied_poker-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name='pied_poker',
-    version='1.0.8',
+    version='1.0.9',
     description='A Python package to run flexible and fast poker simulations using a monte carlo style simulator.',
     long_description='A Python package to run flexible and fast poker simulations using a monte carlo style simulator.',
     url='https://github.com/elleklinton/PiedPoker',
     author='Ellek Linton',
     author_email='ellek@elleklinton.com',
     license='GNU LGPLv3',
     packages=['pied_poker',
```

