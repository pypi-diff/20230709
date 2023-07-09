# Comparing `tmp/dgisim-0.2.dev0.tar.gz` & `tmp/dgisim-0.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgisim-0.2.dev0.tar", last modified: Sun Jul  9 00:13:39 2023, max compression
+gzip compressed data, was "dgisim-0.2.dev1.tar", last modified: Sun Jul  9 01:30:00 2023, max compression
```

## Comparing `dgisim-0.2.dev0.tar` & `dgisim-0.2.dev1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.334931 dgisim-0.2.dev0/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1065 2023-02-15 18:18:52.000000 dgisim-0.2.dev0/LICENSE
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     6962 2023-07-09 00:13:39.334376 dgisim-0.2.dev0/PKG-INFO
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     4375 2023-07-09 00:09:20.000000 dgisim-0.2.dev0/README.md
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.287731 dgisim-0.2.dev0/dgisim/
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.298595 dgisim-0.2.dev0/dgisim/src/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      928 2023-07-09 00:06:09.000000 dgisim-0.2.dev0/dgisim/src/__init__.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.301894 dgisim-0.2.dev0/dgisim/src/action/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:00.000000 dgisim-0.2.dev0/dgisim/src/action/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     6827 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/action/action.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     3475 2023-07-08 23:37:31.000000 dgisim-0.2.dev0/dgisim/src/action/action_generator.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    15539 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/action/action_generator_generator.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      276 2023-07-08 23:36:31.000000 dgisim-0.2.dev0/dgisim/src/action/enums.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      647 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/action/types.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    11755 2023-07-08 23:43:20.000000 dgisim-0.2.dev0/dgisim/src/agents.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.304435 dgisim-0.2.dev0/dgisim/src/card/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:07.000000 dgisim-0.2.dev0/dgisim/src/card/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    34168 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/card/card.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     3938 2023-07-08 23:16:29.000000 dgisim-0.2.dev0/dgisim/src/card/cards.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      686 2023-07-08 23:17:02.000000 dgisim-0.2.dev0/dgisim/src/card/cards_set.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.307098 dgisim-0.2.dev0/dgisim/src/character/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:12.000000 dgisim-0.2.dev0/dgisim/src/character/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    24971 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/character/character.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     6293 2023-07-08 23:09:50.000000 dgisim-0.2.dev0/dgisim/src/character/characters.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      459 2023-07-08 23:17:18.000000 dgisim-0.2.dev0/dgisim/src/character/characters_set.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      683 2023-07-08 23:11:13.000000 dgisim-0.2.dev0/dgisim/src/character/enums.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    11920 2023-07-08 21:45:04.000000 dgisim-0.2.dev0/dgisim/src/cli.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    10173 2023-07-08 22:26:38.000000 dgisim-0.2.dev0/dgisim/src/dices.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.310553 dgisim-0.2.dev0/dgisim/src/effect/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:16.000000 dgisim-0.2.dev0/dgisim/src/effect/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    44279 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/effect/effect.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     2181 2023-07-08 23:07:04.000000 dgisim-0.2.dev0/dgisim/src/effect/effect_stack.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      806 2023-07-08 22:39:44.000000 dgisim-0.2.dev0/dgisim/src/effect/effects_template.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      726 2023-07-08 22:39:20.000000 dgisim-0.2.dev0/dgisim/src/effect/enums.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1247 2023-07-08 22:37:50.000000 dgisim-0.2.dev0/dgisim/src/effect/structs.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     5464 2023-07-08 21:45:34.000000 dgisim-0.2.dev0/dgisim/src/element.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      963 2023-07-08 22:33:10.000000 dgisim-0.2.dev0/dgisim/src/event.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     7130 2023-07-08 21:25:18.000000 dgisim-0.2.dev0/dgisim/src/game_state_machine.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.313692 dgisim-0.2.dev0/dgisim/src/helper/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)       86 2023-07-08 23:41:02.000000 dgisim-0.2.dev0/dgisim/src/helper/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     3707 2023-07-08 22:26:17.000000 dgisim-0.2.dev0/dgisim/src/helper/hashable_dict.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     9098 2023-07-08 22:29:08.000000 dgisim-0.2.dev0/dgisim/src/helper/level_print.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1284 2023-07-08 22:30:12.000000 dgisim-0.2.dev0/dgisim/src/helper/quality_of_life.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     3934 2023-07-08 22:31:24.000000 dgisim-0.2.dev0/dgisim/src/mode.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.314881 dgisim-0.2.dev0/dgisim/src/phase/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)       20 2023-07-08 23:32:15.000000 dgisim-0.2.dev0/dgisim/src/phase/__init__.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.319548 dgisim-0.2.dev0/dgisim/src/phase/default/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      397 2023-07-08 23:33:53.000000 dgisim-0.2.dev0/dgisim/src/phase/default/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    17142 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/phase/default/action_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     6090 2023-07-08 22:22:28.000000 dgisim-0.2.dev0/dgisim/src/phase/default/card_select_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     7024 2023-07-08 23:45:15.000000 dgisim-0.2.dev0/dgisim/src/phase/default/end_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      906 2023-07-08 22:23:01.000000 dgisim-0.2.dev0/dgisim/src/phase/default/game_end_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     5896 2023-07-08 22:23:13.000000 dgisim-0.2.dev0/dgisim/src/phase/default/roll_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     4353 2023-07-08 22:23:28.000000 dgisim-0.2.dev0/dgisim/src/phase/default/starting_hand_select_phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1550 2023-07-08 22:21:20.000000 dgisim-0.2.dev0/dgisim/src/phase/phase.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      538 2023-07-08 21:36:26.000000 dgisim-0.2.dev0/dgisim/src/player_agent.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.323092 dgisim-0.2.dev0/dgisim/src/state/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:04:22.000000 dgisim-0.2.dev0/dgisim/src/state/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      983 2023-07-08 22:16:24.000000 dgisim-0.2.dev0/dgisim/src/state/enums.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    20106 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/state/game_state.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    10577 2023-07-08 22:26:32.000000 dgisim-0.2.dev0/dgisim/src/state/player_state.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.328099 dgisim-0.2.dev0/dgisim/src/status/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:35.000000 dgisim-0.2.dev0/dgisim/src/status/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      682 2023-07-08 21:48:31.000000 dgisim-0.2.dev0/dgisim/src/status/enums.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)    35218 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/status/status.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     8428 2023-07-08 23:51:13.000000 dgisim-0.2.dev0/dgisim/src/status/status_processing.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     2852 2023-07-08 22:15:11.000000 dgisim-0.2.dev0/dgisim/src/status/statuses.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)      180 2023-07-08 22:35:19.000000 dgisim-0.2.dev0/dgisim/src/status/types.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.330577 dgisim-0.2.dev0/dgisim/src/summon/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:39.000000 dgisim-0.2.dev0/dgisim/src/summon/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     5119 2023-07-08 21:54:05.000000 dgisim-0.2.dev0/dgisim/src/summon/summon.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     2636 2023-07-08 22:14:55.000000 dgisim-0.2.dev0/dgisim/src/summon/summons.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.332882 dgisim-0.2.dev0/dgisim/src/support/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:43.000000 dgisim-0.2.dev0/dgisim/src/support/__init__.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     3240 2023-07-08 22:34:57.000000 dgisim-0.2.dev0/dgisim/src/support/support.py
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     4138 2023-07-08 22:14:45.000000 dgisim-0.2.dev0/dgisim/src/support/supports.py
-drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:13:39.292153 dgisim-0.2.dev0/dgisim.egg-info/
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     6962 2023-07-09 00:13:39.000000 dgisim-0.2.dev0/dgisim.egg-info/PKG-INFO
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     2013 2023-07-09 00:13:39.000000 dgisim-0.2.dev0/dgisim.egg-info/SOURCES.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        1 2023-07-09 00:13:39.000000 dgisim-0.2.dev0/dgisim.egg-info/dependency_links.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)       25 2023-07-09 00:13:39.000000 dgisim-0.2.dev0/dgisim.egg-info/requires.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)        7 2023-07-09 00:13:39.000000 dgisim-0.2.dev0/dgisim.egg-info/top_level.txt
--rw-r--r--   0 jarvis_yu   (501) staff       (20)     1475 2023-07-09 00:10:17.000000 dgisim-0.2.dev0/pyproject.toml
--rw-r--r--   0 jarvis_yu   (501) staff       (20)       38 2023-07-09 00:13:39.335076 dgisim-0.2.dev0/setup.cfg
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.261037 dgisim-0.2.dev1/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1065 2023-02-15 18:18:52.000000 dgisim-0.2.dev1/LICENSE
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     7091 2023-07-09 01:30:00.260534 dgisim-0.2.dev1/PKG-INFO
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     4504 2023-07-09 01:27:04.000000 dgisim-0.2.dev1/README.md
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.221389 dgisim-0.2.dev1/dgisim/
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.230277 dgisim-0.2.dev1/dgisim/src/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1314 2023-07-09 01:27:04.000000 dgisim-0.2.dev1/dgisim/src/__init__.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.233214 dgisim-0.2.dev1/dgisim/src/action/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:00.000000 dgisim-0.2.dev1/dgisim/src/action/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     6827 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/action/action.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     3475 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/action/action_generator.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    15539 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/action/action_generator_generator.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      276 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/action/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      647 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/action/types.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    11755 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/agents.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.235035 dgisim-0.2.dev1/dgisim/src/card/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:07.000000 dgisim-0.2.dev1/dgisim/src/card/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    34168 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/card/card.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     3934 2023-07-09 01:27:04.000000 dgisim-0.2.dev1/dgisim/src/card/cards.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      686 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/card/cards_set.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.237585 dgisim-0.2.dev1/dgisim/src/character/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:12.000000 dgisim-0.2.dev1/dgisim/src/character/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    24971 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/character/character.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     6581 2023-07-09 01:27:04.000000 dgisim-0.2.dev1/dgisim/src/character/characters.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      459 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/character/characters_set.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      683 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/character/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    11920 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/cli.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    10173 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/dices.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.240535 dgisim-0.2.dev1/dgisim/src/effect/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:16.000000 dgisim-0.2.dev1/dgisim/src/effect/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    44279 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/effect/effect.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     2181 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/effect/effect_stack.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      806 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/effect/effects_template.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      726 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/effect/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1247 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/effect/structs.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     5464 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/element.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      963 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/event.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     7129 2023-07-09 01:27:04.000000 dgisim-0.2.dev1/dgisim/src/game_state_machine.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.242184 dgisim-0.2.dev1/dgisim/src/helper/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)       86 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/helper/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     3707 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/helper/hashable_dict.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     9098 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/helper/level_print.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1284 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/helper/quality_of_life.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     3934 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/mode.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.243001 dgisim-0.2.dev1/dgisim/src/phase/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)       20 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/phase/__init__.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.247983 dgisim-0.2.dev1/dgisim/src/phase/default/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      397 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/phase/default/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    17142 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/phase/default/action_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     6090 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/phase/default/card_select_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     7024 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/phase/default/end_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      906 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/phase/default/game_end_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     5896 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/phase/default/roll_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     4353 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/phase/default/starting_hand_select_phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1550 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/phase/phase.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      538 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/player_agent.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.250400 dgisim-0.2.dev1/dgisim/src/state/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:04:22.000000 dgisim-0.2.dev1/dgisim/src/state/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      983 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/state/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    20520 2023-07-09 01:27:04.000000 dgisim-0.2.dev1/dgisim/src/state/game_state.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    11144 2023-07-09 01:27:04.000000 dgisim-0.2.dev1/dgisim/src/state/player_state.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.255390 dgisim-0.2.dev1/dgisim/src/status/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:35.000000 dgisim-0.2.dev1/dgisim/src/status/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      682 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/status/enums.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)    35218 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/status/status.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     8428 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/status/status_processing.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     2852 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/status/statuses.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)      180 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/status/types.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.257448 dgisim-0.2.dev1/dgisim/src/summon/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:39.000000 dgisim-0.2.dev1/dgisim/src/summon/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     5119 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/summon/summon.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     2636 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/summon/summons.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.259437 dgisim-0.2.dev1/dgisim/src/support/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 00:05:43.000000 dgisim-0.2.dev1/dgisim/src/support/__init__.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     3240 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/support/support.py
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     4138 2023-07-09 00:17:13.000000 dgisim-0.2.dev1/dgisim/src/support/supports.py
+drwxr-xr-x   0 jarvis_yu   (501) staff       (20)        0 2023-07-09 01:30:00.225716 dgisim-0.2.dev1/dgisim.egg-info/
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     7091 2023-07-09 01:30:00.000000 dgisim-0.2.dev1/dgisim.egg-info/PKG-INFO
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     2013 2023-07-09 01:30:00.000000 dgisim-0.2.dev1/dgisim.egg-info/SOURCES.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        1 2023-07-09 01:30:00.000000 dgisim-0.2.dev1/dgisim.egg-info/dependency_links.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)       25 2023-07-09 01:30:00.000000 dgisim-0.2.dev1/dgisim.egg-info/requires.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)        7 2023-07-09 01:30:00.000000 dgisim-0.2.dev1/dgisim.egg-info/top_level.txt
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)     1475 2023-07-09 01:27:04.000000 dgisim-0.2.dev1/pyproject.toml
+-rw-r--r--   0 jarvis_yu   (501) staff       (20)       38 2023-07-09 01:30:00.261168 dgisim-0.2.dev1/setup.cfg
```

### Comparing `dgisim-0.2.dev0/LICENSE` & `dgisim-0.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/PKG-INFO` & `dgisim-0.2.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgisim
-Version: 0.2.dev0
+Version: 0.2.dev1
 Summary: A highly customizable Genius Invokation TCG Simulator for AI training
 Author: Jarvis Yu
 License: MIT License
         
         Copyright (c) 2023 Leyang Yu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: source, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator
 Project-URL: tracker, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/issues
 Project-URL: changelog, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/CHANGELOG.md
