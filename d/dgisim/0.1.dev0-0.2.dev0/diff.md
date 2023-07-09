# Comparing `tmp/dgisim-0.1.dev0.tar.gz` & `tmp/dgisim-0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgisim-0.1.dev0.tar", last modified: Mon Jul  3 22:21:09 2023, max compression
+gzip compressed data, was "dgisim-0.2.dev0.tar", last modified: Sun Jul  9 00:13:39 2023, max compression
```

## Comparing `dgisim-0.1.dev0.tar` & `dgisim-0.2.dev0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.747501 dgisim-0.1.dev0/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1065 2023-02-15 18:18:52.000000 dgisim-0.1.dev0/LICENSE
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     6814 2023-07-03 22:21:09.746894 dgisim-0.1.dev0/PKG-INFO
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     4468 2023-07-03 22:19:52.000000 dgisim-0.1.dev0/README.md
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.695684 dgisim-0.1.dev0/dgisim.egg-info/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     6814 2023-07-03 22:21:09.000000 dgisim-0.1.dev0/dgisim.egg-info/PKG-INFO
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1942 2023-07-03 22:21:09.000000 dgisim-0.1.dev0/dgisim.egg-info/SOURCES.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        1 2023-07-03 22:21:09.000000 dgisim-0.1.dev0/dgisim.egg-info/dependency_links.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)       25 2023-07-03 22:21:09.000000 dgisim-0.1.dev0/dgisim.egg-info/requires.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        7 2023-07-03 22:21:09.000000 dgisim-0.1.dev0/dgisim.egg-info/top_level.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1254 2023-07-03 21:49:10.000000 dgisim-0.1.dev0/pyproject.toml
--rw-r--r--   0 jarvis_yu   (501) staff       (20)       38 2023-07-03 22:21:09.747648 dgisim-0.1.dev0/setup.cfg
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.690283 dgisim-0.1.dev0/src/
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.700837 dgisim-0.1.dev0/src/dgisim/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 21:33:39.000000 dgisim-0.1.dev0/src/dgisim/__init__.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.703470 dgisim-0.1.dev0/src/dgisim/action/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-06-28 19:50:29.000000 dgisim-0.1.dev0/src/dgisim/action/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     6648 2023-07-03 21:39:02.000000 dgisim-0.1.dev0/src/dgisim/action/action.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     2107 2023-07-03 21:05:16.000000 dgisim-0.1.dev0/src/dgisim/action/action_generator.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      517 2023-07-03 21:00:50.000000 dgisim-0.1.dev0/src/dgisim/action/types.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    20755 2023-07-03 21:22:18.000000 dgisim-0.1.dev0/src/dgisim/agents.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.705974 dgisim-0.1.dev0/src/dgisim/card/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-04-10 21:52:38.000000 dgisim-0.1.dev0/src/dgisim/card/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    32846 2023-07-03 21:03:29.000000 dgisim-0.1.dev0/src/dgisim/card/card.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     3530 2023-07-03 21:39:13.000000 dgisim-0.1.dev0/src/dgisim/card/cards.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      877 2023-07-03 21:04:05.000000 dgisim-0.1.dev0/src/dgisim/card/cards_set.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.709065 dgisim-0.1.dev0/src/dgisim/character/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-02-21 20:53:54.000000 dgisim-0.1.dev0/src/dgisim/character/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    25356 2023-07-03 21:39:36.000000 dgisim-0.1.dev0/src/dgisim/character/character.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      650 2023-07-03 21:07:21.000000 dgisim-0.1.dev0/src/dgisim/character/character_skill_enum.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     6806 2023-07-03 21:07:40.000000 dgisim-0.1.dev0/src/dgisim/character/characters.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      525 2023-07-03 21:07:31.000000 dgisim-0.1.dev0/src/dgisim/character/characters_set.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     8987 2023-07-03 21:43:27.000000 dgisim-0.1.dev0/src/dgisim/cli.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     9545 2023-07-03 21:22:18.000000 dgisim-0.1.dev0/src/dgisim/dices.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.714917 dgisim-0.1.dev0/src/dgisim/effect/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-05-30 22:12:07.000000 dgisim-0.1.dev0/src/dgisim/effect/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    41563 2023-07-03 21:08:25.000000 dgisim-0.1.dev0/src/dgisim/effect/effect.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     2147 2023-07-03 21:08:39.000000 dgisim-0.1.dev0/src/dgisim/effect/effect_stack.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      761 2023-07-03 21:39:47.000000 dgisim-0.1.dev0/src/dgisim/effect/effects_template.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      640 2023-07-02 22:52:34.000000 dgisim-0.1.dev0/src/dgisim/effect/enums.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      755 2023-07-03 21:09:13.000000 dgisim-0.1.dev0/src/dgisim/effect/structs.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.716291 dgisim-0.1.dev0/src/dgisim/element/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-02-24 23:27:01.000000 dgisim-0.1.dev0/src/dgisim/element/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     5250 2023-07-03 21:09:56.000000 dgisim-0.1.dev0/src/dgisim/element/element.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.717600 dgisim-0.1.dev0/src/dgisim/event/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-06-24 15:51:54.000000 dgisim-0.1.dev0/src/dgisim/event/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      882 2023-07-03 21:09:56.000000 dgisim-0.1.dev0/src/dgisim/event/event.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     6587 2023-07-03 21:22:30.000000 dgisim-0.1.dev0/src/dgisim/game_state_machine.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.721068 dgisim-0.1.dev0/src/dgisim/helper/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-02-18 00:08:49.000000 dgisim-0.1.dev0/src/dgisim/helper/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     3515 2023-06-24 11:10:20.000000 dgisim-0.1.dev0/src/dgisim/helper/hashable_dict.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     8833 2023-07-02 22:52:34.000000 dgisim-0.1.dev0/src/dgisim/helper/level_print.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      634 2023-06-24 15:51:54.000000 dgisim-0.1.dev0/src/dgisim/helper/quality_of_life.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     3202 2023-07-03 21:37:41.000000 dgisim-0.1.dev0/src/dgisim/mode.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.728484 dgisim-0.1.dev0/src/dgisim/phase/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-02-15 21:56:21.000000 dgisim-0.1.dev0/src/dgisim/phase/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    13364 2023-07-03 21:10:44.000000 dgisim-0.1.dev0/src/dgisim/phase/action_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     4127 2023-07-03 21:11:41.000000 dgisim-0.1.dev0/src/dgisim/phase/card_select_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     6354 2023-07-03 21:41:15.000000 dgisim-0.1.dev0/src/dgisim/phase/end_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      267 2023-07-03 21:13:40.000000 dgisim-0.1.dev0/src/dgisim/phase/game_end_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1257 2023-07-03 21:13:40.000000 dgisim-0.1.dev0/src/dgisim/phase/phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1775 2023-07-03 21:13:40.000000 dgisim-0.1.dev0/src/dgisim/phase/roll_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     2687 2023-07-03 21:14:16.000000 dgisim-0.1.dev0/src/dgisim/phase/starting_hand_select_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      555 2023-07-03 21:23:47.000000 dgisim-0.1.dev0/src/dgisim/player_agent.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.733604 dgisim-0.1.dev0/src/dgisim/state/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-04-10 21:52:38.000000 dgisim-0.1.dev0/src/dgisim/state/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      947 2023-07-02 22:52:34.000000 dgisim-0.1.dev0/src/dgisim/state/enums.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    26897 2023-07-03 21:41:15.000000 dgisim-0.1.dev0/src/dgisim/state/game_state.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     9362 2023-07-03 21:17:43.000000 dgisim-0.1.dev0/src/dgisim/state/player_state.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.740462 dgisim-0.1.dev0/src/dgisim/status/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-05-30 22:12:07.000000 dgisim-0.1.dev0/src/dgisim/status/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      642 2023-07-02 22:52:34.000000 dgisim-0.1.dev0/src/dgisim/status/enums.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    33544 2023-07-03 21:41:15.000000 dgisim-0.1.dev0/src/dgisim/status/status.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     8142 2023-07-03 21:18:04.000000 dgisim-0.1.dev0/src/dgisim/status/status_processing.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     2762 2023-07-03 21:18:26.000000 dgisim-0.1.dev0/src/dgisim/status/statuses.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      143 2023-07-03 21:41:15.000000 dgisim-0.1.dev0/src/dgisim/status/types.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.743035 dgisim-0.1.dev0/src/dgisim/summon/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-06-11 14:32:47.000000 dgisim-0.1.dev0/src/dgisim/summon/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     4498 2023-07-03 21:18:47.000000 dgisim-0.1.dev0/src/dgisim/summon/summon.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     2547 2023-07-03 21:18:56.000000 dgisim-0.1.dev0/src/dgisim/summon/summons.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-03 22:21:09.745447 dgisim-0.1.dev0/src/dgisim/support/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-06-25 19:24:23.000000 dgisim-0.1.dev0/src/dgisim/support/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     2722 2023-07-03 21:26:33.000000 dgisim-0.1.dev0/src/dgisim/support/support.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     4049 2023-07-03 21:26:33.000000 dgisim-0.1.dev0/src/dgisim/support/supports.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.334931 dgisim-0.2.dev0/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1065 2023-02-15 18:18:52.000000 dgisim-0.2.dev0/LICENSE
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     6962 2023-07-09 00:13:39.334376 dgisim-0.2.dev0/PKG-INFO
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     4375 2023-07-09 00:09:20.000000 dgisim-0.2.dev0/README.md
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.287731 dgisim-0.2.dev0/dgisim/
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.298595 dgisim-0.2.dev0/dgisim/src/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      928 2023-07-09 00:06:09.000000 dgisim-0.2.dev0/dgisim/src/__init__.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.301894 dgisim-0.2.dev0/dgisim/src/action/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:00.000000 dgisim-0.2.dev0/dgisim/src/action/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     6827 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/action/action.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     3475 2023-07-08 23:37:31.000000 dgisim-0.2.dev0/dgisim/src/action/action_generator.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    15539 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/action/action_generator_generator.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      276 2023-07-08 23:36:31.000000 dgisim-0.2.dev0/dgisim/src/action/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      647 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/action/types.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    11755 2023-07-08 23:43:20.000000 dgisim-0.2.dev0/dgisim/src/agents.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.304435 dgisim-0.2.dev0/dgisim/src/card/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:07.000000 dgisim-0.2.dev0/dgisim/src/card/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    34168 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/card/card.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     3938 2023-07-08 23:16:29.000000 dgisim-0.2.dev0/dgisim/src/card/cards.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      686 2023-07-08 23:17:02.000000 dgisim-0.2.dev0/dgisim/src/card/cards_set.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.307098 dgisim-0.2.dev0/dgisim/src/character/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:12.000000 dgisim-0.2.dev0/dgisim/src/character/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    24971 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/character/character.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     6293 2023-07-08 23:09:50.000000 dgisim-0.2.dev0/dgisim/src/character/characters.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      459 2023-07-08 23:17:18.000000 dgisim-0.2.dev0/dgisim/src/character/characters_set.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      683 2023-07-08 23:11:13.000000 dgisim-0.2.dev0/dgisim/src/character/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    11920 2023-07-08 21:45:04.000000 dgisim-0.2.dev0/dgisim/src/cli.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    10173 2023-07-08 22:26:38.000000 dgisim-0.2.dev0/dgisim/src/dices.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.310553 dgisim-0.2.dev0/dgisim/src/effect/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:16.000000 dgisim-0.2.dev0/dgisim/src/effect/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    44279 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/effect/effect.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     2181 2023-07-08 23:07:04.000000 dgisim-0.2.dev0/dgisim/src/effect/effect_stack.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      806 2023-07-08 22:39:44.000000 dgisim-0.2.dev0/dgisim/src/effect/effects_template.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      726 2023-07-08 22:39:20.000000 dgisim-0.2.dev0/dgisim/src/effect/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1247 2023-07-08 22:37:50.000000 dgisim-0.2.dev0/dgisim/src/effect/structs.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     5464 2023-07-08 21:45:34.000000 dgisim-0.2.dev0/dgisim/src/element.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      963 2023-07-08 22:33:10.000000 dgisim-0.2.dev0/dgisim/src/event.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     7130 2023-07-08 21:25:18.000000 dgisim-0.2.dev0/dgisim/src/game_state_machine.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.313692 dgisim-0.2.dev0/dgisim/src/helper/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)       86 2023-07-08 23:41:02.000000 dgisim-0.2.dev0/dgisim/src/helper/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     3707 2023-07-08 22:26:17.000000 dgisim-0.2.dev0/dgisim/src/helper/hashable_dict.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     9098 2023-07-08 22:29:08.000000 dgisim-0.2.dev0/dgisim/src/helper/level_print.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1284 2023-07-08 22:30:12.000000 dgisim-0.2.dev0/dgisim/src/helper/quality_of_life.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     3934 2023-07-08 22:31:24.000000 dgisim-0.2.dev0/dgisim/src/mode.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.314881 dgisim-0.2.dev0/dgisim/src/phase/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)       20 2023-07-08 23:32:15.000000 dgisim-0.2.dev0/dgisim/src/phase/__init__.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.319548 dgisim-0.2.dev0/dgisim/src/phase/default/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      397 2023-07-08 23:33:53.000000 dgisim-0.2.dev0/dgisim/src/phase/default/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    17142 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/phase/default/action_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     6090 2023-07-08 22:22:28.000000 dgisim-0.2.dev0/dgisim/src/phase/default/card_select_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     7024 2023-07-08 23:45:15.000000 dgisim-0.2.dev0/dgisim/src/phase/default/end_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      906 2023-07-08 22:23:01.000000 dgisim-0.2.dev0/dgisim/src/phase/default/game_end_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     5896 2023-07-08 22:23:13.000000 dgisim-0.2.dev0/dgisim/src/phase/default/roll_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     4353 2023-07-08 22:23:28.000000 dgisim-0.2.dev0/dgisim/src/phase/default/starting_hand_select_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1550 2023-07-08 22:21:20.000000 dgisim-0.2.dev0/dgisim/src/phase/phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      538 2023-07-08 21:36:26.000000 dgisim-0.2.dev0/dgisim/src/player_agent.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.323092 dgisim-0.2.dev0/dgisim/src/state/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:04:22.000000 dgisim-0.2.dev0/dgisim/src/state/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      983 2023-07-08 22:16:24.000000 dgisim-0.2.dev0/dgisim/src/state/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    20106 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/state/game_state.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    10577 2023-07-08 22:26:32.000000 dgisim-0.2.dev0/dgisim/src/state/player_state.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.328099 dgisim-0.2.dev0/dgisim/src/status/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:35.000000 dgisim-0.2.dev0/dgisim/src/status/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      682 2023-07-08 21:48:31.000000 dgisim-0.2.dev0/dgisim/src/status/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    35218 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/status/status.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     8428 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/status/status_processing.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     2852 2023-07-08 22:15:11.000000 dgisim-0.2.dev0/dgisim/src/status/statuses.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      180 2023-07-08 22:35:19.000000 dgisim-0.2.dev0/dgisim/src/status/types.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.330577 dgisim-0.2.dev0/dgisim/src/summon/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:39.000000 dgisim-0.2.dev0/dgisim/src/summon/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     5119 2023-07-08 21:54:05.000000 dgisim-0.2.dev0/dgisim/src/summon/summon.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     2636 2023-07-08 22:14:55.000000 dgisim-0.2.dev0/dgisim/src/summon/summons.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.332882 dgisim-0.2.dev0/dgisim/src/support/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:43.000000 dgisim-0.2.dev0/dgisim/src/support/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     3240 2023-07-08 22:34:57.000000 dgisim-0.2.dev0/dgisim/src/support/support.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     4138 2023-07-08 22:14:45.000000 dgisim-0.2.dev0/dgisim/src/support/supports.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.292153 dgisim-0.2.dev0/dgisim.egg-info/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     6962 2023-07-09 00:13:39.000000 dgisim-0.2.dev0/dgisim.egg-info/PKG-INFO
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     2013 2023-07-09 00:13:39.000000 dgisim-0.2.dev0/dgisim.egg-info/SOURCES.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        1 2023-07-09 00:13:39.000000 dgisim-0.2.dev0/dgisim.egg-info/dependency_links.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)       25 2023-07-09 00:13:39.000000 dgisim-0.2.dev0/dgisim.egg-info/requires.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        7 2023-07-09 00:13:39.000000 dgisim-0.2.dev0/dgisim.egg-info/top_level.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1475 2023-07-09 00:10:17.000000 dgisim-0.2.dev0/pyproject.toml
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)       38 2023-07-09 00:13:39.335076 dgisim-0.2.dev0/setup.cfg
```

### Comparing `dgisim-0.1.dev0/LICENSE` & `dgisim-0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `dgisim-0.1.dev0/PKG-INFO` & `dgisim-0.2.dev0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgisim
-Version: 0.1.dev0
+Version: 0.2.dev0
 Summary: A highly customizable Genius Invokation TCG Simulator for AI training
 Author: Jarvis Yu
 License: MIT License
         
         Copyright (c) 2023 Leyang Yu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,14 +22,16 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: source, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator
 Project-URL: tracker, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/issues
+Project-URL: changelog, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/CHANGELOG.md
+Project-URL: documentation, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki/v0.2.dev0-Documentation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -37,29 +39,32 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.10.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dottore Genius Invokation TCG Simulator
 
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
 [![Coverage Status](https://coveralls.io/repos/github/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/badge.svg?branch=master)](https://coveralls.io/github/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator?branch=master)
 
 A Genshin Impact Genius Invokation TCG simulator intended to be used for AI training (for now).
 
 The simulator is modeled as a finite state machine, where all game states are immutable.
 
-## Install
+Basic rules of Genius Invokation TCG can be found [here](https://genshin-impact.fandom.com/wiki/Genius_Invokation_TCG).
 
-Make sure your Python version `>= 3.10.11`.
+## Installation
+
+Make sure your Python version `>= 3.10`.
 
 ```shell
 pip install dgisim
 ```
 
 Note that this is a developing project and the final API to users is not set in stone.
 So you may play with it, but using it in production is not recommended at the current stage.
@@ -67,15 +72,15 @@
 ## Simple Guide
 
 Once installed, you may have a try with the CLI to play the simulator in command line.
 
 You might want to run a simple python program like this:
 
 ```py
-from dgisim.cli import CLISession
+from dgisim import CLISession
 
 session = CLISession()
 session.run()
 ```
 
 See CLI's [README](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/cli_readme.md)
 for showcase and explanations of the CLI.
@@ -128,27 +133,21 @@
 - [x] Implement game phase of End Phase (summons and some support card or statuses take action)
 - [x] Implement game phase of Game End Phase (one player wins or draw)
 - [x] Implement CLI for better debugging experience
 - [x] Implement interactive active CLI that accepts user input as action
 - [x] Implement lazy player agent for minimal testing purposes
 - [x] Implement random player agent for testing purposes
 - [x] Implement player action validity checker
-- [ ] Implement player action choices provider
-  - [x] all action phase choices provider
-  - [x] all end phase choices provider
-  - [ ] Other choices provider (trivial for now)
+- [x] Implement player action choices provider
 - [ ] Implement greedy player agent for testing purposes
 
 > Just in case you don't know, **_WIP_** means "work in progress".
 
 ## Future Plans
 
-The fully developed project will be published to PyPI (beta versions will be available once all that
-are left is adding more characters and cards)
-
 I have the plan to implement a simple cross-platform GUI interface for the simulator. But that will
 be in a separate repo.
 
 Once this project is done, I'll be reading relative papers and develop an AI for this game. The AI
 is supposed to be used for learning strategies and making decks, but not against another player
 directly.
```

