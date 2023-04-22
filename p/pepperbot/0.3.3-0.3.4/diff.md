# Comparing `tmp/pepperbot-0.3.3.tar.gz` & `tmp/pepperbot-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperbot-0.3.3.tar", last modified: Fri Apr  7 15:08:38 2023, max compression
+gzip compressed data, was "pepperbot-0.3.4.tar", last modified: Sat Apr 22 16:22:16 2023, max compression
```

## Comparing `pepperbot-0.3.3.tar` & `pepperbot-0.3.4.tar`

### file list

```diff
@@ -1,88 +1,78 @@
--rw-r--r--   0        0        0     1084 2021-03-30 09:01:51.964858 pepperbot-0.3.3/LICENSE
--rw-r--r--   0        0        0     4377 2022-05-04 12:53:57.037526 pepperbot-0.3.3/README.md
--rw-r--r--   0        0        0       39 2022-02-20 09:58:20.149020 pepperbot-0.3.3/cli/__init__.py
--rw-r--r--   0        0        0      571 2023-04-07 15:06:56.893810 pepperbot-0.3.3/pepperbot/__init__.py
--rw-r--r--   0        0        0     2115 2023-04-05 15:06:17.937614 pepperbot-0.3.3/pepperbot/adapters/keaimao/__init__.py
--rw-r--r--   0        0        0     5816 2023-04-05 15:32:10.549854 pepperbot-0.3.3/pepperbot/adapters/keaimao/api/__init__.py
--rw-r--r--   0        0        0      470 2022-05-03 11:40:55.336433 pepperbot-0.3.3/pepperbot/adapters/keaimao/event/__init__.py
--rw-r--r--   0        0        0     1324 2022-05-03 11:43:52.905702 pepperbot-0.3.3/pepperbot/adapters/keaimao/event/kwargs.py
--rw-r--r--   0        0        0    21222 2022-04-13 12:45:33.068068 pepperbot-0.3.3/pepperbot/adapters/keaimao/event/records/EventFriendMsg.js
--rw-r--r--   0        0        0    10263 2022-02-20 09:58:20.299888 pepperbot-0.3.3/pepperbot/adapters/keaimao/event/records/EventGroupMessage.js
--rw-r--r--   0        0        0        0 2022-02-20 09:58:20.300841 pepperbot-0.3.3/pepperbot/adapters/keaimao/message/segment.py
--rw-r--r--   0        0        0     4665 2023-04-05 15:06:17.937614 pepperbot-0.3.3/pepperbot/adapters/onebot/__init__.py
--rw-r--r--   0        0        0     7415 2023-04-05 15:29:22.101697 pepperbot-0.3.3/pepperbot/adapters/onebot/api/__init__.py
--rw-r--r--   0        0        0     6292 2022-07-11 07:24:20.096774 pepperbot-0.3.3/pepperbot/adapters/onebot/event/__init__.py
--rw-r--r--   0        0        0     7812 2023-04-05 15:58:46.762390 pepperbot-0.3.3/pepperbot/adapters/onebot/event/kwargs.py
--rw-r--r--   0        0        0       75 2022-02-20 09:58:20.306537 pepperbot-0.3.3/pepperbot/adapters/onebot/models/GroupFile.py
--rw-r--r--   0        0        0       75 2022-02-20 09:58:20.307058 pepperbot-0.3.3/pepperbot/adapters/onebot/models/GroupInfo.py
--rw-r--r--   0        0        0       74 2022-02-20 09:58:20.307058 pepperbot-0.3.3/pepperbot/adapters/onebot/models/UserInfo.py
--rw-r--r--   0        0        0       52 2022-02-20 09:58:20.308047 pepperbot-0.3.3/pepperbot/adapters/onebot/models/__init__.py
--rw-r--r--   0        0        0      682 2022-02-20 09:58:20.308047 pepperbot-0.3.3/pepperbot/adapters/onebot/models/api/__init__.py
--rw-r--r--   0        0        0      362 2022-02-20 09:58:20.309048 pepperbot-0.3.3/pepperbot/adapters/onebot/models/events/GroupIncrease.py
--rw-r--r--   0        0        0      742 2022-02-20 09:58:20.309048 pepperbot-0.3.3/pepperbot/adapters/onebot/models/events/MetaEvent.py
--rw-r--r--   0        0        0       56 2022-02-20 09:58:20.310049 pepperbot-0.3.3/pepperbot/adapters/onebot/models/events/__init__.py
--rw-r--r--   0        0        0      462 2022-02-20 09:58:20.310049 pepperbot-0.3.3/pepperbot/adapters/onebot/models/friend.py
--rw-r--r--   0        0        0      572 2022-02-20 09:58:20.311051 pepperbot-0.3.3/pepperbot/adapters/onebot/models/pokes.py
--rw-r--r--   0        0        0      395 2022-02-20 09:58:20.311051 pepperbot-0.3.3/pepperbot/adapters/onebot/models/sender.py
--rw-r--r--   0        0        0      350 2022-02-20 09:58:20.312569 pepperbot-0.3.3/pepperbot/adapters/onebot/models/stranger.py
--rw-r--r--   0        0        0     1571 2023-04-05 15:26:55.780718 pepperbot-0.3.3/pepperbot/adapters/onebot/models/user.py
--rw-r--r--   0        0        0     7780 2023-04-05 15:06:17.937614 pepperbot-0.3.3/pepperbot/adapters/telegram/__init__.py
--rw-r--r--   0        0        0     3029 2022-05-05 09:07:29.026257 pepperbot-0.3.3/pepperbot/adapters/telegram/api/__init__.py
--rw-r--r--   0        0        0      449 2022-05-04 11:33:34.123784 pepperbot-0.3.3/pepperbot/adapters/telegram/event/__init__.py
--rw-r--r--   0        0        0     3808 2022-05-04 11:47:21.389787 pepperbot-0.3.3/pepperbot/adapters/telegram/event/kwargs.py
--rw-r--r--   0        0        0      753 2023-04-05 14:48:47.217690 pepperbot-0.3.3/pepperbot/config.py
--rw-r--r--   0        0        0        0 2022-02-20 09:58:20.315950 pepperbot-0.3.3/pepperbot/core/__init__.py
--rw-r--r--   0        0        0     2772 2023-04-05 15:47:15.930750 pepperbot-0.3.3/pepperbot/core/bot/api_caller.py
--rw-r--r--   0        0        0      835 2022-02-20 09:58:20.317490 pepperbot-0.3.3/pepperbot/core/bot/decorators.py
--rw-r--r--   0        0        0     2813 2022-05-04 10:32:18.441065 pepperbot-0.3.3/pepperbot/core/bot/universal.py
--rw-r--r--   0        0        0        0 2022-02-20 09:58:20.319000 pepperbot-0.3.3/pepperbot/core/event/__init__.py
--rw-r--r--   0        0        0      753 2023-04-05 15:06:17.936621 pepperbot-0.3.3/pepperbot/core/event/base_adapter.py
--rw-r--r--   0        0        0    12242 2023-04-05 15:06:17.937614 pepperbot-0.3.3/pepperbot/core/event/handle.py
--rw-r--r--   0        0        0      742 2022-05-03 08:40:18.814352 pepperbot-0.3.3/pepperbot/core/event/kwargs.py
--rw-r--r--   0        0        0     4123 2022-05-04 11:43:18.005633 pepperbot-0.3.3/pepperbot/core/event/universal.py
--rw-r--r--   0        0        0     3020 2022-05-04 06:33:33.296283 pepperbot-0.3.3/pepperbot/core/event/utils.py
--rw-r--r--   0        0        0      931 2022-05-03 12:01:53.466811 pepperbot-0.3.3/pepperbot/core/message/base.py
--rw-r--r--   0        0        0    11139 2023-04-02 14:27:09.833323 pepperbot-0.3.3/pepperbot/core/message/chain.py
--rw-r--r--   0        0        0    14059 2023-04-04 15:55:12.677163 pepperbot-0.3.3/pepperbot/core/message/segment.py
--rw-r--r--   0        0        0     1044 2022-02-20 09:58:20.324089 pepperbot-0.3.3/pepperbot/core/route/__init__.py
--rw-r--r--   0        0        0     6255 2022-04-11 09:47:48.635228 pepperbot-0.3.3/pepperbot/core/route/cache.py
--rw-r--r--   0        0        0      326 2022-02-20 09:58:20.368067 pepperbot-0.3.3/pepperbot/core/route/hook.py
--rw-r--r--   0        0        0     5523 2022-04-28 11:47:52.526761 pepperbot-0.3.3/pepperbot/core/route/parse.py
--rw-r--r--   0        0        0     1724 2022-05-05 08:45:13.054285 pepperbot-0.3.3/pepperbot/core/route/utils.py
--rw-r--r--   0        0        0    11430 2022-07-17 09:28:53.518455 pepperbot-0.3.3/pepperbot/core/route/validate.py
--rw-r--r--   0        0        0     1173 2022-05-09 03:01:19.221113 pepperbot-0.3.3/pepperbot/exceptions.py
--rw-r--r--   0        0        0        0 2022-02-20 09:58:20.371633 pepperbot-0.3.3/pepperbot/extensions/__init__.py
--rw-r--r--   0        0        0     2146 2022-07-12 14:55:41.437631 pepperbot-0.3.3/pepperbot/extensions/action/__init__.py
--rw-r--r--   0        0        0     1323 2022-02-20 09:58:20.372621 pepperbot-0.3.3/pepperbot/extensions/action/action.py
--rw-r--r--   0        0        0     9917 2022-02-20 09:58:20.372621 pepperbot-0.3.3/pepperbot/extensions/action/chain.py
--rw-r--r--   0        0        0     2813 2022-02-20 09:58:20.373773 pepperbot-0.3.3/pepperbot/extensions/action/decorators.py
--rw-r--r--   0        0        0     2413 2022-02-20 09:58:20.374299 pepperbot-0.3.3/pepperbot/extensions/action/runner.py
--rw-r--r--   0        0        0     2433 2022-02-20 09:58:20.376049 pepperbot-0.3.3/pepperbot/extensions/command/__init__.py
--rw-r--r--   0        0        0       26 2022-02-20 09:58:20.376575 pepperbot-0.3.3/pepperbot/extensions/command/commands/__init__.py
--rw-r--r--   0        0        0    19797 2022-02-20 09:58:20.377095 pepperbot-0.3.3/pepperbot/extensions/command/commands/commands.py
--rw-r--r--   0        0        0    17966 2023-04-07 15:07:39.875170 pepperbot-0.3.3/pepperbot/extensions/command/handle.py
--rw-r--r--   0        0        0    12257 2022-05-05 09:09:27.492605 pepperbot-0.3.3/pepperbot/extensions/command/pattern.py
--rw-r--r--   0        0        0     3166 2023-04-07 15:04:27.332364 pepperbot-0.3.3/pepperbot/extensions/command/utils.py
--rw-r--r--   0        0        0     1944 2023-04-07 14:27:38.062798 pepperbot-0.3.3/pepperbot/extensions/log/__init__.py
--rw-r--r--   0        0        0      103 2023-04-07 14:00:53.161961 pepperbot-0.3.3/pepperbot/extensions/scheduler/__init__.py
--rw-r--r--   0        0        0     6965 2023-04-07 14:26:32.119176 pepperbot-0.3.3/pepperbot/initial.py
--rw-r--r--   0        0        0       79 2022-02-20 09:58:20.384843 pepperbot-0.3.3/pepperbot/store/__init__.py
--rw-r--r--   0        0        0     6664 2022-02-20 12:53:51.961902 pepperbot-0.3.3/pepperbot/store/command.py
--rw-r--r--   0        0        0        0 2022-02-20 09:58:20.385358 pepperbot-0.3.3/pepperbot/store/message.py
--rw-r--r--   0        0        0    13280 2023-04-05 15:04:13.650889 pepperbot-0.3.3/pepperbot/store/meta.py
--rw-r--r--   0        0        0      847 2022-02-20 09:58:20.387351 pepperbot-0.3.3/pepperbot/types.py
--rw-r--r--   0        0        0        0 2021-05-20 10:22:56.350973 pepperbot-0.3.3/pepperbot/utils/__init__.py
--rw-r--r--   0        0        0     4511 2023-04-05 14:57:06.725648 pepperbot-0.3.3/pepperbot/utils/common.py
--rw-r--r--   0        0        0     1743 2023-04-07 15:08:38.217525 pepperbot-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2021-02-17 16:09:40.523059 pepperbot-0.3.3/tests/__init__.py
--rw-r--r--   0        0        0     5265 2022-02-20 09:58:20.393826 pepperbot-0.3.3/tests/command/test_parse.py
--rw-r--r--   0        0        0      458 2021-05-20 06:46:35.532000 pepperbot-0.3.3/tests/context.py
--rw-r--r--   0        0        0      334 2021-05-20 10:15:22.378106 pepperbot-0.3.3/tests/is_flash.py
--rw-r--r--   0        0        0     1775 2021-05-20 08:57:32.459172 pepperbot-0.3.3/tests/messageChain.py
--rw-r--r--   0        0        0      589 2021-12-19 07:28:12.204746 pepperbot-0.3.3/tests/parse_pattern.py
--rw-r--r--   0        0        0     3335 2021-12-20 07:19:18.332221 pepperbot-0.3.3/tests/pattern.py
--rw-r--r--   0        0        0        0 2021-05-29 16:07:13.445106 pepperbot-0.3.3/tests/response/__init__.py
--rw-r--r--   0        0        0     2148 2022-02-20 09:58:20.394827 pepperbot-0.3.3/tests/response/fake_server.py
--rw-r--r--   0        0        0     1304 2021-05-29 17:05:54.532212 pepperbot-0.3.3/tests/response/poke.py
--rw-r--r--   0        0        0     2640 2021-05-20 11:42:38.152329 pepperbot-0.3.3/tests/tree.py
--rw-r--r--   0        0        0     5485 1970-01-01 00:00:00.000000 pepperbot-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2021-03-30 09:01:51.964858 pepperbot-0.3.4/LICENSE
+-rw-r--r--   0        0        0     4242 2023-04-09 16:21:30.526457 pepperbot-0.3.4/README.md
+-rw-r--r--   0        0        0      273 2023-04-10 16:48:13.652944 pepperbot-0.3.4/cli/__init__.py
+-rw-r--r--   0        0        0      631 2023-04-22 14:40:27.359697 pepperbot-0.3.4/pepperbot/__init__.py
+-rw-r--r--   0        0        0     2819 2023-04-15 23:10:33.259712 pepperbot-0.3.4/pepperbot/adapters/keaimao/__init__.py
+-rw-r--r--   0        0        0     5722 2023-04-20 11:08:26.809253 pepperbot-0.3.4/pepperbot/adapters/keaimao/api/__init__.py
+-rw-r--r--   0        0        0     2636 2023-04-15 23:07:16.981274 pepperbot-0.3.4/pepperbot/adapters/keaimao/event/__init__.py
+-rw-r--r--   0        0        0    21222 2022-04-13 12:45:33.068068 pepperbot-0.3.4/pepperbot/adapters/keaimao/event/records/EventFriendMsg.js
+-rw-r--r--   0        0        0    10263 2022-02-20 09:58:20.299888 pepperbot-0.3.4/pepperbot/adapters/keaimao/event/records/EventGroupMessage.js
+-rw-r--r--   0        0        0     6524 2023-04-16 02:25:50.305638 pepperbot-0.3.4/pepperbot/adapters/onebot/__init__.py
+-rw-r--r--   0        0        0    25015 2023-04-15 13:09:02.414734 pepperbot-0.3.4/pepperbot/adapters/onebot/api/__init__.py
+-rw-r--r--   0        0        0    11305 2023-04-20 11:07:29.210764 pepperbot-0.3.4/pepperbot/adapters/onebot/event/__init__.py
+-rw-r--r--   0        0        0       67 2023-04-14 16:22:16.875389 pepperbot-0.3.4/pepperbot/adapters/onebot/models/__init__.py
+-rw-r--r--   0        0        0      696 2023-04-14 16:01:58.086198 pepperbot-0.3.4/pepperbot/adapters/onebot/models/group.py
+-rw-r--r--   0        0        0      572 2022-02-20 09:58:20.311051 pepperbot-0.3.4/pepperbot/adapters/onebot/models/message.py
+-rw-r--r--   0        0        0     1395 2023-04-14 16:22:28.359913 pepperbot-0.3.4/pepperbot/adapters/onebot/models/user.py
+-rw-r--r--   0        0        0     9174 2023-04-19 05:26:45.684428 pepperbot-0.3.4/pepperbot/adapters/telegram/__init__.py
+-rw-r--r--   0        0        0     2931 2023-04-20 11:10:48.986337 pepperbot-0.3.4/pepperbot/adapters/telegram/api/__init__.py
+-rw-r--r--   0        0        0     4663 2023-04-19 05:22:27.264737 pepperbot-0.3.4/pepperbot/adapters/telegram/event/__init__.py
+-rw-r--r--   0        0        0      900 2023-04-14 17:09:33.793304 pepperbot-0.3.4/pepperbot/adapters/universal/__init__.py
+-rw-r--r--   0        0        0     2709 2023-04-20 11:10:48.986337 pepperbot-0.3.4/pepperbot/adapters/universal/api/__init__.py
+-rw-r--r--   0        0        0     3245 2023-04-15 23:11:30.691877 pepperbot-0.3.4/pepperbot/adapters/universal/event/__init__.py
+-rw-r--r--   0        0        0      766 2023-04-10 15:18:25.547755 pepperbot-0.3.4/pepperbot/config.py
+-rw-r--r--   0        0        0        0 2022-02-20 09:58:20.315950 pepperbot-0.3.4/pepperbot/core/__init__.py
+-rw-r--r--   0        0        0     2796 2023-04-14 15:03:07.150287 pepperbot-0.3.4/pepperbot/core/api/api_caller.py
+-rw-r--r--   0        0        0      835 2022-02-20 09:58:20.317490 pepperbot-0.3.4/pepperbot/core/api/decorators.py
+-rw-r--r--   0        0        0        0 2022-02-20 09:58:20.319000 pepperbot-0.3.4/pepperbot/core/event/__init__.py
+-rw-r--r--   0        0        0     1514 2023-04-16 00:04:42.470521 pepperbot-0.3.4/pepperbot/core/event/base_adapter.py
+-rw-r--r--   0        0        0    22216 2023-04-22 15:01:15.299917 pepperbot-0.3.4/pepperbot/core/event/handle.py
+-rw-r--r--   0        0        0     1642 2023-04-19 05:27:57.642248 pepperbot-0.3.4/pepperbot/core/event/universal.py
+-rw-r--r--   0        0        0     3020 2022-05-04 06:33:33.296283 pepperbot-0.3.4/pepperbot/core/event/utils.py
+-rw-r--r--   0        0        0      931 2022-05-03 12:01:53.466811 pepperbot-0.3.4/pepperbot/core/message/base.py
+-rw-r--r--   0        0        0    11166 2023-04-22 06:17:19.872292 pepperbot-0.3.4/pepperbot/core/message/chain.py
+-rw-r--r--   0        0        0    16761 2023-04-22 07:06:21.608086 pepperbot-0.3.4/pepperbot/core/message/segment.py
+-rw-r--r--   0        0        0       84 2023-04-22 12:37:07.245598 pepperbot-0.3.4/pepperbot/core/route/__init__.py
+-rw-r--r--   0        0        0     5629 2023-04-22 14:47:07.876298 pepperbot-0.3.4/pepperbot/core/route/available/__init__.py
+-rw-r--r--   0        0        0     1359 2023-04-22 15:10:40.463249 pepperbot-0.3.4/pepperbot/core/route/available/decorators.py
+-rw-r--r--   0        0        0     4873 2023-04-20 12:01:02.327347 pepperbot-0.3.4/pepperbot/core/route/cache.py
+-rw-r--r--   0        0        0      326 2022-02-20 09:58:20.368067 pepperbot-0.3.4/pepperbot/core/route/hook.py
+-rw-r--r--   0        0        0     6520 2023-04-20 12:02:43.500740 pepperbot-0.3.4/pepperbot/core/route/parse.py
+-rw-r--r--   0        0        0     1812 2023-04-11 17:35:49.039234 pepperbot-0.3.4/pepperbot/core/route/utils.py
+-rw-r--r--   0        0        0    13071 2023-04-20 08:52:11.814433 pepperbot-0.3.4/pepperbot/core/route/validate.py
+-rw-r--r--   0        0        0     1165 2023-04-20 10:22:17.059555 pepperbot-0.3.4/pepperbot/exceptions.py
+-rw-r--r--   0        0        0        0 2022-02-20 09:58:20.371633 pepperbot-0.3.4/pepperbot/extensions/__init__.py
+-rw-r--r--   0        0        0     2146 2022-07-12 14:55:41.437631 pepperbot-0.3.4/pepperbot/extensions/action/__init__.py
+-rw-r--r--   0        0        0     1323 2022-02-20 09:58:20.372621 pepperbot-0.3.4/pepperbot/extensions/action/action.py
+-rw-r--r--   0        0        0     9917 2022-02-20 09:58:20.372621 pepperbot-0.3.4/pepperbot/extensions/action/chain.py
+-rw-r--r--   0        0        0     2813 2022-02-20 09:58:20.373773 pepperbot-0.3.4/pepperbot/extensions/action/decorators.py
+-rw-r--r--   0        0        0     2413 2022-02-20 09:58:20.374299 pepperbot-0.3.4/pepperbot/extensions/action/runner.py
+-rw-r--r--   0        0        0     5316 2023-04-20 14:56:40.268659 pepperbot-0.3.4/pepperbot/extensions/command/__init__.py
+-rw-r--r--   0        0        0    31844 2023-04-22 15:51:38.702263 pepperbot-0.3.4/pepperbot/extensions/command/handle.py
+-rw-r--r--   0        0        0    12345 2023-04-22 13:03:26.717222 pepperbot-0.3.4/pepperbot/extensions/command/pattern.py
+-rw-r--r--   0        0        0     2491 2023-04-20 11:29:18.885191 pepperbot-0.3.4/pepperbot/extensions/command/sender.py
+-rw-r--r--   0        0        0     3180 2023-04-20 11:24:06.077698 pepperbot-0.3.4/pepperbot/extensions/command/utils.py
+-rw-r--r--   0        0        0     2093 2023-04-20 10:57:14.518991 pepperbot-0.3.4/pepperbot/extensions/log/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-07 14:00:53.161961 pepperbot-0.3.4/pepperbot/extensions/scheduler/__init__.py
+-rw-r--r--   0        0        0     8449 2023-04-20 10:23:25.131218 pepperbot-0.3.4/pepperbot/initial.py
+-rw-r--r--   0        0        0       79 2022-02-20 09:58:20.384843 pepperbot-0.3.4/pepperbot/store/__init__.py
+-rw-r--r--   0        0        0     6047 2023-04-22 14:11:02.794934 pepperbot-0.3.4/pepperbot/store/command.py
+-rw-r--r--   0        0        0     2421 2023-04-22 14:42:16.694644 pepperbot-0.3.4/pepperbot/store/event.py
+-rw-r--r--   0        0        0    14141 2023-04-22 14:20:55.717103 pepperbot-0.3.4/pepperbot/store/meta.py
+-rw-r--r--   0        0        0     2426 2023-04-12 14:36:34.483507 pepperbot-0.3.4/pepperbot/store/orm.py
+-rw-r--r--   0        0        0     1539 2023-04-20 15:00:26.563551 pepperbot-0.3.4/pepperbot/types.py
+-rw-r--r--   0        0        0        0 2021-05-20 10:22:56.350973 pepperbot-0.3.4/pepperbot/utils/__init__.py
+-rw-r--r--   0        0        0     5480 2023-04-22 13:18:32.526987 pepperbot-0.3.4/pepperbot/utils/common.py
+-rw-r--r--   0        0        0     1774 2023-04-22 16:22:16.096908 pepperbot-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-02-17 16:09:40.523059 pepperbot-0.3.4/tests/__init__.py
+-rw-r--r--   0        0        0     5265 2022-02-20 09:58:20.393826 pepperbot-0.3.4/tests/command/test_parse.py
+-rw-r--r--   0        0        0      458 2021-05-20 06:46:35.532000 pepperbot-0.3.4/tests/context.py
+-rw-r--r--   0        0        0      334 2021-05-20 10:15:22.378106 pepperbot-0.3.4/tests/is_flash.py
+-rw-r--r--   0        0        0     1775 2021-05-20 08:57:32.459172 pepperbot-0.3.4/tests/messageChain.py
+-rw-r--r--   0        0        0      589 2021-12-19 07:28:12.204746 pepperbot-0.3.4/tests/parse_pattern.py
+-rw-r--r--   0        0        0     3335 2023-04-20 10:31:00.764749 pepperbot-0.3.4/tests/pattern.py
+-rw-r--r--   0        0        0        0 2021-05-29 16:07:13.445106 pepperbot-0.3.4/tests/response/__init__.py
+-rw-r--r--   0        0        0     2148 2022-02-20 09:58:20.394827 pepperbot-0.3.4/tests/response/fake_server.py
+-rw-r--r--   0        0        0     1304 2021-05-29 17:05:54.532212 pepperbot-0.3.4/tests/response/poke.py
+-rw-r--r--   0        0        0     2640 2021-05-20 11:42:38.152329 pepperbot-0.3.4/tests/tree.py
+-rw-r--r--   0        0        0     5389 1970-01-01 00:00:00.000000 pepperbot-0.3.4/PKG-INFO
```

### Comparing `pepperbot-0.3.3/LICENSE` & `pepperbot-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/README.md` & `pepperbot-0.3.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 <h1 align="center">PepperBot</h1>
 
 <p align="center">
