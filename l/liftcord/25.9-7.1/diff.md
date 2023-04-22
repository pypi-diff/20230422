# Comparing `tmp/liftcord-25.9.tar.gz` & `tmp/liftcord-7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liftcord-25.9.tar", last modified: Sat Apr 22 09:02:38 2023, max compression
+gzip compressed data, was "liftcord-7.1.tar", last modified: Fri Apr 21 20:03:57 2023, max compression
```

## Comparing `liftcord-25.9.tar` & `liftcord-7.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 09:02:38.347267 liftcord-25.9/
--rw-rw-rw-   0        0        0      859 2023-04-22 09:02:38.344269 liftcord-25.9/PKG-INFO
--rw-rw-rw-   0        0        0     2945 2023-04-21 18:00:23.000000 liftcord-25.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-22 09:02:37.391856 liftcord-25.9/liftcord/
--rw-rw-rw-   0        0        0     1888 2023-04-21 19:02:13.000000 liftcord-25.9/liftcord/__init__.py
--rw-rw-rw-   0        0        0    11058 2023-04-21 19:02:34.000000 liftcord-25.9/liftcord/__main__.py
--rw-rw-rw-   0        0        0     1410 2023-04-21 18:00:25.000000 liftcord-25.9/liftcord/_types.py
--rw-rw-rw-   0        0        0    65763 2023-04-21 18:00:25.000000 liftcord-25.9/liftcord/abc.py
--rw-rw-rw-   0        0        0    26864 2023-04-21 18:00:25.000000 liftcord-25.9/liftcord/activity.py
-drwxrwxrwx   0        0        0        0 2023-04-22 09:02:37.563750 liftcord-25.9/liftcord/app_commands/
--rw-rw-rw-   0        0        0      424 2023-04-21 18:00:31.000000 liftcord-25.9/liftcord/app_commands/__init__.py
--rw-rw-rw-   0        0        0    18077 2023-04-21 18:00:31.000000 liftcord-25.9/liftcord/app_commands/checks.py
--rw-rw-rw-   0        0        0    95614 2023-04-21 18:00:31.000000 liftcord-25.9/liftcord/app_commands/commands.py
--rw-rw-rw-   0        0        0    19006 2023-04-21 18:00:31.000000 liftcord-25.9/liftcord/app_commands/errors.py
--rw-rw-rw-   0        0        0    38502 2023-04-21 18:00:31.000000 liftcord-25.9/liftcord/app_commands/models.py
--rw-rw-rw-   0        0        0    13123 2023-04-21 18:00:32.000000 liftcord-25.9/liftcord/app_commands/namespace.py
--rw-rw-rw-   0        0        0    32499 2023-04-21 18:00:32.000000 liftcord-25.9/liftcord/app_commands/transformers.py
--rw-rw-rw-   0        0        0    10686 2023-04-21 18:00:32.000000 liftcord-25.9/liftcord/app_commands/translator.py
--rw-rw-rw-   0        0        0    47965 2023-04-21 18:00:32.000000 liftcord-25.9/liftcord/app_commands/tree.py
--rw-rw-rw-   0        0        0    12713 2023-04-21 18:00:25.000000 liftcord-25.9/liftcord/appinfo.py
--rw-rw-rw-   0        0        0    15837 2023-04-21 18:00:25.000000 liftcord-25.9/liftcord/asset.py
--rw-rw-rw-   0        0        0    35298 2023-04-21 18:00:25.000000 liftcord-25.9/liftcord/audit_logs.py
--rw-rw-rw-   0        0        0    23833 2023-04-21 18:00:25.000000 liftcord-25.9/liftcord/automod.py
--rw-rw-rw-   0        0        0     3751 2023-04-21 18:00:25.000000 liftcord-25.9/liftcord/backoff.py
--rw-rw-rw-   0        0        0   116590 2023-04-21 18:00:26.000000 liftcord-25.9/liftcord/channel.py
--rw-rw-rw-   0        0        0    86215 2023-04-22 00:58:21.000000 liftcord-25.9/liftcord/client.py
--rw-rw-rw-   0        0        0    14168 2023-04-21 18:00:26.000000 liftcord-25.9/liftcord/colour.py
--rw-rw-rw-   0        0        0    16836 2023-04-21 18:00:26.000000 liftcord-25.9/liftcord/components.py
--rw-rw-rw-   0        0        0     3032 2023-04-21 18:00:26.000000 liftcord-25.9/liftcord/context_managers.py
--rw-rw-rw-   0        0        0    22722 2023-04-21 21:12:50.000000 liftcord-25.9/liftcord/embeds.py
--rw-rw-rw-   0        0        0     8574 2023-04-21 18:00:26.000000 liftcord-25.9/liftcord/emoji.py
--rw-rw-rw-   0        0        0    22229 2023-04-21 18:00:26.000000 liftcord-25.9/liftcord/enums.py
--rw-rw-rw-   0        0        0     8952 2023-04-21 18:00:26.000000 liftcord-25.9/liftcord/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-22 09:02:36.831206 liftcord-25.9/liftcord/ext/
-drwxrwxrwx   0        0        0        0 2023-04-22 09:02:37.737643 liftcord-25.9/liftcord/ext/commands/
--rw-rw-rw-   0        0        0      437 2023-04-21 18:00:32.000000 liftcord-25.9/liftcord/ext/commands/__init__.py
--rw-rw-rw-   0        0        0     2638 2023-04-21 18:00:32.000000 liftcord-25.9/liftcord/ext/commands/_types.py
--rw-rw-rw-   0        0        0    51771 2023-04-21 19:01:40.000000 liftcord-25.9/liftcord/ext/commands/bot.py
--rw-rw-rw-   0        0        0    30163 2023-04-21 18:00:33.000000 liftcord-25.9/liftcord/ext/commands/cog.py
--rw-rw-rw-   0        0        0    39689 2023-04-21 18:00:33.000000 liftcord-25.9/liftcord/ext/commands/context.py
--rw-rw-rw-   0        0        0    45402 2023-04-21 18:00:33.000000 liftcord-25.9/liftcord/ext/commands/converter.py
--rw-rw-rw-   0        0        0     9716 2023-04-21 18:00:33.000000 liftcord-25.9/liftcord/ext/commands/cooldowns.py
--rw-rw-rw-   0        0        0    89320 2023-04-21 18:00:33.000000 liftcord-25.9/liftcord/ext/commands/core.py
--rw-rw-rw-   0        0        0    36354 2023-04-21 18:00:33.000000 liftcord-25.9/liftcord/ext/commands/errors.py
--rw-rw-rw-   0        0        0    22966 2023-04-21 18:00:33.000000 liftcord-25.9/liftcord/ext/commands/flags.py
--rw-rw-rw-   0        0        0    57705 2023-04-21 18:00:33.000000 liftcord-25.9/liftcord/ext/commands/help.py
--rw-rw-rw-   0        0        0    36595 2023-04-21 18:00:33.000000 liftcord-25.9/liftcord/ext/commands/hybrid.py
--rw-rw-rw-   0        0        0     8361 2023-04-21 21:16:08.000000 liftcord-25.9/liftcord/ext/commands/parameters.py
--rw-rw-rw-   0        0        0     6247 2023-04-21 18:00:34.000000 liftcord-25.9/liftcord/ext/commands/view.py
-drwxrwxrwx   0        0        0        0 2023-04-22 09:02:37.756631 liftcord-25.9/liftcord/ext/tasks/
--rw-rw-rw-   0        0        0    29180 2023-04-21 18:00:34.000000 liftcord-25.9/liftcord/ext/tasks/__init__.py
--rw-rw-rw-   0        0        0     5378 2023-04-21 18:00:26.000000 liftcord-25.9/liftcord/file.py
--rw-rw-rw-   0        0        0    53230 2023-04-21 18:00:27.000000 liftcord-25.9/liftcord/flags.py
--rw-rw-rw-   0        0        0    35681 2023-04-22 09:01:18.000000 liftcord-25.9/liftcord/gateway.py
--rw-rw-rw-   0        0        0   150604 2023-04-21 18:00:27.000000 liftcord-25.9/liftcord/guild.py
--rw-rw-rw-   0        0        0    89896 2023-04-21 18:00:27.000000 liftcord-25.9/liftcord/http.py
--rw-rw-rw-   0        0        0    13334 2023-04-21 18:00:27.000000 liftcord-25.9/liftcord/integrations.py
--rw-rw-rw-   0        0        0    44610 2023-04-21 18:00:27.000000 liftcord-25.9/liftcord/interactions.py
--rw-rw-rw-   0        0        0    20595 2023-04-21 18:00:27.000000 liftcord-25.9/liftcord/invite.py
--rw-rw-rw-   0        0        0    40760 2023-04-21 18:00:27.000000 liftcord-25.9/liftcord/member.py
--rw-rw-rw-   0        0        0     5592 2023-04-21 18:00:27.000000 liftcord-25.9/liftcord/mentions.py
--rw-rw-rw-   0        0        0    85396 2023-04-21 18:00:27.000000 liftcord-25.9/liftcord/message.py
--rw-rw-rw-   0        0        0     1485 2023-04-21 18:00:27.000000 liftcord-25.9/liftcord/mixins.py
-drwxrwxrwx   0        0        0        0 2023-04-22 09:02:37.776620 liftcord-25.9/liftcord/mobile/
--rw-rw-rw-   0        0        0     1175 2023-04-21 19:08:03.000000 liftcord-25.9/liftcord/mobile/__init__.py
--rw-rw-rw-   0        0        0     3702 2023-04-21 18:00:28.000000 liftcord-25.9/liftcord/object.py
--rw-rw-rw-   0        0        0     3646 2023-04-21 18:00:28.000000 liftcord-25.9/liftcord/oggparse.py
--rw-rw-rw-   0        0        0    15065 2023-04-21 18:00:28.000000 liftcord-25.9/liftcord/opus.py
--rw-rw-rw-   0        0        0     7950 2023-04-21 18:00:28.000000 liftcord-25.9/liftcord/partial_emoji.py
--rw-rw-rw-   0        0        0    29602 2023-04-21 18:00:28.000000 liftcord-25.9/liftcord/permissions.py
--rw-rw-rw-   0        0        0    26456 2023-04-21 18:00:28.000000 liftcord-25.9/liftcord/player.py
--rw-rw-rw-   0        0        0    31867 2023-04-21 19:04:49.000000 liftcord-25.9/liftcord/pylogz.py
--rw-rw-rw-   0        0        0    16826 2023-04-21 18:00:28.000000 liftcord-25.9/liftcord/raw_models.py
--rw-rw-rw-   0        0        0     8229 2023-04-21 18:00:28.000000 liftcord-25.9/liftcord/reaction.py
--rw-rw-rw-   0        0        0    17906 2023-04-21 18:00:28.000000 liftcord-25.9/liftcord/role.py
--rw-rw-rw-   0        0        0    23629 2023-04-21 18:00:29.000000 liftcord-25.9/liftcord/scheduled_event.py
--rw-rw-rw-   0        0        0    20129 2023-04-21 18:00:29.000000 liftcord-25.9/liftcord/shard.py
--rw-rw-rw-   0        0        0     6498 2023-04-21 18:00:29.000000 liftcord-25.9/liftcord/stage_instance.py
--rw-rw-rw-   0        0        0    73339 2023-04-21 18:00:29.000000 liftcord-25.9/liftcord/state.py
--rw-rw-rw-   0        0        0    16039 2023-04-21 18:00:29.000000 liftcord-25.9/liftcord/sticker.py
--rw-rw-rw-   0        0        0     4607 2023-04-21 18:00:29.000000 liftcord-25.9/liftcord/team.py
--rw-rw-rw-   0        0        0     9574 2023-04-21 18:00:29.000000 liftcord-25.9/liftcord/template.py
--rw-rw-rw-   0        0        0    32456 2023-04-21 18:00:30.000000 liftcord-25.9/liftcord/threads.py
-drwxrwxrwx   0        0        0        0 2023-04-22 09:02:38.093423 liftcord-25.9/liftcord/types/
--rw-rw-rw-   0        0        0      149 2023-04-21 18:00:34.000000 liftcord-25.9/liftcord/types/__init__.py
--rw-rw-rw-   0        0        0     2707 2023-04-21 18:00:34.000000 liftcord-25.9/liftcord/types/activity.py
--rw-rw-rw-   0        0        0     2487 2023-04-21 18:00:34.000000 liftcord-25.9/liftcord/types/appinfo.py
--rw-rw-rw-   0        0        0     8192 2023-04-21 18:00:34.000000 liftcord-25.9/liftcord/types/audit_log.py
--rw-rw-rw-   0        0        0     4009 2023-04-21 18:00:34.000000 liftcord-25.9/liftcord/types/automod.py
--rw-rw-rw-   0        0        0     4637 2023-04-21 18:00:34.000000 liftcord-25.9/liftcord/types/channel.py
--rw-rw-rw-   0        0        0     6266 2023-04-21 18:00:34.000000 liftcord-25.9/liftcord/types/command.py
--rw-rw-rw-   0        0        0     3057 2023-04-21 18:00:34.000000 liftcord-25.9/liftcord/types/components.py
--rw-rw-rw-   0        0        0     2329 2023-04-21 18:00:34.000000 liftcord-25.9/liftcord/types/embed.py
--rw-rw-rw-   0        0        0     1528 2023-04-21 18:00:35.000000 liftcord-25.9/liftcord/types/emoji.py
--rw-rw-rw-   0        0        0     8453 2023-04-21 18:00:35.000000 liftcord-25.9/liftcord/types/gateway.py
--rw-rw-rw-   0        0        0     5279 2023-04-21 18:00:35.000000 liftcord-25.9/liftcord/types/guild.py
--rw-rw-rw-   0        0        0     2288 2023-04-21 18:00:35.000000 liftcord-25.9/liftcord/types/integration.py
--rw-rw-rw-   0        0        0     6923 2023-04-21 18:00:35.000000 liftcord-25.9/liftcord/types/interactions.py
--rw-rw-rw-   0        0        0     2704 2023-04-21 18:00:35.000000 liftcord-25.9/liftcord/types/invite.py
--rw-rw-rw-   0        0        0     1898 2023-04-21 18:00:35.000000 liftcord-25.9/liftcord/types/member.py
--rw-rw-rw-   0        0        0     4251 2023-04-21 18:00:35.000000 liftcord-25.9/liftcord/types/message.py
--rw-rw-rw-   0        0        0     1746 2023-04-21 18:00:35.000000 liftcord-25.9/liftcord/types/role.py
--rw-rw-rw-   0        0        0     3294 2023-04-21 18:00:35.000000 liftcord-25.9/liftcord/types/scheduled_event.py
--rw-rw-rw-   0        0        0     1182 2023-04-21 18:00:35.000000 liftcord-25.9/liftcord/types/snowflake.py
--rw-rw-rw-   0        0        0     2257 2023-04-21 18:00:35.000000 liftcord-25.9/liftcord/types/sticker.py
--rw-rw-rw-   0        0        0     1499 2023-04-21 18:00:35.000000 liftcord-25.9/liftcord/types/team.py
--rw-rw-rw-   0        0        0     1609 2023-04-21 18:00:35.000000 liftcord-25.9/liftcord/types/template.py
--rw-rw-rw-   0        0        0     2454 2023-04-21 18:00:36.000000 liftcord-25.9/liftcord/types/threads.py
--rw-rw-rw-   0        0        0     1540 2023-04-21 18:00:36.000000 liftcord-25.9/liftcord/types/user.py
--rw-rw-rw-   0        0        0     2268 2023-04-21 18:00:36.000000 liftcord-25.9/liftcord/types/voice.py
--rw-rw-rw-   0        0        0     1978 2023-04-21 18:00:36.000000 liftcord-25.9/liftcord/types/webhook.py
--rw-rw-rw-   0        0        0     1460 2023-04-21 18:00:36.000000 liftcord-25.9/liftcord/types/welcome_screen.py
--rw-rw-rw-   0        0        0     1883 2023-04-21 18:00:36.000000 liftcord-25.9/liftcord/types/widget.py
-drwxrwxrwx   0        0        0        0 2023-04-22 09:02:38.218346 liftcord-25.9/liftcord/ui/
--rw-rw-rw-   0        0        0      285 2023-04-21 18:00:36.000000 liftcord-25.9/liftcord/ui/__init__.py
--rw-rw-rw-   0        0        0    10620 2023-04-21 18:00:37.000000 liftcord-25.9/liftcord/ui/button.py
--rw-rw-rw-   0        0        0     4372 2023-04-21 18:00:37.000000 liftcord-25.9/liftcord/ui/item.py
--rw-rw-rw-   0        0        0     7012 2023-04-21 18:00:37.000000 liftcord-25.9/liftcord/ui/modal.py
--rw-rw-rw-   0        0        0    34049 2023-04-21 18:00:37.000000 liftcord-25.9/liftcord/ui/select.py
--rw-rw-rw-   0        0        0     8058 2023-04-21 18:00:37.000000 liftcord-25.9/liftcord/ui/text_input.py
--rw-rw-rw-   0        0        0    22878 2023-04-21 18:00:37.000000 liftcord-25.9/liftcord/ui/view.py
--rw-rw-rw-   0        0        0    15390 2023-04-21 18:00:30.000000 liftcord-25.9/liftcord/user.py
--rw-rw-rw-   0        0        0    41460 2023-04-21 18:00:30.000000 liftcord-25.9/liftcord/utils.py
--rw-rw-rw-   0        0        0    24974 2023-04-21 18:00:30.000000 liftcord-25.9/liftcord/voice_client.py
-drwxrwxrwx   0        0        0        0 2023-04-22 09:02:38.236334 liftcord-25.9/liftcord/webhook/
--rw-rw-rw-   0        0        0      182 2023-04-21 18:00:37.000000 liftcord-25.9/liftcord/webhook/__init__.py
--rw-rw-rw-   0        0        0    69566 2023-04-21 18:00:37.000000 liftcord-25.9/liftcord/webhook/async_.py
--rw-rw-rw-   0        0        0    42587 2023-04-21 18:00:38.000000 liftcord-25.9/liftcord/webhook/sync.py
--rw-rw-rw-   0        0        0     7539 2023-04-21 18:00:30.000000 liftcord-25.9/liftcord/welcome_screen.py
--rw-rw-rw-   0        0        0    10168 2023-04-21 18:00:31.000000 liftcord-25.9/liftcord/widget.py
-drwxrwxrwx   0        0        0        0 2023-04-22 09:02:37.483801 liftcord-25.9/liftcord.egg-info/
--rw-rw-rw-   0        0        0      859 2023-04-22 09:02:36.000000 liftcord-25.9/liftcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3094 2023-04-22 09:02:36.000000 liftcord-25.9/liftcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 09:02:36.000000 liftcord-25.9/liftcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-22 09:02:36.000000 liftcord-25.9/liftcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-22 09:02:36.000000 liftcord-25.9/liftcord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 09:02:38.348266 liftcord-25.9/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-04-22 09:01:23.000000 liftcord-25.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:03:57.512354 liftcord-7.1/
+-rw-rw-rw-   0        0        0      858 2023-04-21 20:03:57.457389 liftcord-7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2945 2023-04-21 18:00:23.000000 liftcord-7.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 20:03:56.440017 liftcord-7.1/liftcord/
+-rw-rw-rw-   0        0        0     1888 2023-04-21 19:02:13.000000 liftcord-7.1/liftcord/__init__.py
+-rw-rw-rw-   0        0        0    11058 2023-04-21 19:02:34.000000 liftcord-7.1/liftcord/__main__.py
+-rw-rw-rw-   0        0        0     1410 2023-04-21 18:00:25.000000 liftcord-7.1/liftcord/_types.py
+-rw-rw-rw-   0        0        0    65763 2023-04-21 18:00:25.000000 liftcord-7.1/liftcord/abc.py
+-rw-rw-rw-   0        0        0    26864 2023-04-21 18:00:25.000000 liftcord-7.1/liftcord/activity.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:03:56.703853 liftcord-7.1/liftcord/app_commands/
+-rw-rw-rw-   0        0        0      424 2023-04-21 18:00:31.000000 liftcord-7.1/liftcord/app_commands/__init__.py
+-rw-rw-rw-   0        0        0    18077 2023-04-21 18:00:31.000000 liftcord-7.1/liftcord/app_commands/checks.py
+-rw-rw-rw-   0        0        0    95614 2023-04-21 18:00:31.000000 liftcord-7.1/liftcord/app_commands/commands.py
+-rw-rw-rw-   0        0        0    19006 2023-04-21 18:00:31.000000 liftcord-7.1/liftcord/app_commands/errors.py
+-rw-rw-rw-   0        0        0    38502 2023-04-21 18:00:31.000000 liftcord-7.1/liftcord/app_commands/models.py
+-rw-rw-rw-   0        0        0    13123 2023-04-21 18:00:32.000000 liftcord-7.1/liftcord/app_commands/namespace.py
+-rw-rw-rw-   0        0        0    32499 2023-04-21 18:00:32.000000 liftcord-7.1/liftcord/app_commands/transformers.py
+-rw-rw-rw-   0        0        0    10686 2023-04-21 18:00:32.000000 liftcord-7.1/liftcord/app_commands/translator.py
+-rw-rw-rw-   0        0        0    47965 2023-04-21 18:00:32.000000 liftcord-7.1/liftcord/app_commands/tree.py
+-rw-rw-rw-   0        0        0    12713 2023-04-21 18:00:25.000000 liftcord-7.1/liftcord/appinfo.py
+-rw-rw-rw-   0        0        0    15837 2023-04-21 18:00:25.000000 liftcord-7.1/liftcord/asset.py
+-rw-rw-rw-   0        0        0    35298 2023-04-21 18:00:25.000000 liftcord-7.1/liftcord/audit_logs.py
+-rw-rw-rw-   0        0        0    23833 2023-04-21 18:00:25.000000 liftcord-7.1/liftcord/automod.py
+-rw-rw-rw-   0        0        0     3751 2023-04-21 18:00:25.000000 liftcord-7.1/liftcord/backoff.py
+-rw-rw-rw-   0        0        0   116590 2023-04-21 18:00:26.000000 liftcord-7.1/liftcord/channel.py
+-rw-rw-rw-   0        0        0    86035 2023-04-21 20:02:20.000000 liftcord-7.1/liftcord/client.py
+-rw-rw-rw-   0        0        0    14168 2023-04-21 18:00:26.000000 liftcord-7.1/liftcord/colour.py
+-rw-rw-rw-   0        0        0    16836 2023-04-21 18:00:26.000000 liftcord-7.1/liftcord/components.py
+-rw-rw-rw-   0        0        0     3032 2023-04-21 18:00:26.000000 liftcord-7.1/liftcord/context_managers.py
+-rw-rw-rw-   0        0        0    22722 2023-04-21 18:00:26.000000 liftcord-7.1/liftcord/embeds.py
+-rw-rw-rw-   0        0        0     8574 2023-04-21 18:00:26.000000 liftcord-7.1/liftcord/emoji.py
+-rw-rw-rw-   0        0        0    22229 2023-04-21 18:00:26.000000 liftcord-7.1/liftcord/enums.py
+-rw-rw-rw-   0        0        0     8952 2023-04-21 18:00:26.000000 liftcord-7.1/liftcord/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:03:55.724459 liftcord-7.1/liftcord/ext/
+drwxrwxrwx   0        0        0        0 2023-04-21 20:03:56.900732 liftcord-7.1/liftcord/ext/commands/
+-rw-rw-rw-   0        0        0      437 2023-04-21 18:00:32.000000 liftcord-7.1/liftcord/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     2638 2023-04-21 18:00:32.000000 liftcord-7.1/liftcord/ext/commands/_types.py
+-rw-rw-rw-   0        0        0    51771 2023-04-21 19:01:40.000000 liftcord-7.1/liftcord/ext/commands/bot.py
+-rw-rw-rw-   0        0        0    30163 2023-04-21 18:00:33.000000 liftcord-7.1/liftcord/ext/commands/cog.py
+-rw-rw-rw-   0        0        0    39689 2023-04-21 18:00:33.000000 liftcord-7.1/liftcord/ext/commands/context.py
+-rw-rw-rw-   0        0        0    45402 2023-04-21 18:00:33.000000 liftcord-7.1/liftcord/ext/commands/converter.py
+-rw-rw-rw-   0        0        0     9716 2023-04-21 18:00:33.000000 liftcord-7.1/liftcord/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0    89320 2023-04-21 18:00:33.000000 liftcord-7.1/liftcord/ext/commands/core.py
+-rw-rw-rw-   0        0        0    36354 2023-04-21 18:00:33.000000 liftcord-7.1/liftcord/ext/commands/errors.py
+-rw-rw-rw-   0        0        0    22966 2023-04-21 18:00:33.000000 liftcord-7.1/liftcord/ext/commands/flags.py
+-rw-rw-rw-   0        0        0    57705 2023-04-21 18:00:33.000000 liftcord-7.1/liftcord/ext/commands/help.py
+-rw-rw-rw-   0        0        0    36595 2023-04-21 18:00:33.000000 liftcord-7.1/liftcord/ext/commands/hybrid.py
+-rw-rw-rw-   0        0        0     8361 2023-04-21 18:00:34.000000 liftcord-7.1/liftcord/ext/commands/parameters.py
+-rw-rw-rw-   0        0        0     6247 2023-04-21 18:00:34.000000 liftcord-7.1/liftcord/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:03:56.904729 liftcord-7.1/liftcord/ext/tasks/
+-rw-rw-rw-   0        0        0    29180 2023-04-21 18:00:34.000000 liftcord-7.1/liftcord/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0     5378 2023-04-21 18:00:26.000000 liftcord-7.1/liftcord/file.py
+-rw-rw-rw-   0        0        0    53230 2023-04-21 18:00:27.000000 liftcord-7.1/liftcord/flags.py
+-rw-rw-rw-   0        0        0    35191 2023-04-21 18:00:27.000000 liftcord-7.1/liftcord/gateway.py
+-rw-rw-rw-   0        0        0   150604 2023-04-21 18:00:27.000000 liftcord-7.1/liftcord/guild.py
+-rw-rw-rw-   0        0        0    89896 2023-04-21 18:00:27.000000 liftcord-7.1/liftcord/http.py
+-rw-rw-rw-   0        0        0    13334 2023-04-21 18:00:27.000000 liftcord-7.1/liftcord/integrations.py
+-rw-rw-rw-   0        0        0    44610 2023-04-21 18:00:27.000000 liftcord-7.1/liftcord/interactions.py
+-rw-rw-rw-   0        0        0    20595 2023-04-21 18:00:27.000000 liftcord-7.1/liftcord/invite.py
+-rw-rw-rw-   0        0        0    40760 2023-04-21 18:00:27.000000 liftcord-7.1/liftcord/member.py
+-rw-rw-rw-   0        0        0     5592 2023-04-21 18:00:27.000000 liftcord-7.1/liftcord/mentions.py
+-rw-rw-rw-   0        0        0    85396 2023-04-21 18:00:27.000000 liftcord-7.1/liftcord/message.py
+-rw-rw-rw-   0        0        0     1485 2023-04-21 18:00:27.000000 liftcord-7.1/liftcord/mixins.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:03:56.909726 liftcord-7.1/liftcord/mobile/
+-rw-rw-rw-   0        0        0     1175 2023-04-21 19:08:03.000000 liftcord-7.1/liftcord/mobile/__init__.py
+-rw-rw-rw-   0        0        0     3702 2023-04-21 18:00:28.000000 liftcord-7.1/liftcord/object.py
+-rw-rw-rw-   0        0        0     3646 2023-04-21 18:00:28.000000 liftcord-7.1/liftcord/oggparse.py
+-rw-rw-rw-   0        0        0    15065 2023-04-21 18:00:28.000000 liftcord-7.1/liftcord/opus.py
+-rw-rw-rw-   0        0        0     7950 2023-04-21 18:00:28.000000 liftcord-7.1/liftcord/partial_emoji.py
+-rw-rw-rw-   0        0        0    29602 2023-04-21 18:00:28.000000 liftcord-7.1/liftcord/permissions.py
+-rw-rw-rw-   0        0        0    26456 2023-04-21 18:00:28.000000 liftcord-7.1/liftcord/player.py
+-rw-rw-rw-   0        0        0    31867 2023-04-21 19:04:49.000000 liftcord-7.1/liftcord/pylogz.py
+-rw-rw-rw-   0        0        0    16826 2023-04-21 18:00:28.000000 liftcord-7.1/liftcord/raw_models.py
+-rw-rw-rw-   0        0        0     8229 2023-04-21 18:00:28.000000 liftcord-7.1/liftcord/reaction.py
+-rw-rw-rw-   0        0        0    17906 2023-04-21 18:00:28.000000 liftcord-7.1/liftcord/role.py
+-rw-rw-rw-   0        0        0    23629 2023-04-21 18:00:29.000000 liftcord-7.1/liftcord/scheduled_event.py
+-rw-rw-rw-   0        0        0    20129 2023-04-21 18:00:29.000000 liftcord-7.1/liftcord/shard.py
+-rw-rw-rw-   0        0        0     6498 2023-04-21 18:00:29.000000 liftcord-7.1/liftcord/stage_instance.py
+-rw-rw-rw-   0        0        0    73339 2023-04-21 18:00:29.000000 liftcord-7.1/liftcord/state.py
+-rw-rw-rw-   0        0        0    16039 2023-04-21 18:00:29.000000 liftcord-7.1/liftcord/sticker.py
+-rw-rw-rw-   0        0        0     4607 2023-04-21 18:00:29.000000 liftcord-7.1/liftcord/team.py
+-rw-rw-rw-   0        0        0     9574 2023-04-21 18:00:29.000000 liftcord-7.1/liftcord/template.py
+-rw-rw-rw-   0        0        0    32456 2023-04-21 18:00:30.000000 liftcord-7.1/liftcord/threads.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:03:57.300484 liftcord-7.1/liftcord/types/
+-rw-rw-rw-   0        0        0      149 2023-04-21 18:00:34.000000 liftcord-7.1/liftcord/types/__init__.py
+-rw-rw-rw-   0        0        0     2707 2023-04-21 18:00:34.000000 liftcord-7.1/liftcord/types/activity.py
+-rw-rw-rw-   0        0        0     2487 2023-04-21 18:00:34.000000 liftcord-7.1/liftcord/types/appinfo.py
+-rw-rw-rw-   0        0        0     8192 2023-04-21 18:00:34.000000 liftcord-7.1/liftcord/types/audit_log.py
+-rw-rw-rw-   0        0        0     4009 2023-04-21 18:00:34.000000 liftcord-7.1/liftcord/types/automod.py
+-rw-rw-rw-   0        0        0     4637 2023-04-21 18:00:34.000000 liftcord-7.1/liftcord/types/channel.py
+-rw-rw-rw-   0        0        0     6266 2023-04-21 18:00:34.000000 liftcord-7.1/liftcord/types/command.py
+-rw-rw-rw-   0        0        0     3057 2023-04-21 18:00:34.000000 liftcord-7.1/liftcord/types/components.py
+-rw-rw-rw-   0        0        0     2329 2023-04-21 18:00:34.000000 liftcord-7.1/liftcord/types/embed.py
+-rw-rw-rw-   0        0        0     1528 2023-04-21 18:00:35.000000 liftcord-7.1/liftcord/types/emoji.py
+-rw-rw-rw-   0        0        0     8453 2023-04-21 18:00:35.000000 liftcord-7.1/liftcord/types/gateway.py
+-rw-rw-rw-   0        0        0     5279 2023-04-21 18:00:35.000000 liftcord-7.1/liftcord/types/guild.py
+-rw-rw-rw-   0        0        0     2288 2023-04-21 18:00:35.000000 liftcord-7.1/liftcord/types/integration.py
+-rw-rw-rw-   0        0        0     6923 2023-04-21 18:00:35.000000 liftcord-7.1/liftcord/types/interactions.py
+-rw-rw-rw-   0        0        0     2704 2023-04-21 18:00:35.000000 liftcord-7.1/liftcord/types/invite.py
+-rw-rw-rw-   0        0        0     1898 2023-04-21 18:00:35.000000 liftcord-7.1/liftcord/types/member.py
+-rw-rw-rw-   0        0        0     4251 2023-04-21 18:00:35.000000 liftcord-7.1/liftcord/types/message.py
+-rw-rw-rw-   0        0        0     1746 2023-04-21 18:00:35.000000 liftcord-7.1/liftcord/types/role.py
+-rw-rw-rw-   0        0        0     3294 2023-04-21 18:00:35.000000 liftcord-7.1/liftcord/types/scheduled_event.py
+-rw-rw-rw-   0        0        0     1182 2023-04-21 18:00:35.000000 liftcord-7.1/liftcord/types/snowflake.py
+-rw-rw-rw-   0        0        0     2257 2023-04-21 18:00:35.000000 liftcord-7.1/liftcord/types/sticker.py
+-rw-rw-rw-   0        0        0     1499 2023-04-21 18:00:35.000000 liftcord-7.1/liftcord/types/team.py
+-rw-rw-rw-   0        0        0     1609 2023-04-21 18:00:35.000000 liftcord-7.1/liftcord/types/template.py
+-rw-rw-rw-   0        0        0     2454 2023-04-21 18:00:36.000000 liftcord-7.1/liftcord/types/threads.py
+-rw-rw-rw-   0        0        0     1540 2023-04-21 18:00:36.000000 liftcord-7.1/liftcord/types/user.py
+-rw-rw-rw-   0        0        0     2268 2023-04-21 18:00:36.000000 liftcord-7.1/liftcord/types/voice.py
+-rw-rw-rw-   0        0        0     1978 2023-04-21 18:00:36.000000 liftcord-7.1/liftcord/types/webhook.py
+-rw-rw-rw-   0        0        0     1460 2023-04-21 18:00:36.000000 liftcord-7.1/liftcord/types/welcome_screen.py
+-rw-rw-rw-   0        0        0     1883 2023-04-21 18:00:36.000000 liftcord-7.1/liftcord/types/widget.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:03:57.370442 liftcord-7.1/liftcord/ui/
+-rw-rw-rw-   0        0        0      285 2023-04-21 18:00:36.000000 liftcord-7.1/liftcord/ui/__init__.py
+-rw-rw-rw-   0        0        0    10620 2023-04-21 18:00:37.000000 liftcord-7.1/liftcord/ui/button.py
+-rw-rw-rw-   0        0        0     4372 2023-04-21 18:00:37.000000 liftcord-7.1/liftcord/ui/item.py
+-rw-rw-rw-   0        0        0     7012 2023-04-21 18:00:37.000000 liftcord-7.1/liftcord/ui/modal.py
+-rw-rw-rw-   0        0        0    34049 2023-04-21 18:00:37.000000 liftcord-7.1/liftcord/ui/select.py
+-rw-rw-rw-   0        0        0     8058 2023-04-21 18:00:37.000000 liftcord-7.1/liftcord/ui/text_input.py
+-rw-rw-rw-   0        0        0    22878 2023-04-21 18:00:37.000000 liftcord-7.1/liftcord/ui/view.py
+-rw-rw-rw-   0        0        0    15390 2023-04-21 18:00:30.000000 liftcord-7.1/liftcord/user.py
+-rw-rw-rw-   0        0        0    41460 2023-04-21 18:00:30.000000 liftcord-7.1/liftcord/utils.py
+-rw-rw-rw-   0        0        0    24974 2023-04-21 18:00:30.000000 liftcord-7.1/liftcord/voice_client.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:03:57.452390 liftcord-7.1/liftcord/webhook/
+-rw-rw-rw-   0        0        0      182 2023-04-21 18:00:37.000000 liftcord-7.1/liftcord/webhook/__init__.py
+-rw-rw-rw-   0        0        0    69566 2023-04-21 18:00:37.000000 liftcord-7.1/liftcord/webhook/async_.py
+-rw-rw-rw-   0        0        0    42587 2023-04-21 18:00:38.000000 liftcord-7.1/liftcord/webhook/sync.py
+-rw-rw-rw-   0        0        0     7539 2023-04-21 18:00:30.000000 liftcord-7.1/liftcord/welcome_screen.py
+-rw-rw-rw-   0        0        0    10168 2023-04-21 18:00:31.000000 liftcord-7.1/liftcord/widget.py
+drwxrwxrwx   0        0        0        0 2023-04-21 20:03:56.575932 liftcord-7.1/liftcord.egg-info/
+-rw-rw-rw-   0        0        0      858 2023-04-21 20:03:55.000000 liftcord-7.1/liftcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3094 2023-04-21 20:03:55.000000 liftcord-7.1/liftcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 20:03:55.000000 liftcord-7.1/liftcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-21 20:03:55.000000 liftcord-7.1/liftcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 20:03:55.000000 liftcord-7.1/liftcord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 20:03:57.519350 liftcord-7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1215 2023-04-21 20:03:15.000000 liftcord-7.1/setup.py
```

### Comparing `liftcord-25.9/PKG-INFO` & `liftcord-7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liftcord
-Version: 25.9
+Version: 7.1
 Summary: A Python wrapper for the Discord API
 Home-page: https://github.com/devliftz/lift.py
 Author: go.
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `liftcord-25.9/README.rst` & `liftcord-7.1/README.rst`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/__init__.py` & `liftcord-7.1/liftcord/__init__.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/__main__.py` & `liftcord-7.1/liftcord/__main__.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/_types.py` & `liftcord-7.1/liftcord/_types.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/abc.py` & `liftcord-7.1/liftcord/abc.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/activity.py` & `liftcord-7.1/liftcord/activity.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/app_commands/checks.py` & `liftcord-7.1/liftcord/app_commands/checks.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/app_commands/commands.py` & `liftcord-7.1/liftcord/app_commands/commands.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/app_commands/errors.py` & `liftcord-7.1/liftcord/app_commands/errors.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/app_commands/models.py` & `liftcord-7.1/liftcord/app_commands/models.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/app_commands/namespace.py` & `liftcord-7.1/liftcord/app_commands/namespace.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/app_commands/transformers.py` & `liftcord-7.1/liftcord/app_commands/transformers.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/app_commands/translator.py` & `liftcord-7.1/liftcord/app_commands/translator.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/app_commands/tree.py` & `liftcord-7.1/liftcord/app_commands/tree.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/appinfo.py` & `liftcord-7.1/liftcord/appinfo.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/asset.py` & `liftcord-7.1/liftcord/asset.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/audit_logs.py` & `liftcord-7.1/liftcord/audit_logs.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/automod.py` & `liftcord-7.1/liftcord/automod.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/backoff.py` & `liftcord-7.1/liftcord/backoff.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/channel.py` & `liftcord-7.1/liftcord/channel.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/client.py` & `liftcord-7.1/liftcord/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
-import os
+
 import liftcord
 import asyncio
 import datetime
 from datetime import datetime
 import logging
 from typing import (
     TYPE_CHECKING,
@@ -75,33 +75,35 @@
 from .appinfo import AppInfo
 from .ui.view import View
 from .stage_instance import StageInstance
 from .threads import Thread
 from .sticker import GuildSticker, StandardSticker, StickerPack, _sticker_factory
 from .pylogz import Colorate, Colors
 
-now = datetime.now()
-ctzo = now.strftime("%Y-%m-%d")
-cto = now.strftime("%H:%M:%S")
-cvf = os.getcwd()
-ghda = ctzo + " " + cto
-
-print(f"""
-
-\033[31moooo   o8o   .o88o.     .\033[0m                                     \033[0mVersion: {liftcord.__version__}\033[0m              
-\033[31m `888   `"'   888 `"\   .o8                                   \033[0mAPI Server: api.icey.fr\033[0m
- \033[33m888  oooo  o888oo  .o888oo      oo.ooooo.  oooo    ooo\033[0m       \033[0mCurrent date: {ctzo}\033[0m
- \033[32m888  `888   888      888        888' `88b  `88.  .8'\033[0m         \033[0mCurrent time: {cto}\033[0m
- \033[34m888   888   888      888        888   888   `88..8'\033[0m          \033[0mFile path: {cvf}\033[0m
- \033[36m888   888   888      888 . .o.  888   888    `888'\033[0m           
-\033[35mo888o o888o o888o     `888" Y8P  888bod8P'     .8'\033[0m     
-                                 \033[31m888       .o..P'\033[0m      
-                                \033[31mo888o      `Y8P'\033[0m   
-                                
-                                """)
+ct = datetime.now()
+cto = ct.strftime(f"%H:%M")
+
+ctz = ct.date()
+ctzo = ctz.strftime(f"%Y %m %d")
+
+print(Colorate.Horizontal(Colors.purple_to_blue, f"""
+
+    oooo   o8o   .o88o.     .                                     Version: {liftcord.__version__}              
+    `888   `"'   888 `"   .o8                                     API Server: api.icey.fr
+     888  oooo  o888oo  .o888oo     oo.ooooo.  oooo    ooo        Current date: {ctzo}
+     888  `888   888      888        888' `88b  `88.  .8'         Current time: {cto}
+     888   888   888      888        888   888   `88..8'          File path: {__file__}
+     888   888   888      888 . .o.  888   888    `888'           
+    o888o o888o o888o     "888" Y8P  888bod8P'     .8'     
+                                     888       .o..P'      
+                                    o888o      `Y8P'       
+                                                       
+                                             
+                                             
+                                             """))
 
 if TYPE_CHECKING:
     from types import TracebackType
 
     from typing_extensions import Self
 
     from .abc import Messageable, PrivateChannel, Snowflake, SnowflakeTime
@@ -618,16 +620,16 @@
         LoginFailure
             The wrong credentials are passed.
         HTTPException
             An unknown HTTP related error occurred,
             usually when it isn't 200 or the known incorrect credentials
             passing status code.
         """
-        print(f"\033[31mI \033[33m{ghda} \033[32mliftcord.client \033[0m\033[1mLogging in using static token")
-        print(f"\033[31mI \033[33m{ghda} \033[32mliftcord.api \033[0m\033[1mConnected to api.icey.fr")
+
+        _log.info('logging in using static token')
 
         if self.loop is _loop:
             await self._async_setup_hook()
 
         if not isinstance(token, str):
             raise TypeError(f'expected token to be a str, received {token.__class__.__name__} instead')
         token = token.strip()
```

### Comparing `liftcord-25.9/liftcord/colour.py` & `liftcord-7.1/liftcord/colour.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/components.py` & `liftcord-7.1/liftcord/components.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/context_managers.py` & `liftcord-7.1/liftcord/context_managers.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/embeds.py` & `liftcord-7.1/liftcord/embeds.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/emoji.py` & `liftcord-7.1/liftcord/emoji.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/enums.py` & `liftcord-7.1/liftcord/enums.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/errors.py` & `liftcord-7.1/liftcord/errors.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ext/commands/_types.py` & `liftcord-7.1/liftcord/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ext/commands/bot.py` & `liftcord-7.1/liftcord/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ext/commands/cog.py` & `liftcord-7.1/liftcord/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ext/commands/context.py` & `liftcord-7.1/liftcord/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ext/commands/converter.py` & `liftcord-7.1/liftcord/ext/commands/converter.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ext/commands/cooldowns.py` & `liftcord-7.1/liftcord/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ext/commands/core.py` & `liftcord-7.1/liftcord/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ext/commands/errors.py` & `liftcord-7.1/liftcord/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ext/commands/flags.py` & `liftcord-7.1/liftcord/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ext/commands/help.py` & `liftcord-7.1/liftcord/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ext/commands/hybrid.py` & `liftcord-7.1/liftcord/ext/commands/hybrid.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ext/commands/parameters.py` & `liftcord-7.1/liftcord/ext/commands/parameters.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ext/commands/view.py` & `liftcord-7.1/liftcord/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ext/tasks/__init__.py` & `liftcord-7.1/liftcord/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/file.py` & `liftcord-7.1/liftcord/file.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/flags.py` & `liftcord-7.1/liftcord/flags.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/gateway.py` & `liftcord-7.1/liftcord/gateway.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,25 +26,17 @@
 import asyncio
 from collections import deque
 import concurrent.futures
 import logging
 import struct
 import sys
 import time
-import os
 import threading
 import traceback
 import zlib
-from datetime import datetime
-
-now = datetime.now()
-ctzo = now.strftime("%Y-%m-%d")
-cto = now.strftime("%H:%M:%S")
-cvf = os.getcwd()
-ghda = ctzo + " " + cto
 
 from typing import Any, Callable, Coroutine, Deque, Dict, List, TYPE_CHECKING, NamedTuple, Optional, TypeVar
 
 import aiohttp
 import yarl
 
 from . import utils
@@ -123,15 +115,15 @@
         self.remaining -= 1
         return 0.0
 
     async def block(self) -> None:
         async with self.lock:
             delta = self.get_delay()
             if delta:
-                print(f"\033[31mI \033[33m{ghda} \033[32mliftcord.gateway \033[0m\033[1mWebsocket in Shard ID {self.shard_id} is ratelimited.")
+                _log.warning('WebSocket in shard ID %s is ratelimited, waiting %.2f seconds', self.shard_id, delta)
                 await asyncio.sleep(delta)
 
 
 class KeepAliveHandler(threading.Thread):
     def __init__(
         self,
         *args: Any,
@@ -155,15 +147,15 @@
         self._last_recv: float = time.perf_counter()
         self.latency: float = float('inf')
         self.heartbeat_timeout: float = ws._max_heartbeat_timeout
 
     def run(self) -> None:
         while not self._stop_ev.wait(self.interval):
             if self._last_recv + self.heartbeat_timeout < time.perf_counter():
-                print(f"\033[31mI \033[33m{ghda} \033[32mliftcord.gateway \033[0m\033[1mShard ID {self.shard_id} has stoppe responding. Closing and restarting")
+                _log.warning("Shard ID %s has stopped responding to the gateway. Closing and restarting.", self.shard_id)
                 coro = self.ws.close(4000)
                 f = asyncio.run_coroutine_threadsafe(coro, loop=self.ws.loop)
 
                 try:
                     f.result()
                 except Exception:
                     _log.exception('An error occurred while stopping the gateway. Ignoring.')
@@ -397,15 +389,15 @@
 
         if client._enable_debug_events:
             ws.send = ws.debug_send
             ws.log_receive = ws.debug_log_receive
 
         client._connection._update_references(ws)
 
-        print(f"\033[31mI \033[33m{ghda} \033[32mliftcord.gateway \033[0m\033[1mCreated Websocket connected to {gateway}")
+        _log.debug('Created websocket connected to %s', gateway)
 
         # poll event for OP Hello
         await ws.poll_event()
 
         if not resume:
             await ws.identify()
             return ws
@@ -472,44 +464,44 @@
             }
 
         if state._intents is not None:
             payload['d']['intents'] = state._intents.value
 
         await self.call_hooks('before_identify', self.shard_id, initial=self._initial_identify)
         await self.send_as_json(payload)
-        print(f"\033[31mI \033[33m{ghda} \033[32mliftcord.gateway \033[0m\033[1mShard ID {self.shard_id} has sent Identify payload")
+        _log.debug('Shard ID %s has sent the IDENTIFY payload.', self.shard_id)
 
     async def resume(self) -> None:
         """Sends the RESUME packet."""
         payload = {
             'op': self.RESUME,
             'd': {
                 'seq': self.sequence,
                 'session_id': self.session_id,
                 'token': self.token,
             },
         }
 
         await self.send_as_json(payload)
-        print(f"\033[31mI \033[33m{ghda} \033[32mliftcord.gateway \033[0m\033[1mShard ID {self.shard_id} has sent Resume payload")
+        _log.debug('Shard ID %s has sent the RESUME payload.', self.shard_id)
 
     async def received_message(self, msg: Any, /) -> None:
         if type(msg) is bytes:
             self._buffer.extend(msg)
 
             if len(msg) < 4 or msg[-4:] != b'\x00\x00\xff\xff':
                 return
             msg = self._zlib.decompress(self._buffer)
             msg = msg.decode('utf-8')
             self._buffer = bytearray()
 
         self.log_receive(msg)
         msg = utils._from_json(msg)
 
-    
+        _log.debug('For Shard ID %s: WebSocket Event: %s', self.shard_id, msg)
         event = msg.get('t')
         if event:
             self._dispatch('socket_event_type', event)
 
         op = msg.get('op')
         data = msg.get('d')
         seq = msg.get('s')
@@ -520,15 +512,15 @@
             self._keep_alive.tick()
 
         if op != self.DISPATCH:
             if op == self.RECONNECT:
                 # "reconnect" can only be handled by the Client
                 # so we terminate our connection and raise an
                 # internal exception signalling to reconnect.
-                print(f"\033[31mI \033[33m{ghda} \033[32mliftcord.gateway.rd \033[0m\033[1mRecived Reconnect opcode")
+                _log.debug('Received RECONNECT opcode.')
                 await self.close()
                 raise ReconnectWebSocket(self.shard_id)
 
             if op == self.HEARTBEAT_ACK:
                 if self._keep_alive:
                     self._keep_alive.ack()
                 return
@@ -551,31 +543,31 @@
                 if data is True:
                     await self.close()
                     raise ReconnectWebSocket(self.shard_id)
 
                 self.sequence = None
                 self.session_id = None
                 self.gateway = self.DEFAULT_GATEWAY
-                print(f"\033[31mI \033[33m{ghda} \033[32mliftcord.gateway \033[0m\033[1mShard ID {self.shard_id} session has been invalidated")
+                _log.info('Shard ID %s session has been invalidated.', self.shard_id)
                 await self.close(code=1000)
                 raise ReconnectWebSocket(self.shard_id, resume=False)
 
             _log.warning('Unknown OP code %s.', op)
             return
 
         if event == 'READY':
             self.sequence = msg['s']
             self.session_id = data['session_id']
             self.gateway = yarl.URL(data['resume_gateway_url'])
-            print(f"\033[31mI \033[33m{ghda} \033[32mliftcord.gateway \033[0m\033[1mShard ID {self.shard_id} connected to Gateway")
+            _log.info('Shard ID %s has connected to Gateway (Session ID: %s).', self.shard_id, self.session_id)
 
         elif event == 'RESUMED':
             # pass back the shard ID to the resumed handler
             data['__shard_id__'] = self.shard_id
-            print(f"\033[31mI \033[33m{ghda} \033[32mliftcord.gateway \033[0m\033[1mShardID {self.shard_id} has Resumed connection")
+            _log.info('Shard ID %s has successfully RESUMED session %s.', self.shard_id, self.session_id)
 
         try:
             func = self._discord_parsers[event]
         except KeyError:
             _log.debug('Unknown event %s.', event)
         else:
             func(data)
```

### Comparing `liftcord-25.9/liftcord/guild.py` & `liftcord-7.1/liftcord/guild.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/http.py` & `liftcord-7.1/liftcord/http.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/integrations.py` & `liftcord-7.1/liftcord/integrations.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/interactions.py` & `liftcord-7.1/liftcord/interactions.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/invite.py` & `liftcord-7.1/liftcord/invite.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/member.py` & `liftcord-7.1/liftcord/member.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/mentions.py` & `liftcord-7.1/liftcord/mentions.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/message.py` & `liftcord-7.1/liftcord/message.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/mixins.py` & `liftcord-7.1/liftcord/mixins.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/mobile/__init__.py` & `liftcord-7.1/liftcord/mobile/__init__.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/object.py` & `liftcord-7.1/liftcord/object.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/oggparse.py` & `liftcord-7.1/liftcord/oggparse.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/opus.py` & `liftcord-7.1/liftcord/opus.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/partial_emoji.py` & `liftcord-7.1/liftcord/partial_emoji.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/permissions.py` & `liftcord-7.1/liftcord/permissions.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/player.py` & `liftcord-7.1/liftcord/player.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/pylogz.py` & `liftcord-7.1/liftcord/pylogz.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/raw_models.py` & `liftcord-7.1/liftcord/raw_models.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/reaction.py` & `liftcord-7.1/liftcord/reaction.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/role.py` & `liftcord-7.1/liftcord/role.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/scheduled_event.py` & `liftcord-7.1/liftcord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/shard.py` & `liftcord-7.1/liftcord/shard.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/stage_instance.py` & `liftcord-7.1/liftcord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/state.py` & `liftcord-7.1/liftcord/state.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/sticker.py` & `liftcord-7.1/liftcord/sticker.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/team.py` & `liftcord-7.1/liftcord/team.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/template.py` & `liftcord-7.1/liftcord/template.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/threads.py` & `liftcord-7.1/liftcord/threads.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/activity.py` & `liftcord-7.1/liftcord/types/activity.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/appinfo.py` & `liftcord-7.1/liftcord/types/appinfo.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/audit_log.py` & `liftcord-7.1/liftcord/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/automod.py` & `liftcord-7.1/liftcord/types/automod.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/channel.py` & `liftcord-7.1/liftcord/types/channel.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/command.py` & `liftcord-7.1/liftcord/types/command.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/components.py` & `liftcord-7.1/liftcord/types/components.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/embed.py` & `liftcord-7.1/liftcord/types/embed.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/emoji.py` & `liftcord-7.1/liftcord/types/emoji.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/gateway.py` & `liftcord-7.1/liftcord/types/gateway.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/guild.py` & `liftcord-7.1/liftcord/types/guild.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/integration.py` & `liftcord-7.1/liftcord/types/integration.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/interactions.py` & `liftcord-7.1/liftcord/types/interactions.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/invite.py` & `liftcord-7.1/liftcord/types/invite.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/member.py` & `liftcord-7.1/liftcord/types/member.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/message.py` & `liftcord-7.1/liftcord/types/message.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/role.py` & `liftcord-7.1/liftcord/types/role.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/scheduled_event.py` & `liftcord-7.1/liftcord/types/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/snowflake.py` & `liftcord-7.1/liftcord/types/snowflake.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/sticker.py` & `liftcord-7.1/liftcord/types/sticker.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/team.py` & `liftcord-7.1/liftcord/types/team.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/template.py` & `liftcord-7.1/liftcord/types/template.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/threads.py` & `liftcord-7.1/liftcord/types/threads.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/user.py` & `liftcord-7.1/liftcord/types/user.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/voice.py` & `liftcord-7.1/liftcord/types/voice.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/webhook.py` & `liftcord-7.1/liftcord/types/webhook.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/welcome_screen.py` & `liftcord-7.1/liftcord/types/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/types/widget.py` & `liftcord-7.1/liftcord/types/widget.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ui/button.py` & `liftcord-7.1/liftcord/ui/button.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ui/item.py` & `liftcord-7.1/liftcord/ui/item.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ui/modal.py` & `liftcord-7.1/liftcord/ui/modal.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ui/select.py` & `liftcord-7.1/liftcord/ui/select.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ui/text_input.py` & `liftcord-7.1/liftcord/ui/text_input.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/ui/view.py` & `liftcord-7.1/liftcord/ui/view.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/user.py` & `liftcord-7.1/liftcord/user.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/utils.py` & `liftcord-7.1/liftcord/utils.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/voice_client.py` & `liftcord-7.1/liftcord/voice_client.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/webhook/async_.py` & `liftcord-7.1/liftcord/webhook/async_.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/webhook/sync.py` & `liftcord-7.1/liftcord/webhook/sync.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/welcome_screen.py` & `liftcord-7.1/liftcord/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord/widget.py` & `liftcord-7.1/liftcord/widget.py`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/liftcord.egg-info/PKG-INFO` & `liftcord-7.1/liftcord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liftcord
-Version: 25.9
+Version: 7.1
 Summary: A Python wrapper for the Discord API
 Home-page: https://github.com/devliftz/lift.py
 Author: go.
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `liftcord-25.9/liftcord.egg-info/SOURCES.txt` & `liftcord-7.1/liftcord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liftcord-25.9/setup.py` & `liftcord-7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'liftcord.mobile'
 ]
 
 setup(
     name='liftcord',
     author='go.',
     url='https://github.com/devliftz/lift.py',
-    version=25.9,
+    version=7.1,
     packages=packages,
     license='MIT',
     description='A Python wrapper for the Discord API',
     long_description_content_type='text/x-rst',
     include_package_data=True,
     install_requires=['aiohttp>=3.7.4,<4'],
     python_requires='>=3.8.0',
```