### Comparing `dgisim-0.1.dev0/README.md` & `dgisim-0.2.dev0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # Dottore Genius Invokation TCG Simulator
 
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
 [![Coverage Status](https://coveralls.io/repos/github/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/badge.svg?branch=master)](https://coveralls.io/github/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator?branch=master)
 
 A Genshin Impact Genius Invokation TCG simulator intended to be used for AI training (for now).
 
 The simulator is modeled as a finite state machine, where all game states are immutable.
 
-## Install
+Basic rules of Genius Invokation TCG can be found [here](https://genshin-impact.fandom.com/wiki/Genius_Invokation_TCG).
 
-Make sure your Python version `>= 3.10.11`.
+## Installation
+
+Make sure your Python version `>= 3.10`.
 
 ```shell
 pip install dgisim
 ```
 
 Note that this is a developing project and the final API to users is not set in stone.
 So you may play with it, but using it in production is not recommended at the current stage.
@@ -20,15 +23,15 @@
 ## Simple Guide
 
 Once installed, you may have a try with the CLI to play the simulator in command line.
 
 You might want to run a simple python program like this:
 
 ```py
-from dgisim.cli import CLISession
+from dgisim import CLISession
 
 session = CLISession()
 session.run()
 ```
 
 See CLI's [README](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/cli_readme.md)
 for showcase and explanations of the CLI.
@@ -81,27 +84,21 @@
 - [x] Implement game phase of End Phase (summons and some support card or statuses take action)
 - [x] Implement game phase of Game End Phase (one player wins or draw)
 - [x] Implement CLI for better debugging experience
 - [x] Implement interactive active CLI that accepts user input as action
 - [x] Implement lazy player agent for minimal testing purposes
 - [x] Implement random player agent for testing purposes
 - [x] Implement player action validity checker
-- [ ] Implement player action choices provider
-  - [x] all action phase choices provider
-  - [x] all end phase choices provider
-  - [ ] Other choices provider (trivial for now)
+- [x] Implement player action choices provider
 - [ ] Implement greedy player agent for testing purposes
 
 > Just in case you don't know, **_WIP_** means "work in progress".
 
 ## Future Plans
 
-The fully developed project will be published to PyPI (beta versions will be available once all that
-are left is adding more characters and cards)
-
 I have the plan to implement a simple cross-platform GUI interface for the simulator. But that will
 be in a separate repo.
 
 Once this project is done, I'll be reading relative papers and develop an AI for this game. The AI
 is supposed to be used for learning strategies and making decks, but not against another player
 directly.
```

### Comparing `dgisim-0.1.dev0/dgisim.egg-info/PKG-INFO` & `dgisim-0.2.dev0/dgisim.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgisim
-Version: 0.1.dev0
+Version: 0.2.dev0
 Summary: A highly customizable Genius Invokation TCG Simulator for AI training
 Author: Jarvis Yu
 License: MIT License
         
         Copyright (c) 2023 Leyang Yu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,14 +22,16 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: source, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator
 Project-URL: tracker, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/issues
+Project-URL: changelog, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/CHANGELOG.md
+Project-URL: documentation, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki/v0.2.dev0-Documentation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -37,29 +39,32 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.10.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dottore Genius Invokation TCG Simulator
 
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
 [![Coverage Status](https://coveralls.io/repos/github/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/badge.svg?branch=master)](https://coveralls.io/github/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator?branch=master)
 
 A Genshin Impact Genius Invokation TCG simulator intended to be used for AI training (for now).
 
 The simulator is modeled as a finite state machine, where all game states are immutable.
 
-## Install
+Basic rules of Genius Invokation TCG can be found [here](https://genshin-impact.fandom.com/wiki/Genius_Invokation_TCG).
 
-Make sure your Python version `>= 3.10.11`.
+## Installation
+
+Make sure your Python version `>= 3.10`.
 
 ```shell
 pip install dgisim
 ```
 
 Note that this is a developing project and the final API to users is not set in stone.
 So you may play with it, but using it in production is not recommended at the current stage.
@@ -67,15 +72,15 @@
 ## Simple Guide
 
 Once installed, you may have a try with the CLI to play the simulator in command line.
 
 You might want to run a simple python program like this:
 
 ```py
-from dgisim.cli import CLISession
+from dgisim import CLISession
 
 session = CLISession()
 session.run()
 ```
 
 See CLI's [README](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/docs/cli_readme.md)
 for showcase and explanations of the CLI.
@@ -128,27 +133,21 @@
 - [x] Implement game phase of End Phase (summons and some support card or statuses take action)
 - [x] Implement game phase of Game End Phase (one player wins or draw)
 - [x] Implement CLI for better debugging experience
 - [x] Implement interactive active CLI that accepts user input as action
 - [x] Implement lazy player agent for minimal testing purposes
 - [x] Implement random player agent for testing purposes
 - [x] Implement player action validity checker
-- [ ] Implement player action choices provider
-  - [x] all action phase choices provider
-  - [x] all end phase choices provider
-  - [ ] Other choices provider (trivial for now)
+- [x] Implement player action choices provider
 - [ ] Implement greedy player agent for testing purposes
 
 > Just in case you don't know, **_WIP_** means "work in progress".
 
 ## Future Plans
 
-The fully developed project will be published to PyPI (beta versions will be available once all that
-are left is adding more characters and cards)
-
 I have the plan to implement a simple cross-platform GUI interface for the simulator. But that will
 be in a separate repo.
 
 Once this project is done, I'll be reading relative papers and develop an AI for this game. The AI
 is supposed to be used for learning strategies and making decks, but not against another player
 directly.
```

### Comparing `dgisim-0.1.dev0/dgisim.egg-info/SOURCES.txt` & `dgisim-0.2.dev0/dgisim.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -2,65 +2,66 @@
 README.md
 pyproject.toml
 dgisim.egg-info/PKG-INFO
 dgisim.egg-info/SOURCES.txt
 dgisim.egg-info/dependency_links.txt
 dgisim.egg-info/requires.txt
 dgisim.egg-info/top_level.txt
-src/dgisim/__init__.py
-src/dgisim/agents.py
-src/dgisim/cli.py
-src/dgisim/dices.py
-src/dgisim/game_state_machine.py
-src/dgisim/mode.py
-src/dgisim/player_agent.py
-src/dgisim/action/__init__.py
-src/dgisim/action/action.py
-src/dgisim/action/action_generator.py
-src/dgisim/action/types.py
-src/dgisim/card/__init__.py
-src/dgisim/card/card.py
-src/dgisim/card/cards.py
-src/dgisim/card/cards_set.py
-src/dgisim/character/__init__.py
-src/dgisim/character/character.py
-src/dgisim/character/character_skill_enum.py
-src/dgisim/character/characters.py
-src/dgisim/character/characters_set.py
-src/dgisim/effect/__init__.py
-src/dgisim/effect/effect.py
-src/dgisim/effect/effect_stack.py
-src/dgisim/effect/effects_template.py
-src/dgisim/effect/enums.py
-src/dgisim/effect/structs.py
-src/dgisim/element/__init__.py
-src/dgisim/element/element.py
-src/dgisim/event/__init__.py
-src/dgisim/event/event.py
-src/dgisim/helper/__init__.py
-src/dgisim/helper/hashable_dict.py
-src/dgisim/helper/level_print.py
-src/dgisim/helper/quality_of_life.py
-src/dgisim/phase/__init__.py
-src/dgisim/phase/action_phase.py
-src/dgisim/phase/card_select_phase.py
-src/dgisim/phase/end_phase.py
-src/dgisim/phase/game_end_phase.py
-src/dgisim/phase/phase.py
-src/dgisim/phase/roll_phase.py
-src/dgisim/phase/starting_hand_select_phase.py
-src/dgisim/state/__init__.py
-src/dgisim/state/enums.py
-src/dgisim/state/game_state.py
-src/dgisim/state/player_state.py
-src/dgisim/status/__init__.py
-src/dgisim/status/enums.py
-src/dgisim/status/status.py
-src/dgisim/status/status_processing.py
-src/dgisim/status/statuses.py
-src/dgisim/status/types.py
-src/dgisim/summon/__init__.py
-src/dgisim/summon/summon.py
-src/dgisim/summon/summons.py
-src/dgisim/support/__init__.py
-src/dgisim/support/support.py
-src/dgisim/support/supports.py
+dgisim/src/__init__.py
+dgisim/src/agents.py
+dgisim/src/cli.py
+dgisim/src/dices.py
+dgisim/src/element.py
+dgisim/src/event.py
+dgisim/src/game_state_machine.py
+dgisim/src/mode.py
+dgisim/src/player_agent.py
+dgisim/src/action/__init__.py
+dgisim/src/action/action.py
+dgisim/src/action/action_generator.py
+dgisim/src/action/action_generator_generator.py
+dgisim/src/action/enums.py
+dgisim/src/action/types.py
+dgisim/src/card/__init__.py
+dgisim/src/card/card.py
+dgisim/src/card/cards.py
+dgisim/src/card/cards_set.py
+dgisim/src/character/__init__.py
+dgisim/src/character/character.py
+dgisim/src/character/characters.py
+dgisim/src/character/characters_set.py
+dgisim/src/character/enums.py
+dgisim/src/effect/__init__.py
+dgisim/src/effect/effect.py
+dgisim/src/effect/effect_stack.py
+dgisim/src/effect/effects_template.py
+dgisim/src/effect/enums.py
+dgisim/src/effect/structs.py
+dgisim/src/helper/__init__.py
+dgisim/src/helper/hashable_dict.py
+dgisim/src/helper/level_print.py
+dgisim/src/helper/quality_of_life.py
+dgisim/src/phase/__init__.py
+dgisim/src/phase/phase.py
+dgisim/src/phase/default/__init__.py
+dgisim/src/phase/default/action_phase.py
+dgisim/src/phase/default/card_select_phase.py
+dgisim/src/phase/default/end_phase.py
+dgisim/src/phase/default/game_end_phase.py
+dgisim/src/phase/default/roll_phase.py
+dgisim/src/phase/default/starting_hand_select_phase.py
+dgisim/src/state/__init__.py
+dgisim/src/state/enums.py
+dgisim/src/state/game_state.py
+dgisim/src/state/player_state.py
+dgisim/src/status/__init__.py
+dgisim/src/status/enums.py
+dgisim/src/status/status.py
+dgisim/src/status/status_processing.py
+dgisim/src/status/statuses.py
+dgisim/src/status/types.py
+dgisim/src/summon/__init__.py
+dgisim/src/summon/summon.py
+dgisim/src/summon/summons.py
+dgisim/src/support/__init__.py
+dgisim/src/support/support.py
+dgisim/src/support/supports.py
```

### Comparing `dgisim-0.1.dev0/pyproject.toml` & `dgisim-0.2.dev0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dgisim"
-version = "0.1.dev0"
+version = "0.2.dev0"
 license = {file = "LICENSE"}
 
 description = "A highly customizable Genius Invokation TCG Simulator for AI training"
 authors = [{ name="Jarvis Yu" }]
-requires-python = ">=3.10.11"
+requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -32,10 +32,12 @@
 dependencies = [
     "typing-extensions == 4.5.0",
 ]
 
 [project.urls]
 source = "https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator"
 tracker = "https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/issues"
+changelog = "https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/CHANGELOG.md"
+documentation = "https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki/v0.2.dev0-Documentation"
 
 [tool.setuptools.package-dir]
-dgisim = "src/dgisim"
+dgisim = "dgisim/src"
```

### Comparing `dgisim-0.1.dev0/src/dgisim/action/action.py` & `dgisim-0.2.dev0/dgisim/src/action/action.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,57 @@
 from __future__ import annotations
 from dataclasses import dataclass, fields, replace
 from typing import Any, TYPE_CHECKING
 from typing_extensions import Self
 
 from ..card.cards import Cards
-from ..character.character_skill_enum import CharacterSkill
+from ..character.enums import CharacterSkill
 from ..dices import ActualDices
 from ..effect.enums import ZONE
 from ..effect.structs import StaticTarget
-from ..element.element import Element
+from ..element import Element
+from ..helper.quality_of_life import dataclass_repr
 from ..state.enums import PID
 
 if TYPE_CHECKING:
     from ..state.game_state import GameState
     from ..card.card import Card
 
+__all__ = [
+    "PlayerAction",
+    "CardsSelectAction",
+    "DicesSelectAction",
+    "CharacterSelectAction",
+    "EndRoundAction",
+    "GameAction",
+    "ElementalTuningAction",
+    "CardAction",
+    "SkillAction",
+    "SwapAction",
+    "DeathSwapAction",
+    "Instruction",
+    "DiceOnlyInstruction",
+    "StaticTargetInstruction",
+    "SourceTargetInstruction",
+]
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class PlayerAction:
     @classmethod
     def _empty(cls) -> Self:
         """
         This is just for action generator
         """
         return cls()
 
     @classmethod
     def _all_none(cls) -> Self:
         """
         This is just for action generator
+        Sets all fields to None ready to be filled later
         """
         self = cls._empty()
         for field in fields(self):
             object.__setattr__(self, field.name, None)
         return self
 
     def _set_attr(self, name: str, val: Any) -> Self:
@@ -59,116 +78,114 @@
             for field in fields(self)
         )
         return all(
             isinstance(val, field_type)
             for field_type, val in field_type_val
         )
 
-    def __str__(self) -> str:
-        cls_fields = fields(self)
-        paired_fields = (
-            f"{field.name}={str(self.__getattribute__(field.name))}" for field in cls_fields)
-        return f"{self.__class__.__name__}:({', '.join(paired_fields)})"
+    def __repr__(self) -> str:
+        return dataclass_repr(self)
 
 
-@dataclass(frozen=True, kw_only=True)
-class CardSelectAction(PlayerAction):
+@dataclass(frozen=True, kw_only=True, repr=False)
+class CardsSelectAction(PlayerAction):
     selected_cards: Cards
 
     def num_cards(self) -> int:
         return self.selected_cards.num_cards()
 
     @classmethod
     def _empty(cls) -> Self:
         return cls(selected_cards=Cards({}))
 
-    def __str__(self) -> str:
-        name = self.__class__.__name__
-        cards = '; '.join(str(self.selected_cards).split('\n'))
-        return f"{name}[{cards}]"
 
+@dataclass(frozen=True, kw_only=True, repr=False)
+class DicesSelectAction(PlayerAction):
+    selected_dices: ActualDices
 
-@dataclass(frozen=True, kw_only=True)
+    def num_cards(self) -> int:
+        return self.selected_dices.num_dices()
+
+    @classmethod
+    def _empty(cls) -> Self:
+        return cls(selected_dices=ActualDices({}))
+
+
+@dataclass(frozen=True, kw_only=True, repr=False)
 class CharacterSelectAction(PlayerAction):
     char_id: int
 
     @classmethod
     def _empty(cls) -> Self:
         return cls(char_id=-1)
 
 
-@dataclass(frozen=True, kw_only=True)
+@dataclass(frozen=True, kw_only=True, repr=False)
 class EndRoundAction(PlayerAction):
     pass
 
 
-@dataclass(frozen=True, kw_only=True)
+@dataclass(frozen=True, kw_only=True, repr=False)
 class GameAction(PlayerAction):
     def is_valid_action(self, game_state: GameState) -> bool:
         raise Exception("Not overriden")
 
 
-@dataclass(frozen=True, kw_only=True)
+@dataclass(frozen=True, kw_only=True, repr=False)
 class ElementalTuningAction(GameAction):
     card: type[Card]
     dice_elem: Element
 
     @classmethod
     def _empty(cls) -> Self:
         from ..card.card import Card
         return cls(card=Card, dice_elem=Element.ANY)
 
 
-@dataclass(frozen=True, kw_only=True)
+@dataclass(frozen=True, kw_only=True, repr=False)
 class CardAction(GameAction):
     card: type[Card]
     instruction: Instruction
 
     @classmethod
     def _empty(cls) -> Self:
         from ..card.card import Card
         return cls(card=Card, instruction=Instruction._empty())
 
-    def __str__(self) -> str:
-        return f"<{self.card.__name__}, {self.instruction}>"
-
 
-@dataclass(frozen=True, kw_only=True)
+@dataclass(frozen=True, kw_only=True, repr=False)
 class SkillAction(GameAction):
     skill: CharacterSkill
     instruction: DiceOnlyInstruction
 
     @classmethod
     def _empty(cls) -> Self:
         return cls(skill=CharacterSkill.NORMAL_ATTACK, instruction=DiceOnlyInstruction._empty())
 
-    def __str__(self) -> str:
-        return f"<{self.skill}, {self.instruction}>"
 
-
-@dataclass(frozen=True, kw_only=True)
+@dataclass(frozen=True, kw_only=True, repr=False)
 class SwapAction(GameAction):
     char_id: int
     instruction: Instruction
 
     @classmethod
     def _empty(cls) -> Self:
         return cls(char_id=-1, instruction=Instruction._empty())
 
 
-@dataclass(frozen=True, kw_only=True)
+@dataclass(frozen=True, kw_only=True, repr=False)
 class DeathSwapAction(GameAction):
     char_id: int
 
     @classmethod
     def _empty(cls) -> Self:
         return cls(char_id=-1)
 
 
-@dataclass(frozen=True, kw_only=True)
+@dataclass(frozen=True, kw_only=True, repr=False)
 class Instruction:
     dices: ActualDices
 
     @classmethod
     def _empty(cls) -> Self:
         return cls(dices=ActualDices({}))
 
@@ -206,29 +223,24 @@
             for field in fields(self)
         )
         return all(
             isinstance(val, field_type)
             for field_type, val in field_type_val
         )
 
-    def __str__(self) -> str:
-        cls_fields = fields(self)
-        paired_fields = (
-            f"{field.name}={str(self.__getattribute__(field.name))}"
-            for field in cls_fields
-        )
-        return f"{self.__class__.__name__}:({', '.join(paired_fields)})"
+    def __repr__(self) -> str:
+        return dataclass_repr(self)
 
 
-@dataclass(frozen=True, kw_only=True)
+@dataclass(frozen=True, kw_only=True, repr=False)
 class DiceOnlyInstruction(Instruction):
     pass
 
 
-@dataclass(frozen=True, kw_only=True)
+@dataclass(frozen=True, kw_only=True, repr=False)
 class StaticTargetInstruction(Instruction):
     target: StaticTarget
 
     @classmethod
     def _empty(cls) -> Self:
         return cls(
             dices=ActualDices({}),
@@ -236,15 +248,15 @@
                 pid=PID.P1,
                 zone=ZONE.CHARACTERS,
                 id=-1,
             ),
         )
 
 
-@dataclass(frozen=True, kw_only=True)
+@dataclass(frozen=True, kw_only=True, repr=False)
 class SourceTargetInstruction(Instruction):
     source: StaticTarget
     target: StaticTarget
 
     @classmethod
     def _empty(cls) -> Self:
         target = StaticTarget(
```

### Comparing `dgisim-0.1.dev0/src/dgisim/action/action_generator.py` & `dgisim-0.2.dev0/dgisim/src/action/action_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,96 @@
 from __future__ import annotations
 from dataclasses import dataclass, replace, fields
 from typing import Callable, TYPE_CHECKING
 from typing_extensions import Self
 
 if TYPE_CHECKING:
-    from ..state.game_state import GameState
-    from ..state.enums import PID
+    from ..card.cards import Cards
     from ..dices import ActualDices
+    from ..state.enums import PID
+    from ..state.game_state import GameState
 
     from .action import PlayerAction, Instruction
     from .types import DecidedChoiceType, GivenChoiceType
 
+__all__ = [
+    "ActionGenerator",
+]
+
+
+def _dummy_choices_helper(_: ActionGenerator) -> GivenChoiceType:
+    raise NotImplementedError("You are supposed to override this if needed")
+
+
+def _dummy_fill_helper(_a: ActionGenerator, _b: DecidedChoiceType) -> ActionGenerator:
+    raise NotImplementedError("You are supposed to override this if needed")
+
 
 @dataclass(frozen=True, kw_only=True)
 class ActionGenerator:
+    """
+    ActionGenerator is a class recording a state of choices made so far.
+
+    If both action and instruction is None, then this action generator is used 
+    to generate other ActionGenerators that may eventually generate some action.
+    """
     game_state: GameState
     pid: PID
-    action: PlayerAction
+    action: None | PlayerAction = None
     instruction: None | Instruction = None
-    _choices_helper: Callable[[Self], GivenChoiceType]
-    _fill_helper: Callable[[Self, DecidedChoiceType], Self]
+    # used to provide all valid choices for users to choose
+    _choices_helper: Callable[[Self], GivenChoiceType] = _dummy_choices_helper  # type: ignore
+    # takes user's choice and check if it is valid, if so return another
+    # action generator representing the next phase of choice, otherwise raise
+    # Exception
+    _fill_helper: Callable[[Self, DecidedChoiceType], Self] = _dummy_fill_helper  # type: ignore
 
     def _action_filled(self) -> bool:
-        return self.action._filled(exceptions={"instruction"})
+        return self.action is None \
+            or self.action._filled(exceptions={"instruction"})
 
     def _instruction_filled(self) -> bool:
         return self.instruction is None \
             or self.instruction._filled()
 
     def _legal_action(self) -> bool:
-        return self.action.legal()
+        return self.action is None or self.action.legal()
 
     def _legal_instruction(self) -> bool:
         return self.instruction is None or self.instruction.legal()
 
     def filled(self) -> bool:
-        return self._action_filled() and self._instruction_filled()
+        """
+        Return if ActionGenerator is ready to produce the final action
+        """
+        return not (self.action is None and self.instruction is None) \
+            and self._action_filled() and self._instruction_filled()
 
     def valid(self) -> bool:
         return self._legal_action() and self._legal_instruction()
 
     def generate_action(self) -> PlayerAction:
         assert self.filled()
+        assert self.action is not None
         action = self.action
         if self.instruction is not None:
             action = replace(action, instruction=self.instruction)
         return action
 
     def choices(self) -> GivenChoiceType:
         assert not self.filled()
         return self._choices_helper(self)
 
     def dices_available(self) -> ActualDices:
         return self.game_state.get_player(self.pid).get_dices()
 
+    def hand_cards_available(self) -> Cards:
+        return self.game_state.get_player(self.pid).get_hand_cards()
+
     def choose(self, choice: DecidedChoiceType) -> ActionGenerator:
+        assert not self.filled()
         return self._fill_helper(self, choice)
 
     def __str__(self) -> str:
         field_pairs = [f"<{field.name}, {getattr(self, field.name)}>" for field in fields(self)]
         content = '\n'.join(field_pairs)
         return self.__class__.__name__ + '\n' + content
```

### Comparing `dgisim-0.1.dev0/src/dgisim/card/card.py` & `dgisim-0.2.dev0/dgisim/src/card/card.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,92 @@
+"""
+This file contains the base class "Card" for all cards,
+and implementation of all cards.
+
+The classes are divided into 4 sections ordered. Within each section, they are
+ordered alphabetically.
+
+- base class, which is Card
+- type classes, used to identify what type of card a card is
+- template classes, starting with an '_', are templates for other classes
+- concrete classes, the implementation of cards that are actually in the game
+"""
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from dataclasses import replace
 from typing_extensions import override
 
 from ..action import action as act
 from ..action import action_generator as acg
 from ..character import character as chr
 from ..effect import effect as eft
 from ..status import status as stt
 from ..support import support as sp
 
-from ..character.character_skill_enum import CharacterSkill
+from ..character.enums import CharacterSkill
 from ..dices import AbstractDices, ActualDices
 from ..effect.enums import ZONE
 from ..effect.structs import StaticTarget
-from ..element.element import Element
-from ..event.event import CardEvent
+from ..element import Element
+from ..event import CardEvent
 from ..helper.quality_of_life import BIG_INT
 from ..state.enums import PID
 from ..status.enums import PREPROCESSABLES
 from ..status.status_processing import StatusProcessing
 
 if TYPE_CHECKING:
+    from ..action.types import DecidedChoiceType, GivenChoiceType
     from ..state import game_state as gs
 
-    from ..action.types import DecidedChoiceType, GivenChoiceType
+__all__ = [
+    # base
+    "Card",
+
+    # special one
+    "OmniCard",
+
+    # type
+    "EventCard",
+    "EquipmentCard",
+    "SupportCard",
+    "CompanionCard",
+    "LocationCard",
+    "FoodCard",
+
+    # Event Card
+    ## Food Card ##
+    "JueyunGuoba",
+    "LotusFlowerCrisp",
+    "MintyMeatRolls",
+    "MondstadtHashBrown",
+    "MushroomPizza",
+    "NorthernSmokedChicken",
+    "SweetMadame",
+    ## Other ##
+    "CalxsArts",
+    "ChangingShifts",
+    "LeaveItToMe",
+    "Starsigns",
+
+    # Support Card
+    ## Companion ##
+    "Xudong",
+    ## Location ##
+
+    # Character Specific
+    ## Kaeya ##
+    "ColdBloodedStrike",
+    ## Keqing ##
+    "LightningStiletto",
+    "ThunderingPenance",
+    ## Rhodeia of Loch ##
+    "StreamingSurge",
+]
+
+############################## base ##############################
 
 
 class Card:
     _DICE_COST = AbstractDices({Element.OMNI: BIG_INT})
 
     @classmethod
     def effects(
@@ -147,25 +205,27 @@
             pid: PID,
     ) -> None | acg.ActionGenerator:
         return None
 
     def __eq__(self, other: object) -> bool:
         return type(self) == type(other)
 
-    def __str__(self) -> str:
+    def __repr__(self) -> str:
         return self.__class__.__name__
 
     @staticmethod
     def is_combat_action() -> bool:
         return False
 
     @classmethod
     def name(cls) -> str:
         return cls.__name__
 
+############################## helpers functions ##############################
+
 
 class _UsableFuncs:
     @staticmethod
     def active_combat_talent_skill_card_usable(
             game_state: gs.GameState,
             pid: PID,
             char: type[chr.Character]
@@ -203,19 +263,163 @@
             instruction: act.StaticTargetInstruction,
     ) -> bool:
         return instruction.target.pid == pid \
             and instruction.target.zone is ZONE.CHARACTERS \
             and instruction.target.id == game_state.get_player(pid).get_characters().get_active_character_id()
 
 
+class _DiceOnlyChoiceProvider(Card):
+    @classmethod
+    def _choices_helper(
+            cls,
+            action_generator: acg.ActionGenerator,
+    ) -> GivenChoiceType:
+        game_state = action_generator.game_state
+        pid = action_generator.pid
+
+        assert action_generator._action_filled()
+
+        instruction = action_generator.instruction
+        assert type(instruction) is act.DiceOnlyInstruction
+        if instruction.dices is None:
+            return cls.preprocessed_dice_cost(game_state, pid)[1]
+
+        raise Exception(
+            "Not Reached! Should be called when there is something to fill. action_generator:\n"
+            + f"{action_generator}"
+        )
+
+    @classmethod
+    def _fill_helper(
+        cls,
+        action_generator: acg.ActionGenerator,
+        player_choice: DecidedChoiceType,
+    ) -> acg.ActionGenerator:
+        assert action_generator._action_filled()
+
+        instruction = action_generator.instruction
+        assert type(instruction) is act.DiceOnlyInstruction
+        if instruction.dices is None:
+            assert isinstance(player_choice, ActualDices)
+            return replace(
+                action_generator,
+                instruction=replace(instruction, dices=player_choice),
+            )
+
+        raise Exception("Not Reached!")
+
+    @override
+    @classmethod
+    def action_generator(
+            cls,
+            game_state: gs.GameState,
+            pid: PID,
+    ) -> None | acg.ActionGenerator:
+        if not cls.strictly_usable(game_state, pid):
+            return None
+        return acg.ActionGenerator(
+            game_state=game_state,
+            pid=pid,
+            action=replace(act.CardAction._all_none(), card=cls),
+            instruction=act.DiceOnlyInstruction._all_none(),
+            _choices_helper=cls._choices_helper,
+            _fill_helper=cls._fill_helper,
+        )
+
+
+class _CharTargetChoiceProvider(Card):
+    @classmethod
+    def _valid_char(cls, char: chr.Character) -> bool:
+        return not char.defeated()
+
+    @classmethod
+    def _choices_helper(
+            cls,
+            action_generator: acg.ActionGenerator,
+    ) -> GivenChoiceType:
+        game_state = action_generator.game_state
+        pid = action_generator.pid
+
+        assert action_generator._action_filled()
+
+        instruction = action_generator.instruction
+        assert type(instruction) is act.StaticTargetInstruction
+        if instruction.target is None:
+            chars = game_state.get_player(pid).get_characters()
+            chars = [char for char in chars if cls._valid_char(char)]
+            return tuple(
+                StaticTarget(
+                    pid=pid,
+                    zone=ZONE.CHARACTERS,
+                    id=char.get_id(),
+                )
+                for char in chars
+            )
+
+        elif instruction.dices is None:
+            return cls.preprocessed_dice_cost(game_state, pid)[1]
+
+        raise Exception(
+            "Not Reached! Should be called when there is something to fill. action_generator:\n"
+            + f"{action_generator}"
+        )
+
+    @classmethod
+    def _fill_helper(
+        cls,
+        action_generator: acg.ActionGenerator,
+        player_choice: DecidedChoiceType,
+    ) -> acg.ActionGenerator:
+        assert action_generator._action_filled()
+
+        instruction = action_generator.instruction
+        assert isinstance(instruction, act.StaticTargetInstruction)
+        if instruction.target is None:
+            assert isinstance(player_choice, StaticTarget)
+            return replace(
+                action_generator,
+                instruction=replace(instruction, target=player_choice),
+            )
+
+        elif instruction.dices is None:
+            assert isinstance(player_choice, ActualDices)
+            return replace(
+                action_generator,
+                instruction=replace(instruction, dices=player_choice),
+            )
+
+        raise Exception("Not Reached!")
+
+    @override
+    @classmethod
+    def action_generator(
+            cls,
+            game_state: gs.GameState,
+            pid: PID,
+    ) -> None | acg.ActionGenerator:
+        if not cls.strictly_usable(game_state, pid):
+            return None
+        return acg.ActionGenerator(
+            game_state=game_state,
+            pid=pid,
+            action=replace(act.CardAction._all_none(), card=cls),
+            instruction=act.StaticTargetInstruction._all_none(),
+            _choices_helper=cls._choices_helper,
+            _fill_helper=cls._fill_helper,
+        )
+
+############################## special card ##############################
+
+
 class OmniCard(Card):
     """ the card used to hide opponent's cards """
     pass
 
 
+############################## type card ##############################
 class _CombatActionCard(Card):
     @override
     @staticmethod
     def is_combat_action() -> bool:
         return True
 
 
@@ -369,160 +573,14 @@
     pass
 
 
 class LocationCard(SupportCard):
     pass
 
 
-# <<<<<<<<<<<<<<<<<<<< Helpers <<<<<<<<<<<<<<<<<<<<
-class _DiceOnlyChoiceProvider(Card):
-    @classmethod
-    def _choices_helper(
-            cls,
-            action_generator: acg.ActionGenerator,
-    ) -> GivenChoiceType:
-        game_state = action_generator.game_state
-        pid = action_generator.pid
-
-        assert action_generator._action_filled()
-
-        instruction = action_generator.instruction
-        assert type(instruction) is act.DiceOnlyInstruction
-        if instruction.dices is None:
-            return cls.preprocessed_dice_cost(game_state, pid)[1]
-
-        raise Exception(
-            "Not Reached! Should be called when there is something to fill. action_generator:\n"
-            + f"{action_generator}"
-        )
-
-    @classmethod
-    def _fill_helper(
-        cls,
-        action_generator: acg.ActionGenerator,
-        player_choice: DecidedChoiceType,
-    ) -> acg.ActionGenerator:
-        assert action_generator._action_filled()
-
-        instruction = action_generator.instruction
-        assert type(instruction) is act.DiceOnlyInstruction
-        if instruction.dices is None:
-            assert isinstance(player_choice, ActualDices)
-            return replace(
-                action_generator,
-                instruction=replace(instruction, dices=player_choice),
-            )
-
-        raise Exception("Not Reached!")
-
-    @override
-    @classmethod
-    def action_generator(
-            cls,
-            game_state: gs.GameState,
-            pid: PID,
-    ) -> None | acg.ActionGenerator:
-        if not cls.strictly_usable(game_state, pid):
-            return None
-        return acg.ActionGenerator(
-            game_state=game_state,
-            pid=pid,
-            action=replace(act.CardAction._all_none(), card=cls),
-            instruction=act.DiceOnlyInstruction._all_none(),
-            _choices_helper=cls._choices_helper,
-            _fill_helper=cls._fill_helper,
-        )
-
-
-class _CharTargetChoiceProvider(Card):
-    @classmethod
-    def _valid_char(cls, char: chr.Character) -> bool:
-        return not char.defeated()
-
-    @classmethod
-    def _choices_helper(
-            cls,
-            action_generator: acg.ActionGenerator,
-    ) -> GivenChoiceType:
-        game_state = action_generator.game_state
-        pid = action_generator.pid
-
-        assert action_generator._action_filled()
-
-        instruction = action_generator.instruction
-        assert type(instruction) is act.StaticTargetInstruction
-        if instruction.target is None:
-            chars = game_state.get_player(pid).get_characters()
-            chars = [char for char in chars if cls._valid_char(char)]
-            return tuple(
-                StaticTarget(
-                    pid=pid,
-                    zone=ZONE.CHARACTERS,
-                    id=char.get_id(),
-                )
-                for char in chars
-            )
-
-        elif instruction.dices is None:
-            return cls.preprocessed_dice_cost(game_state, pid)[1]
-
-        raise Exception(
-            "Not Reached! Should be called when there is something to fill. action_generator:\n"
-            + f"{action_generator}"
-        )
-
-    @classmethod
-    def _fill_helper(
-        cls,
-        action_generator: acg.ActionGenerator,
-        player_choice: DecidedChoiceType,
-    ) -> acg.ActionGenerator:
-        assert action_generator._action_filled()
-
-        instruction = action_generator.instruction
-        assert isinstance(instruction, act.StaticTargetInstruction)
-        if instruction.target is None:
-            assert isinstance(player_choice, StaticTarget)
-            return replace(
-                action_generator,
-                instruction=replace(instruction, target=player_choice),
-            )
-
-        elif instruction.dices is None:
-            assert isinstance(player_choice, ActualDices)
-            return replace(
-                action_generator,
-                instruction=replace(instruction, dices=player_choice),
-            )
-
-        raise Exception("Not Reached!")
-
-    @override
-    @classmethod
-    def action_generator(
-            cls,
-            game_state: gs.GameState,
-            pid: PID,
-    ) -> None | acg.ActionGenerator:
-        if not cls.strictly_usable(game_state, pid):
-            return None
-        return acg.ActionGenerator(
-            game_state=game_state,
-            pid=pid,
-            action=replace(act.CardAction._all_none(), card=cls),
-            instruction=act.StaticTargetInstruction._all_none(),
-            _choices_helper=cls._choices_helper,
-            _fill_helper=cls._fill_helper,
-        )
-# >>>>>>>>>>>>>>>>>>>> Helpers >>>>>>>>>>>>>>>>>>>>
-
-# <<<<<<<<<<<<<<<<<<<< Event Cards <<<<<<<<<<<<<<<<<<<<
-# <<<<<<<<<<<<<<<<<<<< Event Cards / Food Cards <<<<<<<<<<<<<<<<<<<<
-
-
 class FoodCard(EventCard):
     @override
     @classmethod
     def _loosely_usable(cls, game_state: gs.GameState, pid: PID) -> bool:
         characters = game_state.get_player(pid).get_characters()
         if all(not cls._valid_char(char) for char in characters):
             return False
@@ -588,30 +646,16 @@
     @override
     @classmethod
     def _valid_char(cls, char: chr.Character) -> bool:
         return char.get_hp() < char.get_max_hp() \
             and super()._valid_char(char)
 
 
-class SweetMadame(_DirectHealCard, _CharTargetChoiceProvider):
-    _DICE_COST = AbstractDices({})
-
-    @override
-    @classmethod
-    def heal_amount(cls) -> int:
-        return 1
-
-
-class MondstadtHashBrown(_DirectHealCard, _CharTargetChoiceProvider):
-    _DICE_COST = AbstractDices({Element.OMNI: 1})
-
-    @override
-    @classmethod
-    def heal_amount(cls) -> int:
-        return 2
+# <<<<<<<<<<<<<<<<<<<< Event Cards <<<<<<<<<<<<<<<<<<<<
+# <<<<<<<<<<<<<<<<<<<< Event Cards / Food Cards <<<<<<<<<<<<<<<<<<<<
 
 
 class JueyunGuoba(FoodCard, _CharTargetChoiceProvider):
     _DICE_COST = AbstractDices({})
 
     @override
     @classmethod
@@ -651,14 +695,23 @@
             eft.AddCharacterStatusEffect(
                 target=instruction.target,
                 status=stt.MintyMeatRollsStatus,
             ),
         )
 
 
+class MondstadtHashBrown(_DirectHealCard, _CharTargetChoiceProvider):
+    _DICE_COST = AbstractDices({Element.OMNI: 1})
+
+    @override
+    @classmethod
+    def heal_amount(cls) -> int:
+        return 2
+
+
 class MushroomPizza(FoodCard, _CharTargetChoiceProvider):
     """
     Heal first then the status
     """
 
     _DICE_COST = AbstractDices({Element.OMNI: 1})
 
@@ -693,61 +746,25 @@
         return (
             eft.AddCharacterStatusEffect(
                 instruction.target,
                 stt.NorthernSmokedChickenStatus,
             ),
         )
 
-# >>>>>>>>>>>>>>>>>>>> Event Cards / Food Cards >>>>>>>>>>>>>>>>>>>>
 
-
-class Starsigns(EventCard, _DiceOnlyChoiceProvider):
-    _DICE_COST = AbstractDices({Element.ANY: 2})
-
-    @override
-    @classmethod
-    def _loosely_usable(cls, game_state: gs.GameState, pid: PID) -> bool:
-        """ Check active character doesn't have full energy """
-        active_character = game_state.get_player(pid).get_active_character()
-        if active_character is None or active_character.get_energy() >= active_character.get_max_energy():
-            return False
-        return super()._loosely_usable(game_state, pid)
+class SweetMadame(_DirectHealCard, _CharTargetChoiceProvider):
+    _DICE_COST = AbstractDices({})
 
     @override
     @classmethod
-    def _valid_instruction(
-            cls,
-            game_state: gs.GameState,
-            pid: PID,
-            instruction: act.Instruction
-    ) -> bool:
-        """ Check target is active character and .loosely_usable() """
-        if not isinstance(instruction, act.DiceOnlyInstruction):
-            return False
+    def heal_amount(cls) -> int:
+        return 1
 
-        return cls.loosely_usable(game_state, pid)
 
-    @override
-    @classmethod
-    def effects(
-            cls,
-            game_state: gs.GameState,
-            pid: PID,
-            instruction: act.Instruction,
-    ) -> tuple[eft.Effect, ...]:
-        return (
-            eft.EnergyRechargeEffect(
-                StaticTarget(
-                    pid=pid,
-                    zone=ZONE.CHARACTERS,
-                    id=game_state.get_player(pid).just_get_active_character().get_id(),
-                ),
-                1
-            ),
-        )
+# >>>>>>>>>>>>>>>>>>>> Event Cards / Food Cards >>>>>>>>>>>>>>>>>>>>
 
 
 class CalxsArts(EventCard, _DiceOnlyChoiceProvider):
     _DICE_COST = AbstractDices({Element.OMNI: 1})
 
     @override
     @classmethod
@@ -830,14 +847,60 @@
         return (
             eft.AddCombatStatusEffect(
                 target_pid=pid,
                 status=stt.LeaveItToMeStatus,
             ),
         )
 
+
+class Starsigns(EventCard, _DiceOnlyChoiceProvider):
+    _DICE_COST = AbstractDices({Element.ANY: 2})
+
+    @override
+    @classmethod
+    def _loosely_usable(cls, game_state: gs.GameState, pid: PID) -> bool:
+        """ Check active character doesn't have full energy """
+        active_character = game_state.get_player(pid).get_active_character()
+        if active_character is None or active_character.get_energy() >= active_character.get_max_energy():
+            return False
+        return super()._loosely_usable(game_state, pid)
+
+    @override
+    @classmethod
+    def _valid_instruction(
+            cls,
+            game_state: gs.GameState,
+            pid: PID,
+            instruction: act.Instruction
+    ) -> bool:
+        """ Check target is active character and .loosely_usable() """
+        if not isinstance(instruction, act.DiceOnlyInstruction):
+            return False
+
+        return cls.loosely_usable(game_state, pid)
+
+    @override
+    @classmethod
+    def effects(
+            cls,
+            game_state: gs.GameState,
+            pid: PID,
+            instruction: act.Instruction,
+    ) -> tuple[eft.Effect, ...]:
+        return (
+            eft.EnergyRechargeEffect(
+                StaticTarget(
+                    pid=pid,
+                    zone=ZONE.CHARACTERS,
+                    id=game_state.get_player(pid).just_get_active_character().get_id(),
+                ),
+                1
+            ),
+        )
+
 # >>>>>>>>>>>>>>>>>>>> Event Cards >>>>>>>>>>>>>>>>>>>>
 
 # <<<<<<<<<<<<<<<<<<<< Support Cards <<<<<<<<<<<<<<<<<<<<
 # <<<<<<<<<<<<<<<<<<<< Support Cards / Companion Cards <<<<<<<<<<<<<<<<<<<<
 
 
 class Xudong(CompanionCard):
@@ -856,14 +919,62 @@
                 support=sp.XudongSupport,
             ),
         )
 
 # >>>>>>>>>>>>>>>>>>>> Support Cards / Companion Cards >>>>>>>>>>>>>>>>>>>>
 # >>>>>>>>>>>>>>>>>>>> Support Cards >>>>>>>>>>>>>>>>>>>>
 
+#### Kaeya ####
+
+
+class ColdBloodedStrike(EquipmentCard, _CombatActionCard, _DiceOnlyChoiceProvider):
+    _DICE_COST = AbstractDices({Element.CRYO: 4})
+
+    @override
+    @classmethod
+    def _loosely_usable(cls, game_state: gs.GameState, pid: PID) -> bool:
+        return _UsableFuncs.active_combat_talent_skill_card_usable(game_state, pid, chr.Kaeya) \
+            and super()._loosely_usable(game_state, pid)
+
+    @override
+    @classmethod
+    def _valid_instruction(
+            cls,
+            game_state: gs.GameState,
+            pid: PID,
+            instruction: act.Instruction
+    ) -> bool:
+        return isinstance(instruction, act.DiceOnlyInstruction) \
+            and cls._loosely_usable(game_state, pid)
+
+    @override
+    @classmethod
+    def effects(
+            cls,
+            game_state: gs.GameState,
+            pid: PID,
+            instruction: act.Instruction,
+    ) -> tuple[eft.Effect, ...]:
+        assert isinstance(instruction, act.DiceOnlyInstruction)
+        target = StaticTarget(
+            pid=pid,
+            zone=ZONE.CHARACTERS,
+            id=game_state.get_player(pid).just_get_active_character().get_id(),
+        )
+        return (
+            eft.AddCharacterStatusEffect(
+                target=target,
+                status=stt.ColdBloodedStrikeStatus,
+            ),
+            eft.CastSkillEffect(
+                target=target,
+                skill=CharacterSkill.ELEMENTAL_SKILL1,
+            ),
+        )
+
 #### Keqing ####
 
 
 class LightningStiletto(EventCard, _CombatActionCard, _CharTargetChoiceProvider):
     _DICE_COST = AbstractDices({Element.ELECTRO: 3})
 
     @override
@@ -961,62 +1072,14 @@
             ),
             eft.CastSkillEffect(
                 target=target,
                 skill=CharacterSkill.ELEMENTAL_SKILL1,
             ),
         )
 