-<img  src="./archive/icon.png" width="200">
+<img  src="./archive/icon.png" width="200" />
 </p>
 
 <p align="center">一个符合直觉的跨社交平台机器人框架，轻松地在平台间传递消息，支持QQ、微信、Telegram</p>
 <p align="center">
 <a href="https://ssmjae.github.io/PepperBot/">文档</a> ·
 <a href="https://jq.qq.com/?_wv=1027&k=EPhcRRib">QQ交流群</a>  
-<!-- <a href="https://jq.qq.com/?_wv=1027&k=EPhcRRib">微信交流群</a> · 
-<a href="https://jq.qq.com/?_wv=1027&k=EPhcRRib">TG交流群</a>  -->
 </p>
 
 <p align="center">
 <img src="./archive/coverage-badge.svg" />
 </p>
 
 ## 生而跨平台
@@ -107,7 +105,9 @@
             # 发送一条群消息
             # 接受任意个参数，必须是合法的消息片段，比如Text，Face，Image
             await bot.group_message(
                 Text("没人"),
                 Image("http://123.jpg"),
             )
 ```
+
+## 生态
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                             ****** PepperBot ******
                              [./archive/icon.png]
 ä¸ä¸ªç¬¦åç´è§çè·¨ç¤¾äº¤å¹³å°æºå¨äººæ¡æ¶ï¼è½»æ¾å°å¨å¹³å°é´ä¼ éæ¶æ¯ï¼æ¯æQQãå¾®ä¿¡ãTelegram
-                            ææ¡£ Â· QQäº¤æµç¾¤
+                             ææ¡£ Â· QQäº¤æµç¾¤
                         [./archive/coverage-badge.svg]
 ## çèè·¨å¹³å° - QQ åºäº `Onebot` - å¾®ä¿¡åºäº`å¯ç±ç«` -
 Telegramåºäº`Pyrogram` - æä¾äºè·¨å¹³å°ãæç¨çæ¶æ¯ç±»å(çæ®µ) -
 éç¨äºä»¶ï¼æ¯å¦ç¾¤æ¶æ¯ãç§èæ¶æ¯ç­ï¼æä¾äºç»ä¸çæ¥å£ï¼åªéè¦åä¸æ¬¡ä»£ç ï¼å°±å¯ä»¥æ ç¼åºç¨å°åä¸ªå¹³å°ä¸ï¼è·¨å¹³å°çæ¶æ¯ä¼ éä»æªå¦æ­¤è½»æ¾éæ
 - [ ] å¯ä»¥è·¨ç¾¤ãè·¨å¹³å°å±äº«æä»¤(çç¶æ) ## æ§è½ä¹å¤ç¨ -
 åºå±åºäºå¼æ­¥ç Sanic æ¡æ¶(ç®åæä¸å®çæç python web
 æ¡æ¶ï¼[æ§è½æå¥½ç](https://www.techempower.com/benchmarks/
@@ -43,8 +43,9 @@
 if "æ¤åæ" == chain.pure_text: await chain.withdraw() #
 å¯ä»¥ç´æ¥âæ¤åæ¶æ¯âï¼ç¬¦åç´è§ if "è¸¢åºæ" ==
 chain.pure_text: await sender.kickout() # å¯ä»¥ç´æ¥è¸¢åºåè¨ç¾¤å #
 ä¹å¯ä»¥å¯¹æ¶æ¯é¾è¿è¡inæä½ï¼ç¸å½äºin chain.pure_text if
 "ç¦è¨æ" in chain: await sender.ban(10) # å¯ä»¥ç´æ¥ç¦è¨åè¨ç¾¤å if
 chain.regex("æäºº(å¨|å|å|å¨å).?"): # åéä¸æ¡ç¾¤æ¶æ¯ #
 æ¥åä»»æä¸ªåæ°ï¼å¿é¡»æ¯åæ³çæ¶æ¯çæ®µï¼æ¯å¦Textï¼Faceï¼Image
-await bot.group_message( Text("æ²¡äºº"), Image("http://123.jpg"), ) ```
+await bot.group_message( Text("æ²¡äºº"), Image("http://123.jpg"), ) ``` ##
+çæ
```

### Comparing `pepperbot-0.3.3/pepperbot/__init__.py` & `pepperbot-0.3.4/pepperbot/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 import better_exceptions
 from better_exceptions import encoding
 
 from pepperbot.extensions.log import logger
 from pepperbot.extensions.scheduler import async_scheduler
+from pepperbot.store.meta import BotRoute
 
 from .initial import PepperBot
 
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 __all__ = (
     "__version__",
     "PepperBot",
     "logger",
     "async_scheduler",
+    "BotRoute",
 )
 
 # https://github.com/Qix-/better-exceptions/issues/53
 # 中文windows默认编码是gb2312，管道符号无法正常显示，手动设置为utf-8
 encoding.ENCODING = "utf-8"
 
 better_exceptions.hook()
```

### Comparing `pepperbot-0.3.3/pepperbot/adapters/keaimao/api/__init__.py` & `pepperbot-0.3.4/pepperbot/adapters/keaimao/api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,29 +49,29 @@
 
 
 from typing import TYPE_CHECKING, Dict
 
 if TYPE_CHECKING:
     from pepperbot.core.message.segment import T_SegmentInstance
 
-from pepperbot.core.bot.api_caller import ApiCaller
+from pepperbot.core.api.api_caller import ApiCaller
 from pepperbot.core.message.segment import Image, Music, T_SegmentClass, Text, Video
 from pepperbot.exceptions import BackendApiError, EventHandleError
 from pepperbot.store.meta import get_bot_id, get_keaimao_caller
 from pepperbot.types import BaseBot
 
 KEAIMAO_SEGMENT_ACTION_MAPPING: Dict[T_SegmentClass, str] = {
     Image: "SendImageMsg",
     Music: "SendMusicMsg",
     Text: "SendTextMsg",
     Video: "SendVideoMsg",
 }
 
 
-class KeaimaoApi:
+class KeaimaoAPI:
     @staticmethod
     async def get_login_accounts():
         try:
             return await get_keaimao_caller()("GetLoggedAccountList")
         except:
             raise EventHandleError(f"无法获取可爱猫机器人登录信息，请确认可爱猫正常运行")
 
@@ -101,41 +101,37 @@
 class KeaimaoProperties(BaseBot):
     bot_id: str
     group_id: str
     private_id: str
     api_caller: ApiCaller
 
 
-class KeaimaoCommonApi(KeaimaoProperties):
-    pass
-
-
-class KeaimaoGroupApi(KeaimaoProperties):
+class KeaimaoGroupAPI(KeaimaoProperties):
     async def group_message(self, *segments: "T_SegmentInstance"):
-        return await KeaimaoApi.group_message(self.group_id, *segments)
+        return await KeaimaoAPI.group_message(self.group_id, *segments)
 
 
-class KeaimaoPrivateApi(KeaimaoProperties):
+class KeaimaoPrivateAPI(KeaimaoProperties):
     pass
 
 
-class KeaimaoGroupBot(KeaimaoCommonApi, KeaimaoGroupApi):
+class KeaimaoGroupBot(KeaimaoGroupAPI):
     __slots__ = (
         "bot_id",
         "group_id",
         "api_caller",
     )
 
     def __init__(self, bot_id: str, group_id: str):
         self.bot_id = bot_id
         self.group_id = group_id
         self.api_caller = get_keaimao_caller()
 
 
-class KeaimaoPrivateBot(KeaimaoCommonApi, KeaimaoPrivateApi):
+class KeaimaoPrivateBot(KeaimaoPrivateAPI):
     __slots__ = (
         "bot_id",
         "private_id",
         "api_caller",
     )
 
     def __init__(self, bot_id: str, private_id: str):
```

### Comparing `pepperbot-0.3.3/pepperbot/adapters/keaimao/event/records/EventFriendMsg.js` & `pepperbot-0.3.4/pepperbot/adapters/keaimao/event/records/EventFriendMsg.js`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/pepperbot/adapters/keaimao/event/records/EventGroupMessage.js` & `pepperbot-0.3.4/pepperbot/adapters/keaimao/event/records/EventGroupMessage.js`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/pepperbot/adapters/onebot/models/pokes.py` & `pepperbot-0.3.4/pepperbot/adapters/onebot/models/message.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/pepperbot/adapters/telegram/__init__.py` & `pepperbot-0.3.4/pepperbot/adapters/telegram/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Dict, Optional, cast
 
 from devtools import debug
-from pepperbot.adapters.telegram.event import (
-    TelegramCommonEvent,
-    TelegramGroupEvent,
-    TelegramMetaEvent,
-    TelegramPrivateEvent,
-)
-from pepperbot.adapters.telegram.event.kwargs import TELEGRAM_KWARGS_MAPPING
+from pepperbot.adapters.telegram.event import TelegramEvent
 from pepperbot.core.event.base_adapter import BaseAdapter
 from pepperbot.exceptions import EventHandleError
 from pepperbot.extensions.log import debug_log, logger
-from pepperbot.types import T_RouteMode
+from pepperbot.store.event import ProtocolEvent, filter_event_by_type
+from pepperbot.types import T_ConversationType
 from pepperbot.utils.common import get_own_attributes
 from pyrogram import ContinuePropagation, filters
 from pyrogram.client import Client
 from pyrogram.enums.chat_type import ChatType
 from pyrogram.handlers.callback_query_handler import CallbackQueryHandler
 from pyrogram.handlers.chat_join_request_handler import ChatJoinRequestHandler
 from pyrogram.handlers.chat_member_updated_handler import ChatMemberUpdatedHandler
@@ -23,34 +18,56 @@
 from pyrogram.handlers.edited_message_handler import EditedMessageHandler
 from pyrogram.handlers.inline_query_handler import InlineQueryHandler
 from pyrogram.handlers.message_handler import MessageHandler
 from pyrogram.handlers.raw_update_handler import RawUpdateHandler
 from pyrogram.types import CallbackQuery, ChatEventFilter, Message
 
 
-class TelegramAdapter(BaseAdapter):
-    event_prefix = "telegram_"
-    meta_events = list(get_own_attributes(TelegramMetaEvent))
-    common_events = list(get_own_attributes(TelegramCommonEvent))
-    group_events = list(get_own_attributes(TelegramGroupEvent))
-    private_events = list(get_own_attributes(TelegramPrivateEvent))
+own_attributes = get_own_attributes(TelegramEvent)
+
+events: list[ProtocolEvent] = [getattr(TelegramEvent, attr) for attr in own_attributes]
 
-    all_events = [*meta_events, *common_events, *group_events, *private_events]
 
-    kwargs = TELEGRAM_KWARGS_MAPPING
+class TelegramAdapter(BaseAdapter):
+    kwargs_mapping = {
+        cast(str, event.protocol_event_name): event.keyword_arguments
+        for event in events
+    }
+
+    all_events = events
+    all_event_names = [cast(str, event.protocol_event_name) for event in events]
+
+    meta_events = filter_event_by_type(events, ("meta",))
+    meta_event_names = [cast(str, event.protocol_event_name) for event in meta_events]
+    notice_events = filter_event_by_type(events, ("notice",))
+    notice_event_names = [
+        cast(str, event.protocol_event_name) for event in notice_events
+    ]
+    request_events = filter_event_by_type(events, ("request",))
+    request_event_names = [
+        cast(str, event.protocol_event_name) for event in request_events
+    ]
+    message_events = filter_event_by_type(events, ("message",))
+    message_event_names = [
+        cast(str, event.protocol_event_name) for event in message_events
+    ]
+
+    group_events = filter_event_by_type(events, ("group",))
+    private_events = filter_event_by_type(events, ("private",))
 
     @staticmethod
-    def get_event_name(raw_event: Dict):
-        return raw_event["event_name"]
+    def get_event(raw_event: Dict):
+        # debug(raw_event)
+        return getattr(TelegramEvent, raw_event["event_name"])
 
     @staticmethod
-    def get_route_mode(raw_event: Dict, raw_event_name: str):
+    def get_conversation_type(raw_event: Dict, raw_event_name: str):
         callback_object = raw_event["callback_object"]
 
-        debug_log(callback_object)
+        # debug_log(callback_object)
 
         if isinstance(callback_object, CallbackQuery):
             chat_type: ChatType = callback_object.message.chat.type
 
         elif isinstance(callback_object, Message):
             chat_type: ChatType = callback_object.chat.type
 
@@ -63,15 +80,15 @@
             mode = "group"
         else:
             raise EventHandleError(f"")
 
         return mode
 
     @staticmethod
-    def get_source_id(raw_event: Dict, mode: T_RouteMode):
+    def get_source_id(raw_event: Dict, mode: T_ConversationType):
         source_id: Optional[str] = None
 
         callback_object = raw_event["callback_object"]
         if mode == "group":
             # 注意不是from_user.id，是来源id，比如群号
             source_id = callback_object.chat.id
 
@@ -79,70 +96,89 @@
             source_id = callback_object.from_user.id
 
         elif mode == "channel":
             source_id = callback_object.chat.id
 
         return source_id
 
+    @staticmethod
+    def get_user_id(raw_event: Dict, mode: T_ConversationType):
+        callback_object = raw_event["callback_object"]
+
+        # debug_log(callback_object)
+
+        user_id: Optional[int | str] = None
+
+        if isinstance(callback_object, CallbackQuery):
+            user_id = callback_object.from_user.id
+
+        elif isinstance(callback_object, Message):
+            user_id = callback_object.from_user.id
+
+        else:
+            user_id = callback_object.user.id
+
+        return str(user_id) if user_id else None
+
 
 async def any_handler(client: Client, update: Any, handle_event, users, chats):
     await handle_event(
         "telegram",
         dict(
-            event_name=TelegramMetaEvent.raw_update,
+            event_name=TelegramEvent.raw_update.raw_event_name,
             callback_object=update,
             users=users,
             chats=chats,
         ),
     )
 
     raise ContinuePropagation
 
 
 async def private_message_handler(client: Client, callback_object: Any, handle_event):
     await handle_event(
         "telegram",
         dict(
-            event_name=TelegramPrivateEvent.private_message,
+            event_name=TelegramEvent.private_message.raw_event_name,
             callback_object=callback_object,
         ),
     )
 
     raise ContinuePropagation
 
 
 async def group_message_handler(client: Client, callback_object: Any, handle_event):
     await handle_event(
         "telegram",
         dict(
-            event_name=TelegramGroupEvent.group_message,
+            event_name=TelegramEvent.group_message.raw_event_name,
             callback_object=callback_object,
         ),
     )
 
     raise ContinuePropagation
 
 
 async def edited_message_handler(client: Client, callback_object: Any, handle_event):
     await handle_event(
         "telegram",
         dict(
-            event_name=TelegramCommonEvent.edited_message,
+            event_name=TelegramEvent.edited_message.raw_event_name,
             callback_object=callback_object,
         ),
     )
 
     raise ContinuePropagation
 
 
 async def callback_query_handler(client: Client, callback_object: Any, handle_event):
     await handle_event(
         "telegram",
         dict(
-            event_name=TelegramCommonEvent.callback_query,
+            event_name=TelegramEvent.callback_query.raw_event_name,
             callback_object=callback_object,
         ),
     )
 
     raise ContinuePropagation
 
 
@@ -155,27 +191,27 @@
 
 async def chosen_inline_result_handler(
     client: Client, callback_object: Any, handle_event
 ):
     await handle_event(
         "telegram",
         dict(
-            event_name=TelegramCommonEvent.chosen_inline_result,
+            event_name=TelegramEvent.chosen_inline_result.raw_event_name,
             callback_object=callback_object,
         ),
     )
 
     raise ContinuePropagation
 
 
 async def inline_query_handler(client: Client, callback_object: Any, handle_event):
     await handle_event(
         "telegram",
         dict(
-            event_name=TelegramCommonEvent.inline_query,
+            event_name=TelegramEvent.inline_query.raw_event_name,
             callback_object=callback_object,
         ),
     )
 
     raise ContinuePropagation
 
 
