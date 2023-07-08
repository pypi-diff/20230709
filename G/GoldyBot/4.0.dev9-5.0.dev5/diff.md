# Comparing `tmp/GoldyBot-4.0.dev9.tar.gz` & `tmp/GoldyBot-5.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoldyBot-4.0.dev9.tar", last modified: Tue Apr 26 22:00:00 2022, max compression
+gzip compressed data, was "GoldyBot-5.0.dev5.tar", last modified: Sat Jul  8 23:43:26 2023, max compression
```

## Comparing `GoldyBot-4.0.dev9.tar` & `GoldyBot-5.0.dev5.tar`

### file list

```diff
@@ -1,81 +1,182 @@
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.331998 GoldyBot-4.0.dev9/
-drwxrwxrwx   0        0        0        0 2022-04-26 21:59:59.971002 GoldyBot-4.0.dev9/GoldyBot/
--rw-rw-rw-   0        0        0      527 2022-04-24 19:05:07.000000 GoldyBot-4.0.dev9/GoldyBot/__init__.py
--rw-rw-rw-   0        0        0      107 2022-04-24 19:05:00.000000 GoldyBot-4.0.dev9/GoldyBot/assets.py
--rw-rw-rw-   0        0        0     3021 2022-04-25 10:03:13.000000 GoldyBot-4.0.dev9/GoldyBot/bot.py
--rw-rw-rw-   0        0        0     4130 2022-04-24 00:33:52.000000 GoldyBot-4.0.dev9/GoldyBot/cache.py
--rw-rw-rw-   0        0        0     2678 2022-04-19 18:53:42.000000 GoldyBot-4.0.dev9/GoldyBot/config.py
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.031000 GoldyBot-4.0.dev9/GoldyBot/database/
--rw-rw-rw-   0        0        0       58 2022-04-07 15:48:00.000000 GoldyBot-4.0.dev9/GoldyBot/database/__init__.py
--rw-rw-rw-   0        0        0     2489 2022-04-11 22:06:48.000000 GoldyBot-4.0.dev9/GoldyBot/database/database.py
--rw-rw-rw-   0        0        0      178 2022-04-07 15:47:57.000000 GoldyBot-4.0.dev9/GoldyBot/database/member.py
--rw-rw-rw-   0        0        0     1382 2022-04-23 23:56:04.000000 GoldyBot-4.0.dev9/GoldyBot/errors.py
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.051999 GoldyBot-4.0.dev9/GoldyBot/ext/
--rw-rw-rw-   0        0        0       35 2022-04-06 23:32:29.000000 GoldyBot-4.0.dev9/GoldyBot/ext/__init__.py
--rw-rw-rw-   0        0        0    11866 2022-04-26 21:58:23.000000 GoldyBot-4.0.dev9/GoldyBot/ext/commands.py
--rw-rw-rw-   0        0        0     3656 2022-04-23 23:25:36.000000 GoldyBot-4.0.dev9/GoldyBot/ext/extenstions.py
--rw-rw-rw-   0        0        0     2296 2022-04-11 21:00:55.000000 GoldyBot-4.0.dev9/GoldyBot/files.py
--rw-rw-rw-   0        0        0     2690 2022-04-24 15:41:23.000000 GoldyBot-4.0.dev9/GoldyBot/goldy.py
--rw-rw-rw-   0        0        0      110 2022-04-26 21:58:47.000000 GoldyBot-4.0.dev9/GoldyBot/info.py
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.053998 GoldyBot-4.0.dev9/GoldyBot/internal_modules/
--rw-rw-rw-   0        0        0        0 2022-04-06 23:32:29.000000 GoldyBot-4.0.dev9/GoldyBot/internal_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.068998 GoldyBot-4.0.dev9/GoldyBot/internal_modules/v4/
--rw-rw-rw-   0        0        0        0 2022-04-06 23:32:29.000000 GoldyBot-4.0.dev9/GoldyBot/internal_modules/v4/__init__.py
--rw-rw-rw-   0        0        0     5771 2022-04-24 17:31:14.000000 GoldyBot-4.0.dev9/GoldyBot/internal_modules/v4/admin.py
--rw-rw-rw-   0        0        0     4969 2022-04-22 23:04:14.000000 GoldyBot-4.0.dev9/GoldyBot/logging.py
--rw-rw-rw-   0        0        0     7259 2022-04-24 17:08:14.000000 GoldyBot-4.0.dev9/GoldyBot/modules.py
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.109997 GoldyBot-4.0.dev9/GoldyBot/objects/
--rw-rw-rw-   0        0        0       42 2022-04-25 08:03:40.000000 GoldyBot-4.0.dev9/GoldyBot/objects/__init__.py
--rw-rw-rw-   0        0        0    10327 2022-04-24 17:52:55.000000 GoldyBot-4.0.dev9/GoldyBot/objects/command.py
--rw-rw-rw-   0        0        0      367 2022-04-19 17:50:53.000000 GoldyBot-4.0.dev9/GoldyBot/objects/member.py
--rw-rw-rw-   0        0        0     1430 2022-04-17 22:08:01.000000 GoldyBot-4.0.dev9/GoldyBot/objects/role.py
--rw-rw-rw-   0        0        0     1280 2022-04-25 22:29:27.000000 GoldyBot-4.0.dev9/GoldyBot/objects/slash.py
--rw-rw-rw-   0        0        0     1133 2022-04-24 23:21:15.000000 GoldyBot-4.0.dev9/GoldyBot/paths.py
--rw-rw-rw-   0        0        0      122 2022-04-20 14:05:29.000000 GoldyBot-4.0.dev9/GoldyBot/settings.py
--rw-rw-rw-   0        0        0     1209 2022-04-13 21:15:06.000000 GoldyBot-4.0.dev9/GoldyBot/system.py
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.125001 GoldyBot-4.0.dev9/GoldyBot/templates/
--rw-rw-rw-   0        0        0       78 2022-04-15 23:48:00.000000 GoldyBot-4.0.dev9/GoldyBot/templates/__init__.py
--rw-rw-rw-   0        0        0      306 2022-04-13 13:42:09.000000 GoldyBot-4.0.dev9/GoldyBot/templates/goldy_config.json
--rw-rw-rw-   0        0        0     1157 2022-04-07 15:47:40.000000 GoldyBot-4.0.dev9/GoldyBot/token.py
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.133002 GoldyBot-4.0.dev9/GoldyBot/utility/
--rw-rw-rw-   0        0        0      106 2022-04-24 12:42:45.000000 GoldyBot-4.0.dev9/GoldyBot/utility/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.164998 GoldyBot-4.0.dev9/GoldyBot/utility/commands/
--rw-rw-rw-   0        0        0      386 2022-04-25 08:45:54.000000 GoldyBot-4.0.dev9/GoldyBot/utility/commands/__init__.py
--rw-rw-rw-   0        0        0      328 2022-04-24 19:06:57.000000 GoldyBot-4.0.dev9/GoldyBot/utility/commands/_icon_.py
--rw-rw-rw-   0        0        0      238 2022-04-23 16:12:49.000000 GoldyBot-4.0.dev9/GoldyBot/utility/commands/_mention_.py
--rw-rw-rw-   0        0        0     3776 2022-04-25 09:38:24.000000 GoldyBot-4.0.dev9/GoldyBot/utility/commands/_send_.py
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.187999 GoldyBot-4.0.dev9/GoldyBot/utility/goldy/
--rw-rw-rw-   0        0        0      386 2022-04-25 08:03:18.000000 GoldyBot-4.0.dev9/GoldyBot/utility/goldy/__init__.py
--rw-rw-rw-   0        0        0      207 2022-04-06 23:32:29.000000 GoldyBot-4.0.dev9/GoldyBot/utility/goldy/colours.py
--rw-rw-rw-   0        0        0      112 2022-04-06 23:32:29.000000 GoldyBot-4.0.dev9/GoldyBot/utility/goldy/embed.py
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.221001 GoldyBot-4.0.dev9/GoldyBot/utility/guilds/
--rw-rw-rw-   0        0        0      375 2022-04-24 15:51:11.000000 GoldyBot-4.0.dev9/GoldyBot/utility/guilds/__init__.py
--rw-rw-rw-   0        0        0     1642 2022-04-24 18:44:36.000000 GoldyBot-4.0.dev9/GoldyBot/utility/guilds/config.py
--rw-rw-rw-   0        0        0     5100 2022-04-24 18:20:58.000000 GoldyBot-4.0.dev9/GoldyBot/utility/guilds/guild.py
--rw-rw-rw-   0        0        0      570 2022-04-24 18:19:53.000000 GoldyBot-4.0.dev9/GoldyBot/utility/guilds/guild_config_template.json
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.295999 GoldyBot-4.0.dev9/GoldyBot/utility/msgs/
--rw-rw-rw-   0        0        0       53 2022-04-19 15:42:59.000000 GoldyBot-4.0.dev9/GoldyBot/utility/msgs/__init__.py
--rw-rw-rw-   0        0        0     1105 2022-04-19 18:45:33.000000 GoldyBot-4.0.dev9/GoldyBot/utility/msgs/bot.py
--rw-rw-rw-   0        0        0       50 2022-04-12 23:00:04.000000 GoldyBot-4.0.dev9/GoldyBot/utility/msgs/cache.py
--rw-rw-rw-   0        0        0      379 2022-04-24 12:49:50.000000 GoldyBot-4.0.dev9/GoldyBot/utility/msgs/goldy.py
--rw-rw-rw-   0        0        0      222 2022-04-06 23:32:29.000000 GoldyBot-4.0.dev9/GoldyBot/utility/msgs/help.py
--rw-rw-rw-   0        0        0      966 2022-04-19 15:11:02.000000 GoldyBot-4.0.dev9/GoldyBot/utility/msgs/reload.py
--rw-rw-rw-   0        0        0      780 2022-04-19 15:42:32.000000 GoldyBot-4.0.dev9/GoldyBot/utility/msgs/unload.py
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.320999 GoldyBot-4.0.dev9/GoldyBot/utility/nextcordpy/
--rw-rw-rw-   0        0        0       34 2022-04-10 23:33:39.000000 GoldyBot-4.0.dev9/GoldyBot/utility/nextcordpy/__init__.py
--rw-rw-rw-   0        0        0     7758 2022-04-10 23:33:52.000000 GoldyBot-4.0.dev9/GoldyBot/utility/nextcordpy/help_command.py
--rw-rw-rw-   0        0        0      356 2022-04-24 18:31:16.000000 GoldyBot-4.0.dev9/GoldyBot/utility/nextcordpy/prefix.py
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.328997 GoldyBot-4.0.dev9/GoldyBot/utility/v3_support/
--rw-rw-rw-   0        0        0      697 2022-04-07 14:05:00.000000 GoldyBot-4.0.dev9/GoldyBot/utility/v3_support/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-26 22:00:00.005001 GoldyBot-4.0.dev9/GoldyBot.egg-info/
--rw-rw-rw-   0        0        0     1117 2022-04-26 21:59:59.000000 GoldyBot-4.0.dev9/GoldyBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1788 2022-04-26 21:59:59.000000 GoldyBot-4.0.dev9/GoldyBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-26 21:59:59.000000 GoldyBot-4.0.dev9/GoldyBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2022-04-26 21:59:59.000000 GoldyBot-4.0.dev9/GoldyBot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-04-26 21:59:59.000000 GoldyBot-4.0.dev9/GoldyBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       32 2022-04-15 23:56:15.000000 GoldyBot-4.0.dev9/MANIFEST.in
--rw-rw-rw-   0        0        0     1117 2022-04-26 22:00:00.330999 GoldyBot-4.0.dev9/PKG-INFO
--rw-rw-rw-   0        0        0      382 2022-04-15 22:59:41.000000 GoldyBot-4.0.dev9/README.txt
--rw-rw-rw-   0        0        0       69 2022-04-25 22:30:36.000000 GoldyBot-4.0.dev9/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-04-26 22:00:00.331998 GoldyBot-4.0.dev9/setup.cfg
--rw-rw-rw-   0        0        0      956 2022-04-26 21:58:53.000000 GoldyBot-4.0.dev9/setup.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.499566 GoldyBot-5.0.dev5/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       65 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/.gitattributes
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.467566 GoldyBot-5.0.dev5/.github/
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.471566 GoldyBot-5.0.dev5/.github/workflows/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      888 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/.github/workflows/documentation.yaml
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      775 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/.github/workflows/lint_and_test.yaml
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      176 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/.gitignore
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      301 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/Dockerfile
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.472566 GoldyBot-5.0.dev5/GoldyBot/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1256 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/__init__.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.474566 GoldyBot-5.0.dev5/GoldyBot/assets/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)    37153 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/assets/ding.mp3
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      397 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/assets/goldy.json
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       98 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/assets/run.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       76 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/assets/token.env
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.474566 GoldyBot-5.0.dev5/GoldyBot/cli/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       50 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/cli/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1873 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/cli/__main__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1419 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/cli/_setup.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      421 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/config.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1673 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/errors.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1043 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/file_templates.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.475566 GoldyBot-5.0.dev5/GoldyBot/goldy/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)    10935 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/__init__.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.477566 GoldyBot-5.0.dev5/GoldyBot/goldy/commands/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/commands/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     7958 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/commands/command.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2687 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/commands/decorator.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     8115 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/commands/group_command.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     4719 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/commands/listener.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     3358 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/commands/loader.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     5695 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/commands/prefix_command.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     6075 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/commands/slash_command.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.477566 GoldyBot-5.0.dev5/GoldyBot/goldy/database/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     4701 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/database/__init__.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.477566 GoldyBot-5.0.dev5/GoldyBot/goldy/database/databases/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     3836 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/database/databases/__init__.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.478566 GoldyBot-5.0.dev5/GoldyBot/goldy/database/wrappers/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1363 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/database/wrappers/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2926 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/database/wrappers/member.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.478566 GoldyBot-5.0.dev5/GoldyBot/goldy/extensions/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     3714 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/extensions/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     7441 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/extensions/extension_loader.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2854 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/goldy_config.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.478566 GoldyBot-5.0.dev5/GoldyBot/goldy/guilds/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     4029 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/guilds/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2591 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/guilds/guild.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.479566 GoldyBot-5.0.dev5/GoldyBot/goldy/live_console/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1016 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/live_console/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2177 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/live_console/app.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.479566 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      609 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/__init__.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.480566 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/channels/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        0 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/channels/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1222 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/channels/delete_channel.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1158 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/channels/get_channel.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      508 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/colours.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.480566 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/embeds/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        0 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/embeds/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     4255 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/embeds/embed.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     5798 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/front_end_errors.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.481566 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/guilds/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        0 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/guilds/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1237 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/guilds/get_channels.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1074 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/guilds/get_guild_data.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.481566 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/messages/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        0 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/messages/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1317 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/messages/delete_msg.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     9357 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/messages/send_msg.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.482566 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/slash_options/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        0 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/slash_options/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2523 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/slash_options/auto_complete.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     4952 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/nextcore_utils/slash_options/slash_option.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.483566 GoldyBot-5.0.dev5/GoldyBot/goldy/objects/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      285 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/objects/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2303 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/objects/channel.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2241 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/objects/invokable.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1811 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/objects/member.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1079 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/objects/message.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.483566 GoldyBot-5.0.dev5/GoldyBot/goldy/objects/platter/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2438 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/objects/platter/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1522 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/objects/platter/golden_platter.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      965 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/objects/platter/silver_platter.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     3505 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/permission_system.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      193 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/perms.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2833 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/presence.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.484566 GoldyBot-5.0.dev5/GoldyBot/goldy/recipes/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2491 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/recipes/__init__.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.484566 GoldyBot-5.0.dev5/GoldyBot/goldy/recipes/buttons/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/recipes/buttons/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     3764 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/recipes/buttons/button.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1812 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/system.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     3580 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/goldy/token.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      404 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/info.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.484566 GoldyBot-5.0.dev5/GoldyBot/internal_extensions/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2809 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/internal_extensions/extensions.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2645 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/internal_extensions/goldy.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     8378 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/internal_extensions/timestamps.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      523 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/logging.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      530 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/GoldyBot/paths.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.486566 GoldyBot-5.0.dev5/GoldyBot/utils/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      181 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/utils/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      375 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/utils/_async.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      283 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/utils/_lambda.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1196 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/utils/cache.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1771 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/utils/human_datetime.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      251 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/GoldyBot/utils/strings.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.473566 GoldyBot-5.0.dev5/GoldyBot.egg-info/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)    47828 2023-07-08 23:43:26.000000 GoldyBot-5.0.dev5/GoldyBot.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     4403 2023-07-08 23:43:26.000000 GoldyBot-5.0.dev5/GoldyBot.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        1 2023-07-08 23:43:26.000000 GoldyBot-5.0.dev5/GoldyBot.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      105 2023-07-08 23:43:26.000000 GoldyBot-5.0.dev5/GoldyBot.egg-info/entry_points.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      289 2023-07-08 23:43:26.000000 GoldyBot-5.0.dev5/GoldyBot.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        9 2023-07-08 23:43:26.000000 GoldyBot-5.0.dev5/GoldyBot.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)    35123 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/LICENSE
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      347 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/Makefile
+-rw-r--r--   0 goldy     (1001) goldy     (1001)    47828 2023-07-08 23:43:26.499566 GoldyBot-5.0.dev5/PKG-INFO
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     6242 2023-07-08 23:42:49.000000 GoldyBot-5.0.dev5/README.md
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.487566 GoldyBot-5.0.dev5/assets/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2049 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/assets/.$software_design_1.drawio.bkp
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2793 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/assets/.$software_design_1.drawio.dtmp
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.487566 GoldyBot-5.0.dev5/assets/goldy_art/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)   581942 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/assets/goldy_art/1.png
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2793 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/assets/software_design_1.drawio
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.489566 GoldyBot-5.0.dev5/demo/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       85 2023-07-04 21:02:56.000000 GoldyBot-5.0.dev5/demo/cli_demo.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      210 2023-06-18 12:02:46.000000 GoldyBot-5.0.dev5/demo/run.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.489566 GoldyBot-5.0.dev5/demo-docker/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        0 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/demo-docker/.gitkeep
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      669 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docker-compose.yml
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.490566 GoldyBot-5.0.dev5/docker_stuff/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       47 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docker_stuff/cli.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       98 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docker_stuff/run.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       84 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docker_stuff/run.sh
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.494566 GoldyBot-5.0.dev5/docs/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      634 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docs/Makefile
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.495566 GoldyBot-5.0.dev5/docs/_static/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)   581942 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docs/_static/logo.png
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      756 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/api_documentation.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      109 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docs/cli.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1818 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/conf.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      137 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/examples.buttons.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      114 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/examples.reply.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      247 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/examples.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      164 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/examples.slash_options.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      149 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/examples.sub_commands.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1021 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/goldy.commands.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      155 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docs/goldy.database.databases.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      225 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/goldy.database.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      325 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/goldy.database.wrappers.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2097 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docs/goldy.extensions.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      243 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docs/goldy.guilds.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      311 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docs/goldy.live_console.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      191 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docs/goldy.nextcore_utils.channels.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      150 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docs/goldy.nextcore_utils.embeds.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      174 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docs/goldy.nextcore_utils.guilds.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      311 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docs/goldy.nextcore_utils.messages.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      515 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/goldy.nextcore_utils.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      192 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docs/goldy.nextcore_utils.slash_options.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      818 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/goldy.objects.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      277 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/goldy.recipes.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      694 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/goldy.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      400 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/index.rst
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      765 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/docs/make.bat
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      639 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/docs/utils.rst
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.497566 GoldyBot-5.0.dev5/examples/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1370 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/examples/buttons.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      387 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/examples/reply.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1286 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/examples/slash_options.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1215 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/examples/sub_commands.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     3255 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/pyproject.toml
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.497566 GoldyBot-5.0.dev5/scripts/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      173 2023-07-08 23:42:49.000000 GoldyBot-5.0.dev5/scripts/add_cname.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      256 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/scripts/docker_build.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       38 2023-07-08 23:43:26.499566 GoldyBot-5.0.dev5/setup.cfg
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.498566 GoldyBot-5.0.dev5/tests/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       95 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/tests/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      167 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/tests/test_config.json
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      609 2023-06-18 11:58:26.000000 GoldyBot-5.0.dev5/tests/test_config.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:43:26.499566 GoldyBot-5.0.dev5/tests/utils/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        0 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/tests/utils/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      785 2023-07-08 23:42:52.000000 GoldyBot-5.0.dev5/tests/utils/test_cache_lookup.py
```

