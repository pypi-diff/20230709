# Comparing `tmp/fl-api-requester-1.0.4.tar.gz` & `tmp/fl-api-requester-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fl-api-requester-1.0.4.tar", last modified: Sun Jul  9 15:22:55 2023, max compression
+gzip compressed data, was "fl-api-requester-1.0.5.tar", last modified: Sun Jul  9 18:52:45 2023, max compression
```

## Comparing `fl-api-requester-1.0.4.tar` & `fl-api-requester-1.0.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.157472 fl-api-requester-1.0.4/
--rw-rw-rw-   0        0        0     1073 2023-06-25 18:54:15.000000 fl-api-requester-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1313 2023-07-09 15:22:55.157472 fl-api-requester-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      827 2023-07-03 21:57:13.000000 fl-api-requester-1.0.4/README.md
--rw-rw-rw-   0        0        0      597 2023-07-09 15:15:29.000000 fl-api-requester-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-09 15:22:55.157472 fl-api-requester-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.062434 fl-api-requester-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.089434 fl-api-requester-1.0.4/src/fl_api_requester/
--rw-rw-rw-   0        0        0     2237 2023-06-26 16:51:37.000000 fl-api-requester-1.0.4/src/fl_api_requester/FLAPIConnectionData.py
--rw-rw-rw-   0        0        0     8465 2023-07-09 15:19:21.000000 fl-api-requester-1.0.4/src/fl_api_requester/FLAPIRequester.py
--rw-rw-rw-   0        0        0      124 2023-06-25 20:27:37.000000 fl-api-requester-1.0.4/src/fl_api_requester/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.117432 fl-api-requester-1.0.4/src/fl_api_requester/dto/
--rw-rw-rw-   0        0        0       45 2023-06-25 17:08:13.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/DTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.070443 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.119433 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/alliance/
--rw-rw-rw-   0        0        0      164 2023-06-26 16:25:59.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/alliance/CreateAllianceDTO.py
--rw-rw-rw-   0        0        0      170 2023-06-26 16:26:03.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/alliance/RemoveAllianceDTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.120443 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/authentication/
--rw-rw-rw-   0        0        0      188 2023-06-26 16:26:13.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/authentication/AuthenticationRequestDTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.126433 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/discord/
--rw-rw-rw-   0        0        0      246 2023-06-26 16:26:26.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/discord/AddAllianceToDiscordDTO.py
--rw-rw-rw-   0        0        0      358 2023-07-03 19:59:49.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/discord/AddChannelsToDiscordDTO.py
--rw-rw-rw-   0        0        0      339 2023-07-03 19:59:59.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/discord/CreateDiscordDTO.py
--rw-rw-rw-   0        0        0      258 2023-07-03 19:58:33.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/discord/RemoveChannelsFromDiscordDTO.py
--rw-rw-rw-   0        0        0      204 2023-06-26 16:26:57.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/discord/RemoveDiscordDTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.127440 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/discord_channel/
--rw-rw-rw-   0        0        0      213 2023-07-03 19:59:46.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/discord_channel/DiscordChannelRequestDTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.130434 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/planet/
--rw-rw-rw-   0        0        0      210 2023-06-26 16:27:19.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/planet/AddPlanetDTO.py
--rw-rw-rw-   0        0        0      196 2023-06-26 16:27:28.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/planet/RemovePlanetDTO.py
--rw-rw-rw-   0        0        0      226 2023-06-26 16:27:44.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/planet/RemoveSpecificPlanetDTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.136439 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/player/
--rw-rw-rw-   0        0        0      161 2023-06-26 16:30:05.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/player/CreatePlayerDTO.py
--rw-rw-rw-   0        0        0      173 2023-06-26 16:30:13.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/player/RemovePlayerDTO.py
--rw-rw-rw-   0        0        0      196 2023-06-26 16:30:26.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/player/SetAllianceDTO.py
--rw-rw-rw-   0        0        0      244 2023-06-26 16:30:38.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/player/SetPlayerRolesDTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.141433 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/war/
--rw-rw-rw-   0        0        0      161 2023-06-26 16:31:11.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/war/StartWarDTO.py
--rw-rw-rw-   0        0        0      159 2023-06-26 16:30:56.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/war/StopWarDTO.py
--rw-rw-rw-   0        0        0      252 2023-06-26 16:31:09.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/request/war/WarAttackRequestDTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.079435 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.143449 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/alliance/
--rw-rw-rw-   0        0        0      341 2023-06-26 16:10:18.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/alliance/AllianceDTO.py
--rw-rw-rw-   0        0        0      161 2023-06-26 16:11:22.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/alliance/AllianceNameDTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.144433 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/authentication/
--rw-rw-rw-   0        0        0      255 2023-06-26 16:08:21.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/authentication/AuthenticationResponseDTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.145447 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/discord/
--rw-rw-rw-   0        0        0      422 2023-07-03 20:01:47.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/discord/DiscordDTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.146433 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/discord_channel/
--rw-rw-rw-   0        0        0      192 2023-07-03 20:01:18.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/discord_channel/DiscordChannelResponseDTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.149443 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/planet/
--rw-rw-rw-   0        0        0      225 2023-06-26 16:11:39.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/planet/PlanetDTO.py
--rw-rw-rw-   0        0        0      250 2023-06-26 16:31:50.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/planet/PlanetOwnerDTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.150443 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/player/
--rw-rw-rw-   0        0        0      398 2023-06-26 16:24:19.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/player/PlayerDTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.153434 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/war/
--rw-rw-rw-   0        0        0      494 2023-07-03 19:43:57.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/war/WarAttackResponseDTO.py
--rw-rw-rw-   0        0        0      499 2023-07-03 19:43:20.000000 fl-api-requester-1.0.4/src/fl_api_requester/dto/response/war/WarDTO.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.156440 fl-api-requester-1.0.4/src/fl_api_requester/exception/
--rw-rw-rw-   0        0        0      568 2023-06-25 19:57:26.000000 fl-api-requester-1.0.4/src/fl_api_requester/exception/APIErrorException.py
-drwxrwxrwx   0        0        0        0 2023-07-09 15:22:55.116433 fl-api-requester-1.0.4/src/fl_api_requester.egg-info/
--rw-rw-rw-   0        0        0     1313 2023-07-09 15:22:55.000000 fl-api-requester-1.0.4/src/fl_api_requester.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2253 2023-07-09 15:22:55.000000 fl-api-requester-1.0.4/src/fl_api_requester.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 15:22:55.000000 fl-api-requester-1.0.4/src/fl_api_requester.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-09 15:22:55.000000 fl-api-requester-1.0.4/src/fl_api_requester.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-09 15:22:55.000000 fl-api-requester-1.0.4/src/fl_api_requester.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.361886 fl-api-requester-1.0.5/
+-rw-rw-rw-   0        0        0     1073 2023-06-25 18:54:15.000000 fl-api-requester-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1313 2023-07-09 18:52:45.360886 fl-api-requester-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      827 2023-07-03 21:57:13.000000 fl-api-requester-1.0.5/README.md
+-rw-rw-rw-   0        0        0      597 2023-07-09 18:52:09.000000 fl-api-requester-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 18:52:45.361886 fl-api-requester-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.247899 fl-api-requester-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.304885 fl-api-requester-1.0.5/src/fl_api_requester/
+-rw-rw-rw-   0        0        0     2237 2023-06-26 16:51:37.000000 fl-api-requester-1.0.5/src/fl_api_requester/FLAPIConnectionData.py
+-rw-rw-rw-   0        0        0     8462 2023-07-09 18:51:40.000000 fl-api-requester-1.0.5/src/fl_api_requester/FLAPIRequester.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 20:27:37.000000 fl-api-requester-1.0.5/src/fl_api_requester/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.324885 fl-api-requester-1.0.5/src/fl_api_requester/dto/
+-rw-rw-rw-   0        0        0       45 2023-06-25 17:08:13.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/DTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.252887 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.326885 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/alliance/
+-rw-rw-rw-   0        0        0      164 2023-06-26 16:25:59.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/alliance/CreateAllianceDTO.py
+-rw-rw-rw-   0        0        0      170 2023-06-26 16:26:03.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/alliance/RemoveAllianceDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.327886 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/authentication/
+-rw-rw-rw-   0        0        0      188 2023-06-26 16:26:13.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/authentication/AuthenticationRequestDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.334887 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/discord/
+-rw-rw-rw-   0        0        0      246 2023-06-26 16:26:26.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/discord/AddAllianceToDiscordDTO.py
+-rw-rw-rw-   0        0        0      358 2023-07-03 19:59:49.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/discord/AddChannelsToDiscordDTO.py
+-rw-rw-rw-   0        0        0      339 2023-07-03 19:59:59.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/discord/CreateDiscordDTO.py
+-rw-rw-rw-   0        0        0      258 2023-07-03 19:58:33.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/discord/RemoveChannelsFromDiscordDTO.py
+-rw-rw-rw-   0        0        0      204 2023-06-26 16:26:57.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/discord/RemoveDiscordDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.335889 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/discord_channel/
+-rw-rw-rw-   0        0        0      213 2023-07-03 19:59:46.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/discord_channel/DiscordChannelRequestDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.338885 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/planet/
+-rw-rw-rw-   0        0        0      210 2023-06-26 16:27:19.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/planet/AddPlanetDTO.py
+-rw-rw-rw-   0        0        0      196 2023-06-26 16:27:28.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/planet/RemovePlanetDTO.py
+-rw-rw-rw-   0        0        0      226 2023-06-26 16:27:44.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/planet/RemoveSpecificPlanetDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.342885 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/player/
+-rw-rw-rw-   0        0        0      161 2023-06-26 16:30:05.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/player/CreatePlayerDTO.py
+-rw-rw-rw-   0        0        0      173 2023-06-26 16:30:13.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/player/RemovePlayerDTO.py
+-rw-rw-rw-   0        0        0      196 2023-06-26 16:30:26.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/player/SetAllianceDTO.py
+-rw-rw-rw-   0        0        0      244 2023-06-26 16:30:38.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/player/SetPlayerRolesDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.346887 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/war/
+-rw-rw-rw-   0        0        0      161 2023-06-26 16:31:11.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/war/StartWarDTO.py
+-rw-rw-rw-   0        0        0      159 2023-06-26 16:30:56.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/war/StopWarDTO.py
+-rw-rw-rw-   0        0        0      252 2023-06-26 16:31:09.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/request/war/WarAttackRequestDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.256886 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.348885 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/alliance/
+-rw-rw-rw-   0        0        0      341 2023-06-26 16:10:18.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/alliance/AllianceDTO.py
+-rw-rw-rw-   0        0        0      161 2023-06-26 16:11:22.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/alliance/AllianceNameDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.350887 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/authentication/
+-rw-rw-rw-   0        0        0      255 2023-06-26 16:08:21.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/authentication/AuthenticationResponseDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.351886 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/discord/
+-rw-rw-rw-   0        0        0      422 2023-07-03 20:01:47.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/discord/DiscordDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.352887 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/discord_channel/
+-rw-rw-rw-   0        0        0      192 2023-07-03 20:01:18.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/discord_channel/DiscordChannelResponseDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.354893 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/planet/
+-rw-rw-rw-   0        0        0      225 2023-06-26 16:11:39.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/planet/PlanetDTO.py
+-rw-rw-rw-   0        0        0      250 2023-06-26 16:31:50.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/planet/PlanetOwnerDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.355886 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/player/
+-rw-rw-rw-   0        0        0      398 2023-06-26 16:24:19.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/player/PlayerDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.357885 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/war/
+-rw-rw-rw-   0        0        0      494 2023-07-03 19:43:57.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/war/WarAttackResponseDTO.py
+-rw-rw-rw-   0        0        0      499 2023-07-03 19:43:20.000000 fl-api-requester-1.0.5/src/fl_api_requester/dto/response/war/WarDTO.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.359886 fl-api-requester-1.0.5/src/fl_api_requester/exception/
+-rw-rw-rw-   0        0        0      568 2023-06-25 19:57:26.000000 fl-api-requester-1.0.5/src/fl_api_requester/exception/APIErrorException.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:52:45.323885 fl-api-requester-1.0.5/src/fl_api_requester.egg-info/
+-rw-rw-rw-   0        0        0     1313 2023-07-09 18:52:45.000000 fl-api-requester-1.0.5/src/fl_api_requester.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2253 2023-07-09 18:52:45.000000 fl-api-requester-1.0.5/src/fl_api_requester.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 18:52:45.000000 fl-api-requester-1.0.5/src/fl_api_requester.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-09 18:52:45.000000 fl-api-requester-1.0.5/src/fl_api_requester.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-09 18:52:45.000000 fl-api-requester-1.0.5/src/fl_api_requester.egg-info/top_level.txt
```

### Comparing `fl-api-requester-1.0.4/LICENSE` & `fl-api-requester-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.4/PKG-INFO` & `fl-api-requester-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fl-api-requester
-Version: 1.0.4
+Version: 1.0.5
 Summary: The France Leader API requester.
 Author-email: FL-GL <franceleadergl@gmail.com>
 Project-URL: Homepage, https://github.com/France-Leader-Galaxy-Life/FL-Python-API-Requester
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `fl-api-requester-1.0.4/README.md` & `fl-api-requester-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.4/pyproject.toml` & `fl-api-requester-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fl-api-requester"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
     { name="FL-GL", email="franceleadergl@gmail.com" }
 ]
 description = "The France Leader API requester."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `fl-api-requester-1.0.4/src/fl_api_requester/FLAPIConnectionData.py` & `fl-api-requester-1.0.5/src/fl_api_requester/FLAPIConnectionData.py`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.4/src/fl_api_requester/FLAPIRequester.py` & `fl-api-requester-1.0.5/src/fl_api_requester/FLAPIRequester.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     ###########
     # Discord #
     ###########
 
     def get_discord(self, discord_id: int) -> DiscordDTO:
         return [
             from_dict(AllianceDTO, alliance) 
-            for alliance in self._send_get_request(f"/discord/get/{discord_id}")
+            for alliance in self.__send_request(f"/discord/get/{discord_id}")
         ]
     
     def create_discord(self, discord_data: CreateDiscordDTO) -> DiscordDTO:
         return from_dict(DiscordDTO, self.__send_request("/discord/create", "POST", discord_data))
 
     def add_alliance_to_discord(self, discord_data: AddAllianceToDiscordDTO) -> DiscordDTO:
         return from_dict(DiscordDTO, self.__send_request("/discord/add-alliance", "POST", discord_data))
```

### Comparing `fl-api-requester-1.0.4/src/fl_api_requester/exception/APIErrorException.py` & `fl-api-requester-1.0.5/src/fl_api_requester/exception/APIErrorException.py`

 * *Files identical despite different names*

### Comparing `fl-api-requester-1.0.4/src/fl_api_requester.egg-info/PKG-INFO` & `fl-api-requester-1.0.5/src/fl_api_requester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fl-api-requester
-Version: 1.0.4
+Version: 1.0.5
 Summary: The France Leader API requester.
 Author-email: FL-GL <franceleadergl@gmail.com>
 Project-URL: Homepage, https://github.com/France-Leader-Galaxy-Life/FL-Python-API-Requester
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `fl-api-requester-1.0.4/src/fl_api_requester.egg-info/SOURCES.txt` & `fl-api-requester-1.0.5/src/fl_api_requester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