@@ -184,14 +220,15 @@
     avoid circlely import caused by `handle_event`
 
     pass `handle_event` as parameter to avoid multiple times import
     """
 
     async def wrapper(client, callback_object, *args):
         try:
+            debug(*args)
             return await handler(client, callback_object, handle_event, *args)
 
         except ContinuePropagation:
             raise ContinuePropagation
 
         except Exception as e:
             logger.exception(e)
```

### Comparing `pepperbot-0.3.3/pepperbot/adapters/telegram/api/__init__.py` & `pepperbot-0.3.4/pepperbot/adapters/telegram/api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING, Dict, Iterable, List, Tuple
 
 if TYPE_CHECKING:
     from pepperbot.core.message.segment import T_SegmentInstance
 
-from pepperbot.core.bot.api_caller import ApiCaller
+from pepperbot.core.api.api_caller import ApiCaller
 from pepperbot.core.message.segment import (
     Audio,
     Image,
     Music,
     T_SegmentClass,
     Text,
     Video,
@@ -24,15 +24,15 @@
     Audio: "send_audio",
     Image: "send_photo",
     Text: "send_message",
     Video: "send_video",
 }
 
 
-class TelegramApi:
+class TelegramAPI:
     @staticmethod
     async def send_message(chat_id: str, iterable: Iterable["T_SegmentInstance"]):
         client = get_telegram_caller()
 
         for segment in iterable:
             segment_type = segment.__class__
 
@@ -45,56 +45,52 @@
                 )
 
             else:
                 logger.error(f"尚未适配的消息类型 telegram {segment_type}")
 
     @staticmethod
     async def group_message(chat_id: str, *segments: "T_SegmentInstance"):
-        await TelegramApi.send_message(chat_id, segments)
+        await TelegramAPI.send_message(chat_id, segments)
 
     @staticmethod
     async def private_message(chat_id: str, *segments: "T_SegmentInstance"):
-        await TelegramApi.send_message(chat_id, segments)
+        await TelegramAPI.send_message(chat_id, segments)
 
 
 class TelegramProperties(BaseBot):
     bot_id: str
     group_id: str
     private_id: str
     api_caller: Client
 
 
-class TelegramCommonApi(TelegramProperties):
-    pass
-
-
-class TelegramGroupApi(TelegramProperties):
+class TelegramGroupAPI(TelegramProperties):
     async def group_message(self, *segments: "T_SegmentInstance"):
-        return await TelegramApi.group_message(self.group_id, *segments)
+        return await TelegramAPI.group_message(self.group_id, *segments)
 
 
-class TelegramPrivateApi(TelegramProperties):
+class TelegramPrivateAPI(TelegramProperties):
     async def private_message(self, *segments: "T_SegmentInstance"):
-        return await TelegramApi.private_message(self.private_id, *segments)
+        return await TelegramAPI.private_message(self.private_id, *segments)
 
 
-class TelegramGroupBot(TelegramCommonApi, TelegramGroupApi):
+class TelegramGroupBot(TelegramGroupAPI):
     __slots__ = (
         "bot_id",
         "group_id",
         "api_caller",
     )
 
     def __init__(self, bot_id: str, group_id: str):
         self.bot_id = bot_id
         self.group_id = group_id
         self.api_caller = get_telegram_caller()
 
 
-class TelegramPrivateBot(TelegramCommonApi, TelegramPrivateApi):
+class TelegramPrivateBot(TelegramPrivateAPI):
     __slots__ = (
         "bot_id",
         "private_id",
         "api_caller",
     )
 
     def __init__(self, bot_id: str, private_id: str):
```

### Comparing `pepperbot-0.3.3/pepperbot/config.py` & `pepperbot-0.3.4/pepperbot/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 
 
 class Logger(BaseModel):
     level: int = logging.INFO
     write_to_log: bool = False
 
 
-class Sqlite(BaseModel):
-    path = "./db.sqlite3"
+class Database(BaseModel):
+    url = "sqlite:///db.sqlite3"
 
 
 class GlobalConfig(BaseSettings):
     class Config:
         env_file = ".env"
         env_file_encoding = "utf-8"
         env_prefix = "p_"
         env_nested_delimiter = "__"
 
     debug = Debug()
     logger = Logger()
-    sqlite = Sqlite()
+    database = Database()
 
 
 global_config = GlobalConfig()
```

### Comparing `pepperbot-0.3.3/pepperbot/core/bot/api_caller.py` & `pepperbot-0.3.4/pepperbot/core/api/api_caller.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,17 @@
         # 注销client
 
         self.client.close()
 
         # todo 没有找到在del中调用AsyncClient.aclose的方法
         # self.client.aclose().__await__()
 
-    def to_onebot(self, action: str, kwargs: dict, *, direct=True) -> dict[str, Any]:
+    def to_onebot(
+        self, action: str, kwargs: dict = {}, *, direct=True
+    ) -> dict[str, Any]:
         """direct时，直接返回["data"]"""
 
         # debug_log(kwargs)
         httpx_result = self.client.post(
             f"http://{self.host}:{self.port}/{action}",
             json=kwargs,
         )
@@ -73,15 +75,15 @@
             logger.exception(exception)
             raise exception
 
         except Exception as exception:
             logger.exception("无法序列化协议端返回的数据，请检查是否正确配置了对应的ip、端口、协议")
             raise exception
 
-    def to_keaimao(self, action: str, kwargs) -> dict[str, Any]:
+    def to_keaimao(self, action: str, kwargs={}) -> dict[str, Any]:
         kwargs["event"] = action
 
         debug(kwargs)
 
         return self.client.post(f"http://{self.host}:{self.port}", json=kwargs).json()
 
     async def __call__(self, action: str, **kwargs):
```

### Comparing `pepperbot-0.3.3/pepperbot/core/bot/decorators.py` & `pepperbot-0.3.4/pepperbot/core/api/decorators.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/pepperbot/core/bot/universal.py` & `pepperbot-0.3.4/pepperbot/adapters/universal/api/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,58 @@
 from typing import List, Optional, Type, cast
 
-from pepperbot.adapters.keaimao.api import KeaimaoApi, KeaimaoGroupApi, KeaimaoGroupBot
+from pepperbot.adapters.keaimao.api import KeaimaoAPI, KeaimaoGroupAPI, KeaimaoGroupBot
 from pepperbot.adapters.onebot.api import (
-    OnebotV11Api,
-    OnebotV11GroupApi,
+    OnebotV11API,
+    OnebotV11GroupAPI,
     OnebotV11GroupBot,
 )
-from pepperbot.adapters.telegram.api import TelegramApi, TelegramGroupApi
+from pepperbot.adapters.telegram.api import TelegramAPI, TelegramGroupAPI
 from pepperbot.core.message.chain import T_SegmentInstance
 
 # from pepperbot.core.event.utils import get_bot_instance
 from pepperbot.exceptions import BackendApiError, EventHandleError
 from pepperbot.types import BaseBot, T_BotProtocol
 
 
-class ArbitraryApi:
-    onebot = OnebotV11Api
-    keaimao = KeaimaoApi
-    telegram = TelegramApi
+class ArbitraryAPI:
+    onebot = OnebotV11API
+    keaimao = KeaimaoAPI
+    telegram = TelegramAPI
 
 
 class UniversalProperties(BaseBot):
     protocol: T_BotProtocol
     bot_id: str
     group_id: str
-    arbitrary: Type[ArbitraryApi]
+    arbitrary: Type[ArbitraryAPI]
     onebot: Optional[OnebotV11GroupBot]
     keaimao: Optional[KeaimaoGroupBot]
     # telegram: Optional[TelegramGroupBot]
 
 
-class UniversalCommonApi(UniversalProperties):
-
-    pass
-
-
-class UniversalGroupApi(UniversalProperties):
+class UniversalGroupAPI(UniversalProperties):
     async def group_message(self, *segments: T_SegmentInstance):
         if self.onebot:
             return await self.onebot.group_message(*segments)
 
         elif self.keaimao:
             return await self.keaimao.group_message(*segments)
 
         else:
             raise BackendApiError()
 
     group_msg = group_message
 
 
-class UniversalPrivateApi(UniversalProperties):
+class UniversalPrivateAPI(UniversalProperties):
     pass
 
 
-class UniversalGroupBot(UniversalCommonApi, UniversalGroupApi):
+class UniversalGroupBot(UniversalGroupAPI):
     """
     universal api直接绑定在bot身上，方法都是实例化的，因为最常用
     chain 也实例化，常用
     onebot, keaimao, telegram的方法，不太常用，也可以实例化，
     同一个协议，同一个消息来源，只会多创建一个api实例，可以接受
     """
 
@@ -78,24 +73,24 @@
         group_id: str,
     ):
         self.protocol = protocol
 
         self.bot_id = bot_id
         self.group_id = group_id
 
-        self.arbitrary = ArbitraryApi
+        self.arbitrary = ArbitraryAPI
 
         from pepperbot.core.event.handle import get_or_create_bot
 
         bot_instance = get_or_create_bot(protocol, "group", group_id)
 
         self.onebot = (
             cast(OnebotV11GroupBot, bot_instance) if protocol == "onebot" else None
         )
         self.keaimao = (
             cast(KeaimaoGroupBot, bot_instance) if protocol == "keaimao" else None
         )
         self.telegram = bot_instance if protocol == "telegram" else None
 
 
-class UniversalPrivateBot(UniversalCommonApi, UniversalPrivateApi):
+class UniversalPrivateBot(UniversalPrivateAPI):
     pass
```

### Comparing `pepperbot-0.3.3/pepperbot/core/event/handle.py` & `pepperbot-0.3.4/pepperbot/core/message/chain.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,358 +1,385 @@
-import json
-from typing import Any, Callable, Dict, List, Literal, Optional, Set, Union, cast
-
-import arrow
-from devtools import debug, pformat
-from pepperbot.adapters.keaimao import KeaimaoAdapter
-from pepperbot.adapters.keaimao.api import KeaimaoGroupBot, KeaimaoPrivateBot
-from pepperbot.adapters.onebot import OnebotV11Adapter
-from pepperbot.adapters.onebot.api import OnebotV11GroupBot, OnebotV11PrivateBot
-from pepperbot.adapters.telegram import TelegramAdapter
-from pepperbot.adapters.telegram.api import TelegramGroupBot, TelegramPrivateBot
-from pepperbot.core.bot.universal import UniversalGroupBot, UniversalPrivateBot
-from pepperbot.core.event.base_adapter import BaseAdapter
-from pepperbot.core.event.kwargs import UNIVERSAL_KWARGS_MAPPING
-from pepperbot.core.event.universal import (
-    ALL_GROUP_EVENTS,
-    ALL_META_EVENTS,
-    ALL_PRIVATE_EVENTS,
-    ALL_UNIVERSAL_EVENTS,
-    GROUP_COMMAND_TRIGGER_EVENTS,
-    PRIVATE_COMMAND_TRIGGER_EVENTS,
-    UNIVERSAL_PROTOCOL_EVENT_MAPPING,
-)
-from pepperbot.core.event.utils import skip_current_onebot_event
-from pepperbot.exceptions import EventHandleError, StopPropagation
-from pepperbot.extensions.command.handle import run_class_commands
-from pepperbot.extensions.log import debug_log, logger
-from pepperbot.store.meta import (
-    EventHandlerKwarg,
-    EventMeta,
-    RouteMapping,
-    T_HandlerKwargMapping,
-    class_handler_mapping,
-    get_bot_id,
-    get_onebot_caller,
-    initial_bot_info,
-    onebot_event_meta,
-    route_mapping,
-    route_validator_mapping,
+import re
+from pprint import pprint
+from random import random
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Coroutine,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    cast,
 )
-from pepperbot.types import BaseBot, T_BotProtocol, T_RouteMode
-from pepperbot.utils.common import await_or_sync, deepawait_or_sync, fit_kwargs
-from pyrogram.enums.chat_type import ChatType
-from pyrogram.types import CallbackQuery, Message
-
-
-async def handle_event(protocol: T_BotProtocol, raw_event: Dict):
-    logger.info("-" * 50)
-
-    if not route_mapping.has_initial:
-        await initial_bot_info()
-        logger.success("成功获取bot元信息")
-        route_mapping.has_initial = True
-
-    adapter = get_adapter(protocol)
-    raw_event_name = adapter.get_event_name(raw_event)
-    """ raw event without protocol prefix """
-    protocol_event_name: str = f"{protocol}_" + raw_event_name
-    """ raw event with protocol prefix """
-
-    # go-cqhhtp will buffer outdated messages
-    if protocol == "onebot":
-        if not onebot_event_meta.has_skip_buffered_event:
-            flag = skip_current_onebot_event(raw_event, raw_event_name)
-            if not flag:
-                return
-
-    mode = adapter.get_route_mode(raw_event, raw_event_name)
-    source_id = adapter.get_source_id(raw_event, mode)
-
-    debug_log("", f"mode {mode} source_id {source_id}")
-
-    if not (mode and source_id):
-        if protocol == "onebot":
-            if raw_event_name == "meta_event":
-                logger.info(
-                    f"接收到 <lc>{protocol}</lc> 的元事件 <lc>{raw_event['meta_event_type']}</lc>"
-                )
-                return
-
-        raise EventHandleError(
-            f"无效或尚未适配的事件 <lc>{protocol}</lc> 的事件 <lc>{raw_event_name}</lc>"
-        )
-
-    logger.info(
-        f"接收到 <lc>{protocol}</lc> 的事件 <lc>{raw_event_name}</lc>，来自于 <lc>{mode}</lc> 模式的 <lc>{source_id}</lc>"
-    )
-
-    event_meta = EventMeta(
-        protocol=protocol,
-        mode=mode,
-        source_id=source_id,
-        raw_event=raw_event,
-        raw_event_name=raw_event_name,
-        protocol_event_name=protocol_event_name,
-    )
 
-    await dispatch_class_commands(event_meta)
-    await dispatch_class_handlers(event_meta)
+from devtools import debug
+from pepperbot.core.message.base import BaseMessageSegment
 
-
-PROTOCOL_ADAPTER_MAPPING: Dict[T_BotProtocol, Any] = {
-    "onebot": OnebotV11Adapter,
-    "keaimao": KeaimaoAdapter,
-    "telegram": TelegramAdapter,
+# if TYPE_CHECKING:
+from pepperbot.core.message.segment import (
+    At,
+    Audio,
+    Image,
+    Music,
+    OnebotFace,
+    OnebotShare,
+    Poke,
+    Reply,
+    T_SegmentClass,
+    T_SegmentClassOrInstance,
+    T_SegmentInstance,
+    Text,
+    Video,
+    Voice,
+    keaimao_image_factory,
+    keaimao_text_factory,
+    keaimao_video_factory,
+    onebot_at_factory,
+    onebot_audio_factory,
+    onebot_face_factory,
+    onebot_image_factory,
+    onebot_poke_factory,
+    onebot_reply_factory,
+    onebot_text_factory,
+    onebot_video_factory,
+    telegram_image_factory,
+    telegram_text_factory,
+    telegram_video_factory,
+)
+from pepperbot.exceptions import EventHandleError
+from pepperbot.extensions.log import logger
+from pepperbot.store.event import EventMetadata
+from pepperbot.types import T_BotProtocol, T_ConversationType
+from pepperbot.utils.common import await_or_sync
+from pyrogram.enums.message_media_type import MessageMediaType
+
+
+ONEBOT_SEGMENT_FACTORY_MAPPING: Dict[str, Callable[[Dict], T_SegmentInstance]] = {
+    "at": onebot_at_factory,
+    "record": onebot_audio_factory,
+    "image": onebot_image_factory,
+    "face": onebot_face_factory,
+    "poke": onebot_poke_factory,
+    "reply": onebot_reply_factory,
+    "text": onebot_text_factory,
+    "video": onebot_video_factory,
 }
 
+KEAIMAO_SEGMENT_FACTORY_MAPPING: Dict[int, Callable[[Dict], T_SegmentInstance]] = {
+    3: keaimao_image_factory,
+    1: keaimao_text_factory,
+    43: keaimao_video_factory,
+}
 
-def get_adapter(protocol: T_BotProtocol) -> BaseAdapter:
-    return PROTOCOL_ADAPTER_MAPPING[protocol]
-
-
-async def dispatch_class_commands(event_meta: EventMeta):
-    mode = event_meta.mode
-    protocol = event_meta.protocol
-    source_id = event_meta.source_id
+TELEGRAM_SEGMENT_FACTORY_MAPPING: Dict[
+    Optional[MessageMediaType],
+    Callable[[Dict], Union[T_SegmentInstance, Coroutine[Any, Any, T_SegmentInstance]]],
+] = {
+    MessageMediaType.PHOTO: telegram_image_factory,
+    None: telegram_text_factory,
+    MessageMediaType.VIDEO: telegram_video_factory,
+    # MessageMediaType.STICKER: telegram_sticker_factory,
+}
 
-    command_trigger_events: List[str]
 
-    if mode == "group":
-        command_trigger_events = GROUP_COMMAND_TRIGGER_EVENTS
-    elif mode == "private":
-        command_trigger_events = PRIVATE_COMMAND_TRIGGER_EVENTS
-    else:
-        raise EventHandleError(f"")
+async def construct_segments(
+    protocol: T_BotProtocol, mode: T_ConversationType, raw_event: Dict
+) -> List[T_SegmentInstance]:
+    result: List[T_SegmentInstance] = []
 
-    if not event_meta.protocol_event_name in command_trigger_events:
-        logger.info(
-            f"<lc>{protocol}</lc> 的事件 <lc>{event_meta.raw_event_name}</lc> 非指令触发事件"
+    if protocol == "onebot":
+        raw_chain: List[dict] = raw_event.get("message", list)
+        for raw_segment in raw_chain:
+            segment_type: str = raw_segment["type"]
+
+            segment_factory = ONEBOT_SEGMENT_FACTORY_MAPPING.get(segment_type)
+            if not segment_factory:
+                # raise EventHandleError()
+                logger.error(f"尚未适配的 {protocol} 消息类型 {segment_type}，将忽略该消息片段")
+                continue
+
+            segment_instance = segment_factory(raw_segment)
+            result.append(segment_instance)
+
+    elif protocol == "keaimao":
+        message_type: int = raw_event["type"]
+        message_factory = KEAIMAO_SEGMENT_FACTORY_MAPPING.get(message_type)
+        if not message_factory:
+            # raise EventHandleError(f"尚未适配的可爱猫消息类型")
+            logger.error(f"尚未适配的 {protocol} 消息类型 {message_type}，将忽略该消息片段")
+            return []
+
+        segment_instance = message_factory(raw_event)
+        result.append(segment_instance)
+
+    elif protocol == "telegram":
+        telegram_message_type: Optional[MessageMediaType] = getattr(
+            raw_event["callback_object"], "media", None
         )
-        return
-
-    class_command_names: Set[str] = set()
-    """ 在global_commands、mapping、validator中重复注册的指令应该只运行一次 """
-
-    # 单一消息来源
-    class_command_names |= route_mapping.global_commands[protocol][mode]
-    class_command_names |= route_mapping.mapping[protocol][mode][source_id]["commands"]
-    class_command_names |= await with_validators(mode, source_id, "commands")
+        message_factory = TELEGRAM_SEGMENT_FACTORY_MAPPING.get(telegram_message_type)
+        if not message_factory:
+            # raise EventHandleError(f"尚未适配的 telegram 消息类型")
+            logger.error(f"尚未适配的 {protocol} 消息类型 {telegram_message_type}，将忽略该消息片段")
+            return []
 
-    if not class_command_names:
-        logger.info(f"<lc>{mode}</lc> 模式的 <lc>{source_id}</lc> 尚未注册指令")
-        return
+        segment_instance = await await_or_sync(message_factory, raw_event)
+        result.append(segment_instance)
 
-    logger.info(f"<lc>{mode}</lc> 模式的 <lc>{source_id}</lc> 存在注册的指令，开始执行")
-    await run_class_commands(event_meta, class_command_names)
-
-    # lock_user
-    # for rule_id, rule in lock_user_mapping.items():
-    #     if source_id in rule[protocol]:
-    #         await run_class_command(mode="lock_user",rule_id)
-
-    # if mode =="group" or mode =="channel":
-    #     lock_source_mapping
-
-    # lock_source
-
-
-async def dispatch_class_handlers(event_meta: EventMeta):
-
-    mode = event_meta.mode
-    protocol = event_meta.protocol
-    source_id = event_meta.source_id
-
-    class_handler_names: Set[str] = set()
-    """ 对同一个消息来源，在处理一次事件时,同一个class_handler也只应调用一次 """
+    else:
+        raise EventHandleError(f"尚未支持 {protocol} 的消息链构造")
 
-    class_handler_names |= route_mapping.global_handlers[protocol][mode]
-    class_handler_names |= route_mapping.mapping[protocol][mode][source_id][
-        "class_handlers"
-    ]
-    class_handler_names |= await with_validators(mode, source_id, "commands")
+    # debug(result)
+    return result
 
-    debug_log(class_handler_names, "所有可用class_handler")
 
-    if not class_handler_names:
-        logger.info(
-            f"<lc>{event_meta.mode}</lc> 模式的 <lc>{event_meta.source_id}</lc> 尚未注册class_handler"
-        )
-        return
+async def chain_factory(event_meta: EventMetadata):
+    chain = MessageChain(
+        event_meta.protocol,
+        # 能够构造MessageChain的事件，一定可以获取到conversation_type
+        cast(T_ConversationType, event_meta.conversation_type),
+        event_meta.raw_event,
+        event_meta.source_id,
+        event_meta.user_id,
+    )
+    await chain.construct()
+    return chain
 
-    # 比如group_message这样的实现了统一事件的事件
-    # 如果用户同时定义了group_message和onebot_group_message，应该执行两次
-    event_mapping = UNIVERSAL_PROTOCOL_EVENT_MAPPING.get(event_meta.raw_event_name)
-    if event_mapping and event_meta.protocol_event_name in event_mapping:
-        await run_class_handlers(
-            event_meta,
-            class_handler_names,
-            universal=True,
-        )
 
-    await run_class_handlers(
-        event_meta,
-        class_handler_names,
+class MessageChain:
+    __slots__ = (
+        "id",
+        "segments",
+        "raw_event",
+        "source_id",
+        "user_id",
+        "protocol",
+        "mode",
+        "onebot_message_id",
     )
 
+    onebot_message_id: str
 
-async def with_validators(
-    mode: T_RouteMode, source_id: str, target: Literal["class_handlers", "commands"]
-):
-    results: Set[str] = set()
-
-    for validator_name, validator_dict in route_mapping.mapping["validators"][
-        mode
-    ].items():
-        validator = route_validator_mapping[validator_name]
-
-        if await await_or_sync(validator, **{"mode": mode, "source_id": source_id}):
-            results |= validator_dict[target]
-
-    return results
-
-
-async def run_class_handlers(
-    event_meta: EventMeta,
-    class_handler_names: Set[str],
-    universal=False,
-):
-    if universal:
-        target_event_name = event_meta.raw_event_name
-    else:
-        target_event_name = event_meta.protocol_event_name
-
-    kwargs = await get_event_handler_kwargs(event_meta, universal=universal)
-    debug_log(kwargs, f"当前事件 <lc>{target_event_name}</lc> 可用的参数")
+    def __init__(
+        self,
+        protocol: T_BotProtocol,
+        mode: T_ConversationType,
+        raw_event: Dict,
+        source_id: str,
+        user_id: str,
+    ) -> None:
+        # debug(locals())
+
+        self.id = random()
+        self.segments: List[T_SegmentInstance] = []
+
+        self.raw_event = raw_event
+        self.source_id = source_id
+        self.user_id = user_id
+        self.protocol = protocol
+        self.mode = mode
+
+        self.onebot_message_id = raw_event.get("message_id", "")
+
+    async def construct(self):
+        self.segments = await construct_segments(
+            self.protocol,  # type:ignore
+            self.mode,  # type:ignore
+            self.raw_event,
+        )
 
-    for class_handler_name in class_handler_names:
-        class_handler_cache = class_handler_mapping[class_handler_name]
-        debug_log(class_handler_cache)
-
-        event_handler = class_handler_cache.event_handlers.get(target_event_name)
-        if not event_handler:
-            logger.info(
-                f"class_handler <lc>{class_handler_name}</lc> 未定义 <lc>{target_event_name}</lc>"
-            )
-            return
+    # def __repr__(self) -> str:
+    #     json.dumps
 
-        logger.info(
-            f"开始执行class_handler <lc>{class_handler_name}</lc> 的事件响应 <lc>{target_event_name}</lc>",
+    def __equal(self, segment: "BaseMessageSegment", other: T_SegmentClassOrInstance):
+        # 如果是实例，data是否相等
+        if isinstance(other, BaseMessageSegment):
+            if segment == other:
+                return True
+
+        # 是否是同一类型
+        else:
+            if type(segment) == other:
+                return True
+
+        return False
+
+    # todo part in raw operator in
+    # if
+
+    def has(self, other: T_SegmentClassOrInstance):
+        for segment in self.segments:
+            if self.__equal(segment, other):
+                return True
+
+        return False
+
+    def has_and_first(
+        self, other: T_SegmentClassOrInstance
+    ) -> Tuple[bool, T_SegmentInstance]:
+        for segment in self.segments:
+            if self.__equal(segment, other):
+                return True, segment
+
+        # 返回Text只是为了提供更好的类型注解，因为python并不能自动判断union类型的分支情况
+        # 即 True => type1 , False => type2
+        # generic可以，不过还是直接Text("")最简单
+        return False, Text("")
+
+    def has_and_last(self, other: T_SegmentClassOrInstance):
+        for segment in reversed(self.segments):
+            if self.__equal(segment, other):
+                return True, segment
+
+        return False, Text("")
+
+    def has_and_all(self, other: T_SegmentClassOrInstance):
+        results = []
+
+        for segment in self.segments:
+            if self.__equal(segment, other):
+                results.append(segment)
+
+        if len(results):
+            return True, results
+        return False, Text("")
+
+    def __getItems(self, type_: T_SegmentClass):
+        results = []
+
+        for segment in self.segments:
+            if isinstance(segment, type_):
+                results.append(segment)
+
+        return results
+
+    @property
+    def at(self) -> List[At]:
+        return self.__getItems(At)
+
+    @property
+    def onebot_faces(self) -> List[OnebotFace]:
+        return self.__getItems(OnebotFace)
+
+    @property
+    def audio(self) -> List[Audio]:
+        return self.__getItems(Audio)
+
+    @property
+    def images(self) -> List[Image]:
+        return self.__getItems(Image)
+
+    @property
+    def replies(self) -> List[Reply]:
+        return self.__getItems(Reply)
+
+    @property
+    def music(self) -> List[Music]:
+        return self.__getItems(Music)
+
+    @property
+    def text(self) -> List[Text]:
+        return self.__getItems(Text)
+
+    @property
+    def pure_text(self) -> str:
+        result = ""
+        for segment in self.text:
+            result += segment.content
+
+        return result
+
+    def any(self, *parts: str):
+        for part in parts:
+            if part in self.pure_text:
+                return True
+        return False
+
+    def regex(self, part: str):
+        if re.search(part, self.pure_text):
+            return True
+        return False
+
+    def regex_any(self, *parts: str):
+        for part in parts:
+            if re.search(part, self.pure_text):
+                return True
+        return False
+
+    def all(self, *parts: str):
+        for part in parts:
+            if part not in self.pure_text:
+                return False
+        return True
+
+    def regex_all(self, *parts: str):
+        for part in parts:
+            if not re.search(part, self.pure_text):
+                return False
+        return True
+
+    def startswith(self, string: str):
+        return self.pure_text.startswith(string)
+
+    def endswith(self, string: str):
+        return self.pure_text.endswith(string)
+
+    async def onebot_reply(self, *segments: T_SegmentInstance):
+        from pepperbot.adapters.onebot.api import OnebotV11API
+
+        if self.mode == "group":
+            api = OnebotV11API.group_message
+        else:
+            api = OnebotV11API.private_message
+
+        return await api(
+            self.source_id,
+            *[Reply(self.onebot_message_id), *segments],
         )
 
-        try:
-            await await_or_sync(event_handler, **fit_kwargs(event_handler, kwargs))
-
-        except StopPropagation:
-            logger.info(f"用户抛出 StopPropagation，停止执行后续事件响应")
-            break
-
-        except:
-            logger.exception("当前事件响应执行异常，将继续执行下一个事件响应")
-
-
-async def get_event_handler_kwargs(
-    event_meta: EventMeta,
-    universal=False,
-) -> Dict[str, Any]:
-    """
-    不包含meta event, common + group + private
-
-    telegram的common事件，也已经识别好了mode，不需要手动判断
-    """
-
-    protocol = event_meta.protocol
-    mode = event_meta.mode
-    source_id = event_meta.source_id
-    raw_event = event_meta.raw_event
-
-    if universal:
-        mapping = UNIVERSAL_KWARGS_MAPPING
-        # universal内部会根据protocol创建对应的bot实例，并挂载
-        # 比如self.onebot == OnebotV11GroupBot
-        bot_instance = get_or_create_bot(protocol, mode, source_id, universal=True)
+    async def onebot_withdraw(
+        self,
+    ):
+        """仅群聊中有效，需要管理员权限"""
 
-    else:
-        adapter = get_adapter(protocol)
+        from pepperbot.adapters.onebot.api import OnebotV11API
 
-        # event_name已经在handler_event中校验过存在，不需要再校验
-        # if event_meta.raw_event_name not in adapter.all_events:
-        #     raise EventHandleError(
-        #         f"尚未为 <lc>{protocol}</lc> 事件 <lc>{event_meta.raw_event_name}</lc> 适配参数"
-        #     )
-
-        mapping = adapter.kwargs
-        bot_instance = get_or_create_bot(protocol, mode, source_id)
-
-    injected_kwargs = dict(
-        protocol=protocol,
-        mode=mode,
-        source_id=source_id,
-        raw_event=raw_event,
-        event_meta=event_meta,
-        bot=bot_instance,
-    )
+        return await OnebotV11API.withdraw_message(self.onebot_message_id)
 
-    kwarg_list: List[EventHandlerKwarg] = mapping.get(event_meta.raw_event_name, [])
-    kwargs: Dict[str, Any] = {}
+    def __getitem__(self, index: int) -> T_SegmentInstance:
+        return self.segments[index]
 
-    for kwarg in kwarg_list:
-        kwargs[kwarg.name] = await deepawait_or_sync(
-            kwarg.value,
-            **fit_kwargs(kwarg.value, injected_kwargs),
-        )
+    def __contains__(self, item: Union[str, T_SegmentClassOrInstance]):
+        if isinstance(item, str):
+            if item in self.pure_text:
+                return True
 
-    return kwargs
+        else:
+            for segment in self.segments:
+                if self.__equal(segment, item):
+                    return True
 
+        return False
 
-def get_or_create_bot(
-    protocol: T_BotProtocol,
-    mode: T_RouteMode,
-    identifier: str,
-    universal=False,
-) -> BaseBot:
+    def __eq__(self, other: "MessageChain") -> bool:
+        if not isinstance(other, MessageChain):
+            return False
 
-    instances_dict = route_mapping.bot_instances
+        return self.id == other.id
 
-    if universal:
-        key = ("universal", mode, identifier)
-    else:
-        key = (protocol, mode, identifier)
+    def __len__(self):
+        return len(self.segments)
 
-    bot_instance: Optional[BaseBot] = None
+    def only(self, _type: T_SegmentClassOrInstance) -> bool:
+        for segment in self.segments:
+            if not self.__equal(segment, _type):
+                return False
 
-    if key in instances_dict:
-        bot_instance = instances_dict[key]
-        return bot_instance
-
-    if universal:
-        # ? todo private add_group
-        bot_instance = UniversalGroupBot(protocol, mode, identifier)
-        return bot_instance
-
-    bot_id = get_bot_id(protocol)
-
-    # 如果能用3.10的match就好了
-    if mode == "group":
-        if protocol == "onebot":
-            bot_instance = OnebotV11GroupBot(bot_id, identifier)
-        elif protocol == "keaimao":
-            bot_instance = KeaimaoGroupBot(bot_id, identifier)
-        elif protocol == "telegram":
-            bot_instance = TelegramGroupBot(bot_id, identifier)
-
-    elif mode == "private":
-        if protocol == "onebot":
-            bot_instance = OnebotV11PrivateBot(bot_id, identifier)
-        elif protocol == "keaimao":
-            bot_instance = KeaimaoPrivateBot(bot_id, identifier)
-        elif protocol == "telegram":
-            bot_instance = TelegramPrivateBot(bot_id, identifier)
-
-    if not bot_instance:
-        raise EventHandleError(
-            f"未能创建bot实例 <lc>{protocol}</lc> <lc>{mode}</lc> <lc>{identifier}</lc>"
-        )
+        return True
 
-    instances_dict[key] = bot_instance
+    def only_one(self, _type: T_SegmentClassOrInstance) -> bool:
+        if len(self.segments) != 1:
+            return False
 
-    return bot_instance
+        return self.__equal(self.segments[0], _type)
```

### Comparing `pepperbot-0.3.3/pepperbot/core/event/utils.py` & `pepperbot-0.3.4/pepperbot/core/event/utils.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/pepperbot/core/message/base.py` & `pepperbot-0.3.4/pepperbot/core/message/base.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/pepperbot/core/message/chain.py` & `pepperbot-0.3.4/pepperbot/extensions/command/pattern.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,394 +1,392 @@
 import re
-from pprint import pprint
-from random import random
+from copy import deepcopy
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
-    Coroutine,
     Dict,
     List,
     Optional,
+    OrderedDict,
     Tuple,
     Union,
+    cast,
 )
 
-from devtools import debug
-from pepperbot.core.message.base import BaseMessageSegment
-
-# if TYPE_CHECKING:
-from pepperbot.core.message.segment import (
-    At,
-    Audio,
-    Image,
-    Music,
-    OnebotFace,
-    OnebotShare,
-    Poke,
-    Reply,
-    T_SegmentClass,
-    T_SegmentClassOrInstance,
-    T_SegmentInstance,
-    Text,
-    Video,
-    Voice,
-    keaimao_image_factory,
-    keaimao_text_factory,
-    keaimao_video_factory,
-    onebot_at_factory,
-    onebot_audio_factory,
-    onebot_face_factory,
-    onebot_image_factory,
-    onebot_poke_factory,
-    onebot_reply_factory,
-    onebot_text_factory,
-    onebot_video_factory,
-    telegram_image_factory,
-    telegram_text_factory,
-    telegram_video_factory,
+from pepperbot.core.message.chain import MessageChain, T_SegmentInstance
+from pepperbot.core.message.segment import Text
+from pepperbot.exceptions import PatternFormatError
+from pepperbot.extensions.log import debug_log, logger
+from pepperbot.store.command import (
+    FALSE_TEXTS,
+    TRUE_TEXTS,
+    VALID_TEXT_TYPES,
+    ClassCommandMethodCache,
+    GT_PatternArg,
+    T_CompressedPatterns,
+    T_PatternArgClass,
+    T_PatternArgInstance,
+    T_ValidTextTypeClass,
+    T_ValidTextTypeInstance,
 )
-from pepperbot.exceptions import EventHandleError
-from pepperbot.extensions.log import logger
-from pepperbot.store.meta import EventMeta
-from pepperbot.types import T_BotProtocol, T_RouteMode
-from pepperbot.utils.common import await_or_sync
-from pyrogram.enums.message_media_type import MessageMediaType
-
-
-ONEBOT_SEGMENT_FACTORY_MAPPING: Dict[str, Callable[[Dict], T_SegmentInstance]] = {
-    "at": onebot_at_factory,
-    "record": onebot_audio_factory,
-    "image": onebot_image_factory,
-    "face": onebot_face_factory,
-    "poke": onebot_poke_factory,
-    "reply": onebot_reply_factory,
-    "text": onebot_text_factory,
-    "video": onebot_video_factory,
-}
-
-KEAIMAO_SEGMENT_FACTORY_MAPPING: Dict[int, Callable[[Dict], T_SegmentInstance]] = {
-    3: keaimao_image_factory,
-    1: keaimao_text_factory,
-    43: keaimao_video_factory,
-}
-
-TELEGRAM_SEGMENT_FACTORY_MAPPING: Dict[
-    Optional[MessageMediaType],
-    Callable[[Dict], Union[T_SegmentInstance, Coroutine[Any, Any, T_SegmentInstance]]],
-] = {
-    MessageMediaType.PHOTO: telegram_image_factory,
-    None: telegram_text_factory,
-    MessageMediaType.VIDEO: telegram_video_factory,
-    # MessageMediaType.STICKER: telegram_sticker_factory,
-}
-
-
-async def construct_segments(
-    protocol: T_BotProtocol, mode: T_RouteMode, raw_event: Dict
-) -> List[T_SegmentInstance]:
-
-    result: List[T_SegmentInstance] = []
-
-    if protocol == "onebot":
-        raw_chain: List[dict] = raw_event.get("message", list)
-        for raw_segment in raw_chain:
-            segment_type: str = raw_segment["type"]
-
-            segment_factory = ONEBOT_SEGMENT_FACTORY_MAPPING.get(segment_type)
-            if not segment_factory:
-                # raise EventHandleError()
-                logger.error(f"尚未适配的 {protocol} 消息类型 {segment_type}，将忽略该消息片段")
-                continue
-
-            segment_instance = segment_factory(raw_segment)
-            result.append(segment_instance)
-
-    elif protocol == "keaimao":
-        message_type: int = raw_event["type"]
-        message_factory = KEAIMAO_SEGMENT_FACTORY_MAPPING.get(message_type)
-        if not message_factory:
-            # raise EventHandleError(f"尚未适配的可爱猫消息类型")
-            logger.error(f"尚未适配的 {protocol} 消息类型 {message_type}，将忽略该消息片段")
-            return []
-
-        segment_instance = message_factory(raw_event)
-        result.append(segment_instance)
-
-    elif protocol == "telegram":
-        telegram_message_type: Optional[MessageMediaType] = getattr(
-            raw_event["callback_object"], "media", None
-        )
-        message_factory = TELEGRAM_SEGMENT_FACTORY_MAPPING.get(telegram_message_type)
-        if not message_factory:
-            # raise EventHandleError(f"尚未适配的 telegram 消息类型")
-            logger.error(f"尚未适配的 {protocol} 消息类型 {telegram_message_type}，将忽略该消息片段")
-            return []
 
-        segment_instance = await await_or_sync(message_factory, raw_event)
-        result.append(segment_instance)
+if TYPE_CHECKING:
+    from pepperbot.extensions.command.sender import CommandSender
 
-    else:
-        raise EventHandleError(f"尚未支持 {protocol} 的消息链构造")
 
-    # debug(result)
-    return result
+def merge_multi_text_with_space(*texts: Text):
+    """
+    为什么要合并字符串呢？应为接收到的消息类型，可能是分片的，也可能是连续的，
+    为了保持一致，全部转换成连续的，再进行正则会方便很多
+    """
+    merged_string = ""
+    text_count = len(texts)
 
+    for index, text in enumerate(texts, start=1):
+        merged_string += text.content
 
-async def chain_factory(event_meta: EventMeta):
-    chain = MessageChain(
-        event_meta.protocol,
-        event_meta.mode,
-        event_meta.raw_event,
-        event_meta.source_id,
-    )
-    await chain.construct()
-    return chain
-
-
-class MessageChain:
-    __slots__ = (
-        "id",
-        "segments",
-        "raw_event",
-        "source_id",
-        "protocol",
-        "mode",
-        "onebot_message_id",
-    )
-
-    onebot_message_id: str
-
-    def __init__(
-        self,
-        protocol: T_BotProtocol,
-        mode: T_RouteMode,
-        raw_event: Dict,
-        source_id: str,
-    ) -> None:
-        """
-        [summary]
-
-        Args:
-            event: [description]
-            source_id: 当mode为group时，source_id就是group_id，mode为private时同理
-            protocol: [description]
-            mode: [description]
-
-        """
-        # debug(locals())
-
-        self.id = random()
-        self.segments: List[T_SegmentInstance] = []
-
-        self.raw_event = raw_event
-        self.source_id = source_id
-        self.protocol = protocol
-        self.mode = mode
-
-        self.onebot_message_id = raw_event.get("message_id", "")
-
-    async def construct(self):
-        self.segments = await construct_segments(
-            self.protocol,  # type:ignore
-            self.mode,  # type:ignore
-            self.raw_event,
-        )
+        if index != text_count:
+            merged_string += " "
+
+    return Text(merged_string)
+
+
+T_CompressedSegments = List[T_SegmentInstance]
+
+
+def merge_text_of_segments(segments: List[T_SegmentInstance]) -> T_CompressedSegments:
+    """合并相邻的Text片段，空格分隔，方便正则"""
+    debug_log(segments)
+
+    if len(segments) <= 1:
+        return segments
 
-    # def __repr__(self) -> str:
-    #     json.dumps
+    compressed_segments: T_CompressedSegments = []
 
-    def __equal(self, segment: "BaseMessageSegment", other: T_SegmentClassOrInstance):
-        # 如果是实例，data是否相等
-        if isinstance(other, BaseMessageSegment):
-            if segment == other:
-                return True
+    text_buffer: List[Text] = []
+    last_segment_type = Text
+    segments_count = len(segments)
 
-        # 是否是同一类型
+    for index, segment in enumerate(segments, start=1):
+        # True, True
+        if last_segment_type == Text and isinstance(segment, Text):
+            text_buffer.append(segment)
+
+            if index == segments_count:
+                compressed_segments.append(merge_multi_text_with_space(*text_buffer))
+
+        # False, True
+        elif last_segment_type != Text and isinstance(segment, Text):
+            text_buffer.append(segment)
+
+            if index == segments_count:
+                compressed_segments.append(merge_multi_text_with_space(*text_buffer))
+
+        # True, False
+        elif last_segment_type == Text and not isinstance(segment, Text):
+            if text_buffer:
+                compressed_segments.append(merge_multi_text_with_space(*text_buffer))
+                text_buffer = []
+
+            compressed_segments.append(segment)
+
+        # False, False
         else:
-            if type(segment) == other:
-                return True
+            compressed_segments.append(segment)
 
-        return False
+        last_segment_type = segment.__class__
 
-    # todo part in raw operator in
-    # if
+    return compressed_segments
 
-    def has(self, other: T_SegmentClassOrInstance):
-        for segment in self.segments:
-            if self.__equal(segment, other):
-                return True
 
-        return False
+def merge_text_of_patterns(
+    patterns: List[Tuple[str, T_PatternArgClass]]
+) -> T_CompressedPatterns:
+    """
+    合并patterns中的str, int, float, bool, 即python的四种简单类型
+    不管有几个连续的Textable segment，都解析为List[Tuple[str, ModelField]]
+
+    其它类型解析为Tuple[str, ModelField]
+
+    [
+        [
+            ("字符1", str),
+            ("字符2", float),
+            ("字符3", int),
+        ],
+        ("表情1", Face),
+        ("图片1", Image),
+        [
+            ("字符4", bool),
+            ("字符5", float),
+        ],
+    ]
+    """
+    if not patterns:
+        return []
+
+    # 只有一个元素的情况
+    if len(patterns) == 1:
+        arg_type = patterns[0][1]
 
-    def has_and_first(
-        self, other: T_SegmentClassOrInstance
-    ) -> Tuple[bool, T_SegmentInstance]:
-        for segment in self.segments:
-            if self.__equal(segment, other):
-                return True, segment
+        if arg_type in VALID_TEXT_TYPES:
+            return [patterns]
+        else:
+            return patterns  # type:ignore
 
-        # 返回Text只是为了提供更好的类型注解，因为python并不能自动判断union类型的分支情况
-        # 即 True => type1 , False => type2
-        # generic可以，不过还是直接Text("")最简单
-        return False, Text("")
+    compressed_patterns: T_CompressedPatterns = []
 
-    def has_and_last(self, other: T_SegmentClassOrInstance):
-        for segment in reversed(self.segments):
-            if self.__equal(segment, other):
-                return True, segment
+    text_buffer = []
+    last_pattern_type = str
+    patterns_count = len(patterns)
 
-        return False, Text("")
+    for index, (arg_name, arg_type) in enumerate(patterns, start=1):
+        # Text 都转换为str, 方便比较
+        last_type = str if last_pattern_type in VALID_TEXT_TYPES else last_pattern_type
+        current_type = str if arg_type in VALID_TEXT_TYPES else arg_type
 
-    def has_and_all(self, other: T_SegmentClassOrInstance):
-        results = []
+        # True, True
+        if last_type == current_type == str:
+            text_buffer.append((arg_name, arg_type))
 
-        for segment in self.segments:
-            if self.__equal(segment, other):
-                results.append(segment)
+            if index == patterns_count:
+                compressed_patterns.append(deepcopy(text_buffer))
 
-        if len(results):
-            return True, results
-        return False, Text("")
+        # False, True
+        elif last_type != str and current_type == str:
+            text_buffer.append((arg_name, arg_type))
 
-    def __getItems(self, type_: T_SegmentClass):
-        results = []
+            if index == patterns_count:
+                compressed_patterns.append(deepcopy(text_buffer))
 
-        for segment in self.segments:
-            if isinstance(segment, type_):
-                results.append(segment)
+        # True, False
+        elif last_type == str and current_type != str:
+            if text_buffer:
+                compressed_patterns.append(deepcopy(text_buffer))
+                text_buffer = []
 
-        return results
+            compressed_patterns.append((arg_name, arg_type))
+
+        # False, False
+        else:
+            compressed_patterns.append((arg_name, arg_type))
 
-    @property
-    def at(self)-> list[At]:
-        return self.__getItems(At)
-
-    @property
-    def onebot_faces(self)-> list[OnebotFace]:
-        return self.__getItems(OnebotFace)
-
-    @property
-    def audio(self)-> list[Audio]:
-        return self.__getItems(Audio)
-
-    @property
-    def images(self)-> list[Image]:
-        return self.__getItems(Image)
-
-    @property
-    def replies(self)-> list[Reply]:
-        return self.__getItems(Reply)
-
-    @property
-    def music(self)-> list[Music]:
-        return self.__getItems(Music)
-
-    @property
-    def text(
-        self,
-    ) -> list[Text]:
-        return self.__getItems(Text)
-
-    @property
-    def pure_text(self) -> str:
-        result = ""
-        for segment in self.text:
-            result += segment.content
-
-        return result
-
-    def any(self, *parts: str):
-        for part in parts:
-            if part in self.pure_text:
-                return True
-        return False
-
-    def regex(self, part: str):
-        if re.search(part, self.pure_text):
-            return True
-        return False
-
-    def regex_any(self, *parts: str):
-        for part in parts:
-            if re.search(part, self.pure_text):
-                return True
-        return False
-
-    def all(self, *parts: str):
-        for part in parts:
-            if part not in self.pure_text:
-                return False
-        return True
-
-    def regex_all(self, *parts: str):
-        for part in parts:
-            if not re.search(part, self.pure_text):
-                return False
-        return True
-
-    def startswith(self, string: str):
-        return self.pure_text.startswith(string)
+        last_pattern_type = arg_type
 
-    def endswith(self, string: str):
-        return self.pure_text.endswith(string)
+    return compressed_patterns
 
-    async def onebot_reply(self, *segments: T_SegmentInstance):
-        from pepperbot.adapters.onebot.api import OnebotV11Api
 
-        if self.mode == "group":
-            api = OnebotV11Api.group_message
+def match_by_regex(
+    text_patterns: List[Tuple[str, T_ValidTextTypeClass]], segment: Text
+):
+    """通过正则，匹配对应的text和pattern"""
+    regex = r""
+    arg_count = len(text_patterns)
+
+    for index, text_pattern in enumerate(text_patterns):
+        (arg_name, arg_type) = text_pattern
+
+        # 拼接正则，所有文字参数，应该都是空格分格的
+        if index != arg_count - 1:
+            regex += r"(\S+)\s*"
         else:
-            api = OnebotV11Api.private_message
+            regex += r"(\S+)"
 
-        return await api(
-            self.source_id,
-            *[Reply(self.onebot_message_id), *segments],
-        )
+        # logger.debug(pformat(arg_type))
 
-    async def onebot_withdraw(
-        self,
-    ):
-        # await self.api(
-        #     "delete_msg",
-        #     **{
-        #         "message_id": self.messageId,
-        #     },
-        # )
-        pass
+    # logger.debug(pformat(regex, segment.content))
+    match = re.search(regex, segment.content)
+    if not match:
+        raise PatternFormatError(f"pattern匹配失败-->正则失败")
+
+    texts = match.groups()
+    # logger.debug(pformat(texts))
+
+    if len(texts) != arg_count:
+        raise PatternFormatError(f"未按照格式提供参数 参数之间使用空格分隔")
+
+    return texts
+
+
+def try_convert_type(
+    arg_name: str, arg_type: T_ValidTextTypeClass, text_without_type: str
+):
+    # logger.debug(pformat(text_without_type, arg_type))
+
+    result: T_ValidTextTypeInstance
 
-    def __getitem__(self, index: int) -> T_SegmentInstance:
-        return self.segments[index]
+    if arg_type == str:
+        result = text_without_type
 
-    def __contains__(self, item: Union[str, T_SegmentClassOrInstance]):
-        if isinstance(item, str):
-            if item in self.pure_text:
-                return True
+    if arg_type == bool:
+        if not (text_without_type in TRUE_TEXTS or text_without_type in FALSE_TEXTS):
+            raise PatternFormatError(f"未按照格式提供参数 {arg_name} 应为bool类型")
 
         else:
-            for segment in self.segments:
-                if self.__equal(segment, item):
-                    return True
+            if text_without_type in TRUE_TEXTS:
+                result = True
+            else:
+                result = False
+
+    else:  # 解析int, float
+        try:
+            result = arg_type(text_without_type)  # type:ignore
 
-        return False
+        except Exception as e:
+            raise PatternFormatError(f"未按照格式提供参数 {arg_name}应为{arg_type}类型")
 
-    def __eq__(self, other: "MessageChain") -> bool:
-        if not isinstance(other, MessageChain):
-            return False
+    return result
+
+
+def get_pattern_results(
+    compressed_patterns: List[
+        Union[List[Tuple[str, GT_PatternArg]], Tuple[str, GT_PatternArg]]
+    ],
+    compressed_segments: List[T_SegmentInstance],
+):
+    pattern_result: OrderedDict[str, T_PatternArgInstance] = OrderedDict()
+
+    for index, (segment, pattern) in enumerate(
+        zip(compressed_segments, compressed_patterns)
+    ):
+        # logger.debug(pformat(type(segment)))
+        # logger.debug(pformat(type(chunk)))
 
-        return self.id == other.id
+        if isinstance(segment, Text):
+            if not isinstance(pattern, list):  # 所有text都被解析为list[(arg_name, arg_type)]
+                raise PatternFormatError("未按照格式提供参数")
+
+            text_patterns = cast(List[Tuple[str, T_ValidTextTypeClass]], pattern)
+            texts = match_by_regex(text_patterns, segment)
+
+            for index, text_without_type in enumerate(texts):
+                arg_name, arg_type = text_patterns[index]
+
+                pattern_result[arg_name] = try_convert_type(
+                    arg_name,
+                    arg_type,
+                    text_without_type,
+                )
+
+        # todo 支持pydantic的Field，比如gt,lt,对输出的报错信息，转为PatternFormotError
+        # 最好能找到，pydantic中是怎么使用ModelField进行字段验证的，只是使用就好了
+        # snap: int = Field(
+        #     42,
+        #     title="The Snap",
+        #     description="this is the value of snap",
+        #     gt=30,
+        #     lt=50,
+        # )
 
-    def __len__(self):
-        return len(self.segments)
+        # 支持pydantic的validate装饰器
+        # for arg_name, validators in command_pattern.__validators__.items():
+        #     for validator in validators:
+        #         validator.func(command_pattern.__class__, pattern_result[arg_name])
+
+        else:  # 检测是否是有效类型，Face，Image之类
+            pattern = cast(Tuple[str, GT_PatternArg], pattern)
+            arg_name, arg_type = pattern
+
+            if type(segment) != arg_type:
+                raise PatternFormatError(f"未按照格式提供参数 {arg_name} 应为 {arg_type} 类型")
+
+            pattern_result[arg_name] = segment
+
+    return pattern_result
+
+
+def pattern_config(
+    with_format_hint: bool = True,
+    on_format_error: Optional[
+        Callable[[T_CompressedSegments, T_CompressedPatterns], str]
+    ] = None,
+    retry: int = 3,
+):
+    """装饰器，函数粒度的config"""
+    PATTERN_CONFIG = "__pattern_config__"
+    pass
+
+
+async def parse_pattern(
+    cache: ClassCommandMethodCache,
+    method_name,
+    command_kwargs: Dict[str, Any],
+):
+    """
+    根据签名中的PatternArg，自动解析参数，并转换为对应类型，自动注入函数调用中
+
+    满足pattern放行，如果不满足，会对方法调用进行拦截，
+    """
+
+    chain: MessageChain = command_kwargs["chain"]
+    sender: "CommandSender" = command_kwargs["sender"]
+    prefix: str = command_kwargs["prefix"]
+
+    if not cache.compressed_patterns:
+        return {}
+
+    compressed_patterns = cache.compressed_patterns
+
+    # todo pydantic有没有原生的功能
+    # 尝试解析，解析失败，报错
+    # todo List(展开), Any, Union, List[Union/Any]
+
+    format_hint = "请按照 "
+    for arg_name, arg_type in cache.patterns:
+        format_hint += f"<{arg_name} : {arg_type.__name__}> "
+    format_hint += "的格式输入\n不需要输入<或者>，:右侧是该参数的类型"
+
+    # formot_hint添加prefix
+    # if method_name == "initial":
+
+    results = {}
+
+    try:
+        compressed_segments = merge_text_of_segments(chain.segments)
+        debug_log(compressed_segments)
+
+        if len(compressed_segments) != len(compressed_patterns):
+            raise PatternFormatError(
+                f"未提供足够参数，应为{len(cache.patterns)}个，" + f"获得{len(chain.segments)}个"
+            )
+
+        # 对initial应用pattern的情况，支持prefix
+        # 目前仅支持文字prefix
+        if method_name == "initial":
+            if not isinstance(compressed_segments[0], Text):
+                return PatternFormatError("目前仅支持文字前缀")
+
+            with_prefix = compressed_segments[0].content
+            without_prefix = re.sub(f"^{prefix}", "", with_prefix)
+            compressed_segments[0].content = without_prefix
+
+        results = get_pattern_results(compressed_patterns, compressed_segments)
+
+    except PatternFormatError as e:
+        # if on_format_error:
+        #     return_text = await await_or_normal(
+        #         on_format_error, *args, **kwargs
+        #     )
+        #     if return_text:
+        #         await bot.group_msg(return_text)
+        # else:
+        await sender.send_message(
+            # Text(f"{e}\n{formot_hint if with_formot_hint else ''}")
+            Text(f"{e}\n{format_hint}")
+        )
 
-    def only(self, _type: T_SegmentClassOrInstance) -> bool:
-        for segment in self.segments:
-            if not self.__equal(segment, _type):
-                return False
+        logger.error("指令解析失败")
+        raise e  # 需要中断指令的执行
 
-        return True
+    else:
+        # todo patternResults的maxSize
+
+        debug_log(results)
+        return results
 
-    def only_one(self, _type: T_SegmentClassOrInstance) -> bool:
-        if len(self.segments) != 1:
-            return False
+    # finally:
+    # # 满足pattern时，提供解析好的字典
+    # context.setdefault("pattern", {})
+    # context["pattern"][f.__name__] = result
 
-        return self.__equal(self.segments[0], _type)
+    # return await await_or_normal(f, self, *args, **kwargs)
```

### Comparing `pepperbot-0.3.3/pepperbot/core/message/segment.py` & `pepperbot-0.3.4/pepperbot/core/message/segment.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,44 @@
+import base64
+import hashlib
 import os
 from random import random
-from typing import (
-    Any,
-    Dict,
-    List,
-    Literal,
-    Optional,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-)
+from typing import Any, Dict, List, Literal, Optional, Tuple, Type, TypeVar, Union
 
+import aiofiles
+import httpx
 from devtools import debug
-from pepperbot.core.message.base import BaseMessageSegment
-from pepperbot.exceptions import EventHandleError
-from pepperbot.store.meta import get_telegram_caller
 from pyrogram.enums.parse_mode import ParseMode
 from pyrogram.types import Message
 
+from pepperbot.core.message.base import BaseMessageSegment
+from pepperbot.exceptions import EventHandleError
+
 
 async def telegram_download_media(file_id: str, file_name: str):
     """
     通过client.download_media，获取到文件的filepath，实现跨平台转发
 
     https://docs.pyrogram.org/api/methods/download_media?highlight=download_media#pyrogram.Client.download_media
     """
+    from pepperbot.store.meta import get_telegram_caller
+
     client = get_telegram_caller()
 
     await client.download_media(file_id, file_name=file_name)
 
     file_path = f"file:///{os.getcwd()}/downloads/{file_name}"
 
     return file_path
 
 
 class At(BaseMessageSegment):
     __slots__ = ("user_id",)
 
     def __init__(self, user_id: str):
-
         self.user_id = user_id
 
         super().__init__(**{"identifier": user_id})
 
     async def onebot(self):
         return {
             "type": "at",
@@ -66,15 +61,14 @@
     )
 
     def __init__(
         self,
         file_path: str,
         telegram_lazy_download=False,
     ):
-
         self.temporary_file_path = file_path
         self.telegram_lazy_download = telegram_lazy_download
         self.file_path = ""
 
         super().__init__(**{"identifier": file_path})
 
     async def get_file_path(self):
@@ -134,15 +128,14 @@
 
     def __init__(
         self,
         file_path: str,
         mode: Optional[Literal["flash"]] = None,
         telegram_lazy_download=False,
     ):
-
         self.temporary_file_path = file_path
         self.file_path = file_path
 
         self.mode = mode
         self.telegram_lazy_download = telegram_lazy_download
 
         super().__init__(**{"identifier": file_path})
@@ -198,17 +191,50 @@
     async def telegram(self):
         await self.get_file_path()
 
         return {
             "photo": self.file_path,
         }
 
-    def download(self):
-        # todo download
-        pass
+    async def download(
+        self,
+        full_path: Optional[str] = None,
+        save_dir: Optional[str] = None,
+        file_name: Optional[str] = None,
+        extension: str = "jpg",
+    ) -> str:
+        """返回下载后的绝对(完整)路径
+
+        如果提供了full_path(需要提供文件的扩展类型)，则直接下载到该路径，其他参数无效
+        """
+
+        if full_path:
+            save_path = full_path
+        else:
+            # 通过hash值来命名文件，避免重复
+            save_path = f"{file_name if file_name else hash_string(self.temporary_file_path)}.{extension}"
+            if save_dir:
+                save_path = os.path.join(save_dir, save_path)
+
+            save_path = os.path.abspath(save_path)
+
+        if self.temporary_file_path.startswith("http"):
+            await download_file(self.file_path, save_path)
+            return save_path
+
+        elif self.temporary_file_path.startswith("file://"):
+            return self.file_path[7:]
+
+        elif self.temporary_file_path.startswith("base64://"):
+            with open(save_path, "wb") as f:
+                f.write(base64.b64decode(self.temporary_file_path))
+            return save_path
+
+        else:
+            raise EventHandleError(f"无法解析的图片路径 {self.file_path}")
 
     def onebot_to_flash(self):
         self.mode = "flash"
 
         return self
 
     def onebot_un_flash(self):
@@ -227,14 +253,37 @@
             return f"file:///{path}"
         else:
             raise EventHandleError(f"无法解析的图片路径 {path}")
 
     return path
 
 
+def hash_string(string: str):
+    h = hashlib.sha256()
+    h.update(string.encode("utf-8"))
+    return h.hexdigest()
+
+
+async def download_file(url: str, save_path: str):
+    """使用httpx，流式下载"""
+
+    # 以防万一，还是再调用一次，保证绝对是绝对路径
+    absolute_path = os.path.abspath(save_path)
+
+    directory = os.path.dirname(absolute_path)  # 获取文件夹路径
+    if not os.path.exists(directory):  # 如果文件夹不存在
+        os.makedirs(directory)  # 创建文件夹
+
+    async with httpx.AsyncClient() as client:
+        async with client.stream("GET", url) as response:
+            async with aiofiles.open(absolute_path, "wb") as f:
+                async for chunk in response.aiter_bytes(chunk_size=8192):
+                    await f.write(chunk)
+
+
 def onebot_image_factory(raw_segment: Dict):
     file_path = raw_segment["data"].get("url")
     if not file_path:
         raise Exception("无法解析图片地址")
 
     file_path = validate_image_path(file_path)
 
@@ -255,15 +304,14 @@
 class Music(BaseMessageSegment):
     __slots__ = (
         "music_id",
         "source",
     )
 
     def __init__(self, music_id: str, source: Literal["qq", "163", "xm"] = "qq"):
-
         self.music_id = music_id
         self.source = source
 
         super().__init__(**{"identifier": music_id + source})
 
     async def onebot(self):
         return {
@@ -292,15 +340,14 @@
     return Music(validate_image_path(path))
 
 
 class OnebotFace(BaseMessageSegment):
     __slots__ = ("face_id",)
 
     def __init__(self, face_id: int):
-
         self.face_id = face_id
 
         super().__init__(**{"identifier": face_id})
 
     async def onebot(self):
         return {
             "type": "face",
@@ -326,15 +373,14 @@
     def __init__(
         self,
         url: str,
         title: str = "",
         content: Optional[str] = None,
         image_url: Optional[str] = None,
     ):
-
         self.url = url
         self.title = title
         self.content = content
         self.image_url = image_url
 
         super().__init__(**{"identifier": url})
 
@@ -350,15 +396,14 @@
         }
 
 
 class Poke(BaseMessageSegment):
     __slots__ = ("user_id",)
 
     def __init__(self, user_id: str):
-
         self.user_id = user_id
 
         super().__init__(**{"identifier": user_id})
 
     async def onebot(self):
         return {
             "type": "poke",
@@ -373,15 +418,14 @@
     return Poke(user_id)
 
 
 class Reply(BaseMessageSegment):
     __slots__ = ("message_id",)
 
     def __init__(self, message_id: str):
-
         self.message_id = message_id
 
         super().__init__(**{"identifier": message_id})
 
     async def onebot(self):
         return {
             "type": "reply",
@@ -396,15 +440,14 @@
     return Reply(message_id)
 
 
 class Text(BaseMessageSegment):
     __slots__ = ("content",)
 
     def __init__(self, content: str):
-
         self.content = content
 
         super().__init__(**{"identifier": content})
 
     async def onebot(self):
         return {
             "type": "text",
@@ -445,15 +488,14 @@
     )
 
     def __init__(
         self,
         file_path: str,
         telegram_lazy_download=False,
     ):
-
         self.temporary_file_path = file_path
         self.telegram_lazy_download = telegram_lazy_download
         self.file_path = ""
 
         super().__init__(**{"identifier": file_path})
 
     async def get_file_path(self):
@@ -567,10 +609,49 @@
     Text,
     Video,
     Voice,
 )
 T_SegmentClassOrInstance = Union[T_SegmentClass, T_SegmentInstance]
 GT_SegmentClassOrInstance = TypeVar(
     "GT_SegmentClassOrInstance",
-    T_SegmentClass,
-    T_SegmentInstance,
+    Type[At],
+    Type[Audio],
+    Type[Image],
+    Type[Music],
+    Type[OnebotFace],
+    Type[OnebotShare],
+    Type[Poke],
+    Type[Reply],
+    Type[Text],
+    Type[Video],
+    Type[Voice],
+    At,
+    Audio,
+    Image,
+    Music,
+    OnebotFace,
+    OnebotShare,
+    Poke,
+    Reply,
+    Text,
+    Video,
+    Voice,
+)
+GT_PatternArg = TypeVar(
+    "GT_PatternArg",
+    str,
+    int,
+    float,
+    bool,
+    At,
+    Audio,
+    Image,
+    Music,
+    OnebotFace,
+    OnebotShare,
+    Poke,
+    Reply,
+    Text,
+    Video,
+    Voice,
 )
+""" 泛型中的类型，不能是Union的，必须展开 """
```

### Comparing `pepperbot-0.3.3/pepperbot/core/route/cache.py` & `pepperbot-0.3.4/pepperbot/core/route/cache.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,177 +2,123 @@
 import random
 import re
 from ast import Call
 from collections import OrderedDict
 from typing import Callable, Dict, List, Set, Tuple, Union, cast, get_args, get_origin
 
 from devtools import debug
+
 from pepperbot.core.message.segment import Text
 from pepperbot.exceptions import EventHandlerDefineError, InitializationError
 from pepperbot.extensions.command.handle import LIFECYCLE_WITHOUT_PATTERNS
 from pepperbot.extensions.command.pattern import merge_text_of_patterns
 from pepperbot.store.command import (
-    COMMAND_CONFIG,
+    PATTERN_ARG_TYPES,
     ClassCommandCache,
+    ClassCommandConfigCache,
+    ClassCommandMethodCache,
     CommandConfig,
-    CommandMethodCache,
+    GT_PatternArg,
     PatternArg,
-    T_PatternArg,
-    class_command_config_mapping,
-    class_command_mapping,
-    runtime_pattern_arg_types,
+    T_PatternArgClass,
 )
-
-# from pepperbot.parse import (
-#     GROUP_EVENTS,
-#     GROUP_EVENTS_T,
-#     GroupEvent,
-#     is_valid_friend_method,
-#     is_valid_group_method,
-# )
-# from pepperbot.parse.bots import *
-# from pepperbot.parse.kwargs import (
-#     DEFAULT_KWARGS,
-#     HANDLER_KWARGS_MAP,
-#    EventHandlerKwarg,
-#     construct_GroupCommonBot,
-# )
 from pepperbot.store.meta import (
     ClassHandlerCache,
+    class_command_config_mapping,
+    class_command_mapping,
     class_handler_mapping,
     route_validator_mapping,
 )
+from pepperbot.types import COMMAND_CONFIG, BaseClassCommand
 from pepperbot.utils.common import get_own_methods
 
 """ 
 todo
 如果未注册对应的适配器，而且类响应器中定义了事件响应
 两种方法，忽略或者报错，可以设置
  """
 
 
-def cache_class_handler(class_handler: Callable, handler_name: str):
+def cache_class_handler(class_handler: object, handler_name: str):
+    """在parse中，已经验证过class_handler的合法性，这里不再重复验证"""
 
     #  不要每次都创建实例，on/register监听器新增时建立一次保存起来即可
-    class_handler_instance = class_handler()
+    class_handler_instance = class_handler()  # type: ignore
 
     # groupHandler可能有多个装饰器，比如register, withCommand
     # 先解析为与装饰器名称相关的缓存至groupMeta，
     # 解析完所有装饰器之后，再生成classHandlers.groupCache中的缓存
     # 生成缓存时，确保register的存在，不然报错(withCommand也可以向group中推送meta信息)
     # 这才是真正的meta，全局保存class和对应的meta，而不是绑定到class上，可能会涉及到bound和unbound的问题
 
     event_handlers: Dict[str, Callable] = {}
 
     # 初始化时，遍历生成缓存，不要每次接收到消息都去遍历
     for method in get_own_methods(class_handler_instance):
         method_name = method.__name__
-
-        # todo 多protocol合并的事件
-        # if not is_valid_group_method(method_name):
-        #     # if is_valid_friend_method(method.__name__):
-        #     raise EventHandlerDefineError(f"")
-
-        # if not is_valid_event_handler(class_handler, method, method_name):
-        #     raise EventHandlerDefineError(f"")
-
         event_handlers[method_name] = method
 
     class_handler_mapping[handler_name] = ClassHandlerCache(
         class_instance=class_handler_instance,
         event_handlers=event_handlers,
     )
     # 是否可以只实例化一次botInstance？动态注入groupId
     # 似乎每个群一个bot，效果更好一点
     # 为每一个group，缓存一个GroupCommonBot
     # botInstance=construct_GroupCommonBot({"group_id": id}, cast(Any, None)),
 
 
-def cache_class_command(class_command: Callable, command_name: str):
-    # 多个group handler，相同command的处理(解析所有指令和groupId，重新生成缓存)
-    # 同一个commandClass，就实例化一次
+def cache_class_command(class_command: BaseClassCommand, command_name: str):
+    """同一个commandClass，就实例化一次"""
 
-    # if lifecycle_name not in get_own_methods():
+    class_command_instance = class_command()  # type: ignore
 
-    class_command_instance = class_command()
     command_method_mapping = {}
 
     for method in get_own_methods(class_command_instance):
         method_name = method.__name__
 
-        patterns: List[Tuple[str, T_PatternArg]] = []
+        patterns: List[Tuple[str, T_PatternArgClass]] = []
         compressed_patterns = []
 
         if method_name not in LIFECYCLE_WITHOUT_PATTERNS:
+            # signature可以获取到被装饰器装饰过的函数的真实参数签名
             signature = inspect.signature(method)
 
             for arg_name, p in signature.parameters.items():
-
                 if p.default == "PatternArg":
                     annotation = p.annotation
-                    if annotation not in runtime_pattern_arg_types:
+                    if annotation not in PATTERN_ARG_TYPES:
                         raise InitializationError(f"仅支持str, bool, int, float和所有消息类型")
 
                     # 未具体指定类型(int, float, bool)的Text按照str处理
                     patterns.append(
                         (arg_name, annotation if annotation != Text else str)
                     )
 
-            # debug(patterns)
-
             compressed_patterns = merge_text_of_patterns(patterns)
+        # debug(patterns)
         # debug(compressed_patterns)
 
-        command_method_mapping[method_name] = CommandMethodCache(
+        command_method_mapping[method_name] = ClassCommandMethodCache(
             method=method,
             patterns=patterns,
             compressed_patterns=compressed_patterns,
         )
 
     class_command_mapping[command_name] = ClassCommandCache(
         class_instance=class_command_instance,
         command_method_mapping=command_method_mapping,
     )
 
-    command_config: CommandConfig = getattr(class_command, COMMAND_CONFIG)
-
-    class_command_config_mapping[command_name]["default"] = command_config
 
-    # debug(commandKwargs)
-
-    # command_methods = {}
-    # for method in get_own_methods(class_command_instance):
-    #     method_name = method.__name__
-
-    #     if not is_valid_command_method(method):
-    #         raise ClassCommandDifinationError()
-
-    #     commandBuffer.methods[method.__name__] = method
-
-    # if "initial" not in command_methods.keys():
-    #     raise ClassCommandDifinationError()
-
-    # commandBuffer = ClassCommandCache(
-    #     instance=class_command_instance,
-    #     kwargs=command_kwargs,
-    #     methods=command_methods,
-    # )
-
-    # classHandlers.commandCache[commandClass] = commandBuffer
-
-    # maxSize = commandKwargs["maxSize"]
-    # timeout = commandKwargs["timeout"]
-    # mode = commandKwargs["mode"]
-
-    # commandContext = CommandContext(
-    #     maxSize=maxSize or globalContext.maxSize,
-    #     timeout=timeout or globalContext.timeout,
-    #     mode=mode,
-    # )
-
-    # globalContext.cache[commandClass] = commandContext
-
-    # class_command_mapping
+def cache_class_command_config(command_name: str, command_config: CommandConfig):
+    # TODO 验证一下
+    # TODO 相关的文档，怎么避免意外创建多个command config
+    class_command_config_mapping[command_config.config_id] = ClassCommandConfigCache(
+        class_command_name=command_name,
+        command_config=command_config,
+    )
 
 
 def cache_route_validator(validator: Callable, validator_name: str):
     route_validator_mapping[validator_name] = validator
```

### Comparing `pepperbot-0.3.3/pepperbot/core/route/utils.py` & `pepperbot-0.3.4/pepperbot/core/route/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import json
 from typing import Any, Iterable
 
 from devtools import pformat
 from pepperbot.core.event.handle import handle_event
 from pepperbot.core.route.parse import parse_routes
 from pepperbot.exceptions import EventHandleError
@@ -36,33 +37,36 @@
 
 
 async def http_receiver(request, protocol: T_BotProtocol):
     try:
         raw_event = request.json
 
         logger.debug(pformat(raw_event))
-        await handle_event(protocol, raw_event)
+
+        asyncio.create_task(handle_event(protocol, raw_event))
 
     except EventHandleError as e:
         logger.exception(e)
 
     except Exception:
         logger.exception("事件处理异常")
 
     finally:
+        # 必须返回一个response
         return text("")
 
 
 async def websocket_receiver(request, ws, protocol: T_BotProtocol):
     while True:
         try:
             data = await ws.recv()
             raw_event = json.loads(data)
 
             logger.debug(pformat(raw_event))
-            await handle_event(protocol, raw_event)
+
+            asyncio.create_task(handle_event(protocol, raw_event))
 
         except EventHandleError as e:
             logger.exception(e)
 
         except Exception:
             logger.exception("事件处理异常")
```

### Comparing `pepperbot-0.3.3/pepperbot/core/route/validate.py` & `pepperbot-0.3.4/pepperbot/core/route/validate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,57 @@
 from ast import Call
 import ast
 import inspect
+import keyword
 import re
-from typing import Any, Callable, Dict, List, Sequence, Union, get_args, get_origin
+from typing import Any, Callable, Dict, List, Sequence, Set, Union, get_args, get_origin
 
 from devtools import debug
-from pepperbot.adapters.keaimao.event.kwargs import KEAIMAO_KWARGS_MAPPING
-from pepperbot.adapters.onebot.event.kwargs import ONEBOTV11_KWARGS_MAPPING
-from pepperbot.adapters.telegram.event.kwargs import TELEGRAM_KWARGS_MAPPING
-from pepperbot.core.event.kwargs import UNIVERSAL_KWARGS_MAPPING
-from pepperbot.core.event.universal import (
-    ALL_COMMON_EVENTS,
-    ALL_GROUP_EVENTS,
-    ALL_META_EVENTS,
-    ALL_PRIVATE_EVENTS,
-)
+from pepperbot.adapters.keaimao import KeaimaoAdapter
+from pepperbot.adapters.keaimao.event import KeaimaoEvent
+from pepperbot.adapters.onebot import OnebotV11Adapter
+from pepperbot.adapters.onebot.event import OnebotV11Event
+from pepperbot.adapters.telegram import TelegramAdapter
+from pepperbot.adapters.telegram.event import TelegramEvent
+from pepperbot.adapters.universal import UniversalAdapter
+from pepperbot.adapters.universal.event import UniversalEvent
+from pepperbot.core.event.universal import ALL_PROTOCOL_EVENT_NAMES
 from pepperbot.exceptions import InitializationError
 from pepperbot.extensions.command.handle import (
     COMMAND_DEFAULT_KWARGS,
-    LIFECYCLE_NO_PROGRAMMIC,
     LIFECYCLE_WITHOUT_PATTERNS,
-    common_kwargs,
+    COMMAND_COMMON_KWARGS,
 )
-from pepperbot.store.command import runtime_pattern_arg_types
-from pepperbot.store.meta import EventHandlerKwarg
+from pepperbot.store.command import PATTERN_ARG_TYPES
+from pepperbot.store.event import EventHandlerKwarg
+from pepperbot.types import COMMAND_CONFIG
 from pepperbot.utils.common import get_own_methods
 
 
 def is_valid_class_handler(class_handler: object):
     for method in get_own_methods(class_handler):
         method_name = method.__name__
 
-        is_handler_method_name_valid(method_name)
-        is_handler_method_args_valid(class_handler, method, method_name)
+        is_class_handler_method_name_valid(method_name)
+        is_class_handler_method_args_valid(class_handler, method, method_name)
 
     return True
 
 
-def is_handler_method_name_valid(method_name: str):
-    if not (
-        method_name in ALL_META_EVENTS
-        or method_name in ALL_COMMON_EVENTS
-        or method_name in ALL_GROUP_EVENTS
-        or method_name in ALL_PRIVATE_EVENTS
-    ):
-        raise InitializationError(f"无效的事件名 {method_name}")
+def is_class_handler_method_name_valid(method_name: str):
+    # if not (method_name in ALL_EVENTS):
+    #     raise InitializationError(f"无效的事件名 {method_name}")
 
+    # 允许非事件名的方法名
+    return True
 
-def gen_usable_kwargs_hint(method_name_kwargs_mapping: Dict, method_name: str):
-
-    kwarg_list: List[EventHandlerKwarg] = method_name_kwargs_mapping.get(
-        method_name, common_kwargs
-    )
 
+def gen_usable_kwargs_hint(keyword_arguments: Sequence[EventHandlerKwarg]):
     kwarg_name_type_mapping = {}
-    for kwarg in kwarg_list:
+    for kwarg in keyword_arguments:
         kwarg_name_type_mapping[kwarg.name] = kwarg.type_
 
     usable_kwargs_hint = "\n可用的参数及类型有\n"
     kwargs_count = len(kwarg_name_type_mapping)
 
     for index, (kwargName, kwargType) in enumerate(
         kwarg_name_type_mapping.items(), start=1
@@ -102,122 +95,134 @@
     if wrong_type_flag:
         raise InitializationError(
             common_prefix
             + f"的参数{parameter_name}的类型应该为{supposed_type}，而不是{parameter_type}"
         )
 
 
-def is_handler_method_args_valid(
+def is_class_handler_method_args_valid(
     class_handler: Any, method: Callable, method_name: str
 ):
+    if method_name not in ALL_PROTOCOL_EVENT_NAMES:
+        return
 
     if "onebot" in method_name:
-        mapping = ONEBOTV11_KWARGS_MAPPING
-        event_name = method_name.replace("onebot_", "")
+        keyword_arguments = OnebotV11Adapter.kwargs_mapping[method_name]
 
     elif "keaimao" in method_name:
-        mapping = KEAIMAO_KWARGS_MAPPING
-        event_name = method_name.replace("keaimao_", "")
+        keyword_arguments = KeaimaoAdapter.kwargs_mapping[method_name]
 
     elif "telegram" in method_name:
-        mapping = TELEGRAM_KWARGS_MAPPING
-        event_name = method_name.replace("telegram_", "")
+        keyword_arguments = TelegramAdapter.kwargs_mapping[method_name]
 
     else:
-        mapping = UNIVERSAL_KWARGS_MAPPING
-        event_name = method_name
+        keyword_arguments = UniversalAdapter.kwargs_mapping[method_name]
 
     kwarg_name_type_mapping, usable_kwargs_hint = gen_usable_kwargs_hint(
-        mapping, event_name
+        keyword_arguments
     )
     usable_kwarg_names = kwarg_name_type_mapping.keys()
 
     source_file_name = inspect.getsourcefile(class_handler)
     class_handler_name = class_handler.__name__
 
     common_prefix = (
         f"\n{source_file_name}文件中的类响应器{class_handler_name}的" + f"{method_name}事件"
     )
 
-    all_args, var_args, var_kwargs = inspect.getargs(method.__code__)
+    # all_args, var_args, var_kwargs = inspect.getargs(method.__code__)
 
-    if var_args or var_kwargs:
-        raise InitializationError(
-            common_prefix
-            + "不需要提供*或者**参数，PepperBot会自动根据声明的参数以及类型注入"
-            + usable_kwargs_hint
-        )
+    # if var_args or var_kwargs:
+    #     raise InitializationError(
+    #         common_prefix
+    #         + "不需要提供*或者**参数，PepperBot会自动根据声明的参数以及类型注入"
+    #         + usable_kwargs_hint
+    #     )
+
+    parameters = inspect.signature(method).parameters
 
-    for arg_name in all_args[1:]:  # 第一个是self
+    for arg_name in (list(parameters.keys()))[1:]:  # 第一个是self
         if arg_name not in usable_kwarg_names:
             raise InitializationError(
                 common_prefix + f"上不存在参数{arg_name}" + usable_kwargs_hint
             )
 
         if arg_name not in method.__annotations__.keys():
             raise InitializationError(
                 common_prefix
                 + f"的参数{arg_name}未提供类型注解，其类型为{kwarg_name_type_mapping[arg_name]}"
                 + usable_kwargs_hint
             )
 
     # 经过上两步验证，此时的参数，一定是有效的，而且有类型注解
     for arg_name, arg_type in method.__annotations__.items():
-
         supposed_arg_type = kwarg_name_type_mapping[arg_name]
 
         is_kwarg_annotation_correct(
             arg_name, arg_type, supposed_arg_type, common_prefix
         )
 
 
 def is_valid_class_command(class_command: Any):
+    assert hasattr(
+        class_command, COMMAND_CONFIG
+    ), f"需要通过as_command装饰器修饰{class_command.__class__.__name__}"
+
     source_file_name = inspect.getsourcefile(class_command)
     class_command_name = class_command.__name__
 
     common_prefix = f"\n{source_file_name} 文件中的指令 {class_command_name} 的"
 
     methods = list(get_own_methods(class_command))
     method_names = [method.__name__ for method in methods]
+    method_mapping = {method.__name__: method for method in methods}
 
     if not "initial" in method_names:
         raise InitializationError("指令必须定义initial方法作为入口")
 
     for method in methods:
         method_name = method.__name__
 
-        is_command_method_args_valid(method, method_name, common_prefix)
-        is_command_method_return_valid(method, method_name, method_names, common_prefix)
+        is_class_command_method_return_valid(
+            method, method_name, method_names, common_prefix
+        )
+
+    # 先通过上面的验证，此时的方法一定有返回值，并且只返回了一个值
+    involved_method_names = get_all_returned_identifiers(methods)
+
+    # 只验证被返回的方法，其他的方法不需要验证
+    for method_name in involved_method_names:
+        method = method_mapping[method_name]
+        is_class_command_method_args_valid(method, method_name, common_prefix)
 
     return True
 
 
-def is_command_method_args_valid(
+def is_class_command_method_args_valid(
     method: Callable, method_name: str, common_prefix: str
 ):
-
     common_prefix += f"{method_name}方法"
 
     signature = inspect.signature(method)
 
     for arg_name, p in signature.parameters.items():
-
         # self
         if arg_name == "self":
             continue
 
         # no *, **
         if p.kind == p.VAR_POSITIONAL or p.kind == p.VAR_KEYWORD:
             raise InitializationError(
                 common_prefix + "不需要提供*或者**参数，PepperBot会自动根据声明的参数以及类型注入"
             )
 
         ## has type hint
+        keyword_arguments = COMMAND_DEFAULT_KWARGS.get(method_name, COMMAND_COMMON_KWARGS)
         kwarg_name_type_mapping, usable_kwargs_hint = gen_usable_kwargs_hint(
-            COMMAND_DEFAULT_KWARGS, method_name
+            keyword_arguments
         )
 
         if p.annotation == p.empty:
             raise InitializationError(
                 common_prefix
                 + f"指令的方法 {method_name} 的参数 {arg_name} 未提供类型注解"
                 + usable_kwargs_hint
@@ -233,28 +238,28 @@
                 )
 
             # type hint correct
             if p.default != "PatternArg":
                 supposed_type = kwarg_name_type_mapping.get(arg_name)
                 if not supposed_type:
                     raise InitializationError(
-                        common_prefix + f"{arg_name} 无对应的类型，请确认该参数是否为有效参数"
+                        common_prefix + f"中不存在参数 {arg_name} ，请确认该参数是否为有效参数"
                     )
 
                 is_kwarg_annotation_correct(
                     arg_name, p.annotation, supposed_type, common_prefix
                 )
 
         # pattern args
         if p.default == "PatternArg":
             # no pattern in lifecycle hooks
             if method_name in LIFECYCLE_WITHOUT_PATTERNS:
                 raise InitializationError(common_prefix + f"这些生命周期不应支持pattern")
 
-            if p.annotation not in runtime_pattern_arg_types:
+            if p.annotation not in PATTERN_ARG_TYPES:
                 raise InitializationError(
                     common_prefix + f"仅支持str, bool, int, float和所有消息类型"
                 )
 
 
 def get_ids(elt):
     """Extract identifiers if present. If not return None"""
@@ -275,15 +280,29 @@
     {'ids': None,
      'lineno': 5,
      'statement': <_ast.Return object at 0x00000233AC6240D0>},
     {'ids': ['x', 'y'],
      'lineno': 7,
      'statement': <_ast.Return object at 0x00000233AC624100>}]
     """