-#### Kaeya ####
-
-
-class ColdBloodedStrike(EquipmentCard, _CombatActionCard, _DiceOnlyChoiceProvider):
-    _DICE_COST = AbstractDices({Element.CRYO: 4})
-
-    @override
-    @classmethod
-    def _loosely_usable(cls, game_state: gs.GameState, pid: PID) -> bool:
-        return _UsableFuncs.active_combat_talent_skill_card_usable(game_state, pid, chr.Kaeya) \
-            and super()._loosely_usable(game_state, pid)
-
-    @override
-    @classmethod
-    def _valid_instruction(
-            cls,
-            game_state: gs.GameState,
-            pid: PID,
-            instruction: act.Instruction
-    ) -> bool:
-        return isinstance(instruction, act.DiceOnlyInstruction) \
-            and cls._loosely_usable(game_state, pid)
-
-    @override
-    @classmethod
-    def effects(
-            cls,
-            game_state: gs.GameState,
-            pid: PID,
-            instruction: act.Instruction,
-    ) -> tuple[eft.Effect, ...]:
-        assert isinstance(instruction, act.DiceOnlyInstruction)
-        target = StaticTarget(
-            pid=pid,
-            zone=ZONE.CHARACTERS,
-            id=game_state.get_player(pid).just_get_active_character().get_id(),
-        )
-        return (
-            eft.AddCharacterStatusEffect(
-                target=target,
-                status=stt.ColdBloodedStrikeStatus,
-            ),
-            eft.CastSkillEffect(
-                target=target,
-                skill=CharacterSkill.ELEMENTAL_SKILL1,
-            ),
-        )
-
 
 #### Rhodeia of Loch ####
 
 class StreamingSurge(EquipmentCard, _CombatActionCard, _DiceOnlyChoiceProvider):
     _DICE_COST = AbstractDices({Element.HYDRO: 4})
 
     @override
@@ -1056,10 +1119,7 @@
                 status=stt.StreamingSurgeStatus,
             ),
             eft.CastSkillEffect(
                 target=target,
                 skill=CharacterSkill.ELEMENTAL_BURST,
             ),
         )
-
-
-########### type ##########
```

### Comparing `dgisim-0.1.dev0/src/dgisim/card/cards_set.py` & `dgisim-0.2.dev0/dgisim/src/card/cards_set.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 from .card import *
 
