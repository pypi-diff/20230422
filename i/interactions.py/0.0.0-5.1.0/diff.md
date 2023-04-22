# Comparing `tmp/interactions.py-0.0.0.tar.gz` & `tmp/interactions.py-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactions.py-0.0.0.tar", last modified: Mon Apr 10 21:49:46 2023, max compression
+gzip compressed data, was "interactions.py-5.1.0.tar", last modified: Sat Apr 22 06:01:32 2023, max compression
```

## Comparing `interactions.py-0.0.0.tar` & `interactions.py-5.1.0.tar`

### file list

```diff
@@ -1,11 +1,192 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 21:49:46.033644 interactions.py-0.0.0/
--rw-rw-rw-   0        0        0      160 2023-04-10 21:49:46.032645 interactions.py-0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 21:49:46.021631 interactions.py-0.0.0/interactions/
--rw-rw-rw-   0        0        0       74 2023-04-10 21:46:32.000000 interactions.py-0.0.0/interactions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 21:49:46.031644 interactions.py-0.0.0/interactions.py.egg-info/
--rw-rw-rw-   0        0        0      160 2023-04-10 21:49:45.000000 interactions.py-0.0.0/interactions.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-04-10 21:49:45.000000 interactions.py-0.0.0/interactions.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 21:49:45.000000 interactions.py-0.0.0/interactions.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 21:49:45.000000 interactions.py-0.0.0/interactions.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 21:49:46.033644 interactions.py-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      234 2023-04-10 21:49:43.000000 interactions.py-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.968174 interactions.py-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-22 06:00:58.000000 interactions.py-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-22 06:00:58.000000 interactions.py-5.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-22 06:01:32.968174 interactions.py-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-22 06:00:58.000000 interactions.py-5.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.944173 interactions.py-5.1.0/interactions/
+-rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.944173 interactions.py-5.1.0/interactions/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.944173 interactions.py-5.1.0/interactions/api/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23833 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.948173 interactions.py-5.1.0/interactions/api/events/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/_template.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/channel_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/guild_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/member_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/message_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/reaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/role_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/stage_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/thread_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/user_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/events/processors/voice_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.948173 interactions.py-5.1.0/interactions/api/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/gateway/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/gateway/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.948173 interactions.py-5.1.0/interactions/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20993 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.948173 interactions.py-5.1.0/interactions/api/http/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22791 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35371 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/scheduled_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/http_requests/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/http/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.952173 interactions.py-5.1.0/interactions/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/audio_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/api/voice/voice_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.952173 interactions.py-5.1.0/interactions/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/bin/opus-x64.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/bin/opus-x86.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.952173 interactions.py-5.1.0/interactions/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/auto_shard_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88115 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.952173 interactions.py-5.1.0/interactions/client/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/mixins/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/mixins/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/mixins/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31386 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/smart_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.956173 interactions.py-5.1.0/interactions/client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/attr_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/attr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/attr_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/deserialise_app_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/input_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/client/utils/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.956173 interactions.py-5.1.0/interactions/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.956173 interactions.py-5.1.0/interactions/ext/debug_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/debug_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/debug_extension/debug_application_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/debug_extension/debug_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/debug_extension/debug_exts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/debug_extension/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/jurigged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.956173 interactions.py-5.1.0/interactions/ext/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/mypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.956173 interactions.py-5.1.0/interactions/ext/prefixed_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/prefixed_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/prefixed_commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/prefixed_commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/prefixed_commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/prefixed_commands/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/prefixed_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/ext/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.956173 interactions.py-5.1.0/interactions/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.964173 interactions.py-5.1.0/interactions/models/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/app_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102171 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30028 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95041 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37369 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/scheduled_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/stage_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/voice_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/discord/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.964173 interactions.py-5.1.0/interactions/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/active_voice_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.964173 interactions.py-5.1.0/interactions/models/internal/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/annotations/slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55399 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/application_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/auto_defer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34488 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17637 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/localisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.964173 interactions.py-5.1.0/interactions/models/internal/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/tasks/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/internal/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.964173 interactions.py-5.1.0/interactions/models/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/misc/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/models/misc/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 06:00:58.000000 interactions.py-5.1.0/interactions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.944173 interactions.py-5.1.0/interactions.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-22 06:01:32.000000 interactions.py-5.1.0/interactions.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-22 06:01:32.000000 interactions.py-5.1.0/interactions.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 06:01:32.000000 interactions.py-5.1.0/interactions.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-22 06:01:32.000000 interactions.py-5.1.0/interactions.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 06:01:32.000000 interactions.py-5.1.0/interactions.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-22 06:00:58.000000 interactions.py-5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-22 06:00:58.000000 interactions.py-5.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-22 06:01:32.968174 interactions.py-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-22 06:01:26.000000 interactions.py-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 06:01:32.968174 interactions.py-5.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/test_cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/test_emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-22 06:00:58.000000 interactions.py-5.1.0/tests/utils.py
```