-    (tree,) = ast.parse(inspect.getsource(f).lstrip()).body
+    function_source = inspect.getsource(f)
+    without_first_indent = function_source.lstrip()
+
+    # debug(function_source)
+
+    while without_first_indent.startswith("@"):
+        without_decorator = without_first_indent[without_first_indent.index("\n") :]
+        without_first_indent = without_decorator.lstrip()
+
+        # debug(without_decorator)
+        # debug(without_first_indent)
+
+    # 如果有装饰器，装饰器也会一并获取到，
+    # 要手动去掉，不然无法正常解析函数定义
+    (tree,) = ast.parse(without_first_indent).body
 
     return_statements: List = []
 
     for node in ast.walk(tree):
         if isinstance(node, (ast.Return,)):
             return_statements.append(
                 dict(
@@ -292,15 +311,30 @@
                     ids=get_ids(node.value),
                 )
             )
 
     return return_statements
 
 
-def is_command_method_return_valid(
+def get_all_returned_identifiers(f_list: list[Callable]):
+    identifiers: Set[str] = set()
+
+    for f in f_list:
+        return_statements = get_return_identifiers(f)
+
+        for info in return_statements:
+            ids = info["ids"]
+
+            if ids:  # 不为None，且len(ids) == 1
+                identifiers.update(ids)
+
+    return identifiers
+
+
+def is_class_command_method_return_valid(
     method: Callable, method_name: str, method_names: List[str], common_prefix: str
 ):
     """
     通过ast，保证方法返回值要么为None，要么是同一class的其它方法名
 
     同时不能是catch, timeout, exit，不应该由指令作者主动触发；initial和finish可以
 
@@ -317,21 +351,22 @@
         if len(ids) > 1:  # 不能返回多个值
             wrong = True
 
         identifier = ids[0]
         if identifier not in method_names:  # 要么返回下一步的方法名，要么不返回
             wrong = True
 
-        if identifier in LIFECYCLE_NO_PROGRAMMIC:
+        if identifier in LIFECYCLE_WITHOUT_PATTERNS:  # 不应该由指令作者主动触发
             wrong = True
 
         if wrong:
             raise InitializationError(
-                common_prefix + f"方法 {method_name} 的返回值可以为除catch, timeout, exit以外的生命周期，"
-                "即initial和finish，或者直接返回None(不返回)以结束会话"
+                common_prefix
+                + f"方法 {method_name} 的返回值只能是initial生命周期，或者用户自己定义的方法名，以继续会话；"
+                "直接返回None，或者不写返回语句，以结束会话"
             )
 
 
 def is_valid_route_validator(validator: Callable):
     """参数检查"""
 
     validator.__annotations__
```

### Comparing `pepperbot-0.3.3/pepperbot/exceptions.py` & `pepperbot-0.3.4/pepperbot/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,39 +21,35 @@
 
 class ClassCommandDefinitionError(PepperBotBaseException):
     """未按照commandClass规范定义命令类，导致的异常"""
 
     pass
 
 
-class PatternFormotError(PepperBotBaseException):
+class PatternFormatError(PepperBotBaseException):
     pass
 
 
 class PatternValidateError(PepperBotBaseException):
     pass
 
 
 class ClassCommandOnFinish(PepperBotBaseException):
-
     pass
 
 
 class ClassCommandOnExit(PepperBotBaseException):
-
     pass
 
 
 class ClassCommandOnTimeout(PepperBotBaseException):
-
     pass
 
 
 class EventHandlerDefineError(PepperBotBaseException):
-
     pass
 
 
 class InitializationError(PepperBotBaseException):
     pass
```

### Comparing `pepperbot-0.3.3/pepperbot/extensions/action/__init__.py` & `pepperbot-0.3.4/pepperbot/extensions/action/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/pepperbot/extensions/action/action.py` & `pepperbot-0.3.4/pepperbot/extensions/action/action.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/pepperbot/extensions/action/chain.py` & `pepperbot-0.3.4/pepperbot/extensions/action/chain.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/pepperbot/extensions/action/decorators.py` & `pepperbot-0.3.4/pepperbot/extensions/action/decorators.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/pepperbot/extensions/action/runner.py` & `pepperbot-0.3.4/pepperbot/extensions/action/runner.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/pepperbot/extensions/command/utils.py` & `pepperbot-0.3.4/pepperbot/extensions/command/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 import re
 import time
 from typing import Any, Callable, Dict, Iterable, List, Sequence, Set, Tuple
 
-from devtools import pformat
+from devtools import debug, pformat
+
 from pepperbot.core.message.chain import MessageChain
 from pepperbot.core.message.segment import At
+from pepperbot.extensions.log import debug_log, logger
 from pepperbot.store.command import CommandConfig
 from pepperbot.store.meta import get_bot_id
-from pepperbot.extensions.log import debug_log, logger
-
-
-from devtools import debug
 
 
 def meet_text_prefix(
     chain: MessageChain,
     command_name: str,
     command_config: CommandConfig,
 ) -> Tuple[bool, str, str, str]:
-
     aliases: Set[str] = set(command_config.aliases)
     if command_config.include_class_name:
         aliases.add(command_name)
     # aliases.add("")  # 保证下方循环至少执行一次
 
     if command_config.need_prefix:
         prefixes: Iterable[str] = set(command_config.prefixes)
     else:  # 保证下方循环至少执行一次
         prefixes = [""]
 
     debug_log(command_name, "指令名")
     debug_log(prefixes, "所有前缀")
     debug_log(aliases, "所有别名")
-
-    debug_log(chain.pure_text)
+    debug_log(chain.pure_text, "纯文本")
 
     for alias in aliases:
         for prefix in prefixes:
-            final_prefix = prefix + alias
+            prefix_with_alias = prefix + alias
 
             # 如果是At + Text的情况，pure_text之前会多出一个空格
             # 因为经常性，At和Text之间，会手动加一个空格，不如不去掉，就会导致判断失效
             # 必须有^，不然，当有多个指令时，某一个final_prefix是另一个final_prefix的子集时，会导致错误匹配
             # 比如，/a和/ab，当输入/a时，会匹配到/a和/ab，此时如果/a指令在前，/ab就不会被匹配到
-            if re.search(f"^{final_prefix}", chain.pure_text.strip()):
-                debug_log(f"^{final_prefix} 满足 {command_name} 的执行条件")
+            if not re.search(f"^{prefix_with_alias}", chain.pure_text.strip()):
+                debug_log(f"{prefix_with_alias} 不满足 {command_name} 的执行条件")
+                continue
 
-                return True, final_prefix, prefix, alias
+            debug_log(f"^{prefix_with_alias} 满足 {command_name} 的执行条件")
 
-            else:
-                debug_log(f"{final_prefix} 不满足 {command_name} 的执行条件")
+            return True, prefix_with_alias, prefix, alias
 
     return False, "", "", ""
 
 
 def meet_command_prefix(
     chain: MessageChain,
     command_name: str,
```

### Comparing `pepperbot-0.3.3/pepperbot/extensions/log/__init__.py` & `pepperbot-0.3.4/pepperbot/extensions/log/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import logging
 import os
 import sys
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from devtools.prettier import pformat
 from loguru import logger
 from pepperbot.config import global_config
 
 
 __all__ = (
@@ -55,21 +55,23 @@
     diagnose=True,
     # enqueue=True, # 需要阻塞式的日志输出
     format=formatter,  # type:ignore
 )
 logger = logger.opt(colors=True)
 
 
-def debug_log(message: Any, title: str = ""):
-    frame = inspect.stack()[1]
-    file_path = frame.filename
-    lineno = frame.lineno
+def debug_log(message: Optional[Any] = None, title: str = ""):
+    # 获取frame就很“昂贵”，所以只有在debug模式下才会获取
+    if global_config.logger.level <= 10:  # DEBUG
+        frame = inspect.stack()[1]
+        file_path = frame.filename
+        lineno = frame.lineno
 
-    logger.bind(title=title, file_path=file_path, lineno=lineno).debug("")
+        logger.bind(title=title, file_path=file_path, lineno=lineno).debug("")
 
-    if global_config.logger.level <= 10:  # DEBUG
-        print(pformat(message, highlight=True))
+        if message:
+            print(pformat(message, highlight=True))
 
 
 # TODO 整合sanic的日志
 # TODO 统一logging为loguru
 logging.getLogger("apscheduler").setLevel(global_config.logger.level)
```

### Comparing `pepperbot-0.3.3/pepperbot/initial.py` & `pepperbot-0.3.4/pepperbot/initial.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,36 +2,38 @@
 
 from apscheduler.triggers.interval import IntervalTrigger
 from devtools import debug, pformat
 from sanic import Sanic
 
 from pepperbot.adapters.telegram import register_telegram_event
 from pepperbot.config import global_config
-from pepperbot.core.bot.api_caller import ApiCaller
+from pepperbot.core.api.api_caller import ApiCaller
 from pepperbot.core.route.utils import (
     create_bot_routes,
     create_web_routes,
     http_receiver,
     websocket_receiver,
 )
 from pepperbot.exceptions import InitializationError
 from pepperbot.extensions.command.handle import check_command_timeout
-from pepperbot.extensions.log import logger
+from pepperbot.extensions.log import debug_log, logger
 from pepperbot.extensions.scheduler import async_scheduler
+from pepperbot.store.orm import engine, metadata, set_metadata
 from pepperbot.store.meta import (
-    ALL_AVAILABLE_BOT_PROTOCOLS,
     DEFAULT_URI,
     BotRoute,
-    api_callers,
     clean_bot_instances,
     output_config,
+    api_callers,
     register_routes,
-    route_mapping,
 )
-from pepperbot.types import T_BotProtocol, T_WebProtocol
+from pepperbot.types import BOT_PROTOCOLS, T_BotProtocol, T_WebProtocol
+
+# from dotenv import load_dotenv
+# import os
 
 sanic_app = Sanic("PepperBot")
 
 async_create_telegram_handler: Optional[Callable] = None
 
 
 async def _ensure_async_scheduler_start():
@@ -51,33 +53,37 @@
 
         sanic_app.config.INSPECTOR = debug
         sanic_app.config.WEBSOCKET_PING_TIMEOUT = None  # type:ignore
 
         sanic_app.register_listener(self.main_process_start, "main_process_start")
         sanic_app.register_listener(self.after_server_start, "after_server_start")
 
+        # load_dotenv()  # take environment variables from .env.
+        # debug_log(os.environ)
+
     def register_adapter(
         self,
         bot_protocol: Literal["onebot", "keaimao"],
         receive_protocol: T_WebProtocol,
         backend_protocol: T_WebProtocol,
         backend_port: int,
         backend_host="127.0.0.1",
         receive_uri: str = "",
     ):
         uri: str
         request_handler: Optional[Callable] = None
 
-        if bot_protocol not in ALL_AVAILABLE_BOT_PROTOCOLS:
+        if bot_protocol not in BOT_PROTOCOLS:
             raise InitializationError(f"尚不支持的机器人协议 {bot_protocol}")
 
         if receive_uri:
             uri = receive_uri
         else:
             if receive_protocol == "http":
+                # TODO lambda重名问题，动态创建
                 request_handler = lambda request: http_receiver(request, bot_protocol)
                 uri = DEFAULT_URI[bot_protocol] + "/http"
 
             elif receive_protocol == "websocket":
                 request_handler = lambda request, ws: websocket_receiver(
                     request, ws, bot_protocol
                 )
@@ -107,19 +113,23 @@
         else:
             raise InitializationError(f"未知通信协议 {backend_protocol}")
 
         api_callers[bot_protocol] = api_caller
 
     def register_telegram(self, *args, **kwargs):
         # sanic启动至少需要一个route，虽然这个route并不会被调用
+        # sanic不允许重名的handler，lambda表达式会导致重名(都为lambda)
+        async def telegram_handler(request):
+            return 1
+
         create_web_routes(
             sanic_app,
             receive_protocol="http",
             uri="/telegram/http",
-            request_handler=lambda request: 1,
+            request_handler=telegram_handler,
         )
 
         async def create_client_under_async_context():
             """
             pyrogram client require to be created under same async context
             for the reason that it interacts with sqlite
 
@@ -135,15 +145,15 @@
             logger.success("PepperBot successfully create pyrogram client")
 
             await pyrogram_client.start()
 
         global async_create_telegram_handler
         async_create_telegram_handler = create_client_under_async_context
 
-    def register_plugin(self):
+    def register_plugin(self) -> None:
         pass
 
     def apply_routes(self, routes: Iterable[BotRoute]):
         create_bot_routes([*routes, *register_routes])
 
     def share_state_command(self):
         pass
@@ -152,28 +162,49 @@
     async def main_process_start(app, loop):
         """
         https://sanic.dev/en/guide/basics/listeners.html#asgi-mode
 
         If you are running your application with an ASGI server, main_process_start and main_process_stop will be ignored
         """
 
+        # TODO 主动获取bot info
+        await set_metadata("has_initial_bot_info", False)
+
+        # TODO 在各adapter初始化完成之后，再获取
+        # 所以需要实现一个hook，after_adapter_init
+
+        # main process、worker process都需要读取.env
+        # 主动读取一次，这样即使用户定义的BaseSetting中没有制定env_file，也能读取到
+        # load_dotenv()  # take environment variables from .env.
         logger.success(
             f"PepperBot successfully load .env config \n {pformat(global_config)}"
         )
 
         logger.success(f"PepperBot successfully create bot routes")
-        output_config()
+        # output_config()
+        # debug(per_worker)
+
+        # 必须放到最后，等model都定义好了再执行
+        # note that this has to be the same metadata that is used in ormar Models definition
+        metadata.create_all(engine)
+        # 保证过期(无效)的command status一定被清理，不会干扰has_running_command的判断
+        await check_command_timeout()
 
     @staticmethod
     async def after_server_start(app, loop):
         # ensure that async_scheduler is created under same async context
         # https://github.com/sanic-org/sanic/issues/743
         # global async_scheduler
         # async_scheduler = AsyncIOScheduler({'event_loop': loop})
 
+        # 正常情况下，主进程设置一次就行了
+        # 但是如果自动重启，那么就需要在每次重启后都设置一次
+        if app.config["AUTO_RELOAD"]:
+            await set_metadata("has_initial_bot_info", False)
+
         if async_create_telegram_handler:
             async_scheduler.add_job(async_create_telegram_handler)
 
         async_scheduler.add_job(check_command_timeout, IntervalTrigger(seconds=10))
         # async_scheduler.add_job(clean_bot_instances)
         async_scheduler.add_job(_ensure_async_scheduler_start)
```

### Comparing `pepperbot-0.3.3/pepperbot/store/command.py` & `pepperbot-0.3.4/pepperbot/store/command.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,244 +1,211 @@
 from __future__ import annotations
+from collections import deque
+import pickle
 
 import time
-from collections import defaultdict, deque
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
-    Deque,
     Dict,
-    ForwardRef,
+    Generic,
     List,
     Literal,
+    Optional,
     Sequence,
-    Set,
     Tuple,
     Type,
+    TypeVar,
     Union,
+    cast,
 )