-Project-URL: documentation, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki/v0.2.dev0-Documentation
+Project-URL: documentation, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki/v0.2.dev1-Documentation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -58,18 +58,21 @@
 
 Basic rules of Genius Invokation TCG can be found [here](https://genshin-impact.fandom.com/wiki/Genius_Invokation_TCG).
 
 ## Installation
 
 Make sure your Python version `>= 3.10`.
 
-```shell
+```
 pip install dgisim
 ```
 
+You may check [wiki](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki)
+for more information on the package.
+
 Note that this is a developing project and the final API to users is not set in stone.
 So you may play with it, but using it in production is not recommended at the current stage.
 
 ## Simple Guide
 
 Once installed, you may have a try with the CLI to play the simulator in command line.
```

### Comparing `dgisim-0.2.dev0/README.md` & `dgisim-0.2.dev1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,21 @@
 
 Basic rules of Genius Invokation TCG can be found [here](https://genshin-impact.fandom.com/wiki/Genius_Invokation_TCG).
 
 ## Installation
 
 Make sure your Python version `>= 3.10`.
 
-```shell
+```
 pip install dgisim
 ```
 
+You may check [wiki](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki)
+for more information on the package.
+
 Note that this is a developing project and the final API to users is not set in stone.
 So you may play with it, but using it in production is not recommended at the current stage.
 
 ## Simple Guide
 
 Once installed, you may have a try with the CLI to play the simulator in command line.
```

### Comparing `dgisim-0.2.dev0/dgisim/src/__init__.py` & `dgisim-0.2.dev1/dgisim/src/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,55 @@
 # sub-packages
 from .card.card import Card
+from .card.cards import Cards
 from .character.character import Character
+from .character.characters import Characters
 from .effect.effect import Effect
+from .effect.effect_stack import EffectStack
 from .phase import Phase
+from .state.enums import ACT, PID
 from .state.game_state import GameState
 from .state.player_state import PlayerState
 from .status.status import Status
+from .status.statuses import Statuses
 from .summon.summon import Summon
+from .summon.summons import Summons
 from .support.support import Support
+from .support.supports import Supports
 
 # module files
 from .cli import CLISession
 from .dices import AbstractDices, ActualDices, Dices
 from .element import Element, ElementalAura
 from .game_state_machine import GameStateMachine
 from .mode import DefaultMode, Mode
 from .player_agent import PlayerAgent
 
 __all__ = [
+    "ACT",
     "AbstractDices",
     "ActualDices",
     "CLISession",
     "Card",
+    "Cards",
     "Character",
+    "Characters",
     "DefaultMode",
     "Dices",
     "Effect",
+    "EffectStack",
     "Element",
     "ElementalAura",
     "GameState",
     "GameStateMachine",
     "Mode",
+    "PID",
     "Phase",
     "PlayerAgent",
     "PlayerState",
     "Status",
+    "Statuses",
     "Summon",
+    "Summons",
     "Support",
+    "Supports",
 ]
```

### Comparing `dgisim-0.2.dev0/dgisim/src/action/action.py` & `dgisim-0.2.dev1/dgisim/src/action/action.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/action/action_generator.py` & `dgisim-0.2.dev1/dgisim/src/action/action_generator.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/action/action_generator_generator.py` & `dgisim-0.2.dev1/dgisim/src/action/action_generator_generator.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/action/types.py` & `dgisim-0.2.dev1/dgisim/src/action/types.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/agents.py` & `dgisim-0.2.dev1/dgisim/src/agents.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/card/card.py` & `dgisim-0.2.dev1/dgisim/src/card/card.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/card/cards.py` & `dgisim-0.2.dev1/dgisim/src/card/cards.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 ]
 
 
 class Cards:
     """
     A container for easy management of cards.
     """
-    def __init__(self, mapping: dict[type[Card], int]) -> None:
-        self._cards = HashableDict.from_dict(mapping)
+    def __init__(self, cards: dict[type[Card], int]) -> None:
+        self._cards = HashableDict.from_dict(cards)
 
     @classmethod
     def from_empty(cls) -> Cards:
         return Cards({})
 
     def __add__(self, other: Cards | dict[type[Card], int]) -> Cards:
         other_cards: dict[type[Card], int]
```

### Comparing `dgisim-0.2.dev0/dgisim/src/card/cards_set.py` & `dgisim-0.2.dev1/dgisim/src/card/cards_set.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/character/character.py` & `dgisim-0.2.dev1/dgisim/src/character/character.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/character/characters.py` & `dgisim-0.2.dev1/dgisim/src/character/characters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import Callable, Iterator, Optional, TYPE_CHECKING, Union
+from typing import Callable, Iterator, Optional, TYPE_CHECKING, Union, Iterable
 
 if TYPE_CHECKING:
     from .character import Character
 
 __all__ = [
     "Characters",
 ]
@@ -13,14 +13,24 @@
         self._characters = characters
         self._active_character_id = active_character_id
 
     @classmethod
     def from_default(cls, characters: tuple[Character, ...]) -> Characters:
         return cls(characters, None)
 
+    @classmethod
+    def from_list(cls, characters: Iterable[type[Character]]) -> Characters:
+        return Characters(
+            tuple(
+                char.from_default(i + 1)
+                for i, char in enumerate(characters)
+            ),
+            None,
+        )
+
     def get_characters(self) -> tuple[Character, ...]:
         return self._characters
 
     def get_active_character_id(self) -> Optional[int]:
         return self._active_character_id
 
     def get_character_in_activity_order(self) -> tuple[Character, ...]:
```

### Comparing `dgisim-0.2.dev0/dgisim/src/character/enums.py` & `dgisim-0.2.dev1/dgisim/src/character/enums.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/cli.py` & `dgisim-0.2.dev1/dgisim/src/cli.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/dices.py` & `dgisim-0.2.dev1/dgisim/src/dices.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/effect/effect.py` & `dgisim-0.2.dev1/dgisim/src/effect/effect.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/effect/effect_stack.py` & `dgisim-0.2.dev1/dgisim/src/effect/effect_stack.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/effect/effects_template.py` & `dgisim-0.2.dev1/dgisim/src/effect/effects_template.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/effect/enums.py` & `dgisim-0.2.dev1/dgisim/src/effect/enums.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/effect/structs.py` & `dgisim-0.2.dev1/dgisim/src/effect/structs.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/element.py` & `dgisim-0.2.dev1/dgisim/src/element.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/event.py` & `dgisim-0.2.dev1/dgisim/src/event.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/game_state_machine.py` & `dgisim-0.2.dev1/dgisim/src/game_state_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             return False
         action_idx = len(self._history) - 1
         self._action_history.append(action_idx)
         self._actions[action_idx] = action
         self._game_state = next_state
         if observe:
             print(GamePrinter.dict_game_printer(self._game_state.dict_str()))
-            input(">>> ")
+            input(":> ")
         self._append_history(self._game_state)
         return True
 
     def step_until_phase(self, phase: type[Phase] | Phase, observe=False) -> None:
         if isinstance(phase, Phase):
             phase = type(phase)
         while isinstance(self._game_state.get_phase(), phase):
```

### Comparing `dgisim-0.2.dev0/dgisim/src/helper/hashable_dict.py` & `dgisim-0.2.dev1/dgisim/src/helper/hashable_dict.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/helper/level_print.py` & `dgisim-0.2.dev1/dgisim/src/helper/level_print.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/helper/quality_of_life.py` & `dgisim-0.2.dev1/dgisim/src/helper/quality_of_life.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/mode.py` & `dgisim-0.2.dev1/dgisim/src/mode.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/phase/default/action_phase.py` & `dgisim-0.2.dev1/dgisim/src/phase/default/action_phase.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/phase/default/card_select_phase.py` & `dgisim-0.2.dev1/dgisim/src/phase/default/card_select_phase.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/phase/default/end_phase.py` & `dgisim-0.2.dev1/dgisim/src/phase/default/end_phase.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/phase/default/game_end_phase.py` & `dgisim-0.2.dev1/dgisim/src/phase/default/game_end_phase.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/phase/default/roll_phase.py` & `dgisim-0.2.dev1/dgisim/src/phase/default/roll_phase.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/phase/default/starting_hand_select_phase.py` & `dgisim-0.2.dev1/dgisim/src/phase/default/starting_hand_select_phase.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/phase/phase.py` & `dgisim-0.2.dev1/dgisim/src/phase/phase.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/player_agent.py` & `dgisim-0.2.dev1/dgisim/src/player_agent.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/state/enums.py` & `dgisim-0.2.dev1/dgisim/src/state/enums.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/state/game_state.py` & `dgisim-0.2.dev1/dgisim/src/state/game_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 from typing import Callable, Optional
+from typing_extensions import Self
 
 from .. import mode as md
 from ..action import action as act
 from ..action import action_generator as acg
 from ..effect import effect as eft
 from ..phase.default import game_end_phase as gep
 from ..phase import phase as ph
@@ -35,15 +36,15 @@
 class GameState:
     """
     The class which represents a moment or a state of the game, containing all
     information required to proceed to the next game state.
 
     To proceed when the game doesn't require a player action at the moment,
     run step(), otherwise run action_step(player_action).
-    
+
     To tell if a player action is required, run waiting_for().
     """
 
     def __init__(
         self,
         mode: md.Mode,
         phase: ph.Phase,
@@ -65,23 +66,35 @@
         # checkers
         self._card_checker = CardChecker(self)
         self._swap_checker = SwapChecker(self)
         self._skill_checker = SkillChecker(self)
         self._elem_tuning_checker = ElementalTuningChecker(self)
 
     @classmethod
-    def from_default(cls):
+    def from_default(cls) -> Self:
         mode = md.DefaultMode()
         return cls(
             mode=mode,
             phase=mode.card_select_phase(),
             round=0,
             active_player_id=PID.P1,
-            player1=ps.PlayerState.examplePlayer(mode),
-            player2=ps.PlayerState.examplePlayer(mode),
+            player1=ps.PlayerState.example_player(mode),
+            player2=ps.PlayerState.example_player(mode),
+            effect_stack=EffectStack(()),
+        )
+
+    @classmethod
+    def from_players(cls, mode: md.Mode, player1: ps.PlayerState, player2: ps.PlayerState) -> Self:
+        return cls(
+            mode=mode,
+            phase=mode.card_select_phase(),
+            round=0,
+            active_player_id=PID.P1,
+            player1=player1,
+            player2=player2,
             effect_stack=EffectStack(()),
         )
 
     def factory(self):
         return GameStateFactory(self)
 
     def get_mode(self) -> md.Mode:
```

### Comparing `dgisim-0.2.dev0/dgisim/src/state/player_state.py` & `dgisim-0.2.dev1/dgisim/src/state/player_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 from __future__ import annotations
 from typing import Callable, Optional, Union, TYPE_CHECKING
+from typing_extensions import Self
 
-from ..card import cards as cds
 from ..character import character as chr
 from ..status import statuses as sts
 from ..support import support as sp
 
+from ..card.cards import Cards
 from ..character.characters import Characters
 from ..dices import ActualDices
 from ..summon.summons import Summons
 from ..support.supports import Supports
 
 from .enums import ACT
 
 if TYPE_CHECKING:
     from ..mode import Mode
 
 __all__ = [
     "PlayerState",
 ]
 
+
 class PlayerState:
     def __init__(
         self,
         phase: ACT,
         characters: Characters,
         combat_statuses: sts.Statuses,
         summons: Summons,
         supports: Supports,
         card_redraw_chances: int,
         dice_reroll_chances: int,
         dices: ActualDices,
-        hand_cards: cds.Cards,
-        deck_cards: cds.Cards,
-        publicly_used_cards: cds.Cards,
-        publicly_gained_cards: cds.Cards,
+        hand_cards: Cards,
+        deck_cards: Cards,
+        publicly_used_cards: Cards,
+        publicly_gained_cards: Cards,
     ):
         # REMINDER: don't forget to update factory when adding new fields
         self._phase = phase
         self._card_redraw_chances = card_redraw_chances
         self._dice_reroll_chances = dice_reroll_chances
         self._characters = characters
         self._combat_statuses = combat_statuses
@@ -73,24 +75,24 @@
 
     def get_supports(self) -> Supports:
         return self._supports
 
     def get_dices(self) -> ActualDices:
         return self._dices
 
-    def get_hand_cards(self) -> cds.Cards:
+    def get_hand_cards(self) -> Cards:
         return self._hand_cards
 
-    def get_deck_cards(self) -> cds.Cards:
+    def get_deck_cards(self) -> Cards:
         return self._deck_cards
 
-    def get_publicly_used_cards(self) -> cds.Cards:
+    def get_publicly_used_cards(self) -> Cards:
         return self._publicly_used_cards
 
-    def get_publicly_gained_cards(self) -> cds.Cards:
+    def get_publicly_gained_cards(self) -> Cards:
         return self._publicly_gained_cards
 
     def get_active_character(self) -> Optional[chr.Character]:
         return self._characters.get_active_character()
 
     def just_get_active_character(self) -> chr.Character:
         return self._characters.just_get_active_character()
@@ -122,33 +124,50 @@
     def hide_cards(self) -> PlayerState:
         return self.factory().f_hand_cards(
             lambda hcs: hcs.hide_all()
         ).f_deck_cards(
             lambda dcs: dcs.hide_all()
         ).build()
 
-    @staticmethod
-    def examplePlayer(mode: Mode):
+    @classmethod
+    def example_player(cls, mode: Mode) -> Self:
         cards = mode.all_cards()
         chars = mode.all_chars()
-        return PlayerState(
+        return cls(
             phase=ACT.PASSIVE_WAIT_PHASE,
             card_redraw_chances=0,
             dice_reroll_chances=0,
             characters=Characters.from_default(
                 tuple([char.from_default(i + 1) for i, char in enumerate(chars)][:3])
             ),
             combat_statuses=sts.Statuses(()),
             summons=Summons((), mode.summons_limit()),
             supports=Supports((), mode.supports_limit()),
             dices=ActualDices({}),
-            hand_cards=cds.Cards({}),
-            deck_cards=cds.Cards(dict([(card, mode.max_cards_per_kind()) for card in cards])),
-            publicly_used_cards=cds.Cards({}),
-            publicly_gained_cards=cds.Cards({}),
+            hand_cards=Cards({}),
+            deck_cards=Cards(dict([(card, mode.max_cards_per_kind()) for card in cards])),
+            publicly_used_cards=Cards({}),
+            publicly_gained_cards=Cards({}),
+        )
+
+    @classmethod
+    def from_deck(cls, mode: Mode, characters: Characters, cards: Cards) -> Self:
+        return cls(
+            phase=ACT.PASSIVE_WAIT_PHASE,
+            card_redraw_chances=0,
+            dice_reroll_chances=0,
+            characters=characters,
+            combat_statuses=sts.Statuses(()),
+            summons=Summons((), mode.summons_limit()),
+            supports=Supports((), mode.supports_limit()),
+            dices=ActualDices({}),
+            hand_cards=Cards({}),
+            deck_cards=cards,
+            publicly_used_cards=Cards({}),
+            publicly_gained_cards=Cards({}),
         )
 
     def _all_unique_data(self) -> tuple:
         return (
             self._phase,
             self._card_redraw_chances,
             self._characters,
@@ -249,40 +268,40 @@
     def dices(self, dices: ActualDices) -> PlayerStateFactory:
         self._dices = dices
         return self
 
     def f_dices(self, f: Callable[[ActualDices], ActualDices]) -> PlayerStateFactory:
         return self.dices(f(self._dices))
 
-    def hand_cards(self, cards: cds.Cards) -> PlayerStateFactory:
+    def hand_cards(self, cards: Cards) -> PlayerStateFactory:
         self._hand_cards = cards
         return self
 
-    def f_hand_cards(self, f: Callable[[cds.Cards], cds.Cards]) -> PlayerStateFactory:
+    def f_hand_cards(self, f: Callable[[Cards], Cards]) -> PlayerStateFactory:
         return self.hand_cards(f(self._hand_cards))
 
-    def deck_cards(self, cards: cds.Cards) -> PlayerStateFactory:
+    def deck_cards(self, cards: Cards) -> PlayerStateFactory:
         self._deck_cards = cards
         return self
 
-    def f_deck_cards(self, f: Callable[[cds.Cards], cds.Cards]) -> PlayerStateFactory:
+    def f_deck_cards(self, f: Callable[[Cards], Cards]) -> PlayerStateFactory:
         return self.deck_cards(f(self._deck_cards))
 
-    def publicly_used_cards(self, cards: cds.Cards) -> PlayerStateFactory:
+    def publicly_used_cards(self, cards: Cards) -> PlayerStateFactory:
         self._publicly_used_cards = cards
         return self
 
-    def f_publicly_used_cards(self, f: Callable[[cds.Cards], cds.Cards]) -> PlayerStateFactory:
+    def f_publicly_used_cards(self, f: Callable[[Cards], Cards]) -> PlayerStateFactory:
         return self.publicly_used_cards(f(self._publicly_used_cards))
 
-    def publicly_gained_cards(self, cards: cds.Cards) -> PlayerStateFactory:
+    def publicly_gained_cards(self, cards: Cards) -> PlayerStateFactory:
         self._publicly_gained_cards = cards
         return self
 
-    def f_publicly_gained_cards(self, f: Callable[[cds.Cards], cds.Cards]) -> PlayerStateFactory:
+    def f_publicly_gained_cards(self, f: Callable[[Cards], Cards]) -> PlayerStateFactory:
         return self.publicly_gained_cards(f(self._publicly_gained_cards))
 
     def build(self) -> PlayerState:
         return PlayerState(
             phase=self._phase,
             card_redraw_chances=self._card_redraw_chances,
             dice_reroll_chances=self._dice_reroll_chances,
```

### Comparing `dgisim-0.2.dev0/dgisim/src/status/enums.py` & `dgisim-0.2.dev1/dgisim/src/status/enums.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/status/status.py` & `dgisim-0.2.dev1/dgisim/src/status/status.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/status/status_processing.py` & `dgisim-0.2.dev1/dgisim/src/status/status_processing.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/status/statuses.py` & `dgisim-0.2.dev1/dgisim/src/status/statuses.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/summon/summon.py` & `dgisim-0.2.dev1/dgisim/src/summon/summon.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/summon/summons.py` & `dgisim-0.2.dev1/dgisim/src/summon/summons.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/support/support.py` & `dgisim-0.2.dev1/dgisim/src/support/support.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim/src/support/supports.py` & `dgisim-0.2.dev1/dgisim/src/support/supports.py`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/dgisim.egg-info/PKG-INFO` & `dgisim-0.2.dev1/dgisim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgisim
-Version: 0.2.dev0
+Version: 0.2.dev1
 Summary: A highly customizable Genius Invokation TCG Simulator for AI training
 Author: Jarvis Yu
 License: MIT License
         
         Copyright (c) 2023 Leyang Yu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,15 +23,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: source, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator
 Project-URL: tracker, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/issues
 Project-URL: changelog, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/CHANGELOG.md
-Project-URL: documentation, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki/v0.2.dev0-Documentation
+Project-URL: documentation, https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki/v0.2.dev1-Documentation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -58,18 +58,21 @@
 
 Basic rules of Genius Invokation TCG can be found [here](https://genshin-impact.fandom.com/wiki/Genius_Invokation_TCG).
 
 ## Installation
 
 Make sure your Python version `>= 3.10`.
 
-```shell
+```
 pip install dgisim
 ```
 
+You may check [wiki](https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki)
+for more information on the package.
+
 Note that this is a developing project and the final API to users is not set in stone.
 So you may play with it, but using it in production is not recommended at the current stage.
 
 ## Simple Guide
 
 Once installed, you may have a try with the CLI to play the simulator in command line.
```

### Comparing `dgisim-0.2.dev0/dgisim.egg-info/SOURCES.txt` & `dgisim-0.2.dev1/dgisim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dgisim-0.2.dev0/pyproject.toml` & `dgisim-0.2.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dgisim"
-version = "0.2.dev0"
+version = "0.2.dev1"
 license = {file = "LICENSE"}
 
 description = "A highly customizable Genius Invokation TCG Simulator for AI training"
 authors = [{ name="Jarvis Yu" }]
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
@@ -33,11 +33,11 @@
     "typing-extensions == 4.5.0",
 ]
 
 [project.urls]
 source = "https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator"
 tracker = "https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/issues"
 changelog = "https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/blob/master/CHANGELOG.md"
-documentation = "https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki/v0.2.dev0-Documentation"
+documentation = "https://github.com/Jarvis-Yu/Dottore-Genius-Invokation-TCG-Simulator/wiki/v0.2.dev1-Documentation"
 
 [tool.setuptools.package-dir]
 dgisim = "dgisim/src"
```