-DEFAULT_CARDS: frozenset[type[Card]] = frozenset({
-    Starsigns,
-    # Food
-    JueyunGuoba,
-    LotusFlowerCrisp,
-    NorthernSmokedChicken,
-    SweetMadame,
-    MondstadtHashBrown,
-    MushroomPizza,
-    MintyMeatRolls,
-})
+__all__ = [
+    "default_cards",
+]
 
 _DEFAULT_CARDS: list[type[Card]] = [
     # Equipment Card
     ThunderingPenance,
     ColdBloodedStrike,
     StreamingSurge,
```

### Comparing `dgisim-0.1.dev0/src/dgisim/character/character.py` & `dgisim-0.2.dev0/dgisim/src/character/character.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+This file contains the base class Character for all characters,
+and implementation of all characters. (in alphabetic order)
+"""
 from __future__ import annotations
 from typing import Callable, Optional, TYPE_CHECKING, Union
 from typing_extensions import override
 from functools import lru_cache
 
 from ..card import card as cd
 from ..effect import effect as eft
@@ -9,23 +13,31 @@
 from ..status import statuses as stts
 from ..summon import summon as sm
 
 from ..dices import AbstractDices
 from ..effect.effects_template import *
 from ..effect.enums import ZONE, DYNAMIC_CHARACTER_TARGET
 from ..effect.structs import StaticTarget, DamageType
-from ..element.element import *
-from ..helper.level_print import INDENT, level_print
+from ..element import *
 from ..state.enums import PID
-
-from .character_skill_enum import CharacterSkill
+from .enums import CharacterSkill
 
 if TYPE_CHECKING:
     from ..state.game_state import GameState
 
+__all__ = [
+    # base
+    "Character",
+
+    # concretes
+    "Kaeya",
+    "Keqing",
+    "RhodeiaOfLoch",
+]
+
 class Character:
     _ELEMENT = Element.ANY
 
     def __init__(
         self,
         id: int,
         hp: int,
@@ -283,31 +295,14 @@
         if not isinstance(other, type(self)):
             return False
         return self._all_unique_data() == other._all_unique_data()
 
     def __hash__(self) -> int:
         return hash(self._all_unique_data())
 
-    def __str__(self) -> str:
-        return self.to_string(0)
-
-    def to_string(self, indent: int) -> str:
-        new_indent = indent + INDENT
-        return level_print({
-            "id": str(self._id),
-            "Aura": str(self._aura),
-            "HP": str(self._hp),
-            "Max HP": str(self._max_hp),
-            "Energy": str(self._energy),
-            "Max Energy": str(self._max_energy),
-            "Talents": str(self._talents),
-            "Equipments": str(self._equipments),
-            "Statuses": str(self._statuses),
-        }, indent)
-
     def dict_str(self) -> Union[dict, str]:
         return {
             "id": str(self._id),
             "Aura": str(self._aura),
             "HP": str(self._hp),
             "Max HP": str(self._max_hp),
             "Energy": str(self._energy),
@@ -441,15 +436,15 @@
                     stt.KeqingTalentStatus(can_infuse=False),
                 )
             )
 
         cards = game_state.get_player(source.pid).get_hand_cards()
         if not can_infuse and cards.contains(cd.LightningStiletto):
             effects.append(
-                eft.RemoveAllCardEffect(
+                eft.PublicRemoveAllCardEffect(
                     source.pid,
                     cd.LightningStiletto,
                 )
             )
             can_infuse = True
 
         if can_infuse:
@@ -470,15 +465,15 @@
                         status=stt.KeqingElectroInfusionStatus(
                             usages=self.BASE_ELECTRO_INFUSION_DURATION
                         ),
                     )
                 )
         else:
             effects.append(
-                eft.AddCardEffect(
+                eft.PublicAddCardEffect(
                     pid=source.pid,
                     card=cd.LightningStiletto,
                 )
             )
 
         return tuple(effects)
 
@@ -581,15 +576,15 @@
                 target=DYNAMIC_CHARACTER_TARGET.OPPO_ACTIVE,
                 element=Element.CRYO,
                 damage=1,
                 damage_type=DamageType(elemental_burst=True),
             ),
             eft.OverrideCombatStatusEffect(
                 target_pid=source.pid,
-                status=stt.Icicle(),
+                status=stt.IcicleStatus(),
             )
         )
 
     @classmethod
     def from_default(cls, id: int = -1) -> Kaeya:
         return cls(
             id=id,
```

### Comparing `dgisim-0.1.dev0/src/dgisim/character/character_skill_enum.py` & `dgisim-0.2.dev0/dgisim/src/character/enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from enum import Enum
 
-from ..event.event import EventType
+from ..event import EventType
+
+__all__ = [
+    "CharacterSkill",
+]
+
 
 class CharacterSkill(Enum):
     NORMAL_ATTACK = 0
     ELEMENTAL_BURST = 1
     ELEMENTAL_SKILL1 = 2
     ELEMENTAL_SKILL2 = 3
 
@@ -13,8 +18,8 @@
             return EventType.NORMAL_ATTACK
         elif self is CharacterSkill.ELEMENTAL_SKILL1:
             return EventType.ELEMENTAL_SKILL1
         elif self is CharacterSkill.ELEMENTAL_SKILL2:
             return EventType.ELEMENTAL_SKILL2
         elif self is CharacterSkill.ELEMENTAL_BURST:
             return EventType.ELEMENTAL_BURST
-        raise NotImplementedError
+        raise NotImplementedError
```

### Comparing `dgisim-0.1.dev0/src/dgisim/character/characters.py` & `dgisim-0.2.dev0/dgisim/src/character/characters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 from typing import Callable, Iterator, Optional, TYPE_CHECKING, Union
 
-from ..helper.level_print import level_print, INDENT
-
 if TYPE_CHECKING:
     from .character import Character
 
+__all__ = [
+    "Characters",
+]
 
 class Characters:
     def __init__(self, characters: tuple[Character, ...], active_character_id: Optional[int]):
         self._characters = characters
         self._active_character_id = active_character_id
 
     @classmethod
@@ -112,17 +113,14 @@
         if not isinstance(other, Characters):
             return False
         return self._all_unique_data() == other._all_unique_data()
 
     def __hash__(self) -> int:
         return hash(self._all_unique_data())
 
-    def __str__(self) -> str:
-        return self.to_string(0)
-
     def __iter__(self) -> Iterator[Character]:
         return iter(self.get_characters())
 
     def contains(self, char: Character | type[Character]) -> bool:
         if isinstance(char, Character):
             return any(
                 c == char
@@ -133,25 +131,14 @@
                 type(c) is char
                 for c in self._characters
             )
 
     def __contains__(self, char: Character | type[Character]) -> bool:
         return self.contains(char)
 
-    def to_string(self, indent: int = 0) -> str:
-        new_indent = indent + INDENT
-        new_new_indent = new_indent + INDENT
-        return level_print({
-            "Active Character": self.get_active_character_name(),
-            "Characters": level_print(dict([
-                (char.name(), char.to_string(new_new_indent))
-                for char in self._characters
-            ]), new_indent),
-        }, indent)
-
     def dict_str(self) -> Union[dict, str]:
         return {
             "Active Character": self.get_active_character_name(),
             "Characters": dict([
                 (char.name(), char.dict_str())
                 for char in self._characters
             ]),
```

### Comparing `dgisim-0.1.dev0/src/dgisim/dices.py` & `dgisim-0.2.dev0/dgisim/src/dices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from __future__ import annotations
 import random
-from enum import Enum
-from typing import Optional, Iterator, Iterable, TypeVar, Union
+from collections import Counter
+from typing import Any, Optional, Iterator, Iterable, TypeVar, Union
 from typing_extensions import Self, override, TYPE_CHECKING
 
 from .helper.hashable_dict import HashableDict
-from .helper.level_print import level_print
 from .helper.quality_of_life import BIG_INT
-from .element.element import Element
+from .element import Element
 
 if TYPE_CHECKING:
     from .state.game_state import GameState
 
+__all__ = [
+    "AbstractDices",
+    "ActualDices",
+    "Dices",
+]
+
 
 class Dices:
+    """
+    Base class for dices
+    """
     _LEGAL_ELEMS = frozenset(elem for elem in Element)
 
     def __init__(self, dices: dict[Element, int]) -> None:
         self._dices = HashableDict(dices)
 
     def __add__(self, other: Dices | dict[Element, int]) -> Self:
         dices: dict[Element, int]
@@ -50,59 +58,83 @@
             for elem, n in self._dices.items()
             if elem in self._LEGAL_ELEMS
         ))
 
     def elems(self) -> Iterable[Element]:
         return self._dices.keys()
 
+    def pick_random_dices(self, num: int) -> tuple[Self, Self]:
+        """
+        Returns the left dices and selected dices
+        """
+        num = min(self.num_dices(), num)
+        if num == 0:
+            return (self, type(self).from_empty())
+        picked_dices: dict[Element, int] = dict(Counter(
+            random.sample(list(self._dices.keys()), counts=self._dices.values(), k=num)
+        ))
+        return type(self)(self._dices - picked_dices), type(self)(picked_dices)
+
     def __contains__(self, elem: Element) -> bool:
         return (
             elem in self._LEGAL_ELEMS
             and self[elem] > 0
         )
 
     def __iter__(self) -> Iterator[Element]:
         return (
             elem
             for elem in self._dices
             if self[elem] > 0
         )
 
     def __getitem__(self, index: Element) -> int:
-        if index in self._dices:
-            return self._dices[index]
-        return 0
+        return self._dices.get(index, 0)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Dices):
             return False
         return self._dices == other._dices
 
     def __hash__(self) -> int:
         return hash(self._dices)
 
-    def __str__(self) -> str:
-        return self.to_string(0)
-
-    def to_string(self, indent: int = 0) -> str:
+    def __repr__(self) -> str:
         existing_dices = dict([
             (dice.name, str(num))
             for dice, num in self._dices.items()
             if num != 0
         ])
-        return level_print(existing_dices, indent)
+        return (
+            '{'
+            + ", ".join(
+                f"{key}: {val}"
+                for key, val in existing_dices.items()
+            )
+            + '}'
+        )
 
-    def dict_str(self) -> Union[dict, str]:
+    def to_dict(self) -> dict[Element, int]:
+        return dict(self._dices.items())
+
+    def dict_str(self) -> dict[str, Any]:
         existing_dices = dict([
             (dice.name, str(num))
             for dice, num in self._dices.items()
             if num != 0
         ])
         return existing_dices
 
+    @classmethod
+    def from_empty(cls) -> Self:
+        return cls(dict([
+            (elem, 0)
+            for elem in cls._LEGAL_ELEMS
+        ]))
+
 
 _PURE_ELEMS = frozenset({
     Element.PYRO,
     Element.HYDRO,
     Element.ANEMO,
     Element.ELECTRO,
     Element.DENDRO,
@@ -122,15 +154,14 @@
         Element.ANEMO,
         Element.ELECTRO,
         Element.DENDRO,
         Element.CRYO,
         Element.GEO,
     })
 
-
     def _satisfy(self, requirement: AbstractDices) -> bool:
         assert self.is_legal() and requirement.is_legal()
 
         # satisfy all pure elements first
         pure_deducted = HashableDict((
             (elem, self[elem] - requirement[elem])
             for elem in _PURE_ELEMS
@@ -237,21 +268,14 @@
         if omni_required > 0:
             if remaining[Element.OMNI] < omni_required:
                 return None
             answer[Element.OMNI] += omni_required
         return ActualDices(answer)
 
     @classmethod
-    def from_empty(cls) -> ActualDices:
-        return ActualDices(dict([
-            (elem, 0)
-            for elem in ActualDices._LEGAL_ELEMS
-        ]))
-
-    @classmethod
     def from_random(cls, size: int) -> ActualDices:
         dices = ActualDices.from_empty()
         dices._dices._unfreeze()
         for i in range(size):
             elem = random.choice(tuple(ActualDices._LEGAL_ELEMS))
             dices._dices[elem] += 1
         dices._dices.freeze()
```

### Comparing `dgisim-0.1.dev0/src/dgisim/effect/effect.py` & `dgisim-0.2.dev0/dgisim/src/effect/effect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,166 @@
+"""
+This file contains the base class "Effect" for all effects,
+and implementation of all effects.
+
+The classes are divided into 5 sections ordered. Within each section, they are
+ordered alphabetically.
+
+- base class, which is Effect
+- type classes, used to identify what type of effect an effect is
+- phase classes, effects that controls the flow of the game
+- concrete classes, the implementation of effects that are actually in the game
+"""
 from __future__ import annotations
 from dataclasses import asdict, dataclass, field, replace
 from typing import FrozenSet, Iterable, Optional, TYPE_CHECKING, Union
 
 from ..character import character as chr
+from ..helper.quality_of_life import dataclass_repr
 from ..status import status as stt
 from ..summon import summon as sm
 from ..support import support as sp
 
-from ..character.character_skill_enum import CharacterSkill
-from ..element.element import Element, Reaction, ReactionDetail
+from ..character.enums import CharacterSkill
+from ..element import Element, Reaction, ReactionDetail
 from ..helper.quality_of_life import just, case_val
 from ..state.enums import PID, ACT
 from ..status.enums import PREPROCESSABLES
 from ..status.status_processing import StatusProcessing
-
 from .enums import DYNAMIC_CHARACTER_TARGET, TRIGGERING_SIGNAL, ZONE
 from .structs import StaticTarget, DamageType
 
 if TYPE_CHECKING:
     from ..card.card import Card
     from ..dices import ActualDices
     from ..state.game_state import GameState
     from ..status.statuses import Statuses
 
+__all__ = [
+    # base
+    "Effect",
+
+    # type
+    "CheckerEffect",
+    "DirectEffect",
+    "PhaseEffect",
+    "TriggerrbleEffect",
+
+    # Triggerrable Effect
+    "AllStatusTriggererEffect",
+    "TriggerStatusEffect",
+    "TriggerCombatStatusEffect",
+    "TriggerSummonEffect",
+    "TriggerSupportEffect",
+
+    # Phase Effect
+    "DeathSwapPhaseStartEffect",
+    "DeathSwapPhaseEndEffect",
+    "EndPhaseCheckoutEffect",
+    "EndRoundEffect",
+    "TurnEndEffect",
+    "SetBothPlayerPhaseEffect",
+
+    # Checker Effect
+    "SwapCharacterCheckerEffect",
+    "DeathCheckCheckerEffect",
+    "DefeatedCheckerEffect",
+
+    # Direct Effect
+    "SwapCharacterEffect",
+    "ForwardSwapCharacterEffect",
+    "SpecificDamageEffect",
+    "ReferredDamageEffect",
+    "EnergyRechargeEffect",
+    "EnergyDrainEffect",
+    "RecoverHPEffect",
+    "PublicAddCardEffect",
+    "PublicRemoveCardEffect",
+    "PublicRemoveAllCardEffect",
+    "RemoveDiceEffect",
+    "AddCharacterStatusEffect",
+    "RemoveCharacterStatusEffect",
+    "UpdateCharacterStatusEffect",
+    "OverrideCharacterStatusEffect",
+    "AddCombatStatusEffect",
+    "RemoveCombatStatusEffect",
+    "UpdateCombatStatusEffect",
+    "OverrideCombatStatusEffect",
+    "AddSummonEffect",
+    "RemoveSummonEffect",
+    "UpdateSummonEffect",
+    "OverrideSummonEffect",
+    "AllSummonIncreaseUsage",
+    "OneSummonIncreaseUsage",
+    "AddSupportEffect",
+    "RemoveSupportEffect",
+    "UpdateSupportEffect",
+    "OverrideSupportEffect",
+    "CastSkillEffect",
+    "BroadCastSkillInfoEffect",
+]
+
+############################## base ##############################
 
-@dataclass(frozen=True)
+
+@dataclass(frozen=True, repr=False)
 class Effect:
     def execute(self, game_state: GameState) -> GameState:
         raise Exception("Not Overriden or Implemented")
 
     def name(self) -> str:
         return self.__class__.__name__
 
     def dict_str(self) -> Union[dict, str]:
         return asdict(self)
 
-    def __str__(self) -> str:
-        return self.__class__.__name__
+    def __repr__(self) -> str:
+        return dataclass_repr(self)
 
 
-@dataclass(frozen=True)
+############################## type ##############################
+@dataclass(frozen=True, repr=False)
 class TriggerrbleEffect(Effect):
     pass
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class DirectEffect(Effect):
     pass
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class CheckerEffect(Effect):
     pass
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class PhaseEffect(Effect):
     pass
 
+############################## Triggerrable Effect ##############################
+
+
+@dataclass(frozen=True, repr=False)
+class AllStatusTriggererEffect(TriggerrbleEffect):
+    """
+    This effect triggers the characters' statuses with the provided signal in order.
+    """
+    pid: PID
+    signal: TRIGGERING_SIGNAL
 
-@dataclass(frozen=True)
-class TriggerStatusEffect(Effect):
+    def execute(self, game_state: GameState) -> GameState:
+        effects = StatusProcessing.trigger_all_statuses_effects(game_state, self.pid, self.signal)
+        return game_state.factory().f_effect_stack(
+            lambda es: es.push_many_fl(effects)
+        ).build()
+
+
+@dataclass(frozen=True, repr=False)
+class TriggerStatusEffect(TriggerrbleEffect):
     target: StaticTarget
     status: type[Union[stt.CharacterTalentStatus, stt.EquipmentStatus, stt.CharacterStatus]]
     signal: TRIGGERING_SIGNAL
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
         if not isinstance(character, chr.Character):
@@ -85,16 +181,16 @@
             return game_state
         effects = status.react_to_signal(game_state, self.target, self.signal)
         return game_state.factory().f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
-@dataclass(frozen=True)
-class TriggerCombatStatusEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class TriggerCombatStatusEffect(TriggerrbleEffect):
     target_pid: PID  # the player the status belongs to
     status: type[stt.CombatStatus]
     signal: TRIGGERING_SIGNAL
 
     def execute(self, game_state: GameState) -> GameState:
         effects: Iterable[Effect] = []
         statuses = game_state.get_player(self.target_pid).get_combat_statuses()
@@ -111,16 +207,16 @@
             self.signal,
         )
         return game_state.factory().f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
-@dataclass(frozen=True)
-class TriggerSummonEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class TriggerSummonEffect(TriggerrbleEffect):
     target_pid: PID
     summon: type[sm.Summon]
     signal: TRIGGERING_SIGNAL
 
     def execute(self, game_state: GameState) -> GameState:
         effects: Iterable[Effect] = []
         summons = game_state.get_player(self.target_pid).get_summons()
@@ -137,16 +233,16 @@
             self.signal,
         )
         return game_state.factory().f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
-@dataclass(frozen=True)
-class TriggerSupportEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class TriggerSupportEffect(TriggerrbleEffect):
     target_pid: PID
     support_type: type[sp.Support]
     sid: int
     signal: TRIGGERING_SIGNAL
 
     def execute(self, game_state: GameState) -> GameState:
         effects: Iterable[Effect] = []
@@ -163,124 +259,23 @@
             ),
             self.signal,
         )
         return game_state.factory().f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
+############################## Phase Effect ##############################
 
-@dataclass(frozen=True)
-class AllStatusTriggererEffect(TriggerrbleEffect):
-    """
-    This effect triggers the characters' statuses with the provided signal in order.
-    """
-    pid: PID
-    signal: TRIGGERING_SIGNAL
-
-    def execute(self, game_state: GameState) -> GameState:
-        effects = StatusProcessing.trigger_all_statuses_effects(game_state, self.pid, self.signal)
-        return game_state.factory().f_effect_stack(
-            lambda es: es.push_many_fl(effects)
-        ).build()
-
-
-@dataclass(frozen=True)
-class SwapCharacterCheckerEffect(CheckerEffect):
-    my_active: StaticTarget
-    oppo_active: StaticTarget
 
-    def execute(self, game_state: GameState) -> GameState:
-        my_ac_id = game_state.get_player(self.my_active.pid).just_get_active_character().get_id()
-        oppo_ac_id = game_state.get_player(
-            self.oppo_active.pid).just_get_active_character().get_id()
-        my_pid = self.my_active.pid
-        effects: list[Effect] = []
-        if my_pid.is_player1():
-            my_signal = TRIGGERING_SIGNAL.SWAP_EVENT_1
-            oppo_signal = TRIGGERING_SIGNAL.SWAP_EVENT_2
-        else:
-            my_signal = TRIGGERING_SIGNAL.SWAP_EVENT_2
-            oppo_signal = TRIGGERING_SIGNAL.SWAP_EVENT_1
-        if my_ac_id != self.my_active.id:
-            effects += [
-                AllStatusTriggererEffect(
-                    pid=my_pid,
-                    signal=my_signal,
-                ),
-            ]
-        if oppo_ac_id != self.oppo_active.id:
-            effects += [
-                AllStatusTriggererEffect(
-                    pid=my_pid,
-                    signal=oppo_signal,
-                ),
-            ]
-        if not effects:
-            return game_state
-        return game_state.factory().f_effect_stack(
-            lambda es: es.push_many_fl(effects)
-        ).build()
-
-
-@dataclass(frozen=True)
-class DeathCheckCheckerEffect(CheckerEffect):
-    def execute(self, game_state: GameState) -> GameState:
-        p1_character = game_state.get_player1().get_characters().get_active_character()
-        p2_character = game_state.get_player2().get_characters().get_active_character()
-        assert p1_character is not None and p2_character is not None
-        pid: PID
-        if p1_character.defeated():
-            pid = PID.P1
-        elif p2_character.defeated():
-            pid = PID.P2
-        else:  # if no one defeated, continue
-            return game_state
-        death_swap_player = game_state.get_player(pid)
-        waiting_player = game_state.get_other_player(pid)
-        # TODO: check if game ends
-        if death_swap_player.defeated():
-            raise Exception("Not reached, should be caught by DefeatedCheckerEffect")
-        effects: list[Effect] = []
-        # TODO: trigger other death based effects
-        effects.append(DeathSwapPhaseStartEffect())
-        effects.append(DeathSwapPhaseEndEffect(
-            pid,
-            death_swap_player.get_phase(),
-            waiting_player.get_phase(),
-        ))
-        return game_state.factory().effect_stack(
-            game_state.get_effect_stack().push_many_fl(tuple(effects))
-        ).player(
-            pid,
-            game_state.get_player(pid).factory().phase(
-                ACT.ACTION_PHASE
-            ).build()
-        ).other_player(
-            pid,
-            game_state.get_other_player(pid).factory().phase(
-                ACT.PASSIVE_WAIT_PHASE
-            ).build()
-        ).build()
-
-
-@dataclass(frozen=True)
-class DefeatedCheckerEffect(CheckerEffect):
-    def execute(self, game_state: GameState) -> GameState:
-        if game_state.get_player1().defeated() \
-                or game_state.get_player2().defeated():
-            return game_state.factory().phase(game_state.get_mode().game_end_phase()).build()
-        return game_state
-
-
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class DeathSwapPhaseStartEffect(PhaseEffect):
     pass
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class DeathSwapPhaseEndEffect(PhaseEffect):
     my_pid: PID
     my_last_phase: ACT
     other_last_phase: ACT
 
     def execute(self, game_state: GameState) -> GameState:
         player = game_state.get_player(self.my_pid)
@@ -292,15 +287,15 @@
             player
         ).other_player(
             self.my_pid,
             other_player
         ).build()
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class EndPhaseCheckoutEffect(PhaseEffect):
     """
     This is responsible for triggering character statuses/summons/supports by the
     end of the round.
     """
 
     def execute(self, game_state: GameState) -> GameState:
@@ -314,15 +309,15 @@
             # TODO: add active_player's team status, summons status... here
         ]
         return game_state.factory().f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class EndRoundEffect(PhaseEffect):
     """
     This is responsible for triggering other clean ups (e.g. remove satiated)
     """
 
     def execute(self, game_state: GameState) -> GameState:
         active_id = game_state.get_active_player_id()
@@ -335,15 +330,15 @@
             # TODO: add active_player's team status, summons status... here
         ]
         return game_state.factory().f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class TurnEndEffect(PhaseEffect):
     def execute(self, game_state: GameState) -> GameState:
         active_player_id = game_state.get_active_player_id()
         player = game_state.get_player(active_player_id)
         other_player = game_state.get_other_player(active_player_id)
         assert player.get_phase() is ACT.ACTION_PHASE
         # TODO: other tidy up
@@ -356,45 +351,119 @@
             player.factory().phase(ACT.PASSIVE_WAIT_PHASE).build()
         ).other_player(
             active_player_id,
             other_player.factory().phase(ACT.ACTION_PHASE).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class EndPhaseTurnEndEffect(PhaseEffect):
-    def execute(self, game_state: GameState) -> GameState:
-        active_player_id = game_state.get_active_player_id()
-        player = game_state.get_player(active_player_id)
-        other_player = game_state.get_other_player(active_player_id)
-        assert player.get_phase().is_active_wait_phase()
-        return game_state.factory().active_player_id(
-            active_player_id.other()
-        ).player(
-            active_player_id,
-            player.factory().phase(ACT.PASSIVE_WAIT_PHASE).build()
-        ).other_player(
-            active_player_id,
-            other_player.factory().phase(ACT.ACTIVE_WAIT_PHASE).build()
-        ).build()
-
-
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class SetBothPlayerPhaseEffect(PhaseEffect):
     phase: ACT
 
     def execute(self, game_state: GameState) -> GameState:
         return game_state.factory().f_player1(
             lambda p: p.factory().phase(self.phase).build()
         ).f_player2(
             lambda p: p.factory().phase(self.phase).build()
         ).build()
 
+############################## Checker Effect ##############################
+
+
+@dataclass(frozen=True, repr=False)
+class SwapCharacterCheckerEffect(CheckerEffect):
+    my_active: StaticTarget
+    oppo_active: StaticTarget
+
+    def execute(self, game_state: GameState) -> GameState:
+        my_ac_id = game_state.get_player(self.my_active.pid).just_get_active_character().get_id()
+        oppo_ac_id = game_state.get_player(
+            self.oppo_active.pid).just_get_active_character().get_id()
+        my_pid = self.my_active.pid
+        effects: list[Effect] = []
+        if my_pid.is_player1():
+            my_signal = TRIGGERING_SIGNAL.SWAP_EVENT_1
+            oppo_signal = TRIGGERING_SIGNAL.SWAP_EVENT_2
+        else:
+            my_signal = TRIGGERING_SIGNAL.SWAP_EVENT_2
+            oppo_signal = TRIGGERING_SIGNAL.SWAP_EVENT_1
+        if my_ac_id != self.my_active.id:
+            effects += [
+                AllStatusTriggererEffect(
+                    pid=my_pid,
+                    signal=my_signal,
+                ),
+            ]
+        if oppo_ac_id != self.oppo_active.id:
+            effects += [
+                AllStatusTriggererEffect(
+                    pid=my_pid,
+                    signal=oppo_signal,
+                ),
+            ]
+        if not effects:
+            return game_state
+        return game_state.factory().f_effect_stack(
+            lambda es: es.push_many_fl(effects)
+        ).build()
+
+
+@dataclass(frozen=True, repr=False)
+class DeathCheckCheckerEffect(CheckerEffect):
+    def execute(self, game_state: GameState) -> GameState:
+        p1_character = game_state.get_player1().get_characters().get_active_character()
+        p2_character = game_state.get_player2().get_characters().get_active_character()
+        assert p1_character is not None and p2_character is not None
+        pid: PID
+        if p1_character.defeated():
+            pid = PID.P1
+        elif p2_character.defeated():
+            pid = PID.P2
+        else:  # if no one defeated, continue
+            return game_state
+        death_swap_player = game_state.get_player(pid)
+        waiting_player = game_state.get_other_player(pid)
+        # TODO: check if game ends
+        if death_swap_player.defeated():
+            raise Exception("Not reached, should be caught by DefeatedCheckerEffect")
+        effects: list[Effect] = []
+        # TODO: trigger other death based effects
+        effects.append(DeathSwapPhaseStartEffect())
+        effects.append(DeathSwapPhaseEndEffect(
+            pid,
+            death_swap_player.get_phase(),
+            waiting_player.get_phase(),
+        ))
+        return game_state.factory().effect_stack(
+            game_state.get_effect_stack().push_many_fl(tuple(effects))
+        ).player(
+            pid,
+            game_state.get_player(pid).factory().phase(
+                ACT.ACTION_PHASE
+            ).build()
+        ).other_player(
+            pid,
+            game_state.get_other_player(pid).factory().phase(
+                ACT.PASSIVE_WAIT_PHASE
+            ).build()
+        ).build()
+
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
+class DefeatedCheckerEffect(CheckerEffect):
+    def execute(self, game_state: GameState) -> GameState:
+        if game_state.get_player1().defeated() \
+                or game_state.get_player2().defeated():
+            return game_state.factory().phase(game_state.get_mode().game_end_phase()).build()
+        return game_state
+
+############################## Direct Effect ##############################
+
+
+@dataclass(frozen=True, repr=False)
 class SwapCharacterEffect(DirectEffect):
     target: StaticTarget
 
     def execute(self, game_state: GameState) -> GameState:
         assert self.target.zone == ZONE.CHARACTERS
         pid = self.target.pid
         player = game_state.get_player(pid)
@@ -417,15 +486,15 @@
                 lambda cs: cs.factory().active_character_id(self.target.id).build()
             ).build()
         ).f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class ForwardSwapCharacterEffect(DirectEffect):
     target_player: PID
 
     def execute(self, game_state: GameState) -> GameState:
         characters = game_state.get_player(self.target_player).get_characters()
         ordered_chars = characters.get_character_in_activity_order()
         next_char: Optional[chr.Character] = None
@@ -452,16 +521,16 @@
     Element.CRYO,
     Element.GEO,
     Element.PHYSICAL,
     Element.PIERCING,
 })
 
 
-@dataclass(frozen=True, kw_only=True)
-class SpecificDamageEffect(Effect):
+@dataclass(frozen=True, kw_only=True, repr=False)
+class SpecificDamageEffect(DirectEffect):
     source: StaticTarget
     target: StaticTarget
     element: Element
     damage: int
     damage_type: DamageType
     reaction: Optional[ReactionDetail] = None
 
@@ -660,16 +729,16 @@
                 lambda cs: cs.factory().character(target).build()
             ).build()
         ).f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
-@dataclass(frozen=True)
-class ReferredDamageEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class ReferredDamageEffect(DirectEffect):
     source: StaticTarget
     target: DYNAMIC_CHARACTER_TARGET
     element: Element
     damage: int
     damage_type: DamageType
     # this field is used as a reference if the target is OFF_FIELD
     # e.g. super-conduct caused by swirl
@@ -724,16 +793,16 @@
             )
 
         return game_state.factory().f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
-@dataclass(frozen=True)
-class EnergyRechargeEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class EnergyRechargeEffect(DirectEffect):
     target: StaticTarget
     recharge: int
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
         if not isinstance(character, chr.Character):
             return game_state
@@ -746,16 +815,16 @@
         player = player.factory().characters(characters).build()
         return game_state.factory().player(
             self.target.pid,
             player
         ).build()
 
 
-@dataclass(frozen=True)
-class EnergyDrainEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class EnergyDrainEffect(DirectEffect):
     target: StaticTarget
     drain: int
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
         if not isinstance(character, chr.Character):
             return game_state
@@ -768,16 +837,16 @@
         player = player.factory().characters(characters).build()
         return game_state.factory().player(
             self.target.pid,
             player
         ).build()
 
 
-@dataclass(frozen=True)
-class RecoverHPEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class RecoverHPEffect(DirectEffect):
     target: StaticTarget
     recovery: int
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
         if not isinstance(character, chr.Character):
             return game_state
@@ -791,56 +860,74 @@
                     character.get_id(),
                     lambda c: c.factory().hp(hp).build()
                 ).build()
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class RemoveCardEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class PublicAddCardEffect(DirectEffect):
+    pid: PID
+    card: type[Card]
+
+    def execute(self, game_state: GameState) -> GameState:
+        return game_state.factory().f_player(
+            self.pid,
+            lambda p: p.factory().f_hand_cards(
+                lambda cs: cs.add(self.card)
+            ).f_publicly_gained_cards(
+                lambda cs: cs.add(self.card)
+            ).build()
+        ).build()
+
+
+@dataclass(frozen=True, repr=False)
+class PublicRemoveCardEffect(DirectEffect):
     pid: PID
     card: type[Card]
 
     def execute(self, game_state: GameState) -> GameState:
         pid = self.pid
         card = self.card
         hand_cards = game_state.get_player(pid).get_hand_cards()
-        if not hand_cards.contains(card) or hand_cards[card] <= 0:
+        if not hand_cards.contains(card):
             return game_state
         return game_state.factory().f_player(
             pid,
             lambda p: p.factory().f_hand_cards(
                 lambda cs: cs.remove(card)
             ).f_publicly_used_cards(
                 lambda cs: cs.add(card)
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class RemoveAllCardEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class PublicRemoveAllCardEffect(DirectEffect):
     pid: PID
     card: type[Card]
 
     def execute(self, game_state: GameState) -> GameState:
         pid = self.pid
         card = self.card
         hand_cards = game_state.get_player(pid).get_hand_cards()
         if not hand_cards.contains(card) or hand_cards[card] <= 0:
             return game_state
         return game_state.factory().f_player(
             pid,
             lambda p: p.factory().f_hand_cards(
                 lambda cs: cs.remove_all(card)
+            ).f_publicly_used_cards(
+                lambda cs: cs + {card: hand_cards[card]}
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class RemoveDiceEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class RemoveDiceEffect(DirectEffect):
     pid: PID
     dices: ActualDices
 
     def execute(self, game_state: GameState) -> GameState:
         pid = self.pid
         dices = self.dices
         new_dices = game_state.get_player(pid).get_dices() - dices
@@ -848,16 +935,16 @@
             raise Exception("Not enough dices for this effect")
         return game_state.factory().f_player(
             pid,
             lambda p: p.factory().dices(new_dices).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class AddCharacterStatusEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class AddCharacterStatusEffect(DirectEffect):
     target: StaticTarget
     status: type[Union[stt.CharacterTalentStatus, stt.EquipmentStatus, stt.CharacterStatus]]
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
         assert isinstance(character, chr.Character)
         if issubclass(self.status, stt.CharacterTalentStatus):
@@ -876,15 +963,15 @@
             self.target.pid,
             lambda p: p.factory().f_characters(
                 lambda cs: cs.factory().character(character).build()
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class RemoveCharacterStatusEffect(DirectEffect):
     target: StaticTarget
     status: type[Union[stt.CharacterTalentStatus, stt.EquipmentStatus, stt.CharacterStatus]]
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_character_target(self.target)
         if character is None:
@@ -906,16 +993,16 @@
             self.target.pid,
             lambda p: p.factory().f_characters(
                 lambda cs: cs.factory().character(new_character).build()
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class UpdateCharacterStatusEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class UpdateCharacterStatusEffect(DirectEffect):
     target: StaticTarget
     status: Union[stt.CharacterTalentStatus, stt.EquipmentStatus, stt.CharacterStatus]
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
         assert isinstance(character, chr.Character)
         if isinstance(self.status, stt.CharacterTalentStatus):
@@ -934,16 +1021,16 @@
             self.target.pid,
             lambda p: p.factory().f_characters(
                 lambda cs: cs.factory().character(character).build()
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class OverrideCharacterStatusEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class OverrideCharacterStatusEffect(DirectEffect):
     target: StaticTarget
     status: Union[stt.CharacterTalentStatus, stt.EquipmentStatus, stt.CharacterStatus]
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
         assert isinstance(character, chr.Character)
         if isinstance(self.status, stt.CharacterTalentStatus):
@@ -962,128 +1049,128 @@
             self.target.pid,
             lambda p: p.factory().f_characters(
                 lambda cs: cs.factory().character(character).build()
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class AddCombatStatusEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class AddCombatStatusEffect(DirectEffect):
     target_pid: PID
     status: type[stt.CombatStatus]
 
     def execute(self, game_state: GameState) -> GameState:
         return game_state.factory().f_player(
             self.target_pid,
             lambda p: p.factory().f_combat_statuses(
                 lambda ss: ss.update_status(self.status())
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class RemoveCombatStatusEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class RemoveCombatStatusEffect(DirectEffect):
     target_pid: PID
     status: type[stt.CombatStatus]
 
     def execute(self, game_state: GameState) -> GameState:
         return game_state.factory().f_player(
             self.target_pid,
             lambda p: p.factory().f_combat_statuses(
                 lambda ss: ss.remove(self.status)
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class UpdateCombatStatusEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class UpdateCombatStatusEffect(DirectEffect):
     target_pid: PID
     status: stt.CombatStatus
 
     def execute(self, game_state: GameState) -> GameState:
         return game_state.factory().f_player(
             self.target_pid,
             lambda p: p.factory().f_combat_statuses(
                 lambda ss: ss.update_status(self.status)
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class OverrideCombatStatusEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class OverrideCombatStatusEffect(DirectEffect):
     target_pid: PID
     status: stt.CombatStatus
 
     def execute(self, game_state: GameState) -> GameState:
         return game_state.factory().f_player(
             self.target_pid,
             lambda p: p.factory().f_combat_statuses(
                 lambda ss: ss.update_status(self.status, override=True)
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class AddSummonEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class AddSummonEffect(DirectEffect):
     target_pid: PID
     summon: type[sm.Summon]
 
     def execute(self, game_state: GameState) -> GameState:
         return game_state.factory().f_player(
             self.target_pid,
             lambda p: p.factory().f_summons(
                 lambda ss: ss.update_summon(self.summon())
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class RemoveSummonEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class RemoveSummonEffect(DirectEffect):
     target_pid: PID
     summon: type[sm.Summon]
 
     def execute(self, game_state: GameState) -> GameState:
         return game_state.factory().f_player(
             self.target_pid,
             lambda p: p.factory().f_summons(
                 lambda ss: ss.remove_summon(self.summon)
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class UpdateSummonEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class UpdateSummonEffect(DirectEffect):
     target_pid: PID
     summon: sm.Summon
 
     def execute(self, game_state: GameState) -> GameState:
         return game_state.factory().f_player(
             self.target_pid,
             lambda p: p.factory().f_summons(
                 lambda ss: ss.update_summon(self.summon)
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class OverrideSummonEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class OverrideSummonEffect(DirectEffect):
     target_pid: PID
     summon: sm.Summon
 
     def execute(self, game_state: GameState) -> GameState:
         return game_state.factory().f_player(
             self.target_pid,
             lambda p: p.factory().f_summons(
                 lambda ss: ss.update_summon(self.summon, override=True)
             ).build()
         ).build()
 
 
-@dataclass(frozen=True, kw_only=True)
-class AllSummonIncreaseUsage(Effect):
+@dataclass(frozen=True, kw_only=True, repr=False)
+class AllSummonIncreaseUsage(DirectEffect):
     target_pid: PID
     d_usages: int = 1
 
     def execute(self, game_state: GameState) -> GameState:
         effects: list[Effect] = []
         summons = game_state.get_player(self.target_pid).get_summons()
         for summon in summons:
@@ -1094,16 +1181,16 @@
                 )
             )
         return game_state.factory().f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
-@dataclass(frozen=True, kw_only=True)
-class OneSummonIncreaseUsage(Effect):
+@dataclass(frozen=True, kw_only=True, repr=False)
+class OneSummonIncreaseUsage(DirectEffect):
     target_pid: PID
     summon_type: type[sm.Summon]
     d_usages: int = 1
 
     def execute(self, game_state: GameState) -> GameState:
         effects: list[Effect] = []
         summons = game_state.get_player(self.target_pid).get_summons()
@@ -1118,86 +1205,72 @@
             )
         )
         return game_state.factory().f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
-@dataclass(frozen=True)
-class AddSupportEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class AddSupportEffect(DirectEffect):
     target_pid: PID
     support: type[sp.Support]
 
     def execute(self, game_state: GameState) -> GameState:
         return game_state.factory().f_player(
             self.target_pid,
             lambda p: p.factory().f_supports(
                 lambda ss: ss.update_support(self.support(sid=ss.new_sid(self.support)))
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class RemoveSupportEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class RemoveSupportEffect(DirectEffect):
     target_pid: PID
     sid: int
 
     def execute(self, game_state: GameState) -> GameState:
         return game_state.factory().f_player(
             self.target_pid,
             lambda p: p.factory().f_supports(
                 lambda ss: ss.remove_by_sid(self.sid)
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class UpdateSupportEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class UpdateSupportEffect(DirectEffect):
     target_pid: PID
     support: sp.Support
 
     def execute(self, game_state: GameState) -> GameState:
         return game_state.factory().f_player(
             self.target_pid,
             lambda p: p.factory().f_supports(
                 lambda ss: ss.update_support(self.support)
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class OverrideSupportEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class OverrideSupportEffect(DirectEffect):
     target_pid: PID
     support: sp.Support
 
     def execute(self, game_state: GameState) -> GameState:
         return game_state.factory().f_player(
             self.target_pid,
             lambda p: p.factory().f_supports(
                 lambda ss: ss.update_support(self.support, override=True)
             ).build()
         ).build()
 
 
-@dataclass(frozen=True)
-class AddCardEffect(Effect):
-    pid: PID
-    card: type[Card]
-
-    def execute(self, game_state: GameState) -> GameState:
-        return game_state.factory().f_player(
-            self.pid,
-            lambda p: p.factory().f_hand_cards(
-                lambda cs: cs.add(self.card)
-            ).build()
-        ).build()
-
-
-@dataclass(frozen=True)
-class CastSkillEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class CastSkillEffect(DirectEffect):
     target: StaticTarget
     skill: CharacterSkill
 
     def execute(self, game_state: GameState) -> GameState:
         character = game_state.get_target(self.target)
         assert isinstance(character, chr.Character)
         if not character.can_cast_skill():
@@ -1206,16 +1279,16 @@
         if not effects:
             return game_state
         return game_state.factory().f_effect_stack(
             lambda es: es.push_many_fl(effects)
         ).build()
 
 
-@dataclass(frozen=True)
-class BroadCastSkillInfoEffect(Effect):
+@dataclass(frozen=True, repr=False)
+class BroadCastSkillInfoEffect(DirectEffect):
     source: StaticTarget
     skill: CharacterSkill
 
     def execute(self, game_state: GameState) -> GameState:
         return StatusProcessing.inform_all_statuses(
             game_state,
             self.source.pid,
```

### Comparing `dgisim-0.1.dev0/src/dgisim/effect/effect_stack.py` & `dgisim-0.2.dev0/dgisim/src/effect/effect_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from __future__ import annotations
 from typing import Iterable, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .effect import Effect
 
+__all__ = [
+    "EffectStack",
+]
+
 
 class EffectStack:
     def __init__(self, effects: tuple[Effect, ...]) -> None:
         self._effects = effects
 
     def is_not_empty(self) -> bool:
         return not self.is_empty()
```

### Comparing `dgisim-0.1.dev0/src/dgisim/effect/effects_template.py` & `dgisim-0.2.dev0/dgisim/src/effect/effects_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 from .enums import DYNAMIC_CHARACTER_TARGET
 from .structs import DamageType
 
 if TYPE_CHECKING:
     from .structs import StaticTarget
 
+__all__ = [
+    "normal_attack_template",
+]
+
 
 def normal_attack_template(
         source: StaticTarget,
         element: eft.Element,
         damage: int,
         dices_num: int,
 ) -> tuple[eft.Effect, ...]:
```

### Comparing `dgisim-0.1.dev0/src/dgisim/element/element.py` & `dgisim-0.2.dev0/dgisim/src/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,25 @@
+"""
+This file contains the enums and structs of elements and reactions.
+"""
 from __future__ import annotations
 from dataclasses import dataclass
 from enum import Enum
 from typing import FrozenSet, Optional, Iterator
 
-from ..helper.hashable_dict import HashableDict
+from .helper.hashable_dict import HashableDict
+
+__all__ = [
+    "AURA_ELEMENTS",
+    "AURA_ELEMENTS_ORDERED",
+    "Element",
+    "ElementalAura",
+    "Reaction",
+    "ReactionDetail",
+]
 
 
 class Element(Enum):
     OMNI = 0
     PYRO = 1
     HYDRO = 2
     ANEMO = 3
```

### Comparing `dgisim-0.1.dev0/src/dgisim/event/event.py` & `dgisim-0.2.dev0/dgisim/src/event.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from enum import Enum
 from typing import TYPE_CHECKING
 
-
 if TYPE_CHECKING:
-    from ..card.card import Card
-    from ..effect.structs import StaticTarget
-    from ..dices import AbstractDices
-    from ..state.enums import PID
+    from .card.card import Card
+    from .effect.structs import StaticTarget
+    from .dices import AbstractDices
+    from .state.enums import PID
+
+__all__ = [
+    "CardEvent",
+    "EventSpeed",
+    "EventType",
+    "GameEvent",
+]
+
 
 class EventSpeed(Enum):
     FAST_ACTION = "Fast-Action"
     COMBAT_ACTION = "Combat-Action"
 
 
 class EventType(Enum):
@@ -26,12 +33,13 @@
 @dataclass(frozen=True, kw_only=True)
 class GameEvent:
     target: StaticTarget
     event_type: EventType
     event_speed: EventSpeed
     dices_cost: AbstractDices
 
+
 @dataclass(frozen=True, kw_only=True)
 class CardEvent:
     pid: PID
     card_type: type[Card]
     dices_cost: AbstractDices
```

### Comparing `dgisim-0.1.dev0/src/dgisim/game_state_machine.py` & `dgisim-0.2.dev0/dgisim/src/game_state_machine.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,26 @@
 from .action.action import PlayerAction
 from .helper.level_print import GamePrinter
 from .phase.phase import Phase
 from .player_agent import PlayerAgent
 from .state.enums import PID
 from .state.game_state import GameState
 
+__all__ = [
+    "GameStateMachine",
+]
+
 
 class GameStateMachine:
     def __init__(self, game_state: GameState, player1: PlayerAgent, player2: PlayerAgent):
         self._history = [game_state]
+        self._perspective_history: dict[PID, list[GameState]] = {
+            PID.P1: [game_state.prespective_view(PID.P1)],
+            PID.P2: [game_state.prespective_view(PID.P2)],
+        }
         self._action_history: list[int] = []
         self._actions: dict[int, PlayerAction] = {}
         self._game_state = game_state
         self._playerAgent1 = player1
         self._playerAgent2 = player2
 
     @classmethod
@@ -77,33 +85,38 @@
 
     def next_index(self, index: int) -> int:
         return min(self.latest_index(), index + 1)
 
     def get_game_state_at(self, index: int) -> GameState:
         return self._history[index]
 
+    def _append_history(self, game_state: GameState) -> None:
+        self._history.append(self._game_state)
+        self._perspective_history[PID.P1].append(self._game_state.prespective_view(PID.P1))
+        self._perspective_history[PID.P2].append(self._game_state.prespective_view(PID.P2))
+
     def _step(self, observe=False) -> None:
         self._game_state = self._game_state.step()
         if observe:
             print(GamePrinter.dict_game_printer(self._game_state.dict_str()))
-            input(">>> ")
-        self._history.append(self._game_state)
+            input(":> ")
+        self._append_history(self._game_state)
 
     def _action_step(self, pid: PID, action: PlayerAction, observe=False) -> bool:
         next_state = self._game_state.action_step(pid, action)
         if next_state is None:
             return False
         action_idx = len(self._history) - 1
         self._action_history.append(action_idx)
         self._actions[action_idx] = action
         self._game_state = next_state
         if observe:
             print(GamePrinter.dict_game_printer(self._game_state.dict_str()))
             input(">>> ")
-        self._history.append(self._game_state)
+        self._append_history(self._game_state)
         return True
 
     def step_until_phase(self, phase: type[Phase] | Phase, observe=False) -> None:
         if isinstance(phase, Phase):
             phase = type(phase)
         while isinstance(self._game_state.get_phase(), phase):
             self.one_step(observe=observe)
@@ -130,15 +143,15 @@
         if pid is None:
             self._step(observe=observe)
         else:
             patience = 5
             while patience > 0 \
                     and not self._action_step(
                         pid,
-                        self.player_agent(pid).choose_action(self._history, pid),
+                        self.player_agent(pid).choose_action(self._perspective_history[pid], pid),
                         observe=observe,
                     ):
                 patience -= 1
 
     def changing_step(self, observe=False) -> None:
         game_state = self._game_state
         self.one_step(observe=observe)
```

### Comparing `dgisim-0.1.dev0/src/dgisim/helper/hashable_dict.py` & `dgisim-0.2.dev0/dgisim/src/helper/hashable_dict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import annotations
-from typing import Dict, Any
-from typing_extensions import override
+from typing import Any
+
+__all__ = [
+    "HashableDict"
+]
 
 
 class HashableDict(dict):
     """
     Inheritates dict but implements __hash__().
 
     In order to safely use __hash__(), there's a boolean property _frozen,
@@ -13,14 +16,17 @@
 
     If you want to create the HashableDict, make some modifications and then
     freeze it, add a keyword argument frozen=False when initializing, and call
     .freeze() later.
 
     You cannot call any setter, deleter or hash method of a frozen HashableDict.
     If you do so, Exception will be raised.
+
+    Note that though __add__ and __sub__ are overriden, but they are designed for
+    int values only!
     """
 
     def __init__(self, *args, frozen=True, **kwargs):
         """
         Used in the same way as dict.__init__().
 
         from_dict() is preferred when trying to copy a HashableDict than __init__().
@@ -66,32 +72,35 @@
         super().__delattr__(*args, **kwargs)
 
     def __delitem__(self, *args, **kwargs):
         if self.frozen():
             raise Exception("Calling __delitem__() to a frozen HashableDict!")
         super().__delitem__(*args, **kwargs)
 
-    def __add__(self, other: Dict[Any, int]):
+    def __add__(self, other: dict[Any, int]):
         keys = set(self.keys()).union(other.keys())
         return HashableDict(
             [(key, self.get(key, 0) + other.get(key, 0)) for key in keys]
         )
 
-    def __sub__(self, other: Dict[Any, int]):
+    def __sub__(self, other: dict[Any, int]):
         keys = set(self.keys()).union(other.keys())
         return HashableDict(
             [(key, self.get(key, 0) - other.get(key, 0)) for key in keys]
         )
 
     def __hash__(self) -> int:  # type: ignore
         """ Exception is raised if the HashableDict is not frozen. """
         if not self.frozen():
             raise Exception("Calling __hash__() to a non-frozen HashableDict!")
         return hash(frozenset(self.items()))
 
+    def all_val_non_negative(self) -> bool:
+        return all(val >= 0 for val in self.values())
+
     @classmethod
     def from_dict(cls, d: dict) -> HashableDict:
         """
         This method is preferred when trying to copy a HashableDict than __init__()
         """
         if isinstance(d, HashableDict) and d.frozen():
             return d
```

### Comparing `dgisim-0.1.dev0/src/dgisim/helper/level_print.py` & `dgisim-0.2.dev0/dgisim/src/helper/level_print.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from typing import Dict, Union
 
+__all__ = [
+    "GamePrinter",
+    "INDENT",
+    "StrDrawer",
+    "level_print",
+]
+
 _INDENTATION = "| "
 INDENT = len(_INDENTATION)
 
 
 def level_print(strs: Dict[str, str], indent: int = 0) -> str:
     indentation = _INDENTATION * (indent // INDENT)
     str_builder = []
@@ -53,15 +60,15 @@
         y_end = y + len(s)
         if y_end > self._lim_y:
             self._lim_y = y_end
         return (x, y_end)
 
     def insert_at_nextline(self, y: int, s: str) -> tuple[int, int]:
         return self.insert_at(self.lim_x() + 1, y, s)
-    
+
     def insert_board_at(self, x: int, y: int, other: StrDrawer) -> tuple[int, int]:
         max_x, max_y = 0, 0
         for insertion in other._insertions:
             nx, ny = self.insert_at(
                 insertion.x + x,
                 insertion.y + y,
                 insertion.s,
@@ -79,14 +86,15 @@
     def draw(self) -> str:
         board = [[' ' for j in range(self._lim_y + 1)] for i in range(self._lim_x + 1)]
         for insertion in self._insertions:
             for i, c in enumerate(insertion.s):
                 board[insertion.x][insertion.y + i] = c
         return '\n'.join(''.join(cs).rstrip() for cs in board)
 
+
 class GamePrinter:
 
     @staticmethod
     def _pair(d: dict, key: str) -> str:
         return "<" + key + ": " + str(d[key]) + ">"
 
     @staticmethod
@@ -180,14 +188,19 @@
             0,
             GamePrinter._insert_str_str_dict("Deck Cards", player["Deck Cards"]),
         )
         board.insert_board_at_nextline(
             0,
             GamePrinter._insert_str_str_dict("Publicly Used Cards", player["Publicly Used Cards"]),
         )
+        board.insert_board_at_nextline(
+            0,
+            GamePrinter._insert_str_str_dict(
+                "Publicly Gained Cards", player["Publicly Gained Cards"]),
+        )
         return board
 
     @staticmethod
     def _insert_effect(name: str, effect: Union[dict, str]) -> StrDrawer:
         board = StrDrawer()
         board.insert_at(0, 0, f"<{name}>")
         if type(effect) is str:
@@ -195,15 +208,15 @@
                 board.insert_at_nextline(2, f"<{effect}>")
         else:
             assert type(effect) is dict
             for field, content in effect.items():
                 content = ''.join(c for c in str(content) if c != '\n')
                 board.insert_at_nextline(2, f"<{field}: {content}>")
         return board
-    
+
     @staticmethod
     def _insert_effects(name: str, effects: dict) -> StrDrawer:
         board = StrDrawer()
         board.insert_at(0, 0, f"<{name}>")
         es = []
         for effect in effects:
             es.append(GamePrinter._insert_effect(effect, effects[effect]))
@@ -228,15 +241,15 @@
         p2_board = GamePrinter._insert_player(
             f"{'*' if not p1_active else ''}Player2",
             game_state["Player2"]
         )
         player_row_start = 2
         board.insert_board_at(player_row_start, 0, p1_board)
         px, py = board.insert_board_at(player_row_start, p1_board.lim_y() + 4, p2_board)
-        for i in range(player_row_start, board.lim_x()+1):
+        for i in range(player_row_start, board.lim_x() + 1):
             board.insert_at(i, p1_board.lim_y() + 2, '|')
             board.insert_at(i, py + 2, '|')
         board.insert_at_nextline(0, "-" * (board.lim_y()))
         board.insert_at(1, 0, "-" * (board.lim_y()))
 
         board.insert_board_at_nextline(
             0,
```

### Comparing `dgisim-0.1.dev0/src/dgisim/phase/action_phase.py` & `dgisim-0.2.dev0/dgisim/src/phase/default/action_phase.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 from __future__ import annotations
 from typing import Optional, TYPE_CHECKING
 
-from ..phase import phase as ph
+from .. import phase as ph
 
-from ..action.action import *
-from ..effect.effect import *
-from ..event.event import *
-from ..state.enums import PID, ACT
+from ...action.action import *
+from ...action.action_generator import ActionGenerator
+from ...action.enums import ActionType
+from ...character.enums import CharacterSkill
+from ...effect.effect import *
+from ...effect.enums import TRIGGERING_SIGNAL, ZONE
+from ...effect.structs import StaticTarget
+from ...element import Element
+from ...event import *
+from ...helper.quality_of_life import just
+from ...state.enums import PID, ACT
 
 if TYPE_CHECKING:
-    from ..state.game_state import GameState
+    from ...action.types import DecidedChoiceType, GivenChoiceType
+    from ...state.game_state import GameState
+
+__all__ = [
+    "ActionPhase",
+]
 
 
 class ActionPhase(ph.Phase):
     def _start_up_phase(self, game_state: GameState) -> GameState:
         # TODO: Handle before action statuses
         active_player_id = game_state.get_active_player_id()
         return game_state.factory().player(
@@ -215,15 +227,15 @@
         new_dices = dices - paid_dices
         if not new_dices.is_legal():
             print(f"Fail with new dices: <{new_dices}> for card: {card.name()}")
             assert False
             return None
 
         # Card
-        new_effects.append(RemoveCardEffect(pid, card))
+        new_effects.append(PublicRemoveCardEffect(pid, card))
         new_effects += card.effects(game_state, pid, action.instruction)
         if card.is_combat_action():
             new_effects.append(AllStatusTriggererEffect(
                 pid,
                 TRIGGERING_SIGNAL.COMBAT_ACTION,
             ))
             new_effects.append(TurnEndEffect())
@@ -249,20 +261,23 @@
         if action.card not in cards \
                 or dices[action.dice_elem] == 0 \
                 or action.dice_elem is active_character_elem \
                 or dices[Element.OMNI] + dices[active_character_elem] == dices.num_dices():
             print(f"{action} cannot be performed in game state:\n{game_state}")
             assert False
             return None
+        from ...card.card import OmniCard
         return game_state.factory().f_player(
             pid,
             lambda p: p.factory().f_dices(
                 lambda ds: ds + {action.dice_elem: -1, active_character_elem: 1}
             ).f_hand_cards(
                 lambda hcs: hcs.remove(action.card)
+            ).f_publicly_used_cards(
+                lambda pucs: pucs.add(OmniCard)
             ).build()
         ).build()
 
     def _handle_death_swap_action(
             self,
             game_state: GameState,
             pid: PID,
@@ -313,33 +328,110 @@
             action: PlayerAction
     ) -> Optional[GameState]:
         # check action arrived at the right state
         if pid is not self.waiting_for(game_state):
             raise Exception(f"Unexpected action from {pid} at game state:\n{game_state}")
 
         # check death swap phase
-        effect_stack = game_state.get_effect_stack()
-        if effect_stack.is_not_empty() and isinstance(effect_stack.peek(), DeathSwapPhaseStartEffect):
+        if game_state.death_swapping(pid):
             if not isinstance(action, DeathSwapAction):
                 raise Exception(f"Trying to execute {action} when a death swap is expected")
             # game_state = game_state.factory().effect_stack(effect_stack.pop()[0]).build()
 
         if isinstance(action, GameAction):
             return self._handle_game_action(game_state, pid, action)
         elif isinstance(action, EndRoundAction):
             return self._handle_end_round(game_state, pid, action)
         raise Exception("Unknown Game State to process")
 
     def waiting_for(self, game_state: GameState) -> Optional[PID]:
         effect_stack = game_state.get_effect_stack()
         # if no effects are to be executed or death swap phase is inserted
-        if effect_stack.is_empty() \
-                or isinstance(effect_stack.peek(), DeathSwapPhaseStartEffect):
+        if effect_stack.is_empty() or game_state.death_swapping():
             return super().waiting_for(game_state)
         else:
             return None
 
+    @classmethod
+    def _choices_helper(cls, action_generator: ActionGenerator) -> GivenChoiceType:
+        game_state = action_generator.game_state
+        pid = action_generator.pid
+
+        # death swap check
+        if game_state.death_swapping(pid):
+            return (ActionType.SWAP_CHARACTER, )
+
+        choices: list[ActionType] = []
+
+        # cards
+        if game_state.card_checker().playable(pid):
+            choices.append(ActionType.PLAY_CARD)
+
+        # skills
+        if game_state.skill_checker().skillable(pid):
+            choices.append(ActionType.CAST_SKILL)
+
+        # swaps
+        if game_state.swap_checker().swappable(pid):
+            choices.append(ActionType.SWAP_CHARACTER)
+
+        # elemental tuning
+        if game_state.elem_tuning_checker().usable(pid):
+            choices.append(ActionType.ELEMENTAL_TUNING)
+
+        # unconditional end round
+        choices.append(ActionType.END_ROUND)
+        return tuple(choices)
+
+    @classmethod
+    def _fill_helper(
+        cls,
+        action_generator: ActionGenerator,
+        player_choice: DecidedChoiceType,
+    ) -> ActionGenerator:
+        game_state = action_generator.game_state
+        pid = action_generator.pid
+
+        if game_state.death_swapping(pid):
+            assert player_choice is ActionType.SWAP_CHARACTER
+            from ...action.action_generator_generator import SwapActGenGenerator
+            return just(SwapActGenGenerator.action_generator(game_state, pid))
+
+        if player_choice is ActionType.PLAY_CARD:
+            assert game_state.card_checker().playable(pid)
+            from ...action.action_generator_generator import CardActGenGenerator
+            return just(CardActGenGenerator.action_generator(game_state, pid))
+        elif player_choice is ActionType.SWAP_CHARACTER:
+            assert game_state.swap_checker().swappable(pid)
+            from ...action.action_generator_generator import SwapActGenGenerator
+            return just(SwapActGenGenerator.action_generator(game_state, pid))
+        elif player_choice is ActionType.CAST_SKILL:
+            assert game_state.skill_checker().skillable(pid)
+            from ...action.action_generator_generator import SkillActGenGenerator
+            return just(SkillActGenGenerator.action_generator(game_state, pid))
+        elif player_choice is ActionType.ELEMENTAL_TUNING:
+            assert game_state.elem_tuning_checker().usable(pid)
+            from ...action.action_generator_generator import ElemTuningActGenGenerator
+            return just(ElemTuningActGenGenerator.action_generator(game_state, pid))
+        elif player_choice is ActionType.END_ROUND:
+            return ActionGenerator(game_state=game_state, pid=pid, action=EndRoundAction())
+        else:
+            action_type_name = ActionType.__name__
+            if isinstance(player_choice, ActionType):
+                raise Exception(f"Unhandled player {action_type_name} {player_choice}")
+            else:
+                raise TypeError(f"Unexpected player choice {player_choice} where"
+                                + f"where {action_type_name} is expected")
+
+    def action_generator(self, game_state: GameState, pid: PID) -> ActionGenerator | None:
+        return ActionGenerator(
+            game_state=game_state,
+            pid=pid,
+            _choices_helper=self._choices_helper,
+            _fill_helper=self._fill_helper,
+        )
+
     def __eq__(self, other: object) -> bool:
         return isinstance(other, ActionPhase)
 
     def __hash__(self) -> int:
         return hash(self.__class__.__name__)
```

### Comparing `dgisim-0.1.dev0/src/dgisim/phase/end_phase.py` & `dgisim-0.2.dev0/dgisim/src/phase/default/end_phase.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 from __future__ import annotations
 from typing import Optional, TYPE_CHECKING
 
-from ..phase import phase as ph
+from .. import phase as ph
 
-from ..action.action import *
-from ..dices import ActualDices
-from ..effect.effect import *
-from ..state.enums import PID, ACT
+from ...action.action import *
+from ...action.action_generator import ActionGenerator
+from ...dices import ActualDices
+from ...effect.effect import *
+from ...effect.enums import ZONE
+from ...effect.structs import StaticTarget
+from ...state.enums import PID, ACT
 
 if TYPE_CHECKING:
-    from ..state.game_state import GameState
+    from ...action.types import DecidedChoiceType, GivenChoiceType
+    from ...state.game_state import GameState
+
+
+__all__ = [
+    "EndPhase",
+]
 
 
 class EndPhase(ph.Phase):
     _CARDS_DRAWN = 2
 
     def _initialize_end_phase(self, game_state: GameState) -> GameState:
         active_pid = game_state.get_active_player_id()
@@ -30,17 +39,21 @@
             lambda p: p.factory().phase(ACT.ACTIVE_WAIT_PHASE).build()
         ).build()
 
     def _to_roll_phase(self, game_state: GameState, new_round: int) -> GameState:
         active_player_id = game_state.get_active_player_id()
         active_player = game_state.get_player(active_player_id)
         other_player = game_state.get_other_player(active_player_id)
-        active_player_deck, new_cards = active_player.get_deck_cards().pick_random_cards(self._CARDS_DRAWN)
+        active_player_deck, new_cards = (
+            active_player.get_deck_cards().pick_random_cards(self._CARDS_DRAWN)
+        )
         active_player_hand = active_player.get_hand_cards() + new_cards
-        other_player_deck, new_cards = other_player.get_deck_cards().pick_random_cards(self._CARDS_DRAWN)
+        other_player_deck, new_cards = (
+            other_player.get_deck_cards().pick_random_cards(self._CARDS_DRAWN)
+        )
         other_player_hand = other_player.get_hand_cards() + new_cards
         return game_state.factory().round(
             new_round
         ).phase(
             game_state.get_mode().roll_phase()
         ).f_player(
             active_player_id,
@@ -111,32 +124,41 @@
             new_round = game_state.get_round() + 1
             if new_round > game_state.get_mode().round_limit():
                 return self._end_game(game_state)
             else:
                 return self._to_roll_phase(game_state, new_round)
         raise Exception("Unknown Game State to process")
 
-    def _handle_death_swap_action(self, game_state: GameState, pid: PID, action: DeathSwapAction) -> Optional[
-        GameState]:
+    def _handle_death_swap_action(
+            self,
+            game_state: GameState,
+            pid: PID,
+            action: DeathSwapAction
+    ) -> Optional[GameState]:
         player = game_state.get_player(pid)
         effect_stack = game_state.get_effect_stack()
         # Add Effects
         active_character = player.get_characters().get_active_character()
         assert active_character is not None
         effect_stack = effect_stack.push_one(SwapCharacterEffect(
             StaticTarget(pid, ZONE.CHARACTERS, action.char_id)
         ))
         return game_state.factory().effect_stack(
             effect_stack
         ).build()
 
-    def step_action(self, game_state: GameState, pid: PID, action: PlayerAction) -> Optional[
-        GameState]:
+    def step_action(
+            self,
+            game_state: GameState,
+            pid: PID,
+            action: PlayerAction
+    ) -> Optional[GameState]:
         effect_stack = game_state.get_effect_stack()
-        if effect_stack.is_not_empty() and isinstance(effect_stack.peek(), DeathSwapPhaseStartEffect):
+        if (effect_stack.is_not_empty()
+                and isinstance(effect_stack.peek(), DeathSwapPhaseStartEffect)):
             game_state = game_state.factory().effect_stack(effect_stack.pop()[0]).build()
         if isinstance(action, DeathSwapAction):
             return self._handle_death_swap_action(game_state, pid, action)
 
         raise NotImplementedError
 
     def waiting_for(self, game_state: GameState) -> Optional[PID]:
@@ -144,12 +166,17 @@
         # if no effects are to be executed or death swap phase is inserted
         if effect_stack.is_not_empty() \
                 and isinstance(effect_stack.peek(), DeathSwapPhaseStartEffect):
             return super().waiting_for(game_state)
         else:
             return None
 
+    def action_generator(self, game_state: GameState, pid: PID) -> ActionGenerator | None:
+        assert game_state.death_swapping(pid)
+        from ...action.action_generator_generator import SwapActGenGenerator
+        return SwapActGenGenerator.action_generator(game_state, pid)
+
     def __eq__(self, other: object) -> bool:
         return isinstance(other, EndPhase)
 
     def __hash__(self) -> int:
         return hash(self.__class__.__name__)
```

### Comparing `dgisim-0.1.dev0/src/dgisim/phase/phase.py` & `dgisim-0.2.dev0/dgisim/src/phase/default/game_end_phase.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 from __future__ import annotations
-from typing import Optional, TYPE_CHECKING
+from typing import TYPE_CHECKING
 
-from ..helper.level_print import level_print_single
+from .. import phase as ph
 
 if TYPE_CHECKING:
-    from ..state.game_state import GameState
-    from ..action.action import PlayerAction
-    from ..state.enums import PID
+    from ...action.action import PlayerAction
+    from ...action.action_generator import ActionGenerator
+    from ...state.game_state import GameState
+    from ...state.enums import PID
 
+__all__ = [
+    "GameEndPhase",
+]
 
-class Phase:
+
+class GameEndPhase(ph.Phase):
     def step(self, game_state: GameState) -> GameState:
-        raise Exception("Not Overriden")
+        raise Exception("Not Reached")
+
+    def step_action(self, game_state: GameState, pid: PID, action: PlayerAction) -> None | GameState:
+        raise Exception("Not Reached")
 
-    def step_action(self, game_state: GameState, pid: PID, action: PlayerAction) -> Optional[
-        GameState]:
-        raise Exception("Not Overriden")
-
-    def waiting_for(self, game_state: GameState) -> Optional[PID]:
-        players = [game_state.get_player1(), game_state.get_player2()]
-        for player in players:
-            if player.get_phase().is_action_phase():
-                return game_state.get_pid(player)
-        return None
+    def action_generator(self, game_state: GameState, pid: PID) -> None | ActionGenerator:
+        raise Exception("Not Reached")
 
     def __eq__(self, other: object) -> bool:
-        return isinstance(other, Phase)
+        return isinstance(other, GameEndPhase)
 
     def __hash__(self) -> int:
         return hash(self.__class__.__name__)
-
-    def __str__(self) -> str:
-        return self.to_string(0)
-
-    def to_string(self, indent: int = 0) -> str:
-        return level_print_single(self.__class__.__name__, indent)
-
-    def dict_str(self) -> dict | str:
-        return self.__class__.__name__
```

### Comparing `dgisim-0.1.dev0/src/dgisim/phase/roll_phase.py` & `dgisim-0.2.dev0/dgisim/src/phase/phase.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING
+from abc import abstractmethod
+from typing import Optional, TYPE_CHECKING
 
-from ..phase import phase as ph
-
-from ..dices import ActualDices
-from ..element.element import Element
-from ..state.enums import ACT
+from ..helper.level_print import level_print_single
 
 if TYPE_CHECKING:
     from ..state.game_state import GameState
+    from ..action.action import PlayerAction
+    from ..action.action_generator import ActionGenerator
+    from ..state.enums import PID
 
+__all__ = [
+    "Phase",
+]
 
-class RollPhase(ph.Phase):
-    _NUM_DICES = 8
-
-    def _get_all_omni_and_to_action_phase(self, game_state: GameState) -> GameState:
-        return game_state.factory().phase(
-            game_state.get_mode().action_phase()
-        ).player1(
-            game_state.get_player1().factory()
-            .phase(ACT.PASSIVE_WAIT_PHASE)
-            .dices(ActualDices.from_all(RollPhase._NUM_DICES, Element.OMNI))
-            # .dices(ActualDices.from_random(RollPhase._NUM_DICES))
-            .build()
-        ).player2(
-            game_state.get_player2().factory()
-            .phase(ACT.PASSIVE_WAIT_PHASE)
-            .dices(ActualDices.from_all(RollPhase._NUM_DICES, Element.OMNI))
-            # .dices(ActualDices.from_random(RollPhase._NUM_DICES))
-            .build()
-        ).build()
 
+class Phase:
+    @abstractmethod
     def step(self, game_state: GameState) -> GameState:
-        # if game_state.get_active_player().is_player1():
-        #     p1_phase = PlayerState.act.ACTIVE_WAIT_PHASE
-        #     p2_phase = PlayerState.act.PASSIVE_WAIT_PHASE
-        # elif game_state.get_active_player().is_player2():
-        #     p1_phase = PlayerState.act.PASSIVE_WAIT_PHASE
-        #     p2_phase = PlayerState.act.ACTIVE_WAIT_PHASE
-        # else:
-        #     raise Exception("Undefined Player id")
-        return self._get_all_omni_and_to_action_phase(game_state)
+        raise NotImplementedError
+
+    @abstractmethod
+    def step_action(self, game_state: GameState, pid: PID, action: PlayerAction) -> Optional[
+            GameState]:
+        raise NotImplementedError
+
+    def waiting_for(self, game_state: GameState) -> Optional[PID]:
+        players = [game_state.get_player1(), game_state.get_player2()]
+        for player in players:
+            if player.get_phase().is_action_phase():
+                return game_state.get_pid(player)
+        return None
+
+    @abstractmethod
+    def action_generator(self, game_state: GameState, pid: PID) -> None | ActionGenerator:
+        raise NotImplementedError
 
     def __eq__(self, other: object) -> bool:
-        return isinstance(other, RollPhase)
+        return isinstance(other, Phase)
 
     def __hash__(self) -> int:
         return hash(self.__class__.__name__)
+
+    def __str__(self) -> str:
+        return self.to_string(0)
+
+    def to_string(self, indent: int = 0) -> str:
+        return level_print_single(self.__class__.__name__, indent)
+
+    def dict_str(self) -> dict | str:
+        return self.__class__.__name__
```

### Comparing `dgisim-0.1.dev0/src/dgisim/state/enums.py` & `dgisim-0.2.dev0/dgisim/src/state/enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from __future__ import annotations
 from enum import Enum
 
+__all__ = [
+    "ACT",
+    "PID",
+]
+
+
 class PID(Enum):
     P1 = 1
     P2 = 2
 
     def is_player1(self) -> bool:
         return self is PID.P1
 
@@ -15,24 +21,25 @@
         if self is PID.P1:
             return PID.P2
         elif self is PID.P2:
             return PID.P1
         else:
             raise Exception("Unknown situation of pid")
 
+
 class ACT(Enum):
     ACTION_PHASE = "Action Phase"
     PASSIVE_WAIT_PHASE = "Passive Wait Phase"
     ACTIVE_WAIT_PHASE = "Aggressive Wait Phase"
     END_PHASE = "End Phase"
 
     def is_action_phase(self) -> bool:
         return self is ACT.ACTION_PHASE
 
     def is_passive_wait_phase(self) -> bool:
         return self is ACT.PASSIVE_WAIT_PHASE
 
     def is_active_wait_phase(self) -> bool:
         return self is ACT.ACTIVE_WAIT_PHASE
-    
+
     def is_end_phase(self) -> bool:
-        return self is ACT.END_PHASE
+        return self is ACT.END_PHASE
```

### Comparing `dgisim-0.1.dev0/src/dgisim/state/player_state.py` & `dgisim-0.2.dev0/dgisim/src/state/player_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,59 +4,68 @@
 from ..card import cards as cds
 from ..character import character as chr
 from ..status import statuses as sts
 from ..support import support as sp
 
 from ..character.characters import Characters
 from ..dices import ActualDices
-from ..helper.level_print import level_print, INDENT
 from ..summon.summons import Summons
 from ..support.supports import Supports
 
 from .enums import ACT
 
 if TYPE_CHECKING:
     from ..mode import Mode
 
+__all__ = [
+    "PlayerState",
+]
 
 class PlayerState:
     def __init__(
         self,
         phase: ACT,
         characters: Characters,
         combat_statuses: sts.Statuses,
         summons: Summons,
         supports: Supports,
         card_redraw_chances: int,
+        dice_reroll_chances: int,
         dices: ActualDices,
         hand_cards: cds.Cards,
         deck_cards: cds.Cards,
         publicly_used_cards: cds.Cards,
+        publicly_gained_cards: cds.Cards,
     ):
         # REMINDER: don't forget to update factory when adding new fields
         self._phase = phase
         self._card_redraw_chances = card_redraw_chances
+        self._dice_reroll_chances = dice_reroll_chances
         self._characters = characters
         self._combat_statuses = combat_statuses
         self._summons = summons
         self._supports = supports
         self._dices = dices
         self._hand_cards = hand_cards
         self._deck_cards = deck_cards
         self._publicly_used_cards = publicly_used_cards
+        self._publicly_gained_cards = publicly_gained_cards
 
     def factory(self) -> PlayerStateFactory:
         return PlayerStateFactory(self)
 
     def get_phase(self) -> ACT:
         return self._phase
 
     def get_card_redraw_chances(self) -> int:
         return self._card_redraw_chances
 
+    def get_dice_reroll_chances(self) -> int:
+        return self._dice_reroll_chances
+
     def get_characters(self) -> Characters:
         return self._characters
 
     def get_combat_statuses(self) -> sts.Statuses:
         return self._combat_statuses
 
     def get_summons(self) -> Summons:
@@ -73,14 +82,17 @@
 
     def get_deck_cards(self) -> cds.Cards:
         return self._deck_cards
 
     def get_publicly_used_cards(self) -> cds.Cards:
         return self._publicly_used_cards
 
+    def get_publicly_gained_cards(self) -> cds.Cards:
+        return self._publicly_gained_cards
+
     def get_active_character(self) -> Optional[chr.Character]:
         return self._characters.get_active_character()
 
     def just_get_active_character(self) -> chr.Character:
         return self._characters.just_get_active_character()
 
     def is_action_phase(self):
@@ -103,31 +115,40 @@
             return support == object
         else:
             raise NotImplementedError
 
     def defeated(self) -> bool:
         return self._characters.all_defeated()
 
+    def hide_cards(self) -> PlayerState:
+        return self.factory().f_hand_cards(
+            lambda hcs: hcs.hide_all()
+        ).f_deck_cards(
+            lambda dcs: dcs.hide_all()
+        ).build()
+
     @staticmethod
     def examplePlayer(mode: Mode):
         cards = mode.all_cards()
         chars = mode.all_chars()
         return PlayerState(
             phase=ACT.PASSIVE_WAIT_PHASE,
             card_redraw_chances=0,
+            dice_reroll_chances=0,
             characters=Characters.from_default(
                 tuple([char.from_default(i + 1) for i, char in enumerate(chars)][:3])
             ),
             combat_statuses=sts.Statuses(()),
             summons=Summons((), mode.summons_limit()),
             supports=Supports((), mode.supports_limit()),
-            hand_cards=cds.Cards(dict([(card, 0) for card in cards])),
             dices=ActualDices({}),
-            deck_cards=cds.Cards(dict([(card, 2) for card in cards])),
-            publicly_used_cards=cds.Cards(dict([(card, 0) for card in cards])),
+            hand_cards=cds.Cards({}),
+            deck_cards=cds.Cards(dict([(card, mode.max_cards_per_kind()) for card in cards])),
+            publicly_used_cards=cds.Cards({}),
+            publicly_gained_cards=cds.Cards({}),
         )
 
     def _all_unique_data(self) -> tuple:
         return (
             self._phase,
             self._card_redraw_chances,
             self._characters,
@@ -143,65 +164,63 @@
         if not isinstance(other, PlayerState):
             return False
         return self._all_unique_data() == other._all_unique_data()
 
     def __hash__(self) -> int:
         return hash(self._all_unique_data())
 
-    def __str__(self) -> str:
-        return self.to_string(0)
-
-    def to_string(self, indent: int = 0):
-        new_indent = indent + INDENT
-        return level_print({
-            "Phase": self._phase.value,
-            # "Card Redraw Chances": str(self._card_redraw_chances),
-            "Characters": self._characters.to_string(new_indent),
-            "Dices": self._dices.to_string(new_indent),
-            # "Hand Cards": self._hand_cards.to_string(new_indent),
-            # "Deck Cards": self._deck_cards.to_string(new_indent),
-            # "Publicly Used Cards": self._publicly_used_cards.to_string(new_indent),
-        }, indent)
-
     def dict_str(self) -> dict[str, Union[dict, str]]:
         return {
             "Phase": self._phase.value,
             "Card Redraw Chances": str(self._card_redraw_chances),
             "Characters": self._characters.dict_str(),
             "Combat Statuses": str(self._combat_statuses),
             "Summons": self._summons.dict_str(),
             "Supports": self._supports.dict_str(),
             "Dices": self._dices.dict_str(),
             "Hand Cards": self._hand_cards.dict_str(),
             "Deck Cards": self._deck_cards.dict_str(),
             "Publicly Used Cards": self._publicly_used_cards.dict_str(),
+            "Publicly Gained Cards": self._publicly_gained_cards.dict_str(),
         }
 
 
 class PlayerStateFactory:
     def __init__(self, player_state: PlayerState) -> None:
         self._phase = player_state.get_phase()
         self._card_redraw_chances = player_state.get_card_redraw_chances()
+        self._dice_reroll_chances = player_state.get_dice_reroll_chances()
         self._characters = player_state.get_characters()
         self._combat_statuses = player_state.get_combat_statuses()
         self._summons = player_state.get_summons()
         self._supports = player_state.get_supports()
-        self._hand_cards = player_state.get_hand_cards()
         self._dices = player_state.get_dices()
+        self._hand_cards = player_state.get_hand_cards()
         self._deck_cards = player_state.get_deck_cards()
         self._publicly_used_cards = player_state.get_publicly_used_cards()
+        self._publicly_gained_cards = player_state.get_publicly_gained_cards()
 
     def phase(self, phase: ACT) -> PlayerStateFactory:
         self._phase = phase
         return self
 
     def card_redraw_chances(self, chances: int) -> PlayerStateFactory:
         self._card_redraw_chances = chances
         return self
 
+    def f_card_redraw_chances(self, f: Callable[[int], int]) -> PlayerStateFactory:
+        return self.card_redraw_chances(f(self._card_redraw_chances))
+
+    def dice_reroll_chances(self, chances: int) -> PlayerStateFactory:
+        self._dice_reroll_chances = chances
+        return self
+
+    def f_dice_reroll_chances(self, f: Callable[[int], int]) -> PlayerStateFactory:
+        return self.dice_reroll_chances(f(self._dice_reroll_chances))
+
     def characters(self, characters: Characters) -> PlayerStateFactory:
         self._characters = characters
         return self
 
     def f_characters(self, f: Callable[[Characters], Characters]) -> PlayerStateFactory:
         self._characters = f(self._characters)
         return self
@@ -223,45 +242,57 @@
     def supports(self, supports: Supports) -> PlayerStateFactory:
         self._supports = supports
         return self
 
     def f_supports(self, f: Callable[[Supports], Supports]) -> PlayerStateFactory:
         return self.supports(f(self._supports))
 
-    def hand_cards(self, cards: cds.Cards) -> PlayerStateFactory:
-        self._hand_cards = cards
-        return self
-
-    def f_hand_cards(self, f: Callable[[cds.Cards], cds.Cards]) -> PlayerStateFactory:
-        return self.hand_cards(f(self._hand_cards))
-
     def dices(self, dices: ActualDices) -> PlayerStateFactory:
         self._dices = dices
         return self
 
     def f_dices(self, f: Callable[[ActualDices], ActualDices]) -> PlayerStateFactory:
         return self.dices(f(self._dices))
 
+    def hand_cards(self, cards: cds.Cards) -> PlayerStateFactory:
+        self._hand_cards = cards
+        return self
+
+    def f_hand_cards(self, f: Callable[[cds.Cards], cds.Cards]) -> PlayerStateFactory:
+        return self.hand_cards(f(self._hand_cards))
+
     def deck_cards(self, cards: cds.Cards) -> PlayerStateFactory:
         self._deck_cards = cards
         return self
 
+    def f_deck_cards(self, f: Callable[[cds.Cards], cds.Cards]) -> PlayerStateFactory:
+        return self.deck_cards(f(self._deck_cards))
+
     def publicly_used_cards(self, cards: cds.Cards) -> PlayerStateFactory:
         self._publicly_used_cards = cards
         return self
 
     def f_publicly_used_cards(self, f: Callable[[cds.Cards], cds.Cards]) -> PlayerStateFactory:
         return self.publicly_used_cards(f(self._publicly_used_cards))
 
+    def publicly_gained_cards(self, cards: cds.Cards) -> PlayerStateFactory:
+        self._publicly_gained_cards = cards
+        return self
+
+    def f_publicly_gained_cards(self, f: Callable[[cds.Cards], cds.Cards]) -> PlayerStateFactory:
+        return self.publicly_gained_cards(f(self._publicly_gained_cards))
+
     def build(self) -> PlayerState:
         return PlayerState(
             phase=self._phase,
             card_redraw_chances=self._card_redraw_chances,
+            dice_reroll_chances=self._dice_reroll_chances,
             characters=self._characters,
             combat_statuses=self._combat_statuses,
             summons=self._summons,
             supports=self._supports,
-            hand_cards=self._hand_cards,
             dices=self._dices,
+            hand_cards=self._hand_cards,
             deck_cards=self._deck_cards,
             publicly_used_cards=self._publicly_used_cards,
+            publicly_gained_cards=self._publicly_gained_cards,
         )
```

### Comparing `dgisim-0.1.dev0/src/dgisim/status/status.py` & `dgisim-0.2.dev0/dgisim/src/status/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,85 @@
+"""
+This file contains the base class "Status" for all statuses,
+and implementation of all statuses.
+
+The classes are divided into 4 sections ordered. Within each section, they are
+ordered alphabetically.
+
+- base class, which is Status
+- type classes, used to identify what type of status a status is
+- template classes, starting with an '_', are templates for other classes
+- concrete classes, the implementation of statuses that are actually in the game
+"""
 from __future__ import annotations
 from dataclasses import dataclass, replace
 from enum import Enum
 from math import ceil
 from typing import ClassVar, Optional, TYPE_CHECKING
 from typing_extensions import override, Self
 
 from ..effect import effect as eft
-from ..event import event as evt
 
-from ..character.character_skill_enum import CharacterSkill
+from ..character.enums import CharacterSkill
 from ..effect.enums import ZONE, TRIGGERING_SIGNAL, DYNAMIC_CHARACTER_TARGET
 from ..effect.structs import StaticTarget, DamageType
-from ..element.element import Element
+from ..element import Element
+from ..event import EventSpeed, EventType, GameEvent
 from ..helper.quality_of_life import just, BIG_INT, case_val
-
 from .enums import PREPROCESSABLES
 
 if TYPE_CHECKING:
     from ..card.card import Card
     from ..state.game_state import GameState
-
     from .types import Preprocessable
 
-
-class TriggerringEvent(Enum):
-    pass
+__all__ = [
+    # base
+    "Status",
+
+    # type
+    "CharacterTalentStatus",  # it should be statuses used to record character-talent related data
+    "EquipmentStatus",  # talent / weapon / artifact
+    "CharacterStatus",  # statues that belongs to one character only
+    "CombatStatus",  # statues that buffs the active character
+
+    # templates
+    "StackedShieldStatus",
+    "FixedShieldStatus",
+
+    # combat status
+    "CatalyzingFieldStatus",
+    "ChangingShiftsStatus",
+    "CrystallizeStatus",
+    "DendroCoreStatus",
+    "FrozenStatus",
+    "LeaveItToMeStatus",
+
+    # character status
+    "JueyunGuobaStatus",
+    "LotusFlowerCrispStatus",
+    "MintyMeatRollsStatus",
+    "MushroomPizzaStatus",
+    "NorthernSmokedChickenStatus",
+    "SatiatedStatus",
+
+    # character specific status
+    ## Kaeya ##
+    "ColdBloodedStrikeStatus",
+    "IcicleStatus",
+    ## Keqing ##
+    "KeqingElectroInfusionStatus",
+    "KeqingTalentStatus",
+    "ThunderingPenanceStatus",
+    ## Rhodeia of Loch ##
+    "StreamingSurgeStatus",
+]
 
 
+############################## base ##############################
 @dataclass(frozen=True)
 class Status:
 
     def __init__(self) -> None:
         if type(self) is Status:  # pragma: no cover
             raise Exception("class Status is not instantiable")
 
@@ -257,14 +306,15 @@
     def _update(self, other: Self) -> Optional[Self]:
         return other
 
     def __str__(self) -> str:
         return self.__class__.__name__.removesuffix("Status")  # pragma: no cover
 
 
+############################## type ##############################
 @dataclass(frozen=True)
 class CharacterTalentStatus(Status):
     """
     Basic status, describing character talents
     """
     pass
 
@@ -288,14 +338,15 @@
 class CombatStatus(Status):
     """
     Basic status, status shared across the team
     """
     pass
 
 
+############################## template ##############################
 @dataclass(frozen=True)
 class _UsageStatus(Status):
     usages: int
     MAX_USAGES: ClassVar[int] = BIG_INT
 
     @staticmethod
     def _auto_destroy() -> bool:
@@ -334,15 +385,15 @@
         return replace(self, usages=new_usages)
 
     def __str__(self) -> str:
         return super().__str__() + f"({self.usages})"  # pragma: no cover
 
 
 @dataclass(frozen=True)
-class ShieldStatus(Status):
+class _ShieldStatus(Status):
     def _is_target(
             self,
             game_state: GameState,
             status_source: StaticTarget,
             item: Preprocessable,
             signal: PREPROCESSABLES,
     ) -> bool:
@@ -370,15 +421,51 @@
             return item.target == attached_active_character
 
         else:
             raise NotImplementedError  # pragma: no cover
 
 
 @dataclass(frozen=True, kw_only=True)
-class StackedShieldStatus(ShieldStatus, _UsageStatus):
+class FixedShieldStatus(_ShieldStatus, _UsageStatus):
+    """ The shield status where only one usage can be consumed by a DMG effect """
+    usages: int
+    MAX_USAGES: ClassVar[int] = BIG_INT
+    SHIELD_AMOUNT: ClassVar[int] = 0  # shield amount per stack
+
+    def _trigerring_condition(self, damage: eft.SpecificDamageEffect) -> bool:
+        return True
+
+    @override
+    def _preprocess(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            item: Preprocessable,
+            signal: PREPROCESSABLES,
+    ) -> tuple[Preprocessable, Optional[Self]]:
+        cls = type(self)
+        if signal is PREPROCESSABLES.DMG_AMOUNT:
+            assert isinstance(item, eft.SpecificDamageEffect)
+            if item.damage > 0 and self.usages > 0 \
+                    and item.element != Element.PIERCING \
+                    and self._is_target(game_state, status_source, item, signal) \
+                    and self._trigerring_condition(item):
+                new_dmg = max(0, item.damage - cls.SHIELD_AMOUNT)
+                new_item = replace(item, damage=new_dmg)
+                new_usages = self.usages - 1
+                if self._auto_destroy() and new_usages == 0:
+                    return new_item, None
+                else:
+                    return new_item, replace(self, usages=new_usages)
+
+        return super()._preprocess(game_state, status_source, item, signal)
+
+
+@dataclass(frozen=True, kw_only=True)
+class StackedShieldStatus(_ShieldStatus, _UsageStatus):
     """ The shield status where all usages can be consumed by a DMG effect """
     usages: int
     MAX_USAGES: ClassVar[int] = BIG_INT
     SHIELD_AMOUNT: ClassVar[int] = 1  # shield amount per usage
 
     @override
     def _preprocess(
@@ -407,46 +494,130 @@
         return super()._preprocess(game_state, status_source, item, signal)
 
     def __str__(self) -> str:
         return super().__str__() + f"({self.usages})"  # pragma: no cover
 
 
 @dataclass(frozen=True, kw_only=True)
-class FixedShieldStatus(ShieldStatus, _UsageStatus):
-    """ The shield status where only one usage can be consumed by a DMG effect """
-    usages: int
+class _InfusionStatus(CharacterStatus, _UsageStatus):
     MAX_USAGES: ClassVar[int] = BIG_INT
-    SHIELD_AMOUNT: ClassVar[int] = 0  # shield amount per stack
-
-    def _trigerring_condition(self, damage: eft.SpecificDamageEffect) -> bool:
-        return True
+    ELEMENT: ClassVar[Optional[Element]] = None
+    damage_boost: int = 0
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
             item: Preprocessable,
             signal: PREPROCESSABLES,
     ) -> tuple[Preprocessable, Optional[Self]]:
-        cls = type(self)
+        assert self.ELEMENT is not None
+        new_item: Optional[eft.SpecificDamageEffect] = None
+        if isinstance(item, eft.SpecificDamageEffect):
+            if signal is PREPROCESSABLES.DMG_ELEMENT:
+                if self._dmg_element_condition(game_state, status_source, item):
+                    new_item = replace(item, element=self.ELEMENT)
+            if signal is PREPROCESSABLES.DMG_AMOUNT:
+                if self.damage_boost != 0  \
+                        and self._dmg_boost_condition(game_state, status_source, item):
+                    new_item = replace(item, damage=item.damage + self.damage_boost)
+        if new_item is not None:
+            return new_item, self
+        else:
+            return item, self
+
+    def _dmg_element_condition(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            item: eft.SpecificDamageEffect,
+    ) -> bool:
+        return item.element is Element.PHYSICAL \
+            and item.damage_type.normal_attack \
+            and status_source == item.source \
+
+
+    def _dmg_boost_condition(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            item: eft.SpecificDamageEffect,
+    ) -> bool:
+        return item.element is self.ELEMENT and status_source == item.source
+
+    @override
+    def _react_to_signal(
+            self, source: StaticTarget, signal: TRIGGERING_SIGNAL
+    ) -> tuple[list[eft.Effect], Optional[Self]]:
+        d_usages = 0
+        if signal is TRIGGERING_SIGNAL.ROUND_END:
+            d_usages = -1
+        return [], replace(self, usages=d_usages)
+
+
+@dataclass(frozen=True, kw_only=True)
+class ElectroInfusionStatus(_InfusionStatus):
+    ELEMENT: ClassVar[Optional[Element]] = Element.ELECTRO
+
+############################## Combat Status ##############################
+
+
+@dataclass(frozen=True)
+class CatalyzingFieldStatus(CombatStatus):
+    damage_boost: ClassVar[int] = 1
+    usages: int = 2
+
+    @override
+    def _preprocess(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            item: Preprocessable,
+            signal: PREPROCESSABLES,
+    ) -> tuple[Preprocessable, Optional[CatalyzingFieldStatus]]:
         if signal is PREPROCESSABLES.DMG_AMOUNT:
             assert isinstance(item, eft.SpecificDamageEffect)
-            if item.damage > 0 and self.usages > 0 \
-                    and item.element != Element.PIERCING \
-                    and self._is_target(game_state, status_source, item, signal) \
-                    and self._trigerring_condition(item):
-                new_dmg = max(0, item.damage - cls.SHIELD_AMOUNT)
-                new_item = replace(item, damage=new_dmg)
-                new_usages = self.usages - 1
-                if self._auto_destroy() and new_usages == 0:
-                    return new_item, None
+            assert self.usages >= 1
+            elem_can_boost = item.element is Element.ELECTRO or item.element is Element.DENDRO
+            legal_to_boost = status_source.pid is item.source.pid
+            target_is_active = item.target.id == game_state.get_player(
+                item.target.pid
+            ).just_get_active_character().get_id()
+            if elem_can_boost and legal_to_boost and target_is_active:
+                new_damage = replace(item, damage=item.damage + CatalyzingFieldStatus.damage_boost)
+                if self.usages == 1:
+                    return new_damage, None
                 else:
-                    return new_item, replace(self, usages=new_usages)
+                    return new_damage, CatalyzingFieldStatus(self.usages - 1)
+        return super()._preprocess(game_state, status_source, item, signal)
+
+    def __str__(self) -> str:
+        return super().__str__() + f"({self.usages})"  # pragma: no cover
+
 
+@dataclass(frozen=True)
+class ChangingShiftsStatus(CombatStatus):
+    COST_DEDUCTION: ClassVar[int] = 1
+
+    @override
+    def _preprocess(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            item: Preprocessable,
+            signal: PREPROCESSABLES,
+    ) -> tuple[Preprocessable, Optional[Self]]:
+        if signal is PREPROCESSABLES.SWAP:
+            assert isinstance(item, GameEvent) and item.event_type is EventType.SWAP
+            if item.target.pid is status_source.pid \
+                    and item.dices_cost.num_dices() >= self.COST_DEDUCTION:
+                assert item.dices_cost.num_dices() == item.dices_cost[Element.ANY]
+                new_cost = (item.dices_cost - {Element.ANY: self.COST_DEDUCTION}).validify()
+                return replace(item, dices_cost=new_cost), None
         return super()._preprocess(game_state, status_source, item, signal)
 
 
 @dataclass(frozen=True, kw_only=True)
 class CrystallizeStatus(CombatStatus, StackedShieldStatus):
     usages: int = 1
     MAX_USAGES: ClassVar[int] = 2
@@ -499,47 +670,14 @@
     #     return DendroCoreStatus(total_count)
 
     def __str__(self) -> str:
         return super().__str__() + f"({self.usages})"  # pragma: no cover
 
 
 @dataclass(frozen=True)
-class CatalyzingFieldStatus(CombatStatus):
-    damage_boost: ClassVar[int] = 1
-    usages: int = 2
-
-    @override
-    def _preprocess(
-            self,
-            game_state: GameState,
-            status_source: StaticTarget,
-            item: Preprocessable,
-            signal: PREPROCESSABLES,
-    ) -> tuple[Preprocessable, Optional[CatalyzingFieldStatus]]:
-        if signal is PREPROCESSABLES.DMG_AMOUNT:
-            assert isinstance(item, eft.SpecificDamageEffect)
-            assert self.usages >= 1
-            elem_can_boost = item.element is Element.ELECTRO or item.element is Element.DENDRO
-            legal_to_boost = status_source.pid is item.source.pid
-            target_is_active = item.target.id == game_state.get_player(
-                item.target.pid
-            ).just_get_active_character().get_id()
-            if elem_can_boost and legal_to_boost and target_is_active:
-                new_damage = replace(item, damage=item.damage + CatalyzingFieldStatus.damage_boost)
-                if self.usages == 1:
-                    return new_damage, None
-                else:
-                    return new_damage, CatalyzingFieldStatus(self.usages - 1)
-        return super()._preprocess(game_state, status_source, item, signal)
-
-    def __str__(self) -> str:
-        return super().__str__() + f"({self.usages})"  # pragma: no cover
-
-
-@dataclass(frozen=True)
 class FrozenStatus(CharacterStatus):
     damage_boost: ClassVar[int] = 2
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
@@ -560,49 +698,33 @@
             self, source: StaticTarget, signal: TRIGGERING_SIGNAL
     ) -> tuple[list[eft.Effect], Optional[FrozenStatus]]:
         if signal is TRIGGERING_SIGNAL.ROUND_END:
             return [], None
         return [], self
 
 
-# <<<<<<<<<<<<<<<<<<<< Food Status <<<<<<<<<<<<<<<<<<<<
 @dataclass(frozen=True)
-class SatiatedStatus(CharacterStatus):
-
+class LeaveItToMeStatus(CombatStatus):
     @override
-    def _react_to_signal(
-            self, source: StaticTarget, signal: TRIGGERING_SIGNAL
-    ) -> tuple[list[eft.Effect], Optional[Self]]:
-        if signal is TRIGGERING_SIGNAL.ROUND_END:
-            return [], None
-        return [], self
-
-
-@dataclass(frozen=True)
-class MushroomPizzaStatus(CharacterStatus, _UsageStatus):
-    usages: int = 2
-    MAX_USAGES: ClassVar[int] = 2
+    def _preprocess(
+            self,
+            game_state: GameState,
+            status_source: StaticTarget,
+            item: Preprocessable,
+            signal: PREPROCESSABLES,
+    ) -> tuple[Preprocessable, Optional[Self]]:
+        if signal is PREPROCESSABLES.SWAP:
+            assert isinstance(item, GameEvent) and item.event_type is EventType.SWAP
+            if item.target.pid is status_source.pid \
+                    and item.event_speed is EventSpeed.COMBAT_ACTION:
+                return replace(item, event_speed=EventSpeed.FAST_ACTION), None
+        return super()._preprocess(game_state, status_source, item, signal)
 
-    @override
-    def _react_to_signal(
-            self, source: StaticTarget, signal: TRIGGERING_SIGNAL
-    ) -> tuple[list[eft.Effect], Optional[Self]]:
-        es: list[eft.Effect] = []
-        d_usages = 0
-        if signal is TRIGGERING_SIGNAL.END_ROUND_CHECK_OUT:
-            es.append(
-                eft.RecoverHPEffect(
-                    source,
-                    1,
-                )
-            )
-        if signal is TRIGGERING_SIGNAL.ROUND_END:
-            d_usages = -1
 
-        return es, replace(self, usages=d_usages)
+############################## Character Status ##############################
 
 
 @dataclass(frozen=True)
 class JueyunGuobaStatus(CharacterStatus, _UsageStatus):
     usages: int = 1
     MAX_USAGES: ClassVar[int] = 1
     damage_boost: ClassVar[int] = 1
@@ -629,31 +751,49 @@
         d_usages = 0
         if signal is TRIGGERING_SIGNAL.ROUND_END:
             d_usages = -1
         return [], replace(self, usages=d_usages)
 
 
 @dataclass(frozen=True)
-class NorthernSmokedChickenStatus(CharacterStatus, _UsageStatus):
+class LotusFlowerCrispStatus(CharacterStatus, FixedShieldStatus):
     usages: int = 1
     MAX_USAGES: ClassVar[int] = 1
+    SHIELD_AMOUNT: ClassVar[int] = 3
+
+    @override
+    def _react_to_signal(
+            self,
+            source: StaticTarget,
+            signal: TRIGGERING_SIGNAL
+    ) -> tuple[list[eft.Effect], Optional[Self]]:
+        d_usages = 0
+        if signal is TRIGGERING_SIGNAL.ROUND_END:
+            d_usages = -BIG_INT
+        return [], replace(self, usages=d_usages)
+
+
+@dataclass(frozen=True)
+class MintyMeatRollsStatus(CharacterStatus, _UsageStatus):
+    usages: int = 3
+    MAX_USAGES: ClassVar[int] = 3
     COST_DEDUCTION: ClassVar[int] = 1
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
             item: Preprocessable,
             signal: PREPROCESSABLES,
     ) -> tuple[Preprocessable, Optional[Self]]:
         if signal is PREPROCESSABLES.SKILL:
-            assert isinstance(item, evt.GameEvent)
+            assert isinstance(item, GameEvent)
             if status_source == item.target \
-                    and item.event_type is evt.EventType.NORMAL_ATTACK \
+                    and item.event_type is EventType.NORMAL_ATTACK \
                     and item.dices_cost[Element.ANY] >= self.COST_DEDUCTION:
                 item = replace(
                     item,
                     dices_cost=(item.dices_cost - {Element.ANY: self.COST_DEDUCTION}).validify()
                 )
                 return item, replace(self, usages=self.usages - 1)
         return super()._preprocess(game_state, status_source, item, signal)
@@ -665,49 +805,55 @@
         d_usages = 0
         if signal is TRIGGERING_SIGNAL.ROUND_END:
             d_usages = -BIG_INT
         return [], replace(self, usages=d_usages)
 
 
 @dataclass(frozen=True)
-class LotusFlowerCrispStatus(CharacterStatus, FixedShieldStatus):
-    usages: int = 1
-    MAX_USAGES: ClassVar[int] = 1
-    SHIELD_AMOUNT: ClassVar[int] = 3
+class MushroomPizzaStatus(CharacterStatus, _UsageStatus):
+    usages: int = 2
+    MAX_USAGES: ClassVar[int] = 2
 
     @override
     def _react_to_signal(
-            self,
-            source: StaticTarget,
-            signal: TRIGGERING_SIGNAL
+            self, source: StaticTarget, signal: TRIGGERING_SIGNAL
     ) -> tuple[list[eft.Effect], Optional[Self]]:
+        es: list[eft.Effect] = []
         d_usages = 0
+        if signal is TRIGGERING_SIGNAL.END_ROUND_CHECK_OUT:
+            es.append(
+                eft.RecoverHPEffect(
+                    source,
+                    1,
+                )
+            )
         if signal is TRIGGERING_SIGNAL.ROUND_END:
-            d_usages = -BIG_INT
-        return [], replace(self, usages=d_usages)
+            d_usages = -1
+
+        return es, replace(self, usages=d_usages)
 
 
 @dataclass(frozen=True)
-class MintyMeatRollsStatus(CharacterStatus, _UsageStatus):
-    usages: int = 3
-    MAX_USAGES: ClassVar[int] = 3
+class NorthernSmokedChickenStatus(CharacterStatus, _UsageStatus):
+    usages: int = 1
+    MAX_USAGES: ClassVar[int] = 1
     COST_DEDUCTION: ClassVar[int] = 1
 
     @override
     def _preprocess(
             self,
             game_state: GameState,
             status_source: StaticTarget,
             item: Preprocessable,
             signal: PREPROCESSABLES,
     ) -> tuple[Preprocessable, Optional[Self]]:
         if signal is PREPROCESSABLES.SKILL:
-            assert isinstance(item, evt.GameEvent)
+            assert isinstance(item, GameEvent)
             if status_source == item.target \
-                    and item.event_type is evt.EventType.NORMAL_ATTACK \
+                    and item.event_type is EventType.NORMAL_ATTACK \
                     and item.dices_cost[Element.ANY] >= self.COST_DEDUCTION:
                 item = replace(
                     item,
                     dices_cost=(item.dices_cost - {Element.ANY: self.COST_DEDUCTION}).validify()
                 )
                 return item, replace(self, usages=self.usages - 1)
         return super()._preprocess(game_state, status_source, item, signal)
@@ -717,170 +863,45 @@
             self, source: StaticTarget, signal: TRIGGERING_SIGNAL
     ) -> tuple[list[eft.Effect], Optional[Self]]:
         d_usages = 0
         if signal is TRIGGERING_SIGNAL.ROUND_END:
             d_usages = -BIG_INT
         return [], replace(self, usages=d_usages)
 
-# >>>>>>>>>>>>>>>>>>>> Food Status >>>>>>>>>>>>>>>>>>>>
-
-
-@dataclass(frozen=True)
-class ChangingShiftsStatus(CombatStatus):
-    COST_DEDUCTION: ClassVar[int] = 1
-
-    @override
-    def _preprocess(
-            self,
-            game_state: GameState,
-            status_source: StaticTarget,
-            item: Preprocessable,
-            signal: PREPROCESSABLES,
-    ) -> tuple[Preprocessable, Optional[Self]]:
-        if signal is PREPROCESSABLES.SWAP:
-            assert isinstance(item, evt.GameEvent) and item.event_type is evt.EventType.SWAP
-            if item.target.pid is status_source.pid \
-                    and item.dices_cost.num_dices() >= self.COST_DEDUCTION:
-                assert item.dices_cost.num_dices() == item.dices_cost[Element.ANY]
-                new_cost = (item.dices_cost - {Element.ANY: self.COST_DEDUCTION}).validify()
-                return replace(item, dices_cost=new_cost), None
-        return super()._preprocess(game_state, status_source, item, signal)
-
 
 @dataclass(frozen=True)
-class LeaveItToMeStatus(CombatStatus):
-    @override
-    def _preprocess(
-            self,
-            game_state: GameState,
-            status_source: StaticTarget,
-            item: Preprocessable,
-            signal: PREPROCESSABLES,
-    ) -> tuple[Preprocessable, Optional[Self]]:
-        if signal is PREPROCESSABLES.SWAP:
-            assert isinstance(item, evt.GameEvent) and item.event_type is evt.EventType.SWAP
-            if item.target.pid is status_source.pid \
-                    and item.event_speed is evt.EventSpeed.COMBAT_ACTION:
-                return replace(item, event_speed=evt.EventSpeed.FAST_ACTION), None
-        return super()._preprocess(game_state, status_source, item, signal)
-
-
-############################## Infusions ##############################
-
-
-@dataclass(frozen=True, kw_only=True)
-class _InfusionStatus(CharacterStatus, _UsageStatus):
-    MAX_USAGES: ClassVar[int] = BIG_INT
-    ELEMENT: ClassVar[Optional[Element]] = None
-    damage_boost: int = 0
-
-    @override
-    def _preprocess(
-            self,
-            game_state: GameState,
-            status_source: StaticTarget,
-            item: Preprocessable,
-            signal: PREPROCESSABLES,
-    ) -> tuple[Preprocessable, Optional[Self]]:
-        assert self.ELEMENT is not None
-        new_item: Optional[eft.SpecificDamageEffect] = None
-        if isinstance(item, eft.SpecificDamageEffect):
-            if signal is PREPROCESSABLES.DMG_ELEMENT:
-                if self._dmg_element_condition(game_state, status_source, item):
-                    new_item = replace(item, element=self.ELEMENT)
-            if signal is PREPROCESSABLES.DMG_AMOUNT:
-                if self.damage_boost != 0  \
-                        and self._dmg_boost_condition(game_state, status_source, item):
-                    new_item = replace(item, damage=item.damage + self.damage_boost)
-        if new_item is not None:
-            return new_item, self
-        else:
-            return item, self
-
-    def _dmg_element_condition(
-            self,
-            game_state: GameState,
-            status_source: StaticTarget,
-            item: eft.SpecificDamageEffect,
-    ) -> bool:
-        return item.element is Element.PHYSICAL \
-            and item.damage_type.normal_attack \
-            and status_source == item.source \
-
-
-    def _dmg_boost_condition(
-            self,
-            game_state: GameState,
-            status_source: StaticTarget,
-            item: eft.SpecificDamageEffect,
-    ) -> bool:
-        return item.element is self.ELEMENT and status_source == item.source
+class SatiatedStatus(CharacterStatus):
 
     @override
     def _react_to_signal(
             self, source: StaticTarget, signal: TRIGGERING_SIGNAL
     ) -> tuple[list[eft.Effect], Optional[Self]]:
-        d_usages = 0
         if signal is TRIGGERING_SIGNAL.ROUND_END:
-            d_usages = -1
-        return [], replace(self, usages=d_usages)
-
-
-@dataclass(frozen=True, kw_only=True)
-class ElectroInfusionStatus(_InfusionStatus):
-    ELEMENT: ClassVar[Optional[Element]] = Element.ELECTRO
-
-
-############################## Character specific ##############################
-
-
-#### Keqing ####
-
-@dataclass(frozen=True, kw_only=True)
-class KeqingTalentStatus(CharacterTalentStatus):
-    can_infuse: bool
-
-    def _react_to_signal(
-            self,
-            source: StaticTarget,
-            signal: TRIGGERING_SIGNAL
-    ) -> tuple[list[eft.Effect], Optional[KeqingTalentStatus]]:
-        if signal is TRIGGERING_SIGNAL.COMBAT_ACTION:
-            return [], type(self)(can_infuse=False)
+            return [], None
         return [], self
 
-    def __str__(self) -> str:
-        return super().__str__() + f"({case_val(self.can_infuse, 1, 0)})"  # pragma: no cover
-
 
-@dataclass(frozen=True, kw_only=True)
-class ThunderingPenanceStatus(EquipmentStatus):
-    pass
-
-
-@dataclass(frozen=True, kw_only=True)
-class KeqingElectroInfusionStatus(ElectroInfusionStatus):
-    pass
-
-    def __str__(self) -> str:
-        return super().__str__() + f"({self.damage_boost})"
+############################## Character Specific Status ##############################
+"""
+Group statues by characters, characters ordered alphabetically
+"""
 
 
 #### Kaeya ####
 
 
 @dataclass(frozen=True, kw_only=True)
-class Icicle(CombatStatus, _UsageStatus):
+class IcicleStatus(CombatStatus, _UsageStatus):
     usages: int = 3
 
     def _react_to_signal(
             self,
             source: StaticTarget,
             signal: TRIGGERING_SIGNAL
-    ) -> tuple[list[eft.Effect], Optional[Icicle]]:
+    ) -> tuple[list[eft.Effect], Optional[IcicleStatus]]:
         if source.pid.is_player1() and signal is TRIGGERING_SIGNAL.SWAP_EVENT_1 \
                 or source.pid.is_player2() and signal is TRIGGERING_SIGNAL.SWAP_EVENT_2:
             effects: list[eft.Effect] = [
                 eft.ReferredDamageEffect(
                     source=source,
                     target=DYNAMIC_CHARACTER_TARGET.OPPO_ACTIVE,
                     element=Element.CRYO,
@@ -944,13 +965,45 @@
             new_self = ColdBloodedStrikeStatus(usages=1, activated=False)
 
         return es, new_self
 
     def __str__(self) -> str:
         return super().__str__() + case_val(self.activated, "(*)", '')
 
+#### Keqing ####
+
+
+@dataclass(frozen=True, kw_only=True)
+class KeqingTalentStatus(CharacterTalentStatus):
+    can_infuse: bool
+
+    def _react_to_signal(
+            self,
+            source: StaticTarget,
+            signal: TRIGGERING_SIGNAL
+    ) -> tuple[list[eft.Effect], Optional[KeqingTalentStatus]]:
+        if signal is TRIGGERING_SIGNAL.COMBAT_ACTION:
+            return [], type(self)(can_infuse=False)
+        return [], self
+
+    def __str__(self) -> str:
+        return super().__str__() + f"({case_val(self.can_infuse, 1, 0)})"  # pragma: no cover
+
+
+@dataclass(frozen=True, kw_only=True)
+class ThunderingPenanceStatus(EquipmentStatus):
+    pass
+
+
+@dataclass(frozen=True, kw_only=True)
+class KeqingElectroInfusionStatus(ElectroInfusionStatus):
+    pass
+
+    def __str__(self) -> str:
+        return super().__str__() + f"({self.damage_boost})"
+
 
 #### Rhodeia of Loch ####
 
 @dataclass(frozen=True, kw_only=True)
 class StreamingSurgeStatus(EquipmentStatus):
     pass
```

### Comparing `dgisim-0.1.dev0/src/dgisim/status/status_processing.py` & `dgisim-0.2.dev0/dgisim/src/status/status_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,38 @@
 from typing import Callable, TYPE_CHECKING
 
 from ..effect import effect as eft
 from ..status import status as stt
 from ..summon import summon as sm
 from ..support import support as sp
 
-from ..character.character_skill_enum import CharacterSkill
+from ..character.enums import CharacterSkill
 from ..state.enums import PID
 from ..effect.enums import ZONE, TRIGGERING_SIGNAL
 from ..effect.structs import StaticTarget
-
 from .enums import PREPROCESSABLES
 
 if TYPE_CHECKING:
     from ..card.card import Card
     from ..state.game_state import GameState
 
     from .types import Preprocessable
 
+__all__ = [
+    "StatusProcessing",
+]
 
 class StatusProcessing:
+    """
+    This class holds static methods that facilitate the preprocessing of items by
+    all statuses.
+
+    e.g. 3 Pyro damage from Bennett with a sword equipped should actually be 4 after
+    preprocessing. (an equipment is also treated as a status)
+    """
     @staticmethod
     def loop_one_player_all_statuses(
             game_state: GameState,
             pid: PID,
             f: Callable[[GameState, stt.Status, StaticTarget], GameState]
     ) -> GameState:
         """
```

### Comparing `dgisim-0.1.dev0/src/dgisim/status/statuses.py` & `dgisim-0.2.dev0/dgisim/src/status/statuses.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,25 @@
 from typing import Iterator, Optional, TYPE_CHECKING, TypeVar
 from typing_extensions import Self
 
 from ..status import status as stt
 
 from ..helper.quality_of_life import just
 
+__all__ = [
+    "Statuses",
+]
 
 _U = TypeVar('_U')
 
 
 class Statuses:
+    """
+    A container for easy statuses managing.
+    """
     def __init__(self, statuses: tuple[stt.Status, ...]):
         self._statuses = statuses
 
     def update_status(self, incoming_status: stt.Status, override: bool = False) -> Self:
         """
         Replaces existing status of the same type with the new_status,
         or append the new_status to the end of current statuses
```

### Comparing `dgisim-0.1.dev0/src/dgisim/summon/summon.py` & `dgisim-0.2.dev0/dgisim/src/summon/summon.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,47 @@
+"""
+This file contains the base class "Summon" for all summons,
+and implementation of all summons.
+
+Note that a summon is basically a Status.
+
+The classes are divided into 3 sections ordered. Within each section, they are
+ordered alphabetically.
+
+- base class, which is Summon
+- template classes, starting with an '_', are templates for other classes
+- concrete classes, the implementation of summons that are actually in the game
+"""
 from __future__ import annotations
 from dataclasses import dataclass, replace
 from typing import ClassVar, Optional, TYPE_CHECKING
 from typing_extensions import override, Self
 
 from ..effect import effect as eft
 from ..status import status as stt
 
 from ..effect.enums import TRIGGERING_SIGNAL, DYNAMIC_CHARACTER_TARGET
 from ..effect.structs import DamageType
-from ..element.element import Element
+from ..element import Element
 from ..helper.quality_of_life import BIG_INT
 
 if TYPE_CHECKING:
     from ..effect.structs import StaticTarget
 
+__all__ = [
+    # base
+    "Summon",
+
+    # concrete implementations
+    "BurningFlameSummon",
+    "OceanicMimicFrogSummon",
+    "OceanicMimicRaptorSummon",
+    "OceanicMimicSquirrelSummon",
+]
+
 
 @dataclass(frozen=True, kw_only=True)
 class Summon(stt.Status):
     usages: int = -1
 
     def __str__(self) -> str:  # pragma: no cover
         return self.__class__.__name__.removesuffix("Summon") + f"({self.usages})"
```

### Comparing `dgisim-0.1.dev0/src/dgisim/summon/summons.py` & `dgisim-0.2.dev0/dgisim/src/summon/summons.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,23 @@
 from typing import Iterator, Optional, TYPE_CHECKING, Union
 
 from ..helper.quality_of_life import just
 
 if TYPE_CHECKING:
     from .summon import Summon
 
+__all__ = [
+    "Summons",
+]
+
 
 class Summons:
+    """
+    A container for easy summons managing.
+    """
     def __init__(self, summons: tuple[Summon, ...], max_num: int):
         assert len(summons) <= max_num
         self._summons = summons
         self._max_num = max_num
 
     def get_summons(self) -> tuple[Summon, ...]:
         return self._summons
```

### Comparing `dgisim-0.1.dev0/src/dgisim/support/support.py` & `dgisim-0.2.dev0/dgisim/src/support/support.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,48 @@
+"""
+This file contains the base class "Support" for all supports,
+and implementation of all supports.
+
+Note that a summon is basically a Status.
+
+The classes are divided into 3 sections ordered. Within each section, they are
+ordered alphabetically.
+
+- base class, which is Support
+- template classes, starting with an '_', are templates for other classes
+- concrete classes, the implementation of summons that are actually in the game
+"""
 from __future__ import annotations
 from dataclasses import dataclass, replace
 from typing import ClassVar, TYPE_CHECKING
 from typing_extensions import Self, override
 
 from ..card import card as cd
 from ..effect import effect as eft
-from ..event import event as evt
+from ..event import CardEvent
 from ..status import status as stt
 
 from ..effect.enums import TRIGGERING_SIGNAL
-from ..element.element import Element
+from ..element import Element
 from ..helper.quality_of_life import BIG_INT
 from ..status.enums import PREPROCESSABLES
 
 if TYPE_CHECKING:
     from ..state.game_state import GameState
     from ..effect.structs import StaticTarget
     from ..status.types import Preprocessable
 
+__all__ = [
+    # base
+    "Support",
+
+    # concrete implementations
+    "XudongSupport",
+]
+
 
 @dataclass(frozen=True, kw_only=True)
 class Support(stt.Status):
     sid: int
 
     def __str__(self) -> str:  # pragma: no cover
         return self.__class__.__name__.removesuffix("Support") \
@@ -42,15 +63,15 @@
             self,
             game_state: GameState,
             status_source: StaticTarget,
             item: Preprocessable,
             signal: PREPROCESSABLES,
     ) -> tuple[Preprocessable, None | Self]:
         if signal is PREPROCESSABLES.CARD:
-            assert isinstance(item, evt.CardEvent)
+            assert isinstance(item, CardEvent)
             if item.pid is status_source.pid \
                     and issubclass(item.card_type, cd.FoodCard) \
                     and item.dices_cost.num_dices() > 0 \
                     and self.usages > 0:
                 # note that this only handle cases when food requires only one kind of dices
                 major_elem: Element
                 if item.dices_cost[Element.OMNI] == item.dices_cost.num_dices():
```

### Comparing `dgisim-0.1.dev0/src/dgisim/support/supports.py` & `dgisim-0.2.dev0/dgisim/src/support/supports.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from __future__ import annotations
 from typing import Iterator
 
 from ..helper.quality_of_life import just
-
 from .support import Support
 
+__all__ = [
+    "Supports",
+]
 
 class Supports:
+    """
+    A container for easy supports managing.
+    """
     def __init__(self, supports: tuple[Support, ...], max_num: int):
         assert len(supports) <= max_num
         self._supports = supports
         self._max_num = max_num
 
     def get_supports(self) -> tuple[Support, ...]:
         return self._supports
```