+from uuid import uuid4
 
-from devtools import debug
+import ormar
+from pydantic import BaseModel, Field
+from typing_extensions import get_args
 
 # if TYPE_CHECKING:
+# field "chain" not yet prepared so type is still a ForwardRef, you might need to call HistoryItem.update_forward_refs().
+# pydantic需要用到
 from pepperbot.core.message.chain import MessageChain
-
-from pepperbot.core.message.segment import T_SegmentClass, T_SegmentInstance
-from pepperbot.types import (
-    BaseClassCommand,
-    T_BotProtocol,
-    T_RouteMode,
-    T_RouteRelation,
+from pepperbot.core.message.segment import (
+    GT_PatternArg,
+    Image,
+    T_SegmentClass,
+    T_SegmentInstance,
 )
-from pydantic import BaseModel, Field
-from typing_extensions import TypedDict, get_args
-
-
-class CommandConfig(BaseModel):
-    need_prefix: bool = False
-    prefixes: Sequence[str] = ["/"]
-    """ 都是正则，自动加上^ """
-    aliases: Sequence[str] = Field(default_factory=list)
-    """ 指令前缀别名 ，都是正则 """
-    include_class_name: bool = True
-    """ 类名本身是否作为指令前缀 """
-    exit_patterns: Sequence[str] = ["^/exit", "^退出"]
-    """ 都是正则，满足条件， """
-    require_at: bool = False
-    """ 是否需要@机器人 """
-    timeout: int = 30
-    """ 会话超时时间，单位秒, """
-    history_size: int = 1
-    """ 
-    保留上一次的raw_event，可以在timeout中复用
-    不然timeout中并没有办法获取到raw_event，因为timeout实在apscheduler中独立调用的 
-    """
-    # lock_user = False
-    # """ 跨消息渠道锁定用户
-    # 不管他是私聊、还是群聊、还是频道，只要是一条规则指定的用户，他们的发言都会被指令接受
-    # """
-    # user_mapping: List[Dict[T_BotProtocol, str]] = Field(default_factory=list)
-    # """
-    # 用户自己负责，是否有重复指定的情况
-    # 如果重复指定了两次，那么就会执行两次
-    # [
-    #     {
-    #         "onebot" : "123455",
-    #         "keaimao" : "wxid_askjhfljdsaf",
-    #     },
-    #     {
-    #         "onebot" : "7890784",
-    #         "keaimao" : "wxid_xnvkjdhf",
-    #     },
-    # ]
-    # """
-    # lock_source = False
-    # """
-    # 指定消息来源，该消息来源(群、频道)内，所有用户的发言都被指令接受
-    # 不要和lock_user同时使用，二选一
-    # 也就是说，normal, lock_user, lock_source是三选一的关系
-    # """
-    # source_mapping: List[Dict[T_BotProtocol, List[str]]] = Field(default_factory=list)
-    # """
-    # [
-    #     {
-    #         "onebot" : ["123455", "2034789"],
-    #         "keaimao" : ["123789@chatroom",],
-    #     },
-    # ]
-    # """
+from pepperbot.store.orm import database, metadata
+from pepperbot.types import T_BotProtocol
 
+TRUE_TEXTS = ("True", "true", "1")
+FALSE_TEXTS = ("False", "false", "0")
 
 VALID_TEXT_TYPES = (str, int, float, bool)
 T_ValidTextTypeInstance = Union[str, int, float, bool]
-T_ValidTextType = Union[Type[str], Type[int], Type[float], Type[bool]]
+T_ValidTextTypeClass = Union[Type[str], Type[int], Type[float], Type[bool]]
 
-T_PatternArg = Union[T_ValidTextType, T_SegmentClass]
-T_PatternArgResult = Union[str, int, float, bool, T_SegmentInstance]
-
-
-TRUE_TEXTS = ("True", "true", "1")
-FALSE_TEXTS = ("False", "false", "0")
+T_PatternArgInstance = Union[T_ValidTextTypeInstance, T_SegmentInstance]
+T_PatternArgClass = Union[T_ValidTextTypeClass, T_SegmentClass]
 
 
 def get_runtime_pattern_arg_types():
-    runtime_generic_types = []
-    for type_ in get_args(T_PatternArg):
+    """获取运行时的T_PatternArg的类型，基础类型 + 所有Segment类型"""
 
+    runtime_generic_types = []
+    for type_ in get_args(GT_PatternArg):
         if type_ is Union:  # T_SegmentClass
             runtime_generic_types.extend(get_args(type_))
 
         else:  # str, bool, int, float
             runtime_generic_types.append(type_)
 
     # debug(runtime_generic_types)
     runtime_class_types = tuple(
         map(lambda generic: get_args(generic)[0], runtime_generic_types)
     )
     # debug(runtime_class_types)
     return runtime_class_types
 
 
-runtime_pattern_arg_types = get_runtime_pattern_arg_types()
+PATTERN_ARG_TYPES = get_runtime_pattern_arg_types()
+""" 运行时的GT_PatternArg的类型，基础类型 + 所有Segment类型 """
+
+
+# TODO 带默认值的pattern
+def PatternArg(default: Optional[GT_PatternArg] = None) -> GT_PatternArg:
+    return cast(GT_PatternArg, "PatternArg")
+    # return cast(GT_PatternArg, default)
+
 
-# class PatternArg:
-#     # pass
-#     # __slots__ = ("type_",)
+# a: Image = PatternArg()
 
-#     def __init__(self):
-#         # self.type_ = type_
 
-#         return 123
+# class PatternArg(Generic[GT_PatternArg]):
+#     """ """
 
+#     __slots__ = (
+#         "type_",
+#         "default",
+#     )
 
-def PatternArg() -> Any:
-    return "PatternArg"
+#     def __init__(
+#         self, type_: Type[GT_PatternArg], default: Optional[GT_PatternArg] = None
+#     ):
+#         self.type_ = type_
+#         self.default = default
+
+
+# a = PatternArg(Image, Image(""))
+
+
+def uuid_str() -> str:
+    return str(uuid4())
+
+
+T_InteractiveStrategy = Literal[
+    "same_source_same_user",
+    "same_source_any_user",
+    "any_source_same_user",
+    "any_source_any_user",
+]
+
+
+class CommandConfig(BaseModel):
+    """pydantic可以自动处理动态默认值的问题
+
+    动态默认值问题是指，如果默认值是[]、{}，则会被复用，导致多个指令共享同一个默认值对象(因为是同一个对象)
+    也就是说，修改会在多个指令间同步
+    """
+
+    config_id: str = Field(default_factory=uuid_str)
+
+    need_prefix: bool = False
+    prefixes: Sequence[str] = ["/"]
+    aliases: Sequence[str] = Field(default_factory=list)
+    include_class_name: bool = True
+    exit_patterns: Sequence[str] = ["^/exit", "^退出"]
+    require_at: bool = False
+    timeout: int = 60
+    history_size: int = 1
+    interactive_strategy: T_InteractiveStrategy = "any_source_same_user"
+    config: Any = None
+    concurrency: bool = True
+    priority: int = 0
+    propagation_group: str = "default"
 
 
 T_CompressedPatterns = List[
-    Union[List[Tuple[str, T_PatternArg]], Tuple[str, T_PatternArg]]
+    Union[List[Tuple[str, GT_PatternArg]], Tuple[str, GT_PatternArg]]
 ]
 
 
-class CommandMethodCache(BaseModel):
+class ClassCommandMethodCache(BaseModel):
+    class Config:
+        arbitrary_types_allowed = True
+
     method: Callable
-    patterns: List[Tuple[str, T_PatternArg]]
+    patterns: List[Tuple[str, T_PatternArgInstance]]
     compressed_patterns: T_CompressedPatterns
     """ cache时缓存便于正则的格式化的pattern，不用每次收到消息都解析 """
 
 
-# CommandMethodCache.update_forward_refs()
-
-
 class ClassCommandCache(BaseModel):
     class Config:
         arbitrary_types_allowed = True
 
     class_instance: Any
-    command_method_mapping: Dict[str, CommandMethodCache] = {}
+    command_method_mapping: Dict[str, ClassCommandMethodCache] = {}
     """ key为方法名，value为实例化后的方法 """
-    # command_config: Dict[str, Any]
-    # lock_user_context_ids: Set[str] = set()
-    """ 
-    允许在BotRoute中，对同一个command设置多个不同的kwargs组合
-    [id1, id2, id3]
-
-    for id in ids:
-        if meet_lock_user_rule()
-    """
-    # lock_source_context_ids
 
 
-class_command_mapping: Dict[str, ClassCommandCache] = {}
-""" ClassCommand.__name__ : ClassHandlerCache """
-
-
-class_command_config_mapping: Dict[str, Dict[str, CommandConfig]] = defaultdict(dict)
-""" 一个command可能有多个config，share_state_command时，复用class_command_cache，
-解耦class_instance和config，不然要重复创建多次
-default是给BotRoute中注册的command用的
-{
-    [command_name] : {
-        "default" : CommandConfig,
-        "id1" : CommandConfig,
-        "id2" : CommandConfig,
-    }
-}
- """
+class ClassCommandConfigCache(BaseModel):
+    class Config:
+        arbitrary_types_allowed = True
 
-COMMAND_CONFIG = "__command_config__"
+    class_command_name: str
+    command_config: CommandConfig
 
 
 class HistoryItem(BaseModel):
     class Config:
         arbitrary_types_allowed = True
 
     raw_event: Dict
     chain: MessageChain
 
 
 # MessageChain = ForwardRef('MessageChain')
 # MessageChain.update_forward_refs()
 
 
-class ClassCommandStatus(BaseModel):
-    """也可以理解为一个session"""
+class ClassCommandStatus(ormar.Model):
+    """保存指令状态，跨进程"""
 
-    pointer: str = "initial"
-    history: Deque[HistoryItem]
-    last_updated_time: float = Field(default_factory=time.time)
-    """ 用来判断timeout """
-    timeout: int
-    context: Dict = Field(default_factory=dict)
-    """ 用户定义，method之间的消息传递方式 """
-
-
-T_CommandStatusKey = Tuple[str, T_BotProtocol, T_RouteMode, str]
-
-normal_command_context_mapping: Dict[T_CommandStatusKey, ClassCommandStatus] = {}
-""" 
-默认情况，不锁定用户，也不锁定消息来源
-{
-    (command_name, protocol, mode, source_id) : status
-}
-"""
-
-
-# class LockRelation(TypedDict):
-#     rule: Dict[T_BotProtocol, List[str]]
-#     context: ClassCommandContext
-
-
-# lock_user_context_mapping: Dict[str, LockRelation] = {}
-"""
-锁定用户
-lock_user_mapping中的每一条规则，都应该有一个单独的context
-
-{
-    id : {
-        rule : {},
-        context : context
-    }
-}
+    class Meta:
+        tablename = "class_command_status"
+        database = database
+        metadata = metadata
+
+    id: int = cast(int, ormar.Integer(primary_key=True))
+
+    command_name = cast(str, ormar.String(max_length=50))
+    config_id: str = cast(str, ormar.String(max_length=50))
+    protocol: T_BotProtocol = cast(T_BotProtocol, ormar.String(max_length=50))
+    conversation_type: str = cast(str, ormar.String(max_length=50))
+    conversation_id: str = cast(str, ormar.String(max_length=50))
+    user_id: str = cast(str, ormar.String(max_length=50))
+
+    pointer: str = cast(str, ormar.String(max_length=50, default="initial"))
+    running: bool = ormar.Boolean(default=False)
+
+    # 通过pickle序列化后的数据
+    history: bytes = ormar.LargeBinary(
+        max_length=100000, default=pickle.dumps(deque(maxlen=1))
+    )
+    context: bytes = ormar.LargeBinary(max_length=100000, default=pickle.dumps({}))
 
-"""
+    """ 用户定义，method之间的消息传递方式 """
+    last_updated_time: float = cast(float, ormar.Float(default=time.time))
+    """ 用来判断timeout """
+    timeout: int = cast(int, ormar.Integer())
```

### Comparing `pepperbot-0.3.3/pepperbot/store/meta.py` & `pepperbot-0.3.4/pepperbot/store/meta.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,108 @@
 from collections import defaultdict
 from typing import (
     Any,
+    Awaitable,
     Callable,
     Dict,
     Iterable,
     List,
     Literal,
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
-    TypedDict,
     Union,
     cast,
 )
+from uuid import UUID
 
-from pepperbot.core.bot.api_caller import ApiCaller
+from pepperbot.core.api.api_caller import ApiCaller
 from pepperbot.exceptions import InitializationError
+from pepperbot.store.command import (
+    ClassCommandCache,
+    ClassCommandConfigCache,
+    CommandConfig,
+)
+from pepperbot.store.event import ProtocolEvent
 from pepperbot.types import (
+    BOT_PROTOCOLS,
+    CONVERSATION_TYPES,
     BaseBot,
     BaseClassCommand,
     T_BotProtocol,
-    T_RouteMode,
+    T_ConversationType,
+    T_HandlerType,
     T_RouteRelation,
     T_RouteValidator,
     T_WebProtocol,
 )
 from pepperbot.utils.common import deepawait_or_sync, fit_kwargs
 from pydantic import BaseModel, Field
 from pyrogram.client import Client
 from rich import print as rich_print
 from rich.tree import Tree
 from typing_extensions import Annotated, NotRequired
 
+from inspect import isclass
+
+
+import sys
+
+if sys.version_info < (3, 11):
+    from typing_extensions import TypedDict
+else:
+    from typing import TypedDict
+
 
 class BotRoute(BaseModel):
     class Config:
         arbitrary_types_allowed = True
 
     handlers: Optional[Iterable[object]] = None
     commands: Optional[Iterable[BaseClassCommand]] = None
-    groups: Optional[T_RouteRelation] = "*"
-    friends: Optional[T_RouteRelation] = "*"
+    groups: Optional[T_RouteRelation] = None  # 默认不应该匹配所有
+    friends: Optional[T_RouteRelation] = None
+
+
+def register(
+    *,
+    handlers: Optional[Iterable[object]] = None,
+    commands: Optional[Iterable[BaseClassCommand]] = None,
+    # 这个可以匹配所有，因为仅建议仅有单个handler时使用，用户一般也不会做太复杂的权限控制
+    groups: Optional[T_RouteRelation] = None,
+    friends: Optional[T_RouteRelation] = None,
+    # **kwargs, # 不允许用户传入其他参数
+):
+    """装饰器风格，实现注册handler和command"""
+
+    def decorator(handler: Callable):
+        if not isclass(handler):
+            raise InitializationError(
+                "register装饰器只能注册class handler，不能注册function handler"
+            )
+
+        # 收集register中的BotRoute，apply_routes中应用
+        register_routes.append(
+            # 通过BotRoute，实现参数的类型检查
+            BotRoute(
+                handlers=handlers,
+                commands=commands,
+                groups=groups,
+                friends=friends,
+            )
+        )
+
+        return handler
+
+    return decorator
+
+
+T_AvailableChecker = Callable[..., Union[bool, Awaitable[bool]]]
 
 
 class ClassHandlerCache(BaseModel):
     class Config:
         arbitrary_types_allowed = True
 
     class_instance: Any
@@ -58,219 +114,178 @@
     {
         "group_message" : bounded_handler,
         "add_group" : bounded_handler,
     }
     """
 
 
-class RouteValidatorCache(BaseModel):
-    class Config:
-        arbitrary_types_allowed = True
+class ApiCallerTypeMap(TypedDict):
+    onebot: NotRequired[ApiCaller]
+    keaimao: NotRequired[ApiCaller]
+    telegram: NotRequired[Client]
+
 
+class BotInfo(BaseModel):
+    """保存每个协议的bot的自身信息
+    id
+    是否是管理员之类
+    """
 
-class RouteMapping(BaseModel):
     class Config:
         arbitrary_types_allowed = True
 
-    global_commands: Dict[T_BotProtocol, Dict[T_RouteMode, Set[str]]] = defaultdict(
-        lambda: defaultdict(set)
-    )
-    """ 
-    对所有群应用的指令，当groups="*"时注册至此
-    对所有私聊消息应用的指令，当friends="*"时注册至此
-    {
-        "onebot" : {
-            "group" : [command1, command2, ],
-            "friend" : []
-            "channel" : []
-        }
-    }
-    """
+    id: int
+    is_admin: bool
+
+
+"""每个worker进程都需要独立进行的初始化工作"""
+
 
-    global_handlers: Dict[T_BotProtocol, Dict[T_RouteMode, Set[str]]] = defaultdict(
-        lambda: defaultdict(set)
+register_routes: List[BotRoute] = []
+""" 通过register装饰器注册的class_handler """
+
+route_mapping: Dict[
+    tuple[
+        Union[T_BotProtocol, Literal["validator"]],
+        T_ConversationType,
+        str,
+        T_HandlerType,
+    ],
+    Set[str],
+] = defaultdict(set)
+""" 路由映射
+
+一个class_handler可能对应多个群，所以只保存class_handler的名字，而不是实例化的对象
+用的时候，通过名字，从class_handler_mapping中获取实例化的对象
+
+统一保存为str，这样不用判断是int还是str了
+
+qq号可能和群号重复，通过conversation_type区分
+
+这里是protocol-group，而不是group-protocol，是因为
+每次接收到消息，protocol是固定的，而group、private不固定
+这样的顺序符合逻辑
+
+{
+    ( "onebot", "group", "123456789", "class_handlers" ) : [ "class_handler_name" ],
+    ( "onebot", "group", "123456789", "class_commands" ) : [ "class_command_name" ],
+    ( "onebot", "private", "123456789", "class_handlers" ) : [ "class_handler_name" ],
+    ( "onebot", "private", "123456789", "class_commands" ) : [ "class_command_name" ],
+    ( "validator", "group", "__unset__", "class_handlers" ) : [ "class_handler_name" ],
+    ( "validator", "group", "__unset__", "class_commands" ) : [ "class_command_name" ],
+}
+
+"""
+
+# 下方都为缓存
+class_handler_mapping: Dict[str, ClassHandlerCache] = {}
+""" ClassHandler.__name__ : ClassHandlerCache """
+
+route_validator_mapping: Dict[str, T_RouteValidator] = {}
+""" ValidatorFunction.__name__ : route_validator """
+
+class_command_mapping: Dict[str, ClassCommandCache] = {}
+""" ClassCommand.__name__ : ClassHandlerCache """
+
+class_command_config_mapping: Dict[str, ClassCommandConfigCache] = {}
+""" 一个command可能有多个config，解耦class_instance和config，复用class_command_cache，不然要重复创建多次
+
+之所以是config_id作为key，是因为在route_mapping中，直接保存的是config_id
+{
+    [command_config_id] : ClassCommandConfigCache(
+        class_command_name = "class_command_name",
+        command_config = CommandConfig,
     )
-    """ 对所有群应用的消息响应器，当groups="*"或者friends="*"时注册至此 
-    {
-        "onebot" : {
-            "group" : [handler1, handler2, ],
-            "friend" : []
-            "channel" : []
-        }
-    }
-    """
-    mapping: Dict[
-        Union[T_BotProtocol, Literal["validators"]],
-        Dict[
-            T_RouteMode,
-            Dict[
-                str,
-                Dict[Literal["class_handlers", "commands"], Set[str]],
-            ],
-        ],
-    ] = defaultdict(lambda: defaultdict(lambda: defaultdict(lambda: defaultdict(set))))
-    """ 
-    一个群消息响应器可能对应多个群，所以只保存索引
-    同意保存为str，这样不用判断是int还是str了
-    qq号可能和群号重复，再套一级字典
-    这里是protocol-group，而不是group-protocol，是因为
-    每次接收到消息，protocol是固定的，而group、private不固定
-    这样的顺序符合逻辑
-
-    mapping可以不需要group private，减少一级嵌套，通过添加标识符，比如private123，
-    减少一级嵌套，不意味不区分GroupBot和PrivateBot
-    protocol还是要区分的
-    之所以现在有group、private，是因为认为群号和qq号可能重复，事实上可以通过标识符避免
-    比如g_123 == group 123, p_123 == private 123, c_123 == channel 123
-    "group" : {
-        123 : {
+}
+"""
 
-        }
-    }
-    还是
-    "g_123" :{
+CLASS_CHECKERS = "__class_checkers__"
 
-    }
-    其实真差不多，多一级的话，还有类型提示
+checkers_cache: Dict[Tuple[str, str], Set[T_AvailableChecker]] = defaultdict(set)
+""" 应用available时，无法判断是否是command，所以不放在对应的cache里，单独建一个 
+{
+    ("class.__name__", CLASS_CHECKERS) : set(checker),
+    ("class.__name__", "method.__name__") : set(checker),
+}
+ """
 
-    {
-        "onebot":{
-            "group" : {
-                12345 : { 
-                    class_handlers : [ClassHandlerCacheName],
-                    commands : [CommandClassName],
-                },
-            },
-            "private" : {
-                "67890" : { 
-                    class_handlers : [ClassHandlerCacheName],
-                    commands : [CommandClassName],
-                }
-            }
-        },
-        "validators" : {
-            "group" : {
-                [validator_name] : {
-                    class_handlers : [],
-                    commands : [],
-                },
-            }
-        }
-    }
-    """
+api_callers: ApiCallerTypeMap = {}
 
-    bot_instances: Dict[
-        Tuple[Union[T_BotProtocol, Literal["universal"]], T_RouteMode, str],
-        BaseBot,
-    ] = Field(default_factory=dict)
-    """ 为每一个消息来源构造一个bot实例的开销是完全可以接受的(即使有三四千个) 
-    {
-        ("universal", "group", identifier) : bot,
-        ("onebot", "private", identifier) : bot,
-    }
-    """
+bot_info: Dict[T_BotProtocol, Dict] = defaultdict(dict)
+""" 保存每个协议的bot的自身信息
+id
+是否是管理员之类
+"""
 
-    bot_info: Dict[T_BotProtocol, Dict] = defaultdict(dict)
-    """ 保存每个协议的bot的自身信息
-    id
-    是否是管理员之类
-    """
 
-    has_initial = False
+bot_instances: Dict[
+    Tuple[Union[T_BotProtocol, Literal["universal"]], T_ConversationType, str],
+    BaseBot,
+] = {}
+""" 为每一个消息来源构造一个bot实例的开销是完全可以接受的(即使有三四千个) 
+{
+    ("universal", "group", identifier) : bot,
+    ("onebot", "private", identifier) : bot,
+}
+"""
 
 
 class OnebotEventMeta(BaseModel):
     has_skip_buffered_event = False
     buffered_message_count = 0
 
 
 onebot_event_meta = OnebotEventMeta()
 
 
+LAST_ONEBOT_HEARTBEAT_TIME = "last_onebot_heartbeat_time"
+
+
 def get_bot_id(protocol: T_BotProtocol):
-    return str(route_mapping.bot_info[protocol]["bot_id"])
+    return str(bot_info[protocol]["bot_id"])
 
 
 async def initial_bot_info():
+    """数据会保存至数据库，所以所有worker中，只需要执行一次"""
+
     for protocol in api_callers:
         if protocol == "onebot":
-            if not route_mapping.bot_info.get("onebot"):
-                from pepperbot.adapters.onebot.api import OnebotV11Api
+            if not bot_info.get("onebot"):
+                from pepperbot.adapters.onebot.api import OnebotV11API
 
-                bot_id = (await OnebotV11Api.get_login_info())["user_id"]
-                route_mapping.bot_info["onebot"]["bot_id"] = bot_id
+                bot_id = (await OnebotV11API.get_login_info())["user_id"]
+                bot_info["onebot"]["bot_id"] = str(bot_id)
 
         elif protocol == "keaimao":
-            if not route_mapping.bot_info.get("keaimao"):
-                from pepperbot.adapters.keaimao.api import KeaimaoApi
+            if not bot_info.get("keaimao"):
+                from pepperbot.adapters.keaimao.api import KeaimaoAPI
 
-                bot_id = (await KeaimaoApi.get_login_accounts())[0]["wxid"]
-                route_mapping.bot_info["keaimao"]["bot_id"] = bot_id
+                accounts = cast(List, await KeaimaoAPI.get_login_accounts())
+                bot_id = accounts[0]["wxid"]
+                bot_info["keaimao"]["bot_id"] = bot_id
 
         elif protocol == "telegram":
-            if not route_mapping.bot_info.get("telegram"):
+            if not bot_info.get("telegram"):
                 # from pepperbot.adapters.telegram.api import TelegramApi
                 client = get_telegram_caller()
 
                 me = await client.get_me()
                 bot_id = str(me.id)
-                route_mapping.bot_info["telegram"]["bot_id"] = bot_id
+                bot_info["telegram"]["bot_id"] = bot_id
 
         else:
-            raise InitializationError()
+            raise InitializationError(f"未知的协议: {protocol}")
 
 
 def clean_bot_instances():
     """每24小时清理一次，释放内存"""
-    route_mapping.bot_instances.clear()
-
-
-class LifecycleHandler(BaseModel):
-    """函数形式的生命周期响应器"""
-
-    pass
-
-
-lifecycle_handlers = defaultdict(list)
-
-
-class_handler_mapping: Dict[str, ClassHandlerCache] = {}
-""" ClassHandler.__name__ : ClassHandlerCache """
-
-route_validator_mapping: Dict[str, T_RouteValidator] = {}
-
-route_mapping = RouteMapping()
-
-
-class ApiCallerTypeMap(TypedDict):
-    onebot: NotRequired[ApiCaller]
-    keaimao: NotRequired[ApiCaller]
-    telegram: NotRequired[Client]
+    bot_instances.clear()
 
 
 # api_callers: Dict[T_BotProtocol, ApiCaller] = {}
-api_callers: ApiCallerTypeMap = {}
-
-register_routes: List[BotRoute] = []
-""" 通过register装饰器注册的class_handler """
-
-
-class BotMetaState(BaseModel):
-    router = {}
-    class_handlers = {}
-    function_handlers = {}
-    commands = {}
-
-
-bot_meta_state = BotMetaState()
-
-
-def cache_command_class(command_class: object):
-    if command_class not in bot_meta_state.commands:
-        bot_meta_state.commands[command_class.__class__] = command_class
 
 
 def get_api_caller(protocol: T_BotProtocol):
     api_caller = api_callers.get(protocol)
 
     assert api_caller, f"无法获取 {protocol} 对应的api_caller，请确保你注册了对应的adapter"
 
@@ -317,47 +332,45 @@
 DEFAULT_URI = {
     "onebot": "/onebot",
     "keaimao": "/keaimao",
     "telegram": "/telegram",
 }
 
 
-ALL_AVAILABLE_BOT_PROTOCOLS: Iterable[T_BotProtocol] = ["onebot", "keaimao", "telegram"]
-ALL_AVAILABLE_ROUTE_MODES: Iterable[T_RouteMode] = ["group", "private", "channel"]
-
-
-class EventHandlerKwarg(BaseModel):
-    name: str
-    type_: Any
-    value: Any
-    """ 
-    value可以为嵌套协程，会自动await直到不可await，以获取结果 
-
-    也可以为函数，自动call到un callable，
-    
-    协程嵌套同步函数再嵌套协程也没有问题
-    """
-
-
-T_HandlerKwargMapping = Dict[str, List[EventHandlerKwarg]]
-
-
-def get_route_chinese(route_mode: T_RouteMode) -> str:
+def get_route_chinese(route_mode: T_ConversationType) -> str:
     if route_mode == "group":
         route_name = "群"
     elif route_mode == "private":
         route_name = "好友"
     else:
         route_name = "频道"
 
     return route_name
 
 
-def output_config():
+def filter_route_mapping(
+    protocol: Optional[T_BotProtocol] = None,
+    conversation_type: Optional[T_ConversationType] = None,
+    conversation_id: Optional[str] = None,
+    handler_type: Optional[T_HandlerType] = None,
+):
+    for p, ct, cid, ht in route_mapping.keys():
+        if protocol and p != protocol:
+            continue
+        if conversation_type and ct != conversation_type:
+            continue
+        if conversation_id and cid != conversation_id:
+            continue
+        if handler_type and ht != handler_type:
+            continue
+
+        yield (p, ct, cid, ht)
+
 
+def output_config():
     tree = Tree("协议适配")
 
     for protocol, api_caller in api_callers.items():
         caller_tree = tree.add(protocol)
         if protocol != "telegram":
             api_caller = cast(ApiCaller, api_caller)
 
@@ -366,65 +379,74 @@
             caller_tree.add(f"[green]API端口").add(str(api_caller.port))
         # else:
 
     rich_print(tree)
 
     tree = Tree("路由")
 
-    for protocol in ALL_AVAILABLE_BOT_PROTOCOLS:
+    for protocol in BOT_PROTOCOLS:
         protocol_tree = tree.add(protocol)
 
-        for route_mode in ALL_AVAILABLE_ROUTE_MODES:
-            route_name = get_route_chinese(route_mode)
+        for conversation_type in CONVERSATION_TYPES:
+            route_name = get_route_chinese(conversation_type)
 
-            global_commands = route_mapping.global_commands[protocol][route_mode]
+            (p, ct, cid, ht) = filter_route_mapping(
+                protocol=protocol,
+                conversation_type=conversation_type,
+                conversation_id="__global__",
+                handler_type="class_commands",
+            )
             if global_commands:
                 global_commands_tree = protocol_tree.add(f"全局{route_name}指令")
                 for command_name in global_commands:
                     global_commands_tree.add(command_name)
 
-            commands = route_mapping.mapping[protocol][route_mode]
+            commands = filter_route_mapping(
+                protocol=protocol,
+                conversation_type=conversation_type,
+                handler_type="class_commands",
+            )
             if commands:
                 commands_tree = None
 
                 for source_id, cache in commands.items():
                     if not cache["commands"]:
                         continue
                     if not commands_tree:
                         commands_tree = protocol_tree.add(f"指定来源{route_name}指令")
 
                     source_id_tree = commands_tree.add(source_id)
                     for command_name in cache["commands"]:
                         source_id_tree.add(command_name)
 
-            global_handlers = route_mapping.global_handlers[protocol][route_mode]
+            global_handlers = global_handlers[protocol][conversation_type]
             if global_handlers:
                 global_handlers_tree = protocol_tree.add(f"全局{route_name}响应器")
                 for handler_name in global_handlers:
                     global_handlers_tree.add(handler_name)
 
-            handlers = route_mapping.mapping[protocol][route_mode]
+            handlers = mapping[protocol][conversation_type]
             if handlers:
                 handlers_tree = None
 
                 for source_id, cache in handlers.items():
                     if not cache["class_handlers"]:
                         continue
 
                     if not handlers_tree:
                         handlers_tree = protocol_tree.add(f"指定来源{route_name}响应器")
 
                     source_id_tree = handlers_tree.add(source_id)
                     for handler_name in cache["class_handlers"]:
                         source_id_tree.add(handler_name)
 
-    for route_mode in ALL_AVAILABLE_ROUTE_MODES:
-        route_name = get_route_chinese(route_mode)
+    for conversation_type in CONVERSATION_TYPES:
+        route_name = get_route_chinese(conversation_type)
 
-        validators = route_mapping.mapping["validators"][route_mode]
+        validators = mapping["validators"][conversation_type]
         if not validators:
             continue
 
         validator_tree = tree.add("动态判断")
 
         for validator_name, cache in validators.items():
             if cache["commands"] or cache["class_handlers"]:
@@ -438,16 +460,7 @@
 
     rich_print(tree)
 
     # DisplayTree(
     #     name=f"事件",
     #     node=[method for method in groupCache.methods.keys()],
     # )
-
-
-class EventMeta(BaseModel):
-    protocol: T_BotProtocol
-    mode: T_RouteMode
-    source_id: str
-    raw_event: Dict
-    raw_event_name: str
-    protocol_event_name: str
```

### Comparing `pepperbot-0.3.3/pepperbot/utils/common.py` & `pepperbot-0.3.4/pepperbot/utils/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import asyncio
+import functools
 import inspect
 from inspect import isawaitable, iscoroutine
 from types import FunctionType
 from typing import Any, Callable, Coroutine, Dict, List, Union, cast
+from devtools import debug
 from pydantic import BaseModel
 
 
 class DictNoNone(dict):
     def __setitem__(self, key, value):
         if key in self or value is not None:
             dict.__setitem__(self, key, value)
@@ -14,46 +17,70 @@
 def get_current_function_name():
     return inspect.currentframe().f_back.f_code.co_name  # type:ignore
 
 
 def get_own_methods(instance: object):
     """从class上获取所有非__开头的方法"""
     for methodName in dir(instance):
-
         methodOrProperty = getattr(instance, methodName)
 
         if callable(methodOrProperty):
             if not methodName.startswith("__"):
                 yield cast(FunctionType, methodOrProperty)
 
 
 def get_own_attributes(instance: object):
+    """从class上获取所有非__开头的属性"""
+
     for property in dir(instance):
         if not property.startswith("__"):
             yield property
 
 
-async def await_or_sync(
-    functionOrCoroutine: Union[Any, FunctionType], *args, **kwargs
-) -> Any:
+async def await_or_sync(obj: Union[Any, FunctionType], *args, **kwargs) -> Any:
     """
     针对bound method，iscoroutine和isawaitable对bound method无效
 
     判断__func__也不行
     """
-    if callable(functionOrCoroutine):
-        result = functionOrCoroutine(*args, **kwargs)
-        # 针对bounded mothoud
-        if iscoroutine(result):
-            if result.__name__ == functionOrCoroutine.__name__:
-                result = await result
 
+    # while isinstance(obj, functools.partial):
+    #     obj = obj.func
+
+    if (
+        asyncio.iscoroutinefunction(obj)
+        or (callable(obj) and asyncio.iscoroutinefunction(obj.__call__))
+        # or iscoroutine(obj)
+        # or isawaitable(obj)
+    ):
+        # debug("coroutine")
+        result = await obj(*args, **kwargs)  # type: ignore
         return result
+    else:
+        if callable(obj):
+            # debug("sync")
+            result = await asyncio.to_thread(obj, *args, **kwargs)
+            # loop = asyncio.get_event_loop()
+            # with_kwargs = functools.partial(functionOrCoroutine, *args, **kwargs)
+
+            # result = await loop.run_in_executor(None, with_kwargs)
+            return result
+        else:
+            return None
 
-    return None
+    # if callable(functionOrCoroutine):
+    #     result = functionOrCoroutine(*args, **kwargs)
+    #     # 针对bounded mothoud
+    #     if iscoroutine(result):
+    #         if result.__name__ == functionOrCoroutine.__name__:
+    #             result = await result
+
+    #     return result
+
+    # return None
 
     # debug(functionOrCoroutine)
     # debug(dir(functionOrCoroutine))
     # debug(functionOrCoroutine.__func__)
     # debug(functionOrCoroutine.__name__)
     # debug(functionOrCoroutine.__call__)
     # debug(iscoroutine(functionOrCoroutine.__func__))
@@ -98,15 +125,16 @@
     刨除没有在函数中定义的，但是提供了的额外参数
 
     可以是lambda函数
 
     定义时是位置参数或者关键字参数都可以，因为位置参数也可以通过关键词参数的形式赋值
     """
     # validKwargNames = method.__annotations__.keys()
-    provided_arg_names = inspect.getargs(method.__code__)[0]
+    # provided_arg_names = inspect.getargs(method.__code__)[0]
+    provided_arg_names = inspect.signature(method).parameters
 
     fitted_args = {}
 
     for arg_name in kwargs.keys():
         if arg_name in provided_arg_names:
             fitted_args[arg_name] = kwargs[arg_name]
 
@@ -131,15 +159,14 @@
         print(tree.name)
 
     treeLength = len(tree.node)
     for index, node in enumerate(tree.node):
         newPrefixes = [*prefixes]
 
         if index == treeLength - 1:
-
             if isinstance(node, DisplayTree):
                 print("".join([*prefixes, lastBranch]), node.name)
 
                 newPrefixes.append(space)
             else:
                 newPrefixes.append(lastBranch)
```

### Comparing `pepperbot-0.3.3/pyproject.toml` & `pepperbot-0.3.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 ]
 classifiers = [
     "Programming Language :: Python",
 ]
 dependencies = [
     "Pyrogram>=2.0.102",
     "TgCrypto>=1.2.5",
+    "apscheduler>=3",
     "arrow>=1.2.3",
     "better-exceptions>=0.3.3",
     "devtools>=0.10.0",
     "httpx>=0.23.3",
     "loguru>=0.6.0",
-    "pydantic>=1.10.6",
+    "ormar[orjson,sqlite]>=0.12.1",
+    "pydantic>=1.10.4",
     "python-dotenv>=1.0.0",
     "rich>=13.3.2",
-    "sanic>=21.12.1",
-    "apscheduler>=3",
+    "sanic>=23",
 ]
 description = "An intuitive multi-platform bot framework, easily forward messages among platforms, support QQ, WeChat, Telegram. 一个符合直觉的跨社交平台机器人框架，轻松地在平台间传递消息，支持QQ、微信、Telegram"
 keywords = [
     "Telegram",
     "async",
     "asyncio",
     "bot",
@@ -38,15 +39,15 @@
     "type-annotations",
     "type-hint",
     "wechat",
 ]
 name = "pepperbot"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "0.3.3"
+version = "0.3.4"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 documentation = "https://SSmJaE.github.io/PepperBot"
 homepage = "https://github.com/SSmJaE/PepperBot"
```

### Comparing `pepperbot-0.3.3/tests/command/test_parse.py` & `pepperbot-0.3.4/tests/command/test_parse.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/tests/messageChain.py` & `pepperbot-0.3.4/tests/messageChain.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/tests/parse_pattern.py` & `pepperbot-0.3.4/tests/parse_pattern.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/tests/pattern.py` & `pepperbot-0.3.4/tests/pattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pydantic import Field
 
 
 BASE_DIR = path.dirname(path.dirname(path.abspath(__file__)))
 sys.path.append(BASE_DIR)
 
 
-from pepperbot.exceptions import PatternFormotError, PatternValidateError
+from pepperbot.exceptions import PatternFormatError, PatternValidateError
 from pepperbot.command import pattern
 from pepperbot.main import *
 from pydantic import validator
 
 mockEvent = {
     "message_id": 12345,
     "message": [],
@@ -61,24 +61,24 @@
 
     class Config:
         arbitrary_types_allowed = True
 
     @validator("装备数")
     def check_装备数(cls, value):
         if value not in [11, 12, 13]:
-            raise PatternFormotError("请输入有效序号")
+            raise PatternFormatError("请输入有效序号")
 
 
 class Order(BaseModel):
     order: int
 
     @validator("order")
     def check_order(cls, value):
         if value not in [11, 12, 13]:
-            raise PatternFormotError("请输入有效序号")
+            raise PatternFormatError("请输入有效序号")
 
 
 # create_model(
 #     "OrderModel",
 #     order=(int, ...),
 #     __validators__={"username_validator": validator("username")(username_alphanumeric)},
 # )
```

### Comparing `pepperbot-0.3.3/tests/response/fake_server.py` & `pepperbot-0.3.4/tests/response/fake_server.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/tests/response/poke.py` & `pepperbot-0.3.4/tests/response/poke.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/tests/tree.py` & `pepperbot-0.3.4/tests/tree.py`

 * *Files identical despite different names*

### Comparing `pepperbot-0.3.3/PKG-INFO` & `pepperbot-0.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 Metadata-Version: 2.1
 Name: pepperbot
-Version: 0.3.3
+Version: 0.3.4
 Summary: An intuitive multi-platform bot framework, easily forward messages among platforms, support QQ, WeChat, Telegram. 一个符合直觉的跨社交平台机器人框架，轻松地在平台间传递消息，支持QQ、微信、Telegram
 Keywords: Telegram async asyncio bot chinese cqhttp cross-platform framework keaimao onebot pydantic pyrogram python qq type-annotations type-hint wechat
 Home-page: https://github.com/SSmJaE/PepperBot
 Author-Email: SSmJaE <ssmjae327@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python
 Project-URL: Documentation, https://SSmJaE.github.io/PepperBot
 Project-URL: Homepage, https://github.com/SSmJaE/PepperBot
 Project-URL: Repository, https://github.com/SSmJaE/PepperBot
 Requires-Python: >=3.10
 Requires-Dist: Pyrogram>=2.0.102
 Requires-Dist: TgCrypto>=1.2.5
+Requires-Dist: apscheduler>=3
 Requires-Dist: arrow>=1.2.3
 Requires-Dist: better-exceptions>=0.3.3
 Requires-Dist: devtools>=0.10.0
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: loguru>=0.6.0
-Requires-Dist: pydantic>=1.10.6
+Requires-Dist: ormar[orjson,sqlite]>=0.12.1
+Requires-Dist: pydantic>=1.10.4
 Requires-Dist: python-dotenv>=1.0.0
 Requires-Dist: rich>=13.3.2
-Requires-Dist: sanic>=21.12.1
-Requires-Dist: apscheduler>=3
+Requires-Dist: sanic>=23
 Description-Content-Type: text/markdown
 
 <h1 align="center">PepperBot</h1>
 
 <p align="center">
-<img  src="./archive/icon.png" width="200">
+<img  src="./archive/icon.png" width="200" />
 </p>
 
 <p align="center">一个符合直觉的跨社交平台机器人框架，轻松地在平台间传递消息，支持QQ、微信、Telegram</p>
 <p align="center">
 <a href="https://ssmjae.github.io/PepperBot/">文档</a> ·
 <a href="https://jq.qq.com/?_wv=1027&k=EPhcRRib">QQ交流群</a>  
-<!-- <a href="https://jq.qq.com/?_wv=1027&k=EPhcRRib">微信交流群</a> · 
-<a href="https://jq.qq.com/?_wv=1027&k=EPhcRRib">TG交流群</a>  -->
 </p>
 
 <p align="center">
 <img src="./archive/coverage-badge.svg" />
 </p>
 
 ## 生而跨平台
@@ -134,7 +133,9 @@
             # 发送一条群消息
             # 接受任意个参数，必须是合法的消息片段，比如Text，Face，Image
             await bot.group_message(
                 Text("没人"),
                 Image("http://123.jpg"),
             )
 ```
+
+## 生态
```

